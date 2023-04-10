# Comparing `tmp/onnx2tf-1.9.0.tar.gz` & `tmp/onnx2tf-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2tf-1.9.0.tar", last modified: Sun Apr  9 13:40:15 2023, max compression
+gzip compressed data, was "onnx2tf-1.9.1.tar", last modified: Mon Apr 10 09:45:48 2023, max compression
```

## Comparing `onnx2tf-1.9.0.tar` & `onnx2tf-1.9.1.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:40:15.855645 onnx2tf-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/LICENSE_onnx-tensorflow
--rw-r--r--   0 runner    (1001) docker     (123)   100778 2023-04-09 13:40:15.851645 onnx2tf-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   100236 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:40:15.831645 onnx2tf-1.9.0/onnx2tf/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96451 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/onnx2tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:40:15.851645 onnx2tf-1.9.0/onnx2tf/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Abs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Acos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Acosh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/And.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ArgMax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ArgMin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Asin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Asinh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Atan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Atanh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/AveragePool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/BatchNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Bernoulli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/BitShift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Celu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ConcatFromSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ConstantOfShape.py
--rw-r--r--   0 runner    (1001) docker     (123)    37236 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ConvTranspose.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Cos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Cosh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/CumSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/DepthToSpace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/DequantizeLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Det.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Div.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/DynamicQuantizeLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Einsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Elu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Equal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Erf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/EyeLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Floor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/FusedConv.py
--rw-r--r--   0 runner    (1001) docker     (123)    33062 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/GRU.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/GatherElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/GatherND.py
--rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Gemm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/GlobalAveragePool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/GlobalLpPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/GlobalMaxPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Greater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/GreaterOrEqual.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/GridSample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/HardSigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/HardSwish.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Hardmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/If.py
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/InstanceNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/IsInf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/IsNaN.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/LRN.py
--rw-r--r--   0 runner    (1001) docker     (123)    43088 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/LayerNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/LeakyRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Less.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/LessOrEqual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/LogSoftmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/LpNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/MatMul.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/MatMulInteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Max.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/MaxPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/MaxUnpool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/MeanVarianceNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Min.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Mul.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Multinomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Neg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/NonMaxSuppression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/NonZero.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Not.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/OneHot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Or.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/PRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Pow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/QLinearAdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/QLinearConcat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/QLinearConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/QLinearLeakyRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/QLinearMatMul.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/QLinearMul.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/QLinearSigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/QLinearSoftmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/QuantizeLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    27652 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/RNN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/RandomNormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/RandomNormalLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/RandomUniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/RandomUniformLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Reciprocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceL1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceL2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceLogSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceLogSumExp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceMax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceMean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceMin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceProd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReduceSumSquare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Relu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    25352 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ReverseSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/RoiAlign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Round.py
--rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ScaleAndTranslate.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ScatterElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ScatterND.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Selu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/SequenceAt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/SequenceConstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/SequenceEmpty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/SequenceErase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/SequenceInsert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/SequenceLength.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Shrink.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Sin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Sinh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Size.py
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Softplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Softsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/SpaceToDepth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/SplitToSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Sqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Squeeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Tan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/ThresholdedRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/TopK.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Trilu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Unique.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Unsqueeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Where.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/Xor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/_Loop.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:40:15.851645 onnx2tf-1.9.0/onnx2tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)   199853 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/utils/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/onnx2tf/utils/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:40:15.831645 onnx2tf-1.9.0/onnx2tf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)   100778 2023-04-09 13:40:15.000000 onnx2tf-1.9.0/onnx2tf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-09 13:40:15.000000 onnx2tf-1.9.0/onnx2tf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:40:15.000000 onnx2tf-1.9.0/onnx2tf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-09 13:40:15.000000 onnx2tf-1.9.0/onnx2tf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 13:40:15.000000 onnx2tf-1.9.0/onnx2tf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:40:15.855645 onnx2tf-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:40:15.851645 onnx2tf-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-09 13:40:09.000000 onnx2tf-1.9.0/tests/test_model_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:45:48.207406 onnx2tf-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/LICENSE_onnx-tensorflow
+-rw-r--r--   0 runner    (1001) docker     (123)   104575 2023-04-10 09:45:48.207406 onnx2tf-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   104033 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:45:48.183406 onnx2tf-1.9.1/onnx2tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96544 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/onnx2tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:45:48.207406 onnx2tf-1.9.1/onnx2tf/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Abs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Acos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Acosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/And.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ArgMax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ArgMin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Asin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Asinh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Atan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Atanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/AveragePool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/BatchNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Bernoulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/BitShift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Celu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ConcatFromSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ConstantOfShape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37236 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ConvTranspose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Cos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Cosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/CumSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/DepthToSpace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/DequantizeLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Det.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Div.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/DynamicQuantizeLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Einsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Elu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Erf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/EyeLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/FusedConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/GRU.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/GatherElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/GatherND.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Gemm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/GlobalAveragePool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/GlobalLpPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/GlobalMaxPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Greater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/GreaterOrEqual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/GridSample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/HardSigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/HardSwish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Hardmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/If.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/InstanceNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/IsInf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/IsNaN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/LRN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43088 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/LayerNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/LeakyRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Less.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/LessOrEqual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/LogSoftmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/LpNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/MatMul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/MatMulInteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Max.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/MaxPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/MaxUnpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/MeanVarianceNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Mul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Multinomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/NonMaxSuppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/NonZero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Not.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/OneHot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Or.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/PRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Pow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/QLinearAdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/QLinearConcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/QLinearConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/QLinearLeakyRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/QLinearMatMul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/QLinearMul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/QLinearSigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/QLinearSoftmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/QuantizeLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27652 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/RNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/RandomNormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/RandomNormalLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/RandomUniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/RandomUniformLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceL1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceL2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceLogSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceLogSumExp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceMax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceMean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceMin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceProd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReduceSumSquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25352 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ReverseSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/RoiAlign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Round.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ScaleAndTranslate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ScatterElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ScatterND.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Selu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/SequenceAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/SequenceConstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/SequenceEmpty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/SequenceErase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/SequenceInsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/SequenceLength.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Shrink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Sin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Sinh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Softplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Softsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/SpaceToDepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/SplitToSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Tan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/ThresholdedRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/TopK.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Trilu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/Xor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/_Loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:45:48.207406 onnx2tf-1.9.1/onnx2tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199853 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/utils/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/onnx2tf/utils/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:45:48.183406 onnx2tf-1.9.1/onnx2tf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)   104575 2023-04-10 09:45:48.000000 onnx2tf-1.9.1/onnx2tf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-10 09:45:48.000000 onnx2tf-1.9.1/onnx2tf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:45:48.000000 onnx2tf-1.9.1/onnx2tf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 09:45:48.000000 onnx2tf-1.9.1/onnx2tf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 09:45:48.000000 onnx2tf-1.9.1/onnx2tf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 09:45:48.207406 onnx2tf-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:45:48.207406 onnx2tf-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-10 09:45:39.000000 onnx2tf-1.9.1/tests/test_model_convert.py
```

### Comparing `onnx2tf-1.9.0/LICENSE` & `onnx2tf-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/LICENSE_onnx-tensorflow` & `onnx2tf-1.9.1/LICENSE_onnx-tensorflow`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/PKG-INFO` & `onnx2tf-1.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: onnx2tf
-Version: 1.9.0
-Summary: Self-Created Tools to convert ONNX files (NCHW) to TensorFlow/TFLite/Keras format (NHWC). The purpose of this tool is to solve the massive Transpose extrapolation problem in onnx-tensorflow (onnx-tf).
-Home-page: https://github.com/PINTO0309/onnx2tf
-Author: Katsuya Hyodo
-Author-email: rmsdh122@yahoo.co.jp
-License: MIT License
-Platform: linux
-Platform: unix
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE_onnx-tensorflow
-
 # onnx2tf
 Self-Created Tools to convert ONNX files (NCHW) to TensorFlow/TFLite/Keras format (NHWC). The purpose of this tool is to solve the massive Transpose extrapolation problem in [onnx-tensorflow](https://github.com/onnx/onnx-tensorflow) ([onnx-tf](https://pypi.org/project/onnx-tf/)). I don't need a Star, but give me a pull request. Since I am adding challenging model optimizations and fixing bugs almost daily, I frequently embed potential bugs that would otherwise break through CI's regression testing. Therefore, if you encounter new problems, I recommend that you try a package that is a few versions older, or try the latest package that will be released in a few days.
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/33194443/193840307-fa69eace-05a9-4d93-9c5d-999cf88af28e.png" />
 </p>
 
@@ -252,15 +237,15 @@
 ## Sample Usage
 ### 1. Install
 - HostPC
   ```
   $ docker run --rm -it \
   -v `pwd`:/workdir \
   -w /workdir \
