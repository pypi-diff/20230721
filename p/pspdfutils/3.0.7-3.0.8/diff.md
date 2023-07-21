# Comparing `tmp/pspdfutils-3.0.7.tar.gz` & `tmp/pspdfutils-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pspdfutils-3.0.7.tar", last modified: Fri Jul 21 18:16:36 2023, max compression
+gzip compressed data, was "pspdfutils-3.0.8.tar", last modified: Fri Jul 21 19:46:52 2023, max compression
```

## Comparing `pspdfutils-3.0.7.tar` & `pspdfutils-3.0.8.tar`

### file list

```diff
@@ -1,409 +1,409 @@
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.745442 pspdfutils-3.0.7/
--rw-r-----   0 rrt       (1000) rrt       (1000)    35148 2020-01-25 13:35:25.000000 pspdfutils-3.0.7/COPYING
--rw-r-----   0 rrt       (1000) rrt       (1000)      387 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/MANIFEST.in
--rw-r-----   0 rrt       (1000) rrt       (1000)     2935 2023-07-21 18:16:36.745442 pspdfutils-3.0.7/PKG-INFO
--rw-r-----   0 rrt       (1000) rrt       (1000)     2536 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/README.md
--rw-r-----   0 rrt       (1000) rrt       (1000)       73 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/epsffit-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      686 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/extractres-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      620 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/includeres-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      440 2020-01-25 13:35:25.000000 pspdfutils-3.0.7/man-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      866 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psbook-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      852 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psnup-include.man
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.649440 pspdfutils-3.0.7/pspdfutils.egg-info/
--rw-r-----   0 rrt       (1000) rrt       (1000)     2935 2023-07-21 18:16:36.000000 pspdfutils-3.0.7/pspdfutils.egg-info/PKG-INFO
--rw-r-----   0 rrt       (1000) rrt       (1000)    14540 2023-07-21 18:16:36.000000 pspdfutils-3.0.7/pspdfutils.egg-info/SOURCES.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        1 2023-07-21 18:16:36.000000 pspdfutils-3.0.7/pspdfutils.egg-info/dependency_links.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)      405 2023-07-21 18:16:36.000000 pspdfutils-3.0.7/pspdfutils.egg-info/entry_points.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)       31 2023-07-21 18:16:36.000000 pspdfutils-3.0.7/pspdfutils.egg-info/requires.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        8 2023-07-21 18:16:36.000000 pspdfutils-3.0.7/pspdfutils.egg-info/top_level.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)      298 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psresize-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)       68 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psselect-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)     3224 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/pstops-include.man
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.653440 pspdfutils-3.0.7/psutils/
--rw-r-----   0 rrt       (1000) rrt       (1000)      228 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/__init__.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     8381 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/argparse.py
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.653440 pspdfutils-3.0.7/psutils/command/
--rw-r-----   0 rrt       (1000) rrt       (1000)     5829 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/command/epsffit.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     4229 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/command/extractres.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1917 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/command/includeres.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     2872 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/command/psbook.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     9503 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/command/psjoin.py
--rw-r-----   0 rrt       (1000) rrt       (1000)    10324 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/command/psnup.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     2173 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/command/psresize.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     2685 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/command/psselect.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     3160 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/command/pstops.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1382 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/io.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1338 2023-07-21 08:35:17.000000 pspdfutils-3.0.7/psutils/libpaper.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      980 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/psresources.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     5044 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/readers.py
--rw-r-----   0 rrt       (1000) rrt       (1000)    19306 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/transformers.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1930 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/types.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      913 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils/warnings.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      931 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/psutils.1
--rw-r-----   0 rrt       (1000) rrt       (1000)     2817 2023-07-21 18:14:51.000000 pspdfutils-3.0.7/pyproject.toml
--rw-r-----   0 rrt       (1000) rrt       (1000)       38 2023-07-21 18:16:36.745442 pspdfutils-3.0.7/setup.cfg
--rw-r-----   0 rrt       (1000) rrt       (1000)      539 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/setup.py
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.657440 pspdfutils-3.0.7/tests/
--rw-r-----   0 rrt       (1000) rrt       (1000)      890 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/conftest.py
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.665440 pspdfutils-3.0.7/tests/test-files/
--rw-r-----   0 rrt       (1000) rrt       (1000)    13275 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a3-20.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23046 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a3-20.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     3332 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-1.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    17476 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-1.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     9028 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-11.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20384 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-11.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     3910 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-2.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    17766 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-2.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)    13208 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-20.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23021 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-20.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     4539 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-3.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18056 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-3.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     5005 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-4-0.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18320 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a4-4-0.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     3335 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a5-1.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    17475 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a5-1.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)    13277 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a5-20.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23020 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/a5-20.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.625440 pspdfutils-3.0.7/tests/test-files/epsffit/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.665440 pspdfutils-3.0.7/tests/test-files/epsffit/aspect/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.665440 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.669440 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-maximize/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-maximize/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-maximize/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.669440 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-maximize-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-maximize-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-maximize-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.669440 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.673441 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-maximize/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-maximize/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-maximize/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.673441 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-maximize-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-maximize-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-maximize-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.673441 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/aspect-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.673441 pspdfutils-3.0.7/tests/test-files/epsffit/center/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/center/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78699 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/center/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.673441 pspdfutils-3.0.7/tests/test-files/epsffit/center-maximize/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/center-maximize/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78699 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/center-maximize/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.677441 pspdfutils-3.0.7/tests/test-files/epsffit/center-maximize-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/center-maximize-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78710 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/center-maximize-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.677441 pspdfutils-3.0.7/tests/test-files/epsffit/center-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/center-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78710 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/center-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.677441 pspdfutils-3.0.7/tests/test-files/epsffit/h-texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/h-texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4432 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/h-texlive/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.677441 pspdfutils-3.0.7/tests/test-files/epsffit/m-texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/m-texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4441 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/m-texlive/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.677441 pspdfutils-3.0.7/tests/test-files/epsffit/maximize/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/maximize/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/maximize/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.677441 pspdfutils-3.0.7/tests/test-files/epsffit/maximize-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/maximize-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/maximize-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.677441 pspdfutils-3.0.7/tests/test-files/epsffit/no-options/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/no-options/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/no-options/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.677441 pspdfutils-3.0.7/tests/test-files/epsffit/rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.681441 pspdfutils-3.0.7/tests/test-files/epsffit/showpage/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/showpage/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78725 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/showpage/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.681441 pspdfutils-3.0.7/tests/test-files/epsffit/v-texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/v-texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4433 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/epsffit/v-texlive/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.629440 pspdfutils-3.0.7/tests/test-files/extractres/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.681441 pspdfutils-3.0.7/tests/test-files/extractres/sample/
--rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/ISO-8859-1Encoding-expected.enc
--rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/ISO-8859-1Encoding.enc
--rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02-expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01-expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11851 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)      256 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/includeres-expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    17478 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/extractres/sample/includeres-expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.629440 pspdfutils-3.0.7/tests/test-files/includeres/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.685441 pspdfutils-3.0.7/tests/test-files/includeres/sample/
--rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/includeres/sample/ISO-8859-1Encoding.enc
--rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/includeres/sample/a2ps-a2ps-hdr2.02.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/includeres/sample/a2ps-black+white-Prolog2.01.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)      280 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/includeres/sample/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    17476 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/includeres/sample/expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     4334 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/plot.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.629440 pspdfutils-3.0.7/tests/test-files/psbook/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.685441 pspdfutils-3.0.7/tests/test-files/psbook/20/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/20/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/20/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/20/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.685441 pspdfutils-3.0.7/tests/test-files/psbook/20-signature-4/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/20-signature-4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/20-signature-4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/20-signature-4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.685441 pspdfutils-3.0.7/tests/test-files/psbook/3/
--rw-r-----   0 rrt       (1000) rrt       (1000)       31 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/3/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2867 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/3/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18081 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/3/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.685441 pspdfutils-3.0.7/tests/test-files/psbook/3-signature-4/
--rw-r-----   0 rrt       (1000) rrt       (1000)       31 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/3-signature-4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2867 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/3-signature-4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18081 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/3-signature-4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.685441 pspdfutils-3.0.7/tests/test-files/psbook/invalid-signature-size/
--rw-r-----   0 rrt       (1000) rrt       (1000)       43 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/invalid-signature-size/expected-stderr.txt
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.689441 pspdfutils-3.0.7/tests/test-files/psbook/texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       66 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     7167 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20410 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psbook/texlive/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.633440 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.689441 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19350 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.689441 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-even/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-even/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     3169 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-even/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19502 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-even/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.689441 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-nostrip/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-nostrip/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-nostrip/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    35545 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-nostrip/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.689441 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-save/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-save/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-save/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19474 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-save/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.641440 pspdfutils-3.0.7/tests/test-files/psnup/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.689441 pspdfutils-3.0.7/tests/test-files/psnup/20-1/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.693441 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flip/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flip/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13904 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flip/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30718 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flip/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.693441 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    15184 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31098 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.693441 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13244 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.697441 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13024 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30858 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.697441 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13204 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.697441 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11029 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.701441 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13204 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.701441 pspdfutils-3.0.7/tests/test-files/psnup/20-2/
--rw-r-----   0 rrt       (1000) rrt       (1000)       87 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-2/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11994 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-2/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31268 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-2/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.701441 pspdfutils-3.0.7/tests/test-files/psnup/20-2-inpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)       87 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-2-inpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11314 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-2-inpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30887 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-2-inpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.705441 pspdfutils-3.0.7/tests/test-files/psnup/20-3/
--rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11577 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.705441 pspdfutils-3.0.7/tests/test-files/psnup/20-3-impossible-tolerance/
--rw-r-----   0 rrt       (1000) rrt       (1000)       46 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-impossible-tolerance/expected-stderr.txt
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.705441 pspdfutils-3.0.7/tests/test-files/psnup/20-3-inpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-inpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11357 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-inpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31678 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-inpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.705441 pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedleft/
--rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedleft/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11577 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedleft/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedleft/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.709441 pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedright/
--rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedright/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11592 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedright/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedright/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.709441 pspdfutils-3.0.7/tests/test-files/psnup/20-4/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9162 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30986 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.709441 pspdfutils-3.0.7/tests/test-files/psnup/20-4-297mmx210mm/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-297mmx210mm/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11323 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-297mmx210mm/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31346 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-297mmx210mm/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.709441 pspdfutils-3.0.7/tests/test-files/psnup/20-4-border-20/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-border-20/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9652 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-border-20/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31146 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-border-20/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.709441 pspdfutils-3.0.7/tests/test-files/psnup/20-4-columnmajor/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-columnmajor/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9162 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-columnmajor/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30986 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-columnmajor/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.713441 pspdfutils-3.0.7/tests/test-files/psnup/20-4-flip/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-flip/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10423 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-flip/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31346 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-flip/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.713441 pspdfutils-3.0.7/tests/test-files/psnup/20-4-impossible-border/
--rw-r-----   0 rrt       (1000) rrt       (1000)       28 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-impossible-border/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-impossible-border/expected.pdf
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.713441 pspdfutils-3.0.7/tests/test-files/psnup/20-4-impossible-margin/
--rw-r-----   0 rrt       (1000) rrt       (1000)       28 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-impossible-margin/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-impossible-margin/expected.pdf
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.713441 pspdfutils-3.0.7/tests/test-files/psnup/20-4-inpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-inpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9642 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-inpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31125 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-inpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.713441 pspdfutils-3.0.7/tests/test-files/psnup/20-4-margin-10/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-margin-10/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9552 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-margin-10/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31146 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/20-4-margin-10/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.713441 pspdfutils-3.0.7/tests/test-files/psnup/draw/
--rw-r-----   0 rrt       (1000) rrt       (1000)       25 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/draw/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     3397 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/draw/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    21521 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/draw/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.717441 pspdfutils-3.0.7/tests/test-files/psnup/texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       53 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     7710 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    26045 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/texlive/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.717441 pspdfutils-3.0.7/tests/test-files/psnup/texlive2/
--rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/texlive2/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9322 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/texlive2/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30184 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psnup/texlive2/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.641440 pspdfutils-3.0.7/tests/test-files/psresize/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.717441 pspdfutils-3.0.7/tests/test-files/psresize/20-A3/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A3/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13424 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A3/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30860 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A3/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.717441 pspdfutils-3.0.7/tests/test-files/psresize/20-A3in-A4/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A3in-A4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    12824 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A3in-A4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30901 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A3in-A4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.717441 pspdfutils-3.0.7/tests/test-files/psresize/20-A4/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.721441 pspdfutils-3.0.7/tests/test-files/psresize/20-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13024 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30858 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.721441 pspdfutils-3.0.7/tests/test-files/psresize/20-A5in-A4/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A5in-A4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13204 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A5in-A4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-A5in-A4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.721441 pspdfutils-3.0.7/tests/test-files/psresize/20-Letter/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-Letter/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13224 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-Letter/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30878 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psresize/20-Letter/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.645440 pspdfutils-3.0.7/tests/test-files/psselect/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.721441 pspdfutils-3.0.7/tests/test-files/psselect/even/
--rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/even/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     6613 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/even/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20103 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/even/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.721441 pspdfutils-3.0.7/tests/test-files/psselect/even-reverse/
--rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/even-reverse/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     6613 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/even-reverse/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20103 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/even-reverse/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.725441 pspdfutils-3.0.7/tests/test-files/psselect/individual-pages-and-dash-p/
--rw-r-----   0 rrt       (1000) rrt       (1000)       58 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/individual-pages-and-dash-p/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     6608 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/individual-pages-and-dash-p/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20111 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/individual-pages-and-dash-p/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.725441 pspdfutils-3.0.7/tests/test-files/psselect/invalid-pagerange/
--rw-r-----   0 rrt       (1000) rrt       (1000)       69 2023-05-19 21:27:44.000000 pspdfutils-3.0.7/tests/test-files/psselect/invalid-pagerange/.bak.0.expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)       37 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/invalid-pagerange/expected-stderr.txt
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.725441 pspdfutils-3.0.7/tests/test-files/psselect/negative-range/
--rw-r-----   0 rrt       (1000) rrt       (1000)       40 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/negative-range/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4423 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/negative-range/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18649 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/negative-range/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.725441 pspdfutils-3.0.7/tests/test-files/psselect/odd/
--rw-r-----   0 rrt       (1000) rrt       (1000)       61 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/odd/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     6609 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/odd/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20117 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/odd/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.729442 pspdfutils-3.0.7/tests/test-files/psselect/options-and-complex-pagerange/
--rw-r-----   0 rrt       (1000) rrt       (1000)       47 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/options-and-complex-pagerange/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     5295 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/options-and-complex-pagerange/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19243 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/options-and-complex-pagerange/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.729442 pspdfutils-3.0.7/tests/test-files/psselect/positive-negative-range/
--rw-r-----   0 rrt       (1000) rrt       (1000)       98 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/positive-negative-range/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10114 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/positive-negative-range/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    22455 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/positive-negative-range/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.729442 pspdfutils-3.0.7/tests/test-files/psselect/positive-range/
--rw-r-----   0 rrt       (1000) rrt       (1000)       35 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/positive-range/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4419 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/positive-range/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18655 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/positive-range/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.733441 pspdfutils-3.0.7/tests/test-files/psselect/psnup-texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       97 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/psnup-texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10113 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/psnup-texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    22453 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/psnup-texlive/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.733441 pspdfutils-3.0.7/tests/test-files/psselect/reverse/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/reverse/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/reverse/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/reverse/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.733441 pspdfutils-3.0.7/tests/test-files/psselect/texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       66 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     7048 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20410 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect/texlive/expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)    10113 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect-texlive-output.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    22453 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/psselect-texlive-output.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.645440 pspdfutils-3.0.7/tests/test-files/pstops/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.733441 pspdfutils-3.0.7/tests/test-files/pstops/correct-angles/
--rw-r-----   0 rrt       (1000) rrt       (1000)       21 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/correct-angles/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2050 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/correct-angles/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20081 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/correct-angles/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.737442 pspdfutils-3.0.7/tests/test-files/pstops/default-paper-size/
--rw-r-----   0 rrt       (1000) rrt       (1000)       21 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/default-paper-size/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2082 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/default-paper-size/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20120 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/default-paper-size/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.737442 pspdfutils-3.0.7/tests/test-files/pstops/invalid-pagespecs/
--rw-r-----   0 rrt       (1000) rrt       (1000)      179 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/invalid-pagespecs/expected-stderr.txt
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.737442 pspdfutils-3.0.7/tests/test-files/pstops/multiple-pages/
--rw-r-----   0 rrt       (1000) rrt       (1000)       23 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/multiple-pages/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2305 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/multiple-pages/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20065 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/multiple-pages/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.741442 pspdfutils-3.0.7/tests/test-files/pstops/multiple-turns-and-flips/
--rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/multiple-turns-and-flips/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     1759 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/multiple-turns-and-flips/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19517 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/multiple-turns-and-flips/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.741442 pspdfutils-3.0.7/tests/test-files/pstops/negative-offsets/
--rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/negative-offsets/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     1669 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/negative-offsets/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19485 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/negative-offsets/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.741442 pspdfutils-3.0.7/tests/test-files/pstops/offsets/
--rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/offsets/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     1667 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/offsets/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19483 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/offsets/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 18:16:36.741442 pspdfutils-3.0.7/tests/test-files/pstops/texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       53 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     7735 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    26045 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/pstops/texlive/expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)    78599 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test-files/tiger.eps
--rw-r-----   0 rrt       (1000) rrt       (1000)     1646 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test_epsffit.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1382 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test_extractres.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1082 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test_includeres.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      786 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test_psbook.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      957 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test_psjoin.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     3321 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test_psnup.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      816 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test_psresize.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1657 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test_psselect.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1427 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/test_pstops.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     6952 2023-06-22 20:34:06.000000 pspdfutils-3.0.7/tests/testutils.py
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.785449 pspdfutils-3.0.8/
+-rw-r-----   0 rrt       (1000) rrt       (1000)    35148 2020-01-25 13:35:25.000000 pspdfutils-3.0.8/COPYING
+-rw-r-----   0 rrt       (1000) rrt       (1000)      387 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/MANIFEST.in
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2935 2023-07-21 19:46:52.785449 pspdfutils-3.0.8/PKG-INFO
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2536 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/README.md
+-rw-r-----   0 rrt       (1000) rrt       (1000)       73 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/epsffit-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      686 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/extractres-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      620 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/includeres-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      440 2020-01-25 13:35:25.000000 pspdfutils-3.0.8/man-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      866 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psbook-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      852 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psnup-include.man
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.641445 pspdfutils-3.0.8/pspdfutils.egg-info/
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2935 2023-07-21 19:46:52.000000 pspdfutils-3.0.8/pspdfutils.egg-info/PKG-INFO
+-rw-r-----   0 rrt       (1000) rrt       (1000)    14540 2023-07-21 19:46:52.000000 pspdfutils-3.0.8/pspdfutils.egg-info/SOURCES.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        1 2023-07-21 19:46:52.000000 pspdfutils-3.0.8/pspdfutils.egg-info/dependency_links.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)      405 2023-07-21 19:46:52.000000 pspdfutils-3.0.8/pspdfutils.egg-info/entry_points.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)       24 2023-07-21 19:46:52.000000 pspdfutils-3.0.8/pspdfutils.egg-info/requires.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        8 2023-07-21 19:46:52.000000 pspdfutils-3.0.8/pspdfutils.egg-info/top_level.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)      298 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psresize-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)       68 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psselect-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3224 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/pstops-include.man
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.645445 pspdfutils-3.0.8/psutils/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      228 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/__init__.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     8381 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/argparse.py
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.649445 pspdfutils-3.0.8/psutils/command/
+-rw-r-----   0 rrt       (1000) rrt       (1000)     5829 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/command/epsffit.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4229 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/command/extractres.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1917 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/command/includeres.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2872 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/command/psbook.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9503 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/command/psjoin.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10324 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/command/psnup.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2173 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/command/psresize.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2685 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/command/psselect.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3160 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/command/pstops.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1382 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/io.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1338 2023-07-21 08:35:17.000000 pspdfutils-3.0.8/psutils/libpaper.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      980 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/psresources.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     5044 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/readers.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19306 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/transformers.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1930 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/types.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      913 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils/warnings.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      931 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/psutils.1
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2809 2023-07-21 19:44:49.000000 pspdfutils-3.0.8/pyproject.toml
+-rw-r-----   0 rrt       (1000) rrt       (1000)       38 2023-07-21 19:46:52.785449 pspdfutils-3.0.8/setup.cfg
+-rw-r-----   0 rrt       (1000) rrt       (1000)      539 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/setup.py
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.649445 pspdfutils-3.0.8/tests/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      890 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/conftest.py
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.657445 pspdfutils-3.0.8/tests/test-files/
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13275 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a3-20.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23046 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a3-20.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3332 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-1.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17476 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-1.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9028 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-11.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20384 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-11.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3910 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-2.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17766 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-2.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13208 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-20.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23021 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-20.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4539 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-3.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18056 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-3.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     5005 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-4-0.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18320 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a4-4-0.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3335 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a5-1.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17475 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a5-1.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13277 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a5-20.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23020 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/a5-20.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.541442 pspdfutils-3.0.8/tests/test-files/epsffit/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.657445 pspdfutils-3.0.8/tests/test-files/epsffit/aspect/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.665446 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.669446 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-maximize/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-maximize/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-maximize/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.669446 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-maximize-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-maximize-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-maximize-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.673446 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.673446 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-maximize/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-maximize/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-maximize/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.673446 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-maximize-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-maximize-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-maximize-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.677446 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/aspect-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.677446 pspdfutils-3.0.8/tests/test-files/epsffit/center/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/center/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78699 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/center/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.677446 pspdfutils-3.0.8/tests/test-files/epsffit/center-maximize/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/center-maximize/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78699 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/center-maximize/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.677446 pspdfutils-3.0.8/tests/test-files/epsffit/center-maximize-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/center-maximize-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78710 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/center-maximize-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.681446 pspdfutils-3.0.8/tests/test-files/epsffit/center-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/center-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78710 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/center-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.681446 pspdfutils-3.0.8/tests/test-files/epsffit/h-texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/h-texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4432 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/h-texlive/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.681446 pspdfutils-3.0.8/tests/test-files/epsffit/m-texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/m-texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4441 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/m-texlive/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.681446 pspdfutils-3.0.8/tests/test-files/epsffit/maximize/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/maximize/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/maximize/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.681446 pspdfutils-3.0.8/tests/test-files/epsffit/maximize-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/maximize-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/maximize-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.685446 pspdfutils-3.0.8/tests/test-files/epsffit/no-options/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/no-options/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/no-options/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.685446 pspdfutils-3.0.8/tests/test-files/epsffit/rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.685446 pspdfutils-3.0.8/tests/test-files/epsffit/showpage/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/showpage/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78725 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/showpage/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.685446 pspdfutils-3.0.8/tests/test-files/epsffit/v-texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/v-texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4433 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/epsffit/v-texlive/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.541442 pspdfutils-3.0.8/tests/test-files/extractres/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.689446 pspdfutils-3.0.8/tests/test-files/extractres/sample/
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/ISO-8859-1Encoding-expected.enc
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/ISO-8859-1Encoding.enc
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02-expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01-expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11851 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)      256 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/includeres-expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17478 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/extractres/sample/includeres-expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.541442 pspdfutils-3.0.8/tests/test-files/includeres/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.701447 pspdfutils-3.0.8/tests/test-files/includeres/sample/
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/includeres/sample/ISO-8859-1Encoding.enc
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/includeres/sample/a2ps-a2ps-hdr2.02.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/includeres/sample/a2ps-black+white-Prolog2.01.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)      280 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/includeres/sample/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17476 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/includeres/sample/expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4334 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/plot.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.549442 pspdfutils-3.0.8/tests/test-files/psbook/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.705447 pspdfutils-3.0.8/tests/test-files/psbook/20/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/20/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/20/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/20/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.705447 pspdfutils-3.0.8/tests/test-files/psbook/20-signature-4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/20-signature-4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/20-signature-4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/20-signature-4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.709447 pspdfutils-3.0.8/tests/test-files/psbook/3/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       31 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/3/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2867 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/3/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18081 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/3/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.709447 pspdfutils-3.0.8/tests/test-files/psbook/3-signature-4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       31 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/3-signature-4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2867 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/3-signature-4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18081 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/3-signature-4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.709447 pspdfutils-3.0.8/tests/test-files/psbook/invalid-signature-size/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       43 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/invalid-signature-size/expected-stderr.txt
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.709447 pspdfutils-3.0.8/tests/test-files/psbook/texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       66 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     7167 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20410 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psbook/texlive/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.549442 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.713447 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19350 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.713447 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-even/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-even/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3169 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-even/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19502 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-even/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.713447 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-nostrip/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-nostrip/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-nostrip/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    35545 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-nostrip/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.713447 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-save/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-save/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-save/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19474 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-save/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.577443 pspdfutils-3.0.8/tests/test-files/psnup/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.717447 pspdfutils-3.0.8/tests/test-files/psnup/20-1/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.717447 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flip/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flip/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    14844 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flip/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30718 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flip/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.717447 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    16124 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31098 2023-07-21 19:41:58.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.717447 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    14184 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-07-21 19:41:58.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.721447 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13964 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30858 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.737448 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    14144 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.737448 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11029 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.741448 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    14144 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.741448 pspdfutils-3.0.8/tests/test-files/psnup/20-2/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       87 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-2/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17430 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-2/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31268 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-2/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.741448 pspdfutils-3.0.8/tests/test-files/psnup/20-2-inpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       87 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-2-inpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    16450 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-2-inpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30887 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-2-inpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.741448 pspdfutils-3.0.8/tests/test-files/psnup/20-3/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20703 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.741448 pspdfutils-3.0.8/tests/test-files/psnup/20-3-impossible-tolerance/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       46 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-impossible-tolerance/expected-stderr.txt
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.745448 pspdfutils-3.0.8/tests/test-files/psnup/20-3-inpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-inpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20274 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-inpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31678 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-inpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.745448 pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedleft/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedleft/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20703 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedleft/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedleft/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.749448 pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedright/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedright/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20913 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedright/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedright/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.749448 pspdfutils-3.0.8/tests/test-files/psnup/20-4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19724 2023-07-21 19:41:59.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30986 2023-07-21 19:41:57.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.749448 pspdfutils-3.0.8/tests/test-files/psnup/20-4-297mmx210mm/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-297mmx210mm/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    24919 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-297mmx210mm/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31346 2023-07-21 19:41:58.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-297mmx210mm/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.753448 pspdfutils-3.0.8/tests/test-files/psnup/20-4-border-20/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-border-20/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20944 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-border-20/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31146 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-border-20/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.753448 pspdfutils-3.0.8/tests/test-files/psnup/20-4-columnmajor/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-columnmajor/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19714 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-columnmajor/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30986 2023-07-21 19:41:58.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-columnmajor/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.753448 pspdfutils-3.0.8/tests/test-files/psnup/20-4-flip/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-flip/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    22879 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-flip/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31346 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-flip/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.753448 pspdfutils-3.0.8/tests/test-files/psnup/20-4-impossible-border/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       28 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-impossible-border/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-impossible-border/expected.pdf
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.757448 pspdfutils-3.0.8/tests/test-files/psnup/20-4-impossible-margin/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       28 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-impossible-margin/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-impossible-margin/expected.pdf
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.757448 pspdfutils-3.0.8/tests/test-files/psnup/20-4-inpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-inpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20924 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-inpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31125 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-inpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.757448 pspdfutils-3.0.8/tests/test-files/psnup/20-4-margin-10/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-margin-10/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20794 2023-07-21 19:42:00.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-margin-10/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31146 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/20-4-margin-10/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.757448 pspdfutils-3.0.8/tests/test-files/psnup/draw/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       25 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/draw/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     5238 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/draw/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    21521 2023-07-21 19:41:58.000000 pspdfutils-3.0.8/tests/test-files/psnup/draw/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.757448 pspdfutils-3.0.8/tests/test-files/psnup/texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       53 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10473 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    26045 2023-07-21 19:42:09.000000 pspdfutils-3.0.8/tests/test-files/psnup/texlive/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.761448 pspdfutils-3.0.8/tests/test-files/psnup/texlive2/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/texlive2/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    68462 2023-07-21 19:42:01.000000 pspdfutils-3.0.8/tests/test-files/psnup/texlive2/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30184 2023-07-21 19:41:58.000000 pspdfutils-3.0.8/tests/test-files/psnup/texlive2/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.585443 pspdfutils-3.0.8/tests/test-files/psresize/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.761448 pspdfutils-3.0.8/tests/test-files/psresize/20-A3/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A3/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    14364 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A3/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30860 2023-07-21 19:42:23.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A3/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.761448 pspdfutils-3.0.8/tests/test-files/psresize/20-A3in-A4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A3in-A4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13764 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A3in-A4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30901 2023-07-21 19:42:18.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A3in-A4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.761448 pspdfutils-3.0.8/tests/test-files/psresize/20-A4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:42:18.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-07-21 19:42:18.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-07-21 19:42:23.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.765448 pspdfutils-3.0.8/tests/test-files/psresize/20-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13964 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30858 2023-07-21 19:42:23.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.765448 pspdfutils-3.0.8/tests/test-files/psresize/20-A5in-A4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A5in-A4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    14144 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A5in-A4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-07-21 19:42:23.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-A5in-A4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.765448 pspdfutils-3.0.8/tests/test-files/psresize/20-Letter/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-Letter/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    14164 2023-07-21 19:42:19.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-Letter/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30878 2023-07-21 19:42:23.000000 pspdfutils-3.0.8/tests/test-files/psresize/20-Letter/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.617444 pspdfutils-3.0.8/tests/test-files/psselect/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.765448 pspdfutils-3.0.8/tests/test-files/psselect/even/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/even/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6613 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/even/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20103 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/even/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.769449 pspdfutils-3.0.8/tests/test-files/psselect/even-reverse/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/even-reverse/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6613 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/even-reverse/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20103 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/even-reverse/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.769449 pspdfutils-3.0.8/tests/test-files/psselect/individual-pages-and-dash-p/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       58 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/individual-pages-and-dash-p/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6608 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/individual-pages-and-dash-p/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20111 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/individual-pages-and-dash-p/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.769449 pspdfutils-3.0.8/tests/test-files/psselect/invalid-pagerange/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       69 2023-05-19 21:27:44.000000 pspdfutils-3.0.8/tests/test-files/psselect/invalid-pagerange/.bak.0.expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)       37 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/invalid-pagerange/expected-stderr.txt
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.769449 pspdfutils-3.0.8/tests/test-files/psselect/negative-range/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       40 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/negative-range/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4423 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/negative-range/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18649 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/negative-range/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.773449 pspdfutils-3.0.8/tests/test-files/psselect/odd/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       61 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/odd/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6609 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/odd/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20117 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/odd/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.773449 pspdfutils-3.0.8/tests/test-files/psselect/options-and-complex-pagerange/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       47 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/options-and-complex-pagerange/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     5295 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/options-and-complex-pagerange/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19243 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/options-and-complex-pagerange/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.773449 pspdfutils-3.0.8/tests/test-files/psselect/positive-negative-range/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       98 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/positive-negative-range/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10114 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/positive-negative-range/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    22455 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/positive-negative-range/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.773449 pspdfutils-3.0.8/tests/test-files/psselect/positive-range/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       35 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/positive-range/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4419 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/positive-range/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18655 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/positive-range/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.773449 pspdfutils-3.0.8/tests/test-files/psselect/psnup-texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       97 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/psnup-texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10113 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/psnup-texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    22453 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/psnup-texlive/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.777449 pspdfutils-3.0.8/tests/test-files/psselect/reverse/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/reverse/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/reverse/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/reverse/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.777449 pspdfutils-3.0.8/tests/test-files/psselect/texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       66 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     7048 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20410 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect/texlive/expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10113 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect-texlive-output.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    22453 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/psselect-texlive-output.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.625445 pspdfutils-3.0.8/tests/test-files/pstops/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.777449 pspdfutils-3.0.8/tests/test-files/pstops/correct-angles/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       21 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/correct-angles/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2564 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/correct-angles/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20081 2023-07-21 19:42:55.000000 pspdfutils-3.0.8/tests/test-files/pstops/correct-angles/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.777449 pspdfutils-3.0.8/tests/test-files/pstops/default-paper-size/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       21 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/default-paper-size/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2611 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/default-paper-size/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20120 2023-07-21 19:42:55.000000 pspdfutils-3.0.8/tests/test-files/pstops/default-paper-size/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.777449 pspdfutils-3.0.8/tests/test-files/pstops/invalid-pagespecs/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      179 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/invalid-pagespecs/expected-stderr.txt
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.781449 pspdfutils-3.0.8/tests/test-files/pstops/multiple-pages/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       23 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/multiple-pages/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2399 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/multiple-pages/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20065 2023-07-21 19:42:55.000000 pspdfutils-3.0.8/tests/test-files/pstops/multiple-pages/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.781449 pspdfutils-3.0.8/tests/test-files/pstops/multiple-turns-and-flips/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/multiple-turns-and-flips/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1806 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/multiple-turns-and-flips/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19517 2023-07-21 19:42:55.000000 pspdfutils-3.0.8/tests/test-files/pstops/multiple-turns-and-flips/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.781449 pspdfutils-3.0.8/tests/test-files/pstops/negative-offsets/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/negative-offsets/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1716 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/negative-offsets/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19485 2023-07-21 19:42:55.000000 pspdfutils-3.0.8/tests/test-files/pstops/negative-offsets/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.781449 pspdfutils-3.0.8/tests/test-files/pstops/offsets/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/offsets/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1714 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/offsets/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19483 2023-07-21 19:42:55.000000 pspdfutils-3.0.8/tests/test-files/pstops/offsets/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-07-21 19:46:52.785449 pspdfutils-3.0.8/tests/test-files/pstops/texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       53 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10498 2023-07-21 19:42:53.000000 pspdfutils-3.0.8/tests/test-files/pstops/texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    26045 2023-07-21 19:42:55.000000 pspdfutils-3.0.8/tests/test-files/pstops/texlive/expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78599 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test-files/tiger.eps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1646 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test_epsffit.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1382 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test_extractres.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1082 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test_includeres.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      786 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test_psbook.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      957 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test_psjoin.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3321 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test_psnup.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      816 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test_psresize.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1657 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test_psselect.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1427 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/test_pstops.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6952 2023-06-22 20:34:06.000000 pspdfutils-3.0.8/tests/testutils.py
```

### Comparing `pspdfutils-3.0.7/COPYING` & `pspdfutils-3.0.8/COPYING`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/PKG-INFO` & `pspdfutils-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspdfutils
-Version: 3.0.7
+Version: 3.0.8
 Summary: Manipulate PDF and PostScript documents
 Author-email: Reuben Thomas <rrt@sc3d.org>
 License: GPL v3 or later
 Project-URL: Homepage, https://github.com/rrthomas/psutils
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `pspdfutils-3.0.7/README.md` & `pspdfutils-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/extractres-include.man` & `pspdfutils-3.0.8/extractres-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/includeres-include.man` & `pspdfutils-3.0.8/includeres-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psbook-include.man` & `pspdfutils-3.0.8/psbook-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psnup-include.man` & `pspdfutils-3.0.8/psnup-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/pspdfutils.egg-info/PKG-INFO` & `pspdfutils-3.0.8/pspdfutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspdfutils
-Version: 3.0.7
+Version: 3.0.8
 Summary: Manipulate PDF and PostScript documents
 Author-email: Reuben Thomas <rrt@sc3d.org>
 License: GPL v3 or later
 Project-URL: Homepage, https://github.com/rrthomas/psutils
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `pspdfutils-3.0.7/pspdfutils.egg-info/SOURCES.txt` & `pspdfutils-3.0.8/pspdfutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/pstops-include.man` & `pspdfutils-3.0.8/pstops-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/argparse.py` & `pspdfutils-3.0.8/psutils/argparse.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/command/epsffit.py` & `pspdfutils-3.0.8/psutils/command/epsffit.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/command/extractres.py` & `pspdfutils-3.0.8/psutils/command/extractres.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/command/includeres.py` & `pspdfutils-3.0.8/psutils/command/includeres.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/command/psbook.py` & `pspdfutils-3.0.8/psutils/command/psbook.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/command/psjoin.py` & `pspdfutils-3.0.8/psutils/command/psjoin.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/command/psnup.py` & `pspdfutils-3.0.8/psutils/command/psnup.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/command/psresize.py` & `pspdfutils-3.0.8/psutils/command/psresize.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/command/psselect.py` & `pspdfutils-3.0.8/psutils/command/psselect.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/command/pstops.py` & `pspdfutils-3.0.8/psutils/command/pstops.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/io.py` & `pspdfutils-3.0.8/psutils/io.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/libpaper.py` & `pspdfutils-3.0.8/psutils/libpaper.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/psresources.py` & `pspdfutils-3.0.8/psutils/psresources.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/readers.py` & `pspdfutils-3.0.8/psutils/readers.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/transformers.py` & `pspdfutils-3.0.8/psutils/transformers.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/types.py` & `pspdfutils-3.0.8/psutils/types.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils/warnings.py` & `pspdfutils-3.0.8/psutils/warnings.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/psutils.1` & `pspdfutils-3.0.8/psutils.1`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/pyproject.toml` & `pspdfutils-3.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "pspdfutils"
-version = "3.0.7"
+version = "3.0.8"
 description = "Manipulate PDF and PostScript documents"
 license = {text = "GPL v3 or later"}
 authors = [
     {name = "Reuben Thomas", email = "rrt@sc3d.org"}
 ]
 readme = "README.md"
 urls = {Homepage = "https://github.com/rrthomas/psutils"}
 requires-python = ">= 3.9"
 dependencies = [
     "puremagic",
-    "pypdf >= 3.8.0, < 3.11.0",
+    "pypdf >= 3.12.0",
 ]
 classifiers = [
     "Environment :: Console",
     "Programming Language :: Python :: 3",
 ]
 
 [project.scripts]
