# Comparing `tmp/hezar-0.17.2.tar.gz` & `tmp/hezar-0.17.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.17.2.tar", max compression
+gzip compressed data, was "hezar-0.17.3.tar", max compression
```

## Comparing `hezar-0.17.2.tar` & `hezar-0.17.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1065 2023-07-29 11:46:23.700164 hezar-0.17.2/LICENSE
--rw-r--r--   0        0        0     4309 2023-07-29 11:46:23.700164 hezar-0.17.2/README.md
--rw-r--r--   0        0        0      261 2023-07-29 11:46:23.700164 hezar-0.17.2/hezar/__init__.py
--rw-r--r--   0        0        0     5384 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/builders.py
--rw-r--r--   0        0        0    11117 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/configs.py
--rw-r--r--   0        0        0     2068 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/__init__.py
--rw-r--r--   0        0        0     6333 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4502 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3627 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      282 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1604 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1676 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1634 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11028 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/model.py
--rw-r--r--   0        0        0       67 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3971 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3666 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3809 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      118 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     3603 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/normalizer.py
--rw-r--r--   0        0        0     3333 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      231 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    19353 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8674 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2538 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2177 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    17127 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      161 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5614 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/core_utils.py
--rw-r--r--   0        0        0     3660 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1646 2023-07-29 11:46:23.704164 hezar-0.17.2/pyproject.toml
--rw-r--r--   0        0        0     6789 1970-01-01 00:00:00.000000 hezar-0.17.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-29 13:34:24.747802 hezar-0.17.3/LICENSE
+-rw-r--r--   0        0        0     4309 2023-07-29 13:34:24.747802 hezar-0.17.3/README.md
+-rw-r--r--   0        0        0      261 2023-07-29 13:34:24.747802 hezar-0.17.3/hezar/__init__.py
+-rw-r--r--   0        0        0     5384 2023-07-29 13:34:24.747802 hezar-0.17.3/hezar/builders.py
+-rw-r--r--   0        0        0    11117 2023-07-29 13:34:24.747802 hezar-0.17.3/hezar/configs.py
+-rw-r--r--   0        0        0     2068 2023-07-29 13:34:24.747802 hezar-0.17.3/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-29 13:34:24.747802 hezar-0.17.3/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6333 2023-07-29 13:34:24.747802 hezar-0.17.3/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4502 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3627 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      282 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1604 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11656 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/model.py
+-rw-r--r--   0        0        0       67 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3971 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3666 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3809 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     3603 2023-07-29 13:34:24.751802 hezar-0.17.3/hezar/preprocessors/normalizer.py
+-rw-r--r--   0        0        0     3333 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      231 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    19353 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8674 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2538 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2177 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    17330 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      161 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5614 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0     3660 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:34:24.755802 hezar-0.17.3/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1646 2023-07-29 13:34:24.755802 hezar-0.17.3/pyproject.toml
+-rw-r--r--   0        0        0     6789 1970-01-01 00:00:00.000000 hezar-0.17.3/PKG-INFO
```

### Comparing `hezar-0.17.2/LICENSE` & `hezar-0.17.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/README.md` & `hezar-0.17.3/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/builders.py` & `hezar-0.17.3/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/configs.py` & `hezar-0.17.3/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/constants.py` & `hezar-0.17.3/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/data/data_collators.py` & `hezar-0.17.3/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/data/datasets/dataset.py` & `hezar-0.17.3/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.17.3/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.17.3/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/data/utils/data_utils.py` & `hezar-0.17.3/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/embeddings/embedding.py` & `hezar-0.17.3/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/embeddings/fasttext.py` & `hezar-0.17.3/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/embeddings/word2vec.py` & `hezar-0.17.3/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/metrics/f1.py` & `hezar-0.17.3/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/metrics/metric.py` & `hezar-0.17.3/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/metrics/recall.py` & `hezar-0.17.3/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/metrics/seqeval.py` & `hezar-0.17.3/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.17.3/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.17.3/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.17.3/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.17.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.17.3/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.17.3/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/model.py` & `hezar-0.17.3/hezar/models/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,53 +147,61 @@
                 )
 
     def save(
         self,
         path: Union[str, os.PathLike],
         filename: Optional[str] = None,
         save_config: Optional[bool] = True,
+        save_preprocessor: Optional[bool] = True,
         config_filename: Optional[str] = None,
     ):
         """
         Save model weights and config to a local path
 
         Args:
             path: A local directory to save model, config, etc.
             save_config: Whether to save config along with the model or not.
+            save_preprocessor: Whether to save preprocessor(s) along with the model or not
             config_filename: Model config filename,
             filename: Model weights filename
 
         Returns:
             Path to the saved model
         """
         # save model and config to the repo
         config_filename = config_filename or self.config_filename
         filename = filename or self.model_filename
         os.makedirs(path, exist_ok=True)
         model_save_path = os.path.join(path, filename)
         torch.save(self.state_dict(), model_save_path)
         if save_config:
             self.config.save(save_dir=path, filename=config_filename)
