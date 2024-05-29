# Comparing `tmp/nutcracker-py-0.0.1a36.tar.gz` & `tmp/nutcracker-py-0.0.1a37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutcracker-py-0.0.1a36.tar", last modified: Sun Mar 17 11:22:15 2024, max compression
+gzip compressed data, was "nutcracker-py-0.0.1a37.tar", last modified: Sun Mar 17 15:42:43 2024, max compression
```

## Comparing `nutcracker-py-0.0.1a36.tar` & `nutcracker-py-0.0.1a37.tar`

### file list

```diff
@@ -1,147 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.368288 nutcracker-py-0.0.1a36/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.352288 nutcracker-py-0.0.1a36/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.352288 nutcracker-py-0.0.1a36/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/.github/workflows/pipy_release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-03-17 11:22:15.368288 nutcracker-py-0.0.1a36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.352288 nutcracker-py-0.0.1a36/nutcracker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.352288 nutcracker-py-0.0.1a36/nutcracker/data/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.352288 nutcracker-py-0.0.1a36/nutcracker/data/data_config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.352288 nutcracker-py-0.0.1a36/nutcracker/data/data_config/pile/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/pile/hf-open-llm-leaderboard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/pile/htest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/pile/math.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/pile/mmlu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.364288 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/aqua-rat.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/arc-challenge.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/arc-easy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/commonsenseqa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/gsm8k.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/hellaswag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/hhh-alignment-harmless.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/hhh-alignment-helpful.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/hhh-alignment-honest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/hhh-alignment-other.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-end-ly.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-end-punctuation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-hyphenated-word.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-palindrome.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-repeated-word.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-rhyme.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-spelled-math.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-spelled-number.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-start-vowel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/htest-uppercase.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/math-algebra.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/math-counting-and-probability.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/math-geometry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/math-intermediate-algebra.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/math-number-theory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/math-prealgebra.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/math-precalculus.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/medqa-usmle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-abstract-algebra.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-anatomy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-astronomy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-business-ethics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-clinical-knowledge.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-college-biology.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-college-chemistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-college-computer-science.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-college-mathematics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-college-medicine.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-college-physics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-computer-security.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-conceptual-physics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-econometrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-electrical-engineering.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-elementary-mathematics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-formal-logic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-global-facts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-biology.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-chemistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-computer-science.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-european-history.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-geography.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-government-and-politics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-macroeconomics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-mathematics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-microeconomics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-physics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-psychology.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-statistics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-us-history.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-high-school-world-history.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-human-aging.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-human-sexuality.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-international-law.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-jurisprudence.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-logical-fallacies.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-machine-learning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-management.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-marketing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-medical-genetics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-miscellaneous.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-moral-disputes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-moral-scenarios.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-nutrition.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-philosophy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-prehistory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-professional-accounting.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-professional-law.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-professional-medicine.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-professional-psychology.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-public-relations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-security-studies.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-sociology.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-us-foreign-policy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-virology.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/mmlu-world-religions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/openbookqa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/piqa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/socialiqa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/truthfulqa-mc1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/data_config/task/winogrande.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/instance_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/pile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/data/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.364288 nutcracker-py-0.0.1a36/nutcracker/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/auto_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.364288 nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/frq_engine_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/frq_engine_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/mcq_engine_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/mcq_engine_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/mcq_engine_gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/mcq_engine_zeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/frq_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/mcq_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/evaluator/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.364288 nutcracker-py-0.0.1a36/nutcracker/runs/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/runs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/runs/inquiry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/runs/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/runs/study.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.364288 nutcracker-py-0.0.1a36/nutcracker/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.364288 nutcracker-py-0.0.1a36/nutcracker/tests/mcq_evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/tests/mcq_evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/nutcracker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:15.368288 nutcracker-py-0.0.1a36/nutcracker_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-03-17 11:22:15.000000 nutcracker-py-0.0.1a36/nutcracker_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-03-17 11:22:15.000000 nutcracker-py-0.0.1a36/nutcracker_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 11:22:15.000000 nutcracker-py-0.0.1a36/nutcracker_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-17 11:22:15.000000 nutcracker-py-0.0.1a36/nutcracker_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-17 11:22:15.000000 nutcracker-py-0.0.1a36/nutcracker_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 11:22:15.368288 nutcracker-py-0.0.1a36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-17 11:22:07.000000 nutcracker-py-0.0.1a36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.345879 nutcracker-py-0.0.1a37/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.329879 nutcracker-py-0.0.1a37/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.329879 nutcracker-py-0.0.1a37/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/.github/workflows/pipy_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-03-17 15:42:43.345879 nutcracker-py-0.0.1a37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.329879 nutcracker-py-0.0.1a37/nutcracker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.329879 nutcracker-py-0.0.1a37/nutcracker/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.329879 nutcracker-py-0.0.1a37/nutcracker/data/data_config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.333879 nutcracker-py-0.0.1a37/nutcracker/data/data_config/pile/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/pile/hf-open-llm-leaderboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/pile/htest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/pile/math.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/pile/mmlu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.341879 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/aqua-rat.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/arc-challenge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/arc-easy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/commonsenseqa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/gsm8k.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/hellaswag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/hhh-alignment-harmless.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/hhh-alignment-helpful.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/hhh-alignment-honest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/hhh-alignment-other.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-end-ly.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-end-punctuation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-hyphenated-word.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-palindrome.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-repeated-word.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-rhyme.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-spelled-math.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-spelled-number.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-start-vowel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/htest-uppercase.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/math-algebra.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/math-counting-and-probability.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/math-geometry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/math-intermediate-algebra.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/math-number-theory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/math-prealgebra.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/math-precalculus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/medqa-usmle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-abstract-algebra.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-anatomy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-astronomy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-business-ethics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-clinical-knowledge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-college-biology.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-college-chemistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-college-computer-science.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-college-mathematics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-college-medicine.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-college-physics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-computer-security.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-conceptual-physics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-econometrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-electrical-engineering.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-elementary-mathematics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-formal-logic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-global-facts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-biology.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-chemistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-computer-science.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-european-history.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-geography.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-government-and-politics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-macroeconomics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-mathematics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-microeconomics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-physics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-psychology.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-statistics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-us-history.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-high-school-world-history.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-human-aging.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-human-sexuality.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-international-law.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-jurisprudence.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-logical-fallacies.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-machine-learning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-management.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-marketing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-medical-genetics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-miscellaneous.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-moral-disputes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-moral-scenarios.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-nutrition.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-philosophy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-prehistory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-professional-accounting.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-professional-law.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-professional-medicine.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-professional-psychology.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-public-relations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-security-studies.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-sociology.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-us-foreign-policy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-virology.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/mmlu-world-religions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/openbookqa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/piqa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/socialiqa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/truthfulqa-mc1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/data_config/task/winogrande.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/instance_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/pile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/data/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.341879 nutcracker-py-0.0.1a37/nutcracker/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/auto_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/frq_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.341879 nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/frq_judge_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/frq_judge_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/mcq_judge_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/mcq_judge_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/mcq_judge_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/mcq_judge_zeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/mcq_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/evaluator/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.341879 nutcracker-py-0.0.1a37/nutcracker/runs/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/runs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/runs/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.345879 nutcracker-py-0.0.1a37/nutcracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.345879 nutcracker-py-0.0.1a37/nutcracker/tests/mcq_evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/tests/mcq_evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/nutcracker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 15:42:43.345879 nutcracker-py-0.0.1a37/nutcracker_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-03-17 15:42:43.000000 nutcracker-py-0.0.1a37/nutcracker_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-17 15:42:43.000000 nutcracker-py-0.0.1a37/nutcracker_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 15:42:43.000000 nutcracker-py-0.0.1a37/nutcracker_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-17 15:42:43.000000 nutcracker-py-0.0.1a37/nutcracker_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-17 15:42:43.000000 nutcracker-py-0.0.1a37/nutcracker_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 15:42:43.345879 nutcracker-py-0.0.1a37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-17 15:42:32.000000 nutcracker-py-0.0.1a37/setup.py
```

### Comparing `nutcracker-py-0.0.1a36/.github/workflows/pipy_release.yaml` & `nutcracker-py-0.0.1a37/.github/workflows/pipy_release.yaml`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/LICENSE.txt` & `nutcracker-py-0.0.1a37/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/PKG-INFO` & `nutcracker-py-0.0.1a37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutcracker-py
-Version: 0.0.1a36
+Version: 0.0.1a37
 Summary: streamline LLM evaluation
 Author: Bruce W. Lee
 Author-email: bruce@walnutresearch.com
 Keywords: Evaluation
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyyaml>=6.0.1
```

