# Comparing `tmp/hezar-0.16.0.tar.gz` & `tmp/hezar-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.16.0.tar", max compression
+gzip compressed data, was "hezar-0.17.0.tar", max compression
```

## Comparing `hezar-0.16.0.tar` & `hezar-0.17.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1065 2023-07-27 10:11:58.207428 hezar-0.16.0/LICENSE
--rw-r--r--   0        0        0     4427 2023-07-27 10:11:58.207428 hezar-0.16.0/README.md
--rw-r--r--   0        0        0      261 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/__init__.py
--rw-r--r--   0        0        0     5383 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/builders.py
--rw-r--r--   0        0        0    11117 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/configs.py
--rw-r--r--   0        0        0     2068 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/__init__.py
--rw-r--r--   0        0        0     6333 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4502 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3627 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      282 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1136 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1208 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1172 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0     9544 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/model.py
--rw-r--r--   0        0        0       67 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3354 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3082 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3217 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3347 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      118 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     3492 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/normalizer.py
--rw-r--r--   0        0        0     2954 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      231 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    19346 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8914 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2538 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2177 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    17120 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      161 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5614 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/core_utils.py
--rw-r--r--   0        0        0     3407 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1626 2023-07-27 10:11:58.211428 hezar-0.16.0/pyproject.toml
--rw-r--r--   0        0        0     6874 1970-01-01 00:00:00.000000 hezar-0.16.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-28 09:09:37.337953 hezar-0.17.0/LICENSE
+-rw-r--r--   0        0        0     4427 2023-07-28 09:09:37.337953 hezar-0.17.0/README.md
+-rw-r--r--   0        0        0      261 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/__init__.py
+-rw-r--r--   0        0        0     5384 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/builders.py
+-rw-r--r--   0        0        0    11117 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/configs.py
+-rw-r--r--   0        0        0     2068 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6333 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4502 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3627 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      282 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1604 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11028 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/model.py
+-rw-r--r--   0        0        0       67 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3971 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3666 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3809 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     3603 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/preprocessors/normalizer.py
+-rw-r--r--   0        0        0     3144 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      231 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    19353 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8674 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-28 09:09:37.341953 hezar-0.17.0/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2538 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2177 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    17120 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      161 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5614 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0     3407 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:09:37.345953 hezar-0.17.0/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1626 2023-07-28 09:09:37.345953 hezar-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0     6874 1970-01-01 00:00:00.000000 hezar-0.17.0/PKG-INFO
```

### Comparing `hezar-0.16.0/LICENSE` & `hezar-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/README.md` & `hezar-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/builders.py` & `hezar-0.17.0/hezar/builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
     Args:
         name (str): Name of the embedding in the embeddings' registry
         config (EmbeddingConfig): An EmbeddingConfig instance
         **kwargs: Extra config parameters that are loaded to the embedding
 
     Returns:
-        A Dataset instance
+        A Embedding instance
     """
     if name not in embeddings_registry:
         raise ValueError(f"Unknown embedding name: `{name}`!\n"
                          f"Available embedding names: {list(embeddings_registry.keys())}")
     config = config or embeddings_registry[name].config_class()
     embedding = embeddings_registry[name].module_class(config, **kwargs)
     return embedding
@@ -132,15 +132,15 @@
 
     Args:
         name (str): Name of the metric in the metrics' registry
         config (MetricConfig): A MetricConfig instance
         **kwargs: Extra config parameters that are loaded to the metric
 
     Returns:
-        A Dataset instance
+        A Metric instance
     """
     if name not in metrics_registry:
         raise ValueError(f"Unknown metric name: `{name}`!\n"
                          f"Available metric names: {list(metrics_registry.keys())}")
     name = snake_case(name)
     config = config or metrics_registry[name].config_class()
     metric = metrics_registry[name].module_class(config, **kwargs)