-  ghcr.io/pinto0309/onnx2tf:1.9.0
+  ghcr.io/pinto0309/onnx2tf:1.9.1
 
   or
 
   $ pip install -U onnx \
   && pip install -U nvidia-pyindex \
   && pip install -U onnx-graphsurgeon \
   && pip install -U onnxruntime==1.13.1 \
@@ -528,15 +513,15 @@
 
     |Before|After|
     |:-:|:-:|
     |`HardSwish`<br>![image](https://user-images.githubusercontent.com/33194443/226223099-c7344bcf-d24d-4b35-a1d6-2a03dbfce8c7.png)|`ReLU`<br>![image](https://user-images.githubusercontent.com/33194443/226223213-bd714994-f353-416e-9f54-6d0954a70bb8.png)|
 
 
 ### 7. Calibration data creation for INT8 quantization
-Calibration data (.npy) for INT8 quantization (`-qcind`) is generated as follows. This is a sample when the data used for training is image data. See: https://github.com/PINTO0309/onnx2tf/issues/222
+Calibration data (.npy) for INT8 quantization (`-cind`) is generated as follows. This is a sample when the data used for training is image data. See: https://github.com/PINTO0309/onnx2tf/issues/222
 
 https://www.tensorflow.org/lite/performance/post_training_quantization
 
 ```python
 import cv2
 import glob
 import numpy as np
@@ -563,20 +548,20 @@
 print(f'calib_datas.shape: {calib_datas.shape}') # [10,112,200,3]
 np.save(file='data/calibdata.npy', arr=calib_datas)
 
 loaded_data = np.load('data/calibdata.npy')
 print(f'loaded_data.shape: {loaded_data.shape}') # [10,112,200,3]
 
 """
--qcind INPUT_NAME NUMPY_FILE_PATH MEAN STD
+-cind INPUT_NAME NUMPY_FILE_PATH MEAN STD
 int8_calib_datas = (loaded_data - MEAN) / STD # -1.0 - 1.0
 
 e.g.
--qcind pc_dep 'data/calibdata.npy' [[[[0.485, 0.456, 0.406]]]] [[[[0.229, 0.224, 0.225]]]]
--qcind feat 'data/calibdata2.npy' [[[[0.123, ..., 0.321]]]] [[[[0.112, ..., 0.451]]]]
+-cind pc_dep 'data/calibdata.npy' [[[[0.485, 0.456, 0.406]]]] [[[[0.229, 0.224, 0.225]]]]
+-cind feat 'data/calibdata2.npy' [[[[0.123, ..., 0.321]]]] [[[[0.112, ..., 0.451]]]]
 """
 ```
 
 ### 8. INT8 quantization of models with multiple inputs requiring non-image data
 If you do not need to perform INT8 quantization with this tool alone, the following method is the easiest.
 
 The `-osd` option will output a `saved_model.pb` in the `saved_model` folder with the full size required for quantization. That is, a default signature named `serving_default` is embedded in `.pb`. The `-b` option is used to convert the batch size by rewriting it as a static integer.
@@ -652,15 +637,52 @@
 
 ![image](https://user-images.githubusercontent.com/33194443/225174599-e62173f3-1dd2-48f4-a762-f15ef78cd01e.png)
 
 https://www.tensorflow.org/lite/performance/post_training_quantization
 
 See: https://github.com/PINTO0309/onnx2tf/issues/248
 
-### 9. Conversion to TensorFlow.js
+### 9. Fixing the output of NonMaxSuppression (NMS)
+PyTorch's `NonMaxSuppression (torchvision.ops.nms)` and ONNX's `NonMaxSuppression` are not fully compatible. TorchVision's NMS is very inefficient. Therefore, it is inevitable that converting ONNX using NMS in object detection models and other models will be very redundant and will be converted with a structure that is difficult for TensorFlow.js and TFLite models to take advantage of in devices. This is due to the indefinite number of tensors output by the NMS. In this chapter, I share how to easily tune the ONNX generated using TorchVision's redundant NMS to generate an optimized NMS.
+
+1. There are multiple issues with TorchVision's NMS. First, the batch size specification is not supported; second, the `max_output_boxes_per_class` parameter cannot be specified. Please see the NMS sample ONNX part I generated. The `max_output_boxes_per_class` has been changed to `896` instead of `-Infinity`. The biggest problem with TorchVision NMS is that it generates ONNX with `max_output_boxes_per_class` set to `-Infinity` or `9223372036854775807 (Maximum value of INT64)`, resulting in a variable number of NMS outputs from zero to infinite. Thus, by rewriting `-Infinity` or `9223372036854775807 (Maximum value of INT64)` to a constant value, it is possible to output an NMS that can be effortlessly inferred by TFJS or TFLite.
+![image](https://user-images.githubusercontent.com/33194443/230778827-faab8ffe-d49f-498d-b414-a1a26848a380.png)
+
+    Here you will find committed ONNX components optimized for various devices.
+    https://github.com/PINTO0309/components_of_onnx/tree/main/components_of_onnx/ops
+
+2. In the following example, the `max_output_boxes_per_class` of NMS in the post-processing generated by YOLOv7 is changed from `-Infinity` or `9223372036854775807 (Maximum value of INT64)` to `20`, as shown in the figure below. The name `main01_max_output_boxes_per_class` has been rewritten by me for clarity, but it originally appears as `max_output_boxes_per_class`.
+![image](https://user-images.githubusercontent.com/33194443/230779419-23cc017f-fde9-4777-bb3d-766a35a09efd.png)
+
+    Simply execute the following command. The command rewrites the specified attribute value of the OP specified by ONNX.
+    ```bash
+    pip install sam4onnx
+
+    sam4onnx \
+    --op_name main01_nonmaxsuppression11 \
+    --input_onnx_file_path yolov7.onnx \
+    --output_onnx_file_path nms_yolov7_update.onnx \
+    --input_constants main01_max_output_boxes_per_class int64 [20]
+    ```
+    A tutorial on one of my ONNX modification tools, `sam4onnx`, can be found here.
+
+    https://github.com/PINTO0309/sam4onnx
+
+    Many detailed tutorials are provided below, so if you are interested, please play with them.
+
+    https://github.com/PINTO0309/PINTO_model_zoo/tree/main/307_YOLOv7/post_process_gen_tools
+
+3. Finally, simply convert ONNX to TFLite or saved_model or TFJS using onnx2tf. onnx2tf performs an internal operation to automatically optimize the NMS output to a fixed shape if `max_output_boxes_per_class` is set to a value other than `-Infinity` and `9223372036854775807 (Maximum value of INT64)`. Specify `--output_nms_with_dynamic_tensor` or `-onwdt` if you do not want to optimize for a fixed shape.
+    ```
+    onnx2tf -i nms_yolov7_update.onnx -osd -cotof
+    ```
+    I would be happy if this is a reference for Android + Java or TFJS implementations. There are tons more tricky model optimization techniques described in my blog posts, so you'll have to find them yourself. I don't dare to list the URL here because it is annoying to see so many `issues` being posted. And unfortunately, all articles are in Japanese.
+    ![image](https://user-images.githubusercontent.com/33194443/230780749-9967a34b-abf6-47fe-827d-92e0f6bddf46.png)
+
+### 10. Conversion to TensorFlow.js
 When converting to TensorFlow.js, process as follows.
 
 ```bash
 pip install tensorflowjs
 
 onnx2tf -i mobilenetv2-12.onnx -ois input:1,3,224,224 -osd
 
@@ -671,15 +693,15 @@
 tfjs_model
 ```
 
 See: https://github.com/tensorflow/tfjs/tree/master/tfjs-converter
 
 ![image](https://user-images.githubusercontent.com/33194443/224186149-0b9ce9dc-fe09-48d4-b430-6cc3d0687140.png)
 
-### 10. Conversion to CoreML
+### 11. Conversion to CoreML
 When converting to CoreML, process as follows. The `-k` option is for conversion while maintaining the input channel order in ONNX's NCHW format.
 
 ```bash
 pip install coremltools
 
 onnx2tf -i mobilenetv2-12.onnx -k input -ois input:1,3,224,224 -osd
 ```
```

### Comparing `onnx2tf-1.9.0/README.md` & `onnx2tf-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: onnx2tf
+Version: 1.9.1
+Summary: Self-Created Tools to convert ONNX files (NCHW) to TensorFlow/TFLite/Keras format (NHWC). The purpose of this tool is to solve the massive Transpose extrapolation problem in onnx-tensorflow (onnx-tf).
+Home-page: https://github.com/PINTO0309/onnx2tf
+Author: Katsuya Hyodo
+Author-email: rmsdh122@yahoo.co.jp
+License: MIT License
+Platform: linux
+Platform: unix
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_onnx-tensorflow
+
 # onnx2tf
 Self-Created Tools to convert ONNX files (NCHW) to TensorFlow/TFLite/Keras format (NHWC). The purpose of this tool is to solve the massive Transpose extrapolation problem in [onnx-tensorflow](https://github.com/onnx/onnx-tensorflow) ([onnx-tf](https://pypi.org/project/onnx-tf/)). I don't need a Star, but give me a pull request. Since I am adding challenging model optimizations and fixing bugs almost daily, I frequently embed potential bugs that would otherwise break through CI's regression testing. Therefore, if you encounter new problems, I recommend that you try a package that is a few versions older, or try the latest package that will be released in a few days.
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/33194443/193840307-fa69eace-05a9-4d93-9c5d-999cf88af28e.png" />
 </p>
 
@@ -237,15 +252,15 @@
 ## Sample Usage
 ### 1. Install
 - HostPC
   ```
   $ docker run --rm -it \
   -v `pwd`:/workdir \
   -w /workdir \
-  ghcr.io/pinto0309/onnx2tf:1.9.0
+  ghcr.io/pinto0309/onnx2tf:1.9.1
 
   or
 
   $ pip install -U onnx \
   && pip install -U nvidia-pyindex \
   && pip install -U onnx-graphsurgeon \
   && pip install -U onnxruntime==1.13.1 \
@@ -513,15 +528,15 @@
 
     |Before|After|
     |:-:|:-:|
     |`HardSwish`<br>![image](https://user-images.githubusercontent.com/33194443/226223099-c7344bcf-d24d-4b35-a1d6-2a03dbfce8c7.png)|`ReLU`<br>![image](https://user-images.githubusercontent.com/33194443/226223213-bd714994-f353-416e-9f54-6d0954a70bb8.png)|
 
 
 ### 7. Calibration data creation for INT8 quantization
-Calibration data (.npy) for INT8 quantization (`-qcind`) is generated as follows. This is a sample when the data used for training is image data. See: https://github.com/PINTO0309/onnx2tf/issues/222
+Calibration data (.npy) for INT8 quantization (`-cind`) is generated as follows. This is a sample when the data used for training is image data. See: https://github.com/PINTO0309/onnx2tf/issues/222
 
 https://www.tensorflow.org/lite/performance/post_training_quantization
 
 ```python
 import cv2
 import glob
 import numpy as np
@@ -548,20 +563,20 @@
 print(f'calib_datas.shape: {calib_datas.shape}') # [10,112,200,3]
 np.save(file='data/calibdata.npy', arr=calib_datas)
 
 loaded_data = np.load('data/calibdata.npy')
 print(f'loaded_data.shape: {loaded_data.shape}') # [10,112,200,3]
 
 """
--qcind INPUT_NAME NUMPY_FILE_PATH MEAN STD
+-cind INPUT_NAME NUMPY_FILE_PATH MEAN STD
 int8_calib_datas = (loaded_data - MEAN) / STD # -1.0 - 1.0
 
 e.g.
--qcind pc_dep 'data/calibdata.npy' [[[[0.485, 0.456, 0.406]]]] [[[[0.229, 0.224, 0.225]]]]
--qcind feat 'data/calibdata2.npy' [[[[0.123, ..., 0.321]]]] [[[[0.112, ..., 0.451]]]]
+-cind pc_dep 'data/calibdata.npy' [[[[0.485, 0.456, 0.406]]]] [[[[0.229, 0.224, 0.225]]]]
+-cind feat 'data/calibdata2.npy' [[[[0.123, ..., 0.321]]]] [[[[0.112, ..., 0.451]]]]
 """
 ```
 
 ### 8. INT8 quantization of models with multiple inputs requiring non-image data
 If you do not need to perform INT8 quantization with this tool alone, the following method is the easiest.
 
 The `-osd` option will output a `saved_model.pb` in the `saved_model` folder with the full size required for quantization. That is, a default signature named `serving_default` is embedded in `.pb`. The `-b` option is used to convert the batch size by rewriting it as a static integer.
@@ -637,15 +652,52 @@
 
 ![image](https://user-images.githubusercontent.com/33194443/225174599-e62173f3-1dd2-48f4-a762-f15ef78cd01e.png)
 
 https://www.tensorflow.org/lite/performance/post_training_quantization
 
 See: https://github.com/PINTO0309/onnx2tf/issues/248
 
-### 9. Conversion to TensorFlow.js
+### 9. Fixing the output of NonMaxSuppression (NMS)
+PyTorch's `NonMaxSuppression (torchvision.ops.nms)` and ONNX's `NonMaxSuppression` are not fully compatible. TorchVision's NMS is very inefficient. Therefore, it is inevitable that converting ONNX using NMS in object detection models and other models will be very redundant and will be converted with a structure that is difficult for TensorFlow.js and TFLite models to take advantage of in devices. This is due to the indefinite number of tensors output by the NMS. In this chapter, I share how to easily tune the ONNX generated using TorchVision's redundant NMS to generate an optimized NMS.
+
+1. There are multiple issues with TorchVision's NMS. First, the batch size specification is not supported; second, the `max_output_boxes_per_class` parameter cannot be specified. Please see the NMS sample ONNX part I generated. The `max_output_boxes_per_class` has been changed to `896` instead of `-Infinity`. The biggest problem with TorchVision NMS is that it generates ONNX with `max_output_boxes_per_class` set to `-Infinity` or `9223372036854775807 (Maximum value of INT64)`, resulting in a variable number of NMS outputs from zero to infinite. Thus, by rewriting `-Infinity` or `9223372036854775807 (Maximum value of INT64)` to a constant value, it is possible to output an NMS that can be effortlessly inferred by TFJS or TFLite.
+![image](https://user-images.githubusercontent.com/33194443/230778827-faab8ffe-d49f-498d-b414-a1a26848a380.png)
+
+    Here you will find committed ONNX components optimized for various devices.
+    https://github.com/PINTO0309/components_of_onnx/tree/main/components_of_onnx/ops
+
+2. In the following example, the `max_output_boxes_per_class` of NMS in the post-processing generated by YOLOv7 is changed from `-Infinity` or `9223372036854775807 (Maximum value of INT64)` to `20`, as shown in the figure below. The name `main01_max_output_boxes_per_class` has been rewritten by me for clarity, but it originally appears as `max_output_boxes_per_class`.
+![image](https://user-images.githubusercontent.com/33194443/230779419-23cc017f-fde9-4777-bb3d-766a35a09efd.png)
+
+    Simply execute the following command. The command rewrites the specified attribute value of the OP specified by ONNX.
+    ```bash
+    pip install sam4onnx
+
+    sam4onnx \
+    --op_name main01_nonmaxsuppression11 \
+    --input_onnx_file_path yolov7.onnx \
+    --output_onnx_file_path nms_yolov7_update.onnx \
+    --input_constants main01_max_output_boxes_per_class int64 [20]
+    ```
+    A tutorial on one of my ONNX modification tools, `sam4onnx`, can be found here.
+
+    https://github.com/PINTO0309/sam4onnx
+
+    Many detailed tutorials are provided below, so if you are interested, please play with them.
+
+    https://github.com/PINTO0309/PINTO_model_zoo/tree/main/307_YOLOv7/post_process_gen_tools
+
+3. Finally, simply convert ONNX to TFLite or saved_model or TFJS using onnx2tf. onnx2tf performs an internal operation to automatically optimize the NMS output to a fixed shape if `max_output_boxes_per_class` is set to a value other than `-Infinity` and `9223372036854775807 (Maximum value of INT64)`. Specify `--output_nms_with_dynamic_tensor` or `-onwdt` if you do not want to optimize for a fixed shape.
+    ```
+    onnx2tf -i nms_yolov7_update.onnx -osd -cotof
+    ```
+    I would be happy if this is a reference for Android + Java or TFJS implementations. There are tons more tricky model optimization techniques described in my blog posts, so you'll have to find them yourself. I don't dare to list the URL here because it is annoying to see so many `issues` being posted. And unfortunately, all articles are in Japanese.
+    ![image](https://user-images.githubusercontent.com/33194443/230780749-9967a34b-abf6-47fe-827d-92e0f6bddf46.png)
+
+### 10. Conversion to TensorFlow.js
 When converting to TensorFlow.js, process as follows.
 
 ```bash
 pip install tensorflowjs
 
 onnx2tf -i mobilenetv2-12.onnx -ois input:1,3,224,224 -osd
 
@@ -656,15 +708,15 @@
 tfjs_model
 ```
 
 See: https://github.com/tensorflow/tfjs/tree/master/tfjs-converter
 
 ![image](https://user-images.githubusercontent.com/33194443/224186149-0b9ce9dc-fe09-48d4-b430-6cc3d0687140.png)
 
-### 10. Conversion to CoreML
+### 11. Conversion to CoreML
 When converting to CoreML, process as follows. The `-k` option is for conversion while maintaining the input channel order in ONNX's NCHW format.
 
 ```bash
 pip install coremltools
 
 onnx2tf -i mobilenetv2-12.onnx -k input -ois input:1,3,224,224 -osd
 ```
```

### Comparing `onnx2tf-1.9.0/onnx2tf/onnx2tf.py` & `onnx2tf-1.9.1/onnx2tf/onnx2tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
                 std:  [1,1,1,3] -> [[[[0.229, 0.224, 0.225]]]]\n
             input1: [n,64,64]\n
                 mean: [1,64] -> [0.1, ..., 0.64]\n
                 std:  [1,64] -> [0.05, ..., 0.08]\n
             input2: [n,5]\n
                 mean: [1] -> [0.3]\n
                 std:  [1] -> [0.07]\n
-        qcind=[
+        cind=[
             ["input0","../input0.npy",[[[[0.485, 0.456, 0.406]]]],[[[[0.229, 0.224, 0.225]]]]],\n
             ["input1","./input1.npy",[0.1, ..., 0.64],[0.05, ..., 0.08]],\n
             ["input2","input2.npy",[0.3],[0.07]],\n
         ]
 
     input_output_quant_dtype: Optional[str]
         Input and Output dtypes when doing Full INT8 Quantization.\n
@@ -2007,21 +2007,23 @@
     if args.custom_input_op_name_np_data_path is not None:
         for param in args.custom_input_op_name_np_data_path:
             tmp = []
             if len(param) == 2:
                 tmp.append(str(param[0])) # input_op_name
                 tmp.append(str(param[1])) # numpy_file_path
 
-                if len(param) == 4:
-                    tmp.append(np.asarray(ast.literal_eval(param[2]), dtype=np.float32)) # mean
-                    tmp.append(np.asarray(ast.literal_eval(param[3]), dtype=np.float32)) # std
+            if len(param) == 4:
+                tmp.append(str(param[0])) # input_op_name
+                tmp.append(str(param[1])) # numpy_file_path
+                tmp.append(np.asarray(ast.literal_eval(param[2]), dtype=np.float32)) # mean
+                tmp.append(np.asarray(ast.literal_eval(param[3]), dtype=np.float32)) # std
 
-                custom_params.append(
-                    tmp
-                )
+            custom_params.append(
+                tmp
+            )
 
     if len(custom_params) == 0:
         custom_params = None
 
     args.replace_to_pseudo_operators = [
         name.lower() for name in args.replace_to_pseudo_operators
     ]
```

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Abs.py` & `onnx2tf-1.9.1/onnx2tf/ops/Abs.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Acos.py` & `onnx2tf-1.9.1/onnx2tf/ops/Acos.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Acosh.py` & `onnx2tf-1.9.1/onnx2tf/ops/Acosh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Add.py` & `onnx2tf-1.9.1/onnx2tf/ops/Add.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/And.py` & `onnx2tf-1.9.1/onnx2tf/ops/And.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ArgMax.py` & `onnx2tf-1.9.1/onnx2tf/ops/ArgMax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ArgMin.py` & `onnx2tf-1.9.1/onnx2tf/ops/ArgMin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Asin.py` & `onnx2tf-1.9.1/onnx2tf/ops/Asin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Asinh.py` & `onnx2tf-1.9.1/onnx2tf/ops/Asinh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Atan.py` & `onnx2tf-1.9.1/onnx2tf/ops/Atan.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Atanh.py` & `onnx2tf-1.9.1/onnx2tf/ops/Atanh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/AveragePool.py` & `onnx2tf-1.9.1/onnx2tf/ops/AveragePool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/BatchNormalization.py` & `onnx2tf-1.9.1/onnx2tf/ops/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Bernoulli.py` & `onnx2tf-1.9.1/onnx2tf/ops/Bernoulli.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/BitShift.py` & `onnx2tf-1.9.1/onnx2tf/ops/BitShift.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Cast.py` & `onnx2tf-1.9.1/onnx2tf/ops/Cast.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Ceil.py` & `onnx2tf-1.9.1/onnx2tf/ops/Ceil.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Celu.py` & `onnx2tf-1.9.1/onnx2tf/ops/Celu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Clip.py` & `onnx2tf-1.9.1/onnx2tf/ops/Clip.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Compress.py` & `onnx2tf-1.9.1/onnx2tf/ops/Compress.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Concat.py` & `onnx2tf-1.9.1/onnx2tf/ops/Concat.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ConcatFromSequence.py` & `onnx2tf-1.9.1/onnx2tf/ops/ConcatFromSequence.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Constant.py` & `onnx2tf-1.9.1/onnx2tf/ops/Constant.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ConstantOfShape.py` & `onnx2tf-1.9.1/onnx2tf/ops/ConstantOfShape.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Conv.py` & `onnx2tf-1.9.1/onnx2tf/ops/Conv.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ConvTranspose.py` & `onnx2tf-1.9.1/onnx2tf/ops/ConvTranspose.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Cos.py` & `onnx2tf-1.9.1/onnx2tf/ops/Cos.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Cosh.py` & `onnx2tf-1.9.1/onnx2tf/ops/Cosh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/CumSum.py` & `onnx2tf-1.9.1/onnx2tf/ops/CumSum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/DepthToSpace.py` & `onnx2tf-1.9.1/onnx2tf/ops/DepthToSpace.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/DequantizeLinear.py` & `onnx2tf-1.9.1/onnx2tf/ops/DequantizeLinear.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Det.py` & `onnx2tf-1.9.1/onnx2tf/ops/Det.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Div.py` & `onnx2tf-1.9.1/onnx2tf/ops/Div.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Dropout.py` & `onnx2tf-1.9.1/onnx2tf/ops/Dropout.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/DynamicQuantizeLinear.py` & `onnx2tf-1.9.1/onnx2tf/ops/DynamicQuantizeLinear.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Einsum.py` & `onnx2tf-1.9.1/onnx2tf/ops/Einsum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Elu.py` & `onnx2tf-1.9.1/onnx2tf/ops/Elu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Equal.py` & `onnx2tf-1.9.1/onnx2tf/ops/Equal.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Erf.py` & `onnx2tf-1.9.1/onnx2tf/ops/Erf.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Exp.py` & `onnx2tf-1.9.1/onnx2tf/ops/Exp.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Expand.py` & `onnx2tf-1.9.1/onnx2tf/ops/Expand.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/EyeLike.py` & `onnx2tf-1.9.1/onnx2tf/ops/EyeLike.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Flatten.py` & `onnx2tf-1.9.1/onnx2tf/ops/Flatten.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Floor.py` & `onnx2tf-1.9.1/onnx2tf/ops/Floor.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/FusedConv.py` & `onnx2tf-1.9.1/onnx2tf/ops/FusedConv.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/GRU.py` & `onnx2tf-1.9.1/onnx2tf/ops/GRU.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,16 +163,14 @@
         w_br,
         w_bh,
 
         r_bz,
         r_br,
         r_bh,
 
-        activation_alphas,
-        activation_betas,
         activations,
 
         clip,
         linear_before_reset,
         is_bidirectional,
         go_backwards,
         **kwargs
@@ -192,16 +190,14 @@
         self.w_br=w_br
         self.w_bh=w_bh
 
         self.r_bz=r_bz
         self.r_br=r_br
         self.r_bh=r_bh
 
-        self.activation_alphas = activation_alphas
-        self.activation_betas = activation_betas
         self.activations = activations
 
         self.clip = clip
         self.linear_before_reset = linear_before_reset
         self.is_bidirectional = is_bidirectional
         self.go_backwards = go_backwards
 
@@ -228,15 +224,15 @@
         z = tf.matmul(inputs, tf.transpose(self.w_z)) + tf.matmul(h_prev, tf.transpose(self.r_z)) + self.w_bz + self.r_bz
         r = tf.matmul(inputs, tf.transpose(self.w_r)) + tf.matmul(h_prev, tf.transpose(self.r_r)) + self.w_br + self.r_br
 
 
         # h_default = self.g(np.dot(row, np.transpose(w_h)) + np.dot(r * h_prev, np.transpose(r_h)) + w_bh + r_bh)
         # h_linear = self.g(np.dot(row, np.transpose(w_h)) + r * (np.dot(h_prev, np.transpose(r_h)) + r_bh) + w_bh)
         if not self.linear_before_reset:
-            h = tf.matmul(inputs, tf.transpose(self.w_h)) + tf.matmul(r * h_prev, tf.transpose(self.r_h)) + self.w_bh + self.r_bh
+            h = tf.matmul(inputs, tf.transpose(self.w_h)) + tf.matmul(r * h_prev, tf.transpose(self.r_h)) + self.r_bh + self.w_bh
         else:
             h = tf.matmul(inputs, tf.transpose(self.w_h)) + r * (tf.matmul(h_prev, tf.transpose(self.r_h)) + self.r_bh) + self.w_bh
 
         offsetidx = 2 if self.is_bidirectional and self.go_backwards else 0
 
         if not self.clip:
             z = self.activations[0 + offsetidx](z)
@@ -287,16 +283,14 @@
         w_br,
         w_bh,
 
         r_bz,
         r_br,
         r_bh,
 
-        activation_alphas,
-        activation_betas,
         activations,
 
         clip,
         linear_before_reset,
         is_bidirectional,
         go_backwards,
         enable_rnn_unroll,
@@ -318,16 +312,14 @@
         self.w_br=w_br
         self.w_bh=w_bh
 
         self.r_bz=r_bz
         self.r_br=r_br
         self.r_bh=r_bh
 
-        self.activation_alphas = activation_alphas
-        self.activation_betas = activation_betas
         self.activations = activations
 
         self.return_sequences = return_sequences
         self.is_bidirectional = is_bidirectional
         self.go_backwards = go_backwards
         self.enable_rnn_unroll = enable_rnn_unroll
 
@@ -349,16 +341,14 @@
             self.w_br,
             self.w_bh,
 
             self.r_bz,
             self.r_br,
             self.r_bh,
 
-            self.activation_alphas,
-            self.activation_betas,
             self.activations,
 
             self.clip,
             self.linear_before_reset,
             self.is_bidirectional,
             self.go_backwards,
         )
@@ -509,16 +499,14 @@
     # Different value ranges for each activation function
     #   forward, reverse: 3 items
     #   bidirectional: 6 items
     activation_beta: List[float] = graph_node.attrs.get('activation_beta', [])
 
     # Default activation function setting
     tf_activations: List = None
-    tf_activation_alphas: List = None
-    tf_activation_betas: List = None
 
     clip: float =  graph_node.attrs.get('clip', None)
     direction: str =  graph_node.attrs.get('direction', 'forward')
 
     if direction in ['reverse', 'bidirectional']:
         print(
             f'{Color.RED}ERROR:{Color.RESET} ' +
@@ -738,40 +726,30 @@
         r_z, r_r, r_h = tf.split(tR, num_or_size_splits=3) # [4, 4], [4, 4], [4, 4]
         w_bz, w_br, w_bh, r_bz, r_br, r_bh = tf.split(tB, num_or_size_splits=6) # [4], [4], [4], [4], [4], [4]
 
         # forward
         forward_lstm = CustomGRU(
             hidden_size=hidden_size,
 
-            # w_z=w_z,
-            # w_r=w_r,
-            w_z=w_r,
-            w_r=w_z,
+            w_z=w_z,
+            w_r=w_r,
             w_h=w_h,
 
-            # r_z=r_z,
-            # r_r=r_r,
-            r_z=r_r,
-            r_r=r_z,
+            r_z=r_z,
+            r_r=r_r,
             r_h=r_h,
 
-            # w_bz=w_bz,
-            # w_br=w_br,
-            w_bz=w_br,
-            w_br=w_bz,
+            w_bz=w_bz,
+            w_br=w_br,
             w_bh=w_bh,
 
-            # r_bz=r_bz,
-            # r_br=r_br,
-            r_bz=r_br,
-            r_br=r_bz,
+            r_bz=r_bz,
+            r_br=r_br,
             r_bh=r_bh,
 
-            activation_alphas=tf_activation_alphas,
-            activation_betas=tf_activation_betas,
             activations=tf_activations,
 
             clip=clip,
             linear_before_reset=linear_before_reset,
             is_bidirectional=False,
             go_backwards=False,
             enable_rnn_unroll=enable_rnn_unroll,
@@ -796,16 +774,14 @@
             hidden_size=hidden_size,
             W_z=rW_z,
             W_r=rW_r,
             W_h=rW_h,
             R_z=rR_z,
             R_r=rR_r,
             R_h=rR_h,
-            activation_alphas=tf_activation_alphas,
-            activation_betas=tf_activation_betas,
             activations=tf_activations,
             bias_z=rB_z,
             bias_r=rB_r,
             bias_wh=rB_wh,
             bias_rh=rB_rh,
             clip=clip,
             linear_before_reset=linear_before_reset,
@@ -844,16 +820,14 @@
             hidden_size=hidden_size,
             W_z=fW_z,
             W_r=fW_r,
             W_h=fW_h,
             R_z=fR_z,
             R_r=fR_r,
             R_h=fR_h,
-            activation_alphas=tf_activation_alphas,
-            activation_betas=tf_activation_betas,
             activations=tf_activations,
             bias_z=fB_z,
             bias_r=fB_r,
             bias_wh=fB_wh,
             bias_rh=fB_rh,
             clip=clip,
             linear_before_reset=linear_before_reset,
@@ -867,16 +841,14 @@
             hidden_size=hidden_size,
             W_z=rW_z,
             W_r=rW_r,
             W_h=rW_h,
             R_z=rR_z,
             R_r=rR_r,
             R_h=rR_h,
-            activation_alphas=tf_activation_alphas,
-            activation_betas=tf_activation_betas,
             activations=tf_activations,
             bias_z=rB_z,
             bias_r=rB_r,
             bias_wh=rB_wh,
             bias_rh=rB_rh,
             clip=clip,
             linear_before_reset=linear_before_reset,
@@ -936,16 +908,14 @@
                     'W': W,
                     'R': R,
                     'B': B,
                     'hidden_size': hidden_size,
                     'sequence_lens': sequence_lens,
                     'initial_h': initial_h,
                     'activations': tf_activations,
-                    'activation_alpha': tf_activation_alphas,
-                    'activation_beta': tf_activation_betas,
                     'clip': clip,
                     'linear_before_reset': linear_before_reset,
                     'layout': layout,
                 },
                 'tf_outputs': tf_outputs,
             }
         )
```

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Gather.py` & `onnx2tf-1.9.1/onnx2tf/ops/Gather.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/GatherElements.py` & `onnx2tf-1.9.1/onnx2tf/ops/GatherElements.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/GatherND.py` & `onnx2tf-1.9.1/onnx2tf/ops/GatherND.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Gemm.py` & `onnx2tf-1.9.1/onnx2tf/ops/Gemm.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/GlobalAveragePool.py` & `onnx2tf-1.9.1/onnx2tf/ops/GlobalAveragePool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/GlobalLpPool.py` & `onnx2tf-1.9.1/onnx2tf/ops/GlobalLpPool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/GlobalMaxPool.py` & `onnx2tf-1.9.1/onnx2tf/ops/GlobalMaxPool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Greater.py` & `onnx2tf-1.9.1/onnx2tf/ops/Greater.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/GreaterOrEqual.py` & `onnx2tf-1.9.1/onnx2tf/ops/GreaterOrEqual.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/GridSample.py` & `onnx2tf-1.9.1/onnx2tf/ops/GridSample.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/HardSigmoid.py` & `onnx2tf-1.9.1/onnx2tf/ops/HardSigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/HardSwish.py` & `onnx2tf-1.9.1/onnx2tf/ops/HardSwish.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Hardmax.py` & `onnx2tf-1.9.1/onnx2tf/ops/Hardmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Identity.py` & `onnx2tf-1.9.1/onnx2tf/ops/Identity.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/If.py` & `onnx2tf-1.9.1/onnx2tf/ops/If.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Input.py` & `onnx2tf-1.9.1/onnx2tf/ops/Input.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/InstanceNormalization.py` & `onnx2tf-1.9.1/onnx2tf/ops/InstanceNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Inverse.py` & `onnx2tf-1.9.1/onnx2tf/ops/Inverse.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/IsInf.py` & `onnx2tf-1.9.1/onnx2tf/ops/IsInf.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/IsNaN.py` & `onnx2tf-1.9.1/onnx2tf/ops/IsNaN.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/LRN.py` & `onnx2tf-1.9.1/onnx2tf/ops/LRN.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/LSTM.py` & `onnx2tf-1.9.1/onnx2tf/ops/LSTM.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/LayerNormalization.py` & `onnx2tf-1.9.1/onnx2tf/ops/LayerNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/LeakyRelu.py` & `onnx2tf-1.9.1/onnx2tf/ops/LeakyRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Less.py` & `onnx2tf-1.9.1/onnx2tf/ops/Less.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/LessOrEqual.py` & `onnx2tf-1.9.1/onnx2tf/ops/LessOrEqual.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Log.py` & `onnx2tf-1.9.1/onnx2tf/ops/Log.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/LogSoftmax.py` & `onnx2tf-1.9.1/onnx2tf/ops/LogSoftmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/LpNormalization.py` & `onnx2tf-1.9.1/onnx2tf/ops/LpNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/MatMul.py` & `onnx2tf-1.9.1/onnx2tf/ops/MatMul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/MatMulInteger.py` & `onnx2tf-1.9.1/onnx2tf/ops/MatMulInteger.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Max.py` & `onnx2tf-1.9.1/onnx2tf/ops/Max.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/MaxPool.py` & `onnx2tf-1.9.1/onnx2tf/ops/MaxPool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/MaxUnpool.py` & `onnx2tf-1.9.1/onnx2tf/ops/MaxUnpool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Mean.py` & `onnx2tf-1.9.1/onnx2tf/ops/Mean.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/MeanVarianceNormalization.py` & `onnx2tf-1.9.1/onnx2tf/ops/MeanVarianceNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Min.py` & `onnx2tf-1.9.1/onnx2tf/ops/Min.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Mish.py` & `onnx2tf-1.9.1/onnx2tf/ops/Mish.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Mod.py` & `onnx2tf-1.9.1/onnx2tf/ops/Mod.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Mul.py` & `onnx2tf-1.9.1/onnx2tf/ops/Mul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Multinomial.py` & `onnx2tf-1.9.1/onnx2tf/ops/Multinomial.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Neg.py` & `onnx2tf-1.9.1/onnx2tf/ops/Neg.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/NonMaxSuppression.py` & `onnx2tf-1.9.1/onnx2tf/ops/NonMaxSuppression.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/NonZero.py` & `onnx2tf-1.9.1/onnx2tf/ops/NonZero.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Not.py` & `onnx2tf-1.9.1/onnx2tf/ops/Not.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/OneHot.py` & `onnx2tf-1.9.1/onnx2tf/ops/OneHot.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Or.py` & `onnx2tf-1.9.1/onnx2tf/ops/Or.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/PRelu.py` & `onnx2tf-1.9.1/onnx2tf/ops/PRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Pad.py` & `onnx2tf-1.9.1/onnx2tf/ops/Pad.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Pow.py` & `onnx2tf-1.9.1/onnx2tf/ops/Pow.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/QLinearAdd.py` & `onnx2tf-1.9.1/onnx2tf/ops/QLinearAdd.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/QLinearConcat.py` & `onnx2tf-1.9.1/onnx2tf/ops/QLinearConcat.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/QLinearConv.py` & `onnx2tf-1.9.1/onnx2tf/ops/QLinearConv.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/QLinearLeakyRelu.py` & `onnx2tf-1.9.1/onnx2tf/ops/QLinearLeakyRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/QLinearMatMul.py` & `onnx2tf-1.9.1/onnx2tf/ops/QLinearMatMul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/QLinearMul.py` & `onnx2tf-1.9.1/onnx2tf/ops/QLinearMul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/QLinearSigmoid.py` & `onnx2tf-1.9.1/onnx2tf/ops/QLinearSigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/QLinearSoftmax.py` & `onnx2tf-1.9.1/onnx2tf/ops/QLinearSoftmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/QuantizeLinear.py` & `onnx2tf-1.9.1/onnx2tf/ops/QuantizeLinear.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/RNN.py` & `onnx2tf-1.9.1/onnx2tf/ops/RNN.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/RandomNormal.py` & `onnx2tf-1.9.1/onnx2tf/ops/RandomNormal.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/RandomNormalLike.py` & `onnx2tf-1.9.1/onnx2tf/ops/RandomNormalLike.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/RandomUniform.py` & `onnx2tf-1.9.1/onnx2tf/ops/RandomUniform.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/RandomUniformLike.py` & `onnx2tf-1.9.1/onnx2tf/ops/RandomUniformLike.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Range.py` & `onnx2tf-1.9.1/onnx2tf/ops/Range.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Reciprocal.py` & `onnx2tf-1.9.1/onnx2tf/ops/Reciprocal.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceL1.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceL1.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceL2.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceL2.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceLogSum.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceLogSum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceLogSumExp.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceLogSumExp.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceMax.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceMax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceMean.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceMean.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceMin.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceMin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceProd.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceProd.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceSum.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceSum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReduceSumSquare.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReduceSumSquare.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Relu.py` & `onnx2tf-1.9.1/onnx2tf/ops/Relu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Reshape.py` & `onnx2tf-1.9.1/onnx2tf/ops/Reshape.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Resize.py` & `onnx2tf-1.9.1/onnx2tf/ops/Resize.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ReverseSequence.py` & `onnx2tf-1.9.1/onnx2tf/ops/ReverseSequence.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/RoiAlign.py` & `onnx2tf-1.9.1/onnx2tf/ops/RoiAlign.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Round.py` & `onnx2tf-1.9.1/onnx2tf/ops/Round.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ScaleAndTranslate.py` & `onnx2tf-1.9.1/onnx2tf/ops/ScaleAndTranslate.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Scatter.py` & `onnx2tf-1.9.1/onnx2tf/ops/Scatter.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ScatterElements.py` & `onnx2tf-1.9.1/onnx2tf/ops/ScatterElements.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ScatterND.py` & `onnx2tf-1.9.1/onnx2tf/ops/ScatterND.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Selu.py` & `onnx2tf-1.9.1/onnx2tf/ops/Selu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/SequenceAt.py` & `onnx2tf-1.9.1/onnx2tf/ops/SequenceAt.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/SequenceConstruct.py` & `onnx2tf-1.9.1/onnx2tf/ops/SequenceConstruct.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/SequenceEmpty.py` & `onnx2tf-1.9.1/onnx2tf/ops/SequenceEmpty.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/SequenceErase.py` & `onnx2tf-1.9.1/onnx2tf/ops/SequenceErase.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/SequenceInsert.py` & `onnx2tf-1.9.1/onnx2tf/ops/SequenceInsert.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/SequenceLength.py` & `onnx2tf-1.9.1/onnx2tf/ops/SequenceLength.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Shape.py` & `onnx2tf-1.9.1/onnx2tf/ops/Shape.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Shrink.py` & `onnx2tf-1.9.1/onnx2tf/ops/Shrink.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Sigmoid.py` & `onnx2tf-1.9.1/onnx2tf/ops/Sigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Sign.py` & `onnx2tf-1.9.1/onnx2tf/ops/Sign.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Sin.py` & `onnx2tf-1.9.1/onnx2tf/ops/Sin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Sinh.py` & `onnx2tf-1.9.1/onnx2tf/ops/Sinh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Size.py` & `onnx2tf-1.9.1/onnx2tf/ops/Size.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Slice.py` & `onnx2tf-1.9.1/onnx2tf/ops/Slice.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Softmax.py` & `onnx2tf-1.9.1/onnx2tf/ops/Softmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Softplus.py` & `onnx2tf-1.9.1/onnx2tf/ops/Softplus.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Softsign.py` & `onnx2tf-1.9.1/onnx2tf/ops/Softsign.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/SpaceToDepth.py` & `onnx2tf-1.9.1/onnx2tf/ops/SpaceToDepth.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Split.py` & `onnx2tf-1.9.1/onnx2tf/ops/Split.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/SplitToSequence.py` & `onnx2tf-1.9.1/onnx2tf/ops/SplitToSequence.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Sqrt.py` & `onnx2tf-1.9.1/onnx2tf/ops/Sqrt.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Squeeze.py` & `onnx2tf-1.9.1/onnx2tf/ops/Squeeze.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Sub.py` & `onnx2tf-1.9.1/onnx2tf/ops/Sub.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Sum.py` & `onnx2tf-1.9.1/onnx2tf/ops/Sum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Tan.py` & `onnx2tf-1.9.1/onnx2tf/ops/Tan.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Tanh.py` & `onnx2tf-1.9.1/onnx2tf/ops/Tanh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/ThresholdedRelu.py` & `onnx2tf-1.9.1/onnx2tf/ops/ThresholdedRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Tile.py` & `onnx2tf-1.9.1/onnx2tf/ops/Tile.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/TopK.py` & `onnx2tf-1.9.1/onnx2tf/ops/TopK.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Transpose.py` & `onnx2tf-1.9.1/onnx2tf/ops/Transpose.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Trilu.py` & `onnx2tf-1.9.1/onnx2tf/ops/Trilu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Unique.py` & `onnx2tf-1.9.1/onnx2tf/ops/Unique.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Unsqueeze.py` & `onnx2tf-1.9.1/onnx2tf/ops/Unsqueeze.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Upsample.py` & `onnx2tf-1.9.1/onnx2tf/ops/Upsample.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Where.py` & `onnx2tf-1.9.1/onnx2tf/ops/Where.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/Xor.py` & `onnx2tf-1.9.1/onnx2tf/ops/Xor.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/ops/_Loop.py` & `onnx2tf-1.9.1/onnx2tf/ops/_Loop.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/utils/colors.py` & `onnx2tf-1.9.1/onnx2tf/utils/colors.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/utils/common_functions.py` & `onnx2tf-1.9.1/onnx2tf/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf/utils/enums.py` & `onnx2tf-1.9.1/onnx2tf/utils/enums.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/onnx2tf.egg-info/PKG-INFO` & `onnx2tf-1.9.1/onnx2tf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2tf
-Version: 1.9.0
+Version: 1.9.1
 Summary: Self-Created Tools to convert ONNX files (NCHW) to TensorFlow/TFLite/Keras format (NHWC). The purpose of this tool is to solve the massive Transpose extrapolation problem in onnx-tensorflow (onnx-tf).
 Home-page: https://github.com/PINTO0309/onnx2tf
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -252,15 +252,15 @@
 ## Sample Usage
 ### 1. Install
 - HostPC
   ```
   $ docker run --rm -it \
   -v `pwd`:/workdir \
   -w /workdir \
-  ghcr.io/pinto0309/onnx2tf:1.9.0
+  ghcr.io/pinto0309/onnx2tf:1.9.1
 
   or
 
   $ pip install -U onnx \
   && pip install -U nvidia-pyindex \
   && pip install -U onnx-graphsurgeon \
   && pip install -U onnxruntime==1.13.1 \
@@ -528,15 +528,15 @@
 
     |Before|After|
     |:-:|:-:|
     |`HardSwish`<br>![image](https://user-images.githubusercontent.com/33194443/226223099-c7344bcf-d24d-4b35-a1d6-2a03dbfce8c7.png)|`ReLU`<br>![image](https://user-images.githubusercontent.com/33194443/226223213-bd714994-f353-416e-9f54-6d0954a70bb8.png)|
 
 
 ### 7. Calibration data creation for INT8 quantization
-Calibration data (.npy) for INT8 quantization (`-qcind`) is generated as follows. This is a sample when the data used for training is image data. See: https://github.com/PINTO0309/onnx2tf/issues/222
+Calibration data (.npy) for INT8 quantization (`-cind`) is generated as follows. This is a sample when the data used for training is image data. See: https://github.com/PINTO0309/onnx2tf/issues/222
 
 https://www.tensorflow.org/lite/performance/post_training_quantization
 
 ```python
 import cv2
 import glob
 import numpy as np
@@ -563,20 +563,20 @@
 print(f'calib_datas.shape: {calib_datas.shape}') # [10,112,200,3]
 np.save(file='data/calibdata.npy', arr=calib_datas)
 
 loaded_data = np.load('data/calibdata.npy')
 print(f'loaded_data.shape: {loaded_data.shape}') # [10,112,200,3]
 
 """
--qcind INPUT_NAME NUMPY_FILE_PATH MEAN STD
+-cind INPUT_NAME NUMPY_FILE_PATH MEAN STD
 int8_calib_datas = (loaded_data - MEAN) / STD # -1.0 - 1.0
 
 e.g.
--qcind pc_dep 'data/calibdata.npy' [[[[0.485, 0.456, 0.406]]]] [[[[0.229, 0.224, 0.225]]]]
--qcind feat 'data/calibdata2.npy' [[[[0.123, ..., 0.321]]]] [[[[0.112, ..., 0.451]]]]
+-cind pc_dep 'data/calibdata.npy' [[[[0.485, 0.456, 0.406]]]] [[[[0.229, 0.224, 0.225]]]]
+-cind feat 'data/calibdata2.npy' [[[[0.123, ..., 0.321]]]] [[[[0.112, ..., 0.451]]]]
 """
 ```
 
 ### 8. INT8 quantization of models with multiple inputs requiring non-image data
 If you do not need to perform INT8 quantization with this tool alone, the following method is the easiest.
 
 The `-osd` option will output a `saved_model.pb` in the `saved_model` folder with the full size required for quantization. That is, a default signature named `serving_default` is embedded in `.pb`. The `-b` option is used to convert the batch size by rewriting it as a static integer.
@@ -652,15 +652,52 @@
 
 ![image](https://user-images.githubusercontent.com/33194443/225174599-e62173f3-1dd2-48f4-a762-f15ef78cd01e.png)
 
 https://www.tensorflow.org/lite/performance/post_training_quantization
 
 See: https://github.com/PINTO0309/onnx2tf/issues/248
 
-### 9. Conversion to TensorFlow.js
+### 9. Fixing the output of NonMaxSuppression (NMS)
+PyTorch's `NonMaxSuppression (torchvision.ops.nms)` and ONNX's `NonMaxSuppression` are not fully compatible. TorchVision's NMS is very inefficient. Therefore, it is inevitable that converting ONNX using NMS in object detection models and other models will be very redundant and will be converted with a structure that is difficult for TensorFlow.js and TFLite models to take advantage of in devices. This is due to the indefinite number of tensors output by the NMS. In this chapter, I share how to easily tune the ONNX generated using TorchVision's redundant NMS to generate an optimized NMS.
+
+1. There are multiple issues with TorchVision's NMS. First, the batch size specification is not supported; second, the `max_output_boxes_per_class` parameter cannot be specified. Please see the NMS sample ONNX part I generated. The `max_output_boxes_per_class` has been changed to `896` instead of `-Infinity`. The biggest problem with TorchVision NMS is that it generates ONNX with `max_output_boxes_per_class` set to `-Infinity` or `9223372036854775807 (Maximum value of INT64)`, resulting in a variable number of NMS outputs from zero to infinite. Thus, by rewriting `-Infinity` or `9223372036854775807 (Maximum value of INT64)` to a constant value, it is possible to output an NMS that can be effortlessly inferred by TFJS or TFLite.
+![image](https://user-images.githubusercontent.com/33194443/230778827-faab8ffe-d49f-498d-b414-a1a26848a380.png)
+
+    Here you will find committed ONNX components optimized for various devices.
+    https://github.com/PINTO0309/components_of_onnx/tree/main/components_of_onnx/ops
+
+2. In the following example, the `max_output_boxes_per_class` of NMS in the post-processing generated by YOLOv7 is changed from `-Infinity` or `9223372036854775807 (Maximum value of INT64)` to `20`, as shown in the figure below. The name `main01_max_output_boxes_per_class` has been rewritten by me for clarity, but it originally appears as `max_output_boxes_per_class`.
+![image](https://user-images.githubusercontent.com/33194443/230779419-23cc017f-fde9-4777-bb3d-766a35a09efd.png)
+
+    Simply execute the following command. The command rewrites the specified attribute value of the OP specified by ONNX.
+    ```bash
+    pip install sam4onnx
+
+    sam4onnx \
+    --op_name main01_nonmaxsuppression11 \
+    --input_onnx_file_path yolov7.onnx \
+    --output_onnx_file_path nms_yolov7_update.onnx \
+    --input_constants main01_max_output_boxes_per_class int64 [20]
+    ```
+    A tutorial on one of my ONNX modification tools, `sam4onnx`, can be found here.
+
+    https://github.com/PINTO0309/sam4onnx
+
+    Many detailed tutorials are provided below, so if you are interested, please play with them.
+
+    https://github.com/PINTO0309/PINTO_model_zoo/tree/main/307_YOLOv7/post_process_gen_tools
+
+3. Finally, simply convert ONNX to TFLite or saved_model or TFJS using onnx2tf. onnx2tf performs an internal operation to automatically optimize the NMS output to a fixed shape if `max_output_boxes_per_class` is set to a value other than `-Infinity` and `9223372036854775807 (Maximum value of INT64)`. Specify `--output_nms_with_dynamic_tensor` or `-onwdt` if you do not want to optimize for a fixed shape.
+    ```
+    onnx2tf -i nms_yolov7_update.onnx -osd -cotof
+    ```
+    I would be happy if this is a reference for Android + Java or TFJS implementations. There are tons more tricky model optimization techniques described in my blog posts, so you'll have to find them yourself. I don't dare to list the URL here because it is annoying to see so many `issues` being posted. And unfortunately, all articles are in Japanese.
+    ![image](https://user-images.githubusercontent.com/33194443/230780749-9967a34b-abf6-47fe-827d-92e0f6bddf46.png)
+
+### 10. Conversion to TensorFlow.js
 When converting to TensorFlow.js, process as follows.
 
 ```bash
 pip install tensorflowjs
 
 onnx2tf -i mobilenetv2-12.onnx -ois input:1,3,224,224 -osd
 
@@ -671,15 +708,15 @@
 tfjs_model
 ```
 
 See: https://github.com/tensorflow/tfjs/tree/master/tfjs-converter
 
 ![image](https://user-images.githubusercontent.com/33194443/224186149-0b9ce9dc-fe09-48d4-b430-6cc3d0687140.png)
 
-### 10. Conversion to CoreML
+### 11. Conversion to CoreML
 When converting to CoreML, process as follows. The `-k` option is for conversion while maintaining the input channel order in ONNX's NCHW format.
 
 ```bash
 pip install coremltools
 
 onnx2tf -i mobilenetv2-12.onnx -k input -ois input:1,3,224,224 -osd
 ```
```

### Comparing `onnx2tf-1.9.0/onnx2tf.egg-info/SOURCES.txt` & `onnx2tf-1.9.1/onnx2tf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/setup.py` & `onnx2tf-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.0/tests/test_model_convert.py` & `onnx2tf-1.9.1/tests/test_model_convert.py`

 * *Files identical despite different names*