### Comparing `nutcracker-py-0.0.1a36/README.md` & `nutcracker-py-0.0.1a37/README.md`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/nutcracker/data/instance.py` & `nutcracker-py-0.0.1a37/nutcracker/data/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         self.correct_options = test_data["correct_options"]
 
         # below are derivational attributes that will be updated during code run
         self.user_prompt = self._format_user_prompt()
         self.model_response = None
         self.model_response_logprobs = None
         self.response_correct = False
-        self.response_evaluator_engine = None
+        self.response_evaluator_judge = None
 
 
     
     def _format_user_prompt(self) -> str:
         """Format the user prompt.
 
         Args:
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/data/instance_collection.py` & `nutcracker-py-0.0.1a37/nutcracker/data/instance_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 #
 #
 class InstanceCollection:
     def __init__(self) -> None:
         """Initialize an empty collection of instances."""
         self.instances = []
-        self.evaluator_engine = None
+        self.evaluator_judge = None
 
 
 
     def __len__(self) -> int:
         """Return the number of instances in the collection.
 
         Returns:
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/data/pile.py` & `nutcracker-py-0.0.1a37/nutcracker/data/pile.py`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/nutcracker/data/task.py` & `nutcracker-py-0.0.1a37/nutcracker/data/task.py`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/auto_evaluator.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/auto_evaluator.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 from nutcracker.data.instance import MCQInstance
 from nutcracker.data.instance import FRQInstance
 from nutcracker.evaluator.mcq_evaluator import MCQEvaluator
 from nutcracker.evaluator.frq_evaluator import FRQEvaluator
 #
 #
 class AutoEvaluator:
