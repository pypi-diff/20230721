# Comparing `tmp/dkist-processing-common-4.0.2rc1.tar.gz` & `tmp/dkist-processing-common-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-4.0.2rc1.tar", last modified: Mon Jul 17 18:06:12 2023, max compression
+gzip compressed data, was "dkist-processing-common-4.1.0rc1.tar", last modified: Fri Jul 21 19:08:30 2023, max compression
```

## Comparing `dkist-processing-common-4.0.2rc1.tar` & `dkist-processing-common-4.1.0rc1.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    14872 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.747940 dkist-processing-common-4.0.2rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/changelog/142.bugfix.rst
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/changelog/143.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.747940 dkist-processing-common-4.0.2rc1/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.747940 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.751940 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.751940 dkist-processing-common-4.0.2rc1/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.751940 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     8046 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.751940 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.755940 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11528 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8689 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.755940 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13491 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.755940 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47891 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2364 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18462 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     3843 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3159 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10564 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36336 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11883 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.747940 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1701 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.539888 dkist-processing-common-4.1.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    15229 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-21 19:08:30.543888 dkist-processing-common-4.1.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.531887 dkist-processing-common-4.1.0rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/changelog/145.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.531887 dkist-processing-common-4.1.0rc1/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.531887 dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.531887 dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.535888 dkist-processing-common-4.1.0rc1/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.535888 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4993 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     8088 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.535888 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7860 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.535888 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11528 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.539888 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13491 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.539888 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47891 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2364 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18462 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.539888 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    16288 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10564 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36336 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_task_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11883 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.531887 dkist-processing-common-4.1.0rc1/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-21 19:08:30.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2023-07-21 19:08:30.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-21 19:08:30.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-21 19:08:30.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-21 19:08:30.000000 dkist-processing-common-4.1.0rc1/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.539888 dkist-processing-common-4.1.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-21 19:08:30.539888 dkist-processing-common-4.1.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-07-21 19:08:30.543888 dkist-processing-common-4.1.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-21 19:08:25.000000 dkist-processing-common-4.1.0rc1/setup.py
```

### Comparing `dkist-processing-common-4.0.2rc1/.gitignore` & `dkist-processing-common-4.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/.pre-commit-config.yaml` & `dkist-processing-common-4.1.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/CHANGELOG.rst` & `dkist-processing-common-4.1.0rc1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v4.0.2 (2023-07-17)
+===================
+
+Bugfixes
+--------
+
+- Updates to support new major revisions of `pillow` and `pydantic`. (`#142 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/142>`__)
+
+
+Misc
+----
+
+- Update to latest dkist-header-validator. (`#143 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/143>`__)
+
+
 v4.0.1 (2023-07-11)
 ===================
 
 Misc
 ----
 
 - Update core dependency for airflow upgrade. (`#143 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/143>`__)
```

### Comparing `dkist-processing-common-4.0.2rc1/PKG-INFO` & `dkist-processing-common-4.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 4.0.2rc1
+Version: 4.1.0rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-4.0.2rc1/README.rst` & `dkist-processing-common-4.1.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/bitbucket-pipelines.yml` & `dkist-processing-common-4.1.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/check_changelog_updated.sh` & `dkist-processing-common-4.1.0rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/config.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/constants.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,28 +36,28 @@
 
         Returns
         -------
         The value popped from the set.
         """
         return json.loads(value.pop())
 
-    def __getitem__(self, key: str) -> int | str | float:
+    def __getitem__(self, key: str) -> int | str | float | tuple:
         """Return the constant stored at a specific key. Raise and error if the key doesn't exist."""
         if isinstance(key, Enum):
             key = key.value
         value = self.store.all(key)
         if not value:
             raise KeyError(f"Constant {key} does not exist")
         return self.extract_value(value)
 
     def __delitem__(self, key: str):
         """'delete' a key by making it map to an empty set."""
         self.store.clear_tag(key)
 
-    def __setitem__(self, key: str, value: str | int | float):
+    def __setitem__(self, key: str, value: str | int | float | tuple):
         """Set a constant key with the specified value. Raise an error if the key already exists."""
         if self.store.all(key):
             raise ValueError(f"Constant {key} already exists")
         self.store.add(key, json.dumps(value))
 
     def __iter__(self) -> Generator[str, None, None]:
         """Yield the currently defined constants as strings."""
