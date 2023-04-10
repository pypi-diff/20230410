# Comparing `tmp/spark-nlp-4.3.2.tar.gz` & `tmp/spark-nlp-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spark-nlp-4.3.2.tar", last modified: Tue Mar 14 16:00:25 2023, max compression
+gzip compressed data, was "dist/spark-nlp-4.4.0.tar", last modified: Mon Apr 10 17:00:16 2023, max compression
```

## Comparing `spark-nlp-4.3.2.tar` & `spark-nlp-4.4.0.tar`

### file list

```diff
@@ -1,243 +1,16 @@
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)       67 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/setup.cfg
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6281 2023-03-14 13:16:39.000000 spark-nlp-4.3.2/setup.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/internal/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     2136 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/internal/params_getters_setters.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1187 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/internal/annotator_java_ml.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     2756 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/internal/recursive.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    21409 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/internal/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     2240 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/internal/extended_java_wrapper.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1448 2023-01-29 13:31:11.000000 spark-nlp-4.3.2/sparknlp/internal/annotator_transformer.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     5635 2023-01-29 13:31:11.000000 spark-nlp-4.3.2/sparknlp/annotation.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/common/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1226 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/read_as.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1765 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/annotator_approach.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    11471 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/properties.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     4332 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/annotator_properties.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1306 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/utils.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      823 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/coverage_result.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     4842 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/storage.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1449 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/recursive_annotator_approach.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1880 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/annotator_model.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1169 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/annotator_type.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1103 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/common/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1276 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/util.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    12120 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/functions.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1917 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotation_audio.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/pretrained/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     5748 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/pretrained/pretrained_pipeline.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1099 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/pretrained/utils.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      793 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/pretrained/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     7518 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/pretrained/resource_downloader.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    13069 2023-03-14 13:16:39.000000 spark-nlp-4.3.2/sparknlp/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6018 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/upload_to_hub.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/keyword_extraction/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    13215 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/keyword_extraction/yake_keyword_extraction.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      720 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/keyword_extraction/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/token/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7967 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/token/recursive_tokenizer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     4686 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/token/chunk_tokenizer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7639 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/token/regex_tokenizer.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      861 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/token/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    19939 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/token/tokenizer.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/seq2seq/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    15318 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/seq2seq/gpt2_transformer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9444 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/seq2seq/marian_transformer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    15861 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/seq2seq/t5_transformer.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      833 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/seq2seq/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/pos/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9879 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/pos/perceptron.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      696 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/pos/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/ner/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6798 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/ner/ner_overwriter.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    14291 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/ner/ner_crf.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     5315 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/ner/ner_converter.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     2793 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/ner/ner_approach.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      948 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/ner/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    22139 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/ner/ner_dl.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     7501 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/ner/zero_shot_ner_model.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/param/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     4998 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/param/evaluation_dl_params.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     3005 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/param/classifier_encoder.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      750 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/param/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     5274 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/n_gram_generator.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     2639 2023-03-14 08:56:24.000000 spark-nlp-4.3.2/sparknlp/annotator/date2_chunk.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     3141 2023-03-14 08:56:24.000000 spark-nlp-4.3.2/sparknlp/annotator/chunk2_doc.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9927 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/xlm_roberta_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    13027 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/doc2vec.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9083 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/deberta_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8585 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/roberta_sentence_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     5402 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/sentence_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8814 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/bert_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6052 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/chunk_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9577 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/roberta_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9461 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/bert_sentence_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    13030 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/word2vec.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9714 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/distil_bert_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    15396 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/word_embeddings.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1853 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    10430 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/albert_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9003 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/xlm_roberta_sentence_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9866 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/elmo_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9206 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/camembert_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8579 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/universal_sentence_encoder.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9206 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/longformer_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9772 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/embeddings/xlnet_embeddings.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    10973 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/document_normalizer.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    12680 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/classifier_dl.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7275 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/distil_bert_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    14424 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/sentiment_dl.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8287 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/albert_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8257 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/xlnet_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6983 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6997 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/distil_bert_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7117 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/bert_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8301 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/roberta_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6966 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/camembert_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7286 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/albert_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7187 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/xlnet_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6994 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/longformer_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8371 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6877 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/bert_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6964 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/albert_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6934 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/deberta_for_question_answering.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6325 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/tapas_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8246 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/bert_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8369 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/longformer_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    16053 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/multi_classifier_dl.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8218 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/deberta_for_sequence_classification.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     3023 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7287 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/longformer_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6919 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/roberta_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     6956 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/camembert_for_question_answering.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8367 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/distil_bert_for_sequence_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7293 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/xlm_roberta_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7228 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/roberta_for_token_classification.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7184 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/deberta_for_token_classification.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     8403 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/classifier_dl/camembert_for_sequence_classification.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6373 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/tf_ner_dl_graph_builder.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/er/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9492 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/er/entity_ruler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      692 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/er/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/cv/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      723 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/cv/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    10595 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/cv/swin_for_image_classification.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     8285 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/cv/vit_for_image_classification.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/coref/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     8848 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/coref/spanbert_coref.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)       53 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/coref/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8780 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/normalizer.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/dependency/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    11220 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/dependency/dependency_parser.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      774 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/dependency/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    12464 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/dependency/typed_dependency_parser.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/sentiment/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8154 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/sentiment/sentiment_detector.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9655 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/sentiment/vivekn_sentiment.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      766 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/sentiment/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/matcher/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     4475 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/matcher/multi_date_matcher.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    10636 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/matcher/text_matcher.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     9785 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/matcher/big_text_matcher.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    10201 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/matcher/date_matcher.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      920 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/matcher/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8388 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/matcher/regex_matcher.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/ws/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      693 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/ws/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    16373 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/ws/word_segmenter.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/sentence/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    10806 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/sentence/sentence_detector.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    17874 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/sentence/sentence_detector_dl.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      767 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/sentence/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/spell_check/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    32012 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/spell_check/context_spell_checker.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    11066 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/spell_check/symmetric_delete.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      830 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/spell_check/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    13205 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/spell_check/norvig_sweeting.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     3325 2023-03-14 08:56:24.000000 spark-nlp-4.3.2/sparknlp/annotator/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/audio/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     7867 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/audio/hubert_for_ctc.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      702 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/audio/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6271 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/audio/wav2vec2_for_ctc.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     2948 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/stemmer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     5174 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/chunker.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     7031 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/stop_words_cleaner.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/annotator/ld_dl/
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8087 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/ld_dl/language_detector_dl.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      704 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/ld_dl/__init__.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     8986 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/annotator/lemmatizer.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)    14471 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotator/graph_extraction.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/training/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     4091 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/pos.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     4953 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/conllu.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     3331 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/pub_tator.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6961 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/training/conll.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      244 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/tfgraphs.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6798 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/training/spacy_to_annotation.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      852 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/training/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/tf2contrib/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    11803 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/tf2contrib/rnn.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    25976 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/tf2contrib/lstm_ops.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     8072 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/tf2contrib/gru_ops.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6616 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/tf2contrib/fused_rnn_cell.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    14939 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/tf2contrib/core_rnn_cell.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1228 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/tf2contrib/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)   166408 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/tf2contrib/rnn_cell.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    10819 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/graph_builders.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)        0 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/ner_dl/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      870 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/ner_dl/sentence_grouper.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     2356 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/ner_dl/ner_model_saver.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1311 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/ner_dl/create_graph.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     2593 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/ner_dl/dataset_encoder.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)        0 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/ner_dl/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    22502 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders/ner_dl/ner_model.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     9794 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/graph_builders.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)        0 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      870 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/sentence_grouper.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     2356 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model_saver.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1099 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/create_graph.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     2594 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/dataset_encoder.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)        0 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    23189 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/training/_tf_graph_builders_1x/ner_dl/ner_model.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/base/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      849 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/base/has_recursive_fit.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      841 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/base/has_recursive_transform.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     4279 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/base/recursive_pipeline.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6732 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/base/document_assembler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     3320 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/base/audio_assembler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     5102 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/base/table_assembler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     7659 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/base/embeddings_finisher.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     6551 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/base/doc2_chunk.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     4834 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/base/graph_finisher.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     7064 2023-03-14 08:56:24.000000 spark-nlp-4.3.2/sparknlp/base/multi_document_assembler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    16541 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/base/light_pipeline.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     5075 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/base/token_assembler.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     1307 2023-03-14 08:56:24.000000 spark-nlp-4.3.2/sparknlp/base/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     8577 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/base/finisher.py
--rwxrwxr-x   0 maziyar   (1000) maziyar   (3000)     2674 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/base/token2_chunk.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     3719 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/base/image_assembler.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/sparknlp/logging/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    15958 2023-03-05 11:49:33.000000 spark-nlp-4.3.2/sparknlp/logging/comet.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      642 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/logging/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     2547 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/sparknlp/annotation_image.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    62795 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/PKG-INFO
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/spark_nlp.egg-info/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)       13 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/spark_nlp.egg-info/top_level.txt
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)     9357 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/spark_nlp.egg-info/SOURCES.txt
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    62795 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/spark_nlp.egg-info/PKG-INFO
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)        1 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/spark_nlp.egg-info/dependency_links.txt
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)    50711 2023-03-14 14:43:02.000000 spark-nlp-4.3.2/README.md
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/com/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)        0 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/com/__init__.py
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/com/johnsnowlabs/
-drwxrwxr-x   0 maziyar   (1000) maziyar   (3000)        0 2023-03-14 16:00:25.000000 spark-nlp-4.3.2/com/johnsnowlabs/nlp/
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)      294 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/com/johnsnowlabs/nlp/__init__.py
--rw-rw-r--   0 maziyar   (1000) maziyar   (3000)        0 2022-12-20 14:09:19.000000 spark-nlp-4.3.2/com/johnsnowlabs/__init__.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-04-10 17:00:16.007153 spark-nlp-4.4.0/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    53183 2023-04-10 17:00:16.007153 spark-nlp-4.4.0/PKG-INFO
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    51443 2023-04-10 15:02:46.000000 spark-nlp-4.4.0/README.md
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-04-10 17:00:16.003153 spark-nlp-4.4.0/com/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-05 09:41:28.000000 spark-nlp-4.4.0/com/__init__.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-04-10 17:00:16.003153 spark-nlp-4.4.0/com/johnsnowlabs/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        0 2023-04-05 09:41:28.000000 spark-nlp-4.4.0/com/johnsnowlabs/__init__.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-04-10 17:00:16.007153 spark-nlp-4.4.0/com/johnsnowlabs/nlp/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      294 2023-04-05 09:41:28.000000 spark-nlp-4.4.0/com/johnsnowlabs/nlp/__init__.py
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)       67 2023-04-10 17:00:16.007153 spark-nlp-4.4.0/setup.cfg
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)     6281 2023-04-09 14:32:13.000000 spark-nlp-4.4.0/setup.py
+drwxrwxr-x   0 maziyar   (1000) maziyar   (1000)        0 2023-04-10 17:00:16.007153 spark-nlp-4.4.0/spark_nlp.egg-info/
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)    53183 2023-04-10 17:00:15.000000 spark-nlp-4.4.0/spark_nlp.egg-info/PKG-INFO
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)      238 2023-04-10 17:00:15.000000 spark-nlp-4.4.0/spark_nlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        1 2023-04-10 17:00:15.000000 spark-nlp-4.4.0/spark_nlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 maziyar   (1000) maziyar   (1000)        4 2023-04-10 17:00:15.000000 spark-nlp-4.4.0/spark_nlp.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spark-nlp-4.3.2/setup.py` & `spark-nlp-4.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
 
