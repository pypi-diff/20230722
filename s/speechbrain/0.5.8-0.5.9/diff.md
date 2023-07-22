# Comparing `tmp/speechbrain-0.5.8.tar.gz` & `tmp/speechbrain-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechbrain-0.5.8.tar", last modified: Sun Jun  6 21:24:37 2021, max compression
+gzip compressed data, was "speechbrain-0.5.9.tar", last modified: Thu Jun 17 01:26:00 2021, max compression
```

## Comparing `speechbrain-0.5.8.tar` & `speechbrain-0.5.9.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.485285 speechbrain-0.5.8/
--rw-r--r--   0 mirco     (1000) mirco     (1000)    11357 2021-06-06 20:59:33.000000 speechbrain-0.5.8/LICENSE
--rw-r--r--   0 mirco     (1000) mirco     (1000)    11923 2021-06-06 21:24:37.485285 speechbrain-0.5.8/PKG-INFO
--rw-r--r--   0 mirco     (1000) mirco     (1000)    11572 2021-06-06 20:59:33.000000 speechbrain-0.5.8/README.md
--rw-r--r--   0 mirco     (1000) mirco     (1000)      239 2021-06-06 20:59:33.000000 speechbrain-0.5.8/pyproject.toml
--rw-r--r--   0 mirco     (1000) mirco     (1000)       38 2021-06-06 21:24:37.485285 speechbrain-0.5.8/setup.cfg
--rw-r--r--   0 mirco     (1000) mirco     (1000)      951 2021-06-06 20:59:33.000000 speechbrain-0.5.8/setup.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.465285 speechbrain-0.5.8/speechbrain/
--rw-r--r--   0 mirco     (1000) mirco     (1000)      627 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/__init__.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.469285 speechbrain-0.5.8/speechbrain/alignment/
--rw-r--r--   0 mirco     (1000) mirco     (1000)       57 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/alignment/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    52764 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/alignment/aligner.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    45521 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/core.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.469285 speechbrain-0.5.8/speechbrain/dataio/
--rw-r--r--   0 mirco     (1000) mirco     (1000)      297 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     6642 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/batch.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    29381 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/dataio.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     8579 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/dataloader.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    15527 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/dataset.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    38980 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/encoder.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    10629 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/legacy.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     2276 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/preprocess.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    22874 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/sampler.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     5966 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/dataio/wer.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.473285 speechbrain-0.5.8/speechbrain/decoders/
--rw-r--r--   0 mirco     (1000) mirco     (1000)      130 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/decoders/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    13521 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/decoders/ctc.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    45059 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/decoders/seq2seq.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    19476 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/decoders/transducer.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.473285 speechbrain-0.5.8/speechbrain/lm/
--rw-r--r--   0 mirco     (1000) mirco     (1000)       41 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lm/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     7508 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lm/arpa.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     4500 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lm/counting.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     6874 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lm/ngram.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.473285 speechbrain-0.5.8/speechbrain/lobes/
--rw-r--r--   0 mirco     (1000) mirco     (1000)      211 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    17768 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/augment.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     9707 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/features.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.477285 speechbrain-0.5.8/speechbrain/lobes/models/
--rw-r--r--   0 mirco     (1000) mirco     (1000)    10521 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/CRDNN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     9241 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/ContextNet.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    15594 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/ECAPA_TDNN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     3675 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/ESPnetVGG.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     4933 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/MetricGAN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     3555 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/RNNLM.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     1178 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/VanillaNN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     6846 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/Xvector.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)       69 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    16069 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/conv_tasnet.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     5094 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/convolution.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    40912 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/dual_path.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     9775 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/fairseq_wav2vec.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     5160 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/huggingface_wav2vec.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.477285 speechbrain-0.5.8/speechbrain/lobes/models/transformer/
--rw-r--r--   0 mirco     (1000) mirco     (1000)    21415 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/transformer/Transformer.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     8203 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/transformer/TransformerASR.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     4538 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/transformer/TransformerLM.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     3003 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/transformer/TransformerSE.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)      151 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/transformer/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     7703 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/lobes/models/transformer/conformer.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)      520 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/log-config.yaml
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.477285 speechbrain-0.5.8/speechbrain/nnet/
--rw-r--r--   0 mirco     (1000) mirco     (1000)    32457 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/CNN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    49843 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/RNN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)      351 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     3315 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/activations.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    15390 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/attention.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.481285 speechbrain-0.5.8/speechbrain/nnet/complex_networks/
--rw-r--r--   0 mirco     (1000) mirco     (1000)       50 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/complex_networks/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    14753 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_CNN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    37992 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_RNN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     4020 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_linear.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    26306 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_normalization.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     9840 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_ops.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    13230 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/containers.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     1320 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/dropout.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     3928 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/embedding.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     1825 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/linear.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.481285 speechbrain-0.5.8/speechbrain/nnet/loss/
--rw-r--r--   0 mirco     (1000) mirco     (1000)       65 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/loss/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     6334 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/loss/stoi_loss.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    13423 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/loss/transducer_loss.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    35170 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/losses.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    10415 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/normalization.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     9853 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/pooling.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.481285 speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/
--rw-r--r--   0 mirco     (1000) mirco     (1000)       53 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    20523 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_CNN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    40503 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_RNN.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     7965 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_linear.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     5396 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_normalization.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    28142 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_ops.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    23510 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/schedulers.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.481285 speechbrain-0.5.8/speechbrain/nnet/transducer/
--rw-r--r--   0 mirco     (1000) mirco     (1000)       53 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/transducer/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     3106 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/nnet/transducer/transducer_joint.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.481285 speechbrain-0.5.8/speechbrain/pretrained/
--rw-r--r--   0 mirco     (1000) mirco     (1000)       59 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/pretrained/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     4034 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/pretrained/fetching.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    32709 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/pretrained/interfaces.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.485285 speechbrain-0.5.8/speechbrain/processing/
--rw-r--r--   0 mirco     (1000) mirco     (1000)     5770 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/processing/NMF.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    34437 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/processing/PLDA_LDA.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)       67 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/processing/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    11688 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/processing/decomposition.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    31281 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/processing/diarization.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    38962 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/processing/features.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    52862 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/processing/multi_mic.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    17423 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/processing/signal_processing.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    42719 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/processing/speech_augmentation.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.485285 speechbrain-0.5.8/speechbrain/tokenizers/
--rw-r--r--   0 mirco     (1000) mirco     (1000)    18988 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/tokenizers/SentencePiece.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)       53 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/tokenizers/__init__.py
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.485285 speechbrain-0.5.8/speechbrain/utils/
--rw-r--r--   0 mirco     (1000) mirco     (1000)     2540 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/Accuracy.py
--rwxr-xr-x   0 mirco     (1000) mirco     (1000)     4468 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/DER.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)      320 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/__init__.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     2360 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/callchains.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    43911 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/checkpoints.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    18433 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/data_pipeline.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    15992 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/data_utils.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     9576 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/depgraph.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     6549 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/distributed.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    25691 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/edit_distance.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     2035 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/epoch_loop.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     5331 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/logger.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)    16868 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/metric_stats.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     8063 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/parameter_transfer.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     1290 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/superpowers.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)      419 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/torch_audio_backend.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)     5229 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/utils/train_logger.py
--rw-r--r--   0 mirco     (1000) mirco     (1000)        6 2021-06-06 20:59:33.000000 speechbrain-0.5.8/speechbrain/version.txt
-drwxr-xr-x   0 mirco     (1000) mirco     (1000)        0 2021-06-06 21:24:37.465285 speechbrain-0.5.8/speechbrain.egg-info/
--rw-r--r--   0 mirco     (1000) mirco     (1000)    11923 2021-06-06 21:24:37.000000 speechbrain-0.5.8/speechbrain.egg-info/PKG-INFO
--rw-r--r--   0 mirco     (1000) mirco     (1000)     4069 2021-06-06 21:24:37.000000 speechbrain-0.5.8/speechbrain.egg-info/SOURCES.txt
--rw-r--r--   0 mirco     (1000) mirco     (1000)        1 2021-06-06 21:24:37.000000 speechbrain-0.5.8/speechbrain.egg-info/dependency_links.txt
--rw-r--r--   0 mirco     (1000) mirco     (1000)       93 2021-06-06 21:24:37.000000 speechbrain-0.5.8/speechbrain.egg-info/requires.txt
--rw-r--r--   0 mirco     (1000) mirco     (1000)       12 2021-06-06 21:24:37.000000 speechbrain-0.5.8/speechbrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.020154 speechbrain-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-17 01:25:53.000000 speechbrain-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    12621 2021-06-17 01:26:00.020154 speechbrain-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12270 2021-06-17 01:25:53.000000 speechbrain-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2021-06-17 01:25:53.000000 speechbrain-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-17 01:26:00.020154 speechbrain-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2021-06-17 01:25:53.000000 speechbrain-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.012154 speechbrain-0.5.9/speechbrain/
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.012154 speechbrain-0.5.9/speechbrain/alignment/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/alignment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52764 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/alignment/aligner.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45409 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/core.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.012154 speechbrain-0.5.9/speechbrain/dataio/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6642 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/batch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29385 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/dataio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8579 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15527 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38980 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10629 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2276 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22874 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5966 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/dataio/wer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.012154 speechbrain-0.5.9/speechbrain/decoders/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13521 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/decoders/ctc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45161 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/decoders/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19476 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/decoders/transducer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.012154 speechbrain-0.5.9/speechbrain/lm/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7508 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lm/arpa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4500 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lm/counting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6874 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lm/ngram.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.012154 speechbrain-0.5.9/speechbrain/lobes/
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17660 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/augment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9707 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/features.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.016154 speechbrain-0.5.9/speechbrain/lobes/models/
+-rw-r--r--   0 runner    (1001) docker     (121)    10521 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/CRDNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9241 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/ContextNet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15594 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/ECAPA_TDNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3675 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/ESPnetVGG.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4933 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/MetricGAN.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3555 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/RNNLM.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/VanillaNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6846 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/Xvector.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16069 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/conv_tasnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5094 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40912 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/dual_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9775 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/fairseq_wav2vec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5160 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/huggingface_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.016154 speechbrain-0.5.9/speechbrain/lobes/models/transformer/
+-rw-r--r--   0 runner    (1001) docker     (121)    21415 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/transformer/Transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8203 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/transformer/TransformerASR.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/transformer/TransformerLM.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3003 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/transformer/TransformerSE.py
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7703 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/lobes/models/transformer/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/log-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.016154 speechbrain-0.5.9/speechbrain/nnet/
+-rw-r--r--   0 runner    (1001) docker     (121)    32415 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49843 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/RNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3315 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/activations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15390 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.016154 speechbrain-0.5.9/speechbrain/nnet/complex_networks/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/complex_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14753 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_CNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37992 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_RNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4020 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_linear.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26306 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9840 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_ops.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13230 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3928 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.016154 speechbrain-0.5.9/speechbrain/nnet/loss/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6334 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/loss/stoi_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13423 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/loss/transducer_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35170 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/losses.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10415 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9853 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.020154 speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20523 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_CNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40503 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_RNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7965 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_linear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5396 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28142 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_ops.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23510 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.020154 speechbrain-0.5.9/speechbrain/nnet/transducer/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/transducer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/nnet/transducer/transducer_joint.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.020154 speechbrain-0.5.9/speechbrain/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4034 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/pretrained/fetching.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32708 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/pretrained/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.020154 speechbrain-0.5.9/speechbrain/processing/
+-rw-r--r--   0 runner    (1001) docker     (121)     5770 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/processing/NMF.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34437 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/processing/PLDA_LDA.py
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11687 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/processing/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31275 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/processing/diarization.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38962 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/processing/features.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52930 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/processing/multi_mic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17423 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/processing/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42719 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/processing/speech_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.020154 speechbrain-0.5.9/speechbrain/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (121)    18988 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/tokenizers/SentencePiece.py
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.020154 speechbrain-0.5.9/speechbrain/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     2540 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/Accuracy.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4468 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/DER.py
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3864 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2360 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/callchains.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43911 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18433 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15992 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9576 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6549 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25691 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/epoch_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5331 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16868 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/metric_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8063 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/parameter_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1290 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/superpowers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/torch_audio_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5229 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/utils/train_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-06-17 01:25:53.000000 speechbrain-0.5.9/speechbrain/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 01:26:00.012154 speechbrain-0.5.9/speechbrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12621 2021-06-17 01:25:59.000000 speechbrain-0.5.9/speechbrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4095 2021-06-17 01:25:59.000000 speechbrain-0.5.9/speechbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-17 01:25:59.000000 speechbrain-0.5.9/speechbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-06-17 01:25:59.000000 speechbrain-0.5.9/speechbrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-17 01:25:59.000000 speechbrain-0.5.9/speechbrain.egg-info/top_level.txt
```

### Comparing `speechbrain-0.5.8/LICENSE` & `speechbrain-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/PKG-INFO` & `speechbrain-0.5.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechbrain
-Version: 0.5.8
+Version: 0.5.9
 Summary: All-in-one speech toolkit in pure Python and Pytorch
 Home-page: https://speechbrain.github.io/
 Author: Mirco Ravanelli & Others
 Author-email: speechbrain@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -165,8 +165,24 @@
 - General information can be found on the [website](https://speechbrain.github.io).
 - We offer many tutorials, you can start out from the [basic ones](https://speechbrain.github.io/tutorial_basics.html) about SpeechBrain basic functionalities and building blocks. We provide also more advanced tutorials (e.g SpeechBrain advanced, signal processing ...). You can browse them via the Tutorials drop down menu on [SpeechBrain website](https://speechbrain.github.io) in the upper right.
 - Details on the SpeechBrain API, how to contribute, and the code are given in the [documentation](https://speechbrain.readthedocs.io/en/latest/index.html).
 
 # License
 SpeechBrain is released under the Apache License, version 2.0. The Apache license is a popular BSD-like license. SpeechBrain can be redistributed for free, even for commercial purposes, although you can not take off the license headers (and under some circumstances, you may have to distribute a license document). Apache is not a viral license like the GPL, which forces you to release your modifications to the source code. Also note that this project has no connection to the Apache Foundation, other than that we use the same license terms.
 
+# Citing SpeechBrain
+Please, cite SpeechBrain if you use it for your research or business.
+
+```bibtex
+@misc{speechbrain,
+  title={{SpeechBrain}: A General-Purpose Speech Toolkit},
+  author={Mirco Ravanelli and Titouan Parcollet and Peter Plantinga and Aku Rouhe and Samuele Cornell and Loren Lugosch and Cem Subakan and Nauman Dawalatabad and Abdelwahab Heba and Jianyuan Zhong and Ju-Chieh Chou and Sung-Lin Yeh and Szu-Wei Fu and Chien-Feng Liao and Elena Rastorgueva and François Grondin and William Aris and Hwidong Na and Yan Gao and Renato De Mori and Yoshua Bengio},
+  year={2021},
+  eprint={2106.04624},
+  archivePrefix={arXiv},
+  primaryClass={eess.AS},
+  note={arXiv:2106.04624}
+}
+```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `speechbrain-0.5.8/README.md` & `speechbrain-0.5.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -151,7 +151,23 @@
 Instead of a long and boring README, we prefer to provide you with different resources that can be used to learn how to customize SpeechBrain to adapt it to your needs:
 - General information can be found on the [website](https://speechbrain.github.io).
 - We offer many tutorials, you can start out from the [basic ones](https://speechbrain.github.io/tutorial_basics.html) about SpeechBrain basic functionalities and building blocks. We provide also more advanced tutorials (e.g SpeechBrain advanced, signal processing ...). You can browse them via the Tutorials drop down menu on [SpeechBrain website](https://speechbrain.github.io) in the upper right.
 - Details on the SpeechBrain API, how to contribute, and the code are given in the [documentation](https://speechbrain.readthedocs.io/en/latest/index.html).
 
 # License
 SpeechBrain is released under the Apache License, version 2.0. The Apache license is a popular BSD-like license. SpeechBrain can be redistributed for free, even for commercial purposes, although you can not take off the license headers (and under some circumstances, you may have to distribute a license document). Apache is not a viral license like the GPL, which forces you to release your modifications to the source code. Also note that this project has no connection to the Apache Foundation, other than that we use the same license terms.
+
+# Citing SpeechBrain
+Please, cite SpeechBrain if you use it for your research or business.
+
+```bibtex
+@misc{speechbrain,
+  title={{SpeechBrain}: A General-Purpose Speech Toolkit},
+  author={Mirco Ravanelli and Titouan Parcollet and Peter Plantinga and Aku Rouhe and Samuele Cornell and Loren Lugosch and Cem Subakan and Nauman Dawalatabad and Abdelwahab Heba and Jianyuan Zhong and Ju-Chieh Chou and Sung-Lin Yeh and Szu-Wei Fu and Chien-Feng Liao and Elena Rastorgueva and François Grondin and William Aris and Hwidong Na and Yan Gao and Renato De Mori and Yoshua Bengio},
+  year={2021},
+  eprint={2106.04624},
+  archivePrefix={arXiv},
+  primaryClass={eess.AS},
+  note={arXiv:2106.04624}
+}
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `speechbrain-0.5.8/setup.py` & `speechbrain-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/__init__.py` & `speechbrain-0.5.9/speechbrain/__init__.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/alignment/aligner.py` & `speechbrain-0.5.9/speechbrain/alignment/aligner.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/core.py` & `speechbrain-0.5.9/speechbrain/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 logger = logging.getLogger(__name__)
 DEFAULT_LOG_CONFIG = os.path.dirname(os.path.abspath(__file__))
 DEFAULT_LOG_CONFIG = os.path.join(DEFAULT_LOG_CONFIG, "log-config.yaml")
 torch._C._jit_set_profiling_executor(False)
 torch._C._jit_set_profiling_mode(False)
 INTRA_EPOCH_CKPT_FLAG = "brain_intra_epoch_ckpt"
+PYTHON_VERSION_MAJOR = 3
+PYTHON_VERSION_MINOR = 7
 
 
 def create_experiment_directory(
     experiment_directory,
     hyperparams_to_save=None,
     overrides={},
     log_config=DEFAULT_LOG_CONFIG,
@@ -190,20 +192,14 @@
     parser.add_argument(
         "--device",
         type=str,
         default="cuda:0",
         help="The device to run the experiment on (e.g. 'cuda:0')",
     )
     parser.add_argument(
-        "--data_parallel_count",
-        type=int,
-        default=-1,
-        help="Number of devices that are used for data_parallel computation",
-    )
-    parser.add_argument(
         "--data_parallel_backend",
         default=False,
         action="store_true",
         help="This flag enables training with data_parallel.",
     )
     parser.add_argument(
         "--distributed_launch",
@@ -215,14 +211,20 @@
     parser.add_argument(
         "--distributed_backend",
         type=str,
         default="nccl",
         help="One of {nccl, gloo, mpi}",
     )
     parser.add_argument(
+        "--find_unused_parameters",
+        default=False,
+        action="store_true",
+        help="This flag disable unused parameters detection",
+    )
+    parser.add_argument(
         "--jit_module_keys",
         type=str,
         nargs="*",
         help="A list of keys in the 'modules' dict to jitify",
     )
     parser.add_argument(
         "--auto_mix_prec",
@@ -263,25 +265,16 @@
     param_file = run_opts["param_file"]
     del run_opts["param_file"]
 
     overrides = _convert_to_yaml(overrides)
 
     # Checking that DataParallel use the right number of GPU
     if run_opts["data_parallel_backend"]:
-        if run_opts["data_parallel_count"] == 0:
-            raise ValueError(
-                "data_parallel_count must be > 1."
-                "if data_parallel_count = -1, then use all gpus."
-            )
-        if run_opts["data_parallel_count"] > torch.cuda.device_count():
-            raise ValueError(
-                "data_parallel_count must be <= "
-                + str(torch.cuda.device_count())
-                + "if data_parallel_count = -1, then use all gpus."
-            )
+        if torch.cuda.device_count() == 0:
+            raise ValueError("You must have at least 1 GPU.")
 
     # For DDP, the device args must equal to local_rank used by
     # torch.distributed.launch. If run_opts["local_rank"] exists,
     # use os.environ["LOCAL_RANK"]
     local_rank = None
     if "local_rank" in run_opts:
         local_rank = run_opts["local_rank"]
@@ -424,18 +417,18 @@
 
         # Arguments passed via the run opts dictionary
         run_opt_defaults = {
             "debug": False,
             "debug_batches": 2,
             "debug_epochs": 2,
             "device": "cpu",
-            "data_parallel_count": -1,
             "data_parallel_backend": False,
             "distributed_launch": False,
             "distributed_backend": "nccl",
+            "find_unused_parameters": False,
             "jit_module_keys": None,
             "auto_mix_prec": False,
             "max_grad_norm": 5.0,
             "nonfinite_patience": 3,
             "noprogressbar": False,
             "ckpt_interval_minutes": 0,
         }
@@ -453,19 +446,35 @@
                     logger.info(
                         "Info: " + arg + " arg from hparam file is used"
                     )
                     setattr(self, arg, hparams[arg])
                 else:
                     setattr(self, arg, default)
 
+        # Check Python version
+        if not (
+            sys.version_info.major == PYTHON_VERSION_MAJOR
+            and sys.version_info.minor >= PYTHON_VERSION_MINOR
+        ):
+            logger.warn(
+                "Detected Python "
+                + str(sys.version_info.major)
+                + "."
+                + str(sys.version_info.minor)
+                + ". We suggest using SpeechBrain with Python >="
+                + str(PYTHON_VERSION_MAJOR)
+                + "."
+                + str(PYTHON_VERSION_MINOR)
+            )
+
         if self.data_parallel_backend and self.distributed_launch:
             sys.exit(
                 "To use data_parallel backend, start your script with:\n\t"
                 "python experiment.py hyperparams.yaml "
-                "--data_parallel_backend=True --data_parallel_count=2"
+                "--data_parallel_backend=True"
                 "To use DDP backend, start your script with:\n\t"
                 "python -m torch.distributed.lunch [args]\n"
                 "experiment.py hyperparams.yaml --distributed_launch=True "
                 "--distributed_backend=nccl"
             )
 
         # Switch to the right context
@@ -1090,31 +1099,26 @@
     def _wrap_distributed(self):
         """Wrap modules with distributed wrapper when requested."""
         if not self.distributed_launch and not self.data_parallel_backend:
             return
         elif self.distributed_launch:
             for name, module in self.modules.items():
                 if any(p.requires_grad for p in module.parameters()):
-                    # for ddp, all module must run on same GPU
                     module = SyncBatchNorm.convert_sync_batchnorm(module)
-                    module = DDP(module, device_ids=[self.device])
+                    module = DDP(
+                        module,
+                        device_ids=[self.device],
+                        find_unused_parameters=self.find_unused_parameters,
+                    )
                     self.modules[name] = module
         else:
             # data_parallel_backend
             for name, module in self.modules.items():
                 if any(p.requires_grad for p in module.parameters()):
-                    # if distributed_count = -1 then use all gpus
-                    # otherwise, specify the set of gpu to use
-                    if self.data_parallel_count == -1:
-                        module = DP(module)
-                    else:
-                        module = DP(
-                            module,
-                            [i for i in range(self.data_parallel_count)],
-                        )
+                    module = DP(module)
                     self.modules[name] = module
 
     def evaluate(
         self,
         test_set,
         max_key=None,
         min_key=None,
```

### Comparing `speechbrain-0.5.8/speechbrain/dataio/batch.py` & `speechbrain-0.5.9/speechbrain/dataio/batch.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/dataio/dataio.py` & `speechbrain-0.5.9/speechbrain/dataio/dataio.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
     if not isinstance(files, list):
         files = [files]
 
     waveforms = []
     start = waveforms_obj.get("start", 0)
     # Default stop to start -> if not specified, num_frames becomes 0,
     # which is the torchaudio default
-    stop = waveforms_obj.get("stop", start)
+    stop = waveforms_obj.get("stop", start - 1)
     num_frames = stop - start
     for f in files:
         audio, fs = torchaudio.load(
             f, num_frames=num_frames, frame_offset=start
         )
         waveforms.append(audio)
```

### Comparing `speechbrain-0.5.8/speechbrain/dataio/dataloader.py` & `speechbrain-0.5.9/speechbrain/dataio/dataloader.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/dataio/dataset.py` & `speechbrain-0.5.9/speechbrain/dataio/dataset.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/dataio/encoder.py` & `speechbrain-0.5.9/speechbrain/dataio/encoder.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/dataio/legacy.py` & `speechbrain-0.5.9/speechbrain/dataio/legacy.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/dataio/preprocess.py` & `speechbrain-0.5.9/speechbrain/dataio/preprocess.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/dataio/sampler.py` & `speechbrain-0.5.9/speechbrain/dataio/sampler.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/dataio/wer.py` & `speechbrain-0.5.9/speechbrain/dataio/wer.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/decoders/ctc.py` & `speechbrain-0.5.9/speechbrain/decoders/ctc.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/decoders/seq2seq.py` & `speechbrain-0.5.9/speechbrain/decoders/seq2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,17 @@
         (eos_indices,) = torch.nonzero(is_eos, as_tuple=True)
 
         # Store the hypothesis and their scores when reaching eos.
         if eos_indices.shape[0] > 0:
             for index in eos_indices:
                 # convert to int
                 index = index.item()
-                batch_id = index // self.beam_size
+                batch_id = torch.div(
+                    index, self.beam_size, rounding_mode="floor"
+                )
                 if len(hyps_and_scores[batch_id]) == self.beam_size:
                     continue
                 hyp = alived_seq[index, :]
                 log_probs = alived_log_probs[index, :]
                 final_scores = scores[index] + self.length_rewarding * (
                     timesteps + 1
                 )
@@ -700,15 +702,15 @@
 
             # recover the length normalization
             if self.length_normalization:
                 sequence_scores = sequence_scores * (t + 1)
 
             # The index of which beam the current top-K output came from in (t-1) timesteps.
             predecessors = (
-                candidates // vocab_size
+                torch.div(candidates, vocab_size, rounding_mode="floor")
                 + self.beam_offset.unsqueeze(1).expand_as(candidates)
             ).view(batch_size * self.beam_size)
 
             # Permute the memory to synchoronize with the output.
             memory = self.permute_mem(memory, index=predecessors)
             if self.lm_weight > 0:
                 lm_memory = self.permute_lm_mem(lm_memory, index=predecessors)
```

### Comparing `speechbrain-0.5.8/speechbrain/decoders/transducer.py` & `speechbrain-0.5.9/speechbrain/decoders/transducer.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lm/arpa.py` & `speechbrain-0.5.9/speechbrain/lm/arpa.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lm/counting.py` & `speechbrain-0.5.9/speechbrain/lm/counting.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lm/ngram.py` & `speechbrain-0.5.9/speechbrain/lm/ngram.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/augment.py` & `speechbrain-0.5.9/speechbrain/lobes/augment.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,19 +287,18 @@
 
         Arguments
         ---------
         waveforms : torch.Tensor
             The waveforms to distort
         """
         # Augmentation
-        if self.training:
-            with torch.no_grad():
-                waveforms = self.speed_perturb(waveforms)
-                waveforms = self.drop_freq(waveforms)
-                waveforms = self.drop_chunk(waveforms, lengths)
+        with torch.no_grad():
+            waveforms = self.speed_perturb(waveforms)
+            waveforms = self.drop_freq(waveforms)
+            waveforms = self.drop_chunk(waveforms, lengths)
 
         return waveforms
 
 
 class EnvCorrupt(torch.nn.Module):
     """Environmental Corruptions for speech signals: noise, reverb, babble.
 
@@ -412,25 +411,24 @@
 
         Arguments
         ---------
         waveforms : torch.Tensor
             The waveforms to distort.
         """
         # Augmentation
-        if self.training:
-            with torch.no_grad():
-                if hasattr(self, "add_reverb"):
-                    try:
-                        waveforms = self.add_reverb(waveforms, lengths)
-                    except Exception:
-                        pass
-                if hasattr(self, "add_babble"):
-                    waveforms = self.add_babble(waveforms, lengths)
-                if hasattr(self, "add_noise"):
-                    waveforms = self.add_noise(waveforms, lengths)
+        with torch.no_grad():
+            if hasattr(self, "add_reverb"):
+                try:
+                    waveforms = self.add_reverb(waveforms, lengths)
+                except Exception:
+                    pass
+            if hasattr(self, "add_babble"):
+                waveforms = self.add_babble(waveforms, lengths)
+            if hasattr(self, "add_noise"):
+                waveforms = self.add_noise(waveforms, lengths)
 
         return waveforms
 
 
 def _prepare_openrir(folder, reverb_csv, noise_csv, max_noise_len):
     """Prepare the openrir dataset for adding reverb and noises.
```

### Comparing `speechbrain-0.5.8/speechbrain/lobes/features.py` & `speechbrain-0.5.9/speechbrain/lobes/features.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/CRDNN.py` & `speechbrain-0.5.9/speechbrain/lobes/models/CRDNN.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/ContextNet.py` & `speechbrain-0.5.9/speechbrain/lobes/models/ContextNet.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/ECAPA_TDNN.py` & `speechbrain-0.5.9/speechbrain/lobes/models/ECAPA_TDNN.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/ESPnetVGG.py` & `speechbrain-0.5.9/speechbrain/lobes/models/ESPnetVGG.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/MetricGAN.py` & `speechbrain-0.5.9/speechbrain/lobes/models/MetricGAN.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/RNNLM.py` & `speechbrain-0.5.9/speechbrain/lobes/models/RNNLM.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/VanillaNN.py` & `speechbrain-0.5.9/speechbrain/lobes/models/VanillaNN.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/Xvector.py` & `speechbrain-0.5.9/speechbrain/lobes/models/Xvector.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/conv_tasnet.py` & `speechbrain-0.5.9/speechbrain/lobes/models/conv_tasnet.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/convolution.py` & `speechbrain-0.5.9/speechbrain/lobes/models/convolution.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/dual_path.py` & `speechbrain-0.5.9/speechbrain/lobes/models/dual_path.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/fairseq_wav2vec.py` & `speechbrain-0.5.9/speechbrain/lobes/models/fairseq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/huggingface_wav2vec.py` & `speechbrain-0.5.9/speechbrain/lobes/models/huggingface_wav2vec.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/transformer/Transformer.py` & `speechbrain-0.5.9/speechbrain/lobes/models/transformer/Transformer.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/transformer/TransformerASR.py` & `speechbrain-0.5.9/speechbrain/lobes/models/transformer/TransformerASR.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/transformer/TransformerLM.py` & `speechbrain-0.5.9/speechbrain/lobes/models/transformer/TransformerLM.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/transformer/TransformerSE.py` & `speechbrain-0.5.9/speechbrain/lobes/models/transformer/TransformerSE.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/lobes/models/transformer/conformer.py` & `speechbrain-0.5.9/speechbrain/lobes/models/transformer/conformer.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/log-config.yaml` & `speechbrain-0.5.9/speechbrain/log-config.yaml`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/CNN.py` & `speechbrain-0.5.9/speechbrain/nnet/CNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -1043,22 +1043,22 @@
     ---------
     L_in : int
     stride: int
     kernel_size : int
     dilation : int
     """
     if stride > 1:
-        n_steps = math.ceil(((L_in - kernel_size * dilation) / stride) + 1)
-        L_out = stride * (n_steps - 1) + kernel_size * dilation
-        padding = [kernel_size // 2, kernel_size // 2]
+        half_kernel = torch.div(kernel_size, 2, rounding_mode="floor")
+        padding = [half_kernel, half_kernel]
 
     else:
-        L_out = (L_in - dilation * (kernel_size - 1) - 1) // stride + 1
+        tot_padding = dilation * (kernel_size - 1)
+        half_padding = torch.div(tot_padding, 2, rounding_mode="floor")
 
-        padding = [(L_in - L_out) // 2, (L_in - L_out) // 2]
+        padding = [half_padding, half_padding]
     return padding
 
 
 def get_padding_elem_transposed(
     L_out: int,
     L_in: int,
     stride: int,
```

### Comparing `speechbrain-0.5.8/speechbrain/nnet/RNN.py` & `speechbrain-0.5.9/speechbrain/nnet/RNN.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/activations.py` & `speechbrain-0.5.9/speechbrain/nnet/activations.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/attention.py` & `speechbrain-0.5.9/speechbrain/nnet/attention.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_CNN.py` & `speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_CNN.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_RNN.py` & `speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_RNN.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_linear.py` & `speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_linear.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_normalization.py` & `speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_normalization.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/complex_networks/c_ops.py` & `speechbrain-0.5.9/speechbrain/nnet/complex_networks/c_ops.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/containers.py` & `speechbrain-0.5.9/speechbrain/nnet/containers.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/dropout.py` & `speechbrain-0.5.9/speechbrain/nnet/dropout.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/embedding.py` & `speechbrain-0.5.9/speechbrain/nnet/embedding.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/linear.py` & `speechbrain-0.5.9/speechbrain/nnet/linear.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/loss/stoi_loss.py` & `speechbrain-0.5.9/speechbrain/nnet/loss/stoi_loss.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/loss/transducer_loss.py` & `speechbrain-0.5.9/speechbrain/nnet/loss/transducer_loss.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/losses.py` & `speechbrain-0.5.9/speechbrain/nnet/losses.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/normalization.py` & `speechbrain-0.5.9/speechbrain/nnet/normalization.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/pooling.py` & `speechbrain-0.5.9/speechbrain/nnet/pooling.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_CNN.py` & `speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_CNN.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_RNN.py` & `speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_RNN.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_linear.py` & `speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_linear.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_normalization.py` & `speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_normalization.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/quaternion_networks/q_ops.py` & `speechbrain-0.5.9/speechbrain/nnet/quaternion_networks/q_ops.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/schedulers.py` & `speechbrain-0.5.9/speechbrain/nnet/schedulers.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/nnet/transducer/transducer_joint.py` & `speechbrain-0.5.9/speechbrain/nnet/transducer/transducer_joint.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/pretrained/fetching.py` & `speechbrain-0.5.9/speechbrain/pretrained/fetching.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/pretrained/interfaces.py` & `speechbrain-0.5.9/speechbrain/pretrained/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         for mod in self.MODULES_NEEDED:
             if mod not in modules:
                 raise ValueError(f"Need modules['{mod}']")
 
         # Check MODULES_NEEDED and HPARAMS_NEEDED and
         # make hyperparams available with dot notation
         if self.HPARAMS_NEEDED and hparams is None:
-            raise ValueError(f"Need to provide hparams dict.")
+            raise ValueError("Need to provide hparams dict.")
         if hparams is not None:
             # Also first check that all required params are found:
             for hp in self.HPARAMS_NEEDED:
                 if hp not in hparams:
                     raise ValueError(f"Need hparams['{hp}']")
             self.hparams = SimpleNamespace(**hparams)
```

### Comparing `speechbrain-0.5.8/speechbrain/processing/NMF.py` & `speechbrain-0.5.9/speechbrain/processing/NMF.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/processing/PLDA_LDA.py` & `speechbrain-0.5.9/speechbrain/processing/PLDA_LDA.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/processing/decomposition.py` & `speechbrain-0.5.9/speechbrain/processing/decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,23 +82,23 @@
         b = torch.zeros(a.shape, dtype=a.dtype, device=a.device)
         ids = torch.triu_indices(C, C)
         b[..., 0, ids[0] == ids[1]] = 1.0
 
     bsh = f(b)
 
     # Performing the Cholesky decomposition
-    lsh = torch.cholesky(bsh)
+    lsh = torch.linalg.cholesky(bsh)
     lsh_inv = torch.inverse(lsh)
     lsh_inv_T = torch.transpose(lsh_inv, D - 2, D - 1)
 
     # Computing the matrix C
     csh = torch.matmul(lsh_inv, torch.matmul(ash, lsh_inv_T))
 
     # Performing the eigenvalue decomposition
-    es, ysh = torch.symeig(csh, eigenvectors=True)
+    es, ysh = torch.linalg.eigh(csh, UPLO="U")
 
     # Collecting the eigenvalues
     dsh = torch.zeros(
         a.shape[slice(0, D - 2)] + (2 * C, 2 * C),
         dtype=a.dtype,
         device=a.device,
     )
@@ -162,15 +162,15 @@
     # Computing As * As_T
     ash = f(a)
     ash_T = torch.transpose(ash, -2, -1)
 
     ash_mm_ash_T = torch.matmul(ash, ash_T)
 
     # Finding the eigenvectors and eigenvalues
-    es, ush = torch.symeig(ash_mm_ash_T, eigenvectors=True)
+    es, ush = torch.linalg.eigh(ash_mm_ash_T, UPLO="U")
 
     # Collecting the eigenvalues
     dsh = torch.zeros(ush.shape, dtype=es.dtype, device=es.device)
     dsh[..., range(0, 2 * C), range(0, 2 * C)] = torch.sqrt(es)
 
     # Converting the block matrices to full complex matrices
     us = ginv(ush)
```

### Comparing `speechbrain-0.5.8/speechbrain/processing/diarization.py` & `speechbrain-0.5.9/speechbrain/processing/diarization.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,16 +353,16 @@
         to the largest connected components of the given query node.
     """
 
     n_node = graph.shape[0]
     if sparse.issparse(graph):
         # speed up row-wise access to boolean connection mask
         graph = graph.tocsr()
-    connected_nodes = np.zeros(n_node, dtype=np.bool)
-    nodes_to_explore = np.zeros(n_node, dtype=np.bool)
+    connected_nodes = np.zeros(n_node, dtype=bool)
+    nodes_to_explore = np.zeros(n_node, dtype=bool)
     nodes_to_explore[node_id] = True
     for _ in range(n_node):
         last_num_component = connected_nodes.sum()
         np.logical_or(connected_nodes, nodes_to_explore, out=connected_nodes)
         if last_num_component >= connected_nodes.sum():
             break
         indices = np.where(nodes_to_explore)[0]
```

### Comparing `speechbrain-0.5.8/speechbrain/processing/features.py` & `speechbrain-0.5.9/speechbrain/processing/features.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/processing/multi_mic.py` & `speechbrain-0.5.9/speechbrain/processing/multi_mic.py`

 * *Files 0% similar despite different names*

```diff
@@ -764,15 +764,15 @@
         """
 
         # Get useful dimensions
         n_fft = xxs.shape[2]
 
         # If no tdoa specified, cover the whole frame
         if tdoa_max is None:
-            tdoa_max = n_fft // 2
+            tdoa_max = torch.div(n_fft, 2, rounding_mode="floor")
 
         # Splitting the GCC-PHAT values to search in the range
         slice_1 = xxs[..., 0:tdoa_max, :]
         slice_2 = xxs[..., -tdoa_max:, :]
 
         xxs_sliced = torch.cat((slice_1, slice_2), 2)
 
@@ -1492,15 +1492,17 @@
             subtrs_scalar, return_inverse=True
         )
 
         unique_values = torch.zeros(
             (unique_scalar.shape[0], 2), dtype=unique_scalar.dtype
         )
 
-        unique_values[:, 0] = torch.floor_divide(unique_scalar, index_max + 1)
+        unique_values[:, 0] = torch.div(
+            unique_scalar, index_max + 1, rounding_mode="floor"
+        )
         unique_values[:, 1] = unique_scalar - unique_values[:, 0] * (
             index_max + 1
         )
 
         trs = torch.transpose(torch.reshape(unique_indices, (3, -1)), 0, 1)
 
         pts = pts[unique_values[:, 0], :] + pts[unique_values[:, 1], :]
```

### Comparing `speechbrain-0.5.8/speechbrain/processing/signal_processing.py` & `speechbrain-0.5.9/speechbrain/processing/signal_processing.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/processing/speech_augmentation.py` & `speechbrain-0.5.9/speechbrain/processing/speech_augmentation.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/tokenizers/SentencePiece.py` & `speechbrain-0.5.9/speechbrain/tokenizers/SentencePiece.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/Accuracy.py` & `speechbrain-0.5.9/speechbrain/utils/Accuracy.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/DER.py` & `speechbrain-0.5.9/speechbrain/utils/DER.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/callchains.py` & `speechbrain-0.5.9/speechbrain/utils/callchains.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/checkpoints.py` & `speechbrain-0.5.9/speechbrain/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/data_pipeline.py` & `speechbrain-0.5.9/speechbrain/utils/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/data_utils.py` & `speechbrain-0.5.9/speechbrain/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/depgraph.py` & `speechbrain-0.5.9/speechbrain/utils/depgraph.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/distributed.py` & `speechbrain-0.5.9/speechbrain/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/edit_distance.py` & `speechbrain-0.5.9/speechbrain/utils/edit_distance.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/epoch_loop.py` & `speechbrain-0.5.9/speechbrain/utils/epoch_loop.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/logger.py` & `speechbrain-0.5.9/speechbrain/utils/logger.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/metric_stats.py` & `speechbrain-0.5.9/speechbrain/utils/metric_stats.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/parameter_transfer.py` & `speechbrain-0.5.9/speechbrain/utils/parameter_transfer.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/superpowers.py` & `speechbrain-0.5.9/speechbrain/utils/superpowers.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain/utils/train_logger.py` & `speechbrain-0.5.9/speechbrain/utils/train_logger.py`

 * *Files identical despite different names*

### Comparing `speechbrain-0.5.8/speechbrain.egg-info/PKG-INFO` & `speechbrain-0.5.9/speechbrain.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechbrain
-Version: 0.5.8
+Version: 0.5.9
 Summary: All-in-one speech toolkit in pure Python and Pytorch
 Home-page: https://speechbrain.github.io/
 Author: Mirco Ravanelli & Others
 Author-email: speechbrain@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -165,8 +165,24 @@
 - General information can be found on the [website](https://speechbrain.github.io).
 - We offer many tutorials, you can start out from the [basic ones](https://speechbrain.github.io/tutorial_basics.html) about SpeechBrain basic functionalities and building blocks. We provide also more advanced tutorials (e.g SpeechBrain advanced, signal processing ...). You can browse them via the Tutorials drop down menu on [SpeechBrain website](https://speechbrain.github.io) in the upper right.
 - Details on the SpeechBrain API, how to contribute, and the code are given in the [documentation](https://speechbrain.readthedocs.io/en/latest/index.html).
 
 # License
 SpeechBrain is released under the Apache License, version 2.0. The Apache license is a popular BSD-like license. SpeechBrain can be redistributed for free, even for commercial purposes, although you can not take off the license headers (and under some circumstances, you may have to distribute a license document). Apache is not a viral license like the GPL, which forces you to release your modifications to the source code. Also note that this project has no connection to the Apache Foundation, other than that we use the same license terms.
 
+# Citing SpeechBrain
+Please, cite SpeechBrain if you use it for your research or business.
+
+```bibtex
+@misc{speechbrain,
+  title={{SpeechBrain}: A General-Purpose Speech Toolkit},
+  author={Mirco Ravanelli and Titouan Parcollet and Peter Plantinga and Aku Rouhe and Samuele Cornell and Loren Lugosch and Cem Subakan and Nauman Dawalatabad and Abdelwahab Heba and Jianyuan Zhong and Ju-Chieh Chou and Sung-Lin Yeh and Szu-Wei Fu and Chien-Feng Liao and Elena Rastorgueva and François Grondin and William Aris and Hwidong Na and Yan Gao and Renato De Mori and Yoshua Bengio},
+  year={2021},
+  eprint={2106.04624},
+  archivePrefix={arXiv},
+  primaryClass={eess.AS},
+  note={arXiv:2106.04624}
+}
+```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `speechbrain-0.5.8/speechbrain.egg-info/SOURCES.txt` & `speechbrain-0.5.9/speechbrain.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 speechbrain/processing/signal_processing.py
 speechbrain/processing/speech_augmentation.py
 speechbrain/tokenizers/SentencePiece.py
 speechbrain/tokenizers/__init__.py
 speechbrain/utils/Accuracy.py
 speechbrain/utils/DER.py
 speechbrain/utils/__init__.py
+speechbrain/utils/bleu.py
 speechbrain/utils/callchains.py
 speechbrain/utils/checkpoints.py
 speechbrain/utils/data_pipeline.py
 speechbrain/utils/data_utils.py
 speechbrain/utils/depgraph.py
 speechbrain/utils/distributed.py
 speechbrain/utils/edit_distance.py
```