@@ -30,15 +30,15 @@
 pstops = "psutils.command.pstops:pstops"
 
 [build-system]
 requires = [
     "argparse-manpage[setuptools] >= 4.2",
     "pytest-datafiles",
     "puremagic",
-    "pypdf >= 3.8.0",
+    "pypdf >= 3.12.0",
 ]
 
 [tool.build_manpages]
 manpages = [
     "epsffit.1:module=psutils.command.epsffit:function=get_parser:manual_title=User Command:include=epsffit-include.man",
     "extractres.1:module=psutils.command.extractres:function=get_parser:manual_title=User Commands:include=extractres-include.man",
     "includeres.1:module=psutils.command.includeres:function=get_parser:manual_title=User Commands:include=includeres-include.man",
```

### Comparing `pspdfutils-3.0.7/setup.py` & `pspdfutils-3.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/conftest.py` & `pspdfutils-3.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a3-20.pdf` & `pspdfutils-3.0.8/tests/test-files/a3-20.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a3-20.ps` & `pspdfutils-3.0.8/tests/test-files/a3-20.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-1.pdf` & `pspdfutils-3.0.8/tests/test-files/a4-1.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-1.ps` & `pspdfutils-3.0.8/tests/test-files/a4-1.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-11.pdf` & `pspdfutils-3.0.8/tests/test-files/a4-11.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-11.ps` & `pspdfutils-3.0.8/tests/test-files/a4-11.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-2.pdf` & `pspdfutils-3.0.8/tests/test-files/a4-2.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-2.ps` & `pspdfutils-3.0.8/tests/test-files/a4-2.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-20.pdf` & `pspdfutils-3.0.8/tests/test-files/a4-20.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-20.ps` & `pspdfutils-3.0.8/tests/test-files/a4-20.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-3.pdf` & `pspdfutils-3.0.8/tests/test-files/a4-3.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-3.ps` & `pspdfutils-3.0.8/tests/test-files/a4-3.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-4-0.pdf` & `pspdfutils-3.0.8/tests/test-files/a4-4-0.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a4-4-0.ps` & `pspdfutils-3.0.8/tests/test-files/a4-4-0.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a5-1.pdf` & `pspdfutils-3.0.8/tests/test-files/a5-1.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a5-1.ps` & `pspdfutils-3.0.8/tests/test-files/a5-1.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a5-20.pdf` & `pspdfutils-3.0.8/tests/test-files/a5-20.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/a5-20.ps` & `pspdfutils-3.0.8/tests/test-files/a5-20.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/aspect/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/aspect/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-maximize/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-maximize/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-maximize-rotate/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-maximize-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/aspect-center-rotate/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/aspect-center-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/aspect-maximize/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/aspect-maximize/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/aspect-maximize-rotate/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/aspect-maximize-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/aspect-rotate/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/aspect-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/center/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/center/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/center-maximize/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/center-maximize/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/center-maximize-rotate/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/center-maximize-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/center-rotate/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/center-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/h-texlive/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/h-texlive/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/m-texlive/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/m-texlive/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/maximize/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/maximize/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/maximize-rotate/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/maximize-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/no-options/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/no-options/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/rotate/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/showpage/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/showpage/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/epsffit/v-texlive/expected.eps` & `pspdfutils-3.0.8/tests/test-files/epsffit/v-texlive/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/extractres/sample/ISO-8859-1Encoding-expected.enc` & `pspdfutils-3.0.8/tests/test-files/extractres/sample/ISO-8859-1Encoding-expected.enc`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/extractres/sample/ISO-8859-1Encoding.enc` & `pspdfutils-3.0.8/tests/test-files/extractres/sample/ISO-8859-1Encoding.enc`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02-expected.ps` & `pspdfutils-3.0.8/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02-expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02.ps` & `pspdfutils-3.0.8/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01-expected.ps` & `pspdfutils-3.0.8/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01-expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01.ps` & `pspdfutils-3.0.8/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/extractres/sample/expected.ps` & `pspdfutils-3.0.8/tests/test-files/extractres/sample/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/extractres/sample/includeres-expected.ps` & `pspdfutils-3.0.8/tests/test-files/extractres/sample/includeres-expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/includeres/sample/ISO-8859-1Encoding.enc` & `pspdfutils-3.0.8/tests/test-files/includeres/sample/ISO-8859-1Encoding.enc`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/includeres/sample/a2ps-a2ps-hdr2.02.ps` & `pspdfutils-3.0.8/tests/test-files/includeres/sample/a2ps-a2ps-hdr2.02.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/includeres/sample/a2ps-black+white-Prolog2.01.ps` & `pspdfutils-3.0.8/tests/test-files/includeres/sample/a2ps-black+white-Prolog2.01.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/includeres/sample/expected.ps` & `pspdfutils-3.0.8/tests/test-files/includeres/sample/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/plot.eps` & `pspdfutils-3.0.8/tests/test-files/plot.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/20/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psbook/20/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/20/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psbook/20/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/20-signature-4/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psbook/20-signature-4/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/20-signature-4/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psbook/20-signature-4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/3/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psbook/3/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/3/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psbook/3/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/3-signature-4/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psbook/3-signature-4/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/3-signature-4/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psbook/3-signature-4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/texlive/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psbook/texlive/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psbook/texlive/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psbook/texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-even/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-even/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-even/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-even/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-nostrip/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-nostrip/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-nostrip/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-nostrip/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-save/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-save/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psjoin_to_file/1-2-save/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psjoin_to_file/1-2-save/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-flip/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-flip/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'12885'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'12885'*

 * *DEBUG:pdfminer.psparser:seek: 12885*

 * *DEBUG:pdfminer.psparser:nexttoken: (12885, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=12885, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 12889, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12890, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12895, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12915, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12935, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12955, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12975, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12995, b'0000000451 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 13015, b'0000000654 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 13035, b'0000000984 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 13055, b'0000002314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 13075, b'0000002691 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 13095, b'0000002848 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 13115, b'0000003226 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 13135, b'0000003384 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 13155, b'0000003762 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -69,15 +69,15 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JLPWVJ+Courier</literal></value>
@@ -172,14 +172,20 @@
 </dict>
 </props>
 <data size="326">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -198,31 +204,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>326</number></value>
 </dict>
 </props>
 <data size="326">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -241,31 +253,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>326</number></value>
 </dict>
 </props>
 <data size="326">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -284,31 +302,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>326</number></value>
 </dict>
 </props>
 <data size="326">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -327,31 +351,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>326</number></value>
 </dict>
 </props>
 <data size="326">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -370,31 +400,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>326</number></value>
 </dict>
 </props>
 <data size="326">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -413,31 +449,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>326</number></value>
 </dict>
 </props>
 <data size="326">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -456,31 +498,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>326</number></value>
 </dict>
 </props>
 <data size="326">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -499,31 +547,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>326</number></value>
 </dict>
 </props>
 <data size="326">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -542,31 +596,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -585,31 +645,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -628,31 +694,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -671,31 +743,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -714,31 +792,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -757,31 +841,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -800,31 +890,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -843,31 +939,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -886,31 +988,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -929,31 +1037,37 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -972,34 +1086,40 @@
 <number>0.0</number>
 <number>842</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>327</number></value>
 </dict>
 </props>
 <data size="327">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 842 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-flip/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-flip/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 12% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'14165'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'14165'*

 * *DEBUG:pdfminer.psparser:seek: 14165*

 * *DEBUG:pdfminer.psparser:nexttoken: (14165, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=14165, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 14169, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 14170, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 14175, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14195, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14215, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14235, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14255, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14275, b'0000000481 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14295, b'0000000684 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14315, b'0000001014 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14335, b'0000002344 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14355, b'0000002755 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14375, b'0000002942 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14395, b'0000003354 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14415, b'0000003542 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 14435, b'0000003954 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -69,15 +69,15 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JLPWVJ+Courier</literal></value>
@@ -172,14 +172,20 @@
 </dict>
 </props>
 <data size="360">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -198,31 +204,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>360</number></value>
 </dict>
 </props>
 <data size="360">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -241,31 +253,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>360</number></value>
 </dict>
 </props>
 <data size="360">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -284,31 +302,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>360</number></value>
 </dict>
 </props>
 <data size="360">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -327,31 +351,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>360</number></value>
 </dict>
 </props>
 <data size="360">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -370,31 +400,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>360</number></value>
 </dict>
 </props>
 <data size="360">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -413,31 +449,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>360</number></value>
 </dict>
 </props>
 <data size="360">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -456,31 +498,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>360</number></value>
 </dict>
 </props>
 <data size="360">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -499,31 +547,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>360</number></value>
 </dict>
 </props>
 <data size="360">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -542,31 +596,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -585,31 +645,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -628,31 +694,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -671,31 +743,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -714,31 +792,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -757,31 +841,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -800,31 +890,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -843,31 +939,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -886,31 +988,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -929,31 +1037,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -972,34 +1086,40 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>361</number></value>
 </dict>
 </props>
 <data size="361">q&#10;0.00000000000000006122431852083324 0.999869 -0.999869 0.00000000000000006122431852083324 841.88976400000001 0.176745 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'12225'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'12225'*

 * *DEBUG:pdfminer.psparser:seek: 12225*

 * *DEBUG:pdfminer.psparser:nexttoken: (12225, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=12225, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 12229, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12230, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12235, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12255, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12275, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12295, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12315, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12335, b'0000000481 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12355, b'0000000684 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12375, b'0000001014 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12395, b'0000002344 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12415, b'0000002658 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12435, b'0000002845 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12455, b'0000003160 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12475, b'0000003348 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12495, b'0000003663 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -69,15 +69,15 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JLPWVJ+Courier</literal></value>
@@ -172,14 +172,20 @@
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -198,31 +204,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>263</number></value>
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -241,31 +253,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>263</number></value>
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -284,31 +302,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>263</number></value>
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -327,31 +351,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>263</number></value>
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -370,31 +400,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>263</number></value>
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -413,31 +449,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>263</number></value>
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -456,31 +498,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>263</number></value>
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -499,31 +547,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>263</number></value>
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -542,31 +596,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -585,31 +645,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -628,31 +694,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -671,31 +743,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -714,31 +792,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -757,31 +841,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -800,31 +890,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -843,31 +939,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -886,31 +988,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -929,31 +1037,37 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -972,34 +1086,40 @@
 <number>0.0</number>
 <number>841.8897637795275</number>
 <number>595.275590551181</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 0.0 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'12005'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'12005'*

 * *DEBUG:pdfminer.psparser:seek: 12005*

 * *DEBUG:pdfminer.psparser:nexttoken: (12005, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=12005, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 12009, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12010, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12015, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12035, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12055, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12075, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12095, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12115, b'0000000451 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12135, b'0000000654 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12155, b'0000000984 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12175, b'0000002314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12195, b'0000002647 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12215, b'0000002804 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12235, b'0000003138 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12255, b'0000003296 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12275, b'0000003630 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -69,15 +69,15 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JLPWVJ+Courier</literal></value>
@@ -172,14 +172,20 @@
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -198,31 +204,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -241,31 +253,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -284,31 +302,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -327,31 +351,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -370,31 +400,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -413,31 +449,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -456,31 +498,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -499,31 +547,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -542,31 +596,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -585,31 +645,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -628,31 +694,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -671,31 +743,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -714,31 +792,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -757,31 +841,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -800,31 +890,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -843,31 +939,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -886,31 +988,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -929,31 +1037,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -972,34 +1086,40 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'12185'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'12185'*

 * *DEBUG:pdfminer.psparser:seek: 12185*

 * *DEBUG:pdfminer.psparser:nexttoken: (12185, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=12185, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 12189, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12190, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12195, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12215, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12235, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12255, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12275, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12295, b'0000000451 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12315, b'0000000654 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12335, b'0000000984 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12355, b'0000002314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12375, b'0000002656 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12395, b'0000002813 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12415, b'0000003156 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12435, b'0000003314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12455, b'0000003657 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -69,15 +69,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>QKBZFC+Courier</literal></value>
@@ -172,14 +172,20 @@
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -198,31 +204,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -241,31 +253,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -284,31 +302,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -327,31 +351,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -370,31 +400,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -413,31 +449,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -456,31 +498,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -499,31 +547,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -542,31 +596,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -585,31 +645,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -628,31 +694,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -671,31 +743,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -714,31 +792,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -757,31 +841,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -800,31 +890,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -843,31 +939,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -886,31 +988,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -929,31 +1037,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -972,34 +1086,40 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'12185'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'12185'*

 * *DEBUG:pdfminer.psparser:seek: 12185*

 * *DEBUG:pdfminer.psparser:nexttoken: (12185, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=12185, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 12189, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12190, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12195, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12215, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12235, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12255, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12275, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12295, b'0000000451 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12315, b'0000000654 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12335, b'0000000984 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12355, b'0000002314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12375, b'0000002656 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12395, b'0000002813 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12415, b'0000003156 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12435, b'0000003314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12455, b'0000003657 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -69,15 +69,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>QKBZFC+Courier</literal></value>
@@ -172,14 +172,20 @@
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -198,31 +204,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -241,31 +253,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -284,31 +302,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -327,31 +351,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -370,31 +400,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -413,31 +449,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -456,31 +498,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -499,31 +547,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>291</number></value>
 </dict>
 </props>
 <data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -542,31 +596,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -585,31 +645,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -628,31 +694,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -671,31 +743,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -714,31 +792,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -757,31 +841,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -800,31 +890,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -843,31 +939,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -886,31 +988,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -929,31 +1037,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -972,34 +1086,40 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>292</number></value>
 </dict>
 </props>
 <data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-2/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/texlive/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 7% similar despite different names*

#### pdftotext {} -

```diff
@@ -16,26 +16,8 @@
 
 9
 
 10
 
 11
 
-12
-
-13
-
-14
-
-15
-
-16
-
-17
-
-18
-
-19
-
-20
-
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-2/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-2/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-2-inpaper-A5/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-2-inpaper-A5/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 20% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'10695'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'10695'*

 * *DEBUG:pdfminer.psparser:seek: 10695*

 * *DEBUG:pdfminer.psparser:nexttoken: (10695, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=10695, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 10699, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 10700, b'0 27\n'*

 * *DEBUG:pdfminer.psparser:nextline: 10705, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10725, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10745, b'0000000137 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10765, b'0000000176 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10785, b'0000000225 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10805, b'0000000393 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10825, b'0000000596 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10845, b'0000000926 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10865, b'0000002256 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10885, b'0000002945 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10905, b'0000003114 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10925, b'0000003804 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10945, b'0000003974 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 10965, b'0000004664 00000 n \n'*

 * *[ truncated after 25 lines; 1160 ignored ]*

```diff
@@ -3,23 +3,23 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>10</number></value>
 <key>Kids</key>
 <value><list size="10">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
-<ref id="13" />
-<ref id="15" />
+<ref id="12" />
 <ref id="17" />
-<ref id="19" />
-<ref id="21" />
-<ref id="23" />
-<ref id="25" />
+<ref id="22" />
+<ref id="27" />
+<ref id="32" />
+<ref id="37" />
+<ref id="42" />
+<ref id="47" />
+<ref id="52" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -61,15 +61,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>QKBZFC+Courier</literal></value>
@@ -156,22 +156,53 @@
 </object>
 
 <object id="8">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>638</number></value>
+<value><number>315</number></value>
 </dict>
 </props>
-<data size="638">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="315">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="2">
+<ref id="10" />
+<ref id="11" />
+</list>
+</object>
+
+<object id="10">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>319</number></value>
+</dict>
+</props>
+<data size="319">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="11">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>319</number></value>
+</dict>
+</props>
+<data size="319">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="12">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -192,31 +223,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="14" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="13">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>638</number></value>
+<value><number>315</number></value>
 </dict>
 </props>
-<data size="638">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="315">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="14">
+<list size="2">
+<ref id="15" />
+<ref id="16" />
+</list>
+</object>
+
+<object id="15">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>319</number></value>
+</dict>
+</props>
+<data size="319">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="16">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>319</number></value>
+</dict>
+</props>
+<data size="319">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="17">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -237,31 +299,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="19" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="18">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>638</number></value>
+<value><number>315</number></value>
 </dict>
 </props>
-<data size="638">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="315">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="19">
+<list size="2">
+<ref id="20" />
+<ref id="21" />
+</list>
+</object>
+
+<object id="20">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>319</number></value>
+</dict>
+</props>
+<data size="319">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="21">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>319</number></value>
+</dict>
+</props>
+<data size="319">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -282,31 +375,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>638</number></value>
+<value><number>315</number></value>
 </dict>
 </props>
-<data size="638">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="315">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="24">
+<list size="2">
+<ref id="25" />
+<ref id="26" />
+</list>
+</object>
+
+<object id="25">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>319</number></value>
+</dict>
+</props>
+<data size="319">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="26">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>319</number></value>
+</dict>
+</props>
+<data size="319">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="27">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -327,31 +451,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="29" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="28">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>639</number></value>
+<value><number>315</number></value>
 </dict>
 </props>
-<data size="639">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="315">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="29">
+<list size="2">
+<ref id="30" />
+<ref id="31" />
+</list>
+</object>
+
+<object id="30">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>319</number></value>
+</dict>
+</props>
+<data size="319">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="31">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="32">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -372,31 +527,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="34" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="33">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>640</number></value>
+<value><number>316</number></value>
 </dict>
 </props>
-<data size="640">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="316">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="34">
+<list size="2">
+<ref id="35" />
+<ref id="36" />
+</list>
+</object>
+
+<object id="35">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="36">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -417,31 +603,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>640</number></value>
+<value><number>316</number></value>
 </dict>
 </props>
-<data size="640">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="316">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="39">
+<list size="2">
+<ref id="40" />
+<ref id="41" />
+</list>
+</object>
+
+<object id="40">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="41">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="42">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -462,31 +679,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="44" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="43">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>640</number></value>
+<value><number>316</number></value>
 </dict>
 </props>
-<data size="640">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="316">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="44">
+<list size="2">
+<ref id="45" />
+<ref id="46" />
+</list>
+</object>
+
+<object id="45">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="46">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="47">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -507,31 +755,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="49" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="48">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>640</number></value>
+<value><number>316</number></value>
 </dict>
 </props>
-<data size="640">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="316">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="49">
+<list size="2">
+<ref id="50" />
+<ref id="51" />
+</list>
+</object>
+
+<object id="50">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="51">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -552,34 +831,65 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="53">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>316</number></value>
+</dict>
+</props>
+<data size="316">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="54">
+<list size="2">
+<ref id="55" />
+<ref id="56" />
+</list>
+</object>
+
+<object id="55">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>640</number></value>
+<value><number>320</number></value>
 </dict>
 </props>
-<data size="640">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="320">q&#10;q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 0.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="56">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>320</number></value>
+</dict>
+</props>
+<data size="320">q&#10;0.00000000000000006123233995736766 1 -1 0.00000000000000006123233995736766 595 421.5 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>27</number></value>
+<value><number>57</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-2-inpaper-A5/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-2-inpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-3/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-3/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 27% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'11078'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'11078'*

 * *DEBUG:pdfminer.psparser:seek: 11078*

 * *DEBUG:pdfminer.psparser:nexttoken: (11078, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=11078, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 11082, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 11083, b'0 21\n'*

 * *DEBUG:pdfminer.psparser:nextline: 11088, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11108, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11128, b'0000000115 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11148, b'0000000154 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11168, b'0000000203 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11188, b'0000000383 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11208, b'0000000586 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11228, b'0000000916 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11248, b'0000002246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11268, b'0000003405 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11288, b'0000003586 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11308, b'0000004746 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11328, b'0000004928 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11348, b'0000006088 00000 n \n'*

 * *[ truncated after 25 lines; 905 ignored ]*

```diff
@@ -3,20 +3,20 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>7</number></value>
 <key>Kids</key>
 <value><list size="7">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
-<ref id="13" />
-<ref id="15" />
-<ref id="17" />
-<ref id="19" />
+<ref id="14" />
+<ref id="21" />
+<ref id="28" />
+<ref id="35" />
+<ref id="42" />
+<ref id="49" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -60,15 +60,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JLPWVJ+Courier</literal></value>
@@ -155,22 +155,77 @@
 </object>
 
 <object id="8">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1107</number></value>
+<value><number>355</number></value>
 </dict>
 </props>
-<data size="1107">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="355">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="2">
+<ref id="12" />
+<ref id="13" />
+</list>
+</object>
+
+<object id="10">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>359</number></value>
+</dict>
+</props>
+<data size="359">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="11">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="12">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>735</number></value>
+</dict>
+</props>
+<data size="735">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="13">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="14">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -193,31 +248,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="16" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="15">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1107</number></value>
+<value><number>355</number></value>
 </dict>
 </props>
-<data size="1107">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="355">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="16">
+<list size="2">
+<ref id="19" />
+<ref id="20" />
+</list>
+</object>
+
+<object id="17">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>359</number></value>
+</dict>
+</props>
+<data size="359">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="18">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="19">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>735</number></value>
+</dict>
+</props>
+<data size="735">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="20">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="21">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -240,31 +350,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="23" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="22">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1107</number></value>
+<value><number>355</number></value>
 </dict>
 </props>
-<data size="1107">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="355">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="23">
+<list size="2">
+<ref id="26" />
+<ref id="27" />
+</list>
+</object>
+
+<object id="24">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>359</number></value>
+</dict>
+</props>
+<data size="359">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="25">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="26">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>735</number></value>
+</dict>
+</props>
+<data size="735">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="27">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -287,31 +452,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1110</number></value>
+<value><number>356</number></value>
 </dict>
 </props>
-<data size="1110">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="356">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="30">
+<list size="2">
+<ref id="33" />
+<ref id="34" />
+</list>
+</object>
+
+<object id="31">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>360</number></value>
+</dict>
+</props>
+<data size="360">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="32">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="33">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>737</number></value>
+</dict>
+</props>
+<data size="737">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="34">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="35">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -334,31 +554,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="37" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="36">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1110</number></value>
+<value><number>356</number></value>
 </dict>
 </props>
-<data size="1110">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="356">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="37">
+<list size="2">
+<ref id="40" />
+<ref id="41" />
+</list>
+</object>
+
+<object id="38">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>360</number></value>
+</dict>
+</props>
+<data size="360">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="39">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="40">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>737</number></value>
+</dict>
+</props>
+<data size="737">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="41">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="42">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -381,31 +656,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="44" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="43">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1110</number></value>
+<value><number>356</number></value>
 </dict>
 </props>
-<data size="1110">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="356">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="44">
+<list size="2">
+<ref id="47" />
+<ref id="48" />
+</list>
+</object>
+
+<object id="45">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>360</number></value>
+</dict>
+</props>
+<data size="360">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="46">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="47">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>737</number></value>
+</dict>
+</props>
+<data size="737">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="48">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -426,34 +756,65 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="50">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>356</number></value>
+</dict>
+</props>
+<data size="356">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="51">
+<list size="2">
+<ref id="52" />
+<ref id="53" />
+</list>
+</object>
+
+<object id="52">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>360</number></value>
+</dict>
+</props>
+<data size="360">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>733</number></value>
+<value><number>373</number></value>
 </dict>
 </props>
-<data size="733">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>21</number></value>
+<value><number>54</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-3/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-3/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-3-inpaper-A5/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A5in-A4/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 25% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,41 +1,41 @@
 1
 
-2
+2
 
-3
+3
 
 4
 
-5
+5
 
-6
+6
 
 7
 
-8
+8
 
-9
+9
 
 10
 
-11
+11
 
-12
+12
 
 13
 
-14
+14
 
-15
+15
 
 16
 
-17
+17
 
-18
+18
 
 19
 
-20
+20
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-3-inpaper-A5/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-3-inpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedleft/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedleft/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 27% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'11078'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'11078'*

 * *DEBUG:pdfminer.psparser:seek: 11078*

 * *DEBUG:pdfminer.psparser:nexttoken: (11078, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=11078, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 11082, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 11083, b'0 21\n'*

 * *DEBUG:pdfminer.psparser:nextline: 11088, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11108, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11128, b'0000000115 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11148, b'0000000154 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11168, b'0000000203 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11188, b'0000000383 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11208, b'0000000586 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11228, b'0000000916 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11248, b'0000002246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11268, b'0000003405 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11288, b'0000003586 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11308, b'0000004746 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11328, b'0000004928 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11348, b'0000006088 00000 n \n'*

 * *[ truncated after 25 lines; 905 ignored ]*

```diff
@@ -3,20 +3,20 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>7</number></value>
 <key>Kids</key>
 <value><list size="7">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
-<ref id="13" />
-<ref id="15" />
-<ref id="17" />
-<ref id="19" />
+<ref id="14" />
+<ref id="21" />
+<ref id="28" />
+<ref id="35" />
+<ref id="42" />
+<ref id="49" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -60,15 +60,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JLPWVJ+Courier</literal></value>
@@ -155,22 +155,77 @@
 </object>
 
 <object id="8">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1107</number></value>
+<value><number>355</number></value>
 </dict>
 </props>
-<data size="1107">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="355">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="2">
+<ref id="12" />
+<ref id="13" />
+</list>
+</object>
+
+<object id="10">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>359</number></value>
+</dict>
+</props>
+<data size="359">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="11">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="12">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>735</number></value>
+</dict>
+</props>
+<data size="735">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="13">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="14">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -193,31 +248,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="16" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="15">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1107</number></value>
+<value><number>355</number></value>
 </dict>
 </props>
-<data size="1107">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="355">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="16">
+<list size="2">
+<ref id="19" />
+<ref id="20" />
+</list>
+</object>
+
+<object id="17">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>359</number></value>
+</dict>
+</props>
+<data size="359">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="18">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="19">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>735</number></value>
+</dict>
+</props>
+<data size="735">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="20">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="21">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -240,31 +350,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="23" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="22">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1107</number></value>
+<value><number>355</number></value>
 </dict>
 </props>
-<data size="1107">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="355">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="23">
+<list size="2">
+<ref id="26" />
+<ref id="27" />
+</list>
+</object>
+
+<object id="24">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>359</number></value>
+</dict>
+</props>
+<data size="359">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="25">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="26">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>735</number></value>
+</dict>
+</props>
+<data size="735">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="27">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>372</number></value>
+</dict>
+</props>
+<data size="372">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -287,31 +452,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1110</number></value>
+<value><number>356</number></value>
 </dict>
 </props>
-<data size="1110">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="356">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="30">
+<list size="2">
+<ref id="33" />
+<ref id="34" />
+</list>
+</object>
+
+<object id="31">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>360</number></value>
+</dict>
+</props>
+<data size="360">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="32">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="33">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>737</number></value>
+</dict>
+</props>
+<data size="737">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="34">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="35">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -334,31 +554,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="37" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="36">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1110</number></value>
+<value><number>356</number></value>
 </dict>
 </props>
-<data size="1110">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="356">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="37">
+<list size="2">
+<ref id="40" />
+<ref id="41" />
+</list>
+</object>
+
+<object id="38">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>360</number></value>
+</dict>
+</props>
+<data size="360">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="39">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="40">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>737</number></value>
+</dict>
+</props>
+<data size="737">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="41">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="42">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="3">
@@ -381,31 +656,86 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="44" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="43">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>1110</number></value>
+<value><number>356</number></value>
 </dict>
 </props>
-<data size="1110">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="356">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="44">
+<list size="2">
+<ref id="47" />
+<ref id="48" />
+</list>
+</object>
+
+<object id="45">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>360</number></value>
+</dict>
+</props>
+<data size="360">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="46">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="47">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>737</number></value>
+</dict>
+</props>
+<data size="737">q&#10;q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="48">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>373</number></value>
+</dict>
+</props>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 561.33333300000004 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-1 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -426,34 +756,65 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="50">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>356</number></value>
+</dict>
+</props>
+<data size="356">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="51">
+<list size="2">
+<ref id="52" />
+<ref id="53" />
+</list>
+</object>
+
+<object id="52">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>360</number></value>
+</dict>
+</props>
+<data size="360">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>733</number></value>
+<value><number>373</number></value>
 </dict>
 </props>
-<data size="733">q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="373">q&#10;0.00000000000000002888384584894994 0.471709 -0.471709 0.00000000000000002888384584894994 496.08935600000001 280.66666700000002 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>21</number></value>
+<value><number>54</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedleft/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedleft/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-3-rotatedright/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-3-rotatedright/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-4/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-4-297mmx210mm/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-4-297mmx210mm/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-4-border-20/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-4-border-20/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-4-columnmajor/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-4-columnmajor/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-4-flip/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-4-flip/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-4-inpaper-A5/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-4-inpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/20-4-margin-10/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/20-4-margin-10/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/draw/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/pstops/correct-angles/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 25% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,9 +1,5 @@
 1
 
-2
-
-3
-
-4
+1
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/draw/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/draw/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/texlive/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psnup/texlive2/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psnup/texlive2/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A3/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psresize/20-Letter/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 16% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'12405'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'12405'*

 * *DEBUG:pdfminer.psparser:seek: 12405*

 * *DEBUG:pdfminer.psparser:nexttoken: (12405, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=12405, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 12409, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12410, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12415, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12435, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12455, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12475, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12495, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12515, b'0000000452 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12535, b'0000000655 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12555, b'0000000985 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12575, b'0000002315 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12595, b'0000002667 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12615, b'0000002825 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12635, b'0000003178 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12655, b'0000003337 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12675, b'0000003690 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -63,21 +63,21 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JLPWVJ+Courier</literal></value>
@@ -164,22 +164,28 @@
 </object>
 
 <object id="8">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>301</number></value>
+<value><number>292</number></value>
 </dict>
 </props>
-<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="292">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -192,37 +198,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>301</number></value>
+<value><number>292</number></value>
 </dict>
 </props>
-<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="292">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -235,37 +247,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>301</number></value>
+<value><number>292</number></value>
 </dict>
 </props>
-<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="292">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -278,37 +296,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>301</number></value>
+<value><number>292</number></value>
 </dict>
 </props>
-<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="292">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -321,37 +345,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>301</number></value>
+<value><number>292</number></value>
 </dict>
 </props>
-<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="292">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -364,37 +394,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>301</number></value>
+<value><number>292</number></value>
 </dict>
 </props>
-<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="292">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -407,37 +443,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>301</number></value>
+<value><number>292</number></value>
 </dict>
 </props>
-<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="292">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -450,37 +492,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>301</number></value>
+<value><number>292</number></value>
 </dict>
 </props>
-<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="292">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -493,37 +541,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>301</number></value>
+<value><number>292</number></value>
 </dict>
 </props>
-<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="292">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -536,37 +590,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -579,37 +639,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -622,37 +688,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -665,37 +737,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -708,37 +786,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -751,37 +835,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -794,37 +884,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -837,37 +933,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -880,37 +982,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -923,37 +1031,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -966,40 +1080,46 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>842</number>
-<number>1191</number>
+<number>612</number>
+<number>792</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>302</number></value>
+<value><number>293</number></value>
 </dict>
 </props>
-<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="293">q&#10;0.940618 0.0 0.0 0.940618 26.166270999999998 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A3/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A3/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A3in-A4/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A3in-A4/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 22% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'11805'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'11805'*

 * *DEBUG:pdfminer.psparser:seek: 11805*

 * *DEBUG:pdfminer.psparser:nexttoken: (11805, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=11805, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 11809, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 11810, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 11815, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11835, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11855, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11875, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11895, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11915, b'0000000451 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11935, b'0000000654 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11955, b'0000000984 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11975, b'0000002314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 11995, b'0000002637 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12015, b'0000002794 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12035, b'0000003118 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12055, b'0000003276 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12075, b'0000003600 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -69,15 +69,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>QKBZFC+Courier</literal></value>
@@ -172,14 +172,20 @@
 </dict>
 </props>
 <data size="272">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -198,31 +204,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>272</number></value>
 </dict>
 </props>
 <data size="272">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -241,31 +253,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>272</number></value>
 </dict>
 </props>
 <data size="272">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -284,31 +302,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>272</number></value>
 </dict>
 </props>
 <data size="272">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -327,31 +351,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>272</number></value>
 </dict>
 </props>
 <data size="272">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -370,31 +400,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>272</number></value>
 </dict>
 </props>
 <data size="272">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -413,31 +449,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>272</number></value>
 </dict>
 </props>
 <data size="272">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -456,31 +498,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>272</number></value>
 </dict>
 </props>
 <data size="272">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -499,31 +547,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>272</number></value>
 </dict>
 </props>
 <data size="272">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -542,31 +596,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -585,31 +645,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -628,31 +694,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -671,31 +743,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -714,31 +792,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -757,31 +841,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -800,31 +890,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -843,31 +939,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -886,31 +988,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -929,31 +1037,37 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -972,34 +1086,40 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>273</number></value>
 </dict>
 </props>
 <data size="273">q&#10;0.706651 0.0 0.0 0.706651 0.0 0.18943 cm&#10;0.0 0.0 842 1191 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 242.97900000000001 Tf&#10;1 0 0 1 126.051 923.02099999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 7872.5100000000002 11420 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A3in-A4/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A3in-A4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A4/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A4/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A4/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A5/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A5/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'12005'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'12005'*

 * *DEBUG:pdfminer.psparser:seek: 12005*

 * *DEBUG:pdfminer.psparser:nexttoken: (12005, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=12005, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 12009, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12010, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12015, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12035, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12055, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12075, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12095, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12115, b'0000000451 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12135, b'0000000654 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12155, b'0000000984 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12175, b'0000002314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12195, b'0000002647 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12215, b'0000002804 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12235, b'0000003138 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12255, b'0000003296 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12275, b'0000003630 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -69,15 +69,15 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JLPWVJ+Courier</literal></value>
@@ -172,14 +172,20 @@
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -198,31 +204,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -241,31 +253,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -284,31 +302,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -327,31 +351,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -370,31 +400,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -413,31 +449,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -456,31 +498,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -499,31 +547,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>282</number></value>
 </dict>
 </props>
 <data size="282">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -542,31 +596,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -585,31 +645,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -628,31 +694,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -671,31 +743,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -714,31 +792,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -757,31 +841,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -800,31 +890,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -843,31 +939,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -886,31 +988,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -929,31 +1037,37 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -972,34 +1086,40 @@
 <number>0.0</number>
 <number>420</number>
 <number>595</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>283</number></value>
 </dict>
 </props>
 <data size="283">q&#10;0.705882 0.0 0.0 0.705882 0.0 0.323529 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A5/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A5in-A4/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A3/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 15% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'12185'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'12185'*

 * *DEBUG:pdfminer.psparser:seek: 12185*

 * *DEBUG:pdfminer.psparser:nexttoken: (12185, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=12185, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 12189, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12190, b'0 47\n'*

 * *DEBUG:pdfminer.psparser:nextline: 12195, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12215, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12235, b'0000000207 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12255, b'0000000246 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12275, b'0000000295 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12295, b'0000000451 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12315, b'0000000654 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12335, b'0000000984 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12355, b'0000002314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12375, b'0000002656 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12395, b'0000002813 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12415, b'0000003156 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12435, b'0000003314 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 12455, b'0000003657 00000 n \n'*

 * *[ truncated after 25 lines; 2010 ignored ]*

```diff
@@ -3,33 +3,33 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>20</number></value>
 <key>Kids</key>
 <value><list size="20">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
+<ref id="10" />
 <ref id="13" />
-<ref id="15" />
-<ref id="17" />
+<ref id="16" />
 <ref id="19" />
-<ref id="21" />
-<ref id="23" />
+<ref id="22" />
 <ref id="25" />
-<ref id="27" />
-<ref id="29" />
+<ref id="28" />
 <ref id="31" />
-<ref id="33" />
-<ref id="35" />
+<ref id="34" />
 <ref id="37" />
-<ref id="39" />
-<ref id="41" />
+<ref id="40" />
 <ref id="43" />
-<ref id="45" />
+<ref id="46" />
+<ref id="49" />
+<ref id="52" />
+<ref id="55" />
+<ref id="58" />
+<ref id="61" />
+<ref id="64" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -63,28 +63,28 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
-<value><literal>QKBZFC+Courier</literal></value>
+<value><literal>JLPWVJ+Courier</literal></value>
 <key>FontDescriptor</key>
 <value><ref id="6" /></value>
 <key>Type</key>
 <value><literal>Font</literal></value>
 <key>FirstChar</key>
 <value><number>48</number></value>
 <key>LastChar</key>
@@ -110,15 +110,15 @@
 </object>
 
 <object id="6">
 <dict size="14">
 <key>Type</key>
 <value><literal>FontDescriptor</literal></value>
 <key>FontName</key>
-<value><literal>QKBZFC+Courier</literal></value>
+<value><literal>JLPWVJ+Courier</literal></value>
 <key>FontBBox</key>
 <value><list size="4">
 <number>0</number>
 <number>-15</number>
 <number>516</number>
 <number>616</number>
 </list></value>
@@ -155,31 +155,37 @@
 <value><literal>FlateDecode</literal></value>
 <key>Subtype</key>
 <value><literal>Type1C</literal></value>
 <key>Length</key>
 <value><number>1240</number></value>
 </dict>
 </props>
-<data size="1366">&#1;&#0;&#4;&#2;&#0;&#1;&#1;&#1;&#8;Courier&#0;&#1;&#1;&#1;,&#248;&#27;&#1;&#248;&#28;&#2;&#248;&#29;&#3;&#139;|&#248;&#152;&#248;&#252;&#5;&#248;&#30;&#12;&#0;&#140;&#12;&#1;&#139;&#12;&#3;&#139;&#12;&#4;&#162;&#28;&#5;=&#18;&#247;&#153;&#17;&#247;&#132;&#15;&#247;x&#16;&#0;&#4;&#1;&#1;7M[&#155;&#40;URW&#41;++,Copyright 2014 by &#40;URW&#41;++ Design &#38; DevelopmentNimbus Mono PS RegularNimbus Mono PSCopyright &#40;URW&#41;++,Copyright 2014 by &#40;URW&#41;++ Design &#38; Development&#0;&#0;&#0;&#10;3456789012&#0;&#0;&#20;&#0;&#21;&#0;&#22;&#0;&#23;&#0;&#24;&#0;&#25;&#0;&#26;&#0;&#17;&#0;&#18;&#0;&#19;&#0;&#11;&#2;&#0;&#1;&#0;&#4;&#0;&#146;&#0;&#229;&#1;V&#1;&#215;&#2;&#17;&#2;&#135;&#3;&#8;&#3;u&#3;&#185;&#4;&#30;&#248;&#236;&#14;&#248;&#236;|&#190;&#248;&#165;&#190;&#18;&#248;C&#191;l&#191;&#23;&#19;&#208;&#247;&#171;&#247;&#249;&#21;v&#128;&#129;{{&#150;&#130;&#160;&#31;&#235;&#137;&#216;O&#139;@&#8;CBN3SX&#157;&#174;[&#30;&#130;&#145;&#134;&#141;&#132;&#139;&#8;~&#128;&#128;~{&#152;~&#175;y&#31;&#191;o&#186;~&#190;&#139;&#8;&#247;&#10;&#235;&#222;&#240;&#204;]&#201;E&#170;&#31;&#19;&#224;&#200;&#168;&#173;&#186;&#195;&#26;&#228;&#60;&#207;$VX{mc&#30;ty}z&#139;&#127;&#8;~&#150;&#128;&#153;&#147;&#145;&#142;&#145;&#144;&#30;&#175;&#179;&#180;&#156;&#199;&#139;&#8;&#213;&#195;]Okylnx&#31;s|w&#134;d&#139;&#8;&#14;&#248;&#236;&#139;&#190;&#247;&#7;&#190;&#1;&#248;&#7;&#191;&#3;&#248;&#7;&#247;:&#21;&#251;&#7;D&#7;v&#128;&#130;{z&#151;&#130;&#159;&#31;&#247;,&#6;&#159;&#151;&#148;&#156;&#155;&#128;&#148;v&#31;n&#247;&#7;&#168;&#6;&#160;&#150;&#148;&#156;&#155;&#128;&#148;v&#31;n&#248;&#22;.&#6;&#251;z&#252;&#20;&#5;V&#7;&#247;&#163;&#190;&#21;&#251;m&#6;&#247;^&#247;&#227;&#5;&#154;&#6;&#14;&#248;&#236;|&#190;&#247;&#203;&#190;&#247;.&#190;&#1;&#247;$&#191;&#247;&#149;&#191;&#3;&#247;X&#248;&#188;&#21;&#247;&#128;&#6;&#161;&#150;&#148;&#156;&#155;&#128;&#148;u&#31;&#251;&#180;&#251;&#161;&#6;{&#149;&#128;&#154;&#145;&#144;&#141;&#145;&#152;&#30;&#183;&#161;&#179;&#149;&#179;&#139;&#8;&#220;&#194;Q6&#39;JG,SW&#161;&#182;[&#31;&#130;&#147;&#134;&#141;&#132;&#139;&#8;}&#128;&#128;}|&#153;|&#174;u&#31;&#190;j&#189;{&#193;&#139;&#8;&#247;&#15;&#226;&#229;&#247;&#19;&#247;&#6;&#62;&#221;!`i&#131;xZ&#31;&#14;&#248;&#236;|&#190;&#247;&#172;&#190;&#247;Z&#190;&#1;&#247;&#23;&#189;&#247;&#175;&#191;&#3;&#247;J&#247;&#154;&#21;&#138;&#149;&#139;&#148;&#139;&#144;&#139;&#199;&#155;&#199;&#168;&#181;&#187;&#211;&#216;&#184;&#214;&#139;&#157;&#139;&#154;&#137;&#149;&#134;&#149;&#134;&#143;&#138;&#145;&#139;&#8;&#153;&#149;&#150;&#152;&#162;f&#156;ZJIr]U&#31;@Lg6&#139;&#251;&#9;&#8;&#251;A&#224;&#251;&#14;&#247;&#14;&#239;&#217;&#224;&#247;&#1;&#242;=&#224;,IPeHg&#30;&#146;B&#21;&#162;&#179;&#150;&#156;&#153;&#155;&#171;&#174;&#177;&#158;&#175;&#139;&#8;&#205;&#194;M@:UMD@[&#187;&#244;p&#31;&#14;&#248;&#236;&#138;&#159;&#248;&#169;&#190;&#1;&#248;E&#248;&#176;&#21;&#251;4&#252;&#138;&#137;&#133;&#138;&#135;&#139;&#135;&#25;}&#150;&#128;&#153;&#153;&#145;&#145;&#157;&#145;&#30;&#247;7&#248;&#146;&#5;&#209;&#252;&#20;;&#7;u&#148;&#128;&#156;&#156;&#148;&#150;&#161;&#30;&#168;&#247;&#173;&#7;&#14;&#248;&#236;|&#190;&#247;&#143;&#189;&#247;x&#190;&#18;&#247;&#0;&#191;a&#191;&#247;&#152;&#191;b&#191;&#23;&#19;&#236;&#248;&#24;&#247;&#204;&#21;&#202;&#172;&#170;&#185;&#139;&#197;&#8;&#230;8&#215;&#40;&#40;8?0Q&#171;]&#202;j&#30;&#19;&#242;HkeUL&#26;&#41;&#225;;&#246;&#245;&#225;&#219;&#237;&#202;d&#194;I&#170;&#30;&#19;&#236;1&#247;&#145;&#21;&#213;&#197;WIMR[BBR&#187;&#201;&#204;&#197;&#192;&#209;&#31;&#19;&#242;&#251;&#170;&#4;&#221;&#200;VDDMS=&#60;M&#195;&#210;&#208;&#200;&#194;&#216;&#31;&#14;&#248;&#236;|&#190;&#247;Z&#190;&#247;&#172;&#190;&#1;&#247;&#23;&#191;&#247;&#175;&#189;&#3;&#248;e&#247;&#231;&#21;&#140;&#129;&#139;&#130;&#139;&#135;&#139;N{Ona[C&#62;^@&#139;y&#139;|&#142;&#129;&#144;&#129;&#144;&#135;&#140;&#133;&#139;&#8;}&#129;&#128;}t&#175;z&#189;&#204;&#205;&#164;&#185;&#193;&#31;&#214;&#202;&#175;&#224;&#139;&#247;&#8;&#8;&#247;B6&#247;&#14;&#251;&#14;&#39;=6&#251;&#1;$&#217;6&#234;&#205;&#197;&#177;&#206;&#176;&#30;&#132;&#212;&#21;tc&#128;z|{liewg&#139;&#8;IT&#201;&#214;&#220;&#193;&#201;&#210;&#214;&#186;[&#34;&#167;&#31;&#14;&#248;&#236;|&#190;&#248;&#165;&#190;&#1;&#247;&#0;&#191;&#247;&#173;&#191;&#3;&#248;&#129;&#247;&#242;&#21;&#247;2=&#247;&#0;&#251;&#6;&#251;&#7;=&#251;&#0;&#251;2&#30;&#41;&#7;&#251;3&#217;&#251;&#0;&#247;&#7;&#247;&#6;&#217;&#247;&#0;&#247;3&#30;&#251;&#225;&#231;&#21;&#139;&#201;&#157;&#204;&#168;&#184;&#160;&#171;&#171;&#156;&#180;&#139;&#179;&#139;&#171;z&#160;k&#168;^&#157;J&#139;M&#8;4&#7;&#139;NyIn^vkjzd&#139;c&#139;j&#156;v&#171;n&#184;y&#205;&#139;&#200;&#8;&#14;&#248;&#236;&#139;&#190;&#1;&#247;&#167;&#191;&#3;&#247;&#219;&#248;&#249;&#21;&#251;TOx&#133;&#133;&#133;&#139;}&#25;~&#151;&#127;&#151;&#141;&#149;&#141;&#140;&#143;&#30;&#247;&#17;&#178;&#5;&#252;&#129;&#251;&#26;&#7;u&#128;&#130;{z&#151;&#130;&#160;&#31;&#247;&#212;&#6;&#160;&#150;&#148;&#156;&#155;&#128;&#148;v&#31;&#251;&#26;&#6;&#14;&#248;&#236;&#139;&#190;&#248;&#150;&#190;&#1;&#248;@&#191;&#3;&#247;&#27;&#190;&#21;&#193;&#185;&#201;&#196;&#222;&#219;&#247;&#18;&#247;&#12;&#159;&#168;&#139;&#198;&#8;&#232;2&#220;&#38;MQo[e&#30;wr~m&#139;x&#8;&#127;&#150;&#128;&#153;&#152;&#147;&#146;&#155;&#143;&#30;&#156;&#197;&#198;&#180;&#204;&#139;&#8;&#213;&#203;RJ`yr.1&#31;8&#60;?EEN&#130;&#131;&#24;H&#248;&#41;&#220;&#7;&#160;&#130;&#150;zz&#130;&#128;v&#30;m&#7;&#14;{&#155;&#248;5&#155;&#247;&#22;&#151;&#167;&#152;&#6;&#191;&#10;&#190;&#11;&#182;&#148;&#12;&#12;&#182;&#147;&#12;&#13;&#0;&#0;</data>
+<data size="1366">&#1;&#0;&#4;&#2;&#0;&#1;&#1;&#1;&#8;Courier&#0;&#1;&#1;&#1;,&#248;&#27;&#1;&#248;&#28;&#2;&#248;&#29;&#3;&#139;|&#248;&#152;&#248;&#252;&#5;&#248;&#30;&#12;&#0;&#140;&#12;&#1;&#139;&#12;&#3;&#139;&#12;&#4;&#162;&#28;&#5;=&#18;&#247;&#153;&#17;&#247;&#132;&#15;&#247;x&#16;&#0;&#4;&#1;&#1;7M[&#155;&#40;URW&#41;++,Copyright 2014 by &#40;URW&#41;++ Design &#38; DevelopmentNimbus Mono PS RegularNimbus Mono PSCopyright &#40;URW&#41;++,Copyright 2014 by &#40;URW&#41;++ Design &#38; Development&#0;&#0;&#0;&#10;4567890123&#0;&#0;&#21;&#0;&#22;&#0;&#23;&#0;&#24;&#0;&#25;&#0;&#26;&#0;&#17;&#0;&#18;&#0;&#19;&#0;&#20;&#0;&#11;&#2;&#0;&#1;&#0;&#4;&#0;W&#0;&#200;&#1;I&#1;&#131;&#1;&#249;&#2;z&#2;&#231;&#3;+&#3;&#144;&#4;&#30;&#248;&#236;&#14;&#248;&#236;&#139;&#190;&#247;&#7;&#190;&#1;&#248;&#7;&#191;&#3;&#248;&#7;&#247;:&#21;&#251;&#7;D&#7;v&#128;&#130;{z&#151;&#130;&#159;&#31;&#247;,&#6;&#159;&#151;&#148;&#156;&#155;&#128;&#148;v&#31;n&#247;&#7;&#168;&#6;&#160;&#150;&#148;&#156;&#155;&#128;&#148;v&#31;n&#248;&#22;.&#6;&#251;z&#252;&#20;&#5;V&#7;&#247;&#163;&#190;&#21;&#251;m&#6;&#247;^&#247;&#227;&#5;&#154;&#6;&#14;&#248;&#236;|&#190;&#247;&#203;&#190;&#247;.&#190;&#1;&#247;$&#191;&#247;&#149;&#191;&#3;&#247;X&#248;&#188;&#21;&#247;&#128;&#6;&#161;&#150;&#148;&#156;&#155;&#128;&#148;u&#31;&#251;&#180;&#251;&#161;&#6;{&#149;&#128;&#154;&#145;&#144;&#141;&#145;&#152;&#30;&#183;&#161;&#179;&#149;&#179;&#139;&#8;&#220;&#194;Q6&#39;JG,SW&#161;&#182;[&#31;&#130;&#147;&#134;&#141;&#132;&#139;&#8;}&#128;&#128;}|&#153;|&#174;u&#31;&#190;j&#189;{&#193;&#139;&#8;&#247;&#15;&#226;&#229;&#247;&#19;&#247;&#6;&#62;&#221;!`i&#131;xZ&#31;&#14;&#248;&#236;|&#190;&#247;&#172;&#190;&#247;Z&#190;&#1;&#247;&#23;&#189;&#247;&#175;&#191;&#3;&#247;J&#247;&#154;&#21;&#138;&#149;&#139;&#148;&#139;&#144;&#139;&#199;&#155;&#199;&#168;&#181;&#187;&#211;&#216;&#184;&#214;&#139;&#157;&#139;&#154;&#137;&#149;&#134;&#149;&#134;&#143;&#138;&#145;&#139;&#8;&#153;&#149;&#150;&#152;&#162;f&#156;ZJIr]U&#31;@Lg6&#139;&#251;&#9;&#8;&#251;A&#224;&#251;&#14;&#247;&#14;&#239;&#217;&#224;&#247;&#1;&#242;=&#224;,IPeHg&#30;&#146;B&#21;&#162;&#179;&#150;&#156;&#153;&#155;&#171;&#174;&#177;&#158;&#175;&#139;&#8;&#205;&#194;M@:UMD@[&#187;&#244;p&#31;&#14;&#248;&#236;&#138;&#159;&#248;&#169;&#190;&#1;&#248;E&#248;&#176;&#21;&#251;4&#252;&#138;&#137;&#133;&#138;&#135;&#139;&#135;&#25;}&#150;&#128;&#153;&#153;&#145;&#145;&#157;&#145;&#30;&#247;7&#248;&#146;&#5;&#209;&#252;&#20;;&#7;u&#148;&#128;&#156;&#156;&#148;&#150;&#161;&#30;&#168;&#247;&#173;&#7;&#14;&#248;&#236;|&#190;&#247;&#143;&#189;&#247;x&#190;&#18;&#247;&#0;&#191;a&#191;&#247;&#152;&#191;b&#191;&#23;&#19;&#236;&#248;&#24;&#247;&#204;&#21;&#202;&#172;&#170;&#185;&#139;&#197;&#8;&#230;8&#215;&#40;&#40;8?0Q&#171;]&#202;j&#30;&#19;&#242;HkeUL&#26;&#41;&#225;;&#246;&#245;&#225;&#219;&#237;&#202;d&#194;I&#170;&#30;&#19;&#236;1&#247;&#145;&#21;&#213;&#197;WIMR[BBR&#187;&#201;&#204;&#197;&#192;&#209;&#31;&#19;&#242;&#251;&#170;&#4;&#221;&#200;VDDMS=&#60;M&#195;&#210;&#208;&#200;&#194;&#216;&#31;&#14;&#248;&#236;|&#190;&#247;Z&#190;&#247;&#172;&#190;&#1;&#247;&#23;&#191;&#247;&#175;&#189;&#3;&#248;e&#247;&#231;&#21;&#140;&#129;&#139;&#130;&#139;&#135;&#139;N{Ona[C&#62;^@&#139;y&#139;|&#142;&#129;&#144;&#129;&#144;&#135;&#140;&#133;&#139;&#8;}&#129;&#128;}t&#175;z&#189;&#204;&#205;&#164;&#185;&#193;&#31;&#214;&#202;&#175;&#224;&#139;&#247;&#8;&#8;&#247;B6&#247;&#14;&#251;&#14;&#39;=6&#251;&#1;$&#217;6&#234;&#205;&#197;&#177;&#206;&#176;&#30;&#132;&#212;&#21;tc&#128;z|{liewg&#139;&#8;IT&#201;&#214;&#220;&#193;&#201;&#210;&#214;&#186;[&#34;&#167;&#31;&#14;&#248;&#236;|&#190;&#248;&#165;&#190;&#1;&#247;&#0;&#191;&#247;&#173;&#191;&#3;&#248;&#129;&#247;&#242;&#21;&#247;2=&#247;&#0;&#251;&#6;&#251;&#7;=&#251;&#0;&#251;2&#30;&#41;&#7;&#251;3&#217;&#251;&#0;&#247;&#7;&#247;&#6;&#217;&#247;&#0;&#247;3&#30;&#251;&#225;&#231;&#21;&#139;&#201;&#157;&#204;&#168;&#184;&#160;&#171;&#171;&#156;&#180;&#139;&#179;&#139;&#171;z&#160;k&#168;^&#157;J&#139;M&#8;4&#7;&#139;NyIn^vkjzd&#139;c&#139;j&#156;v&#171;n&#184;y&#205;&#139;&#200;&#8;&#14;&#248;&#236;&#139;&#190;&#1;&#247;&#167;&#191;&#3;&#247;&#219;&#248;&#249;&#21;&#251;TOx&#133;&#133;&#133;&#139;}&#25;~&#151;&#127;&#151;&#141;&#149;&#141;&#140;&#143;&#30;&#247;&#17;&#178;&#5;&#252;&#129;&#251;&#26;&#7;u&#128;&#130;{z&#151;&#130;&#160;&#31;&#247;&#212;&#6;&#160;&#150;&#148;&#156;&#155;&#128;&#148;v&#31;&#251;&#26;&#6;&#14;&#248;&#236;&#139;&#190;&#248;&#150;&#190;&#1;&#248;@&#191;&#3;&#247;&#27;&#190;&#21;&#193;&#185;&#201;&#196;&#222;&#219;&#247;&#18;&#247;&#12;&#159;&#168;&#139;&#198;&#8;&#232;2&#220;&#38;MQo[e&#30;wr~m&#139;x&#8;&#127;&#150;&#128;&#153;&#152;&#147;&#146;&#155;&#143;&#30;&#156;&#197;&#198;&#180;&#204;&#139;&#8;&#213;&#203;RJ`yr.1&#31;8&#60;?EEN&#130;&#131;&#24;H&#248;&#41;&#220;&#7;&#160;&#130;&#150;zz&#130;&#128;v&#30;m&#7;&#14;&#248;&#236;|&#190;&#248;&#165;&#190;&#18;&#248;C&#191;l&#191;&#23;&#19;&#208;&#247;&#171;&#247;&#249;&#21;v&#128;&#129;{{&#150;&#130;&#160;&#31;&#235;&#137;&#216;O&#139;@&#8;CBN3SX&#157;&#174;[&#30;&#130;&#145;&#134;&#141;&#132;&#139;&#8;~&#128;&#128;~{&#152;~&#175;y&#31;&#191;o&#186;~&#190;&#139;&#8;&#247;&#10;&#235;&#222;&#240;&#204;]&#201;E&#170;&#31;&#19;&#224;&#200;&#168;&#173;&#186;&#195;&#26;&#228;&#60;&#207;$VX{mc&#30;ty}z&#139;&#127;&#8;~&#150;&#128;&#153;&#147;&#145;&#142;&#145;&#144;&#30;&#175;&#179;&#180;&#156;&#199;&#139;&#8;&#213;&#195;]Okylnx&#31;s|w&#134;d&#139;&#8;&#14;{&#155;&#248;5&#155;&#247;&#22;&#151;&#167;&#152;&#6;&#191;&#10;&#190;&#11;&#182;&#148;&#12;&#12;&#182;&#147;&#12;&#13;&#0;&#0;</data>
 </stream>
 </object>
 
 <object id="8">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>291</number></value>
+<value><number>301</number></value>
 </dict>
 </props>
-<data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -192,37 +198,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>291</number></value>
+<value><number>301</number></value>
 </dict>
 </props>
-<data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
+<object id="13">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -235,37 +247,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="15" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="14">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>291</number></value>
+<value><number>301</number></value>
 </dict>
 </props>
-<data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="15">
+<list size="1">
+<ref id="14" />
+</list>
+</object>
+
+<object id="16">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -278,37 +296,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="18" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="17">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>291</number></value>
+<value><number>301</number></value>
 </dict>
 </props>
-<data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="18">
+<list size="1">
+<ref id="17" />
+</list>
+</object>
+
+<object id="19">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -321,37 +345,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="21" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="20">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>291</number></value>
+<value><number>301</number></value>
 </dict>
 </props>
-<data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="21">
+<list size="1">
+<ref id="20" />
+</list>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -364,37 +394,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>291</number></value>
+<value><number>301</number></value>
 </dict>
 </props>
-<data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="19">
+<object id="24">
+<list size="1">
+<ref id="23" />
+</list>
+</object>
+
+<object id="25">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -407,37 +443,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="20" /></value>
+<value><ref id="27" /></value>
 </dict>
 </object>
 
-<object id="20">
+<object id="26">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>291</number></value>
+<value><number>301</number></value>
 </dict>
 </props>
-<data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="21">
+<object id="27">
+<list size="1">
+<ref id="26" />
+</list>
+</object>
+
+<object id="28">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -450,37 +492,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="22" /></value>
+<value><ref id="30" /></value>
 </dict>
 </object>
 
-<object id="22">
+<object id="29">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>291</number></value>
+<value><number>301</number></value>
 </dict>
 </props>
-<data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="23">
+<object id="30">
+<list size="1">
+<ref id="29" />
+</list>
+</object>
+
+<object id="31">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -493,37 +541,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="24" /></value>
+<value><ref id="33" /></value>
 </dict>
 </object>
 
-<object id="24">
+<object id="32">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>291</number></value>
+<value><number>301</number></value>
 </dict>
 </props>
-<data size="291">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="301">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="25">
+<object id="33">
+<list size="1">
+<ref id="32" />
+</list>
+</object>
+
+<object id="34">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -536,37 +590,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="26" /></value>
+<value><ref id="36" /></value>
 </dict>
 </object>
 
-<object id="26">
+<object id="35">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="27">
+<object id="36">
+<list size="1">
+<ref id="35" />
+</list>
+</object>
+
+<object id="37">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -579,37 +639,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="28" /></value>
+<value><ref id="39" /></value>
 </dict>
 </object>
 
-<object id="28">
+<object id="38">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="29">
+<object id="39">
+<list size="1">
+<ref id="38" />
+</list>
+</object>
+
+<object id="40">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -622,37 +688,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="30" /></value>
+<value><ref id="42" /></value>
 </dict>
 </object>
 
-<object id="30">
+<object id="41">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;12&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="31">
+<object id="42">
+<list size="1">
+<ref id="41" />
+</list>
+</object>
+
+<object id="43">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -665,37 +737,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="32" /></value>
+<value><ref id="45" /></value>
 </dict>
 </object>
 
-<object id="32">
+<object id="44">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;13&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="33">
+<object id="45">
+<list size="1">
+<ref id="44" />
+</list>
+</object>
+
+<object id="46">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -708,37 +786,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="34" /></value>
+<value><ref id="48" /></value>
 </dict>
 </object>
 
-<object id="34">
+<object id="47">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;14&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="35">
+<object id="48">
+<list size="1">
+<ref id="47" />
+</list>
+</object>
+
+<object id="49">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -751,37 +835,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="36" /></value>
+<value><ref id="51" /></value>
 </dict>
 </object>
 
-<object id="36">
+<object id="50">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;15&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="37">
+<object id="51">
+<list size="1">
+<ref id="50" />
+</list>
+</object>
+
+<object id="52">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -794,37 +884,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="38" /></value>
+<value><ref id="54" /></value>
 </dict>
 </object>
 
-<object id="38">
+<object id="53">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;16&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="39">
+<object id="54">
+<list size="1">
+<ref id="53" />
+</list>
+</object>
+
+<object id="55">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -837,37 +933,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="40" /></value>
+<value><ref id="57" /></value>
 </dict>
 </object>
 
-<object id="40">
+<object id="56">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;17&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="41">
+<object id="57">
+<list size="1">
+<ref id="56" />
+</list>
+</object>
+
+<object id="58">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -880,37 +982,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="42" /></value>
+<value><ref id="60" /></value>
 </dict>
 </object>
 
-<object id="42">
+<object id="59">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;18&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="43">
+<object id="60">
+<list size="1">
+<ref id="59" />
+</list>
+</object>
+
+<object id="61">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -923,37 +1031,43 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="44" /></value>
+<value><ref id="63" /></value>
 </dict>
 </object>
 
-<object id="44">
+<object id="62">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;19&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="45">
+<object id="63">
+<list size="1">
+<ref id="62" />
+</list>
+</object>
+
+<object id="64">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -966,40 +1080,46 @@
 <literal>Text</literal>
 </list></value>
 </dict></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0.0</number>
 <number>0.0</number>
-<number>595</number>
 <number>842</number>
+<number>1191</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="46" /></value>
+<value><ref id="66" /></value>
 </dict>
 </object>
 
-<object id="46">
+<object id="65">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>292</number></value>
+<value><number>302</number></value>
 </dict>
 </props>
-<data size="292">q&#10;1.4151260000000001 0.0 0.0 1.4151260000000001 0.323529 0.0 cm&#10;0.0 0.0 420 595 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 116.383 Tf&#10;1 0 0 1 72.880899999999997 454.61700000000002 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 3072.5100000000002 5470 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="302">q&#10;1.4144890000000001 0.0 0.0 1.4144890000000001 0.18943 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;20&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="66">
+<list size="1">
+<ref id="65" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>47</number></value>
+<value><number>67</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-A5in-A4/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psresize/20-A5in-A4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psresize/20-Letter/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psresize/20-Letter/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/even/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/even/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/even/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/even/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/even-reverse/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/even-reverse/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/even-reverse/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/even-reverse/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/individual-pages-and-dash-p/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/individual-pages-and-dash-p/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/individual-pages-and-dash-p/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/individual-pages-and-dash-p/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/negative-range/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/negative-range/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/negative-range/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/negative-range/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/odd/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/odd/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/odd/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/odd/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/options-and-complex-pagerange/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/options-and-complex-pagerange/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/options-and-complex-pagerange/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/options-and-complex-pagerange/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/positive-negative-range/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/positive-negative-range/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/positive-negative-range/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/positive-negative-range/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/positive-range/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/positive-range/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/positive-range/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/positive-range/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/psnup-texlive/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/psnup-texlive/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/psnup-texlive/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/psnup-texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/reverse/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/reverse/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/reverse/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/reverse/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/texlive/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect/texlive/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect/texlive/expected.ps` & `pspdfutils-3.0.8/tests/test-files/psselect/texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect-texlive-output.pdf` & `pspdfutils-3.0.8/tests/test-files/psselect-texlive-output.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/psselect-texlive-output.ps` & `pspdfutils-3.0.8/tests/test-files/psselect-texlive-output.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/correct-angles/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/pstops/multiple-turns-and-flips/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 10% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,5 +1,3 @@
 1
 
-1
-
```

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/correct-angles/expected.ps` & `pspdfutils-3.0.8/tests/test-files/pstops/correct-angles/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/default-paper-size/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/pstops/default-paper-size/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 7% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'1826'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'1826'*

 * *DEBUG:pdfminer.psparser:seek: 1826*

 * *DEBUG:pdfminer.psparser:nexttoken: (1826, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=1826, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 1830, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 1831, b'0 9\n'*

 * *DEBUG:pdfminer.psparser:nextline: 1835, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1855, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1875, b'0000000074 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1895, b'0000000113 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1915, b'0000000162 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1935, b'0000000330 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1955, b'0000000497 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1975, b'0000000750 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1995, b'0000001109 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2015, b'trailer\n'*

 * *DEBUG:pdfminer.psparser:seek: 2015*

 * *DEBUG:pdfminer.pdfdocument:xref objects: {1: (None, 15, 0), 2: (None, 74, 0), 3: (None, 113, 0), 4: (None, 162, 0), 5: (None, 330, 0), 6: (None, 497, 0), 7: (None, 750, 0), 8: (None, 1109, 0)}*

 * *DEBUG:pdfminer.psparser:nexttoken: (2015, /b'trailer')*

 * *DEBUG:pdfminer.psparser:nexttoken: (2023, /b'<<')*

 * *[ truncated after 25 lines; 296 ignored ]*

```diff
@@ -52,15 +52,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>ZUUUSB+Courier</literal></value>
@@ -138,25 +138,56 @@
 </object>
 
 <object id="8">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>666</number></value>
+<value><number>330</number></value>
 </dict>
 </props>
-<data size="666">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595 421 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="330">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="9">
+<list size="2">
+<ref id="10" />
+<ref id="11" />
+</list>
+</object>
+
+<object id="10">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>334</number></value>
+</dict>
+</props>
+<data size="334">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="11">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>332</number></value>
+</dict>
+</props>
+<data size="332">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595 421 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>9</number></value>
+<value><number>12</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/default-paper-size/expected.ps` & `pspdfutils-3.0.8/tests/test-files/pstops/default-paper-size/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/multiple-pages/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/pstops/multiple-pages/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 4% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'2007'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'2007'*

 * *DEBUG:pdfminer.psparser:seek: 2007*

 * *DEBUG:pdfminer.psparser:nexttoken: (2007, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=2007, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 2011, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 2012, b'0 11\n'*

 * *DEBUG:pdfminer.psparser:nextline: 2017, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2037, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2057, b'0000000080 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2077, b'0000000119 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2097, b'0000000168 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2117, b'0000000324 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2137, b'0000000495 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2157, b'0000000755 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2177, b'0000001220 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2197, b'0000001534 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2217, b'0000001691 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2237, b'trailer\n'*

 * *DEBUG:pdfminer.psparser:seek: 2237*

 * *DEBUG:pdfminer.pdfdocument:xref objects: {1: (None, 15, 0), 2: (None, 80, 0), 3: (None, 119, 0), 4: (None, 168, 0), 5: (None, 324, 0), 6: (None, 495, 0), 7: (None, 755, 0), 8: (None, 1220, 0), 9: (None, 1534, 0), 10: (None, 1691, 0)}*

 * *[ truncated after 25 lines; 382 ignored ]*

```diff
@@ -3,15 +3,15 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>2</number></value>
 <key>Kids</key>
 <value><list size="2">
 <ref id="4" />
-<ref id="9" />
+<ref id="10" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -51,15 +51,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JPUFBP+Courier</literal></value>
@@ -146,14 +146,20 @@
 </dict>
 </props>
 <data size="263">q&#10;1 0.0 0.0 1 100 200 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
+<object id="10">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -172,34 +178,40 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="12" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="11">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>264</number></value>
 </dict>
 </props>
 <data size="264">q&#10;1 0.0 0.0 1 -200 100 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="12">
+<list size="1">
+<ref id="11" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>11</number></value>
+<value><number>13</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/multiple-pages/expected.ps` & `pspdfutils-3.0.8/tests/test-files/pstops/multiple-pages/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/multiple-turns-and-flips/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/pstops/negative-offsets/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'1503'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'1503'*

 * *DEBUG:pdfminer.psparser:seek: 1503*

 * *DEBUG:pdfminer.psparser:nexttoken: (1503, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=1503, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 1507, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 1508, b'0 9\n'*

 * *DEBUG:pdfminer.psparser:nextline: 1512, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1532, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1552, b'0000000074 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1572, b'0000000113 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1592, b'0000000162 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1612, b'0000000318 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1632, b'0000000485 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1652, b'0000000738 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1672, b'0000001097 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 1692, b'trailer\n'*

 * *DEBUG:pdfminer.psparser:seek: 1692*

 * *DEBUG:pdfminer.pdfdocument:xref objects: {1: (None, 15, 0), 2: (None, 74, 0), 3: (None, 113, 0), 4: (None, 162, 0), 5: (None, 318, 0), 6: (None, 485, 0), 7: (None, 738, 0), 8: (None, 1097, 0)}*

 * *DEBUG:pdfminer.psparser:nexttoken: (1692, /b'trailer')*

 * *DEBUG:pdfminer.psparser:nexttoken: (1700, /b'<<')*

 * *[ truncated after 25 lines; 291 ignored ]*

```diff
@@ -50,15 +50,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>ZUUUSB+Courier</literal></value>
@@ -136,25 +136,31 @@
 </object>
 
 <object id="8">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>355</number></value>
+<value><number>265</number></value>
 </dict>
 </props>
-<data size="355">q&#10;0.00000000000000006123233995736766 1 1 -0.00000000000000006123233995736766 -142 0.00000000000005155763024410357 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="265">q&#10;1 0.0 0.0 1 -100 -200 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="9">
+<list size="1">
+<ref id="8" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>9</number></value>
+<value><number>10</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/multiple-turns-and-flips/expected.ps` & `pspdfutils-3.0.8/tests/test-files/pstops/multiple-turns-and-flips/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/negative-offsets/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/pstops/offsets/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 15% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,3 +1 @@
-1
-
```

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/negative-offsets/expected.ps` & `pspdfutils-3.0.8/tests/test-files/pstops/negative-offsets/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/offsets/expected.ps` & `pspdfutils-3.0.8/tests/test-files/pstops/offsets/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/texlive/expected.pdf` & `pspdfutils-3.0.8/tests/test-files/pstops/texlive/expected.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 22% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'7277'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'7277'*

 * *DEBUG:pdfminer.psparser:seek: 7277*

 * *DEBUG:pdfminer.psparser:nexttoken: (7277, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=7277, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 7281, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 7282, b'0 19\n'*

 * *DEBUG:pdfminer.psparser:nextline: 7287, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7307, b'0000000015 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7327, b'0000000108 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7347, b'0000000147 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7367, b'0000000196 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7387, b'0000000364 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7407, b'0000000567 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7427, b'0000000897 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7447, b'0000002227 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7467, b'0000002989 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7487, b'0000003158 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7507, b'0000003921 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7527, b'0000004091 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 7547, b'0000004854 00000 n \n'*

 * *[ truncated after 25 lines; 775 ignored ]*

```diff
@@ -3,19 +3,19 @@
 <key>Type</key>
 <value><literal>Pages</literal></value>
 <key>Count</key>
 <value><number>6</number></value>
 <key>Kids</key>
 <value><list size="6">
 <ref id="4" />
-<ref id="9" />
-<ref id="11" />
-<ref id="13" />
-<ref id="15" />
+<ref id="12" />
 <ref id="17" />
+<ref id="22" />
+<ref id="27" />
+<ref id="32" />
 </list></value>
 </dict>
 </object>
 
 <object id="2">
 <dict size="1">
 <key>Producer</key>
@@ -57,15 +57,15 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="8" /></value>
+<value><ref id="9" /></value>
 </dict>
 </object>
 
 <object id="5">
 <dict size="8">
 <key>BaseFont</key>
 <value><literal>JLPWVJ+Courier</literal></value>
@@ -152,22 +152,53 @@
 </object>
 
 <object id="8">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>711</number></value>
+<value><number>345</number></value>
 </dict>
 </props>
-<data size="711">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="345">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
 <object id="9">
+<list size="2">
+<ref id="10" />
+<ref id="11" />
+</list>
+</object>
+
+<object id="10">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>349</number></value>
+</dict>
+</props>
+<data size="349">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;1&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="11">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>362</number></value>
+</dict>
+</props>
+<data size="362">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;2&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="12">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -188,31 +219,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="10" /></value>
+<value><ref id="14" /></value>
 </dict>
 </object>
 
-<object id="10">
+<object id="13">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>711</number></value>
+<value><number>345</number></value>
 </dict>
 </props>
-<data size="711">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="345">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="11">
+<object id="14">
+<list size="2">
+<ref id="15" />
+<ref id="16" />
+</list>
+</object>
+
+<object id="15">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>349</number></value>
+</dict>
+</props>
+<data size="349">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;3&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="16">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>362</number></value>
+</dict>
+</props>
+<data size="362">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;4&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="17">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -233,31 +295,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="12" /></value>
+<value><ref id="19" /></value>
 </dict>
 </object>
 
-<object id="12">
+<object id="18">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>711</number></value>
+<value><number>345</number></value>
 </dict>
 </props>
-<data size="711">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="345">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="13">
+<object id="19">
+<list size="2">
+<ref id="20" />
+<ref id="21" />
+</list>
+</object>
+
+<object id="20">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>349</number></value>
+</dict>
+</props>
+<data size="349">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;5&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="21">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>362</number></value>
+</dict>
+</props>
+<data size="362">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;6&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="22">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -278,31 +371,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="14" /></value>
+<value><ref id="24" /></value>
 </dict>
 </object>
 
-<object id="14">
+<object id="23">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>711</number></value>
+<value><number>345</number></value>
 </dict>
 </props>
-<data size="711">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="345">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="15">
+<object id="24">
+<list size="2">
+<ref id="25" />
+<ref id="26" />
+</list>
+</object>
+
+<object id="25">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>349</number></value>
+</dict>
+</props>
+<data size="349">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;7&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="26">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>362</number></value>
+</dict>
+</props>
+<data size="362">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;8&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="27">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="2">
@@ -323,31 +447,62 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="16" /></value>
+<value><ref id="29" /></value>
 </dict>
 </object>
 
-<object id="16">
+<object id="28">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
-<value><number>712</number></value>
+<value><number>345</number></value>
 </dict>
 </props>
-<data size="712">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+<data size="345">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
-<object id="17">
+<object id="29">
+<list size="2">
+<ref id="30" />
+<ref id="31" />
+</list>
+</object>
+
+<object id="30">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>349</number></value>
+</dict>
+</props>
+<data size="349">q&#10;q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;9&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="31">
+<stream>
+<props>
+<dict size="1">
+<key>Length</key>
+<value><number>363</number></value>
+</dict>
+</props>
+<data size="363">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 420.94488188976374 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7-0 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;10&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
+</stream>
+</object>
+
+<object id="32">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
 <key>Resources</key>
 <value><dict size="2">
 <key>Font</key>
 <value><dict size="1">
@@ -366,34 +521,40 @@
 <number>0.0</number>
 <number>595</number>
 <number>842</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="1" /></value>
 <key>Contents</key>
-<value><ref id="18" /></value>
+<value><ref id="34" /></value>
 </dict>
 </object>
 
-<object id="18">
+<object id="33">
 <stream>
 <props>
 <dict size="1">
 <key>Length</key>
 <value><number>346</number></value>
 </dict>
 </props>
 <data size="346">q&#10;0.00000000000000004286263797015736 0.7 -0.7 0.00000000000000004286263797015736 595.27559055118104 0.0 cm&#10;0.0 0.0 595 842 re&#10;W&#10;n&#10;q&#10;0.10000000000000001 0 0 0.10000000000000001 0 0 cm&#10;0 g&#10;q&#10;10 0 0 10 0 0 cm&#10;BT&#10;/R7 168.93600000000001 Tf&#10;1 0 0 1 94.953100000000006 649.06399999999996 Tm&#10;&#40;11&#41; Tj&#10;ET&#10;Q&#10;7 w&#10;0 G&#10;240 240 4459.9099999999999 7940 re&#10;S&#10;Q&#10;Q&#10;</data>
 </stream>
 </object>
 
+<object id="34">
+<list size="1">
+<ref id="33" />
+</list>
+</object>
+
 <trailer>
 <dict size="3">
 <key>Size</key>
-<value><number>19</number></value>
+<value><number>35</number></value>
 <key>Root</key>
 <value><ref id="3" /></value>
 <key>Info</key>
 <value><ref id="2" /></value>
 </dict>
 </trailer>
```

### Comparing `pspdfutils-3.0.7/tests/test-files/pstops/texlive/expected.ps` & `pspdfutils-3.0.8/tests/test-files/pstops/texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test-files/tiger.eps` & `pspdfutils-3.0.8/tests/test-files/tiger.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test_epsffit.py` & `pspdfutils-3.0.8/tests/test_epsffit.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test_extractres.py` & `pspdfutils-3.0.8/tests/test_extractres.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test_includeres.py` & `pspdfutils-3.0.8/tests/test_includeres.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test_psbook.py` & `pspdfutils-3.0.8/tests/test_psbook.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test_psjoin.py` & `pspdfutils-3.0.8/tests/test_psjoin.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test_psnup.py` & `pspdfutils-3.0.8/tests/test_psnup.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test_psresize.py` & `pspdfutils-3.0.8/tests/test_psresize.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test_psselect.py` & `pspdfutils-3.0.8/tests/test_psselect.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/test_pstops.py` & `pspdfutils-3.0.8/tests/test_pstops.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.7/tests/testutils.py` & `pspdfutils-3.0.8/tests/testutils.py`

 * *Files identical despite different names*