-    version='4.3.2',  # Required
+    version='4.4.0',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the 'Summary' metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='John Snow Labs Spark NLP is a natural language processing library built on top of Apache Spark ML. It provides simple, performant & accurate NLP annotations for machine learning pipelines, that scale easily in a distributed environment.',  # Required
 
     # This is an optional longer description of your project that represents
```

### Comparing `spark-nlp-4.3.2/README.md` & `spark-nlp-4.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,24 @@
         <img src="https://anaconda.org/johnsnowlabs/spark-nlp/badges/version.svg" /></a>
     <a href="https://github.com/JohnSnowLabs/spark-nlp/blob/master/LICENSE" alt="License">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" /></a>
     <a href="https://pypi.org/project/spark-nlp/" alt="PyPi downloads">
         <img src="https://static.pepy.tech/personalized-badge/spark-nlp?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads" /></a>
 </p>
 
-Spark NLP is a state-of-the-art Natural Language Processing library built on top of Apache Spark. It provides **simple
-**, **performant** & **accurate** NLP annotations for machine learning pipelines that **scale** easily in a distributed
+Spark NLP is a state-of-the-art Natural Language Processing library built on top of Apache Spark. It provides **simple**, **performant** & **accurate** NLP annotations for machine learning pipelines that **scale** easily in a distributed
 environment.