```

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/tags.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/json.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/str.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/manual.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/constants.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     contributing_experiment_ids = "CONTRIBUTING_EXPERIMENT_IDS"
     average_cadence = "AVERAGE_CADENCE"
     maximum_cadence = "MAXIMUM_CADENCE"
     minimum_cadence = "MINIMUM_CADENCE"
     variance_cadence = "VARIANCE_CADENCE"
     num_dsps_repeats = "NUM_DSPS_REPEATS"
     dark_exposure_times = "DARK_EXPOSURE_TIMES"
+    dark_readout_exp_times = "DARK_READOUT_EXP_TIMES"
 
 
 class ConstantsBase:
     """
     Aggregate (from the constant buds flower pot) in a single property on task classes.
 
     It also provides some default constants, but is intended to be subclassed by instruments.
@@ -123,17 +124,22 @@
 
     @property
     def num_dsps_repeats(self) -> int:
         """Get the number of dsps repeats."""
         return self._db_dict[BudName.num_dsps_repeats]
 
     @property
-    def dark_exposure_times(self) -> list[float]:
+    def dark_exposure_times(self) -> tuple[float, ...]:
         """Get a list of exposure times used in the dark calibration."""
-        return self._db_dict[BudName.dark_exposure_times]  # TODO type hinting mismatch here
+        return self._db_dict[BudName.dark_exposure_times]
+
+    @property
+    def dark_readout_exp_times(self) -> tuple[float, ...]:
+        """Get a list of readout exp times for all DARK frames."""
+        return self._db_dict[BudName.dark_readout_exp_times]
 
     @property
     def stokes_params(self) -> [str]:
         """Return the list of stokes parameter names."""
         return ["I", "Q", "U", "V"]
 
     @property
```

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/graphql.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/message.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/parameters.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/quality.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/tags.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     task = "TASK"
     cs_step = "CS_STEP"
     modstate = "MODSTATE"
     dsps_repeat = "DSPS_REPEAT"
     calibrated = "CALIBRATED"  # A flag to indicate the data has been calibrated but not yet output
     quality = "QUALITY"
     exposure_time = "EXP_TIME"
+    readout_exp_time = "READOUT_EXP_TIME"
     quality_task = "QUALITY_TASK"
     parameter = "PARAMETER"
     workflow_task = "WORKFLOW_TASK"
     debug = "DEBUG"
 
 
 class Tag:
```

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         self.instrument: str = self.header["INSTRUME"]
         self.wavelength: float = self.header["LINEWAV"]
         self.proposal_id: str = self.header["PROP_ID"]
         self.experiment_id: str = self.header["EXPER_ID"]
         self.num_dsps_repeats: int = self.header["DSPSREPS"]
         self.current_dsps_repeat: int = self.header["DSPSNUM"]
         self.fpa_exposure_time_ms: float = self.header["XPOSURE"]
+        self.sensor_readout_exposure_time_ms: float = self.header["TEXPOSUR"]
+        self.num_raw_frames_per_fpa: int = self.header["NSUMEXP"]
 
     @property
     def gos_polarizer_angle(self) -> float:
         """Convert the polarizer angle to a float if possible before returning."""
         try:
             return float(self.header["POLANGLE"])
         except ValueError:
```

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/base.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,88 +3,100 @@
 
 from dkist_processing_common.models.constants import BudName
 from dkist_processing_common.models.fits_access import FitsAccessBase
 from dkist_processing_common.models.tags import StemName
 from dkist_processing_common.parsers.cs_step import CSStepFlower
 from dkist_processing_common.parsers.cs_step import NumCSStepBud
 from dkist_processing_common.parsers.dsps_repeat import DspsRepeatNumberFlower
-from dkist_processing_common.parsers.dsps_repeat import TotalDspsRepeatsBud
 from dkist_processing_common.parsers.proposal_id_bud import ProposalIdBud
 from dkist_processing_common.parsers.single_value_single_key_flower import (
     SingleValueSingleKeyFlower,
 )
 from dkist_processing_common.parsers.time import AverageCadenceBud
 from dkist_processing_common.parsers.time import ExposureTimeFlower
 from dkist_processing_common.parsers.time import MaximumCadenceBud
 from dkist_processing_common.parsers.time import MinimumCadenceBud
+from dkist_processing_common.parsers.time import ReadoutExpTimeFlower
 from dkist_processing_common.parsers.time import TaskExposureTimesBud
+from dkist_processing_common.parsers.time import TaskNumReadoutsPerFpaBud
+from dkist_processing_common.parsers.time import TaskReadoutExpTimesBud
 from dkist_processing_common.parsers.time import VarianceCadenceBud
 from dkist_processing_common.parsers.unique_bud import UniqueBud
 
 
 class FitsReader(FitsAccessBase):
     def __init__(self, hdu, name):
         super().__init__(hdu, name)
         self.thing_id: int = self.header["id_key"]
         self.constant_thing: float = self.header["constant"]
         self.name = name
         self.proposal_id: str = self.header.get("ID___013")
         self.ip_task_type: str = self.header.get("DKIST004")