```

### Comparing `hezar-0.16.0/hezar/configs.py` & `hezar-0.17.0/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/constants.py` & `hezar-0.17.0/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/data/data_collators.py` & `hezar-0.17.0/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/data/datasets/dataset.py` & `hezar-0.17.0/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.17.0/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.17.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/data/utils/data_utils.py` & `hezar-0.17.0/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/embeddings/embedding.py` & `hezar-0.17.0/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/embeddings/fasttext.py` & `hezar-0.17.0/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/embeddings/word2vec.py` & `hezar-0.17.0/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/metrics/f1.py` & `hezar-0.17.0/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/metrics/metric.py` & `hezar-0.17.0/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/metrics/recall.py` & `hezar-0.17.0/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/metrics/seqeval.py` & `hezar-0.17.0/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.17.0/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 A BERT Language Model (HuggingFace Transformers) wrapped by a Hezar Model class
 """
+from typing import List, Union
+
 from transformers import BertConfig, BertModel
 
 from ....models import Model
 from ....registry import register_model
 from .bert_lm_config import BertLMConfig
 
 
@@ -20,14 +22,24 @@
         outputs = self.bert(
             input_ids=input_ids,
             attention_mask=attention_mask,
             **kwargs,
         )
         return outputs
 
+    def preprocess(self, inputs: Union[str, List[str]], **kwargs):
+        if isinstance(inputs, str):
+            inputs = [inputs]
+        if "normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["normalizer"]
+            inputs = normalizer(inputs)
+        tokenizer = self.preprocessor["wordpiece_tokenizer"]
+        inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
+        return inputs
+
     def post_process(self, inputs, **kwargs):
         hidden_states = inputs.get("hidden_states", None)
         attentions = inputs.get("attentions", None)
         outputs = {
             "last_hidden_state": inputs.get("last_hidden_state"),
             "hidden_states": hidden_states,
             "attentions": attentions,
```

### Comparing `hezar-0.16.0/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.17.0/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.17.0/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 """
-A DistilBERT Language Model (HuggingFace Transformers) wrapped by a Hezar Model class
+A RoBERTa Language Model (HuggingFace Transformers) wrapped by a Hezar Model class
 """
-from transformers import DistilBertConfig, DistilBertModel
+from typing import List, Union
+
+from transformers import RobertaConfig, RobertaModel
 
 from ....models import Model
 from ....registry import register_model
-from .distilbert_lm_config import DistilBertLMConfig
+from .roberta_lm_config import RobertaLMConfig
 
 
-@register_model("distilbert_lm", config_class=DistilBertLMConfig)
-class DistilBertLM(Model):
+@register_model("roberta_lm", config_class=RobertaLMConfig)
+class RobertaLM(Model):
     def __init__(self, config, **kwargs):
         super().__init__(config=config, **kwargs)
-        self.distilbert = DistilBertModel(DistilBertConfig(**self.config))
+        self.roberta = RobertaModel(RobertaConfig(**self.config))
 
     def forward(self, inputs, **kwargs):
         input_ids = inputs.get("token_ids")
         attention_mask = inputs.get("attention_mask", None)
-        outputs = self.distilbert(
+        outputs = self.roberta(
             input_ids=input_ids,
             attention_mask=attention_mask,
             **kwargs,
         )
         return outputs
 
+    def preprocess(self, inputs: Union[str, List[str]], **kwargs):
+        if isinstance(inputs, str):
+            inputs = [inputs]
+        if "normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["normalizer"]
+            inputs = normalizer(inputs)
+        tokenizer = self.preprocessor["bpe_tokenizer"]
+        inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
+        return inputs
+
     def post_process(self, inputs, **kwargs):
         hidden_states = inputs.get("hidden_states", None)
         attentions = inputs.get("attentions", None)
         outputs = {
             "last_hidden_state": inputs.get("last_hidden_state"),
             "hidden_states": hidden_states,
             "attentions": attentions,
```

### Comparing `hezar-0.16.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.17.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.17.0/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/models/model.py` & `hezar-0.17.0/hezar/models/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_file
 from torch import nn
 
 from ..builders import build_model
 from ..configs import ModelConfig
 from ..constants import DEFAULT_MODEL_CONFIG_FILE, DEFAULT_MODEL_FILE, HEZAR_CACHE_DIR
+from ..preprocessors import Preprocessor
 from ..utils import get_logger
 
 
 __all__ = [
     "Model",
     "ModelConfig",
 ]
@@ -41,37 +42,40 @@
 
     model_filename = DEFAULT_MODEL_FILE
     config_filename = DEFAULT_MODEL_CONFIG_FILE
 
     def __init__(self, config: ModelConfig, *args, **kwargs):
         super().__init__()
         self.config = config.update(kwargs)
+        self._preprocessor = None
 
     @classmethod
     def load(
         cls,
         hub_or_local_path: Union[str, os.PathLike],
         load_locally: Optional[bool] = False,
+        load_preprocessor: Optional[bool] = True,
         model_filename: Optional[str] = None,
         config_filename: Optional[str] = None,
         save_path: Optional[Union[str, os.PathLike]] = None,
         **kwargs,
     ):
         """
         Load the model from local path or hub.
 
         It's recommended to actually use this method with :class:`hezar.Model` rather than any other model class
         unless you actually know that the class is the same as the one on the Hub, because the output will always be
         the one specified on the Hub!
 
         Args:
             hub_or_local_path: Path to the model living on the Hub or local disk.