-    def __init__(self, data: Union[Pile, Task, List[MCQInstance], List[FRQInstance]], mcq_engine = 'recommended', frq_engine = 'recommended', **engine_kwargs) -> None:
+    def __init__(self, data: Union[Pile, Task, List[MCQInstance], List[FRQInstance]], mcq_judge = 'recommended', frq_judge = 'recommended', **judge_kwargs) -> None:
         self.data = data
-        self.engine_kwargs = engine_kwargs
+        self.judge_kwargs = judge_kwargs
         self._control_logging()
-        self.frq_engine = frq_engine
-        self.mcq_engine = mcq_engine
+        self.frq_judge = frq_judge
+        self.mcq_judge = mcq_judge
 
     def run(self, round_digits: int = 5) -> float:
         mcq_data = [instance for instance in self.data if isinstance(instance, MCQInstance)]
         frq_data = [instance for instance in self.data if isinstance(instance, FRQInstance)]
         self.logger.info(f"found {len(mcq_data)} MCQInstances.")
         self.logger.info(f"found {len(frq_data)} FRQInstances.")
 
         if mcq_data:
-            mcq_evaluator = MCQEvaluator(mcq_data, engine=self.mcq_engine, **self.engine_kwargs)
+            mcq_evaluator = MCQEvaluator(mcq_data, judge=self.mcq_judge, **self.judge_kwargs)
             mcq_evaluator.run(round_digits)
 
         if frq_data:
-            frq_evaluator = FRQEvaluator(frq_data, engine=self.frq_engine, **self.engine_kwargs)
+            frq_evaluator = FRQEvaluator(frq_data, judge=self.frq_judge, **self.judge_kwargs)
             frq_evaluator.run(round_digits)
 
         # This function currently does not return accuracy. Modify as needed or use separate reporting.
 
     def _control_logging(self) -> None:
         self.logger = logging.getLogger(__name__)
         self.logger.info(f"AutoEvaluator created with {len(self.data)} instances.")
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/frq_engine_alpha.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/frq_judge_alpha.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #
 from openai import OpenAI
 import openai
 #
 #
 #
-class FRQEngineAlpha:
+class FRQJudgeAlpha:
     def __init__(self):
         # Use the kwargs as needed for configuration
         # Example: self.some_setting = kwargs.get('some_setting', default_value)
         pass
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/frq_engine_beta.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/frq_judge_beta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, List, Set
 #
 from nutcracker.data.instance import FRQInstance
 #
 #
-class FRQEngineBeta:
+class FRQJudgeBeta:
     def __init__(self):
         pass
 
 
 
     def is_correct(self, instance: FRQInstance) -> bool:
         found_options = self._parse_model_response_rule_based(instance.model_response)
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/mcq_engine_alpha.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/mcq_judge_alpha.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #
 from openai import OpenAI
 import openai
 #
 #
 #
-class MCQEngineAlpha:
+class MCQJudgeAlpha:
     def __init__(self):
         # Use the kwargs as needed for configuration
         # Example: self.some_setting = kwargs.get('some_setting', default_value)
         pass
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/mcq_engine_beta.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/mcq_judge_beta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, List, Set
 #
 from nutcracker.data.instance import MCQInstance
 #
 #
-class MCQEngineBeta:
+class MCQJudgeBeta:
     def __init__(self):
         pass
 
 
 
     def is_correct(self, instance: MCQInstance) -> bool:
         found_options = self._parse_model_response_rule_based(instance.model_response)
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/mcq_engine_gamma.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/mcq_judge_gamma.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, List
 #
 from nutcracker.data.instance import MCQInstance
 #
 #
-class MCQEngineGamma:
+class MCQJudgeGamma:
     def __init__(self):
         pass
 
     def is_correct(self, instance: MCQInstance) -> bool:
         # Extract the log probabilities for the first position token
         logprobs = instance.model_response_logprobs[0]
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/engines/mcq_engine_zeta.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/judges/mcq_judge_zeta.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from nutcracker.data.instance import MCQInstance
 #
 #
 from openai import OpenAI
 #
 #
 #
-class MCQEngineZeta:
+class MCQJudgeZeta:
     def __init__(self):
         # Use the kwargs as needed for configuration
         # Example: self.some_setting = kwargs.get('some_setting', default_value)
         pass
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/frq_evaluator.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/frq_evaluator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import List, Set, Optional, Union
 import logging
 #
 from nutcracker.data.task import Task
 from nutcracker.data.pile import Pile
 from nutcracker.data.instance import FRQInstance
 from nutcracker.utils import TqdmLoggingHandler
-from nutcracker.evaluator.engines.frq_engine_alpha import FRQEngineAlpha
-from nutcracker.evaluator.engines.frq_engine_beta import FRQEngineBeta
+from nutcracker.evaluator.judges.frq_judge_alpha import FRQJudgeAlpha
+from nutcracker.evaluator.judges.frq_judge_beta import FRQJudgeBeta
 #
 #
 class FRQEvaluator:
     def __init__(
-        self, data: Union[Pile, Task, List[FRQInstance]], engine: str = 'alpha', **engine_kwargs) -> None:
+        self, data: Union[Pile, Task, List[FRQInstance]], judge: str = 'alpha', **judge_kwargs) -> None:
         self.data = data
-        if engine == 'alpha' or engine == 'recommended':
-            self.response_evaluator_engine = 'frq-engine-alpha'
-            self.engine = FRQEngineAlpha(**engine_kwargs)
-        elif engine == 'beta' or engine == 'recommended':
-            self.response_evaluator_engine = 'frq-engine-beta'
-            self.engine = FRQEngineBeta(**engine_kwargs)
+        if judge == 'alpha' or judge == 'recommended':
+            self.response_evaluator_judge = 'frq-judge-alpha'
+            self.judge = FRQJudgeAlpha(**judge_kwargs)
+        elif judge == 'beta' or judge == 'recommended':
+            self.response_evaluator_judge = 'frq-judge-beta'
+            self.judge = FRQJudgeBeta(**judge_kwargs)
         self._control_logging()
 
 
 
     def run(self, round_digits: int = 5) -> float:
         correct_count = 0
         for instance in TqdmLoggingHandler(self.data, logger=self.logger, desc="Processing Instances"):