-        self.fpa_exposure_time_ms: float = self.header.get("TEXPOSUR")
+        self.fpa_exposure_time_ms: float = self.header.get("XPOSURE")
+        self.sensor_readout_exposure_time_ms: float = self.header.get("TEXPOSUR")
+        self.num_raw_frames_per_fpa: int = self.header.get("NSUMEXP")
         self.num_dsps_repeats: int = self.header["DSPSREPS"]
         self.current_dsps_repeat: int = self.header["DSPSNUM"]
         self.time_obs: str = self.header["DATE-OBS"]
 
 
 @pytest.fixture()
 def basic_header_objs():
     header_dict = {
         "thing0": fits.header.Header(
             {
                 "id_key": 0,
                 "constant": 6.28,
                 "DKIST004": "observe",
                 "ID___013": "proposal_id_1",
-                "TEXPOSUR": 0.0013000123,
+                "XPOSURE": 0.0013000123,
+                "TEXPOSUR": 10.0,
+                "NSUMEXP": 3,
                 "DSPSNUM": 1,
                 "DSPSREPS": 2,
                 "DATE-OBS": "2022-06-17T22:00:00.000",
             }
         ),
         "thing1": fits.header.Header(
             {
                 "id_key": 1,
                 "constant": 6.28,
                 "DKIST004": "observe",
                 "ID___013": "proposal_id_1",
-                "TEXPOSUR": 0.0013000987,
+                "XPOSURE": 0.0013000987,
+                "TEXPOSUR": 10.0,
+                "NSUMEXP": 3,
                 "DSPSNUM": 1,
                 "DSPSREPS": 2,
                 "DATE-OBS": "2022-06-17T22:00:01.000",
             }
         ),
         "thing2": fits.header.Header(
             {
                 "id_key": 2,
                 "constant": 6.28,
                 "DKIST004": "dark",
                 "ID___013": "proposal_id_2",
-                "TEXPOSUR": 12.345,
+                "XPOSURE": 12.345,
+                "TEXPOSUR": 1.123456789,
+                "NSUMEXP": 1,
                 "DSPSNUM": 2,
                 "DSPSREPS": 2,
                 "DATE-OBS": "2022-06-17T22:00:02.000",
             }
         ),
         "thing3": fits.header.Header(
             {
                 "id_key": 0,
                 "constant": 6.28,
                 "DKIST004": "observe",
                 "ID___013": "proposal_id_1",
-                "TEXPOSUR": 100.0,
+                "XPOSURE": 100.0,
+                "TEXPOSUR": 11.0,
+                "NSUMEXP": 4,
                 "DSPSNUM": 2,
                 "DSPSREPS": 2,
                 "DATE-OBS": "2022-06-17T22:00:03.000",
             }
         ),
     }
     return (FitsReader.from_header(header, name=path) for path, header in header_dict.items())
@@ -227,15 +239,15 @@
     petal = list(bud.petals)
     assert len(petal) == 1
     assert petal[0].value == "proposal_id_1"
 
 
 def test_exp_time_flower(basic_header_objs):
     """
-    Given: A set of filepaths and associated headers with TEXPOSUR keywords
+    Given: A set of filepaths and associated headers with XPOSURE keywords
     When: Ingesting with an ExposureTimeFlower
     Then: The filepaths are grouped correctly based on their exposure time
     """
     flower = ExposureTimeFlower()
     assert flower.stem_name == StemName.exposure_time.value
     for fo in basic_header_objs:
         key = fo.name
@@ -247,18 +259,40 @@
     assert petals[0].keys == ["thing0", "thing1"]
     assert petals[1].value == 12.345
     assert petals[1].keys == ["thing2"]
     assert petals[2].value == 100.0
     assert petals[2].keys == ["thing3"]
 
 