-Spark NLP comes with **11000+** pretrained **pipelines** and **models** in more than **200+** languages.
-It also offers tasks such as **Tokenization**, **Word Segmentation**, **Part-of-Speech Tagging**, Word and Sentence **Embeddings**, **Named Entity Recognition**, **Dependency Parsing**, **Spell Checking**, **Text Classification**, **Sentiment Analysis**, **Token Classification**, **Machine Translation** (+180 languages), **Summarization**, **Question Answering**, **Table Question Answering**, **Text Generation**, **Image Classification**, **Automatic Speech Recognition
-**, and many more [NLP tasks](#features).
+Spark NLP comes with **17000+** pretrained **pipelines** and **models** in more than **200+** languages.
+It also offers tasks such as **Tokenization**, **Word Segmentation**, **Part-of-Speech Tagging**, Word and Sentence **Embeddings**, **Named Entity Recognition**, **Dependency Parsing**, **Spell Checking**, **Text Classification**, **Sentiment Analysis**, **Token Classification**, **Machine Translation** (+180 languages), **Summarization**, **Question Answering**, **Table Question Answering**, **Text Generation**, **Image Classification**, **Automatic Speech Recognition**, **Zero-Shot Learning**, and many more [NLP tasks](#features).
 
-**Spark NLP** is the only open-source NLP library in **production** that offers state-of-the-art transformers such as **BERT**, **CamemBERT**, **ALBERT**, **ELECTRA**, **XLNet**, **DistilBERT**, **RoBERTa**, **DeBERTa**, **XLM-RoBERTa**, **Longformer**, **ELMO**, **Universal Sentence Encoder**, **Google T5**, **MarianMT**, **GPT2**, and **Vision Transformers (ViT)** not only to **Python** and **R**, but also to **JVM** ecosystem (**Java**, **Scala**, and **Kotlin**) at **scale** by extending **Apache Spark** natively.
+**Spark NLP** is the only open-source NLP library in **production** that offers state-of-the-art transformers such as **BERT**, **CamemBERT**, **ALBERT**, **ELECTRA**, **XLNet**, **DistilBERT**, **RoBERTa**, **DeBERTa**, **XLM-RoBERTa**, **Longformer**, **ELMO**, **Universal Sentence Encoder**, **Facebook BART**, **Google T5**, **MarianMT**, **OpenAI GPT2**, and **Vision Transformers (ViT)** not only to **Python** and **R**, but also to **JVM** ecosystem (**Java**, **Scala**, and **Kotlin**) at **scale** by extending **Apache Spark** natively.
 
 ## Project's website
 
-Take a look at our official Spark NLP page: [http://nlp.johnsnowlabs.com/](http://nlp.johnsnowlabs.com/) for user
+Take a look at our official Spark NLP page: [https://sparknlp.org/](https://sparknlp.org/) for user
 documentation and examples
 
 ## Community support
 
 - [Slack](https://join.slack.com/t/spark-nlp/shared_invite/zt-198dipu77-L3UWNe_AJ8xqDk0ivmih5Q) For live discussion with the Spark NLP community and the team
 - [GitHub](https://github.com/JohnSnowLabs/spark-nlp) Bug reports, feature requests, and contributions
 - [Discussions](https://github.com/JohnSnowLabs/spark-nlp/discussions) Engage with other community members, share ideas,
@@ -135,40 +133,43 @@
 - ALBERT for Question Answering
 - RoBERTa for Question Answering
 - DeBERTa for Question Answering
 - XLM-RoBERTa for Question Answering
 - Longformer for Question Answering
 - Table Question Answering (TAPAS)
 - Zero-Shot NER Model
+- Zero Shot Text Classification by BERT (ZSL)
 - Neural Machine Translation (MarianMT)
 - Text-To-Text Transfer Transformer (Google T5)
 - Generative Pre-trained Transformer 2 (OpenAI GPT2)
-- Vision Transformer (ViT)
-- Swin Image Classification
+- Seq2Seq for NLG, Translation, and Comprehension (Facebook BART)
+- Vision Transformer (Google ViT)
+- Swin Image Classification (Microsoft Swin Transformer)
+- ConvNext Image Classification (Facebook ConvNext)
 - Automatic Speech Recognition (Wav2Vec2)
 - Automatic Speech Recognition (HuBERT)
 - Named entity recognition (Deep learning)
 - Easy TensorFlow integration
 - GPU Support
 - Full integration with Spark ML functions
-- +9400 pre-trained models in +200 languages!
-- +3200 pre-trained pipelines in +200 languages!
+- +12000 pre-trained models in +200 languages!
+- +5000 pre-trained pipelines in +200 languages!
 - Multi-lingual NER models: Arabic, Bengali, Chinese, Danish, Dutch, English, Finnish, French, German, Hebrew, Italian,
   Japanese, Korean, Norwegian, Persian, Polish, Portuguese, Russian, Spanish, Swedish, Urdu, and more.
 
 ## Requirements
 
 To use Spark NLP you need the following requirements:
 
 - Java 8 and 11
 - Apache Spark 3.3.x, 3.2.x, 3.1.x, 3.0.x
 
 **GPU (optional):**
 
-Spark NLP 4.3.2 is built with TensorFlow 2.7.1 and the following NVIDIA® software are only required for GPU support:
+Spark NLP 4.4.0 is built with TensorFlow 2.7.1 and the following NVIDIA® software are only required for GPU support:
 
 - NVIDIA® GPU drivers version 450.80.02 or higher
 - CUDA® Toolkit 11.2
 - cuDNN SDK 8.1.0
 
 ## Quick Start
 
@@ -176,15 +177,15 @@
 
 ```sh
 $ java -version
 # should be Java 8 or 11 (Oracle or OpenJDK)
 $ conda create -n sparknlp python=3.7 -y
 $ conda activate sparknlp
 # spark-nlp by default is based on pyspark 3.x
-$ pip install spark-nlp==4.3.2 pyspark==3.3.1
+$ pip install spark-nlp==4.4.0 pyspark==3.3.1
 ```
 
 In Python console or Jupyter `Python3` kernel:
 
 ```python
 # Import Spark NLP
 from sparknlp.base import *
@@ -221,19 +222,20 @@
 Output: ['Mona Lisa', 'Leonardo', 'Louvre', 'Paris']
 ```
 
 For more examples, you can visit our dedicated [examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/examples) to showcase all Spark NLP use cases!
 
 ## Apache Spark Support
 
-Spark NLP *4.3.2* has been built on top of Apache Spark 3.2 while fully supports Apache Spark 3.0.x, 3.1.x, 3.2.x, and
+Spark NLP *4.4.0* has been built on top of Apache Spark 3.2 while fully supports Apache Spark 3.0.x, 3.1.x, 3.2.x, and
 3.3.x:
 
 | Spark NLP | Apache Spark 2.3.x | Apache Spark 2.4.x | Apache Spark 3.0.x | Apache Spark 3.1.x | Apache Spark 3.2.x | Apache Spark 3.3.x |
 |-----------|--------------------|--------------------|--------------------|--------------------|--------------------|--------------------|
+| 4.4.x     | NO                 | NO                 | YES                | YES                | YES                | YES                |
 | 4.3.x     | NO                 | NO                 | YES                | YES                | YES                | YES                |
 | 4.2.x     | NO                 | NO                 | YES                | YES                | YES                | YES                |
 | 4.1.x     | NO                 | NO                 | YES                | YES                | YES                | YES                |
 | 4.0.x     | NO                 | NO                 | YES                | YES                | YES                | YES                |
 | 3.4.x     | YES                | YES                | YES                | YES                | Partially          | N/A                |
 | 3.3.x     | YES                | YES                | YES                | YES                | NO                 | NO                 |
 | 3.2.x     | YES                | YES                | YES                | YES                | NO                 | NO                 |
@@ -244,30 +246,31 @@
 NOTE: Starting 4.0.0 release, the default `spark-nlp` and `spark-nlp-gpu` packages are based on Scala 2.12.15 and Apache
 Spark 3.2 by default.
 
 Find out more about `Spark NLP` versions from our [release notes](https://github.com/JohnSnowLabs/spark-nlp/releases).
 
 ## Scala and Python Support
 
-| Spark NLP | Python 3.6 | Python 3.7 | Python 3.8 | Python 3.9 | Scala 2.11 | Scala 2.12 |
-|-----------|------------|------------|------------|------------|------------|------------|
-| 4.3.x     | YES        | YES        | YES        | YES        | NO         | YES        |
-| 4.2.x     | YES        | YES        | YES        | YES        | NO         | YES        |
-| 4.1.x     | YES        | YES        | YES        | YES        | NO         | YES        |
-| 4.0.x     | YES        | YES        | YES        | YES        | NO         | YES        |
-| 3.4.x     | YES        | YES        | YES        | YES        | YES        | YES        |
-| 3.3.x     | YES        | YES        | YES        | NO         | YES        | YES        |
-| 3.2.x     | YES        | YES        | YES        | NO         | YES        | YES        |
-| 3.1.x     | YES        | YES        | YES        | NO         | YES        | YES        |
-| 3.0.x     | YES        | YES        | YES        | NO         | YES        | YES        |
-| 2.7.x     | YES        | YES        | NO         | NO         | YES        | NO         |
+| Spark NLP | Python 3.6 | Python 3.7 | Python 3.8 | Python 3.9 | Python 3.10| Scala 2.11 | Scala 2.12 |
+|-----------|------------|------------|------------|------------|------------|------------|------------|
+| 4.4.x     | NO         | YES        | YES        | YES        | YES        | NO         | YES        |
+| 4.3.x     | YES        | YES        | YES        | YES        | YES        | NO         | YES        |
+| 4.2.x     | YES        | YES        | YES        | YES        | YES        | NO         | YES        |
+| 4.1.x     | YES        | YES        | YES        | YES        | NO         | NO         | YES        |
+| 4.0.x     | YES        | YES        | YES        | YES        | NO         | NO         | YES        |
+| 3.4.x     | YES        | YES        | YES        | YES        | NO         | YES        | YES        |
+| 3.3.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
+| 3.2.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
+| 3.1.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
+| 3.0.x     | YES        | YES        | YES        | NO         | NO         | YES        | YES        |
+| 2.7.x     | YES        | YES        | NO         | NO         | NO         | YES        | NO         |
 
 ## Databricks Support
 
-Spark NLP 4.3.2 has been tested and is compatible with the following runtimes:
+Spark NLP 4.4.0 has been tested and is compatible with the following runtimes:
 
 **CPU:**
 
 - 7.3
 - 7.3 ML
 - 9.1
 - 9.1 ML
@@ -285,42 +288,54 @@
 - 11.0 ML
 - 11.1
 - 11.1 ML
 - 11.2
 - 11.2 ML
 - 11.3
 - 11.3 ML
+- 12.0
+- 12.0 ML
+- 12.1
+- 12.1 ML
+- 12.2
+- 12.2 ML
 
 **GPU:**
 
 - 9.1 ML & GPU
 - 10.1 ML & GPU
 - 10.2 ML & GPU
 - 10.3 ML & GPU
 - 10.4 ML & GPU
 - 10.5 ML & GPU
 - 11.0 ML & GPU
 - 11.1 ML & GPU
 - 11.2 ML & GPU
 - 11.3 ML & GPU
+- 12.0 ML & GPU
+- 12.1 ML & GPU
+- 12.2 ML & GPU
 
 NOTE: Spark NLP 4.x is based on TensorFlow 2.7.x which is compatible with CUDA11 and cuDNN 8.0.2. The only Databricks
 runtimes supporting CUDA 11 are 9.x and above as listed under GPU.
 
 ## EMR Support
 
-Spark NLP 4.3.2 has been tested and is compatible with the following EMR releases:
+Spark NLP 4.4.0 has been tested and is compatible with the following EMR releases:
 
 - emr-6.2.0
 - emr-6.3.0
 - emr-6.3.1
 - emr-6.4.0
 - emr-6.5.0
 - emr-6.6.0
 - emr-6.7.0
+- emr-6.8.0
+- emr-6.9.0
+- emr-6.10.0
 
 Full list of [Amazon EMR 6.x releases](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-release-6x.html)
 
 NOTE: The EMR 6.1.0 and 6.1.1 are not supported.
 
 ## Usage
 
@@ -345,74 +360,74 @@
 3.3.x.
 
 #### Apache Spark 3.x (3.0.x, 3.1.x, 3.2.x, and 3.3.x - Scala 2.12)
 
 ```sh
 # CPU
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
 ```
 
 The `spark-nlp` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp).
 
 ```sh
 # GPU
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.3.2
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.4.0
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.3.2
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.4.0
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.3.2
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.4.0
 
 ```
 
 The `spark-nlp-gpu` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu).
 
 ```sh
 # AArch64
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.3.2
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.4.0
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.3.2
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.4.0
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.3.2
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.4.0
 
 ```
 
 The `spark-nlp-aarch64` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64).
 
 ```sh
 # M1/M2 (Apple Silicon)
 
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.3.2
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.4.0
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.3.2
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.4.0
 
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.3.2
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.4.0
 
 ```
 
 The `spark-nlp-silicon` has been published to
 the [Maven Repository](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon).
 
 **NOTE**: In case you are using large pretrained models like UniversalSentenceEncoder, you need to have the following
 set in your SparkSession:
 
 ```sh
 spark-shell \
   --driver-memory 16g \
   --conf spark.kryoserializer.buffer.max=2000M \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
 ```
 
 ## Scala
 
 Spark NLP supports Scala 2.12.15 if you are using Apache Spark 3.0.x, 3.1.x, 3.2.x, and 3.3.x versions. Our packages are
 deployed to Maven central. To add any of our packages as a dependency in your application you can follow these
 coordinates:
@@ -422,79 +437,79 @@
 **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, and 3.3.x:
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp_2.12</artifactId>
-    <version>4.3.2</version>
+    <version>4.4.0</version>
 </dependency>
 ```
 
 **spark-nlp-gpu:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-gpu_2.12</artifactId>
-    <version>4.3.2</version>
+    <version>4.4.0</version>
 </dependency>
 ```
 
 **spark-nlp-aarch64:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64 -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-aarch64_2.12</artifactId>
-    <version>4.3.2</version>
+    <version>4.4.0</version>
 </dependency>
 ```
 
 **spark-nlp-silicon:**
 
 ```xml
 <!-- https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon -->
 <dependency>
     <groupId>com.johnsnowlabs.nlp</groupId>
     <artifactId>spark-nlp-silicon_2.12</artifactId>
-    <version>4.3.2</version>
+    <version>4.4.0</version>
 </dependency>
 ```
 
 ### SBT
 
 **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, and 3.3.x:
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "4.3.2"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "4.4.0"
 ```
 
 **spark-nlp-gpu:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-gpu
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "4.3.2"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "4.4.0"
 ```
 
 **spark-nlp-aarch64:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "4.3.2"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-aarch64" % "4.4.0"
 ```
 
 **spark-nlp-silicon:**
 
 ```sbtshell
 // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "4.3.2"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "4.4.0"
 ```
 
 Maven
 Central: [https://mvnrepository.com/artifact/com.johnsnowlabs.nlp](https://mvnrepository.com/artifact/com.johnsnowlabs.nlp)
 
 If you are interested, there is a simple SBT project for Spark NLP to guide you on how to use it in your
 projects [Spark NLP SBT Starter](https://github.com/maziyarpanahi/spark-nlp-starter)
@@ -508,15 +523,15 @@
 ### Pip/Conda
 
 If you installed pyspark through pip/conda, you can install `spark-nlp` through the same channel.
 
 Pip:
 
 ```bash
-pip install spark-nlp==4.3.2
+pip install spark-nlp==4.4.0
 ```
 
 Conda:
 
 ```bash
 conda install -c johnsnowlabs spark-nlp
 ```
@@ -537,15 +552,15 @@
 ```python
 spark = SparkSession.builder
     .appName("Spark NLP")
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.kryoserializer.buffer.max", "2000M")
-    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2")
+    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0")
     .getOrCreate()
 ```
 
 If using local jars, you can use `spark.jars` instead for comma-delimited jar files. For cluster setups, of course,
 you'll have to put the jars in a reachable location for all driver and executor nodes.
 
 **Quick example:**
@@ -608,26 +623,26 @@
 ## Apache Zeppelin
 
 Use either one of the following options
 
 - Add the following Maven Coordinates to the interpreter's library list
 
 ```bash
-com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
+com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
 ```
 
 - Add a path to pre-built jar from [here](#compiled-jars) in the interpreter's library list making sure the jar is
   available to driver path
 
 ### Python in Zeppelin
 
 Apart from the previous step, install the python module through pip
 
 ```bash
-pip install spark-nlp==4.3.2
+pip install spark-nlp==4.4.0
 ```
 
 Or you can install `spark-nlp` from inside Zeppelin by using Conda:
 
 ```bash
 python.conda install -c johnsnowlabs spark-nlp
 ```
@@ -647,15 +662,15 @@
 The easiest way to get this done on Linux and macOS is to simply install `spark-nlp` and `pyspark` PyPI packages and
 launch the Jupyter from the same Python environment:
 
 ```sh
 $ conda create -n sparknlp python=3.8 -y
 $ conda activate sparknlp
 # spark-nlp by default is based on pyspark 3.x
-$ pip install spark-nlp==4.3.2 pyspark==3.3.1 jupyter
+$ pip install spark-nlp==4.4.0 pyspark==3.3.1 jupyter
 $ jupyter notebook
 ```
 
 Then you can use `python3` kernel to run your code with creating SparkSession via `spark = sparknlp.start()`.
 
 **Optional:**
 
@@ -664,15 +679,15 @@
 
 ```bash
 export SPARK_HOME=/path/to/your/spark/folder
 export PYSPARK_PYTHON=python3
 export PYSPARK_DRIVER_PYTHON=jupyter
 export PYSPARK_DRIVER_PYTHON_OPTS=notebook
 
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
 ```
 
 Alternatively, you can mix in using `--jars` option for pyspark + `pip install spark-nlp`
 
 If not using pyspark at all, you'll have to run the instructions
 pointed [here](#python-without-explicit-Pyspark-installation)
 
@@ -691,15 +706,15 @@
 This script comes with the two options to define `pyspark` and `spark-nlp` versions via options:
 
 ```sh
 # -p is for pyspark
 # -s is for spark-nlp
 # -g will enable upgrading libcudnn8 to 8.1.0 on Google Colab for GPU usage
 # by default they are set to the latest
-!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 4.3.2
+!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 4.4.0
 ```
 
 [Spark NLP quick start on Google Colab](https://colab.research.google.com/github/JohnSnowLabs/spark-nlp/blob/master/examples/python/quick_start_google_colab.ipynb)
 is a live demo on Google Colab that performs named entity recognitions and sentiment analysis by using Spark NLP
 pretrained pipelines.
 
 ## Kaggle Kernel
@@ -714,15 +729,15 @@
 This script comes with the two options to define `pyspark` and `spark-nlp` versions via options:
 
 ```sh
 # -p is for pyspark
 # -s is for spark-nlp
 # -g will enable upgrading libcudnn8 to 8.1.0 on Kaggle for GPU usage
 # by default they are set to the latest
-!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 4.3.2
+!wget https://setup.johnsnowlabs.com/colab.sh -O - | bash /dev/stdin -p 3.2.3 -s 4.4.0
 ```
 
 [Spark NLP quick start on Kaggle Kernel](https://www.kaggle.com/mozzie/spark-nlp-named-entity-recognition) is a live
 demo on Kaggle Kernel that performs named entity recognitions by using Spark NLP pretrained pipeline.
 
 ## Databricks Cluster
 
@@ -733,17 +748,17 @@
     ```bash
     spark.kryoserializer.buffer.max 2000M
     spark.serializer org.apache.spark.serializer.KryoSerializer
     ```
 
 3. In `Libraries` tab inside your cluster you need to follow these steps:
 
-   3.1. Install New -> PyPI -> `spark-nlp==4.3.2` -> Install
+   3.1. Install New -> PyPI -> `spark-nlp==4.4.0` -> Install
 
-   3.2. Install New -> Maven -> Coordinates -> `com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2` -> Install
+   3.2. Install New -> Maven -> Coordinates -> `com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0` -> Install
 
 4. Now you can attach your notebook to the cluster and use Spark NLP!
 
 NOTE: Databricks' runtimes support different Apache Spark major releases. Please make sure you choose the correct Spark
 NLP Maven package name (Maven Coordinate) for your runtime from
 our [Packages Cheatsheet](https://github.com/JohnSnowLabs/spark-nlp#packages-cheatsheet)
 
@@ -786,24 +801,24 @@
   "Classification": "spark-defaults",
     "Properties": {
       "spark.yarn.stagingDir": "hdfs:///tmp",
       "spark.yarn.preserve.staging.files": "true",
       "spark.kryoserializer.buffer.max": "2000M",
       "spark.serializer": "org.apache.spark.serializer.KryoSerializer",
       "spark.driver.maxResultSize": "0",
-      "spark.jars.packages": "com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2"
+      "spark.jars.packages": "com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0"
     }
 }]
 ```
 
 A sample of AWS CLI to launch EMR cluster:
 
 ```.sh
 aws emr create-cluster \
---name "Spark NLP 4.3.2" \
+--name "Spark NLP 4.4.0" \
 --release-label emr-6.2.0 \
 --applications Name=Hadoop Name=Spark Name=Hive \
 --instance-type m4.4xlarge \
 --instance-count 3 \
 --use-default-roles \
 --log-uri "s3://<S3_BUCKET>/" \
 --bootstrap-actions Path=s3://<S3_BUCKET>/emr-bootstrap.sh,Name=custome \
@@ -859,15 +874,15 @@
   --worker-boot-disk-size=128GB \
   --num-workers=2 \
   --bucket=${BUCKET_NAME} \
   --optional-components=JUPYTER \
   --enable-component-gateway \
   --metadata 'PIP_PACKAGES=spark-nlp spark-nlp-display google-cloud-bigquery google-cloud-storage' \
   --initialization-actions gs://goog-dataproc-initialization-actions-${REGION}/python/pip-install.sh \
-  --properties spark:spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
+  --properties spark:spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
 ```
 
 2. On an existing one, you need to install spark-nlp and spark-nlp-display packages from PyPI.
 
 3. Now, you can attach your notebook to the cluster and use the Spark NLP!
 
 ## Spark NLP Configuration
@@ -898,42 +913,42 @@
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.serializer", "org.apache.spark.serializer.KryoSerializer")
     .config("spark.kryoserializer.buffer.max", "2000m")
     .config("spark.jsl.settings.pretrained.cache_folder", "sample_data/pretrained")
     .config("spark.jsl.settings.storage.cluster_tmp_dir", "sample_data/storage")
-    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2")
+    .config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0")
     .getOrCreate()
 ```
 
 **spark-shell:**
 
 ```sh
 spark-shell \
   --driver-memory 16g \
   --conf spark.driver.maxResultSize=0 \
   --conf spark.serializer=org.apache.spark.serializer.KryoSerializer
   --conf spark.kryoserializer.buffer.max=2000M \
   --conf spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \
   --conf spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
 ```
 
 **pyspark:**
 
 ```sh
 pyspark \
   --driver-memory 16g \
   --conf spark.driver.maxResultSize=0 \
   --conf spark.serializer=org.apache.spark.serializer.KryoSerializer
   --conf spark.kryoserializer.buffer.max=2000M \
   --conf spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \
   --conf spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \
-  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
+  --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
 ```
 
 **Databricks:**
 
 On a new cluster or existing one you need to add the following to the `Advanced Options -> Spark` tab:
 
 ```bash
@@ -1084,15 +1099,15 @@
 | clean_pattern                         |  en  | 3.0.0   |
 | check_spelling                        |  en  | 3.0.0   |
 | dependency_parse                      |  en  | 3.0.0   |
 +---------------------------------------+------+---------+
 */
 ```
 
-#### Please check out our Models Hub for the full list of [pre-trained pipelines](https://nlp.johnsnowlabs.com/models) with examples, demos, benchmarks, and more
+#### Please check out our Models Hub for the full list of [pre-trained pipelines](https://sparknlp.org/models) with examples, demos, benchmarks, and more
 
 ### Models
 
 **Some selected languages:
 ** `Afrikaans, Arabic, Armenian, Basque, Bengali, Breton, Bulgarian, Catalan, Czech, Dutch, English, Esperanto, Finnish, French, Galician, German, Greek, Hausa, Hebrew, Hindi, Hungarian, Indonesian, Irish, Italian, Japanese, Latin, Latvian, Marathi, Norwegian, Persian, Polish, Portuguese, Romanian, Russian, Slovak, Slovenian, Somali, Southern Sotho, Spanish, Swahili, Swedish, Tswana, Turkish, Ukrainian, Zulu`
 
 **Quick online example:**
@@ -1174,47 +1189,47 @@
 AssertionDLModel
 ...
 XlmRoBertaSentenceEmbeddings
 XlnetEmbeddings
 */
 ```
 
-#### Please check out our Models Hub for the full list of [pre-trained models](https://nlp.johnsnowlabs.com/models) with examples, demo, benchmark, and more
+#### Please check out our Models Hub for the full list of [pre-trained models](https://sparknlp.org/models) with examples, demo, benchmark, and more
 
 ## Offline
 
 Spark NLP library and all the pre-trained models/pipelines can be used entirely offline with no access to the Internet.
 If you are behind a proxy or a firewall with no access to the Maven repository (to download packages) or/and no access
 to S3 (to automatically download models and pipelines), you can simply follow the instructions to have Spark NLP without
 any limitations offline:
 
 - Instead of using the Maven package, you need to load our Fat JAR
 - Instead of using PretrainedPipeline for pretrained pipelines or the `.pretrained()` function to download pretrained
-  models, you will need to manually download your pipeline/model from [Models Hub](https://nlp.johnsnowlabs.com/models),
+  models, you will need to manually download your pipeline/model from [Models Hub](https://sparknlp.org/models),
   extract it, and load it.
 
 Example of `SparkSession` with Fat JAR to have Spark NLP offline:
 
 ```python
 spark = SparkSession.builder
     .appName("Spark NLP")
     .master("local[*]")
     .config("spark.driver.memory", "16G")
     .config("spark.driver.maxResultSize", "0")
     .config("spark.kryoserializer.buffer.max", "2000M")
-    .config("spark.jars", "/tmp/spark-nlp-assembly-4.3.2.jar")
+    .config("spark.jars", "/tmp/spark-nlp-assembly-4.4.0.jar")
     .getOrCreate()
 ```
 
 - You can download provided Fat JARs from each [release notes](https://github.com/JohnSnowLabs/spark-nlp/releases),
   please pay attention to pick the one that suits your environment depending on the device (CPU/GPU) and Apache Spark
   version (3.0.x, 3.1.x, 3.2.x, and 3.3.x)
 - If you are local, you can load the Fat JAR from your local FileSystem, however, if you are in a cluster setup you need
   to put the Fat JAR on a distributed FileSystem such as HDFS, DBFS, S3, etc. (
-  i.e., `hdfs:///tmp/spark-nlp-assembly-4.3.2.jar`)
+  i.e., `hdfs:///tmp/spark-nlp-assembly-4.4.0.jar`)
 
 Example of using pretrained Models and Pipelines in offline:
 
 ```python
 # instead of using pretrained() for online:
 # french_pos = PerceptronModel.pretrained("pos_ud_gsd", lang="fr")
 # you download this model, extract it, and use .load
@@ -1236,21 +1251,21 @@
   i.e., `hdfs:///tmp/explain_document_dl_en_2.0.2_2.4_1556530585689/`)
 
 ## Examples
 
 Need more **examples**? Check out our dedicated [Spark NLP Examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/examples)
 repository to showcase all Spark NLP use cases!
 
-Also, don't forget to check [Spark NLP in Action](https://nlp.johnsnowlabs.com/demo) built by Streamlit.
+Also, don't forget to check [Spark NLP in Action](https://sparknlp.org/demo) built by Streamlit.
 
 ### All examples: [spark-nlp/examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/examples)
 
 ## FAQ
 
-[Check our Articles and Videos page here](https://nlp.johnsnowlabs.com/learn)
+[Check our Articles and Videos page here](https://sparknlp.org/learn)
 
 ## Citation
 
 We have published a [paper](https://www.sciencedirect.com/science/article/pii/S2665963821000063) that you can cite for
 the Spark NLP library:
 
 ```bibtex
```

#### html2text {}

```diff
@@ -4,34 +4,34 @@
     square&logo=github] [https://maven-badges.herokuapp.com/maven-central/
 com.johnsnowlabs.nlp/spark-nlp_2.12/badge.svg] [https://badge.fury.io/py/spark-
   nlp.svg] [https://anaconda.org/johnsnowlabs/spark-nlp/badges/version.svg]
     [https://img.shields.io/badge/License-Apache%202.0-blue.svg] [https://
                   static.pepy.tech/personalized-badge/spark-
 nlp?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads]
 Spark NLP is a state-of-the-art Natural Language Processing library built on
-top of Apache Spark. It provides **simple **, **performant** & **accurate** NLP
+top of Apache Spark. It provides **simple**, **performant** & **accurate** NLP
 annotations for machine learning pipelines that **scale** easily in a
-distributed environment. Spark NLP comes with **11000+** pretrained
+distributed environment. Spark NLP comes with **17000+** pretrained
 **pipelines** and **models** in more than **200+** languages. It also offers
 tasks such as **Tokenization**, **Word Segmentation**, **Part-of-Speech
 Tagging**, Word and Sentence **Embeddings**, **Named Entity Recognition**,
 **Dependency Parsing**, **Spell Checking**, **Text Classification**,
 **Sentiment Analysis**, **Token Classification**, **Machine Translation** (+180
 languages), **Summarization**, **Question Answering**, **Table Question
 Answering**, **Text Generation**, **Image Classification**, **Automatic Speech
-Recognition **, and many more [NLP tasks](#features). **Spark NLP** is the only
-open-source NLP library in **production** that offers state-of-the-art
-transformers such as **BERT**, **CamemBERT**, **ALBERT**, **ELECTRA**,
-**XLNet**, **DistilBERT**, **RoBERTa**, **DeBERTa**, **XLM-RoBERTa**,
-**Longformer**, **ELMO**, **Universal Sentence Encoder**, **Google T5**,
-**MarianMT**, **GPT2**, and **Vision Transformers (ViT)** not only to
-**Python** and **R**, but also to **JVM** ecosystem (**Java**, **Scala**, and
-**Kotlin**) at **scale** by extending **Apache Spark** natively. ## Project's
-website Take a look at our official Spark NLP page: [http://
-nlp.johnsnowlabs.com/](http://nlp.johnsnowlabs.com/) for user documentation and
+Recognition**, **Zero-Shot Learning**, and many more [NLP tasks](#features).
+**Spark NLP** is the only open-source NLP library in **production** that offers
+state-of-the-art transformers such as **BERT**, **CamemBERT**, **ALBERT**,
+**ELECTRA**, **XLNet**, **DistilBERT**, **RoBERTa**, **DeBERTa**, **XLM-
+RoBERTa**, **Longformer**, **ELMO**, **Universal Sentence Encoder**, **Facebook
+BART**, **Google T5**, **MarianMT**, **OpenAI GPT2**, and **Vision Transformers
+(ViT)** not only to **Python** and **R**, but also to **JVM** ecosystem
+(**Java**, **Scala**, and **Kotlin**) at **scale** by extending **Apache
+Spark** natively. ## Project's website Take a look at our official Spark NLP
+page: [https://sparknlp.org/](https://sparknlp.org/) for user documentation and
 examples ## Community support - [Slack](https://join.slack.com/t/spark-nlp/
 shared_invite/zt-198dipu77-L3UWNe_AJ8xqDk0ivmih5Q) For live discussion with the
 Spark NLP community and the team - [GitHub](https://github.com/JohnSnowLabs/
 spark-nlp) Bug reports, feature requests, and contributions - [Discussions]
 (https://github.com/JohnSnowLabs/spark-nlp/discussions) Engage with other
 community members, share ideas, and show off how you use Spark NLP! - [Medium]
 (https://medium.com/spark-nlp) Spark NLP articles - [YouTube](https://
@@ -75,84 +75,91 @@
 DeBERTa for Token & Sequence Classification - XLM-RoBERTa for Token & Sequence
 Classification - XLNet for Token & Sequence Classification - Longformer for
 Token & Sequence Classification - BERT for Token & Sequence Classification -
 BERT for Question Answering - CamemBERT for Question Answering - DistilBERT for
 Question Answering - ALBERT for Question Answering - RoBERTa for Question
 Answering - DeBERTa for Question Answering - XLM-RoBERTa for Question Answering
 - Longformer for Question Answering - Table Question Answering (TAPAS) - Zero-
-Shot NER Model - Neural Machine Translation (MarianMT) - Text-To-Text Transfer
-Transformer (Google T5) - Generative Pre-trained Transformer 2 (OpenAI GPT2) -
-Vision Transformer (ViT) - Swin Image Classification - Automatic Speech
-Recognition (Wav2Vec2) - Automatic Speech Recognition (HuBERT) - Named entity
-recognition (Deep learning) - Easy TensorFlow integration - GPU Support - Full
-integration with Spark ML functions - +9400 pre-trained models in +200
-languages! - +3200 pre-trained pipelines in +200 languages! - Multi-lingual NER
-models: Arabic, Bengali, Chinese, Danish, Dutch, English, Finnish, French,
-German, Hebrew, Italian, Japanese, Korean, Norwegian, Persian, Polish,
-Portuguese, Russian, Spanish, Swedish, Urdu, and more. ## Requirements To use
-Spark NLP you need the following requirements: - Java 8 and 11 - Apache Spark
-3.3.x, 3.2.x, 3.1.x, 3.0.x **GPU (optional):** Spark NLP 4.3.2 is built with
-TensorFlow 2.7.1 and the following NVIDIAÂ® software are only required for GPU
-support: - NVIDIAÂ® GPU drivers version 450.80.02 or higher - CUDAÂ® Toolkit
-11.2 - cuDNN SDK 8.1.0 ## Quick Start This is a quick example of how to use
-Spark NLP pre-trained pipeline in Python and PySpark: ```sh $ java -version #
-should be Java 8 or 11 (Oracle or OpenJDK) $ conda create -n sparknlp
-python=3.7 -y $ conda activate sparknlp # spark-nlp by default is based on
-pyspark 3.x $ pip install spark-nlp==4.3.2 pyspark==3.3.1 ``` In Python console
-or Jupyter `Python3` kernel: ```python # Import Spark NLP from sparknlp.base
-import * from sparknlp.annotator import * from sparknlp.pretrained import
-PretrainedPipeline import sparknlp # Start SparkSession with Spark NLP # start
-() functions has 3 parameters: gpu, apple_silicon, and memory # sparknlp.start
-(gpu=True) will start the session with GPU support # sparknlp.start
-(apple_silicon=True) will start the session with macOS M1 & M2 support #
-sparknlp.start(memory="16G") to change the default driver memory in
-SparkSession spark = sparknlp.start() # Download a pre-trained pipeline
-pipeline = PretrainedPipeline('explain_document_dl', lang='en') # Your testing
-dataset text = """ The Mona Lisa is a 16th century oil painting created by
-Leonardo. It's held at the Louvre in Paris. """ # Annotate your testing dataset
-result = pipeline.annotate(text) # What's in the pipeline list(result.keys())
-Output: ['entities', 'stem', 'checked', 'lemma', 'document', 'pos', 'token',
-'ner', 'embeddings', 'sentence'] # Check the results result['entities'] Output:
-['Mona Lisa', 'Leonardo', 'Louvre', 'Paris'] ``` For more examples, you can
-visit our dedicated [examples](https://github.com/JohnSnowLabs/spark-nlp/tree/
-master/examples) to showcase all Spark NLP use cases! ## Apache Spark Support
-Spark NLP *4.3.2* has been built on top of Apache Spark 3.2 while fully
-supports Apache Spark 3.0.x, 3.1.x, 3.2.x, and 3.3.x: | Spark NLP | Apache
-Spark 2.3.x | Apache Spark 2.4.x | Apache Spark 3.0.x | Apache Spark 3.1.x |
-Apache Spark 3.2.x | Apache Spark 3.3.x | |-----------|--------------------|---
------------------|--------------------|--------------------|-------------------
--|--------------------| | 4.3.x | NO | NO | YES | YES | YES | YES | | 4.2.x |
-NO | NO | YES | YES | YES | YES | | 4.1.x | NO | NO | YES | YES | YES | YES | |
-4.0.x | NO | NO | YES | YES | YES | YES | | 3.4.x | YES | YES | YES | YES |
-Partially | N/A | | 3.3.x | YES | YES | YES | YES | NO | NO | | 3.2.x | YES |
-YES | YES | YES | NO | NO | | 3.1.x | YES | YES | YES | YES | NO | NO | | 3.0.x
-| YES | YES | YES | YES | NO | NO | | 2.7.x | YES | YES | NO | NO | NO | NO |
-NOTE: Starting 4.0.0 release, the default `spark-nlp` and `spark-nlp-gpu`
-packages are based on Scala 2.12.15 and Apache Spark 3.2 by default. Find out
-more about `Spark NLP` versions from our [release notes](https://github.com/
-JohnSnowLabs/spark-nlp/releases). ## Scala and Python Support | Spark NLP |
-Python 3.6 | Python 3.7 | Python 3.8 | Python 3.9 | Scala 2.11 | Scala 2.12 |
-|-----------|------------|------------|------------|------------|------------|-
------------| | 4.3.x | YES | YES | YES | YES | NO | YES | | 4.2.x | YES | YES |
-YES | YES | NO | YES | | 4.1.x | YES | YES | YES | YES | NO | YES | | 4.0.x |
-YES | YES | YES | YES | NO | YES | | 3.4.x | YES | YES | YES | YES | YES | YES
-| | 3.3.x | YES | YES | YES | NO | YES | YES | | 3.2.x | YES | YES | YES | NO |
-YES | YES | | 3.1.x | YES | YES | YES | NO | YES | YES | | 3.0.x | YES | YES |
-YES | NO | YES | YES | | 2.7.x | YES | YES | NO | NO | YES | NO | ## Databricks
-Support Spark NLP 4.3.2 has been tested and is compatible with the following
-runtimes: **CPU:** - 7.3 - 7.3 ML - 9.1 - 9.1 ML - 10.1 - 10.1 ML - 10.2 - 10.2
-ML - 10.3 - 10.3 ML - 10.4 - 10.4 ML - 10.5 - 10.5 ML - 11.0 - 11.0 ML - 11.1 -
-11.1 ML - 11.2 - 11.2 ML - 11.3 - 11.3 ML **GPU:** - 9.1 ML & GPU - 10.1 ML &
-GPU - 10.2 ML & GPU - 10.3 ML & GPU - 10.4 ML & GPU - 10.5 ML & GPU - 11.0 ML &
-GPU - 11.1 ML & GPU - 11.2 ML & GPU - 11.3 ML & GPU NOTE: Spark NLP 4.x is
-based on TensorFlow 2.7.x which is compatible with CUDA11 and cuDNN 8.0.2. The
-only Databricks runtimes supporting CUDA 11 are 9.x and above as listed under
-GPU. ## EMR Support Spark NLP 4.3.2 has been tested and is compatible with the
-following EMR releases: - emr-6.2.0 - emr-6.3.0 - emr-6.3.1 - emr-6.4.0 - emr-
-6.5.0 - emr-6.6.0 - emr-6.7.0 Full list of [Amazon EMR 6.x releases](https://
+Shot NER Model - Zero Shot Text Classification by BERT (ZSL) - Neural Machine
+Translation (MarianMT) - Text-To-Text Transfer Transformer (Google T5) -
+Generative Pre-trained Transformer 2 (OpenAI GPT2) - Seq2Seq for NLG,
+Translation, and Comprehension (Facebook BART) - Vision Transformer (Google
+ViT) - Swin Image Classification (Microsoft Swin Transformer) - ConvNext Image
+Classification (Facebook ConvNext) - Automatic Speech Recognition (Wav2Vec2) -
+Automatic Speech Recognition (HuBERT) - Named entity recognition (Deep
+learning) - Easy TensorFlow integration - GPU Support - Full integration with
+Spark ML functions - +12000 pre-trained models in +200 languages! - +5000 pre-
+trained pipelines in +200 languages! - Multi-lingual NER models: Arabic,
+Bengali, Chinese, Danish, Dutch, English, Finnish, French, German, Hebrew,
+Italian, Japanese, Korean, Norwegian, Persian, Polish, Portuguese, Russian,
+Spanish, Swedish, Urdu, and more. ## Requirements To use Spark NLP you need the
+following requirements: - Java 8 and 11 - Apache Spark 3.3.x, 3.2.x, 3.1.x,
+3.0.x **GPU (optional):** Spark NLP 4.4.0 is built with TensorFlow 2.7.1 and
+the following NVIDIAÂ® software are only required for GPU support: - NVIDIAÂ®
+GPU drivers version 450.80.02 or higher - CUDAÂ® Toolkit 11.2 - cuDNN SDK 8.1.0
+## Quick Start This is a quick example of how to use Spark NLP pre-trained
+pipeline in Python and PySpark: ```sh $ java -version # should be Java 8 or 11
+(Oracle or OpenJDK) $ conda create -n sparknlp python=3.7 -y $ conda activate
+sparknlp # spark-nlp by default is based on pyspark 3.x $ pip install spark-
+nlp==4.4.0 pyspark==3.3.1 ``` In Python console or Jupyter `Python3` kernel:
+```python # Import Spark NLP from sparknlp.base import * from
+sparknlp.annotator import * from sparknlp.pretrained import PretrainedPipeline
+import sparknlp # Start SparkSession with Spark NLP # start() functions has 3
+parameters: gpu, apple_silicon, and memory # sparknlp.start(gpu=True) will
+start the session with GPU support # sparknlp.start(apple_silicon=True) will
+start the session with macOS M1 & M2 support # sparknlp.start(memory="16G") to
+change the default driver memory in SparkSession spark = sparknlp.start() #
+Download a pre-trained pipeline pipeline = PretrainedPipeline
+('explain_document_dl', lang='en') # Your testing dataset text = """ The Mona
+Lisa is a 16th century oil painting created by Leonardo. It's held at the
+Louvre in Paris. """ # Annotate your testing dataset result = pipeline.annotate
+(text) # What's in the pipeline list(result.keys()) Output: ['entities',
+'stem', 'checked', 'lemma', 'document', 'pos', 'token', 'ner', 'embeddings',
+'sentence'] # Check the results result['entities'] Output: ['Mona Lisa',
+'Leonardo', 'Louvre', 'Paris'] ``` For more examples, you can visit our
+dedicated [examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/
+examples) to showcase all Spark NLP use cases! ## Apache Spark Support Spark
+NLP *4.4.0* has been built on top of Apache Spark 3.2 while fully supports
+Apache Spark 3.0.x, 3.1.x, 3.2.x, and 3.3.x: | Spark NLP | Apache Spark 2.3.x |
+Apache Spark 2.4.x | Apache Spark 3.0.x | Apache Spark 3.1.x | Apache Spark
+3.2.x | Apache Spark 3.3.x | |-----------|--------------------|----------------
+----|--------------------|--------------------|--------------------|-----------
+---------| | 4.4.x | NO | NO | YES | YES | YES | YES | | 4.3.x | NO | NO | YES
+| YES | YES | YES | | 4.2.x | NO | NO | YES | YES | YES | YES | | 4.1.x | NO |
+NO | YES | YES | YES | YES | | 4.0.x | NO | NO | YES | YES | YES | YES | |
+3.4.x | YES | YES | YES | YES | Partially | N/A | | 3.3.x | YES | YES | YES |
+YES | NO | NO | | 3.2.x | YES | YES | YES | YES | NO | NO | | 3.1.x | YES | YES
+| YES | YES | NO | NO | | 3.0.x | YES | YES | YES | YES | NO | NO | | 2.7.x |
+YES | YES | NO | NO | NO | NO | NOTE: Starting 4.0.0 release, the default
+`spark-nlp` and `spark-nlp-gpu` packages are based on Scala 2.12.15 and Apache
+Spark 3.2 by default. Find out more about `Spark NLP` versions from our
+[release notes](https://github.com/JohnSnowLabs/spark-nlp/releases). ## Scala
+and Python Support | Spark NLP | Python 3.6 | Python 3.7 | Python 3.8 | Python
+3.9 | Python 3.10| Scala 2.11 | Scala 2.12 | |-----------|------------|--------
+----|------------|------------|------------|------------|------------| | 4.4.x
+| NO | YES | YES | YES | YES | NO | YES | | 4.3.x | YES | YES | YES | YES | YES
+| NO | YES | | 4.2.x | YES | YES | YES | YES | YES | NO | YES | | 4.1.x | YES |
+YES | YES | YES | NO | NO | YES | | 4.0.x | YES | YES | YES | YES | NO | NO |
+YES | | 3.4.x | YES | YES | YES | YES | NO | YES | YES | | 3.3.x | YES | YES |
+YES | NO | NO | YES | YES | | 3.2.x | YES | YES | YES | NO | NO | YES | YES | |
+3.1.x | YES | YES | YES | NO | NO | YES | YES | | 3.0.x | YES | YES | YES | NO
+| NO | YES | YES | | 2.7.x | YES | YES | NO | NO | NO | YES | NO | ##
+Databricks Support Spark NLP 4.4.0 has been tested and is compatible with the
+following runtimes: **CPU:** - 7.3 - 7.3 ML - 9.1 - 9.1 ML - 10.1 - 10.1 ML -
+10.2 - 10.2 ML - 10.3 - 10.3 ML - 10.4 - 10.4 ML - 10.5 - 10.5 ML - 11.0 - 11.0
+ML - 11.1 - 11.1 ML - 11.2 - 11.2 ML - 11.3 - 11.3 ML - 12.0 - 12.0 ML - 12.1 -
+12.1 ML - 12.2 - 12.2 ML **GPU:** - 9.1 ML & GPU - 10.1 ML & GPU - 10.2 ML &
+GPU - 10.3 ML & GPU - 10.4 ML & GPU - 10.5 ML & GPU - 11.0 ML & GPU - 11.1 ML &
+GPU - 11.2 ML & GPU - 11.3 ML & GPU - 12.0 ML & GPU - 12.1 ML & GPU - 12.2 ML &
+GPU NOTE: Spark NLP 4.x is based on TensorFlow 2.7.x which is compatible with
+CUDA11 and cuDNN 8.0.2. The only Databricks runtimes supporting CUDA 11 are 9.x
+and above as listed under GPU. ## EMR Support Spark NLP 4.4.0 has been tested
+and is compatible with the following EMR releases: - emr-6.2.0 - emr-6.3.0 -
+emr-6.3.1 - emr-6.4.0 - emr-6.5.0 - emr-6.6.0 - emr-6.7.0 - emr-6.8.0 - emr-
+6.9.0 - emr-6.10.0 Full list of [Amazon EMR 6.x releases](https://
 docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-release-6x.html) NOTE: The EMR
 6.1.0 and 6.1.1 are not supported. ## Usage ## Packages Cheatsheet This is a
 cheatsheet for corresponding Spark NLP Maven package to Apache Spark / PySpark
 major version: | Apache Spark | Spark NLP on CPU | Spark NLP on GPU | Spark NLP
 on AArch64 (linux) | Spark NLP on Apple Silicon | |-----------------|----------
 ----------|----------------------------|--------------------------------|------
 --------------------------------| | 3.0/3.1/3.2/3.3 | `spark-nlp` | `spark-nlp-
@@ -163,73 +170,73 @@
 architectures are limited by the community and we had to build most of the
 dependencies by ourselves to make them compatible. We support these two
 architectures, however, they may not work in some environments. ## Spark
 Packages ### Command line (requires internet connection) Spark NLP supports all
 major releases of Apache Spark 3.0.x, Apache Spark 3.1.x, Apache Spark 3.2.x,
 and Apache Spark 3.3.x. #### Apache Spark 3.x (3.0.x, 3.1.x, 3.2.x, and 3.3.x -
 Scala 2.12) ```sh # CPU spark-shell --packages com.johnsnowlabs.nlp:spark-
-nlp_2.12:4.3.2 pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2
-spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2 ``` The
+nlp_2.12:4.4.0 pyspark --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0
+spark-submit --packages com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0 ``` The
 `spark-nlp` has been published to the [Maven Repository](https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp). ```sh # GPU spark-
-shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.3.2 pyspark --
-packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.3.2 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.3.2 ``` The `spark-nlp-gpu` has been
+shell --packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.4.0 pyspark --
+packages com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.4.0 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp-gpu_2.12:4.4.0 ``` The `spark-nlp-gpu` has been
 published to the [Maven Repository](https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-gpu). ```sh # AArch64 spark-shell --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.3.2 pyspark --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.3.2 spark-submit --packages
-com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.3.2 ``` The `spark-nlp-aarch64`
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.4.0 pyspark --packages
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.4.0 spark-submit --packages
+com.johnsnowlabs.nlp:spark-nlp-aarch64_2.12:4.4.0 ``` The `spark-nlp-aarch64`
 has been published to the [Maven Repository](https://mvnrepository.com/
 artifact/com.johnsnowlabs.nlp/spark-nlp-aarch64). ```sh # M1/M2 (Apple Silicon)
-spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.3.2
-pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.3.2 spark-
-submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.3.2 ``` The
+spark-shell --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.4.0
+pyspark --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.4.0 spark-
+submit --packages com.johnsnowlabs.nlp:spark-nlp-silicon_2.12:4.4.0 ``` The
 `spark-nlp-silicon` has been published to the [Maven Repository](https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon). **NOTE**:
 In case you are using large pretrained models like UniversalSentenceEncoder,
 you need to have the following set in your SparkSession: ```sh spark-shell \ --
 driver-memory 16g \ --conf spark.kryoserializer.buffer.max=2000M \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2 ``` ## Scala Spark NLP supports Scala
+com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0 ``` ## Scala Spark NLP supports Scala
 2.12.15 if you are using Apache Spark 3.0.x, 3.1.x, 3.2.x, and 3.3.x versions.
 Our packages are deployed to Maven central. To add any of our packages as a
 dependency in your application you can follow these coordinates: ### Maven
 **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, and 3.3.x: ```xml
-com.johnsnowlabs.nlp spark-nlp_2.12 4.3.2  ``` **spark-nlp-gpu:** ```xml
-com.johnsnowlabs.nlp spark-nlp-gpu_2.12 4.3.2  ``` **spark-nlp-aarch64:**
-```xml   com.johnsnowlabs.nlp spark-nlp-aarch64_2.12 4.3.2  ``` **spark-nlp-
-silicon:** ```xml   com.johnsnowlabs.nlp spark-nlp-silicon_2.12 4.3.2  ``` ###
+com.johnsnowlabs.nlp spark-nlp_2.12 4.4.0  ``` **spark-nlp-gpu:** ```xml
+com.johnsnowlabs.nlp spark-nlp-gpu_2.12 4.4.0  ``` **spark-nlp-aarch64:**
+```xml   com.johnsnowlabs.nlp spark-nlp-aarch64_2.12 4.4.0  ``` **spark-nlp-
+silicon:** ```xml   com.johnsnowlabs.nlp spark-nlp-silicon_2.12 4.4.0  ``` ###
 SBT **spark-nlp** on Apache Spark 3.0.x, 3.1.x, 3.2.x, and 3.3.x: ```sbtshell /
 / https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "4.3.2" ```
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp" % "4.4.0" ```
 **spark-nlp-gpu:** ```sbtshell // https://mvnrepository.com/artifact/
 com.johnsnowlabs.nlp/spark-nlp-gpu libraryDependencies +=
-"com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "4.3.2" ``` **spark-nlp-aarch64:**
+"com.johnsnowlabs.nlp" %% "spark-nlp-gpu" % "4.4.0" ``` **spark-nlp-aarch64:**
 ```sbtshell // https://mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-
 nlp-aarch64 libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-
-aarch64" % "4.3.2" ``` **spark-nlp-silicon:** ```sbtshell // https://
+aarch64" % "4.4.0" ``` **spark-nlp-silicon:** ```sbtshell // https://
 mvnrepository.com/artifact/com.johnsnowlabs.nlp/spark-nlp-silicon
-libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "4.3.2"
+libraryDependencies += "com.johnsnowlabs.nlp" %% "spark-nlp-silicon" % "4.4.0"
 ``` Maven Central: [https://mvnrepository.com/artifact/com.johnsnowlabs.nlp]
 (https://mvnrepository.com/artifact/com.johnsnowlabs.nlp) If you are
 interested, there is a simple SBT project for Spark NLP to guide you on how to
 use it in your projects [Spark NLP SBT Starter](https://github.com/
 maziyarpanahi/spark-nlp-starter) ## Python Spark NLP supports Python 3.6.x and
 above depending on your major PySpark version. ### Python without explicit
 Pyspark installation ### Pip/Conda If you installed pyspark through pip/conda,
 you can install `spark-nlp` through the same channel. Pip: ```bash pip install
-spark-nlp==4.3.2 ``` Conda: ```bash conda install -c johnsnowlabs spark-nlp ```
+spark-nlp==4.4.0 ``` Conda: ```bash conda install -c johnsnowlabs spark-nlp ```
 PyPI [spark-nlp package](https://pypi.org/project/spark-nlp/) / Anaconda
 [spark-nlp package](https://anaconda.org/JohnSnowLabs/spark-nlp) Then you'll
 have to create a SparkSession either from Spark NLP: ```python import sparknlp
 spark = sparknlp.start() ``` or manually: ```python spark =
 SparkSession.builder .appName("Spark NLP") .master("local[*]") .config
 ("spark.driver.memory", "16G") .config("spark.driver.maxResultSize", "0")
 .config("spark.kryoserializer.buffer.max", "2000M") .config
-("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2")
+("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0")
 .getOrCreate() ``` If using local jars, you can use `spark.jars` instead for
 comma-delimited jar files. For cluster setups, of course, you'll have to put
 the jars in a reachable location for all driver and executor nodes. **Quick
 example:** ```python import sparknlp from sparknlp.pretrained import
 PretrainedPipeline # create or get Spark Session spark = sparknlp.start()
 sparknlp.version() spark.version # download, load and annotate a text by pre-
 trained pipeline pipeline = PretrainedPipeline('recognize_entities_dl', 'en')
@@ -243,71 +250,71 @@
 download the Fat JARs provided here or download it from [Maven Central](https:/
 /mvnrepository.com/artifact/com.johnsnowlabs.nlp). To add JARs to spark
 programs use the `--jars` option: ```sh spark-shell --jars spark-nlp.jar ```
 The preferred way to use the library when running spark programs is using the
 `--packages` option as specified in the `spark-packages` section. ## Apache
 Zeppelin Use either one of the following options - Add the following Maven
 Coordinates to the interpreter's library list ```bash com.johnsnowlabs.nlp:
-spark-nlp_2.12:4.3.2 ``` - Add a path to pre-built jar from [here](#compiled-
+spark-nlp_2.12:4.4.0 ``` - Add a path to pre-built jar from [here](#compiled-
 jars) in the interpreter's library list making sure the jar is available to
 driver path ### Python in Zeppelin Apart from the previous step, install the
-python module through pip ```bash pip install spark-nlp==4.3.2 ``` Or you can
+python module through pip ```bash pip install spark-nlp==4.4.0 ``` Or you can
 install `spark-nlp` from inside Zeppelin by using Conda: ```bash python.conda
 install -c johnsnowlabs spark-nlp ``` Configure Zeppelin properly, use cells
 with %spark.pyspark or any interpreter name you chose. Finally, in Zeppelin
 interpreter settings, make sure you set properly zeppelin.python to the python
 you want to use and install the pip library with (e.g. `python3`). An
 alternative option would be to set `SPARK_SUBMIT_OPTIONS` (zeppelin-env.sh) and
 make sure `--packages` is there as shown earlier since it includes both scala
 and python side installation. ## Jupyter Notebook (Python) **Recommended:** The
 easiest way to get this done on Linux and macOS is to simply install `spark-
 nlp` and `pyspark` PyPI packages and launch the Jupyter from the same Python
 environment: ```sh $ conda create -n sparknlp python=3.8 -y $ conda activate
 sparknlp # spark-nlp by default is based on pyspark 3.x $ pip install spark-
-nlp==4.3.2 pyspark==3.3.1 jupyter $ jupyter notebook ``` Then you can use
+nlp==4.4.0 pyspark==3.3.1 jupyter $ jupyter notebook ``` Then you can use
 `python3` kernel to run your code with creating SparkSession via `spark =
 sparknlp.start()`. **Optional:** If you are in different operating systems and
 require to make Jupyter Notebook run by using pyspark, you can follow these
 steps: ```bash export SPARK_HOME=/path/to/your/spark/folder export
 PYSPARK_PYTHON=python3 export PYSPARK_DRIVER_PYTHON=jupyter export
 PYSPARK_DRIVER_PYTHON_OPTS=notebook pyspark --packages com.johnsnowlabs.nlp:
-spark-nlp_2.12:4.3.2 ``` Alternatively, you can mix in using `--jars` option
+spark-nlp_2.12:4.4.0 ``` Alternatively, you can mix in using `--jars` option
 for pyspark + `pip install spark-nlp` If not using pyspark at all, you'll have
 to run the instructions pointed [here](#python-without-explicit-Pyspark-
 installation) ## Google Colab Notebook Google Colab is perhaps the easiest way
 to get started with spark-nlp. It requires no installation or setup other than
 having a Google account. Run the following code in Google Colab notebook and
 start using spark-nlp right away. ```sh # This is only to setup PySpark and
 Spark NLP on Colab !wget https://setup.johnsnowlabs.com/colab.sh -O - | bash
 ``` This script comes with the two options to define `pyspark` and `spark-nlp`
 versions via options: ```sh # -p is for pyspark # -s is for spark-nlp # -g will
 enable upgrading libcudnn8 to 8.1.0 on Google Colab for GPU usage # by default
 they are set to the latest !wget https://setup.johnsnowlabs.com/colab.sh -O - |
-bash /dev/stdin -p 3.2.3 -s 4.3.2 ``` [Spark NLP quick start on Google Colab]
+bash /dev/stdin -p 3.2.3 -s 4.4.0 ``` [Spark NLP quick start on Google Colab]
 (https://colab.research.google.com/github/JohnSnowLabs/spark-nlp/blob/master/
 examples/python/quick_start_google_colab.ipynb) is a live demo on Google Colab
 that performs named entity recognitions and sentiment analysis by using Spark
 NLP pretrained pipelines. ## Kaggle Kernel Run the following code in Kaggle
 Kernel and start using spark-nlp right away. ```sh # Let's setup Kaggle for
 Spark NLP and PySpark !wget https://setup.johnsnowlabs.com/kaggle.sh -O - |
 bash ``` This script comes with the two options to define `pyspark` and `spark-
 nlp` versions via options: ```sh # -p is for pyspark # -s is for spark-nlp # -
 g will enable upgrading libcudnn8 to 8.1.0 on Kaggle for GPU usage # by default
 they are set to the latest !wget https://setup.johnsnowlabs.com/colab.sh -O - |
-bash /dev/stdin -p 3.2.3 -s 4.3.2 ``` [Spark NLP quick start on Kaggle Kernel]
+bash /dev/stdin -p 3.2.3 -s 4.4.0 ``` [Spark NLP quick start on Kaggle Kernel]
 (https://www.kaggle.com/mozzie/spark-nlp-named-entity-recognition) is a live
 demo on Kaggle Kernel that performs named entity recognitions by using Spark
 NLP pretrained pipeline. ## Databricks Cluster 1. Create a cluster if you don't
 have one already 2. On a new cluster or existing one you need to add the
 following to the `Advanced Options -> Spark` tab: ```bash
 spark.kryoserializer.buffer.max 2000M spark.serializer
 org.apache.spark.serializer.KryoSerializer ``` 3. In `Libraries` tab inside
 your cluster you need to follow these steps: 3.1. Install New -> PyPI -
-> `spark-nlp==4.3.2` -> Install 3.2. Install New -> Maven -> Coordinates -
-> `com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2` -> Install 4. Now you can attach
+> `spark-nlp==4.4.0` -> Install 3.2. Install New -> Maven -> Coordinates -
+> `com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0` -> Install 4. Now you can attach
 your notebook to the cluster and use Spark NLP! NOTE: Databricks' runtimes
 support different Apache Spark major releases. Please make sure you choose the
 correct Spark NLP Maven package name (Maven Coordinate) for your runtime from
 our [Packages Cheatsheet](https://github.com/JohnSnowLabs/spark-nlp#packages-
 cheatsheet) ## EMR Cluster To launch EMR clusters with Apache Spark/PySpark and
 Spark NLP correctly you need to have bootstrap and software configuration. A
 sample of your bootstrap script ```.sh #!/bin/bash set -x -e echo -e 'export
@@ -318,16 +325,16 @@
 S3 (must be public access): ```.json [{ "Classification": "spark-env",
 "Configurations": [{ "Classification": "export", "Properties":
 { "PYSPARK_PYTHON": "/usr/bin/python3" } }] }, { "Classification": "spark-
 defaults", "Properties": { "spark.yarn.stagingDir": "hdfs:///tmp",
 "spark.yarn.preserve.staging.files": "true", "spark.kryoserializer.buffer.max":
 "2000M", "spark.serializer": "org.apache.spark.serializer.KryoSerializer",
 "spark.driver.maxResultSize": "0", "spark.jars.packages":
-"com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2" } }] ``` A sample of AWS CLI to
-launch EMR cluster: ```.sh aws emr create-cluster \ --name "Spark NLP 4.3.2" \
+"com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0" } }] ``` A sample of AWS CLI to
+launch EMR cluster: ```.sh aws emr create-cluster \ --name "Spark NLP 4.4.0" \
 --release-label emr-6.2.0 \ --applications Name=Hadoop Name=Spark Name=Hive \ -
 -instance-type m4.4xlarge \ --instance-count 3 \ --use-default-roles \ --log-
 uri "s3:///" \ --bootstrap-actions Path=s3:///emr-bootstrap.sh,Name=custome \ -
 -configurations "https:///sparknlp-config.json" \ --ec2-attributes
 KeyName=,EmrManagedMasterSecurityGroup=,EmrManagedSlaveSecurityGroup= \ --
 profile  ``` ## GCP Dataproc 1. Create a cluster if you don't have one already
 as follows. At gcloud shell: ```bash gcloud services enable
@@ -346,15 +353,15 @@
 boot-disk-size=128GB \ --num-workers=2 \ --bucket=${BUCKET_NAME} \ --optional-
 components=JUPYTER \ --enable-component-gateway \ --metadata
 'PIP_PACKAGES=spark-nlp spark-nlp-display google-cloud-bigquery google-cloud-
 storage' \ --initialization-actions gs://goog-dataproc-initialization-actions-$
 {REGION}/python/pip-install.sh \ --properties spark:
 spark.serializer=org.apache.spark.serializer.KryoSerializer,spark:
 spark.driver.maxResultSize=0,spark:spark.kryoserializer.buffer.max=2000M,spark:
-spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2 ``` 2. On an
+spark.jars.packages=com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0 ``` 2. On an
 existing one, you need to install spark-nlp and spark-nlp-display packages from
 PyPI. 3. Now, you can attach your notebook to the cluster and use the Spark
 NLP! ## Spark NLP Configuration You can change the following Spark NLP
 configurations via Spark Configuration: | Property Name | Default | Meaning |
 |--------------------------------------------------------|---------------------
 -|-----------------------------------------------------------------------------
 -------------------------------------------------------------------------------
@@ -390,28 +397,28 @@
 configurations. ```python from pyspark.sql import SparkSession spark =
 SparkSession.builder .master("local[*]") .config("spark.driver.memory", "16G")
 .config("spark.driver.maxResultSize", "0") .config("spark.serializer",
 "org.apache.spark.serializer.KryoSerializer") .config
 ("spark.kryoserializer.buffer.max", "2000m") .config
 ("spark.jsl.settings.pretrained.cache_folder", "sample_data/pretrained")
 .config("spark.jsl.settings.storage.cluster_tmp_dir", "sample_data/storage")
-.config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2")
+.config("spark.jars.packages", "com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0")
 .getOrCreate() ``` **spark-shell:** ```sh spark-shell \ --driver-memory 16g \ -
 -conf spark.driver.maxResultSize=0 \ --conf
 spark.serializer=org.apache.spark.serializer.KryoSerializer --conf
 spark.kryoserializer.buffer.max=2000M \ --conf
 spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \ --conf
 spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2 ``` **pyspark:** ```sh pyspark \ --
+com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0 ``` **pyspark:** ```sh pyspark \ --
 driver-memory 16g \ --conf spark.driver.maxResultSize=0 \ --conf
 spark.serializer=org.apache.spark.serializer.KryoSerializer --conf
 spark.kryoserializer.buffer.max=2000M \ --conf
 spark.jsl.settings.pretrained.cache_folder="sample_data/pretrained" \ --conf
 spark.jsl.settings.storage.cluster_tmp_dir="sample_data/storage" \ --packages
-com.johnsnowlabs.nlp:spark-nlp_2.12:4.3.2 ``` **Databricks:** On a new cluster
+com.johnsnowlabs.nlp:spark-nlp_2.12:4.4.0 ``` **Databricks:** On a new cluster
 or existing one you need to add the following to the `Advanced Options -
 > Spark` tab: ```bash spark.kryoserializer.buffer.max 2000M spark.serializer
 org.apache.spark.serializer.KryoSerializer
 spark.jsl.settings.pretrained.cache_folder dbfs:/PATH_TO_CACHE
 spark.jsl.settings.storage.cluster_tmp_dir dbfs:/PATH_TO_STORAGE
 spark.jsl.settings.annotator.log_folder dbfs:/PATH_TO_LOGS ``` NOTE: If this is
 an existing cluster, after adding new configs or changing existing properties
@@ -490,36 +497,35 @@
 ResourceDownloader.showPublicPipelines(lang = "en", version = "3.1.0") /* +----
 -----------------------------------+------+---------+ | Pipeline | lang |
 version | +---------------------------------------+------+---------+ |
 dependency_parse | en | 2.0.2 | ... | clean_slang | en | 3.0.0 | |
 clean_pattern | en | 3.0.0 | | check_spelling | en | 3.0.0 | | dependency_parse
 | en | 3.0.0 | +---------------------------------------+------+---------+ */
 ``` #### Please check out our Models Hub for the full list of [pre-trained
-pipelines](https://nlp.johnsnowlabs.com/models) with examples, demos,
-benchmarks, and more ### Models **Some selected languages: ** `Afrikaans,
-Arabic, Armenian, Basque, Bengali, Breton, Bulgarian, Catalan, Czech, Dutch,
-English, Esperanto, Finnish, French, Galician, German, Greek, Hausa, Hebrew,
-Hindi, Hungarian, Indonesian, Irish, Italian, Japanese, Latin, Latvian,
-Marathi, Norwegian, Persian, Polish, Portuguese, Romanian, Russian, Slovak,
-Slovenian, Somali, Southern Sotho, Spanish, Swahili, Swedish, Tswana, Turkish,
-Ukrainian, Zulu` **Quick online example:** ```python # load NER model trained
-by deep learning approach and GloVe word embeddings ner_dl =
-NerDLModel.pretrained('ner_dl') # load NER model trained by deep learning
-approach and BERT word embeddings ner_bert = NerDLModel.pretrained
-('ner_dl_bert') ``` ```scala // load French POS tagger model trained by
-Universal Dependencies val french_pos = PerceptronModel.pretrained
-("pos_ud_gsd", lang = "fr") // load Italian LemmatizerModel val italian_lemma =
-LemmatizerModel.pretrained("lemma_dxc", lang = "it") ```` **Quick offline
-example:** - Loading `PerceptronModel` annotator model inside Spark NLP
-Pipeline ```scala val french_pos = PerceptronModel.load("/tmp/
-pos_ud_gsd_fr_2.0.2_2.4_1556531457346/") .setInputCols("document", "token")
-.setOutputCol("pos") ``` #### Showing Available Models There are functions in
-Spark NLP that will list all the available Models of a particular Annotator and
-language for you: ```scala import
-com.johnsnowlabs.nlp.pretrained.ResourceDownloader
+pipelines](https://sparknlp.org/models) with examples, demos, benchmarks, and
+more ### Models **Some selected languages: ** `Afrikaans, Arabic, Armenian,
+Basque, Bengali, Breton, Bulgarian, Catalan, Czech, Dutch, English, Esperanto,
+Finnish, French, Galician, German, Greek, Hausa, Hebrew, Hindi, Hungarian,
+Indonesian, Irish, Italian, Japanese, Latin, Latvian, Marathi, Norwegian,
+Persian, Polish, Portuguese, Romanian, Russian, Slovak, Slovenian, Somali,
+Southern Sotho, Spanish, Swahili, Swedish, Tswana, Turkish, Ukrainian, Zulu`
+**Quick online example:** ```python # load NER model trained by deep learning
+approach and GloVe word embeddings ner_dl = NerDLModel.pretrained('ner_dl') #
+load NER model trained by deep learning approach and BERT word embeddings
+ner_bert = NerDLModel.pretrained('ner_dl_bert') ``` ```scala // load French POS
+tagger model trained by Universal Dependencies val french_pos =
+PerceptronModel.pretrained("pos_ud_gsd", lang = "fr") // load Italian
+LemmatizerModel val italian_lemma = LemmatizerModel.pretrained("lemma_dxc",
+lang = "it") ```` **Quick offline example:** - Loading `PerceptronModel`
+annotator model inside Spark NLP Pipeline ```scala val french_pos =
+PerceptronModel.load("/tmp/pos_ud_gsd_fr_2.0.2_2.4_1556531457346/")
+.setInputCols("document", "token") .setOutputCol("pos") ``` #### Showing
+Available Models There are functions in Spark NLP that will list all the
+available Models of a particular Annotator and language for you: ```scala
+import com.johnsnowlabs.nlp.pretrained.ResourceDownloader
 ResourceDownloader.showPublicModels(annotator = "NerDLModel", lang = "en") /
 * +---------------------------------------------+------+---------+ | Model |
 lang | version | +---------------------------------------------+------+--------
 -+ | onto_100 | en | 2.1.0 | | onto_300 | en | 2.1.0 | | ner_dl_bert | en |
 2.2.0 | | onto_100 | en | 2.4.0 | | ner_conll_elmo | en | 3.2.2 | +------------
 ---------------------------------+------+---------+ */ ``` Or if we want to
 check for a particular version: ```scala import
@@ -531,40 +537,40 @@
 ner_weibo_glove_840B_300d | en | 2.6.2 | | nerdl_atis_840b_300d | en | 2.7.1 |
 | nerdl_snips_100d | en | 2.7.3 | +----------------------------+------+--------
 -+ */ ``` And to see a list of available annotators, you can use: ```scala
 import com.johnsnowlabs.nlp.pretrained.ResourceDownloader
 ResourceDownloader.showAvailableAnnotators() /* AlbertEmbeddings
 AlbertForTokenClassification AssertionDLModel ... XlmRoBertaSentenceEmbeddings
 XlnetEmbeddings */ ``` #### Please check out our Models Hub for the full list
-of [pre-trained models](https://nlp.johnsnowlabs.com/models) with examples,
-demo, benchmark, and more ## Offline Spark NLP library and all the pre-trained
+of [pre-trained models](https://sparknlp.org/models) with examples, demo,
+benchmark, and more ## Offline Spark NLP library and all the pre-trained
 models/pipelines can be used entirely offline with no access to the Internet.
 If you are behind a proxy or a firewall with no access to the Maven repository
 (to download packages) or/and no access to S3 (to automatically download models
 and pipelines), you can simply follow the instructions to have Spark NLP
 without any limitations offline: - Instead of using the Maven package, you need
 to load our Fat JAR - Instead of using PretrainedPipeline for pretrained
 pipelines or the `.pretrained()` function to download pretrained models, you
 will need to manually download your pipeline/model from [Models Hub](https://
-nlp.johnsnowlabs.com/models), extract it, and load it. Example of
-`SparkSession` with Fat JAR to have Spark NLP offline: ```python spark =
-SparkSession.builder .appName("Spark NLP") .master("local[*]") .config
-("spark.driver.memory", "16G") .config("spark.driver.maxResultSize", "0")
-.config("spark.kryoserializer.buffer.max", "2000M") .config("spark.jars", "/
-tmp/spark-nlp-assembly-4.3.2.jar") .getOrCreate() ``` - You can download
-provided Fat JARs from each [release notes](https://github.com/JohnSnowLabs/
-spark-nlp/releases), please pay attention to pick the one that suits your
-environment depending on the device (CPU/GPU) and Apache Spark version (3.0.x,
-3.1.x, 3.2.x, and 3.3.x) - If you are local, you can load the Fat JAR from your
-local FileSystem, however, if you are in a cluster setup you need to put the
-Fat JAR on a distributed FileSystem such as HDFS, DBFS, S3, etc. ( i.e., `hdfs:
-///tmp/spark-nlp-assembly-4.3.2.jar`) Example of using pretrained Models and
-Pipelines in offline: ```python # instead of using pretrained() for online: #
-french_pos = PerceptronModel.pretrained("pos_ud_gsd", lang="fr") # you download
-this model, extract it, and use .load french_pos = PerceptronModel.load("/tmp/
+sparknlp.org/models), extract it, and load it. Example of `SparkSession` with
+Fat JAR to have Spark NLP offline: ```python spark = SparkSession.builder
+.appName("Spark NLP") .master("local[*]") .config("spark.driver.memory", "16G")
+.config("spark.driver.maxResultSize", "0") .config
+("spark.kryoserializer.buffer.max", "2000M") .config("spark.jars", "/tmp/spark-
+nlp-assembly-4.4.0.jar") .getOrCreate() ``` - You can download provided Fat
+JARs from each [release notes](https://github.com/JohnSnowLabs/spark-nlp/
+releases), please pay attention to pick the one that suits your environment
+depending on the device (CPU/GPU) and Apache Spark version (3.0.x, 3.1.x,
+3.2.x, and 3.3.x) - If you are local, you can load the Fat JAR from your local
+FileSystem, however, if you are in a cluster setup you need to put the Fat JAR
+on a distributed FileSystem such as HDFS, DBFS, S3, etc. ( i.e., `hdfs:///tmp/
+spark-nlp-assembly-4.4.0.jar`) Example of using pretrained Models and Pipelines
+in offline: ```python # instead of using pretrained() for online: # french_pos
+= PerceptronModel.pretrained("pos_ud_gsd", lang="fr") # you download this
+model, extract it, and use .load french_pos = PerceptronModel.load("/tmp/
 pos_ud_gsd_fr_2.0.2_2.4_1556531457346/") .setInputCols("document", "token")
 .setOutputCol("pos") # example for pipelines # instead of using
 PretrainedPipeline # pipeline = PretrainedPipeline('explain_document_dl',
 lang='en') # you download this pipeline, extract it, and use PipelineModel
 PipelineModel.load("/tmp/explain_document_dl_en_2.0.2_2.4_1556530585689/") ```
 - Since you are downloading and loading models/pipelines manually, this means
 Spark NLP is not downloading the most recent and compatible models/pipelines
@@ -572,31 +578,31 @@
 can load the model/pipeline from your local FileSystem, however, if you are in
 a cluster setup you need to put the model/pipeline on a distributed FileSystem
 such as HDFS, DBFS, S3, etc. ( i.e., `hdfs:///tmp/
 explain_document_dl_en_2.0.2_2.4_1556530585689/`) ## Examples Need more
 **examples**? Check out our dedicated [Spark NLP Examples](https://github.com/
 JohnSnowLabs/spark-nlp/tree/master/examples) repository to showcase all Spark
 NLP use cases! Also, don't forget to check [Spark NLP in Action](https://
-nlp.johnsnowlabs.com/demo) built by Streamlit. ### All examples: [spark-nlp/
-examples](https://github.com/JohnSnowLabs/spark-nlp/tree/master/examples) ##
-FAQ [Check our Articles and Videos page here](https://nlp.johnsnowlabs.com/
-learn) ## Citation We have published a [paper](https://www.sciencedirect.com/
-science/article/pii/S2665963821000063) that you can cite for the Spark NLP
-library: ```bibtex @article{KOCAMAN2021100058, title = {Spark NLP: Natural
-language understanding at scale}, journal = {Software Impacts}, pages =
-{100058}, year = {2021}, issn = {2665-9638}, doi = {https://doi.org/10.1016/
-j.simpa.2021.100058}, url = {https://www.sciencedirect.com/science/article/pii/
-S2665963.2.300063}, author = {Veysel Kocaman and David Talby}, keywords =
-{Spark, Natural language processing, Deep learning, Tensorflow, Cluster},
-abstract = {Spark NLP is a Natural Language Processing (NLP) library built on
-top of Apache Spark ML. It provides simple, performant & accurate NLP
-annotations for machine learning pipelines that can scale easily in a
-distributed environment. Spark NLP comes with 1100+ pretrained pipelines and
-models in more than 192+ languages. It supports nearly all the NLP tasks and
-modules that can be used seamlessly in a cluster. Downloaded more than 2.7
-million times and experiencing 9x growth since January 2020, Spark NLP is used
-by 54% of healthcare organizations as the worldâs most widely used NLP
-library in the enterprise.} } } ``` ## Contributing We appreciate any sort of
-contributions: - ideas - feedback - documentation - bug reports - NLP training
-and testing corpora - Development and testing Clone the repo and submit your
-pull-requests! Or directly create issues in this repo. ## John Snow Labs [http:
-//johnsnowlabs.com](http://johnsnowlabs.com)
+sparknlp.org/demo) built by Streamlit. ### All examples: [spark-nlp/examples]
+(https://github.com/JohnSnowLabs/spark-nlp/tree/master/examples) ## FAQ [Check
+our Articles and Videos page here](https://sparknlp.org/learn) ## Citation We
+have published a [paper](https://www.sciencedirect.com/science/article/pii/
+S2665963821000063) that you can cite for the Spark NLP library: ```bibtex
+@article{KOCAMAN2021100058, title = {Spark NLP: Natural language understanding
+at scale}, journal = {Software Impacts}, pages = {100058}, year = {2021}, issn
+= {2665-9638}, doi = {https://doi.org/10.1016/j.simpa.2021.100058}, url =
+{https://www.sciencedirect.com/science/article/pii/S2665963.2.300063}, author =
+{Veysel Kocaman and David Talby}, keywords = {Spark, Natural language
+processing, Deep learning, Tensorflow, Cluster}, abstract = {Spark NLP is a
+Natural Language Processing (NLP) library built on top of Apache Spark ML. It
+provides simple, performant & accurate NLP annotations for machine learning
+pipelines that can scale easily in a distributed environment. Spark NLP comes
+with 1100+ pretrained pipelines and models in more than 192+ languages. It
+supports nearly all the NLP tasks and modules that can be used seamlessly in a
+cluster. Downloaded more than 2.7 million times and experiencing 9x growth
+since January 2020, Spark NLP is used by 54% of healthcare organizations as the
+worldâs most widely used NLP library in the enterprise.} } } ``` ##
+Contributing We appreciate any sort of contributions: - ideas - feedback -
+documentation - bug reports - NLP training and testing corpora - Development
+and testing Clone the repo and submit your pull-requests! Or directly create
+issues in this repo. ## John Snow Labs [http://johnsnowlabs.com](http://
+johnsnowlabs.com)
```