+            load_locally: Force loading from local path
+            load_preprocessor: Whether to load the preprocessor(s) or not
             model_filename: Optional model filename.
             config_filename: Optional config filename
-            load_locally: Force loading from local path
             save_path: Save model to this path after loading
 
         Returns:
             The fully loaded Hezar model
         """
         # Get device if provided in the kwargs
         device = None or kwargs.pop("device", None)
@@ -102,14 +106,18 @@
         # Get state dict from the model
         state_dict = torch.load(model_path, map_location=torch.device("cpu"))
         model.load_state_dict(state_dict)
         if device:
             model.to(device)
         if save_path:
             model.save(save_path)
+        # Load the preprocessor(s)
+        if load_preprocessor:
+            preprocessor = Preprocessor.load(hub_or_local_path, force_return_dict=True)
+            model.preprocessor = preprocessor
         return model
 
     def load_state_dict(self, state_dict: Mapping[str, Any], **kwargs):
         """
         Flexibly load the state dict to the model.
 
         Any incompatible or missing key is ignored and other layer weights are
@@ -230,39 +238,74 @@
             inputs: The required inputs for the model forward
 
         Returns:
             A dict of outputs like logits, loss, etc.
         """
         raise NotImplementedError
 
+    def preprocess(self, inputs, **kwargs):
+        """
+        Given raw inputs, preprocess the inputs and prepare them for model forward.
+
+        Args:
+            inputs: Raw model inputs
+            **kwargs: Extra kw arguments
+
+        Returns:
+            A dict of inputs for model forward
+        """
+        return inputs
+
     def post_process(self, inputs, **kwargs):
         """
         Process model outputs and return human-readable results. Called in `self.predict()`
 
         Args:
             inputs: model outputs
             **kwargs: extra arguments specific to the derived class
 
         Returns:
             Processed model output values and converted to human-readable results
         """
         return inputs
 
     @torch.inference_mode()
-    def predict(self, inputs, post_process=True, **kwargs) -> Dict:
+    def predict(self, inputs, **kwargs) -> Dict:
         """
         Perform an end-to-end prediction on raw inputs.
 
         Args:
             inputs: Raw inputs e.g, a list of texts, path to images, etc.
-            post_process: Whether to do post-processing step
 
         Returns:
             Output dict of results
         """
+        # Put model in eval mode
         self.eval()
+        # Preprocessing step
+        if self.preprocessor is not None:
+            inputs = self.preprocess(inputs, **kwargs)
+        # Model forward
         model_outputs = self(inputs, **kwargs)
-        if post_process:
-            processed_outputs = self.post_process(model_outputs, **kwargs)
-            return processed_outputs
-
-        return model_outputs
+        # Post-processing step
+        processed_outputs = self.post_process(model_outputs, **kwargs)
+        return processed_outputs
+
+    @property
+    def device(self):
+        return next(self.parameters()).device
+
+    @property
+    def preprocessor(self):
+        return self._preprocessor
+
+    @preprocessor.setter
+    def preprocessor(self, value):
+        if isinstance(value, Preprocessor):
+            preprocessor = OrderedDict()
+            preprocessor[value.config.name] = value
+        elif isinstance(value, (dict, OrderedDict)):
+            preprocessor = OrderedDict(**value)
+        else:
+            raise ValueError(f"Preprocessor value must be a `Preprocessor` or a dict of `Preprocessor` objects "
+                             f"not `{type(value)}`!")
+        self._preprocessor = preprocessor
```

### Comparing `hezar-0.16.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.17.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A BERT model for sequence labeling built using HuggingFace Transformers
 """
-from typing import Dict
+from typing import Dict, List, Union
 
 from torch import nn
 from transformers import BertConfig, BertModel
 
 from ....models import Model
 from ....registry import register_model
 from .bert_sequence_labeling_config import BertSequenceLabelingConfig