-def test_exp_times_seed(basic_header_objs):
+def test_readout_exp_time_flower(basic_header_objs):
+    """
+    Given: A set of filepaths and associated headers with TEXPOSUR keywords
+    When: Ingesting with an ReadoutExpTimeFlower
+    Then: The filepaths are grouped correctly based on their readout exposure time
+    """
+    flower = ReadoutExpTimeFlower()
+    assert flower.stem_name == StemName.readout_exp_time.value
+    for fo in basic_header_objs:
+        key = fo.name
+        flower.update(key, fo)
+
+    petals = sorted(list(flower.petals), key=lambda x: x.value)
+    assert len(petals) == 3
+    assert petals[0].value == 1.123457
+    assert petals[0].keys == ["thing2"]
+    assert petals[1].value == 10.0
+    assert petals[1].keys == ["thing0", "thing1"]
+    assert petals[2].value == 11.0
+    assert petals[2].keys == ["thing3"]
+
+
+def test_fpa_exp_times_bud(basic_header_objs):
     """
     Given: A set of filepaths and associated headers with XPOSURE keywords
-    When: Ingesting with an ExposureTimesBud
+    When: Ingesting with a TaskExposureTimesBud
     Then: All (rounded) exposure times are accounted for in the resulting tuple
     """
     dark_bud = TaskExposureTimesBud(stem_name=BudName.dark_exposure_times, ip_task_type="DARK")
     obs_bud = TaskExposureTimesBud(stem_name="obs_exp_times", ip_task_type="OBSERVE")
     assert dark_bud.stem_name == BudName.dark_exposure_times.value
     for fo in basic_header_objs:
         key = fo.name
@@ -272,14 +306,64 @@
 
     obs_petal = list(obs_bud.petals)
     assert len(obs_petal) == 1
     assert type(obs_petal[0].value) is tuple
     assert tuple(sorted(obs_petal[0].value)) == (0.0013, 100.0)
 
 
+def test_readout_exp_times_bud(basic_header_objs):
+    """
+    Given: A set of filepaths and associated headers with TEXPOSUR keywords
+    When: Ingesting with a TaskReadoutExpTimesBud
+    Then: All (rounded) exposure times are accounted for in the resulting tuple
+    """
+    dark_bud = TaskReadoutExpTimesBud(stem_name=BudName.dark_exposure_times, ip_task_type="DARK")
+    obs_bud = TaskReadoutExpTimesBud(stem_name="obs_exp_times", ip_task_type="OBSERVE")
+    assert dark_bud.stem_name == BudName.dark_exposure_times.value
+    for fo in basic_header_objs:
+        key = fo.name
+        dark_bud.update(key, fo)
+        obs_bud.update(key, fo)
+
+    dark_petal = list(dark_bud.petals)
+    assert len(dark_petal) == 1
+    assert type(dark_petal[0].value) is tuple
+    assert tuple(sorted(dark_petal[0].value)) == (1.123457,)
+
+    obs_petal = list(obs_bud.petals)
+    assert len(obs_petal) == 1
+    assert type(obs_petal[0].value) is tuple
+    assert tuple(sorted(obs_petal[0].value)) == (10.0, 11.0)
+
+
+def test_exp_times_bud(basic_header_objs):
+    """
+    Given: A set of filepaths and associated headers with NSUMEXP keywords
+    When: Ingesting with a TaskNumReadoutsPerFpaBud
+    Then: All NSUMEXP values are accounted for in the resulting tuple
+    """
+    dark_bud = TaskNumReadoutsPerFpaBud(stem_name=BudName.dark_exposure_times, ip_task_type="DARK")
+    obs_bud = TaskNumReadoutsPerFpaBud(stem_name="obs_exp_times", ip_task_type="OBSERVE")
+    assert dark_bud.stem_name == BudName.dark_exposure_times.value
+    for fo in basic_header_objs:
+        key = fo.name
+        dark_bud.update(key, fo)
+        obs_bud.update(key, fo)
+
+    dark_petal = list(dark_bud.petals)
+    assert len(dark_petal) == 1
+    assert type(dark_petal[0].value) is tuple
+    assert tuple(sorted(dark_petal[0].value)) == (1,)
+
+    obs_petal = list(obs_bud.petals)
+    assert len(obs_petal) == 1
+    assert type(obs_petal[0].value) is tuple
+    assert tuple(sorted(obs_petal[0].value)) == (3, 4)
+
+
 def test_dsps_flower(basic_header_objs):
     """
     Given: A set of filepaths and associated headers with DSPS keywords
     When: Ingesting with a DspsRepeatNumber Flower
     Then: The correct values are returned
     """
     flower = DspsRepeatNumberFlower()
