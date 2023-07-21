# Comparing `tmp/dolma-0.6.5.tar.gz` & `tmp/dolma-0.7.0.tar.gz`

## Comparing `dolma-0.6.5.tar` & `dolma-0.7.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 dolma-0.6.5/Cargo.toml
--rw-r--r--   0     1001      123      299 2023-07-18 03:40:55.000000 dolma-0.6.5/.cargo/config.toml
--rw-r--r--   0     1001      123      475 2023-07-18 03:40:55.000000 dolma-0.6.5/.flake8
--rw-r--r--   0     1001      123     5194 2023-07-18 03:40:55.000000 dolma-0.6.5/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     2194 2023-07-18 03:40:55.000000 dolma-0.6.5/.github/workflows/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0     1001      123      691 2023-07-18 03:40:55.000000 dolma-0.6.5/.github/workflows/ISSUE_TEMPLATE/documentation.yml
--rw-r--r--   0     1001      123     1077 2023-07-18 03:40:55.000000 dolma-0.6.5/.github/workflows/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0     1001      123      414 2023-07-18 03:40:55.000000 dolma-0.6.5/.github/workflows/ISSUE_TEMPLATE/question.yml
--rw-r--r--   0     1001      123      549 2023-07-18 03:40:55.000000 dolma-0.6.5/.gitignore
--rw-r--r--   0     1001      123     1813 2023-07-18 03:40:55.000000 dolma-0.6.5/CITATION.cff
--rw-r--r--   0     1001      123    11357 2023-07-18 03:40:55.000000 dolma-0.6.5/LICENSE
--rw-r--r--   0     1001      123     1395 2023-07-18 03:40:55.000000 dolma-0.6.5/Makefile
--rw-r--r--   0     1001      123     3150 2023-07-18 03:40:55.000000 dolma-0.6.5/README.md
--rw-r--r--   0     1001      123     3296 2023-07-18 03:40:55.000000 dolma-0.6.5/pyproject.toml
--rw-r--r--   0     1001      123     1019 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/__init__.py
--rw-r--r--   0     1001      123     4401 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/cli/__init__.py
--rw-r--r--   0     1001      123     1494 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/cli/__main__.py
--rw-r--r--   0     1001      123     5733 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/cli/deduper.py
--rw-r--r--   0     1001      123     5665 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/cli/mixer.py
--rw-r--r--   0     1001      123      473 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/cli/shared.py
--rw-r--r--   0     1001      123     2855 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/cli/tagger.py
--rw-r--r--   0     1001      123      219 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/__init__.py
--rw-r--r--   0     1001      123     6181 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/data_types.py
--rw-r--r--   0     1001      123      483 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/errors.py
--rw-r--r--   0     1001      123     6482 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/ft_dataset.py
--rw-r--r--   0     1001      123     5557 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/ft_tagger.py
--rw-r--r--   0     1001      123      383 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/loggers.py
--rw-r--r--   0     1001      123    15866 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/parallel.py
--rw-r--r--   0     1001      123     6326 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/paths.py
--rw-r--r--   0     1001      123     1254 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/registry.py
--rw-r--r--   0     1001      123    11812 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/runtime.py
--rw-r--r--   0     1001      123     1066 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/taggers.py
--rw-r--r--   0     1001      123       42 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/trainer.py
--rw-r--r--   0     1001      123     2031 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/utils.py
--rw-r--r--   0     1001      123     9515 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/core/vizualizer.py
--rw-r--r--   0     1001      123     3777 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/data/naughty_words_en.txt
--rw-r--r--   0     1001      123        0 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/py.typed
--rw-r--r--   0     1001      123       72 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/taggers/__init__.py
--rw-r--r--   0     1001      123     3277 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/taggers/c4.py
--rw-r--r--   0     1001      123     6433 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/taggers/code.py
--rw-r--r--   0     1001      123     6857 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/taggers/gopher.py
--rw-r--r--   0     1001      123     1898 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/taggers/jigsaw.py
--rw-r--r--   0     1001      123     6639 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/taggers/language.py
--rw-r--r--   0     1001      123     4860 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/taggers/length.py
--rw-r--r--   0     1001      123    10494 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/taggers/pii.py
--rw-r--r--   0     1001      123      744 2023-07-18 03:40:55.000000 dolma-0.6.5/python/dolma/taggers/sampling.py
--rw-r--r--   0     1001      123      232 2023-07-18 03:40:55.000000 dolma-0.6.5/res/logo.md
--rw-r--r--   0     1001      123  1813803 2023-07-18 03:40:55.000000 dolma-0.6.5/res/logo.png
--rw-r--r--   0     1001      123     9277 2023-07-18 03:40:55.000000 dolma-0.6.5/src/bloom_filter.rs
--rw-r--r--   0     1001      123    11000 2023-07-18 03:40:55.000000 dolma-0.6.5/src/deduper.rs
--rw-r--r--   0     1001      123     1498 2023-07-18 03:40:55.000000 dolma-0.6.5/src/lib.rs
--rw-r--r--   0     1001      123     2499 2023-07-18 03:40:55.000000 dolma-0.6.5/src/mixer.rs
--rw-r--r--   0     1001      123    10922 2023-07-18 03:40:55.000000 dolma-0.6.5/src/s3_util.rs
--rw-r--r--   0     1001      123    28608 2023-07-18 03:40:55.000000 dolma-0.6.5/src/shard.rs
--rw-r--r--   0     1001      123      863 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/config/c4-cleaned.json
--rw-r--r--   0     1001      123      567 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/config/dedupe-by-url.json
--rw-r--r--   0     1001      123      537 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/config/dedupe-paragraphs.json
--rw-r--r--   0     1001      123      745 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/config/email-spans.json
--rw-r--r--   0     1001      123      740 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/config/filter-by-spans.json
--rw-r--r--   0     1001      123      713 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/config/mixer.json
--rw-r--r--   0     1001      123      647 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/config/paragraph-spans.json
--rw-r--r--   0     1001      123      489 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/expected/dedupe-by-url.json.gz
--rw-r--r--   0     1001      123      746 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/expected/dedupe-paragraphs.json.gz
--rw-r--r--   0     1001      123    26447 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/expected/email-spans.json.gz
--rw-r--r--   0     1001      123    14879 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/expected/filter-by-spans.json.gz
--rw-r--r--   0     1001      123    15748 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/expected/mixer.json.gz
--rw-r--r--   0     1001      123    26524 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/expected/remove-paragraphs.json.gz
--rw-r--r--   0     1001      123      702 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/provided/attributes/duplicate_paragraphs/000.json.gz
--rw-r--r--   0     1001      123      614 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/provided/attributes/pii/000.json.gz
--rw-r--r--   0     1001      123      570 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/provided/attributes/sample/000.json.gz
--rw-r--r--   0     1001      123      543 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/provided/attributes/toxicity/000.json.gz
--rw-r--r--   0     1001      123    25985 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/data/provided/documents/000.json.gz
--rw-r--r--   0     1001      123      352 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/__init__.py
--rw-r--r--   0     1001      123     3321 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/test_data_types.py
--rw-r--r--   0     1001      123     3349 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/test_deduper.py
--rw-r--r--   0     1001      123     4486 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/test_mixer.py
--rw-r--r--   0     1001      123     1395 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/test_omegaconf.py
--rw-r--r--   0     1001      123     2459 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/test_parallel.py
--rw-r--r--   0     1001      123     9316 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/test_paths.py
--rw-r--r--   0     1001      123     1846 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/test_runtime.py
--rw-r--r--   0     1001      123     9701 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/test_taggers.py
--rw-r--r--   0     1001      123     3996 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/test_utils.py
--rw-r--r--   0     1001      123     3772 2023-07-18 03:40:55.000000 dolma-0.6.5/tests/python/utils.py
--rw-r--r--   0     1001      123    57396 2023-07-18 03:41:01.000000 dolma-0.6.5/Cargo.lock
--rw-r--r--   0        0        0     5288 1970-01-01 00:00:00.000000 dolma-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 dolma-0.7.0/Cargo.toml
+-rw-r--r--   0     1001      123      299 2023-07-21 14:49:36.000000 dolma-0.7.0/.cargo/config.toml
+-rw-r--r--   0     1001      123      475 2023-07-21 14:49:36.000000 dolma-0.7.0/.flake8
+-rw-r--r--   0     1001      123     5194 2023-07-21 14:49:36.000000 dolma-0.7.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     2194 2023-07-21 14:49:36.000000 dolma-0.7.0/.github/workflows/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0     1001      123      691 2023-07-21 14:49:36.000000 dolma-0.7.0/.github/workflows/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0     1001      123     1077 2023-07-21 14:49:36.000000 dolma-0.7.0/.github/workflows/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0     1001      123      414 2023-07-21 14:49:36.000000 dolma-0.7.0/.github/workflows/ISSUE_TEMPLATE/question.yml
+-rw-r--r--   0     1001      123      549 2023-07-21 14:49:36.000000 dolma-0.7.0/.gitignore
+-rw-r--r--   0     1001      123     1813 2023-07-21 14:49:36.000000 dolma-0.7.0/CITATION.cff
+-rw-r--r--   0     1001      123    11357 2023-07-21 14:49:36.000000 dolma-0.7.0/LICENSE
+-rw-r--r--   0     1001      123     1395 2023-07-21 14:49:36.000000 dolma-0.7.0/Makefile
+-rw-r--r--   0     1001      123     3150 2023-07-21 14:49:36.000000 dolma-0.7.0/README.md
+-rw-r--r--   0     1001      123     3296 2023-07-21 14:49:36.000000 dolma-0.7.0/pyproject.toml
+-rw-r--r--   0     1001      123     1019 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/__init__.py
+-rw-r--r--   0     1001      123     4439 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/cli/__init__.py
+-rw-r--r--   0     1001      123     1610 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/cli/__main__.py
+-rw-r--r--   0     1001      123     5811 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/cli/deduper.py
+-rw-r--r--   0     1001      123     5722 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/cli/mixer.py
+-rw-r--r--   0     1001      123      473 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/cli/shared.py
+-rw-r--r--   0     1001      123     3968 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/cli/tagger.py
+-rw-r--r--   0     1001      123      219 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/__init__.py
+-rw-r--r--   0     1001      123     6386 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/data_types.py
+-rw-r--r--   0     1001      123      483 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/errors.py
+-rw-r--r--   0     1001      123     6482 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/ft_dataset.py
+-rw-r--r--   0     1001      123     5557 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/ft_tagger.py
+-rw-r--r--   0     1001      123      383 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/loggers.py
+-rw-r--r--   0     1001      123    16576 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/parallel.py
+-rw-r--r--   0     1001      123     7777 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/paths.py
+-rw-r--r--   0     1001      123     1254 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/registry.py
+-rw-r--r--   0     1001      123    16002 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/runtime.py
+-rw-r--r--   0     1001      123     1170 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/taggers.py
+-rw-r--r--   0     1001      123       42 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/trainer.py
+-rw-r--r--   0     1001      123     2031 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/utils.py
+-rw-r--r--   0     1001      123     9515 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/core/vizualizer.py
+-rw-r--r--   0     1001      123     3777 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/data/naughty_words_en.txt
+-rw-r--r--   0     1001      123        0 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/py.typed
+-rw-r--r--   0     1001      123       72 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/taggers/__init__.py
+-rw-r--r--   0     1001      123     3277 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/taggers/c4.py
+-rw-r--r--   0     1001      123     6433 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/taggers/code.py
+-rw-r--r--   0     1001      123     6857 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/taggers/gopher.py
+-rw-r--r--   0     1001      123     1898 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/taggers/jigsaw.py
+-rw-r--r--   0     1001      123     6639 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/taggers/language.py
+-rw-r--r--   0     1001      123     4860 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/taggers/length.py
+-rw-r--r--   0     1001      123    10494 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/taggers/pii.py
+-rw-r--r--   0     1001      123      744 2023-07-21 14:49:36.000000 dolma-0.7.0/python/dolma/taggers/sampling.py
+-rw-r--r--   0     1001      123      232 2023-07-21 14:49:36.000000 dolma-0.7.0/res/logo.md
+-rw-r--r--   0     1001      123  1813803 2023-07-21 14:49:36.000000 dolma-0.7.0/res/logo.png
+-rw-r--r--   0     1001      123     9277 2023-07-21 14:49:36.000000 dolma-0.7.0/src/bloom_filter.rs
+-rw-r--r--   0     1001      123    11000 2023-07-21 14:49:36.000000 dolma-0.7.0/src/deduper.rs
+-rw-r--r--   0     1001      123     1498 2023-07-21 14:49:36.000000 dolma-0.7.0/src/lib.rs
+-rw-r--r--   0     1001      123     2499 2023-07-21 14:49:36.000000 dolma-0.7.0/src/mixer.rs
+-rw-r--r--   0     1001      123    10922 2023-07-21 14:49:36.000000 dolma-0.7.0/src/s3_util.rs
+-rw-r--r--   0     1001      123    28608 2023-07-21 14:49:36.000000 dolma-0.7.0/src/shard.rs
+-rw-r--r--   0     1001      123      863 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/config/c4-cleaned.json
+-rw-r--r--   0     1001      123      567 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/config/dedupe-by-url.json
+-rw-r--r--   0     1001      123      537 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/config/dedupe-paragraphs.json
+-rw-r--r--   0     1001      123      745 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/config/email-spans.json
+-rw-r--r--   0     1001      123      740 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/config/filter-by-spans.json
+-rw-r--r--   0     1001      123      713 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/config/mixer.json
+-rw-r--r--   0     1001      123      647 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/config/paragraph-spans.json
+-rw-r--r--   0     1001      123      489 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/expected/dedupe-by-url.json.gz
+-rw-r--r--   0     1001      123      746 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/expected/dedupe-paragraphs.json.gz
+-rw-r--r--   0     1001      123    26447 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/expected/email-spans.json.gz
+-rw-r--r--   0     1001      123    14879 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/expected/filter-by-spans.json.gz
+-rw-r--r--   0     1001      123    15748 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/expected/mixer.json.gz
+-rw-r--r--   0     1001      123    26524 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/expected/remove-paragraphs.json.gz
+-rw-r--r--   0     1001      123      702 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/provided/attributes/duplicate_paragraphs/000.json.gz
+-rw-r--r--   0     1001      123      614 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/provided/attributes/pii/000.json.gz
+-rw-r--r--   0     1001      123      570 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/provided/attributes/sample/000.json.gz
+-rw-r--r--   0     1001      123      543 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/provided/attributes/toxicity/000.json.gz
+-rw-r--r--   0     1001      123    25985 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/data/provided/documents/000.json.gz
+-rw-r--r--   0     1001      123      352 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/__init__.py
+-rw-r--r--   0     1001      123     3321 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/test_data_types.py
+-rw-r--r--   0     1001      123     3349 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/test_deduper.py
+-rw-r--r--   0     1001      123     4486 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/test_mixer.py
+-rw-r--r--   0     1001      123     1395 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/test_omegaconf.py
+-rw-r--r--   0     1001      123     2459 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/test_parallel.py
+-rw-r--r--   0     1001      123     9316 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/test_paths.py
+-rw-r--r--   0     1001      123     7625 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/test_runtime.py
+-rw-r--r--   0     1001      123     9701 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/test_taggers.py
+-rw-r--r--   0     1001      123     3996 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/test_utils.py
+-rw-r--r--   0     1001      123     3772 2023-07-21 14:49:36.000000 dolma-0.7.0/tests/python/utils.py
+-rw-r--r--   0     1001      123    57396 2023-07-21 14:49:36.000000 dolma-0.7.0/Cargo.lock
+-rw-r--r--   0        0        0     5288 1970-01-01 00:00:00.000000 dolma-0.7.0/PKG-INFO
```

### Comparing `dolma-0.6.5/Cargo.toml` & `dolma-0.7.0/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dolma"
-version = "0.6.5"
+version = "0.7.0"
 edition = "2021"
 license = "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "dolma"
 crate-type = ["cdylib"]