@@ -60,14 +60,32 @@
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
             "attentions": lm_outputs.attentions,
             **inputs
         }
         return outputs
 
+    def preprocess(self, inputs: Union[str, List[str]], **kwargs):
+        if isinstance(inputs, str):
+            inputs = [inputs]
+        if "normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["normalizer"]
+            inputs = normalizer(inputs)
+        tokenizer = self.preprocessor["wordpiece_tokenizer"]
+        inputs = tokenizer(
+            inputs,
+            return_word_ids=True,
+            return_tokens=True,
+            padding=True,
+            truncation=True,
+            return_tensors="pt",
+            device=self.device,
+        )
+        return inputs
+
     def post_process(self, inputs, **kwargs):
         # TODO sequence labeling outputs should consider rejoining split words into single words with proper tag
         logits = inputs["logits"]
         tokens = inputs["tokens"]
         word_ids = inputs["word_ids"]  # noqa
         predictions = logits.argmax(2).cpu()
         predictions = [[self.config.id2label[p.item()] for p in prediction] for prediction in predictions]
```

### Comparing `hezar-0.16.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.17.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.17.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A BERT model for text classification built using HuggingFace Transformers
 """
-from typing import Dict
+from typing import Dict, List, Union
 
 from torch import nn
 from transformers import BertConfig, BertModel
 
 from ....models import Model
 from ....registry import register_model
 from .bert_text_classification_config import BertTextClassificationConfig
@@ -15,15 +15,14 @@
 class BertTextClassification(Model):
     """
     A standard 🤗Transformers Bert model for text classification
 
     Args:
         config: The whole model config including arguments needed for the inner 🤗Transformers model.
     """
-
     def __init__(self, config: BertTextClassificationConfig, **kwargs):
         super().__init__(config, **kwargs)
         self.bert = BertModel(self._build_inner_config())
         classifier_dropout = (
             self.config.classifier_dropout if self.config.classifier_dropout is not None
             else self.config.hidden_dropout_prob
         )
@@ -61,14 +60,24 @@
         outputs = {
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
             "attentions": lm_outputs.attentions,
         }
         return outputs
 
+    def preprocess(self, inputs: Union[str, List[str]], **kwargs):
+        if isinstance(inputs, str):
+            inputs = [inputs]
+        if "normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["normalizer"]
+            inputs = normalizer(inputs)
+        tokenizer = self.preprocessor["wordpiece_tokenizer"]
+        inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
+        return inputs
+
     def post_process(self, inputs, **kwargs) -> Dict:
         logits = inputs["logits"]
         predictions = logits.argmax(1)
         predictions_probs = logits.softmax(1).max(1)
         outputs = {"labels": [], "probs": []}
         for prediction, prob in zip(predictions, predictions_probs):
             label = self.config.id2label[prediction.item()]
```

### Comparing `hezar-0.16.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.17.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.17.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A DistilBERT model for text classification built using HuggingFace Transformers
 """
-from typing import Dict
+from typing import Dict, List, Union
 
 from torch import nn
 from transformers import DistilBertConfig, DistilBertModel
 
 from ....models import Model
 from ....registry import register_model
 from .distilbert_text_classification_config import DistilBertTextClassificationConfig
@@ -62,14 +62,24 @@
         outputs = {
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
             "attentions": lm_outputs.attentions,
         }
         return outputs
 
+    def preprocess(self, inputs: Union[str, List[str]], **kwargs):
+        if isinstance(inputs, str):
+            inputs = [inputs]
+        if "normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["normalizer"]
+            inputs = normalizer(inputs)
+        tokenizer = self.preprocessor["wordpiece_tokenizer"]
+        inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
+        return inputs
+
     def post_process(self, inputs, **kwargs) -> Dict:
         logits = inputs["logits"]
         predictions = logits.argmax(1)
         predictions_probs = logits.softmax(1).max(1)
         outputs = {"labels": [], "probs": []}
         for prediction, prob in zip(predictions, predictions_probs):
             label = self.config.id2label[prediction.item()]