```

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-4.1.0rc1/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-4.1.0rc1/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 4.0.2rc1
+Version: 4.1.0rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-4.1.0rc1/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
-changelog/142.bugfix.rst
-changelog/143.misc.rst
+changelog/145.feature.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
@@ -51,14 +50,15 @@
 dkist_processing_common/parsers/experiment_id_bud.py
 dkist_processing_common/parsers/id_bud.py
 dkist_processing_common/parsers/l0_fits_access.py
 dkist_processing_common/parsers/l1_fits_access.py
 dkist_processing_common/parsers/proposal_id_bud.py
 dkist_processing_common/parsers/quality.py
 dkist_processing_common/parsers/single_value_single_key_flower.py
+dkist_processing_common/parsers/task.py
 dkist_processing_common/parsers/time.py
 dkist_processing_common/parsers/unique_bud.py
 dkist_processing_common/tasks/__init__.py
 dkist_processing_common/tasks/assemble_movie.py
 dkist_processing_common/tasks/base.py
 dkist_processing_common/tasks/l1_output_data.py
 dkist_processing_common/tasks/output_data_base.py
@@ -95,14 +95,15 @@
 dkist_processing_common/tests/test_parameters.py
 dkist_processing_common/tests/test_parse_l0_input_data.py
 dkist_processing_common/tests/test_publish_catalog_messages.py
 dkist_processing_common/tests/test_quality.py
 dkist_processing_common/tests/test_quality_mixin.py
 dkist_processing_common/tests/test_scratch.py
 dkist_processing_common/tests/test_tags.py
+dkist_processing_common/tests/test_task_parsing.py
 dkist_processing_common/tests/test_teardown.py
 dkist_processing_common/tests/test_transfer_input_data.py
 dkist_processing_common/tests/test_transfer_l1_output_data.py
 dkist_processing_common/tests/test_trial_output_data.py
 dkist_processing_common/tests/test_workflow_task_base.py
 dkist_processing_common/tests/test_write_l1.py
 docs/Makefile
```

### Comparing `dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-4.1.0rc1/dkist_processing_common.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+astropy>=5.1.1
+dkist-fits-specifications>=3.0.0
+dkist-header-validator>=4.0.0
 dkist-processing-core==2.0.2
 dkist-processing-pac>=2.1.1
-dkist-header-validator>=4.0.0rc2
-dkist-fits-specifications>=3.0.0
-astropy>=5.1.1
-numpy>=1.20.2
-pandas>=1.4.2
-hashids==1.3.1
+dkist-spectral-lines>=2.0.0
 globus-sdk>=3.12.0
 gqlclient==0.9.6
-talus==0.2.1
-redis==4.6.0
+hashids==1.3.1
+matplotlib>=3.4
+moviepy>=1.0.3
+numpy>=1.20.2
 object-clerk==0.1.0
-requests>=2.23
-scipy>=1.6.3
-sunpy>=3.0.0
+pandas>=1.4.2
 pillow>=8.3.0
-moviepy>=1.0.3
-matplotlib>=3.4
 pydantic>=1.8.1
+redis==4.6.0
+requests>=2.23
 retry>=0.9.2
-dkist-spectral-lines>=2.0.0
+scipy>=1.6.3
+sunpy>=3.0.0
+talus==0.2.1
 
 [docs]
 sphinx
 sphinx-astropy
 sphinx-changelog
 sphinx-autoapi
 pytest
```

### Comparing `dkist-processing-common-4.0.2rc1/docs/Makefile` & `dkist-processing-common-4.1.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/docs/conf.py` & `dkist-processing-common-4.1.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/docs/make.bat` & `dkist-processing-common-4.1.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/licenses/LICENSE.rst` & `dkist-processing-common-4.1.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/pyproject.toml` & `dkist-processing-common-4.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2rc1/setup.cfg` & `dkist-processing-common-4.1.0rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
+	astropy >= 5.1.1
+	dkist-fits-specifications >= 3.0.0
+	dkist-header-validator >= 4.0.0
 	dkist-processing-core == 2.0.2
 	dkist-processing-pac >= 2.1.1
-	dkist-header-validator >= 4.0.0rc2
-	dkist-fits-specifications >= 3.0.0
-	astropy >= 5.1.1
-	numpy >= 1.20.2
-	pandas >= 1.4.2
-	hashids == 1.3.1
+	dkist-spectral-lines >= 2.0.0
 	globus-sdk >= 3.12.0
 	gqlclient == 0.9.6
-	talus == 0.2.1
-	redis == 4.6.0
+	hashids == 1.3.1
+	matplotlib >= 3.4
+	moviepy >= 1.0.3
+	numpy >= 1.20.2
 	object-clerk == 0.1.0
-	requests >= 2.23
-	scipy >= 1.6.3
-	sunpy >= 3.0.0
+	pandas >= 1.4.2
 	pillow >= 8.3.0
-	moviepy >= 1.0.3
-	matplotlib >= 3.4
 	pydantic >= 1.8.1
+	redis == 4.6.0
+	requests >= 2.23
 	retry >= 0.9.2
-	dkist-spectral-lines >= 2.0.0
+	scipy >= 1.6.3
+	sunpy >= 3.0.0
+	talus == 0.2.1
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-xdist
 	pytest-cov
 	pytest-mock
```