```

### Comparing `dolma-0.6.5/.github/workflows/CI.yml` & `dolma-0.7.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/.github/workflows/ISSUE_TEMPLATE/bug_report.yml` & `dolma-0.7.0/.github/workflows/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/.github/workflows/ISSUE_TEMPLATE/documentation.yml` & `dolma-0.7.0/.github/workflows/ISSUE_TEMPLATE/documentation.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/.github/workflows/ISSUE_TEMPLATE/feature_request.yml` & `dolma-0.7.0/.github/workflows/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/.gitignore` & `dolma-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/CITATION.cff` & `dolma-0.7.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/LICENSE` & `dolma-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/Makefile` & `dolma-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/README.md` & `dolma-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/pyproject.toml` & `dolma-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dolma"
-version = "0.6.5"
+version = "0.7.0"
 description = "Data filters"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "anyascii>=0.3.2",
     "blingfire==0.1.8",
```

### Comparing `dolma-0.6.5/python/dolma/__init__.py` & `dolma-0.7.0/python/dolma/__init__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/cli/__init__.py` & `dolma-0.7.0/python/dolma/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     console = console or Console()
     syntax = Syntax(code=om.to_yaml(config).strip(), lexer="yaml", theme="ansi_dark")
     console.print(syntax)
 
 
 class BaseCli(Generic[D]):
     CONFIG: Type[D]