```

### Comparing `hezar-0.16.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.17.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.17.0/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 A RoBERTa Language Model (HuggingFace Transformers) wrapped by a Hezar Model class
 """
+from typing import List, Union
+
 from torch import nn, tanh
 from transformers import RobertaConfig, RobertaModel
 
 from ....models import Model
 from ....registry import register_model
 from .roberta_text_classification_config import RobertaTextClassificationConfig
 
@@ -47,14 +49,24 @@
         outputs = {
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
             "attentions": lm_outputs.attentions,
         }
         return outputs
 
+    def preprocess(self, inputs: Union[str, List[str]], **kwargs):
+        if isinstance(inputs, str):
+            inputs = [inputs]
+        if "normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["normalizer"]
+            inputs = normalizer(inputs)
+        tokenizer = self.preprocessor["bpe_tokenizer"]
+        inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
+        return inputs
+
     def post_process(self, inputs, **kwargs):
         logits = inputs["logits"]
         predictions = logits.argmax(1)
         predictions_probs = logits.softmax(1).max(1)
         outputs = {"labels": [], "probs": []}
         for prediction, prob in zip(predictions, predictions_probs):
             label = self.config.id2label[prediction.item()]
```

### Comparing `hezar-0.16.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.17.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/preprocessors/normalizer.py` & `hezar-0.17.0/hezar/preprocessors/normalizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,22 +35,27 @@
     def __init__(self, config: NormalizerConfig, **kwargs):
         super().__init__(config, **kwargs)
 
     def __call__(
         self,
         inputs: Union[str, List[str]],
         replace_pattern: str = None,
+        nfkd: bool = None,
+        nfkc: bool = None,
         **kwargs,
     ):
         if isinstance(inputs, str):
             inputs = [inputs]
 
-        if self.config.nfkd:
+        nfkd = nfkd or self.config.nfkd
+        nfkc = nfkc or self.config.nfkc
+
+        if nfkd:
             inputs = [normalizers.NFKD().normalize_str(x) for x in inputs]
-        if self.config.nfkc:
+        if nfkc:
             inputs = [normalizers.NFKC().normalize_str(x) for x in inputs]
 
         # TODO add support for other normalizations
 
         return inputs
 
     @classmethod
```

### Comparing `hezar-0.16.0/hezar/preprocessors/preprocessor.py` & `hezar-0.17.0/hezar/preprocessors/preprocessor.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,28 +36,30 @@
     def push_to_hub(self, hub_path):
         raise NotImplementedError
 
     @classmethod
     def load(
         cls,
         hub_or_local_path,
-        subfolder=None,
+        subfolder: str = None,
+        force_return_dict: bool = False,
         **kwargs
     ):
         """
         Load a preprocessor or a pipeline of preprocessors from a local or Hub path. This method automatically detects
         any preprocessor in the path. If there's only one preprocessor, returns it and if there are more, returns a
         dictionary of preprocessors.
 
         This method must also be overriden by subclasses as it internally calls this method for every possible
         preprocessor found in the repo.
 
         Args:
             hub_or_local_path: Path to hub or local repo
             subfolder: Subfolder for the preprocessor.
+            force_return_dict: Whether to return a dict even if there's only one preprocessor available on the repo
             **kwargs: Extra kwargs
 
         Returns:
             A Preprocessor subclass or a dict of Preprocessor subclass instances
         """
         subfolder = subfolder or cls.preprocessor_subfolder
         preprocessor_files = list_repo_files(hub_or_local_path, subfolder=subfolder)
@@ -74,11 +76,11 @@
                 name = config.get("name", None)
                 if name:
                     preprocessor_cls = get_module_class(name, module_type=RegistryType.PREPROCESSOR)
                     preprocessor = preprocessor_cls.load(hub_or_local_path, subfolder=subfolder)
                     preprocessors[name] = preprocessor
                 else:
                     raise ValueError(f"The config file `{config_file}` does not have the property `name`!")
-        if len(preprocessors) == 1:
+        if len(preprocessors) == 1 and not force_return_dict:
             return list(preprocessors.values())[0]
 
         return preprocessors
```

### Comparing `hezar-0.16.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.17.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.17.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.17.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             sanitized_outputs = {
                 key: value[0] if len(value) > 0 and isinstance(value[0], list) else value
                 for key, value in sanitized_outputs.items()
             }
 
         outputs = convert_batch_dict_dtype(sanitized_outputs, dtype=return_tensors)
         if device and return_tensors == "pt":
-            outputs = {k: v.to(device) for k, v in outputs.items() if isinstance(v, torch.Tensor)}
+            outputs = {k: v.to(device) if isinstance(v, torch.Tensor) else v for k, v in outputs.items()}
 
         return outputs
 
     def set_truncation_and_padding(
         self,
         padding_strategy=None,
         truncation_strategy=None,
```

### Comparing `hezar-0.16.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.17.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/registry.py` & `hezar-0.17.0/hezar/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,17 +63,14 @@
     """
     A class decorator that adds the model class and the config class to the `models_registry`
 
     Args:
         model_name: Model's registry name e.g, `bert_sequence_labeling`
         config_class: Model's config class e.g, `BertSequenceLabelingConfig`. This parameter must be the config class
             itself not a config instance!