-            is_correct = self.engine.is_correct(instance)
+            is_correct = self.judge.is_correct(instance)
             instance.response_correct = is_correct  # Update the instance attribute here
-            instance.response_evaluator_engine = self.response_evaluator_engine # fingerprint
+            instance.response_evaluator_judge = self.response_evaluator_judge # fingerprint
             if is_correct:
                 correct_count += 1
 
         accuracy = correct_count / len(self.data) if len(self.data) > 0 else 0.0
         return round(accuracy, round_digits)
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/mcq_evaluator.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/mcq_evaluator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from typing import List, Set, Optional, Union
 import logging
 #
 from nutcracker.data.task import Task
 from nutcracker.data.pile import Pile
 from nutcracker.data.instance import MCQInstance
 from nutcracker.utils import TqdmLoggingHandler
-from nutcracker.evaluator.engines.mcq_engine_alpha import MCQEngineAlpha
-from nutcracker.evaluator.engines.mcq_engine_beta import MCQEngineBeta
-from nutcracker.evaluator.engines.mcq_engine_gamma import MCQEngineGamma
-from nutcracker.evaluator.engines.mcq_engine_zeta import MCQEngineZeta
+from nutcracker.evaluator.judges.mcq_judge_alpha import MCQJudgeAlpha
+from nutcracker.evaluator.judges.mcq_judge_beta import MCQJudgeBeta
+from nutcracker.evaluator.judges.mcq_judge_gamma import MCQJudgeGamma
+from nutcracker.evaluator.judges.mcq_judge_zeta import MCQJudgeZeta
 #
 #
 class MCQEvaluator:
-    def __init__(self, data: Union[Pile, Task, List[MCQInstance]], engine: str = 'alpha', **engine_kwargs) -> None:
+    def __init__(self, data: Union[Pile, Task, List[MCQInstance]], judge: str = 'alpha', **judge_kwargs) -> None:
         self.data = data
-        if engine == 'alpha':
-            self.response_evaluator_engine = 'mcq-engine-alpha'
-            self.engine = MCQEngineAlpha(**engine_kwargs)
-        elif engine == 'beta':
-            self.response_evaluator_engine = 'mcq-engine-beta'
-            self.engine = MCQEngineBeta(**engine_kwargs)
-        elif engine == 'gamma':
-            self.response_evaluator_engine = 'mcq-engine-gamma'
-            self.engine = MCQEngineGamma(**engine_kwargs)
-        elif engine == 'zeta' or engine == 'recommended':
-            self.response_evaluator_engine = 'mcq-engine-zeta'
-            self.engine = MCQEngineZeta(**engine_kwargs)
+        if judge == 'alpha':
+            self.response_evaluator_judge = 'mcq-judge-alpha'
+            self.judge = MCQJudgeAlpha(**judge_kwargs)
+        elif judge == 'beta':
+            self.response_evaluator_judge = 'mcq-judge-beta'
+            self.judge = MCQJudgeBeta(**judge_kwargs)
+        elif judge == 'gamma':
+            self.response_evaluator_judge = 'mcq-judge-gamma'
+            self.judge = MCQJudgeGamma(**judge_kwargs)
+        elif judge == 'zeta' or judge == 'recommended':
+            self.response_evaluator_judge = 'mcq-judge-zeta'
+            self.judge = MCQJudgeZeta(**judge_kwargs)
         self._control_logging()
 
 
 
     def run(self, round_digits: int = 5) -> float:
         correct_count = 0
         for instance in TqdmLoggingHandler(self.data, logger=self.logger, desc="Processing Instances"):