+        if save_preprocessor:
+            if self.preprocessor is not None:
+                for p in self.preprocessor.values():
+                    p.save(path)
         return model_save_path
 
     def push_to_hub(
         self,
         repo_id: str,
         filename: Optional[str] = None,
         config_filename: Optional[str] = None,
+        push_preprocessor: Optional[bool] = True,
         commit_message: Optional[str] = None,
         private: Optional[bool] = False,
     ):
         """
         Push the model and required files to the hub
 
         Args:
             repo_id: The path (id or repo name) on the hub
             filename: Model file name
             config_filename: Config file name
+            push_preprocessor: Whether to push preprocessor(s) or not
             commit_message (str): Commit message for this push
             private (bool): Whether to create a private repo or not
         """
         config_filename = config_filename or self.config_filename
         filename = filename or self.model_filename
 
         # create remote repo
@@ -211,14 +219,19 @@
         # upload config file
         self.config.push_to_hub(
             repo_id,
             filename=config_filename,
             repo_type="model",
             commit_message=commit_message,
         )
+        # upload preprocessor(s)
+        if push_preprocessor:
+            if self.preprocessor is not None:
+                for p in self.preprocessor.values():
+                    p.push_to_hub(repo_id)
         # upload model file
         upload_file(
             path_or_fileobj=model_save_path,
             path_in_repo=filename,
             repo_id=repo_id,
             commit_message=commit_message,
         )
```

### Comparing `hezar-0.17.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.17.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.17.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.17.3/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.17.3/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.17.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.17.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.17.3/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.17.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/preprocessors/normalizer.py` & `hezar-0.17.3/hezar/preprocessors/normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/preprocessors/preprocessor.py` & `hezar-0.17.3/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.17.3/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.17.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.17.3/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.17.3/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/registry.py` & `hezar-0.17.3/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.17.3/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.17.3/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/trainers/trainer.py` & `hezar-0.17.3/hezar/trainers/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -411,61 +411,69 @@
         config_filename = config_filename or self.trainer_config_file
         subfolder = subfolder or self.trainer_subfolder
         dataset_config_file = dataset_config_file or self.dataset_config_file
 
         self.config.save(path, filename=config_filename, subfolder=subfolder)
         self.model.save(path, filename=model_filename, config_filename=model_config_filename, save_config=True)
         self.train_dataset.config.save(path, filename=dataset_config_file, subfolder=subfolder)
-        if hasattr(self.train_dataset, "tokenizer"):
-            self.train_dataset.tokenizer.save(path)
 
     def push_to_hub(
         self,
         repo_id: str,
         config_filename: str = None,
+        push_model: bool = True,
         model_filename: str = None,
         model_config_filename: str = None,
         subfolder: str = None,
         dataset_config_filename: str = None,
         commit_message: str = None,
         private: bool = False,
     ):
         """
         Push everything to the Hub
 
         Args:
             repo_id: Path to hub
             config_filename: Trainer config file name
+            push_model: Whether to push the model or not
             model_filename: Model file name
             model_config_filename: Model config file name
             subfolder: Path to Trainer files
             dataset_config_filename: Dataset config file name
             commit_message: Commit message for the push
             private: Whether to create a private repo if it doesn't exist already
         """
         config_filename = config_filename or self.trainer_config_file
         subfolder = subfolder or self.trainer_subfolder
         dataset_config_file = dataset_config_filename or self.dataset_config_file
 
         # create remote repo
         create_repo(repo_id, repo_type="model", exist_ok=True, private=private)
-        # save to tmp and prepare for push
-        cache_path = tempfile.mkdtemp()
-
-        self.save(
-            cache_path,
-            config_filename=config_filename,
-            model_filename=model_filename,
-            model_config_filename=model_config_filename,
-            subfolder=subfolder,
-            dataset_config_file=dataset_config_file,
-        )
 
         if not commit_message:
             commit_message = "Hezar: Upload training files"
 
-        upload_folder(
-            repo_id=repo_id,
-            folder_path=cache_path,
-            repo_type="model",
+        # upload train files
+        self.config.push_to_hub(
+            repo_id,
+            filename=config_filename,
+            subfolder=subfolder,
+            private=private,
             commit_message=commit_message,
         )
+        self.train_dataset.config.push_to_hub(
+            repo_id,
+            filename=dataset_config_file,
+            subfolder=subfolder,
+            private=private,
+            commit_message=commit_message
+        )
+
+        # upload model
+        if push_model:
+            self.model.push_to_hub(
+                repo_id,
+                filename=model_filename,
+                config_filename=model_config_filename,
+                commit_message=commit_message,
+                private=private,
+            )
```

### Comparing `hezar-0.17.2/hezar/trainers/trainer_utils.py` & `hezar-0.17.3/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/utils/common_utils.py` & `hezar-0.17.3/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/utils/core_utils.py` & `hezar-0.17.3/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/hezar/utils/hub_utils.py` & `hezar-0.17.3/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.2/pyproject.toml` & `hezar-0.17.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.17.2"
+version = "0.17.3"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.17.2/PKG-INFO` & `hezar-0.17.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.17.2
+Version: 0.17.3
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