-
-    Returns:
-         The class itself
     """
 
     def register(cls):
         if model_name in models_registry:
             logger.warning(f"Model `{model_name}` is already registered. Overwriting...")
 
         if config_class.name != model_name:
@@ -96,17 +93,14 @@
     """
     A class decorator that adds the dataset class and the config class to the `datasets_registry`
 
     Args:
         dataset_name: Dataset's registry name e.g, `text_classification`.
         config_class: Dataset's config class e.g, `TextClassificationDatasetConfig`. This parameter must be the config
             class itself not a config instance!
-
-    Returns:
-         The class itself
     """
 
     def register(cls):
         if dataset_name in datasets_registry:
             logger.warning(f"Dataset `{dataset_name}` is already registered. Overwriting...")
 
         if config_class.name != dataset_name:
@@ -129,17 +123,14 @@
     """
     A class decorator that adds the preprocessor class and the config class to the `preprocessors_registry`
 
     Args:
         preprocessor_name: Preprocessor's registry name e.g, `bpe_tokenizer`.
         config_class: Preprocessor's config class e.g, BPEConfig. This parameter must be the config
             class itself not a config instance!
-
-    Returns:
-         The class itself
     """
 
     def register(cls):
         if preprocessor_name in preprocessors_registry:
             logger.warning(f"Preprocessor `{preprocessor_name}` is already registered. Overwriting...")
 
         if config_class.name != preprocessor_name:
@@ -162,17 +153,14 @@
     """
     A class decorator that adds the embedding class and the config class to the `embeddings_registry`
 
     Args:
         embedding_name: Embedding's registry name e.g, `word2vec_cbow`.
         config_class: Embedding's config class e.g, Word2VecCBOWConfig. This parameter must be the config
             class itself not a config instance!
-
-    Returns:
-         The class itself
     """
 
     def register(cls):
         if embedding_name in embeddings_registry:
             logger.warning(f"Embedding `{embedding_name}` is already registered. Overwriting...")
 
         if config_class.name != embedding_name:
@@ -195,17 +183,14 @@
     """
     A class decorator that adds the Trainer class and the config class to the `trainers_registry`
 
     Args:
         trainer_name: Trainer's registry name e.g, `text_classification_trainer`
         config_class: Trainer's config class e.g, `TextClassificationTrainerConfig`.
             This parameter must be the config class itself not a config instance!
-
-    Returns:
-         The class itself
     """
 
     def register(cls):
         if trainer_name in trainers_registry:
             logger.warning(f"Trainer `{trainer_name}` is already registered. Overwriting...")
 
         if config_class.name != trainer_name:
@@ -227,17 +212,14 @@
 def register_metric(metric_name: str, config_class: Type[MetricConfig]):
     """
     A class decorator that adds the metric class and the config class to the `metrics_registry`
 
     Args:
         metric_name: Metric registry name e.g, `f1`
         config_class: Metric config class
-
-    Returns:
-         The class itself
     """
 
     def register(cls):
         if metric_name in metrics_registry:
             logger.warning(f"Metric `{metric_name}` is already registered. Overwriting...")
         if config_class.name != metric_name:
             raise ValueError(f"`metric_name` and `config.name` are not compatible for `{cls.__name__}`\n"
```

### Comparing `hezar-0.16.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.17.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.17.0/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/trainers/trainer.py` & `hezar-0.17.0/hezar/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/trainers/trainer_utils.py` & `hezar-0.17.0/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/utils/common_utils.py` & `hezar-0.17.0/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/utils/core_utils.py` & `hezar-0.17.0/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/hezar/utils/hub_utils.py` & `hezar-0.17.0/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.16.0/pyproject.toml` & `hezar-0.17.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.16.0"
+version = "0.17.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.16.0/PKG-INFO` & `hezar-0.17.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.16.0
+Version: 0.17.0
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