-            is_correct = self.engine.is_correct(instance)
+            is_correct = self.judge.is_correct(instance)
             instance.response_correct = is_correct  # Update the instance attribute here
-            instance.response_evaluator_engine = self.response_evaluator_engine # fingerprint
+            instance.response_evaluator_judge = self.response_evaluator_judge # fingerprint
             if is_correct:
                 correct_count += 1
 
         accuracy = correct_count / len(self.data) if len(self.data) > 0 else 0.0
         return round(accuracy, round_digits)
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker/evaluator/reporter.py` & `nutcracker-py-0.0.1a37/nutcracker/evaluator/reporter.py`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/nutcracker/runs/schema.py` & `nutcracker-py-0.0.1a37/nutcracker/runs/schema.py`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_intent.py` & `nutcracker-py-0.0.1a37/nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_intent.py`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_rule.py` & `nutcracker-py-0.0.1a37/nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_rule.py`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/nutcracker/utils.py` & `nutcracker-py-0.0.1a37/nutcracker/utils.py`

 * *Files identical despite different names*

### Comparing `nutcracker-py-0.0.1a36/nutcracker_py.egg-info/PKG-INFO` & `nutcracker-py-0.0.1a37/nutcracker_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutcracker-py
-Version: 0.0.1a36
+Version: 0.0.1a37
 Summary: streamline LLM evaluation
 Author: Bruce W. Lee
 Author-email: bruce@walnutresearch.com
 Keywords: Evaluation
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyyaml>=6.0.1
```

### Comparing `nutcracker-py-0.0.1a36/nutcracker_py.egg-info/SOURCES.txt` & `nutcracker-py-0.0.1a37/nutcracker_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -105,25 +105,23 @@
 nutcracker/data/data_config/task/truthfulqa-mc1.yaml
 nutcracker/data/data_config/task/winogrande.yaml
 nutcracker/evaluator/__init__.py
 nutcracker/evaluator/auto_evaluator.py
 nutcracker/evaluator/frq_evaluator.py
 nutcracker/evaluator/mcq_evaluator.py
 nutcracker/evaluator/reporter.py
-nutcracker/evaluator/engines/__init__.py
-nutcracker/evaluator/engines/frq_engine_alpha.py
-nutcracker/evaluator/engines/frq_engine_beta.py
-nutcracker/evaluator/engines/mcq_engine_alpha.py
-nutcracker/evaluator/engines/mcq_engine_beta.py
-nutcracker/evaluator/engines/mcq_engine_gamma.py
-nutcracker/evaluator/engines/mcq_engine_zeta.py
+nutcracker/evaluator/judges/__init__.py
+nutcracker/evaluator/judges/frq_judge_alpha.py
+nutcracker/evaluator/judges/frq_judge_beta.py
+nutcracker/evaluator/judges/mcq_judge_alpha.py
+nutcracker/evaluator/judges/mcq_judge_beta.py
+nutcracker/evaluator/judges/mcq_judge_gamma.py
+nutcracker/evaluator/judges/mcq_judge_zeta.py
 nutcracker/runs/__init__.py
-nutcracker/runs/inquiry.py
 nutcracker/runs/schema.py
-nutcracker/runs/study.py
 nutcracker/tests/__init__.py
 nutcracker/tests/mcq_evaluator/__init__.py
 nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_intent.py
 nutcracker/tests/mcq_evaluator/test_model_response_matching_rigor_rule.py
 nutcracker_py.egg-info/PKG-INFO
 nutcracker_py.egg-info/SOURCES.txt
 nutcracker_py.egg-info/dependency_links.txt
```

### Comparing `nutcracker-py-0.0.1a36/setup.py` & `nutcracker-py-0.0.1a37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from distutils.core import setup
 from setuptools import find_packages
 
-this_version='0.0.1a36'
+this_version='0.0.1a37'
 
 # python setup.py sdist
 # python -m twine upload dist/*
 # pip install -e .
 # git tag -a "0.0.1a12" -m "pypi workflow revamp"
 # git push --tags    
 setup(
```

