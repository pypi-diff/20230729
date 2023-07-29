# Comparing `tmp/hezar-0.17.1.tar.gz` & `tmp/hezar-0.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.17.1.tar", max compression
+gzip compressed data, was "hezar-0.17.2.tar", max compression
```

## Comparing `hezar-0.17.1.tar` & `hezar-0.17.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1065 2023-07-29 08:58:57.060990 hezar-0.17.1/LICENSE
--rw-r--r--   0        0        0     4309 2023-07-29 08:58:57.060990 hezar-0.17.1/README.md
--rw-r--r--   0        0        0      261 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/__init__.py
--rw-r--r--   0        0        0     5384 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/builders.py
--rw-r--r--   0        0        0    11117 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/configs.py
--rw-r--r--   0        0        0     2068 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/data/__init__.py
--rw-r--r--   0        0        0     6333 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4502 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3627 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      282 2023-07-29 08:58:57.060990 hezar-0.17.1/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1604 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1676 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1634 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11028 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/model.py
--rw-r--r--   0        0        0       67 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3971 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3666 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3809 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      118 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     3603 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/preprocessors/normalizer.py
--rw-r--r--   0        0        0     3144 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      231 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    19353 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8674 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2538 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2177 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    17120 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      161 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5614 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/utils/core_utils.py
--rw-r--r--   0        0        0     3407 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-29 08:58:57.064990 hezar-0.17.1/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1646 2023-07-29 08:58:57.064990 hezar-0.17.1/pyproject.toml
--rw-r--r--   0        0        0     6789 1970-01-01 00:00:00.000000 hezar-0.17.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-29 11:46:23.700164 hezar-0.17.2/LICENSE
+-rw-r--r--   0        0        0     4309 2023-07-29 11:46:23.700164 hezar-0.17.2/README.md
+-rw-r--r--   0        0        0      261 2023-07-29 11:46:23.700164 hezar-0.17.2/hezar/__init__.py
+-rw-r--r--   0        0        0     5384 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/builders.py
+-rw-r--r--   0        0        0    11117 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/configs.py
+-rw-r--r--   0        0        0     2068 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6333 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4502 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3627 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      282 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1604 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11028 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/model.py
+-rw-r--r--   0        0        0       67 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3971 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3666 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3809 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     3603 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/normalizer.py
+-rw-r--r--   0        0        0     3333 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      231 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    19353 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8674 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2538 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2177 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    17127 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      161 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5614 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0     3660 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:46:23.704164 hezar-0.17.2/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1646 2023-07-29 11:46:23.704164 hezar-0.17.2/pyproject.toml
+-rw-r--r--   0        0        0     6789 1970-01-01 00:00:00.000000 hezar-0.17.2/PKG-INFO
```

### Comparing `hezar-0.17.1/LICENSE` & `hezar-0.17.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/README.md` & `hezar-0.17.2/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/builders.py` & `hezar-0.17.2/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/configs.py` & `hezar-0.17.2/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/constants.py` & `hezar-0.17.2/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/data/data_collators.py` & `hezar-0.17.2/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/data/datasets/dataset.py` & `hezar-0.17.2/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.17.2/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.17.2/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/data/utils/data_utils.py` & `hezar-0.17.2/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/embeddings/embedding.py` & `hezar-0.17.2/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/embeddings/fasttext.py` & `hezar-0.17.2/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/embeddings/word2vec.py` & `hezar-0.17.2/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/metrics/f1.py` & `hezar-0.17.2/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/metrics/metric.py` & `hezar-0.17.2/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/metrics/recall.py` & `hezar-0.17.2/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/metrics/seqeval.py` & `hezar-0.17.2/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.17.2/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.17.2/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.17.2/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.17.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.17.2/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.17.2/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/model.py` & `hezar-0.17.2/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.17.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.17.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.17.2/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.17.2/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.17.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.17.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.17.2/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.17.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/preprocessors/normalizer.py` & `hezar-0.17.2/hezar/preprocessors/normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/preprocessors/preprocessor.py` & `hezar-0.17.2/hezar/preprocessors/preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from collections import OrderedDict
 
 from huggingface_hub import hf_hub_download
 from omegaconf import OmegaConf
 
 from ..constants import DEFAULT_PREPROCESSOR_SUBFOLDER, RegistryType, RepoType
 from ..utils import get_module_class, list_repo_files
