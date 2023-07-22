# Comparing `tmp/wow_ai_mms-0.0.9.tar.gz` & `tmp/wow_ai_mms-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_mms-0.0.9.tar", max compression
+gzip compressed data, was "wow_ai_mms-0.1.0.tar", max compression
```

## Comparing `wow_ai_mms-0.0.9.tar` & `wow_ai_mms-0.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    17529 2023-07-22 09:49:11.755219 wow_ai_mms-0.0.9/LICENSE
--rw-r--r--   0        0        0     4825 2023-07-22 09:49:11.756724 wow_ai_mms-0.0.9/README.md
--rw-r--r--   0        0        0      262 2023-07-22 11:09:46.596131 wow_ai_mms-0.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-22 09:49:11.836893 wow_ai_mms-0.0.9/wow_ai_mms/__init__.py
--rw-r--r--   0        0        0      630 2023-07-22 09:49:11.837789 wow_ai_mms-0.0.9/wow_ai_mms/_logger.py
--rw-r--r--   0        0        0     5845 2023-07-22 09:49:11.838755 wow_ai_mms-0.0.9/wow_ai_mms/constants.py
--rw-r--r--   0        0        0     3264 2023-07-22 09:49:11.841220 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/MODEL_CARD.md
--rw-r--r--   0        0        0    13987 2023-07-22 09:49:11.842872 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/README.md
--rw-r--r--   0        0        0      697 2023-07-22 09:49:11.845855 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/asr/config/infer_common.yaml
--rw-r--r--   0        0        0      671 2023-07-22 09:49:11.846862 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/asr/infer/example_infer_adapter.sh
--rw-r--r--   0        0        0     2835 2023-07-22 09:49:11.848026 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/asr/infer/mms_infer.py
--rw-r--r--   0        0        0     3366 2023-07-22 09:49:11.849095 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/README.md
--rw-r--r--   0        0        0     6095 2023-07-22 09:49:11.849977 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/align_and_segment.py
--rw-r--r--   0        0        0     5656 2023-07-22 09:49:11.851076 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/align_utils.py
--rw-r--r--   0        0        0     6532 2023-07-22 09:49:11.852153 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/norm_config.py
--rw-r--r--   0        0        0     6069 2023-07-22 09:49:11.853057 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/punctuations.lst
--rw-r--r--   0        0        0     2779 2023-07-22 09:49:11.854211 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/text_normalization.py
--rw-r--r--   0        0        0     7071 2023-07-22 09:49:11.855224 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/lid/infer.py
--rw-r--r--   0        0        0      808 2023-07-22 09:49:11.856391 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/misc/get_sample_size.py
--rw-r--r--   0        0        0     5802 2023-07-22 09:49:11.857738 wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/tts/infer.py
--rw-r--r--   0        0        0        1 2023-07-22 09:49:11.858761 wow_ai_mms-0.0.9/wow_ai_mms/models/__init__.py
--rw-r--r--   0        0        0     7678 2023-07-22 09:49:11.859772 wow_ai_mms-0.0.9/wow_ai_mms/models/alignment.py
--rw-r--r--   0        0        0     9501 2023-07-22 09:49:11.862229 wow_ai_mms-0.0.9/wow_ai_mms/models/asr.py
--rw-r--r--   0        0        0     5706 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/README.md
--rw-r--r--   0        0        0       48 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0     5870 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/criterions/ASG_loss.py
--rw-r--r--   0        0        0      510 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/criterions/__init__.py
--rw-r--r--   0        0        0     5372 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/criterions/cross_entropy_acc.py
--rw-r--r--   0        0        0      248 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/data/__init__.py
--rw-r--r--   0        0        0     3955 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/data/asr_dataset.py
--rw-r--r--   0        0        0     4796 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/data/collaters.py
--rw-r--r--   0        0        0     3429 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/data/data_utils.py
--rw-r--r--   0        0        0     1970 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/data/replabels.py
--rw-r--r--   0        0        0    14677 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/infer.py
--rw-r--r--   0        0        0        0 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/kaldi/__init__.py
--rw-r--r--   0        0        0     2866 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/kaldi/add-self-loop-simple.cc
--rw-r--r--   0        0        0      109 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/kaldi/config/kaldi_initializer.yaml
--rw-r--r--   0        0        0     8265 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/kaldi/kaldi_decoder.py
--rw-r--r--   0        0        0    23441 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/kaldi/kaldi_initializer.py
--rw-r--r--   0        0        0      276 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/models/__init__.py
--rw-r--r--   0        0        0    37260 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/models/vggtransformer.py
--rw-r--r--   0        0        0     6078 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/models/w2l_conv_glu_enc.py
--rw-r--r--   0        0        0     1107 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/README.md
--rw-r--r--   0        0        0        0 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/__init__.py
--rw-r--r--   0        0        0      673 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/hydra/sweeper/ax.yaml
--rw-r--r--   0        0        0      676 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/hydra/sweeper/ax_sil.yaml
--rw-r--r--   0        0        0      551 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/infer.yaml
--rw-r--r--   0        0        0      765 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/run_config/fb_slurm_1.yaml
--rw-r--r--   0        0        0      738 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/run_config/fb_slurm_2g.yaml
--rw-r--r--   0        0        0        0 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/__init__.py
--rw-r--r--   0        0        0     2093 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/base_decoder.py
--rw-r--r--   0        0        0      944 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/decoder.py
--rw-r--r--   0        0        0     2004 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/decoder_config.py
--rw-r--r--   0        0        0    14870 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/flashlight_decoder.py
--rw-r--r--   0        0        0      641 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/viterbi_decoder.py
--rw-r--r--   0        0        0    17857 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/infer.py
--rw-r--r--   0        0        0      273 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/tasks/__init__.py
--rw-r--r--   0        0        0     5397 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/tasks/speech_recognition.py
--rw-r--r--   0        0        0    11842 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/utils/wer_utils.py
--rw-r--r--   0        0        0    17396 2023-06-23 17:31:52.000000 wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/w2l_decoder.py
--rw-r--r--   0        0        0     6857 2023-07-22 09:49:11.863142 wow_ai_mms-0.0.9/wow_ai_mms/models/tts.py
--rw-r--r--   0        0        0     4332 2023-07-22 09:49:11.863901 wow_ai_mms-0.0.9/wow_ai_mms/utils.py
--rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 wow_ai_mms-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    17529 2023-07-22 09:49:11.755219 wow_ai_mms-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4825 2023-07-22 09:49:11.756724 wow_ai_mms-0.1.0/README.md
+-rw-r--r--   0        0        0      262 2023-07-22 11:14:27.917372 wow_ai_mms-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-22 09:49:11.836893 wow_ai_mms-0.1.0/wow_ai_mms/__init__.py
+-rw-r--r--   0        0        0      630 2023-07-22 09:49:11.837789 wow_ai_mms-0.1.0/wow_ai_mms/_logger.py
+-rw-r--r--   0        0        0     5845 2023-07-22 09:49:11.838755 wow_ai_mms-0.1.0/wow_ai_mms/constants.py
+-rw-r--r--   0        0        0     3264 2023-07-22 09:49:11.841220 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/MODEL_CARD.md
+-rw-r--r--   0        0        0    13987 2023-07-22 09:49:11.842872 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/README.md
+-rw-r--r--   0        0        0      697 2023-07-22 09:49:11.845855 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/asr/config/infer_common.yaml
+-rw-r--r--   0        0        0      671 2023-07-22 09:49:11.846862 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/asr/infer/example_infer_adapter.sh
+-rw-r--r--   0        0        0     2835 2023-07-22 09:49:11.848026 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/asr/infer/mms_infer.py
+-rw-r--r--   0        0        0     3366 2023-07-22 09:49:11.849095 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/README.md
+-rw-r--r--   0        0        0     6095 2023-07-22 09:49:11.849977 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/align_and_segment.py
+-rw-r--r--   0        0        0     5656 2023-07-22 09:49:11.851076 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/align_utils.py
+-rw-r--r--   0        0        0     6532 2023-07-22 09:49:11.852153 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/norm_config.py
+-rw-r--r--   0        0        0     6069 2023-07-22 09:49:11.853057 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/punctuations.lst
+-rw-r--r--   0        0        0     2779 2023-07-22 09:49:11.854211 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/text_normalization.py
+-rw-r--r--   0        0        0     7071 2023-07-22 09:49:11.855224 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/lid/infer.py
+-rw-r--r--   0        0        0      808 2023-07-22 09:49:11.856391 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/misc/get_sample_size.py
+-rw-r--r--   0        0        0     5802 2023-07-22 09:49:11.857738 wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/tts/infer.py
+-rw-r--r--   0        0        0        1 2023-07-22 09:49:11.858761 wow_ai_mms-0.1.0/wow_ai_mms/models/__init__.py
+-rw-r--r--   0        0        0     7678 2023-07-22 09:49:11.859772 wow_ai_mms-0.1.0/wow_ai_mms/models/alignment.py
+-rw-r--r--   0        0        0     9492 2023-07-22 11:14:12.875761 wow_ai_mms-0.1.0/wow_ai_mms/models/asr.py
+-rw-r--r--   0        0        0     5706 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/README.md
+-rw-r--r--   0        0        0       48 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     5870 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/criterions/ASG_loss.py
+-rw-r--r--   0        0        0      510 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/criterions/__init__.py
+-rw-r--r--   0        0        0     5372 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/criterions/cross_entropy_acc.py
+-rw-r--r--   0        0        0      248 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/data/__init__.py
+-rw-r--r--   0        0        0     3955 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/data/asr_dataset.py
+-rw-r--r--   0        0        0     4796 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/data/collaters.py
+-rw-r--r--   0        0        0     3429 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/data/data_utils.py
+-rw-r--r--   0        0        0     1970 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/data/replabels.py
+-rw-r--r--   0        0        0    14677 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/infer.py
+-rw-r--r--   0        0        0        0 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/kaldi/__init__.py
+-rw-r--r--   0        0        0     2866 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/kaldi/add-self-loop-simple.cc
+-rw-r--r--   0        0        0      109 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/kaldi/config/kaldi_initializer.yaml
+-rw-r--r--   0        0        0     8265 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/kaldi/kaldi_decoder.py
+-rw-r--r--   0        0        0    23441 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/kaldi/kaldi_initializer.py
+-rw-r--r--   0        0        0      276 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/models/__init__.py
+-rw-r--r--   0        0        0    37260 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/models/vggtransformer.py
+-rw-r--r--   0        0        0     6078 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/models/w2l_conv_glu_enc.py
+-rw-r--r--   0        0        0     1107 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/hydra/sweeper/ax.yaml
+-rw-r--r--   0        0        0      676 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/hydra/sweeper/ax_sil.yaml
+-rw-r--r--   0        0        0      551 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/infer.yaml
+-rw-r--r--   0        0        0      765 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/run_config/fb_slurm_1.yaml
+-rw-r--r--   0        0        0      738 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/run_config/fb_slurm_2g.yaml
+-rw-r--r--   0        0        0        0 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/__init__.py
+-rw-r--r--   0        0        0     2093 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/base_decoder.py
+-rw-r--r--   0        0        0      944 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/decoder.py
+-rw-r--r--   0        0        0     2004 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/decoder_config.py
+-rw-r--r--   0        0        0    14870 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/flashlight_decoder.py
+-rw-r--r--   0        0        0      641 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/viterbi_decoder.py
+-rw-r--r--   0        0        0    17857 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/infer.py
+-rw-r--r--   0        0        0      273 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/tasks/__init__.py
+-rw-r--r--   0        0        0     5397 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/tasks/speech_recognition.py
+-rw-r--r--   0        0        0    11842 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/utils/wer_utils.py
+-rw-r--r--   0        0        0    17396 2023-06-23 17:31:52.000000 wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/w2l_decoder.py
+-rw-r--r--   0        0        0     6857 2023-07-22 09:49:11.863142 wow_ai_mms-0.1.0/wow_ai_mms/models/tts.py
+-rw-r--r--   0        0        0     4332 2023-07-22 09:49:11.863901 wow_ai_mms-0.1.0/wow_ai_mms/utils.py
+-rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 wow_ai_mms-0.1.0/PKG-INFO
```

### Comparing `wow_ai_mms-0.0.9/LICENSE` & `wow_ai_mms-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/README.md` & `wow_ai_mms-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/_logger.py` & `wow_ai_mms-0.1.0/wow_ai_mms/_logger.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/constants.py` & `wow_ai_mms-0.1.0/wow_ai_mms/constants.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/MODEL_CARD.md` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/MODEL_CARD.md`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/README.md` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/asr/config/infer_common.yaml` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/asr/config/infer_common.yaml`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/asr/infer/example_infer_adapter.sh` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/asr/infer/example_infer_adapter.sh`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/asr/infer/mms_infer.py` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/asr/infer/mms_infer.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/README.md` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/align_and_segment.py` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/align_and_segment.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/align_utils.py` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/align_utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/norm_config.py` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/norm_config.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/punctuations.lst` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/punctuations.lst`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/data_prep/text_normalization.py` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/data_prep/text_normalization.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/lid/infer.py` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/lid/infer.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/misc/get_sample_size.py` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/misc/get_sample_size.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/examples/mms/tts/infer.py` & `wow_ai_mms-0.1.0/wow_ai_mms/examples/mms/tts/infer.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/alignment.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/alignment.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/asr.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         cwd = os.getcwd()
         # clone Fairseq
         wow_ai_mms_utils.clone(constants.FAIRSEQ_URL, constants.FAIRSEQ_DIR)
         fairseq_dir = str(constants.FAIRSEQ_DIR.resolve())
         sys.path.append(fairseq_dir)
         os.chdir(fairseq_dir)
         # import
-        from examples.speech_recognition.new.infer import hydra_main
+        from speech_recognition.new.infer import hydra_main
         try:
             from fairseq.data.data_utils_fast import (
                 batch_by_size_fn,
                 batch_by_size_vec,
                 batch_fixed_shapes_fast,
             )
         except ImportError:
```

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/README.md` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/criterions/ASG_loss.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/criterions/ASG_loss.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/criterions/cross_entropy_acc.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/criterions/cross_entropy_acc.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/data/asr_dataset.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/data/asr_dataset.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/data/collaters.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/data/collaters.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/data/data_utils.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/data/replabels.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/data/replabels.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/infer.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/infer.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/kaldi/add-self-loop-simple.cc` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/kaldi/add-self-loop-simple.cc`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/kaldi/kaldi_decoder.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/kaldi/kaldi_decoder.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/kaldi/kaldi_initializer.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/kaldi/kaldi_initializer.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/models/vggtransformer.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/models/vggtransformer.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/models/w2l_conv_glu_enc.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/models/w2l_conv_glu_enc.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/README.md` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/hydra/sweeper/ax.yaml` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/hydra/sweeper/ax.yaml`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/hydra/sweeper/ax_sil.yaml` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/hydra/sweeper/ax_sil.yaml`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/infer.yaml` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/infer.yaml`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/run_config/fb_slurm_1.yaml` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/run_config/fb_slurm_1.yaml`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/conf/run_config/fb_slurm_2g.yaml` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/conf/run_config/fb_slurm_2g.yaml`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/base_decoder.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/base_decoder.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/decoder.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/decoder.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/decoder_config.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/decoder_config.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/flashlight_decoder.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/flashlight_decoder.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/decoders/viterbi_decoder.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/decoders/viterbi_decoder.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/new/infer.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/new/infer.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/tasks/speech_recognition.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/tasks/speech_recognition.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/utils/wer_utils.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/utils/wer_utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/speech_recognition/w2l_decoder.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/speech_recognition/w2l_decoder.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/models/tts.py` & `wow_ai_mms-0.1.0/wow_ai_mms/models/tts.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/wow_ai_mms/utils.py` & `wow_ai_mms-0.1.0/wow_ai_mms/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_mms-0.0.9/PKG-INFO` & `wow_ai_mms-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-mms
-Version: 0.0.9
+Version: 0.1.0
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