+    DESCRIPTION: Optional[str] = None
 
     @classmethod
     def make_parser(cls, parser: A) -> A:
         assert hasattr(cls, "CONFIG"), f"{cls.__name__} must have a CONFIG attribute"
         return make_parser(parser, cls.CONFIG)
 
     @classmethod
```

### Comparing `dolma-0.6.5/python/dolma/cli/__main__.py` & `dolma-0.7.0/python/dolma/cli/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 from pathlib import Path
 from typing import List, Optional
 
 from yaml import safe_load
 
 from .deduper import DeduperCli
 from .mixer import MixerCli
-from .tagger import TaggerCli
+from .tagger import ListTaggerCli, TaggerCli
 
 AVAILABLE_COMMANDS = {
     "dedupe": DeduperCli,
     "mix": MixerCli,
     "tag": TaggerCli,
+    "list": ListTaggerCli
+    # following functionality is not yet implemented
     # "visualize": None,
     # "browse": None,
     # "stats": None,
     # "ft-train": None,
 }
 
 
@@ -34,15 +36,15 @@
     )
     subparsers = parser.add_subparsers(dest="command")
     subparsers.required = True
     subparsers.choices = AVAILABLE_COMMANDS.keys()  # type: ignore
 
     for command, cli in AVAILABLE_COMMANDS.items():
         if cli is not None:
-            cli.make_parser(subparsers.add_parser(command))
+            cli.make_parser(subparsers.add_parser(command, help=cli.DESCRIPTION))
 
     args = parser.parse_args(argv)
 
     # try parsing the config file
     config: Optional[dict] = None
     if config_path := args.__dict__.pop("config"):
         assert config_path.exists(), f"Config file {config_path} does not exist"
```

### Comparing `dolma-0.6.5/python/dolma/cli/deduper.py` & `dolma-0.7.0/python/dolma/cli/deduper.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     processes: int = field(
         default=1, help="Number of processes to use for deduplication. If 1, no multiprocessing will be used."
     )
 
 
 class DeduperCli(BaseCli):
     CONFIG = DeduperConfig
+    DESCRIPTION = "Deduplicate documents or paragraphs using a bloom filter."
 
     @classmethod
     def run(cls, parsed_config: DeduperConfig):
         logger = get_logger("tagger")
 
         dict_config: Dict[str, Any] = {}
```

### Comparing `dolma-0.6.5/python/dolma/cli/mixer.py` & `dolma-0.7.0/python/dolma/cli/mixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     streams: List[StreamConfig] = field(default=[], help="List configurations of streams to be mixed")
     work_dir: WorkDirConfig = field(default=WorkDirConfig(), help="Configuration for temporary work directories.")
     processes: int = field(default=1, help="Number of processes to use for mixing. By default 1 process is used.")
 
 
 class MixerCli(BaseCli):
     CONFIG = MixerConfig