@@ -62,20 +63,23 @@
             A Preprocessor subclass or a dict of Preprocessor subclass instances
         """
         subfolder = subfolder or cls.preprocessor_subfolder
         preprocessor_files = list_repo_files(hub_or_local_path, subfolder=subfolder)
         preprocessors = OrderedDict()
         for f in preprocessor_files:
             if f.endswith(".yaml"):
-                config_file = hf_hub_download(
-                    hub_or_local_path,
-                    filename=f,
-                    subfolder=subfolder,
-                    repo_type=RepoType.MODEL
-                )
+                if os.path.isdir(hub_or_local_path):
+                    config_file = os.path.join(hub_or_local_path, subfolder, f)
+                else:
+                    config_file = hf_hub_download(
+                        hub_or_local_path,
+                        filename=f,
+                        subfolder=subfolder,
+                        repo_type=RepoType.MODEL
+                    )
                 config = OmegaConf.load(config_file)
                 name = config.get("name", None)
                 if name:
                     preprocessor_cls = get_module_class(name, module_type=RegistryType.PREPROCESSOR)
                     preprocessor = preprocessor_cls.load(hub_or_local_path, subfolder=subfolder)
                     preprocessors[name] = preprocessor
                 else:
```

### Comparing `hezar-0.17.1/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.17.2/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.17.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.17.2/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.17.2/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/registry.py` & `hezar-0.17.2/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.17.2/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.17.2/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/trainers/trainer.py` & `hezar-0.17.2/hezar/trainers/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,18 +20,16 @@
     TQDM_BAR_FORMAT,
 )
 from ..data.datasets import Dataset
 from ..models import Model
 from ..utils import get_logger
 from .trainer_utils import MetricsTracker
 
-
 logger = get_logger(__name__)
 
-
 optimizers = {
     "adam": torch.optim.Adam,
     "adamw": torch.optim.AdamW,
     "sgd": torch.optim.SGD,
 }
 lr_schedulers = {
     "reduce_on_plateau": torch.optim.lr_scheduler.ReduceLROnPlateau,
@@ -190,15 +188,15 @@
         metrics_dict = {}
         for metric in self.config.metrics:
             if isinstance(metric, str):
                 if metric not in self.AVAILABLE_METRICS:
                     raise ValueError(f"Invalid metric `{metric}`! Available metrics: {self.AVAILABLE_METRICS}")
                 metrics_dict[metric] = build_metric(metric)
             elif isinstance(metric, MetricConfig):
-                metrics_dict[metric] = build_metric(metric.name, config=metric)
+                metrics_dict[metric.name] = build_metric(metric.name, config=metric)
             else:
                 raise ValueError(f"Invalid metric type `{type(metric)}`! Available metrics: {self.AVAILABLE_METRICS}")
         return metrics_dict
 
     def prepare_input_batch(self, input_batch):
         """
         Every operation required to prepare the inputs for model forward like moving to device, permutations, etc.
@@ -361,15 +359,15 @@
                     input_batch = self.prepare_input_batch(input_batch)
                     # Evaluation on one batch
                     outputs = self.evaluation_step(input_batch)
                     # Compute metrics
                     evaluation_results = self.compute_metrics(
                         outputs["logits"].detach().cpu().numpy(),
                         input_batch["labels"].detach().cpu().numpy(),
-                )
+                    )
                     evaluation_results["loss"] = outputs["loss"]
                     # Gather outputs for metrics
                     self.metrics_tracker.update(evaluation_results)
                     iterator.set_postfix(**self.metrics_tracker.avg())
 
         return self.metrics_tracker.avg()
```

### Comparing `hezar-0.17.1/hezar/trainers/trainer_utils.py` & `hezar-0.17.2/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/utils/common_utils.py` & `hezar-0.17.2/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/utils/core_utils.py` & `hezar-0.17.2/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.1/hezar/utils/hub_utils.py` & `hezar-0.17.2/hezar/utils/hub_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,15 +107,22 @@
         hub_or_local_path: Path to hub or local repo
         subfolder: Optional subfolder path
 
     Returns:
         A list of all file names
     """
     if os.path.isdir(hub_or_local_path):
-        files = os.listdir(hub_or_local_path)
+        files_itr = os.walk(hub_or_local_path)
+        files = []
+        for r, d, f in files_itr:
+            if r == hub_or_local_path:
+                files.append(f)
+            else:
+                for x in f:
+                    files.append(f"{r.replace(f'{hub_or_local_path}/', '')}/{x}")
     else:
         files = HfApi().list_repo_files(hub_or_local_path, repo_type=RepoType.MODEL)
 
     if subfolder is not None:
         files = [x.replace(f"{subfolder}/", "") for x in files if subfolder in x]
 
     return files
```

### Comparing `hezar-0.17.1/pyproject.toml` & `hezar-0.17.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.17.1"
+version = "0.17.2"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.17.1/PKG-INFO` & `hezar-0.17.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.17.1
+Version: 0.17.2
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