+    DESCRIPTION = "Mix documents from multiple streams."
 
     @classmethod
     def run(cls, parsed_config: MixerConfig):
         logger = get_logger("mixer")
 
         dict_config: Dict[str, Any] = {
             "work_dir": {"input": parsed_config.work_dir.input, "output": parsed_config.work_dir.output},
```

### Comparing `dolma-0.6.5/python/dolma/core/data_types.py` & `dolma-0.7.0/python/dolma/core/data_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 
 Data types assumed by Filters.
 
 @kylel, @soldni
 
 """
 
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple
 
 from msgspec import Struct
+from typing_extensions import TypeAlias
+
+TaggerOutputValueType: TypeAlias = Tuple[int, int, float]
+TaggerOutputType: TypeAlias = List[TaggerOutputValueType]
+TaggerOutputDictType: TypeAlias = Dict[str, TaggerOutputType]
 
 
 class InputSpec(Struct):
     id: str
     text: str
     source: str
     version: Optional[str] = None
     # ignoring metadata for now; taggers run on text only
     # metadata: Optional[Dict[str, Any]] = None
 
 
 class OutputSpec(Struct):
     id: str
-    attributes: Dict[str, List[List[Union[int, float]]]]
+    attributes: Dict[str, List[Tuple[int, int, float]]]
     source: Optional[str] = None
 
 
 class Document:
     __slots__ = "source", "version", "id", "text"
 
     def __init__(self, source: str, id: str, text: str, version: Optional[str] = None) -> None:
@@ -76,15 +81,15 @@
     def mention(self, text: str, window: int = 0) -> str:
         return text[max(0, self.start - window) : min(len(text), self.end + window)]
 
     def select(self, doc: Document) -> str:
         return doc.text[self.start : self.end]
 
     @classmethod
-    def from_spec(cls, attribute_name: str, attribute_value: List[Union[int, float]]) -> "Span":
+    def from_spec(cls, attribute_name: str, attribute_value: TaggerOutputValueType) -> "Span":
         if "__" in attribute_name:
             # bff tagger has different name
             exp_name, tgr_name, attr_type = attribute_name.split("__", 2)
         else:
             exp_name = tgr_name = attr_type = attribute_name
 
         start, end, score = attribute_value
@@ -93,20 +98,20 @@
             end=int(end),
             type=attr_type,
             score=float(score),
             experiment=exp_name,
             tagger=tgr_name,
         )
 
-    def to_spec(self) -> Tuple[str, List[Union[int, float]]]:
+    def to_spec(self) -> Tuple[str, TaggerOutputValueType]:
         assert self.experiment is not None, "Experiment name must be set to convert to spec"
         assert self.tagger is not None, "Tagger name must be set to convert to spec"
         return (
             f"{self.experiment}__{self.tagger}__{self.type}",
-            [self.start, self.end, self.score],
+            (self.start, self.end, self.score),
         )
 
     def __len__(self) -> int:
         return self.end - self.start
 
     @classmethod
     def from_json(cls, di: Dict) -> "Span":
@@ -142,15 +147,15 @@
                     for attr_value in attr_values
                 ]
             )
         return DocResult(doc=Document.from_spec(doc), spans=spans)
 
     def to_spec(self) -> Tuple[InputSpec, OutputSpec]:
         doc_spec = self.doc.to_spec()
-        attributes: Dict[str, List[List[Union[int, float]]]] = {}
+        attributes: Dict[str, List[TaggerOutputValueType]] = {}
 
         for span in self.spans:
             attr_name, attr_value = span.to_spec()
             attributes.setdefault(attr_name, []).append(attr_value)
 
         return doc_spec, OutputSpec(source=self.doc.source, id=self.doc.id, attributes=attributes)
```

### Comparing `dolma-0.6.5/python/dolma/core/ft_dataset.py` & `dolma-0.7.0/python/dolma/core/ft_dataset.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/core/ft_tagger.py` & `dolma-0.7.0/python/dolma/core/ft_tagger.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/core/parallel.py` & `dolma-0.7.0/python/dolma/core/parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,23 @@
 from threading import Thread
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import smart_open
 import tqdm
 
 from .errors import DolmaError, DolmaRetryableFailure
-from .paths import add_suffix, glob_path, make_relative, mkdir_p, sub_prefix
+from .paths import (
+    add_suffix,
+    glob_path,
+    join_path,
+    make_relative,
+    mkdir_p,
+    split_path,
+    sub_prefix,
+)
 
 METADATA_SUFFIX = ".done.txt"
 
 
 class BaseParallelProcessor:
     """A base parallel processor that supports applying the same process_single method to a list of files.
 
@@ -112,18 +120,14 @@
 
         if len(self.src_prefixes) == 0:
             raise ValueError("At least one source prefix must be provided.")
 
         if any("*" in p for p in itertools.chain(self.dst_prefixes, self.meta_prefixes)):
             raise ValueError("Destination and metadata prefixes cannot contain wildcards.")
 
-        for i in range(len(self.src_prefixes)):
-            # adding a wildcard to the end of the each source prefix if it doesn't have one
-            self.src_prefixes[i] = add_suffix(p, "*") if "*" not in (p := self.src_prefixes[i]) else p
-
     @classmethod
     def process_single(
         cls,
         source_path: str,
         destination_path: str,
         queue: "Queue[Union[None, Tuple[int, ...]]]",
         **kwargs: Any,
@@ -313,17 +317,32 @@
         return True
 
     def _get_all_paths(self) -> Tuple[List[str], List[str], List[str]]:
         """Get all paths to process using prefixes provided"""
         all_source_paths, all_destination_paths, all_metadata_paths = [], [], []
 
         for src_prefix, dst_prefix, meta_prefix in zip(self.src_prefixes, self.dst_prefixes, self.meta_prefixes):
-            prefix, rel_paths = make_relative(list(glob_path(src_prefix)))
+            current_source_prefixes = sorted(glob_path(src_prefix))
+
+            if len(current_source_prefixes) > 1:
+                # make relative only makes sense if there is more than one path; otherwise, it's unclear
+                # what a relative path would be.
+                prefix, rel_paths = make_relative(current_source_prefixes)
+            elif len(current_source_prefixes) == 1:
+                # in case we have a single path, we can just use the path minus the file as the shared prefix,
+                # and the file as the relative path
+                prot, parts = split_path(current_source_prefixes[0])
+                prefix, rel_paths = join_path(prot, *parts[:-1]), [parts[-1]]
+            else:
+                raise ValueError(f"Could not find any files matching {src_prefix}")
+
+            # shuffle the order of the files so time estimation in progress bars is more accurate
             random.shuffle(rel_paths)
 
+            # get a list of which metadata files already exist
             existing_metadata_names = set(
                 sub_prefix(path, meta_prefix).strip(METADATA_SUFFIX) for path in glob_path(meta_prefix)
             )
 
             for path in rel_paths:
                 if not self.ignore_existing and path in existing_metadata_names:
                     continue
```

### Comparing `dolma-0.6.5/python/dolma/core/paths.py` & `dolma-0.7.0/python/dolma/core/paths.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,32 @@
     "sub_suffix",
     "make_relative",
     "mkdir_p",
     "split_path",
     "join_path",
     "is_glob",
     "split_glob",
+    "partition_path",
 ]
 
 
 FS_KWARGS: Dict[str, Dict[str, Any]] = {
     "": {"auto_mkdir": True},
 }
 
 
+RE_ANY_ESCAPE = re.compile(r"(?<!\\)(\*\?\[\])")
+RE_GLOB_STAR_ESCAPE = re.compile(r"(?<!\\)\*")
+RE_GLOB_ONE_ESCAPE = re.compile(r"(?<!\\)\?")
+RE_GLOB_OPEN_ESCAPE = re.compile(r"(?<!\\)\[")
+RE_GLOB_CLOSE_ESCAPE = re.compile(r"(?<!\\)\]")
+ESCAPE_SYMBOLS_MAP = {"*": "\u2581", "?": "\u2582", "[": "\u2583", "]": "\u2584"}
+REVERSE_ESCAPE_SYMBOLS_MAP = {v: k for k, v in ESCAPE_SYMBOLS_MAP.items()}
+
+
 def _get_fs(path: Union[Path, str]) -> AbstractFileSystem:
     """
     Get the filesystem class for a given path.
     """
     path = str(path)
     protocol = urlparse(path).scheme
     fs = get_filesystem_class(protocol)(**FS_KWARGS.get(protocol, {}))
@@ -42,32 +52,29 @@
     return fs
 
 
 def _escape_glob(s: Union[str, Path]) -> str:
     """
     Escape glob characters in a string.
     """
-    r"(?<!\\)[*?[\]]"
     s = str(s)
-    s = re.sub(r"(?<!\\)\*", "\u2581", s)
-    s = re.sub(r"(?<!\\)\?", "\u2582", s)
-    s = re.sub(r"(?<!\\)\[", "\u2583", s)
-    s = re.sub(r"(?<!\\)\]", "\u2584", s)
+    s = RE_GLOB_STAR_ESCAPE.sub(ESCAPE_SYMBOLS_MAP["*"], s)
+    s = RE_GLOB_ONE_ESCAPE.sub(ESCAPE_SYMBOLS_MAP["?"], s)
+    s = RE_GLOB_OPEN_ESCAPE.sub(ESCAPE_SYMBOLS_MAP["["], s)
+    s = RE_GLOB_CLOSE_ESCAPE.sub(ESCAPE_SYMBOLS_MAP["]"], s)
     return s
 
 
 def _unescape_glob(s: Union[str, Path]) -> str:
     """
     Unescape glob characters in a string.
     """
     s = str(s)
-    s = re.sub("\u2581", "*", s)
-    s = re.sub("\u2582", "?", s)
-    s = re.sub("\u2583", "[", s)
-    s = re.sub("\u2584", "]", s)
+    for k, v in REVERSE_ESCAPE_SYMBOLS_MAP.items():
+        s = s.replace(k, v)
     return s
 
 
 def _pathify(path: Union[Path, str]) -> Tuple[str, Path]:
     """
     Return the protocol and path of a given path.
     """
@@ -83,41 +90,64 @@
     """
     path_str = _unescape_glob(str(path))
     if protocol:
         path_str = f"{protocol}://{path_str.lstrip('/')}"
     return path_str
 
 
+def partition_path(path: str) -> Tuple[str, Tuple[str, ...], Tuple[str, ...]]:
+    """Partition a path into its protocol, symbols before a glob, and symbols after a glob."""
+    # split the path into its protocol and path components
+    prot, path_obj = _pathify(path)
+
+    # we need to first figure out if this path has a glob by checking if any of the escaped symbols for
+    # globs are in the path.
+    glob_locs = [i for i, p in enumerate(path_obj.parts) if any(c in p for c in REVERSE_ESCAPE_SYMBOLS_MAP)]
+
+    # make the path components before the glob
+    pre_glob_path = path_obj.parts[: glob_locs[0]] if glob_locs else path_obj.parts
+    pre_glob_path = tuple(_unescape_glob(p) for p in pre_glob_path)
+
+    # make the path components after the glob
+    post_glob_path = path_obj.parts[glob_locs[0] + 1 :] if glob_locs else ()
+    post_glob_path = tuple(_unescape_glob(p) for p in post_glob_path)
+
+    return prot, pre_glob_path, post_glob_path
+
+
 def split_path(path: str) -> Tuple[str, Tuple[str, ...]]:
     """
     Split a path into its protocol and path components.
     """
     protocol, _path = _pathify(path)
     return protocol, tuple(_unescape_glob(p) for p in _path.parts)
 
 
-def join_path(protocol: str, *parts: Union[str, Iterable[str]]) -> str:
+def join_path(protocol: Union[str, None], *parts: Union[str, Iterable[str]]) -> str:
     """
     Join a path from its protocol and path components.
     """
     all_parts = (_escape_glob(p) for p in chain.from_iterable([p] if isinstance(p, str) else p for p in parts))
     path = str(Path(*all_parts)).rstrip("/")
     if protocol:
         path = f"{protocol}://{path.lstrip('/')}"
     return _unescape_glob(path)
 
 
-def glob_path(path: Union[Path, str], hidden_files: bool = False) -> Iterator[str]:
+def glob_path(path: Union[Path, str], hidden_files: bool = False, autoglob_dirs: bool = True) -> Iterator[str]:
     """
     Expand a glob path into a list of paths.
     """
     path = str(path)
     protocol = urlparse(path).scheme
     fs = _get_fs(path)
 
+    if fs.isdir(path) and autoglob_dirs:
+        path = join_path(None, path, "*")
+
     for gl in fs.glob(path):
         gl = str(gl)
 
         if not hidden_files and Path(gl).name.startswith("."):
             continue
 
         yield join_path(protocol, gl)
@@ -187,22 +217,21 @@
 
 
 def make_relative(paths: List[str]) -> Tuple[str, List[str]]:
     """Find minimum longest root shared among all paths"""
     if len(paths) == 0:
         raise ValueError("Cannot make relative path of empty list")
 
-    common_prot, common_parts = (p := _pathify(paths[0]))[0], p[1].parts
+    common_prot, common_parts, _ = partition_path(paths[0])
 
     for path in paths:
-        current_prot, current_path = _pathify(path)
+        current_prot, current_parts, _ = partition_path(path)
         if current_prot != common_prot:
             raise ValueError(f"Protocols of {path} and {paths[0]} do not match")
 
-        current_parts = current_path.parts
         for i in range(min(len(common_parts), len(current_parts))):
             if common_parts[i] != current_parts[i]:
                 common_parts = common_parts[:i]
                 break
 
     if len(common_parts) > 0:
         common_path = (f"{common_prot}://" if common_prot else "") + str(Path(*common_parts))
```

### Comparing `dolma-0.6.5/python/dolma/core/registry.py` & `dolma-0.7.0/python/dolma/core/registry.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/core/taggers.py` & `dolma-0.7.0/python/dolma/core/taggers.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 Filters.
 
 @kylel, @soldni
 
 """
 from abc import abstractmethod
-from typing import Dict, List, Union
+from typing import List
 
-from .data_types import DocResult, Document, InputSpec
+from .data_types import DocResult, Document, InputSpec, TaggerOutputDictType
+
+# digits after the decimal point
+TAGGER_SCORE_PRECISION = 5
 
 
 class BaseTagger:
     FIELDS: List[str] = ["text"]
 
     @classmethod
     def train(cls, *args, **kwargs):
@@ -22,16 +25,17 @@
     def test(cls, *args, **kwargs):
         raise RuntimeError("This tagger does not support testing")
 
     @abstractmethod
     def predict(self, doc: Document) -> DocResult:
         raise NotImplementedError
 
-    def tag(self, row: InputSpec) -> Dict[str, List[List[Union[int, float]]]]:
+    def tag(self, row: InputSpec) -> TaggerOutputDictType:
         """Internal function that is used by the tagger to get data"""
         doc = Document(source=row.source, version=row.version, id=row.id, text=row.text)
         doc_result = self.predict(doc)
 
-        tagger_output: Dict[str, list] = {}
+        tagger_output: TaggerOutputDictType = {}
         for span in doc_result.spans:
-            tagger_output.setdefault(span.type, []).append([span.start, span.end, round(float(span.score), 5)])
+            output = (span.start, span.end, round(float(span.score), TAGGER_SCORE_PRECISION))
+            tagger_output.setdefault(span.type, []).append(output)
         return tagger_output
```

### Comparing `dolma-0.6.5/python/dolma/core/utils.py` & `dolma-0.7.0/python/dolma/core/utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/core/vizualizer.py` & `dolma-0.7.0/python/dolma/core/vizualizer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/data/naughty_words_en.txt` & `dolma-0.7.0/python/dolma/data/naughty_words_en.txt`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/taggers/c4.py` & `dolma-0.7.0/python/dolma/taggers/c4.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/taggers/code.py` & `dolma-0.7.0/python/dolma/taggers/code.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/taggers/gopher.py` & `dolma-0.7.0/python/dolma/taggers/gopher.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/taggers/jigsaw.py` & `dolma-0.7.0/python/dolma/taggers/jigsaw.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/taggers/language.py` & `dolma-0.7.0/python/dolma/taggers/language.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/taggers/length.py` & `dolma-0.7.0/python/dolma/taggers/length.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/taggers/pii.py` & `dolma-0.7.0/python/dolma/taggers/pii.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/python/dolma/taggers/sampling.py` & `dolma-0.7.0/python/dolma/taggers/sampling.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/res/logo.png` & `dolma-0.7.0/res/logo.png`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/src/bloom_filter.rs` & `dolma-0.7.0/src/bloom_filter.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/src/deduper.rs` & `dolma-0.7.0/src/deduper.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/src/lib.rs` & `dolma-0.7.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/src/mixer.rs` & `dolma-0.7.0/src/mixer.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/src/s3_util.rs` & `dolma-0.7.0/src/s3_util.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/src/shard.rs` & `dolma-0.7.0/src/shard.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/config/c4-cleaned.json` & `dolma-0.7.0/tests/config/c4-cleaned.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/config/dedupe-by-url.json` & `dolma-0.7.0/tests/config/dedupe-by-url.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/config/dedupe-paragraphs.json` & `dolma-0.7.0/tests/config/dedupe-paragraphs.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/config/email-spans.json` & `dolma-0.7.0/tests/config/email-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/config/filter-by-spans.json` & `dolma-0.7.0/tests/config/filter-by-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/config/mixer.json` & `dolma-0.7.0/tests/config/mixer.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/config/paragraph-spans.json` & `dolma-0.7.0/tests/config/paragraph-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/expected/dedupe-paragraphs.json.gz` & `dolma-0.7.0/tests/data/expected/dedupe-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/expected/email-spans.json.gz` & `dolma-0.7.0/tests/data/expected/email-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/expected/filter-by-spans.json.gz` & `dolma-0.7.0/tests/data/expected/filter-by-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/expected/mixer.json.gz` & `dolma-0.7.0/tests/data/expected/mixer.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/expected/remove-paragraphs.json.gz` & `dolma-0.7.0/tests/data/expected/remove-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/provided/attributes/duplicate_paragraphs/000.json.gz` & `dolma-0.7.0/tests/data/provided/attributes/duplicate_paragraphs/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/provided/attributes/pii/000.json.gz` & `dolma-0.7.0/tests/data/provided/attributes/pii/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/provided/attributes/sample/000.json.gz` & `dolma-0.7.0/tests/data/provided/attributes/sample/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/provided/attributes/toxicity/000.json.gz` & `dolma-0.7.0/tests/data/provided/attributes/toxicity/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/data/provided/documents/000.json.gz` & `dolma-0.7.0/tests/data/provided/documents/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/python/test_data_types.py` & `dolma-0.7.0/tests/python/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/python/test_deduper.py` & `dolma-0.7.0/tests/python/test_deduper.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/python/test_mixer.py` & `dolma-0.7.0/tests/python/test_mixer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/python/test_omegaconf.py` & `dolma-0.7.0/tests/python/test_omegaconf.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/python/test_parallel.py` & `dolma-0.7.0/tests/python/test_parallel.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/python/test_paths.py` & `dolma-0.7.0/tests/python/test_paths.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/python/test_taggers.py` & `dolma-0.7.0/tests/python/test_taggers.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/python/test_utils.py` & `dolma-0.7.0/tests/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/tests/python/utils.py` & `dolma-0.7.0/tests/python/utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.5/Cargo.lock` & `dolma-0.7.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -678,15 +678,15 @@
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "dolma"
-version = "0.6.5"
+version = "0.7.0"
 dependencies = [
  "ahash",
  "aws-config",
  "aws-sdk-s3",
  "byteorder",
  "clap",
  "env_logger",
```

### Comparing `dolma-0.6.5/PKG-INFO` & `dolma-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolma
-Version: 0.6.5
+Version: 0.7.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: anyascii >=0.3.2
 Requires-Dist: blingfire ==0.1.8
```

