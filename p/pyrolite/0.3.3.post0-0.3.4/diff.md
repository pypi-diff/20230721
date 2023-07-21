# Comparing `tmp/pyrolite-0.3.3.post0.tar.gz` & `tmp/pyrolite-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrolite-0.3.3.post0.tar", last modified: Wed Jul  5 03:41:52 2023, max compression
+gzip compressed data, was "pyrolite-0.3.4.tar", last modified: Fri Jul 21 06:46:04 2023, max compression
```

## Comparing `pyrolite-0.3.3.post0.tar` & `pyrolite-0.3.4.tar`

### file list

```diff
@@ -1,696 +1,203 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.473302 pyrolite-0.3.3.post0/
--rw-rw-rw-   0        0        0      231 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/.codacy.yml
--rw-rw-rw-   0        0        0      264 2021-03-15 06:56:30.000000 pyrolite-0.3.3.post0/.coveragerc
--rw-rw-rw-   0        0        0       83 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.015331 pyrolite-0.3.3.post0/.github/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.021427 pyrolite-0.3.3.post0/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      588 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-rw-rw-   0        0        0      715 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-rw-rw-   0        0        0     1302 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.029862 pyrolite-0.3.3.post0/.github/workflows/
--rw-rw-rw-   0        0        0      811 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/.github/workflows/docstest.yml
--rw-rw-rw-   0        0        0     2507 2023-07-05 03:37:19.000000 pyrolite-0.3.3.post0/.github/workflows/unittest.yml
--rw-rw-rw-   0        0        0     1341 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/.gitignore
--rw-rw-rw-   0        0        0      577 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/.readthedocs.yml
--rw-rw-rw-   0        0        0      119 2020-06-05 03:51:08.000000 pyrolite-0.3.3.post0/CHANGELOG.md
--rw-rw-rw-   0        0        0      133 2020-02-19 03:00:50.000000 pyrolite-0.3.3.post0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     5147 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     3959 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/LICENSE
--rw-rw-rw-   0        0        0      445 2022-07-06 08:13:53.000000 pyrolite-0.3.3.post0/MANIFEST.in
--rw-rw-rw-   0        0        0    10908 2023-07-05 03:41:52.473302 pyrolite-0.3.3.post0/PKG-INFO
--rw-rw-rw-   0        0        0     9577 2023-07-05 03:37:20.000000 pyrolite-0.3.3.post0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.035853 pyrolite-0.3.3.post0/binder/
--rw-rw-rw-   0        0        0      261 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/binder/environment.yml
--rw-rw-rw-   0        0        0      207 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/binder/postBuild
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.046852 pyrolite-0.3.3.post0/docs/
--rw-rw-rw-   0        0        0      609 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/Makefile
--rw-rw-rw-   0        0        0       13 2021-12-01 08:50:44.000000 pyrolite-0.3.3.post0/docs/docs_require.txt
--rwxrwxrwx   0        0        0      780 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.064854 pyrolite-0.3.3.post0/docs/source/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.076853 pyrolite-0.3.3.post0/docs/source/_patch/
--rw-rw-rw-   0        0        0      725 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/_patch/_sphinx_gallery_patch.py
--rw-rw-rw-   0        0        0     1419 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/_patch/sphinx_gallery_binder.py
--rw-rw-rw-   0        0        0     1988 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/_patch/sphinx_gallery_scrapers.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.091861 pyrolite-0.3.3.post0/docs/source/_static/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.094854 pyrolite-0.3.3.post0/docs/source/_static/css/
--rw-rw-rw-   0        0        0     1743 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/docs/source/_static/css/custom.css
--rw-rw-rw-   0        0        0   280594 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/_static/icon.jpg
--rw-rw-rw-   0        0        0   367817 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/_static/icon.png
--rw-rw-rw-   0        0        0    10738 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/_static/icon_small.jpg
--rw-rw-rw-   0        0        0    17967 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/_static/icon_small.png
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.096854 pyrolite-0.3.3.post0/docs/source/_templates/
--rw-rw-rw-   0        0        0      131 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/_templates/layout.html
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.102852 pyrolite-0.3.3.post0/docs/source/api/
--rw-rw-rw-   0        0        0     1392 2021-03-15 06:56:30.000000 pyrolite-0.3.3.post0/docs/source/api/API.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.115854 pyrolite-0.3.3.post0/docs/source/api/comp/
--rw-rw-rw-   0        0        0      138 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/comp/aggregate.rst
--rw-rw-rw-   0        0        0      132 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/comp/codata.rst
--rw-rw-rw-   0        0        0      132 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/comp/impute.rst
--rw-rw-rw-   0        0        0      163 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/comp/pyrocomp.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.147853 pyrolite-0.3.3.post0/docs/source/api/geochem/
--rw-rw-rw-   0        0        0      146 2020-02-17 08:08:22.000000 pyrolite-0.3.3.post0/docs/source/api/geochem/alteration.rst
--rw-rw-rw-   0        0        0      132 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/geochem/ind.rst
--rw-rw-rw-   0        0        0      139 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/docs/source/api/geochem/ions.rst
--rw-rw-rw-   0        0        0      140 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/geochem/isotope.rst
--rw-rw-rw-   0        0        0      136 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/geochem/magma.rst
--rw-rw-rw-   0        0        0      134 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/geochem/norm.rst
--rw-rw-rw-   0        0        0      136 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/geochem/parse.rst
--rw-rw-rw-   0        0        0      175 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/geochem/pyrochem.rst
--rw-rw-rw-   0        0        0      144 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/geochem/transform.rst
--rw-rw-rw-   0        0        0      928 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/docs/source/api/mineral.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.174855 pyrolite-0.3.3.post0/docs/source/api/plot/
--rw-rw-rw-   0        0        0      132 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/plot/biplot.rst
--rw-rw-rw-   0        0        0      130 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/plot/color.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.185852 pyrolite-0.3.3.post0/docs/source/api/plot/density/
--rw-rw-rw-   0        0        0      134 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/plot/density/density.rst
--rw-rw-rw-   0        0        0      145 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/plot/density/density_grid.rst
--rw-rw-rw-   0        0        0      154 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/plot/density/density_ternary.rst
--rw-rw-rw-   0        0        0      136 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/plot/parallel.rst
--rw-rw-rw-   0        0        0      163 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/plot/pyroplot.rst
--rw-rw-rw-   0        0        0      132 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/plot/spider.rst
--rw-rw-rw-   0        0        0      128 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/api/plot/stem.rst
--rw-rw-rw-   0        0        0      163 2021-08-05 08:05:58.000000 pyrolite-0.3.3.post0/docs/source/api/plot/templates.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.254854 pyrolite-0.3.3.post0/docs/source/api/util/
--rw-rw-rw-   0        0        0      180 2021-08-05 08:04:21.000000 pyrolite-0.3.3.post0/docs/source/api/util/classification.rst
--rw-rw-rw-   0        0        0      151 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/distributions.rst
--rw-rw-rw-   0        0        0      139 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/general.rst
--rw-rw-rw-   0        0        0     1077 2021-03-15 06:56:30.000000 pyrolite-0.3.3.post0/docs/source/api/util/lambdas.rst
--rw-rw-rw-   0        0        0      131 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/docs/source/api/util/log.rst
--rw-rw-rw-   0        0        0      133 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/math.rst
--rw-rw-rw-   0        0        0      133 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/meta.rst
--rw-rw-rw-   0        0        0      139 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/missing.rst
--rw-rw-rw-   0        0        0      129 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/pd.rst
--rw-rw-rw-   0        0        0     1463 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/plot.rst
--rw-rw-rw-   0        0        0      145 2021-08-05 08:00:05.000000 pyrolite-0.3.3.post0/docs/source/api/util/resampling.rst
--rw-rw-rw-   0        0        0      802 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/skl.rst
--rw-rw-rw-   0        0        0      139 2021-03-15 06:56:30.000000 pyrolite-0.3.3.post0/docs/source/api/util/spatial.rst
--rw-rw-rw-   0        0        0      143 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/synthetic.rst
--rw-rw-rw-   0        0        0      133 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/text.rst
--rw-rw-rw-   0        0        0      133 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/time.rst
--rw-rw-rw-   0        0        0      135 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/types.rst
--rw-rw-rw-   0        0        0      135 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/units.rst
--rw-rw-rw-   0        0        0      131 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/api/util/web.rst
--rw-rw-rw-   0        0        0     2976 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/docs/source/cite.rst
--rw-rw-rw-   0        0        0    14266 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/conf.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.279853 pyrolite-0.3.3.post0/docs/source/dev/
--rw-rw-rw-   0        0        0    62814 2023-07-05 03:37:20.000000 pyrolite-0.3.3.post0/docs/source/dev/changelog.rst
--rw-rw-rw-   0        0        0     3757 2020-01-10 09:16:12.000000 pyrolite-0.3.3.post0/docs/source/dev/conduct.rst
--rw-rw-rw-   0        0        0     5365 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/docs/source/dev/contributing.rst
--rw-rw-rw-   0        0        0      909 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/dev/contributors.rst
--rw-rw-rw-   0        0        0     1123 2022-07-06 08:13:53.000000 pyrolite-0.3.3.post0/docs/source/dev/development.rst
--rw-rw-rw-   0        0        0     3969 2021-01-12 03:02:00.000000 pyrolite-0.3.3.post0/docs/source/dev/future.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.295855 pyrolite-0.3.3.post0/docs/source/examples/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.352853 pyrolite-0.3.3.post0/docs/source/examples/comp/
--rw-rw-rw-   0        0        0    12846 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/compositional_data.ipynb
--rw-rw-rw-   0        0        0     9394 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/compositional_data.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/compositional_data.py.md5
--rw-rw-rw-   0        0        0    11316 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/compositional_data.rst
--rw-rw-rw-   0        0        0    27223 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/compositional_data_codeobj.pickle
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.375855 pyrolite-0.3.3.post0/docs/source/examples/comp/images/
--rw-rw-rw-   0        0        0    49439 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/images/sphx_glr_compositional_data_001.png
--rw-rw-rw-   0        0        0    42457 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/images/sphx_glr_compositional_data_002.png
--rw-rw-rw-   0        0        0    77237 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/images/sphx_glr_compositional_data_003.png
--rw-rw-rw-   0        0        0    43029 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/images/sphx_glr_logratiomeans_001.png
--rw-rw-rw-   0        0        0    44833 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/images/sphx_glr_logratiomeans_002.png
--rw-rw-rw-   0        0        0    44960 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/images/sphx_glr_logratiomeans_003.png
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.383853 pyrolite-0.3.3.post0/docs/source/examples/comp/images/thumb/
--rw-rw-rw-   0        0        0    30901 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/images/thumb/sphx_glr_compositional_data_thumb.png
--rw-rw-rw-   0        0        0    26252 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/images/thumb/sphx_glr_logratiomeans_thumb.png
--rw-rw-rw-   0        0        0    43541 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/images/thumb/sphx_glr_logtransforms_thumb.png
--rw-rw-rw-   0        0        0     4637 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logratiomeans.ipynb
--rw-rw-rw-   0        0        0     2667 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logratiomeans.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logratiomeans.py.md5
--rw-rw-rw-   0        0        0     3945 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logratiomeans.rst
--rw-rw-rw-   0        0        0     4909 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logratiomeans_codeobj.pickle
--rw-rw-rw-   0        0        0     6961 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logtransforms.ipynb
--rw-rw-rw-   0        0        0     4449 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logtransforms.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logtransforms.py.md5
--rw-rw-rw-   0        0        0     8444 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logtransforms.rst
--rw-rw-rw-   0        0        0     3298 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/logtransforms_codeobj.pickle
--rw-rw-rw-   0        0        0      911 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/comp/sg_execution_times.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.548923 pyrolite-0.3.3.post0/docs/source/examples/geochem/
--rw-rw-rw-   0        0        0     4070 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/convert_chemistry.ipynb
--rw-rw-rw-   0        0        0     2059 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/convert_chemistry.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/convert_chemistry.py.md5
--rw-rw-rw-   0        0        0     6960 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/convert_chemistry.rst
--rw-rw-rw-   0        0        0     1965 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/convert_chemistry_codeobj.pickle
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.580648 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/
--rw-rw-rw-   0        0        0    30493 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/sphx_glr_ionic_radii_001.png
--rw-rw-rw-   0        0        0    54516 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/sphx_glr_lambdas_001.png
--rw-rw-rw-   0        0        0    42690 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/sphx_glr_lambdas_002.png
--rw-rw-rw-   0        0        0    32807 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/sphx_glr_lambdas_003.png
--rw-rw-rw-   0        0        0    16234 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/sphx_glr_mineral_lattice_001.png
--rw-rw-rw-   0        0        0    21326 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/sphx_glr_mineral_lattice_002.png
--rw-rw-rw-   0        0        0    27245 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/sphx_glr_mineral_lattice_003.png
--rw-rw-rw-   0        0        0    86567 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/sphx_glr_normalization_001.png
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.611799 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/
--rw-rw-rw-   0        0        0    43541 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/sphx_glr_convert_chemistry_thumb.png
--rw-rw-rw-   0        0        0    43541 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/sphx_glr_indexes_selectors_thumb.png
--rw-rw-rw-   0        0        0    30832 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/sphx_glr_ionic_radii_thumb.png
--rw-rw-rw-   0        0        0    27543 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/sphx_glr_lambdas_thumb.png
--rw-rw-rw-   0        0        0    43541 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/sphx_glr_mineral_endmembers_thumb.png
--rw-rw-rw-   0        0        0    18294 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/sphx_glr_mineral_lattice_thumb.png
--rw-rw-rw-   0        0        0    43541 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/sphx_glr_mineral_mindb_thumb.png
--rw-rw-rw-   0        0        0    59847 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/sphx_glr_normalization_thumb.png
--rw-rw-rw-   0        0        0    43541 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/images/thumb/sphx_glr_scaling_thumb.png
--rw-rw-rw-   0        0        0     4799 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/indexes_selectors.ipynb
--rw-rw-rw-   0        0        0     2111 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/indexes_selectors.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/indexes_selectors.py.md5
--rw-rw-rw-   0        0        0    11796 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/indexes_selectors.rst
--rw-rw-rw-   0        0        0     2395 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/indexes_selectors_codeobj.pickle
--rw-rw-rw-   0        0        0     5687 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/ionic_radii.ipynb
--rw-rw-rw-   0        0        0     3811 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/ionic_radii.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/ionic_radii.py.md5
--rw-rw-rw-   0        0        0     5374 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/ionic_radii.rst
--rw-rw-rw-   0        0        0     6503 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/ionic_radii_codeobj.pickle
--rw-rw-rw-   0        0        0     8179 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/lambdas.ipynb
--rw-rw-rw-   0        0        0     6232 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/lambdas.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/lambdas.py.md5
--rw-rw-rw-   0        0        0     7192 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/lambdas.rst
--rw-rw-rw-   0        0        0     4893 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/lambdas_codeobj.pickle
--rw-rw-rw-   0        0        0     5300 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_endmembers.ipynb
--rw-rw-rw-   0        0        0     2760 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_endmembers.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_endmembers.py.md5
--rw-rw-rw-   0        0        0     8768 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_endmembers.rst
--rw-rw-rw-   0        0        0     6570 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_endmembers_codeobj.pickle
--rw-rw-rw-   0        0        0     9553 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_lattice.ipynb
--rw-rw-rw-   0        0        0     7532 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_lattice.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_lattice.py.md5
--rw-rw-rw-   0        0        0     9272 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_lattice.rst
--rw-rw-rw-   0        0        0     8651 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_lattice_codeobj.pickle
--rw-rw-rw-   0        0        0     3221 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_mindb.ipynb
--rw-rw-rw-   0        0        0     1341 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_mindb.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_mindb.py.md5
--rw-rw-rw-   0        0        0     8762 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_mindb.rst
--rw-rw-rw-   0        0        0     1139 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_mindb_codeobj.pickle
--rw-rw-rw-   0        0        0     3428 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/normalization.ipynb
--rw-rw-rw-   0        0        0     1855 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/normalization.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/normalization.py.md5
--rw-rw-rw-   0        0        0     2852 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/normalization.rst
--rw-rw-rw-   0        0        0     4297 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/normalization_codeobj.pickle
--rw-rw-rw-   0        0        0     1806 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/scaling.ipynb
--rw-rw-rw-   0        0        0      559 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/scaling.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/scaling.py.md5
--rw-rw-rw-   0        0        0     2679 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/scaling.rst
--rw-rw-rw-   0        0        0     1418 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/scaling_codeobj.pickle
--rw-rw-rw-   0        0        0     2246 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/geochem/sg_execution_times.rst
--rw-rw-rw-   0        0        0    10658 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/index.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.762857 pyrolite-0.3.3.post0/docs/source/examples/plotting/
--rw-rw-rw-   0        0        0     4494 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/REE_v_radii.ipynb
--rw-rw-rw-   0        0        0     2440 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/REE_v_radii.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/REE_v_radii.py.md5
--rw-rw-rw-   0        0        0     3602 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/REE_v_radii.rst
--rw-rw-rw-   0        0        0     2119 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/REE_v_radii_codeobj.pickle
--rw-rw-rw-   0        0        0    10344 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/density.ipynb
--rw-rw-rw-   0        0        0     6966 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/density.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/density.py.md5
--rw-rw-rw-   0        0        0     8447 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/density.rst
--rw-rw-rw-   0        0        0     9040 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/density_codeobj.pickle
--rw-rw-rw-   0        0        0     4357 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/heatscatter.ipynb
--rw-rw-rw-   0        0        0     2857 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/heatscatter.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/heatscatter.py.md5
--rw-rw-rw-   0        0        0     3998 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/heatscatter.rst
--rw-rw-rw-   0        0        0     3808 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/heatscatter_codeobj.pickle
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.879856 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/
--rw-rw-rw-   0        0        0    62038 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_REE_v_radii_001.png
--rw-rw-rw-   0        0        0    26010 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_REE_v_radii_002.png
--rw-rw-rw-   0        0        0    98921 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_REE_v_radii_003.png
--rw-rw-rw-   0        0        0    15617 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_REE_v_radii_004.png
--rw-rw-rw-   0        0        0    79901 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_density_001.png
--rw-rw-rw-   0        0        0    15327 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_density_002.png
--rw-rw-rw-   0        0        0    14413 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_density_003.png
--rw-rw-rw-   0        0        0    60908 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_density_004.png
--rw-rw-rw-   0        0        0   119445 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_density_005.png
--rw-rw-rw-   0        0        0    53654 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_density_006.png
--rw-rw-rw-   0        0        0    27767 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_density_007.png
--rw-rw-rw-   0        0        0    69473 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_density_008.png
--rw-rw-rw-   0        0        0   161588 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_heatscatter_001.png
--rw-rw-rw-   0        0        0    87593 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_parallel_001.png
--rw-rw-rw-   0        0        0   145009 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_parallel_002.png
--rw-rw-rw-   0        0        0    57062 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_parallel_003.png
--rw-rw-rw-   0        0        0   119585 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_parallel_004.png
--rw-rw-rw-   0        0        0   148765 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_spider_001.png
--rw-rw-rw-   0        0        0   163829 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_spider_002.png
--rw-rw-rw-   0        0        0    33407 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_spider_003.png
--rw-rw-rw-   0        0        0   155595 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_spider_004.png
--rw-rw-rw-   0        0        0   139232 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_spider_005.png
--rw-rw-rw-   0        0        0     7826 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_stem_001.png
--rw-rw-rw-   0        0        0     9171 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_stem_002.png
--rw-rw-rw-   0        0        0    30151 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_templates_001.png
--rw-rw-rw-   0        0        0    23855 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_templates_002.png
--rw-rw-rw-   0        0        0    26320 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_ternary_001.png
--rw-rw-rw-   0        0        0    30876 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_ternary_002.png
--rw-rw-rw-   0        0        0    38275 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/sphx_glr_ternary_003.png
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.907856 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/thumb/
--rw-rw-rw-   0        0        0    31635 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/thumb/sphx_glr_REE_v_radii_thumb.png
--rw-rw-rw-   0        0        0    33856 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/thumb/sphx_glr_density_thumb.png
--rw-rw-rw-   0        0        0    45148 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/thumb/sphx_glr_heatscatter_thumb.png
--rw-rw-rw-   0        0        0    35243 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/thumb/sphx_glr_parallel_thumb.png
--rw-rw-rw-   0        0        0    69030 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/thumb/sphx_glr_spider_thumb.png
--rw-rw-rw-   0        0        0     8136 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/thumb/sphx_glr_stem_thumb.png
--rw-rw-rw-   0        0        0    10523 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/thumb/sphx_glr_templates_thumb.png
--rw-rw-rw-   0        0        0    14102 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/images/thumb/sphx_glr_ternary_thumb.png
--rw-rw-rw-   0        0        0     3872 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/parallel.ipynb
--rw-rw-rw-   0        0        0     2035 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/parallel.py
--rw-rw-rw-   0        0        0       32 2023-05-12 05:07:34.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/parallel.py.md5
--rw-rw-rw-   0        0        0     3315 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/parallel.rst
--rw-rw-rw-   0        0        0     5068 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/parallel_codeobj.pickle
--rw-rw-rw-   0        0        0     2039 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/sg_execution_times.rst
--rw-rw-rw-   0        0        0     7404 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/spider.ipynb
--rw-rw-rw-   0        0        0     4972 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/spider.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/spider.py.md5
--rw-rw-rw-   0        0        0     6236 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/spider.rst
--rw-rw-rw-   0        0        0     3774 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/spider_codeobj.pickle
--rw-rw-rw-   0        0        0     3285 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/stem.ipynb
--rw-rw-rw-   0        0        0     1641 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/stem.py
--rw-rw-rw-   0        0        0       32 2023-05-12 05:07:20.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/stem.py.md5
--rw-rw-rw-   0        0        0     2760 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/stem.rst
--rw-rw-rw-   0        0        0     3646 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/stem_codeobj.pickle
--rw-rw-rw-   0        0        0     3120 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/templates.ipynb
--rw-rw-rw-   0        0        0     1505 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/templates.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/templates.py.md5
--rw-rw-rw-   0        0        0     3736 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/templates.rst
--rw-rw-rw-   0        0        0     1477 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/templates_codeobj.pickle
--rw-rw-rw-   0        0        0     3624 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/ternary.ipynb
--rw-rw-rw-   0        0        0     1683 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/ternary.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/ternary.py.md5
--rw-rw-rw-   0        0        0     4361 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/ternary.rst
--rw-rw-rw-   0        0        0     2686 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/plotting/ternary_codeobj.pickle
--rw-rw-rw-   0        0        0      234 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/searchindex.bak
--rw-rw-rw-   0        0        0    93626 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/searchindex.dat
--rw-rw-rw-   0        0        0      234 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/searchindex.dir
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.948856 pyrolite-0.3.3.post0/docs/source/examples/util/
--rw-rw-rw-   0        0        0     3948 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/TAS.ipynb
--rw-rw-rw-   0        0        0     2084 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/util/TAS.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/TAS.py.md5
--rw-rw-rw-   0        0        0     5385 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/TAS.rst
--rw-rw-rw-   0        0        0     4273 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/TAS_codeobj.pickle
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.963860 pyrolite-0.3.3.post0/docs/source/examples/util/images/
--rw-rw-rw-   0        0        0    34767 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/images/sphx_glr_TAS_001.png
--rw-rw-rw-   0        0        0    37941 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/images/sphx_glr_TAS_002.png
--rw-rw-rw-   0        0        0    19196 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/images/sphx_glr_timescale_001.png
--rw-rw-rw-   0        0        0    21797 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/images/sphx_glr_timescale_002.png
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.971857 pyrolite-0.3.3.post0/docs/source/examples/util/images/thumb/
--rw-rw-rw-   0        0        0    23989 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/images/thumb/sphx_glr_TAS_thumb.png
--rw-rw-rw-   0        0        0    12092 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/images/thumb/sphx_glr_timescale_thumb.png
--rw-rw-rw-   0        0        0      609 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/sg_execution_times.rst
--rw-rw-rw-   0        0        0     6882 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/timescale.ipynb
--rw-rw-rw-   0        0        0     4585 2023-07-03 13:36:26.000000 pyrolite-0.3.3.post0/docs/source/examples/util/timescale.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/timescale.py.md5
--rw-rw-rw-   0        0        0     6156 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/timescale.rst
--rw-rw-rw-   0        0        0    12210 2023-06-02 01:40:52.000000 pyrolite-0.3.3.post0/docs/source/examples/util/timescale_codeobj.pickle
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.974859 pyrolite-0.3.3.post0/docs/source/ext/
--rw-rw-rw-   0        0        0      819 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/docs/source/ext/extensions.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:49.862808 pyrolite-0.3.3.post0/docs/source/gallery/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:50.998856 pyrolite-0.3.3.post0/docs/source/gallery/data/
--rw-rw-rw-   0        0        0      107 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/gallery/data/README.rst
--rw-rw-rw-   0        0        0     1879 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/data/aitchison.py
--rw-rw-rw-   0        0        0      455 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/docs/source/gallery/data/mineral.py
--rw-rw-rw-   0        0        0     2110 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/data/radii.py
--rw-rw-rw-   0        0        0     6665 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/data/refcomp.py
--rw-rw-rw-   0        0        0     1105 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/docs/source/gallery/data/timescale.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.002857 pyrolite-0.3.3.post0/docs/source/gallery/examples/
--rw-rw-rw-   0        0        0      158 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.020857 pyrolite-0.3.3.post0/docs/source/gallery/examples/comp/
--rw-rw-rw-   0        0        0       56 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/comp/README.rst
--rw-rw-rw-   0        0        0     9909 2023-07-03 14:14:29.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/comp/compositional_data.py
--rw-rw-rw-   0        0        0     3213 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/comp/logratiomeans.py
--rw-rw-rw-   0        0        0     5162 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/comp/logtransforms.py
--rw-rw-rw-   0        0        0     4070 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/comp/sphericalcoords.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.063858 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/
--rw-rw-rw-   0        0        0    12365 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/CIPW.py
--rw-rw-rw-   0        0        0       44 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/README.rst
--rw-rw-rw-   0        0        0     2084 2023-07-03 12:41:59.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/convert_chemistry.py
--rw-rw-rw-   0        0        0     2769 2023-07-03 12:41:59.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/indexes_selectors.py
--rw-rw-rw-   0        0        0     3730 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/ionic_radii.py
--rw-rw-rw-   0        0        0    19691 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/lambdas.py
--rw-rw-rw-   0        0        0     2665 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/mineral_endmembers.py
--rw-rw-rw-   0        0        0     7459 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/mineral_lattice.py
--rw-rw-rw-   0        0        0     1248 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/mineral_mindb.py
--rw-rw-rw-   0        0        0     1780 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/normalization.py
--rw-rw-rw-   0        0        0      590 2023-07-03 12:41:59.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/geochem/scaling.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.102857 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/
--rw-rw-rw-   0        0        0      271 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/README.rst
--rw-rw-rw-   0        0        0     2464 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/REE_v_radii.py
--rw-rw-rw-   0        0        0     9635 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/density.py
--rw-rw-rw-   0        0        0     2861 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/heatscatter.py
--rw-rw-rw-   0        0        0     2039 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/parallel.py
--rw-rw-rw-   0        0        0    10866 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/spider.py
--rw-rw-rw-   0        0        0     1643 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/stem.py
--rw-rw-rw-   0        0        0     5586 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/templates.py
--rw-rw-rw-   0        0        0     1736 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/ternary.py
--rw-rw-rw-   0        0        0     3564 2023-07-03 12:45:22.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/plotting/ternary_color.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.117857 pyrolite-0.3.3.post0/docs/source/gallery/examples/util/
--rw-rw-rw-   0        0        0      346 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/util/README.rst
--rw-rw-rw-   0        0        0     3951 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/util/TAS.py
--rw-rw-rw-   0        0        0     1637 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/util/manifold_vis.py
--rw-rw-rw-   0        0        0     4560 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/examples/util/timescale.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.136856 pyrolite-0.3.3.post0/docs/source/gallery/tutorials/
--rw-rw-rw-   0        0        0      308 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/docs/source/gallery/tutorials/README.rst
--rw-rw-rw-   0        0        0     5714 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/tutorials/logo.py
--rw-rw-rw-   0        0        0     8903 2023-07-03 12:45:52.000000 pyrolite-0.3.3.post0/docs/source/gallery/tutorials/plot_formatting.py
--rw-rw-rw-   0        0        0     5396 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/gallery/tutorials/ternary_density.py
--rw-rw-rw-   0        0        0     8568 2020-07-06 10:54:36.000000 pyrolite-0.3.3.post0/docs/source/gettingstarted.rst
--rw-rw-rw-   0        0        0     2964 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/docs/source/index.rst
--rw-rw-rw-   0        0        0     1449 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/docs/source/installation.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.238859 pyrolite-0.3.3.post0/docs/source/tutorials/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.343858 pyrolite-0.3.3.post0/docs/source/tutorials/images/
--rw-rw-rw-   0        0        0    32888 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_logo_001.png
--rw-rw-rw-   0        0        0    70645 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_logo_002.png
--rw-rw-rw-   0        0        0   110389 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_logo_003.png
--rw-rw-rw-   0        0        0   159470 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_logo_004.png
--rw-rw-rw-   0        0        0   190199 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_logo_005.png
--rw-rw-rw-   0        0        0   190199 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_logo_006.png
--rw-rw-rw-   0        0        0     9207 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_001.png
--rw-rw-rw-   0        0        0     6103 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_002.png
--rw-rw-rw-   0        0        0    18050 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_003.png
--rw-rw-rw-   0        0        0     8697 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_004.png
--rw-rw-rw-   0        0        0    11172 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_005.png
--rw-rw-rw-   0        0        0    16009 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_006.png
--rw-rw-rw-   0        0        0    13176 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_007.png
--rw-rw-rw-   0        0        0    22008 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_008.png
--rw-rw-rw-   0        0        0    42464 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_009.png
--rw-rw-rw-   0        0        0    32937 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_010.png
--rw-rw-rw-   0        0        0    29271 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_plot_formatting_011.png
--rw-rw-rw-   0        0        0    69036 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_ternary_density_001.png
--rw-rw-rw-   0        0        0    64371 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/sphx_glr_ternary_density_002.png
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.361376 pyrolite-0.3.3.post0/docs/source/tutorials/images/thumb/
--rw-rw-rw-   0        0        0    55621 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/thumb/sphx_glr_logo_thumb.png
--rw-rw-rw-   0        0        0     9685 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/thumb/sphx_glr_plot_formatting_thumb.png
--rw-rw-rw-   0        0        0    26056 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/images/thumb/sphx_glr_ternary_density_thumb.png
--rw-rw-rw-   0        0        0     1681 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/index.rst
--rw-rw-rw-   0        0        0     8145 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/logo.ipynb
--rw-rw-rw-   0        0        0     5726 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/tutorials/logo.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/logo.py.md5
--rw-rw-rw-   0        0        0     7267 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/logo.rst
--rw-rw-rw-   0        0        0    14503 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/logo_codeobj.pickle
--rw-rw-rw-   0        0        0    12222 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/plot_formatting.ipynb
--rw-rw-rw-   0        0        0     8863 2023-07-03 12:45:58.000000 pyrolite-0.3.3.post0/docs/source/tutorials/plot_formatting.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/plot_formatting.py.md5
--rw-rw-rw-   0        0        0    10559 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/plot_formatting.rst
--rw-rw-rw-   0        0        0    15947 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/plot_formatting_codeobj.pickle
--rw-rw-rw-   0        0        0      234 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/searchindex.bak
--rw-rw-rw-   0        0        0    92962 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/searchindex.dat
--rw-rw-rw-   0        0        0      234 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/searchindex.dir
--rw-rw-rw-   0        0        0      833 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/sg_execution_times.rst
--rw-rw-rw-   0        0        0     7429 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/ternary_density.ipynb
--rw-rw-rw-   0        0        0     5398 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/docs/source/tutorials/ternary_density.py
--rw-rw-rw-   0        0        0       32 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/ternary_density.py.md5
--rw-rw-rw-   0        0        0     6651 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/ternary_density.rst
--rw-rw-rw-   0        0        0     4957 2023-06-02 01:40:56.000000 pyrolite-0.3.3.post0/docs/source/tutorials/ternary_density_codeobj.pickle
--rw-rw-rw-   0        0        0     1367 2023-07-05 03:37:19.000000 pyrolite-0.3.3.post0/environment.yml
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.395373 pyrolite-0.3.3.post0/paper/
--rw-rw-rw-   0        0        0    22704 2020-02-19 03:00:50.000000 pyrolite-0.3.3.post0/paper/paper.bib
--rw-rw-rw-   0        0        0     7002 2020-06-09 12:34:06.000000 pyrolite-0.3.3.post0/paper/paper.md
--rw-rw-rw-   0        0        0     6875 2020-05-08 13:00:22.000000 pyrolite-0.3.3.post0/paper/pyOpenSciSubmission.md
--rw-rw-rw-   0        0        0  2390389 2020-02-19 03:00:50.000000 pyrolite-0.3.3.post0/paper/sphx_glr_heatscatter_001.png
--rw-rw-rw-   0        0        0  2362185 2020-02-19 03:00:50.000000 pyrolite-0.3.3.post0/paper/sphx_glr_spider_005.png
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.479302 pyrolite-0.3.3.post0/pyrolite/
--rw-rw-rw-   0        0        0     1287 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/__init__.py
--rw-rw-rw-   0        0        0      524 2023-07-05 03:41:52.479302 pyrolite-0.3.3.post0/pyrolite/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.485891 pyrolite-0.3.3.post0/pyrolite/comp/
--rw-rw-rw-   0        0        0    13106 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/comp/__init__.py
--rw-rw-rw-   0        0        0     9022 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/comp/aggregate.py
--rw-rw-rw-   0        0        0    21861 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/comp/codata.py
--rw-rw-rw-   0        0        0    13217 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/comp/impute.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:49.908815 pyrolite-0.3.3.post0/pyrolite/data/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.506890 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/
--rw-rw-rw-   0        0        0     1495 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.567893 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/
--rw-rw-rw-   0        0        0     1959 2023-05-12 02:33:50.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-310-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     1850 2023-05-12 03:43:37.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1920 2019-10-13 13:43:28.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-36-pytest-5.1.3.pyc
--rw-rw-rw-   0        0        0     1813 2020-01-16 03:03:46.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0     1926 2019-10-31 03:02:36.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-5.0.0.pyc
--rw-rw-rw-   0        0        0     1926 2020-02-10 07:20:26.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-5.2.1.pyc
--rw-rw-rw-   0        0        0     1926 2020-02-10 05:19:18.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-5.3.5.pyc
--rw-rw-rw-   0        0        0     1926 2020-05-18 07:37:02.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-5.4.2.pyc
--rw-rw-rw-   0        0        0     1937 2020-08-14 06:36:54.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-5.4.3.pyc
--rw-rw-rw-   0        0        0     1937 2020-07-13 06:42:54.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-6.0.0rc1.pyc
--rw-rw-rw-   0        0        0     1937 2020-08-25 06:23:52.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-6.0.1.pyc
--rw-rw-rw-   0        0        0     1941 2021-01-11 05:14:02.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-6.2.1.pyc
--rw-rw-rw-   0        0        0     1964 2021-04-21 04:32:53.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-6.2.3.pyc
--rw-rw-rw-   0        0        0     1981 2022-01-25 05:46:38.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37-pytest-6.2.4.pyc
--rw-rw-rw-   0        0        0     1868 2022-01-25 05:54:04.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      748 2020-01-10 09:16:14.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/boxite.csv
--rw-rw-rw-   0        0        0      852 2020-01-10 09:16:14.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/coxite.csv
--rw-rw-rw-   0        0        0      664 2020-01-10 09:16:14.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/hongite.csv
--rw-rw-rw-   0        0        0      672 2020-01-10 09:16:14.000000 pyrolite-0.3.3.post0/pyrolite/data/Aitchison/kongite.csv
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.572134 pyrolite-0.3.3.post0/pyrolite/data/_config/
--rw-rw-rw-   0        0        0     1113 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/_config/pyrolite.mplstyle
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.581892 pyrolite-0.3.3.post0/pyrolite/data/geochem/
--rw-rw-rw-   0        0        0     3266 2021-10-20 08:20:56.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/geochemdb.json
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.738879 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/
--rw-rw-rw-   0        0        0     1209 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/ARS_Condie1993.csv
--rw-rw-rw-   0        0        0     1343 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/BCC_McLennan2001.csv
--rw-rw-rw-   0        0        0     1698 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/BCC_RudnickGao2003.csv
--rw-rw-rw-   0        0        0     1800 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/BCC_RudnickGao2014.csv
--rw-rw-rw-   0        0        0     1994 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/CH_McDonoughSun1995.csv
--rw-rw-rw-   0        0        0     3718 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/CH_PalmeONeill2014.csv
--rw-rw-rw-   0        0        0      792 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/CH_REE_ONeill2016.csv
--rw-rw-rw-   0        0        0      933 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/CH_SunMcDonough1989.csv
--rw-rw-rw-   0        0        0     1299 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/DDMM_WorkmanHart2005.csv
--rw-rw-rw-   0        0        0     1350 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/DMM_WorkmanHart2005.csv
--rw-rw-rw-   0        0        0     1952 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/DMORB_Gale2013.csv
--rw-rw-rw-   0        0        0     2386 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/DM_SaltersStrake2004.csv
--rw-rw-rw-   0        0        0     1304 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/EDMM_WorkmanHart2005.csv
--rw-rw-rw-   0        0        0     1959 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/EMORB_Gale2013.csv
--rw-rw-rw-   0        0        0      884 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/EMORB_SunMcDonough1989.csv
--rw-rw-rw-   0        0        0     1203 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/EUS_Bau2018.csv
--rw-rw-rw-   0        0        0     1799 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/GLOSS2_Plank2014.csv
--rw-rw-rw-   0        0        0     1262 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/GLOSS_Plank2014.csv
--rw-rw-rw-   0        0        0     1707 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/LCC_McLennan2001.csv
--rw-rw-rw-   0        0        0     1699 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/LCC_RudnickGao2003.csv
--rw-rw-rw-   0        0        0     1800 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/LCC_RudnickGao2014.csv
--rw-rw-rw-   0        0        0     1611 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/MCC_RudnickGao2014.csv
--rw-rw-rw-   0        0        0     1939 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/MORB_Gale2013.csv
--rw-rw-rw-   0        0        0     1396 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/MUQ_Kamber2005.csv
--rw-rw-rw-   0        0        0     1382 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/NASC_Gromet1984.csv
--rw-rw-rw-   0        0        0     1496 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/NMORB_Gale2013.csv
--rw-rw-rw-   0        0        0      891 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/NMORB_SunMcDonough1989.csv
--rw-rw-rw-   0        0        0      870 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/OIB_SunMcDonough1989.csv
--rw-rw-rw-   0        0        0     1238 2021-01-12 03:01:00.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PAAS_Pourmand2012.csv
--rw-rw-rw-   0        0        0     1577 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PAAS_TaylorMcLennan1985.csv
--rw-rw-rw-   0        0        0     1550 2021-01-12 03:00:58.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PHS_Condie1993.csv
--rw-rw-rw-   0        0        0     3648 2021-01-12 03:01:00.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PM_PalmeONeill2014.csv
--rw-rw-rw-   0        0        0      926 2021-01-12 03:01:00.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PM_SunMcDonough1989.csv
--rw-rw-rw-   0        0        0     1550 2021-01-12 03:01:00.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PRS_Condie1993.csv
--rw-rw-rw-   0        0        0     1962 2021-01-12 03:01:00.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PY_McDonoughSun1995.csv
--rw-rw-rw-   0        0        0     1703 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/UCC_McLennan2001.csv
--rw-rw-rw-   0        0        0     1892 2021-01-12 03:01:00.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/UCC_RudnickGao2003.csv
--rw-rw-rw-   0        0        0     1980 2021-01-12 03:01:00.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/UCC_RudnickGao2014.csv
--rw-rw-rw-   0        0        0      988 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp_template.csv
--rw-rw-rw-   0        0        0   238626 2021-01-12 03:01:00.000000 pyrolite-0.3.3.post0/pyrolite/data/geochem/refdb.json
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.745878 pyrolite-0.3.3.post0/pyrolite/data/mineral/
--rw-rw-rw-   0        0        0    32954 2023-07-04 09:11:16.000000 pyrolite-0.3.3.post0/pyrolite/data/mineral/mindb.json
--rw-rw-rw-   0        0        0     3561 2021-01-12 02:59:24.000000 pyrolite-0.3.3.post0/pyrolite/data/mineral/mins.csv
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.753881 pyrolite-0.3.3.post0/pyrolite/data/models/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.757881 pyrolite-0.3.3.post0/pyrolite/data/models/FeldsparTernary/
--rw-rw-rw-   0        0        0     2109 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/data/models/FeldsparTernary/config.json
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.762240 pyrolite-0.3.3.post0/pyrolite/data/models/JensenPlot/
--rw-rw-rw-   0        0        0     1489 2022-07-06 08:13:53.000000 pyrolite-0.3.3.post0/pyrolite/data/models/JensenPlot/config.json
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.764879 pyrolite-0.3.3.post0/pyrolite/data/models/QAP/
--rw-rw-rw-   0        0        0     2918 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/data/models/QAP/config.json
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.767879 pyrolite-0.3.3.post0/pyrolite/data/models/SpinelFeBivariate/
--rw-rw-rw-   0        0        0      981 2022-07-06 08:13:53.000000 pyrolite-0.3.3.post0/pyrolite/data/models/SpinelFeBivariate/config.json
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.772879 pyrolite-0.3.3.post0/pyrolite/data/models/SpinelTrivalentTernary/
--rw-rw-rw-   0        0        0     1083 2022-07-06 08:13:53.000000 pyrolite-0.3.3.post0/pyrolite/data/models/SpinelTrivalentTernary/config.json
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.782880 pyrolite-0.3.3.post0/pyrolite/data/models/TAS/
--rw-rw-rw-   0        0        0     1705 2020-08-07 08:52:24.000000 pyrolite-0.3.3.post0/pyrolite/data/models/TAS/config.json
--rw-rw-rw-   0        0        0     1702 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/data/models/TAS/config_lemaitre.json
--rw-rw-rw-   0        0        0     1581 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/data/models/TAS/config_lemaitre_combined.json
--rw-rw-rw-   0        0        0     1392 2020-06-11 02:49:58.000000 pyrolite-0.3.3.post0/pyrolite/data/models/TAS.clsf.gz
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.786882 pyrolite-0.3.3.post0/pyrolite/data/models/USDASoilTexture/
--rw-rw-rw-   0        0        0     1445 2022-05-04 04:30:05.000000 pyrolite-0.3.3.post0/pyrolite/data/models/USDASoilTexture/config.json
--rw-rw-rw-   0        0        0      276 2020-06-11 02:49:58.000000 pyrolite-0.3.3.post0/pyrolite/data/models/peralkalinity.clsf.gz
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.792881 pyrolite-0.3.3.post0/pyrolite/data/models/sandstones/
--rw-rw-rw-   0        0        0     1126 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/data/models/sandstones/config_herron.json
--rw-rw-rw-   0        0        0     2645 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/data/models/sandstones/config_pettijohn.json
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.799882 pyrolite-0.3.3.post0/pyrolite/data/radii/
--rw-rw-rw-   0        0        0    13045 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/pyrolite/data/radii/shannon.csv
--rw-rw-rw-   0        0        0     6794 2020-07-06 11:03:22.000000 pyrolite-0.3.3.post0/pyrolite/data/radii/whittaker_muntus.csv
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.803882 pyrolite-0.3.3.post0/pyrolite/data/testing/
--rw-rw-rw-   0        0        0   430575 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/data/testing/CIPW_Verma_Test.csv
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.819878 pyrolite-0.3.3.post0/pyrolite/data/timescale/
--rw-rw-rw-   0        0        0    10608 2021-03-15 06:56:30.000000 pyrolite-0.3.3.post0/pyrolite/data/timescale/geotimescale_201807.csv
--rw-rw-rw-   0        0        0    10862 2021-03-15 06:56:30.000000 pyrolite-0.3.3.post0/pyrolite/data/timescale/geotimescale_202003.csv
--rw-rw-rw-   0        0        0    10922 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/data/timescale/geotimescale_202210.csv
--rw-rw-rw-   0        0        0     4132 2020-01-10 09:16:14.000000 pyrolite-0.3.3.post0/pyrolite/data/timescale/timecolors.csv
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.822879 pyrolite-0.3.3.post0/pyrolite/extensions/
--rw-rw-rw-   0        0        0      135 2021-11-10 03:19:48.000000 pyrolite-0.3.3.post0/pyrolite/extensions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.853878 pyrolite-0.3.3.post0/pyrolite/geochem/
--rw-rw-rw-   0        0        0    23503 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/__init__.py
--rw-rw-rw-   0        0        0     6392 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/alteration.py
--rw-rw-rw-   0        0        0    16317 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/ind.py
--rw-rw-rw-   0        0        0     1747 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/ions.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.859880 pyrolite-0.3.3.post0/pyrolite/geochem/isotope/
--rw-rw-rw-   0        0        0     2666 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/isotope/__init__.py
--rw-rw-rw-   0        0        0      784 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/isotope/count.py
--rw-rw-rw-   0        0        0     8463 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/magma.py
--rw-rw-rw-   0        0        0     9742 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/norm.py
--rw-rw-rw-   0        0        0     4613 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/parse.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.863890 pyrolite-0.3.3.post0/pyrolite/geochem/quality/
--rw-rw-rw-   0        0        0     1076 2021-11-10 03:19:43.000000 pyrolite-0.3.3.post0/pyrolite/geochem/quality/__init__.py
--rw-rw-rw-   0        0        0    28782 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/geochem/transform.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.898880 pyrolite-0.3.3.post0/pyrolite/mineral/
--rw-rw-rw-   0        0        0      108 2021-11-10 03:18:33.000000 pyrolite-0.3.3.post0/pyrolite/mineral/__init__.py
--rw-rw-rw-   0        0        0     9419 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/mineral/lattice.py
--rw-rw-rw-   0        0        0     6101 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/mineral/mindb.py
--rw-rw-rw-   0        0        0    47456 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/mineral/normative.py
--rw-rw-rw-   0        0        0     3522 2021-11-10 03:18:46.000000 pyrolite-0.3.3.post0/pyrolite/mineral/sites.py
--rw-rw-rw-   0        0        0    18247 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/mineral/template.py
--rw-rw-rw-   0        0        0     4268 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/mineral/transform.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.920754 pyrolite-0.3.3.post0/pyrolite/plot/
--rw-rw-rw-   0        0        0    20246 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/__init__.py
--rw-rw-rw-   0        0        0     3296 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/biplot.py
--rw-rw-rw-   0        0        0    11326 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/color.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.932982 pyrolite-0.3.3.post0/pyrolite/plot/density/
--rw-rw-rw-   0        0        0    12017 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/density/__init__.py
--rw-rw-rw-   0        0        0     6262 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/density/grid.py
--rw-rw-rw-   0        0        0     5161 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/density/ternary.py
--rw-rw-rw-   0        0        0     2258 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/parallel.py
--rw-rw-rw-   0        0        0    14427 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/spider.py
--rw-rw-rw-   0        0        0     1402 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/stem.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.977029 pyrolite-0.3.3.post0/pyrolite/plot/templates/
--rw-rw-rw-   0        0        0     1719 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/QAP.py
--rw-rw-rw-   0        0        0     2682 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/TAS.py
--rw-rw-rw-   0        0        0     1545 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/USDA_soil_texture.py
--rw-rw-rw-   0        0        0      843 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/__init__.py
--rw-rw-rw-   0        0        0    10060 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/components.py
--rw-rw-rw-   0        0        0     1747 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/feldspar.py
--rw-rw-rw-   0        0        0     1562 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/jensen.py
--rw-rw-rw-   0        0        0     5073 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/pearce.py
--rw-rw-rw-   0        0        0     3998 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/sandstones.py
--rw-rw-rw-   0        0        0     1932 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/plot/templates/spinel.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.053028 pyrolite-0.3.3.post0/pyrolite/util/
--rw-rw-rw-   0        0        0      399 2021-11-10 03:21:52.000000 pyrolite-0.3.3.post0/pyrolite/util/__init__.py
--rw-rw-rw-   0        0        0    28149 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/classification.py
--rw-rw-rw-   0        0        0     2954 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/database.py
--rw-rw-rw-   0        0        0     5179 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/distributions.py
--rw-rw-rw-   0        0        0     2791 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/env.py
--rw-rw-rw-   0        0        0     4749 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/general.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.082236 pyrolite-0.3.3.post0/pyrolite/util/lambdas/
--rw-rw-rw-   0        0        0     6302 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/lambdas/__init__.py
--rw-rw-rw-   0        0        0     4370 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/lambdas/eval.py
--rw-rw-rw-   0        0        0     5066 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/lambdas/oneill.py
--rw-rw-rw-   0        0        0    11202 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/lambdas/opt.py
--rw-rw-rw-   0        0        0     7131 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/lambdas/params.py
--rw-rw-rw-   0        0        0     7304 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/lambdas/plot.py
--rw-rw-rw-   0        0        0     2411 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/lambdas/transform.py
--rw-rw-rw-   0        0        0     3931 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/log.py
--rw-rw-rw-   0        0        0    17468 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/math.py
--rw-rw-rw-   0        0        0     6750 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/meta.py
--rw-rw-rw-   0        0        0     2833 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/missing.py
--rw-rw-rw-   0        0        0     2205 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/multip.py
--rw-rw-rw-   0        0        0     9629 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/pd.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.138029 pyrolite-0.3.3.post0/pyrolite/util/plot/
--rw-rw-rw-   0        0        0      709 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/__init__.py
--rw-rw-rw-   0        0        0    10606 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/axes.py
--rw-rw-rw-   0        0        0    13638 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/density.py
--rw-rw-rw-   0        0        0     4473 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/export.py
--rw-rw-rw-   0        0        0     3692 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/grid.py
--rw-rw-rw-   0        0        0    17208 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/helpers.py
--rw-rw-rw-   0        0        0     4665 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/interpolation.py
--rw-rw-rw-   0        0        0     1482 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/legend.py
--rw-rw-rw-   0        0        0     8543 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/style.py
--rw-rw-rw-   0        0        0     3237 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/plot/transform.py
--rw-rw-rw-   0        0        0    17604 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/resampling.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.169697 pyrolite-0.3.3.post0/pyrolite/util/skl/
--rw-rw-rw-   0        0        0      105 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/skl/__init__.py
--rw-rw-rw-   0        0        0     1936 2021-12-01 09:33:58.000000 pyrolite-0.3.3.post0/pyrolite/util/skl/helpers.py
--rw-rw-rw-   0        0        0     4585 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/skl/impute.py
--rw-rw-rw-   0        0        0     9813 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/skl/pipeline.py
--rw-rw-rw-   0        0        0     3631 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/skl/select.py
--rw-rw-rw-   0        0        0    14121 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/skl/transform.py
--rw-rw-rw-   0        0        0    12012 2022-07-06 08:13:53.000000 pyrolite-0.3.3.post0/pyrolite/util/skl/vis.py
--rw-rw-rw-   0        0        0    12198 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/spatial.py
--rw-rw-rw-   0        0        0    12231 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/synthetic.py
--rw-rw-rw-   0        0        0     7204 2022-07-06 08:13:53.000000 pyrolite-0.3.3.post0/pyrolite/util/text.py
--rw-rw-rw-   0        0        0     9266 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/time.py
--rw-rw-rw-   0        0        0      465 2021-11-10 03:21:54.000000 pyrolite-0.3.3.post0/pyrolite/util/types.py
--rw-rw-rw-   0        0        0     1217 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/pyrolite/util/units.py
--rw-rw-rw-   0        0        0     2103 2021-11-10 03:21:08.000000 pyrolite-0.3.3.post0/pyrolite/util/web.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:51.467373 pyrolite-0.3.3.post0/pyrolite.egg-info/
--rw-rw-rw-   0        0        0    10908 2023-07-05 03:41:49.000000 pyrolite-0.3.3.post0/pyrolite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    25835 2023-07-05 03:41:49.000000 pyrolite-0.3.3.post0/pyrolite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 03:41:49.000000 pyrolite-0.3.3.post0/pyrolite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      563 2023-07-05 03:41:49.000000 pyrolite-0.3.3.post0/pyrolite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-05 03:41:49.000000 pyrolite-0.3.3.post0/pyrolite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      466 2023-07-05 03:41:52.477304 pyrolite-0.3.3.post0/setup.cfg
--rw-rw-rw-   0        0        0     3151 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.176694 pyrolite-0.3.3.post0/test/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.200223 pyrolite-0.3.3.post0/test/comp/
--rw-rw-rw-   0        0        0    14589 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/comp/comp_aggregate.py
--rw-rw-rw-   0        0        0     7270 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/comp/comp_codata.py
--rw-rw-rw-   0        0        0     2202 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/comp/comp_impute.py
--rw-rw-rw-   0        0        0     5608 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/comp/comp_pyrocomp.py
--rw-rw-rw-   0        0        0      917 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/extensions.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.247260 pyrolite-0.3.3.post0/test/geochem/
--rw-rw-rw-   0        0        0     1694 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/geochem/geochem_alteration.py
--rw-rw-rw-   0        0        0    10483 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/geochem/geochem_ind.py
--rw-rw-rw-   0        0        0      220 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/geochem/geochem_isotope.py
--rw-rw-rw-   0        0        0     3948 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/geochem/geochem_magma.py
--rw-rw-rw-   0        0        0     2507 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/geochem/geochem_norm.py
--rw-rw-rw-   0        0        0     4098 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/geochem/geochem_parse.py
--rw-rw-rw-   0        0        0     6575 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/geochem/geochem_pyrochem.py
--rw-rw-rw-   0        0        0      103 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/geochem/geochem_quality.py
--rw-rw-rw-   0        0        0    21815 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/geochem/geochem_transform.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.275259 pyrolite-0.3.3.post0/test/mineral/
--rw-rw-rw-   0        0        0     1287 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/mineral/mineral_lattice.py
--rw-rw-rw-   0        0        0     2842 2023-07-03 12:42:07.000000 pyrolite-0.3.3.post0/test/mineral/mineral_mindb.py
--rw-rw-rw-   0        0        0     7714 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/mineral/mineral_normative.py
--rw-rw-rw-   0        0        0      612 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/mineral/mineral_sites.py
--rw-rw-rw-   0        0        0     5171 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/mineral/mineral_template.py
--rw-rw-rw-   0        0        0     1452 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/mineral/mineral_transform.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.301262 pyrolite-0.3.3.post0/test/plot/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.306260 pyrolite-0.3.3.post0/test/plot/density/
--rw-rw-rw-   0        0        0     6309 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/plot/density/plot_density.py
--rw-rw-rw-   0        0        0      577 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/plot/plot_biplot.py
--rw-rw-rw-   0        0        0     7578 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/plot/plot_color.py
--rw-rw-rw-   0        0        0     1187 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/plot/plot_parallel.py
--rw-rw-rw-   0        0        0     5797 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/plot/plot_pyroplot.py
--rw-rw-rw-   0        0        0     4182 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/plot/plot_spider.py
--rw-rw-rw-   0        0        0     1156 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/plot/plot_stem.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.314260 pyrolite-0.3.3.post0/test/plot/templates/
--rw-rw-rw-   0        0        0     2749 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/plot/templates/plot_templates.py
--rw-rw-rw-   0        0        0     3139 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/plot/templates/plot_templates_components.py
--rw-rw-rw-   0        0        0       29 2020-01-10 09:16:14.000000 pyrolite-0.3.3.post0/test/pytest.ini
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.388783 pyrolite-0.3.3.post0/test/util/
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.411782 pyrolite-0.3.3.post0/test/util/lambdas/
--rw-rw-rw-   0        0        0    10972 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/lambdas/util_lambdas.py
--rw-rw-rw-   0        0        0     1644 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/lambdas/util_lambdas_plot.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.451304 pyrolite-0.3.3.post0/test/util/plot/
--rw-rw-rw-   0        0        0     5244 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/plot/util_plot_axes.py
--rw-rw-rw-   0        0        0     4108 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/plot/util_plot_density.py
--rw-rw-rw-   0        0        0     1139 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/plot/util_plot_export.py
--rw-rw-rw-   0        0        0     2278 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/plot/util_plot_grid.py
--rw-rw-rw-   0        0        0     7268 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/plot/util_plot_helpers.py
--rw-rw-rw-   0        0        0      807 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/plot/util_plot_interpolation.py
--rw-rw-rw-   0        0        0     1363 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/plot/util_plot_legend.py
--rw-rw-rw-   0        0        0      566 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/plot/util_plot_style.py
--rw-rw-rw-   0        0        0     1825 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/plot/util_plot_transform.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:41:52.469303 pyrolite-0.3.3.post0/test/util/skl/
--rw-rw-rw-   0        0        0     2037 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/skl/util_skl_impute.py
--rw-rw-rw-   0        0        0     3220 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/skl/util_skl_pipeline.py
--rw-rw-rw-   0        0        0     2468 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/skl/util_skl_select.py
--rw-rw-rw-   0        0        0     5627 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/skl/util_skl_transform.py
--rw-rw-rw-   0        0        0     3666 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/skl/util_skl_vis.py
--rw-rw-rw-   0        0        0     5079 2023-07-03 12:42:07.000000 pyrolite-0.3.3.post0/test/util/util_classification.py
--rw-rw-rw-   0        0        0     1001 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_distributions.py
--rw-rw-rw-   0        0        0     2696 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_env.py
--rw-rw-rw-   0        0        0     2962 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_general.py
--rw-rw-rw-   0        0        0     2576 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_log.py
--rw-rw-rw-   0        0        0    15378 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_math.py
--rw-rw-rw-   0        0        0     1191 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_meta.py
--rw-rw-rw-   0        0        0     2776 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_missing.py
--rw-rw-rw-   0        0        0     1906 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_multip.py
--rw-rw-rw-   0        0        0     7902 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_pd.py
--rw-rw-rw-   0        0        0     5248 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_resampling.py
--rw-rw-rw-   0        0        0     7991 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_spatial.py
--rw-rw-rw-   0        0        0     4007 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_synthetic.py
--rw-rw-rw-   0        0        0     8378 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_text.py
--rw-rw-rw-   0        0        0     3291 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_time.py
--rw-rw-rw-   0        0        0      735 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_types.py
--rw-rw-rw-   0        0        0     3438 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_units.py
--rw-rw-rw-   0        0        0     1026 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/test/util/util_web.py
--rw-rw-rw-   0        0        0    70636 2023-07-04 09:26:33.000000 pyrolite-0.3.3.post0/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:04.046146 pyrolite-0.3.4/
+-rw-rw-rw-   0        0        0     3959 2020-01-10 09:16:12.000000 pyrolite-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-07-21 06:45:24.000000 pyrolite-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    15409 2023-07-21 06:46:04.045146 pyrolite-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9573 2023-07-21 06:45:24.000000 pyrolite-0.3.4/README.md
+-rw-rw-rw-   0        0        0     3325 2023-07-21 06:45:24.000000 pyrolite-0.3.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.550617 pyrolite-0.3.4/pyrolite/
+-rw-rw-rw-   0        0        0     1363 2023-07-21 06:45:24.000000 pyrolite-0.3.4/pyrolite/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-07-21 06:46:04.047146 pyrolite-0.3.4/pyrolite/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.610616 pyrolite-0.3.4/pyrolite/comp/
+-rw-rw-rw-   0        0        0    13106 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/comp/__init__.py
+-rw-rw-rw-   0        0        0     9022 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/comp/aggregate.py
+-rw-rw-rw-   0        0        0    21858 2023-07-21 06:45:24.000000 pyrolite-0.3.4/pyrolite/comp/codata.py
+-rw-rw-rw-   0        0        0    13217 2023-07-07 12:47:09.000000 pyrolite-0.3.4/pyrolite/comp/impute.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.513616 pyrolite-0.3.4/pyrolite/data/
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.624647 pyrolite-0.3.4/pyrolite/data/Aitchison/
+-rw-rw-rw-   0        0        0     1495 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/data/Aitchison/__init__.py
+-rw-rw-rw-   0        0        0      748 2020-01-10 09:16:14.000000 pyrolite-0.3.4/pyrolite/data/Aitchison/boxite.csv
+-rw-rw-rw-   0        0        0      852 2020-01-10 09:16:14.000000 pyrolite-0.3.4/pyrolite/data/Aitchison/coxite.csv
+-rw-rw-rw-   0        0        0      664 2020-01-10 09:16:14.000000 pyrolite-0.3.4/pyrolite/data/Aitchison/hongite.csv
+-rw-rw-rw-   0        0        0      672 2020-01-10 09:16:14.000000 pyrolite-0.3.4/pyrolite/data/Aitchison/kongite.csv
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.627616 pyrolite-0.3.4/pyrolite/data/_config/
+-rw-rw-rw-   0        0        0     1113 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/_config/pyrolite.mplstyle
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.637619 pyrolite-0.3.4/pyrolite/data/geochem/
+-rw-rw-rw-   0        0        0     3266 2021-10-20 08:20:56.000000 pyrolite-0.3.4/pyrolite/data/geochem/geochemdb.json
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.735616 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/
+-rw-rw-rw-   0        0        0     1209 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/ARS_Condie1993.csv
+-rw-rw-rw-   0        0        0     1343 2020-08-07 08:52:24.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/BCC_McLennan2001.csv
+-rw-rw-rw-   0        0        0     1698 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/BCC_RudnickGao2003.csv
+-rw-rw-rw-   0        0        0     1800 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/BCC_RudnickGao2014.csv
+-rw-rw-rw-   0        0        0     1994 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/CH_McDonoughSun1995.csv
+-rw-rw-rw-   0        0        0     3718 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/CH_PalmeONeill2014.csv
+-rw-rw-rw-   0        0        0      792 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/CH_REE_ONeill2016.csv
+-rw-rw-rw-   0        0        0      933 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/CH_SunMcDonough1989.csv
+-rw-rw-rw-   0        0        0     1299 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/DDMM_WorkmanHart2005.csv
+-rw-rw-rw-   0        0        0     1350 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/DMM_WorkmanHart2005.csv
+-rw-rw-rw-   0        0        0     1952 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/DMORB_Gale2013.csv
+-rw-rw-rw-   0        0        0     2386 2020-08-07 08:52:24.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/DM_SaltersStrake2004.csv
+-rw-rw-rw-   0        0        0     1304 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/EDMM_WorkmanHart2005.csv
+-rw-rw-rw-   0        0        0     1959 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/EMORB_Gale2013.csv
+-rw-rw-rw-   0        0        0      884 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/EMORB_SunMcDonough1989.csv
+-rw-rw-rw-   0        0        0     1203 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/EUS_Bau2018.csv
+-rw-rw-rw-   0        0        0     1799 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/GLOSS2_Plank2014.csv
+-rw-rw-rw-   0        0        0     1262 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/GLOSS_Plank2014.csv
+-rw-rw-rw-   0        0        0     1707 2020-08-07 08:52:24.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/LCC_McLennan2001.csv
+-rw-rw-rw-   0        0        0     1699 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/LCC_RudnickGao2003.csv
+-rw-rw-rw-   0        0        0     1800 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/LCC_RudnickGao2014.csv
+-rw-rw-rw-   0        0        0     1611 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/MCC_RudnickGao2014.csv
+-rw-rw-rw-   0        0        0     1939 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/MORB_Gale2013.csv
+-rw-rw-rw-   0        0        0     1396 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/MUQ_Kamber2005.csv
+-rw-rw-rw-   0        0        0     1382 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/NASC_Gromet1984.csv
+-rw-rw-rw-   0        0        0     1496 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/NMORB_Gale2013.csv
+-rw-rw-rw-   0        0        0      891 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/NMORB_SunMcDonough1989.csv
+-rw-rw-rw-   0        0        0      870 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/OIB_SunMcDonough1989.csv
+-rw-rw-rw-   0        0        0     1238 2021-01-12 03:01:00.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PAAS_Pourmand2012.csv
+-rw-rw-rw-   0        0        0     1577 2020-08-07 08:52:24.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PAAS_TaylorMcLennan1985.csv
+-rw-rw-rw-   0        0        0     1550 2021-01-12 03:00:58.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PHS_Condie1993.csv
+-rw-rw-rw-   0        0        0     3648 2021-01-12 03:01:00.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PM_PalmeONeill2014.csv
+-rw-rw-rw-   0        0        0      926 2021-01-12 03:01:00.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PM_SunMcDonough1989.csv
+-rw-rw-rw-   0        0        0     1550 2021-01-12 03:01:00.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PRS_Condie1993.csv
+-rw-rw-rw-   0        0        0     1962 2021-01-12 03:01:00.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PY_McDonoughSun1995.csv
+-rw-rw-rw-   0        0        0     1703 2020-08-07 08:52:24.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/UCC_McLennan2001.csv
+-rw-rw-rw-   0        0        0     1892 2021-01-12 03:01:00.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/UCC_RudnickGao2003.csv
+-rw-rw-rw-   0        0        0     1980 2021-01-12 03:01:00.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp/UCC_RudnickGao2014.csv
+-rw-rw-rw-   0        0        0      988 2020-08-07 08:52:24.000000 pyrolite-0.3.4/pyrolite/data/geochem/refcomp_template.csv
+-rw-rw-rw-   0        0        0   238626 2021-01-12 03:01:00.000000 pyrolite-0.3.4/pyrolite/data/geochem/refdb.json
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.740618 pyrolite-0.3.4/pyrolite/data/mineral/
+-rw-rw-rw-   0        0        0    32954 2023-07-21 05:06:56.000000 pyrolite-0.3.4/pyrolite/data/mineral/mindb.json
+-rw-rw-rw-   0        0        0     3561 2021-01-12 02:59:24.000000 pyrolite-0.3.4/pyrolite/data/mineral/mins.csv
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.747616 pyrolite-0.3.4/pyrolite/data/models/
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.749616 pyrolite-0.3.4/pyrolite/data/models/FeldsparTernary/
+-rw-rw-rw-   0        0        0     2109 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/data/models/FeldsparTernary/config.json
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.752616 pyrolite-0.3.4/pyrolite/data/models/JensenPlot/
+-rw-rw-rw-   0        0        0     1489 2022-07-06 08:13:53.000000 pyrolite-0.3.4/pyrolite/data/models/JensenPlot/config.json
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.754617 pyrolite-0.3.4/pyrolite/data/models/QAP/
+-rw-rw-rw-   0        0        0     2918 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/data/models/QAP/config.json
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.757618 pyrolite-0.3.4/pyrolite/data/models/SpinelFeBivariate/
+-rw-rw-rw-   0        0        0      981 2022-07-06 08:13:53.000000 pyrolite-0.3.4/pyrolite/data/models/SpinelFeBivariate/config.json
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.760620 pyrolite-0.3.4/pyrolite/data/models/SpinelTrivalentTernary/
+-rw-rw-rw-   0        0        0     1083 2022-07-06 08:13:53.000000 pyrolite-0.3.4/pyrolite/data/models/SpinelTrivalentTernary/config.json
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.768617 pyrolite-0.3.4/pyrolite/data/models/TAS/
+-rw-rw-rw-   0        0        0     1705 2020-08-07 08:52:24.000000 pyrolite-0.3.4/pyrolite/data/models/TAS/config.json
+-rw-rw-rw-   0        0        0     1702 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/data/models/TAS/config_lemaitre.json
+-rw-rw-rw-   0        0        0     1581 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/data/models/TAS/config_lemaitre_combined.json
+-rw-rw-rw-   0        0        0     1392 2020-06-11 02:49:58.000000 pyrolite-0.3.4/pyrolite/data/models/TAS.clsf.gz
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.770616 pyrolite-0.3.4/pyrolite/data/models/USDASoilTexture/
+-rw-rw-rw-   0        0        0     1445 2022-05-04 04:30:05.000000 pyrolite-0.3.4/pyrolite/data/models/USDASoilTexture/config.json
+-rw-rw-rw-   0        0        0      276 2020-06-11 02:49:58.000000 pyrolite-0.3.4/pyrolite/data/models/peralkalinity.clsf.gz
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.776619 pyrolite-0.3.4/pyrolite/data/models/sandstones/
+-rw-rw-rw-   0        0        0     1126 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/data/models/sandstones/config_herron.json
+-rw-rw-rw-   0        0        0     2645 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/data/models/sandstones/config_pettijohn.json
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.781617 pyrolite-0.3.4/pyrolite/data/radii/
+-rw-rw-rw-   0        0        0    13045 2020-07-06 11:03:22.000000 pyrolite-0.3.4/pyrolite/data/radii/shannon.csv
+-rw-rw-rw-   0        0        0     6794 2020-07-06 11:03:22.000000 pyrolite-0.3.4/pyrolite/data/radii/whittaker_muntus.csv
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.784616 pyrolite-0.3.4/pyrolite/data/testing/
+-rw-rw-rw-   0        0        0   430575 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/data/testing/CIPW_Verma_Test.csv
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.796617 pyrolite-0.3.4/pyrolite/data/timescale/
+-rw-rw-rw-   0        0        0    10608 2021-03-15 06:56:30.000000 pyrolite-0.3.4/pyrolite/data/timescale/geotimescale_201807.csv
+-rw-rw-rw-   0        0        0    10862 2021-03-15 06:56:30.000000 pyrolite-0.3.4/pyrolite/data/timescale/geotimescale_202003.csv
+-rw-rw-rw-   0        0        0    10922 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/data/timescale/geotimescale_202210.csv
+-rw-rw-rw-   0        0        0     4132 2020-01-10 09:16:14.000000 pyrolite-0.3.4/pyrolite/data/timescale/timecolors.csv
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.798616 pyrolite-0.3.4/pyrolite/extensions/
+-rw-rw-rw-   0        0        0      135 2021-11-10 03:19:48.000000 pyrolite-0.3.4/pyrolite/extensions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.818616 pyrolite-0.3.4/pyrolite/geochem/
+-rw-rw-rw-   0        0        0    23503 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/geochem/__init__.py
+-rw-rw-rw-   0        0        0     6392 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/geochem/alteration.py
+-rw-rw-rw-   0        0        0    16317 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/geochem/ind.py
+-rw-rw-rw-   0        0        0     1747 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/geochem/ions.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.823619 pyrolite-0.3.4/pyrolite/geochem/isotope/
+-rw-rw-rw-   0        0        0     2666 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/geochem/isotope/__init__.py
+-rw-rw-rw-   0        0        0      784 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/geochem/isotope/count.py
+-rw-rw-rw-   0        0        0     8463 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/geochem/magma.py
+-rw-rw-rw-   0        0        0     9742 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/geochem/norm.py
+-rw-rw-rw-   0        0        0     4613 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/geochem/parse.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.825617 pyrolite-0.3.4/pyrolite/geochem/quality/
+-rw-rw-rw-   0        0        0     1076 2021-11-10 03:19:43.000000 pyrolite-0.3.4/pyrolite/geochem/quality/__init__.py
+-rw-rw-rw-   0        0        0    28782 2023-07-20 03:02:12.000000 pyrolite-0.3.4/pyrolite/geochem/transform.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.846616 pyrolite-0.3.4/pyrolite/mineral/
+-rw-rw-rw-   0        0        0      108 2021-11-10 03:18:33.000000 pyrolite-0.3.4/pyrolite/mineral/__init__.py
+-rw-rw-rw-   0        0        0     9419 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/mineral/lattice.py
+-rw-rw-rw-   0        0        0     6101 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/mineral/mindb.py
+-rw-rw-rw-   0        0        0    47393 2023-07-21 06:45:24.000000 pyrolite-0.3.4/pyrolite/mineral/normative.py
+-rw-rw-rw-   0        0        0     3522 2021-11-10 03:18:46.000000 pyrolite-0.3.4/pyrolite/mineral/sites.py
+-rw-rw-rw-   0        0        0    18247 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/mineral/template.py
+-rw-rw-rw-   0        0        0     4268 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/mineral/transform.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.861616 pyrolite-0.3.4/pyrolite/plot/
+-rw-rw-rw-   0        0        0    20246 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/__init__.py
+-rw-rw-rw-   0        0        0     3296 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/biplot.py
+-rw-rw-rw-   0        0        0    11326 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/color.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.869616 pyrolite-0.3.4/pyrolite/plot/density/
+-rw-rw-rw-   0        0        0    12017 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/density/__init__.py
+-rw-rw-rw-   0        0        0     6262 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/density/grid.py
+-rw-rw-rw-   0        0        0     5161 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/density/ternary.py
+-rw-rw-rw-   0        0        0     2258 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/parallel.py
+-rw-rw-rw-   0        0        0    14427 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/spider.py
+-rw-rw-rw-   0        0        0     1402 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/stem.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.894617 pyrolite-0.3.4/pyrolite/plot/templates/
+-rw-rw-rw-   0        0        0     1719 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/templates/QAP.py
+-rw-rw-rw-   0        0        0     2682 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/templates/TAS.py
+-rw-rw-rw-   0        0        0     1545 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/templates/USDA_soil_texture.py
+-rw-rw-rw-   0        0        0      843 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/templates/__init__.py
+-rw-rw-rw-   0        0        0    10060 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/plot/templates/components.py
+-rw-rw-rw-   0        0        0     1747 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/templates/feldspar.py
+-rw-rw-rw-   0        0        0     1562 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/templates/jensen.py
+-rw-rw-rw-   0        0        0     5073 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/templates/pearce.py
+-rw-rw-rw-   0        0        0     3998 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/templates/sandstones.py
+-rw-rw-rw-   0        0        0     1932 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/plot/templates/spinel.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.952619 pyrolite-0.3.4/pyrolite/util/
+-rw-rw-rw-   0        0        0      399 2021-11-10 03:21:52.000000 pyrolite-0.3.4/pyrolite/util/__init__.py
+-rw-rw-rw-   0        0        0    28149 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/classification.py
+-rw-rw-rw-   0        0        0     2954 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/database.py
+-rw-rw-rw-   0        0        0     5179 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/distributions.py
+-rw-rw-rw-   0        0        0     2791 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/env.py
+-rw-rw-rw-   0        0        0     4749 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/general.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.975622 pyrolite-0.3.4/pyrolite/util/lambdas/
+-rw-rw-rw-   0        0        0     6302 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/lambdas/__init__.py
+-rw-rw-rw-   0        0        0     4370 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/lambdas/eval.py
+-rw-rw-rw-   0        0        0     5066 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/lambdas/oneill.py
+-rw-rw-rw-   0        0        0    11202 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/lambdas/opt.py
+-rw-rw-rw-   0        0        0     7131 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/lambdas/params.py
+-rw-rw-rw-   0        0        0     7304 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/lambdas/plot.py
+-rw-rw-rw-   0        0        0     2411 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/lambdas/transform.py
+-rw-rw-rw-   0        0        0     3931 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/log.py
+-rw-rw-rw-   0        0        0    17468 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/math.py
+-rw-rw-rw-   0        0        0     6714 2023-07-21 06:45:24.000000 pyrolite-0.3.4/pyrolite/util/meta.py
+-rw-rw-rw-   0        0        0     2833 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/missing.py
+-rw-rw-rw-   0        0        0     2205 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/multip.py
+-rw-rw-rw-   0        0        0     9629 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/pd.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:04.004617 pyrolite-0.3.4/pyrolite/util/plot/
+-rw-rw-rw-   0        0        0      709 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/plot/__init__.py
+-rw-rw-rw-   0        0        0    10606 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/plot/axes.py
+-rw-rw-rw-   0        0        0    13638 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/plot/density.py
+-rw-rw-rw-   0        0        0     4473 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/plot/export.py
+-rw-rw-rw-   0        0        0     3692 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/plot/grid.py
+-rw-rw-rw-   0        0        0    17208 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/plot/helpers.py
+-rw-rw-rw-   0        0        0     4665 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/plot/interpolation.py
+-rw-rw-rw-   0        0        0     1482 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/plot/legend.py
+-rw-rw-rw-   0        0        0     8543 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/plot/style.py
+-rw-rw-rw-   0        0        0     3237 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/plot/transform.py
+-rw-rw-rw-   0        0        0    17604 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/resampling.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:04.043147 pyrolite-0.3.4/pyrolite/util/skl/
+-rw-rw-rw-   0        0        0      105 2021-12-01 09:33:58.000000 pyrolite-0.3.4/pyrolite/util/skl/__init__.py
+-rw-rw-rw-   0        0        0     1936 2023-07-13 12:58:01.000000 pyrolite-0.3.4/pyrolite/util/skl/helpers.py
+-rw-rw-rw-   0        0        0     4585 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/skl/impute.py
+-rw-rw-rw-   0        0        0     9813 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/skl/pipeline.py
+-rw-rw-rw-   0        0        0     3631 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/skl/select.py
+-rw-rw-rw-   0        0        0    14121 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/skl/transform.py
+-rw-rw-rw-   0        0        0    12012 2022-07-06 08:13:53.000000 pyrolite-0.3.4/pyrolite/util/skl/vis.py
+-rw-rw-rw-   0        0        0    12282 2023-07-21 06:45:24.000000 pyrolite-0.3.4/pyrolite/util/spatial.py
+-rw-rw-rw-   0        0        0    12231 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/synthetic.py
+-rw-rw-rw-   0        0        0     7204 2022-07-06 08:13:53.000000 pyrolite-0.3.4/pyrolite/util/text.py
+-rw-rw-rw-   0        0        0     9266 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/time.py
+-rw-rw-rw-   0        0        0      465 2021-11-10 03:21:54.000000 pyrolite-0.3.4/pyrolite/util/types.py
+-rw-rw-rw-   0        0        0     1217 2023-07-04 09:26:33.000000 pyrolite-0.3.4/pyrolite/util/units.py
+-rw-rw-rw-   0        0        0     2103 2021-11-10 03:21:08.000000 pyrolite-0.3.4/pyrolite/util/web.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:46:03.597616 pyrolite-0.3.4/pyrolite.egg-info/
+-rw-rw-rw-   0        0        0    15409 2023-07-21 06:46:03.000000 pyrolite-0.3.4/pyrolite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6164 2023-07-21 06:46:03.000000 pyrolite-0.3.4/pyrolite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 06:46:03.000000 pyrolite-0.3.4/pyrolite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      490 2023-07-21 06:46:03.000000 pyrolite-0.3.4/pyrolite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2023-07-21 06:46:03.000000 pyrolite-0.3.4/pyrolite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 06:46:04.047146 pyrolite-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      144 2023-07-21 06:45:24.000000 pyrolite-0.3.4/setup.py
```

### Comparing `pyrolite-0.3.3.post0/LICENSE` & `pyrolite-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/PKG-INFO` & `pyrolite-0.3.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: pyrolite
-Version: 0.3.3.post0
-Summary: Tools for geochemical data analysis.
-Home-page: https://github.com/morganjwilliams/pyrolite
-Author: Morgan Williams
-Author-email: morgan.williams@csiro.au
-License: CSIRO Modifed MIT/BSD
-Project-URL: Documentation, https://pyrolite.readthedocs.io/
-Project-URL: Code, https://github.com/morganjwilliams/pyrolite
-Project-URL: Issue tracker, https://github.com/morganjwilliams/pyrolite/issues
-Keywords: geochemistry,compositional data,visualisation,petrology
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Matplotlib
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: skl
-Provides-Extra: spatial
-Provides-Extra: db
-Provides-Extra: stats
-License-File: LICENSE
-
 # `pyrolite`
 
 <img src="https://raw.githubusercontent.com/morganjwilliams/pyrolite/develop/docs/source/_static/icon.jpg" alt="pyrolite Logo" width="30%" align="right">
 
 [![pyrolite Documentation](https://readthedocs.org/projects/pyrolite/badge/?version=develop)](https://pyrolite.readthedocs.io/)
 [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-review/issues/20)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.02314/status.svg)](https://doi.org/10.21105/joss.02314)
@@ -94,13 +61,13 @@
 If you use pyrolite extensively for your research, citation of the software would be particularly appreciated. It helps quantify the impact of the project (assisting those contributing through paid and volunteer work), and is one way to get the message out and help build the pyrolite community. For information on citing pyrolite, [see the relevant docs page](https://pyrolite.readthedocs.io/en/main/cite.html).
 
 ## Development & Build Status
 
 [![Formatted with Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Code Quality](https://api.codacy.com/project/badge/Grade/fd9912a3faae43bf84a47e3da685d84c)](https://app.codacy.com/gh/morganjwilliams/pyrolite/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=morganjwilliams/pyrolite&amp;utm_campaign=Badge_Grade)
 
-|                                                                                  **master**                                                                                  |                                                                                  **develop**                                                                                   |
+|                                                                                  **main**                                                                                  |                                                                                  **develop**                                                                                   |
 |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|                               [![Unit Tests on Master](https://github.com/morganjwilliams/pyrolite/workflows/Unittest/badge.svg?branch=main)](https://github.com/morganjwilliams/pyrolite/actions?query=workflow:Unittest+branch:main)                                |                               [![Unit Tests on Develop](https://github.com/morganjwilliams/pyrolite/workflows/Unittest/badge.svg?branch=develop)](https://github.com/morganjwilliams/pyrolite/actions?query=workflow:Unittest+branch:develop)                                |
+|                               [![Unit Tests on main](https://github.com/morganjwilliams/pyrolite/workflows/Unittest/badge.svg?branch=main)](https://github.com/morganjwilliams/pyrolite/actions?query=workflow:Unittest+branch:main)                                |                               [![Unit Tests on Develop](https://github.com/morganjwilliams/pyrolite/workflows/Unittest/badge.svg?branch=develop)](https://github.com/morganjwilliams/pyrolite/actions?query=workflow:Unittest+branch:develop)                                |
 | [![Coverage Status](https://coveralls.io/repos/github/morganjwilliams/pyrolite/badge.svg?branch=main)](https://coveralls.io/github/morganjwilliams/pyrolite?branch=main) | [![Coverage Status](https://coveralls.io/repos/github/morganjwilliams/pyrolite/badge.svg?branch=develop)](https://coveralls.io/github/morganjwilliams/pyrolite?branch=develop) |
 
 **Maintainer**: Morgan Williams (morgan.williams _at_ csiro.au)
```

### Comparing `pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_lattice.ipynb` & `pyrolite-0.3.4/pyrolite/mineral/lattice.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,598 +1,589 @@
-00000000: 7b0d 0a20 2022 6365 6c6c 7322 3a20 5b0d  {..  "cells": [.
-00000010: 0a20 2020 207b 0d0a 2020 2020 2020 2263  .    {..      "c
-00000020: 656c 6c5f 7479 7065 223a 2022 636f 6465  ell_type": "code
-00000030: 222c 0d0a 2020 2020 2020 2265 7865 6375  ",..      "execu
-00000040: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
-00000050: 6c2c 0d0a 2020 2020 2020 226d 6574 6164  l,..      "metad
-00000060: 6174 6122 3a20 7b0d 0a20 2020 2020 2020  ata": {..       
-00000070: 2022 636f 6c6c 6170 7365 6422 3a20 6661   "collapsed": fa
-00000080: 6c73 650d 0a20 2020 2020 207d 2c0d 0a20  lse..      },.. 
-00000090: 2020 2020 2022 6f75 7470 7574 7322 3a20       "outputs": 
-000000a0: 5b5d 2c0d 0a20 2020 2020 2022 736f 7572  [],..      "sour
-000000b0: 6365 223a 205b 0d0a 2020 2020 2020 2020  ce": [..        
-000000c0: 2225 6d61 7470 6c6f 746c 6962 2069 6e6c  "%matplotlib inl
-000000d0: 696e 6522 0d0a 2020 2020 2020 5d0d 0a20  ine"..      ].. 
-000000e0: 2020 207d 2c0d 0a20 2020 207b 0d0a 2020     },..    {..  
-000000f0: 2020 2020 2263 656c 6c5f 7479 7065 223a      "cell_type":
-00000100: 2022 6d61 726b 646f 776e 222c 0d0a 2020   "markdown",..  
-00000110: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
-00000120: 7b7d 2c0d 0a20 2020 2020 2022 736f 7572  {},..      "sour
-00000130: 6365 223a 205b 0d0a 2020 2020 2020 2020  ce": [..        
-00000140: 225c 6e4c 6174 7469 6365 2053 7472 6169  "\nLattice Strai
-00000150: 6e20 4361 6c63 756c 6174 696f 6e73 5c6e  n Calculations\n
-00000160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 5c6e  --------------\n
-00000180: 5c6e 3c64 6976 2063 6c61 7373 3d5c 2261  \n<div class=\"a
-00000190: 6c65 7274 2061 6c65 7274 2d69 6e66 6f5c  lert alert-info\
-000001a0: 223e 3c68 343e 4e6f 7465 3c2f 6834 3e3c  "><h4>Note</h4><
-000001b0: 703e 5468 6973 2065 7861 6d70 6c65 2066  p>This example f
-000001c0: 6f6c 6c6f 7773 2074 6861 7420 6769 7665  ollows that give
-000001d0: 6e20 6475 7269 6e67 2061 2049 6e73 7469  n during a Insti
-000001e0: 7475 7465 206f 6620 4164 7661 6e63 6564  tute of Advanced
-000001f0: 2053 7475 6469 6573 204d 6173 7465 7263   Studies Masterc
-00000200: 6c61 7373 5c6e 2020 2020 7769 7468 204a  lass\n    with J
-00000210: 6f6e 2042 6c75 6e64 7920 6174 2074 6865  on Blundy at the
-00000220: 2055 6e69 7665 7273 6974 7920 6f66 2057   University of W
-00000230: 6573 7465 726e 2041 7573 7472 616c 6961  estern Australia
-00000240: 206f 6e20 7468 6520 3239 5c5c 203a 7375   on the 29\\ :su
-00000250: 703a 6074 6860 2041 7072 696c 5c6e 2020  p:`th` April\n  
-00000260: 2020 3230 3139 2c20 616e 6420 6973 2075    2019, and is u
-00000270: 7365 6420 6865 7265 2077 6974 6820 7065  sed here with pe
-00000280: 726d 6973 7369 6f6e 2e3c 2f70 3e3c 2f64  rmission.</p></d
-00000290: 6976 3e5c 6e5c 6e5c 6e50 7972 6f6c 6974  iv>\n\n\nPyrolit
-000002a0: 6520 696e 636c 7564 6573 2061 2066 756e  e includes a fun
-000002b0: 6374 696f 6e20 666f 7220 6361 6c63 756c  ction for calcul
-000002c0: 6174 696e 6720 7265 6c61 7469 7665 206c  ating relative l
-000002d0: 6174 7469 6365 2073 7472 6169 6e20 5b23  attice strain [#
-000002e0: 7265 665f 315d 5f2c 2077 6869 6368 5c6e  ref_1]_, which\n
-000002f0: 746f 6765 7468 6572 2077 6974 6820 7468  together with th
-00000300: 6520 7461 626c 6573 206f 6620 5368 616e  e tables of Shan
-00000310: 6e6f 6e20 696f 6e69 6320 7261 6469 6920  non ionic radii 
-00000320: 616e 6420 596f 756e 6727 7320 6d6f 6475  and Young's modu
-00000330: 6c75 7320 6170 7072 6f78 696d 6174 696f  lus approximatio
-00000340: 6e73 2066 6f72 5c6e 7369 6c69 6361 7465  ns for\nsilicate
-00000350: 2061 6e64 206f 7869 6465 2063 6174 696f   and oxide catio
-00000360: 6e69 6320 7369 7465 7320 656e 6162 6c65  nic sites enable
-00000370: 2072 656c 6174 6976 656c 7920 7369 6d70   relatively simp
-00000380: 6c65 2063 616c 6375 6c61 7469 6f6e 206f  le calculation o
-00000390: 6620 696f 6e69 635c 6e70 6172 7469 7469  f ionic\npartiti
-000003a0: 6f6e 696e 6720 696e 2063 6f6d 6d6f 6e20  oning in common 
-000003b0: 726f 636b 2066 6f72 6d69 6e67 206d 696e  rock forming min
-000003c0: 6572 616c 732e 5c6e 5c6e 5468 6973 2065  erals.\n\nThis e
-000003d0: 7861 6d70 6c65 2062 656c 6f77 2075 7365  xample below use
-000003e0: 7320 7072 6576 696f 7573 6c79 2063 6861  s previously cha
-000003f0: 7261 6374 6572 6973 6564 2063 616c 6369  racterised calci
-00000400: 756d 2061 6e64 2073 6f64 6975 6d20 7061  um and sodium pa
-00000410: 7274 6974 696f 6e5c 6e63 6f65 6666 6963  rtition\ncoeffic
-00000420: 6965 6e74 7320 6265 7477 6565 6e20 706c  ients between pl
-00000430: 6167 696f 636c 6173 6520 2824 4361 416c  agioclase ($CaAl
-00000440: 5f32 5369 5f32 4f5f 3820 2d20 4e61 416c  _2Si_2O_8 - NaAl
-00000450: 5369 5f33 4f38 2429 2061 6e64 2073 696c  Si_3O8$) and sil
-00000460: 6963 6174 6520 6d65 6c74 5c6e 746f 2065  icate melt\nto e
-00000470: 7374 696d 6174 6520 7061 7274 6974 696f  stimate partitio
-00000480: 6e69 6e67 2066 6f72 206f 7468 6572 2063  ning for other c
-00000490: 6174 696f 6e73 2062 6173 6564 206f 6e20  ations based on 
-000004a0: 7468 6569 7220 696f 6e69 6320 7261 6469  their ionic radi
-000004b0: 692e 5c6e 5c6e 4120 6d6f 6465 6c20 7061  i.\n\nA model pa
-000004c0: 7261 6d65 7465 7269 7365 6420 7573 696e  rameterised usin
-000004d0: 6720 736f 6469 756d 2061 6e64 2063 616c  g sodium and cal
-000004e0: 6369 756d 2070 6172 7469 7469 6f6e 2063  cium partition c
-000004f0: 6f65 6666 6963 6965 6e74 7320 5b23 7265  oefficients [#re
-00000500: 665f 325d 5f20 6973 2074 6865 6e5c 6e75  f_2]_ is then\nu
-00000510: 7365 6420 746f 2065 7374 696d 6174 6520  sed to estimate 
-00000520: 7468 6520 7061 7274 6974 696f 6e69 6e67  the partitioning
-00000530: 2066 6f72 206c 616e 7468 616e 756d 2069   for lanthanum i
-00000540: 6e74 6f20 7468 6520 7472 6976 616c 656e  nto the trivalen
-00000550: 7420 7369 7465 2028 6c61 7267 656c 795c  t site (largely\
-00000560: 6e6f 6363 7570 6965 6420 6279 2024 416c  noccupied by $Al
-00000570: 5e7b 332b 7d24 292c 2061 6e64 2065 7874  ^{3+}$), and ext
-00000580: 656e 6465 6420 746f 206f 7468 6572 2074  ended to other t
-00000590: 7269 7661 6c65 6e74 2063 6174 696f 6e73  rivalent cations
-000005a0: 2028 6865 7265 2c20 7468 6520 5261 7265   (here, the Rare
-000005b0: 5c6e 4561 7274 6820 456c 656d 656e 7473  \nEarth Elements
-000005c0: 292e 2054 6865 2066 696e 616c 2073 6563  ). The final sec
-000005d0: 7469 6f6e 206f 6620 7468 6520 6578 616d  tion of the exam
-000005e0: 706c 6520 6869 6768 6c69 6768 7473 2074  ple highlights t
-000005f0: 6865 206d 6563 6861 6e69 736d 2077 6869  he mechanism whi
-00000600: 6368 5c6e 6765 6e65 7261 7465 7320 706c  ch\ngenerates pl
-00000610: 6167 696f 636c 6173 6527 7320 6861 6c6c  agioclase's hall
-00000620: 6d61 726b 2027 6575 726f 7069 756d 2061  mark 'europium a
-00000630: 6e6f 6d61 6c79 272c 2061 6e64 2074 6865  nomaly', and the
-00000640: 2065 6666 6563 7473 206f 6620 7661 7269   effects of vari
-00000650: 6162 6c65 5c6e 6575 726f 7069 756d 206f  able\neuropium o
-00000660: 7869 6461 7469 6f6e 2073 7461 7465 206f  xidation state o
-00000670: 6e20 6275 6c6b 2065 7572 6f70 6975 6d20  n bulk europium 
-00000680: 7061 7274 6974 696f 6e69 6e67 2e5c 6e22  partitioning.\n"
-00000690: 0d0a 2020 2020 2020 5d0d 0a20 2020 207d  ..      ]..    }
-000006a0: 2c0d 0a20 2020 207b 0d0a 2020 2020 2020  ,..    {..      
-000006b0: 2263 656c 6c5f 7479 7065 223a 2022 636f  "cell_type": "co
-000006c0: 6465 222c 0d0a 2020 2020 2020 2265 7865  de",..      "exe
-000006d0: 6375 7469 6f6e 5f63 6f75 6e74 223a 206e  cution_count": n
-000006e0: 756c 6c2c 0d0a 2020 2020 2020 226d 6574  ull,..      "met
-000006f0: 6164 6174 6122 3a20 7b0d 0a20 2020 2020  adata": {..     
-00000700: 2020 2022 636f 6c6c 6170 7365 6422 3a20     "collapsed": 
-00000710: 6661 6c73 650d 0a20 2020 2020 207d 2c0d  false..      },.
-00000720: 0a20 2020 2020 2022 6f75 7470 7574 7322  .      "outputs"
-00000730: 3a20 5b5d 2c0d 0a20 2020 2020 2022 736f  : [],..      "so
-00000740: 7572 6365 223a 205b 0d0a 2020 2020 2020  urce": [..      
-00000750: 2020 2269 6d70 6f72 7420 6e75 6d70 7920    "import numpy 
-00000760: 6173 206e 705c 6e69 6d70 6f72 7420 6d61  as np\nimport ma
-00000770: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
-00000780: 6173 2070 6c74 5c6e 6672 6f6d 2070 7972  as plt\nfrom pyr
-00000790: 6f6c 6974 652e 6765 6f63 6865 6d2e 696e  olite.geochem.in
-000007a0: 6420 696d 706f 7274 2052 4545 2c20 6765  d import REE, ge
-000007b0: 745f 696f 6e69 635f 7261 6469 695c 6e66  t_ionic_radii\nf
-000007c0: 726f 6d20 7079 726f 6c69 7465 2e6d 696e  rom pyrolite.min
-000007d0: 6572 616c 2e6c 6174 7469 6365 2069 6d70  eral.lattice imp
-000007e0: 6f72 7420 7374 7261 696e 5f63 6f65 6666  ort strain_coeff
-000007f0: 6963 6965 6e74 220d 0a20 2020 2020 205d  icient"..      ]
-00000800: 0d0a 2020 2020 7d2c 0d0a 2020 2020 7b0d  ..    },..    {.
-00000810: 0a20 2020 2020 2022 6365 6c6c 5f74 7970  .      "cell_typ
-00000820: 6522 3a20 226d 6172 6b64 6f77 6e22 2c0d  e": "markdown",.
-00000830: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
-00000840: 223a 207b 7d2c 0d0a 2020 2020 2020 2273  ": {},..      "s
-00000850: 6f75 7263 6522 3a20 5b0d 0a20 2020 2020  ource": [..     
-00000860: 2020 2022 4669 7273 742c 2077 6520 6e65     "First, we ne
-00000870: 6564 2074 6f20 6465 6669 6e65 2073 6f6d  ed to define som
-00000880: 6520 6f66 2074 6865 206e 6563 6573 7361  e of the necessa
-00000890: 7279 2070 6172 616d 6574 6572 7320 696e  ry parameters in
-000008a0: 636c 7564 696e 6720 7465 6d70 6572 6174  cluding temperat
-000008b0: 7572 652c 2074 6865 2059 6f75 6e67 2773  ure, the Young's
-000008c0: 5c6e 6d6f 6475 6c69 2066 6f72 2074 6865  \nmoduli for the
-000008d0: 2024 585e 7b32 2b7d 2420 616e 6420 2458   $X^{2+}$ and $X
-000008e0: 5e7b 332b 7d24 2073 6974 6573 2069 6e20  ^{3+}$ sites in 
-000008f0: 706c 6167 696f 636c 6173 6520 2824 455f  plagioclase ($E_
-00000900: 3224 2c5c 6e24 455f 3324 292c 2061 6e64  2$,\n$E_3$), and
-00000910: 2073 6f6d 6520 7265 6665 7265 6e63 6520   some reference 
-00000920: 7061 7274 6974 696f 6e20 636f 6566 6669  partition coeffi
-00000930: 6369 656e 7473 2061 6e64 2072 6164 6969  cients and radii
-00000940: 2066 6f72 2063 616c 6369 756d 2061 6e64   for calcium and
-00000950: 5c6e 736f 6469 756d 3a5c 6e5c 6e22 0d0a  \nsodium:\n\n"..
-00000960: 2020 2020 2020 5d0d 0a20 2020 207d 2c0d        ]..    },.
-00000970: 0a20 2020 207b 0d0a 2020 2020 2020 2263  .    {..      "c
-00000980: 656c 6c5f 7479 7065 223a 2022 636f 6465  ell_type": "code
-00000990: 222c 0d0a 2020 2020 2020 2265 7865 6375  ",..      "execu
-000009a0: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
-000009b0: 6c2c 0d0a 2020 2020 2020 226d 6574 6164  l,..      "metad
-000009c0: 6174 6122 3a20 7b0d 0a20 2020 2020 2020  ata": {..       
-000009d0: 2022 636f 6c6c 6170 7365 6422 3a20 6661   "collapsed": fa
-000009e0: 6c73 650d 0a20 2020 2020 207d 2c0d 0a20  lse..      },.. 
-000009f0: 2020 2020 2022 6f75 7470 7574 7322 3a20       "outputs": 
-00000a00: 5b5d 2c0d 0a20 2020 2020 2022 736f 7572  [],..      "sour
-00000a10: 6365 223a 205b 0d0a 2020 2020 2020 2020  ce": [..        
-00000a20: 2244 5f4e 6120 3d20 312e 3335 2020 2320  "D_Na = 1.35  # 
-00000a30: 5061 7274 6974 696f 6e20 636f 6566 6669  Partition coeffi
-00000a40: 6369 656e 7420 506c 6167 2d4d 656c 745c  cient Plag-Melt\
-00000a50: 6e44 5f43 6120 3d20 342e 3120 2023 2050  nD_Ca = 4.1  # P
-00000a60: 6172 7469 7469 6f6e 2063 6f65 6666 6963  artition coeffic
-00000a70: 6965 6e74 2050 6c61 672d 4d65 6c74 5c6e  ient Plag-Melt\n
-00000a80: 5463 203d 2039 3030 2020 2320 5465 6d70  Tc = 900  # Temp
-00000a90: 6572 6174 7572 652c 205c 7530 3062 3043  erature, \u00b0C
-00000aa0: 5c6e 546b 203d 2054 6320 2b20 3237 332e  \nTk = Tc + 273.
-00000ab0: 3135 2020 2320 5465 6d70 6572 6174 7572  15  # Temperatur
-00000ac0: 652c 204b 5c6e 455f 3220 3d20 3132 3020  e, K\nE_2 = 120 
-00000ad0: 2a20 3130 202a 2a20 3920 2023 2059 6f75  * 10 ** 9  # You
-00000ae0: 6e67 7320 6d6f 6475 6c75 7320 666f 7220  ngs modulus for 
-00000af0: 322b 2073 6974 652c 2050 615c 6e45 5f33  2+ site, Pa\nE_3
-00000b00: 203d 2031 3335 202a 2031 3020 2a2a 2039   = 135 * 10 ** 9
-00000b10: 2020 2320 596f 756e 6773 206d 6f64 756c    # Youngs modul
-00000b20: 7573 2066 6f72 2033 2b20 7369 7465 2c20  us for 3+ site, 
-00000b30: 5061 5c6e 7230 322c 2072 3033 203d 2031  Pa\nr02, r03 = 1
-00000b40: 2e31 3936 2c20 312e 3239 3420 2023 2066  .196, 1.294  # f
-00000b50: 6963 7469 7665 2069 6465 616c 2063 6174  ictive ideal cat
-00000b60: 696f 6e20 7261 6469 6920 666f 7220 7468  ion radii for th
-00000b70: 6573 6520 7369 7465 735c 6e72 4361 203d  ese sites\nrCa =
-00000b80: 2067 6574 5f69 6f6e 6963 5f72 6164 6969   get_ionic_radii
-00000b90: 285c 2243 615c 222c 2063 6861 7267 653d  (\"Ca\", charge=
-00000ba0: 322c 2063 6f6f 7264 696e 6174 696f 6e3d  2, coordination=
-00000bb0: 3829 5c6e 724c 6120 3d20 6765 745f 696f  8)\nrLa = get_io
-00000bc0: 6e69 635f 7261 6469 6928 5c22 4c61 5c22  nic_radii(\"La\"
-00000bd0: 2c20 6368 6172 6765 3d33 2c20 636f 6f72  , charge=3, coor
-00000be0: 6469 6e61 7469 6f6e 3d38 2922 0d0a 2020  dination=8)"..  
-00000bf0: 2020 2020 5d0d 0a20 2020 207d 2c0d 0a20      ]..    },.. 
-00000c00: 2020 207b 0d0a 2020 2020 2020 2263 656c     {..      "cel
-00000c10: 6c5f 7479 7065 223a 2022 6d61 726b 646f  l_type": "markdo
-00000c20: 776e 222c 0d0a 2020 2020 2020 226d 6574  wn",..      "met
-00000c30: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
-00000c40: 2020 2022 736f 7572 6365 223a 205b 0d0a     "source": [..
-00000c50: 2020 2020 2020 2020 2257 6520 6361 6e20          "We can 
-00000c60: 6361 6c63 756c 6174 6520 616e 6420 706c  calculate and pl
-00000c70: 6f74 2074 6865 2070 6172 7469 7469 6f6e  ot the partition
-00000c80: 696e 6720 6f66 2024 585e 7b32 2b7d 2420  ing of $X^{2+}$ 
-00000c90: 6361 7469 6f6e 7320 7265 6c61 7469 7665  cations relative
-00000ca0: 2074 6f5c 6e24 4361 5e7b 322b 7d24 2061   to\n$Ca^{2+}$ a
-00000cb0: 7420 6120 6769 7665 6e20 7465 6d70 6572  t a given temper
-00000cc0: 6174 7572 6520 7573 696e 6720 7468 6569  ature using thei
-00000cd0: 7220 7261 6469 6920 616e 6420 7468 6520  r radii and the 
-00000ce0: 6c61 7474 6963 6520 7374 7261 696e 2066  lattice strain f
-00000cf0: 756e 6374 696f 6e3a 5c6e 5c6e 5c6e 220d  unction:\n\n\n".
-00000d00: 0a20 2020 2020 205d 0d0a 2020 2020 7d2c  .      ]..    },
-00000d10: 0d0a 2020 2020 7b0d 0a20 2020 2020 2022  ..    {..      "
-00000d20: 6365 6c6c 5f74 7970 6522 3a20 2263 6f64  cell_type": "cod
-00000d30: 6522 2c0d 0a20 2020 2020 2022 6578 6563  e",..      "exec
-00000d40: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
-00000d50: 6c6c 2c0d 0a20 2020 2020 2022 6d65 7461  ll,..      "meta
-00000d60: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
-00000d70: 2020 2263 6f6c 6c61 7073 6564 223a 2066    "collapsed": f
-00000d80: 616c 7365 0d0a 2020 2020 2020 7d2c 0d0a  alse..      },..
-00000d90: 2020 2020 2020 226f 7574 7075 7473 223a        "outputs":
-00000da0: 205b 5d2c 0d0a 2020 2020 2020 2273 6f75   [],..      "sou
-00000db0: 7263 6522 3a20 5b0d 0a20 2020 2020 2020  rce": [..       
-00000dc0: 2022 666f 6e74 7369 7a65 203d 2038 5c6e   "fontsize = 8\n
-00000dd0: 6669 672c 2061 7820 3d20 706c 742e 7375  fig, ax = plt.su
-00000de0: 6270 6c6f 7473 2831 295c 6e5c 6e73 6974  bplots(1)\n\nsit
-00000df0: 6532 6c61 6265 6c73 203d 205b 5c22 4e61  e2labels = [\"Na
-00000e00: 5c22 2c20 5c22 4361 5c22 2c20 5c22 4575  \", \"Ca\", \"Eu
-00000e10: 5c22 2c20 5c22 5372 5c22 5d5c 6e23 2067  \", \"Sr\"]\n# g
-00000e20: 6574 2074 6865 2053 6861 6e6e 6f6e 2069  et the Shannon i
-00000e30: 6f6e 6963 2072 6164 6969 2066 6f72 2074  onic radii for t
-00000e40: 6865 2065 6c65 6d65 6e74 7320 696e 2074  he elements in t
-00000e50: 6865 2032 2b20 7369 7465 5c6e 7369 7465  he 2+ site\nsite
-00000e60: 3272 6164 6969 203d 205b 5c6e 2020 2020  2radii = [\n    
-00000e70: 6765 745f 696f 6e69 635f 7261 6469 6928  get_ionic_radii(
-00000e80: 5c22 4e61 5c22 2c20 6368 6172 6765 3d31  \"Na\", charge=1
-00000e90: 2c20 636f 6f72 6469 6e61 7469 6f6e 3d38  , coordination=8
-00000ea0: 292c 5c6e 2020 2020 2a5b 6765 745f 696f  ),\n    *[get_io
-00000eb0: 6e69 635f 7261 6469 6928 656c 2c20 6368  nic_radii(el, ch
-00000ec0: 6172 6765 3d32 2c20 636f 6f72 6469 6e61  arge=2, coordina
-00000ed0: 7469 6f6e 3d38 2920 666f 7220 656c 2069  tion=8) for el i
-00000ee0: 6e20 5b5c 2243 615c 222c 205c 2245 755c  n [\"Ca\", \"Eu\
-00000ef0: 222c 205c 2253 725c 225d 5d2c 5c6e 5d5c  ", \"Sr\"]],\n]\
-00000f00: 6e23 2070 6c6f 7420 7468 6520 7265 6c61  n# plot the rela
-00000f10: 7469 7665 2070 6172 6974 696f 6e69 6e67  tive paritioning
-00000f20: 2063 7572 7665 2066 6f72 2063 6174 696f   curve for catio
-00000f30: 6e73 2069 6e20 7468 6520 322b 2073 6974  ns in the 2+ sit
-00000f40: 655c 6e73 6974 6532 4473 203d 2044 5f43  e\nsite2Ds = D_C
-00000f50: 6120 2a20 6e70 2e61 7272 6179 285c 6e20  a * np.array(\n 
-00000f60: 2020 205b 7374 7261 696e 5f63 6f65 6666     [strain_coeff
-00000f70: 6963 6965 6e74 2872 4361 2c20 7278 2c20  icient(rCa, rx, 
-00000f80: 7230 3d72 3032 2c20 453d 455f 322c 2054  r0=r02, E=E_2, T
-00000f90: 3d54 6b29 2066 6f72 2072 7820 696e 2073  =Tk) for rx in s
-00000fa0: 6974 6532 7261 6469 695d 5c6e 295c 6e61  ite2radii]\n)\na
-00000fb0: 782e 7363 6174 7465 7228 7369 7465 3272  x.scatter(site2r
-00000fc0: 6164 6969 2c20 7369 7465 3244 732c 2063  adii, site2Ds, c
-00000fd0: 6f6c 6f72 3d5c 2267 5c22 2c20 6c61 6265  olor=\"g\", labe
-00000fe0: 6c3d 5c22 2458 5e7b 322b 7d24 2043 6174  l=\"$X^{2+}$ Cat
-00000ff0: 696f 6e73 5c22 295c 6e23 2063 7265 6174  ions\")\n# creat
-00001000: 6520 616e 2069 6e64 6578 206f 6620 7261  e an index of ra
-00001010: 6469 692c 2061 6e64 2070 6c6f 7420 7468  dii, and plot th
-00001020: 6520 7265 6c61 7469 7665 2070 6172 6974  e relative parit
-00001030: 696f 6e69 6e67 2063 7572 7665 2066 6f72  ioning curve for
-00001040: 2074 6865 2073 6974 655c 6e78 7320 3d20   the site\nxs = 
-00001050: 6e70 2e6c 696e 7370 6163 6528 302e 392c  np.linspace(0.9,
-00001060: 2031 2e33 2c20 3230 3029 5c6e 6375 7276   1.3, 200)\ncurv
-00001070: 6532 4473 203d 2044 5f43 6120 2a20 7374  e2Ds = D_Ca * st
-00001080: 7261 696e 5f63 6f65 6666 6963 6965 6e74  rain_coefficient
-00001090: 2872 4361 2c20 7873 2c20 7230 3d72 3032  (rCa, xs, r0=r02
-000010a0: 2c20 453d 455f 322c 2054 3d54 6b29 5c6e  , E=E_2, T=Tk)\n
-000010b0: 6178 2e70 6c6f 7428 7873 2c20 6375 7276  ax.plot(xs, curv
-000010c0: 6532 4473 2c20 636f 6c6f 723d 5c22 302e  e2Ds, color=\"0.
-000010d0: 355c 222c 206c 733d 5c22 2d2d 5c22 295c  5\", ls=\"--\")\
-000010e0: 6e23 2061 6464 2074 6865 2065 6c65 6d65  n# add the eleme
-000010f0: 6e74 206c 6162 656c 7320 6e65 7874 2074  nt labels next t
-00001100: 6f20 7468 6520 706f 696e 7473 5c6e 666f  o the points\nfo
-00001110: 7220 6c2c 2072 2c20 6420 696e 207a 6970  r l, r, d in zip
-00001120: 2873 6974 6532 6c61 6265 6c73 2c20 7369  (site2labels, si
-00001130: 7465 3272 6164 6969 2c20 7369 7465 3244  te2radii, site2D
-00001140: 7329 3a5c 6e20 2020 2061 782e 616e 6e6f  s):\n    ax.anno
-00001150: 7461 7465 285c 6e20 2020 2020 2020 206c  tate(\n        l
-00001160: 2c20 7879 3d28 722c 2064 292c 2078 7963  , xy=(r, d), xyc
-00001170: 6f6f 7264 733d 5c22 6461 7461 5c22 2c20  oords=\"data\", 
-00001180: 6861 3d5c 226c 6566 745c 222c 2076 613d  ha=\"left\", va=
-00001190: 5c22 626f 7474 6f6d 5c22 2c20 666f 6e74  \"bottom\", font
-000011a0: 7369 7a65 3d66 6f6e 7473 697a 655c 6e20  size=fontsize\n 
-000011b0: 2020 2029 5c6e 6669 6722 0d0a 2020 2020     )\nfig"..    
-000011c0: 2020 5d0d 0a20 2020 207d 2c0d 0a20 2020    ]..    },..   
-000011d0: 207b 0d0a 2020 2020 2020 2263 656c 6c5f   {..      "cell_
-000011e0: 7479 7065 223a 2022 6d61 726b 646f 776e  type": "markdown
-000011f0: 222c 0d0a 2020 2020 2020 226d 6574 6164  ",..      "metad
-00001200: 6174 6122 3a20 7b7d 2c0d 0a20 2020 2020  ata": {},..     
-00001210: 2022 736f 7572 6365 223a 205b 0d0a 2020   "source": [..  
-00001220: 2020 2020 2020 2257 6865 6e20 6974 2063        "When it c
-00001230: 6f6d 6573 2074 6f20 6573 7469 6d61 7469  omes to estimati
-00001240: 6e67 2074 6865 2070 6172 7469 7469 6f6e  ng the partition
-00001250: 696e 6720 6f66 2024 585e 7b33 2b7d 2420  ing of $X^{3+}$ 
-00001260: 6361 7469 6f6e 732c 2077 6527 6c6c 206e  cations, we'll n
-00001270: 6565 6420 6120 7265 6665 7265 6e63 655c  eed a reference\
-00001280: 6e70 6f69 6e74 202d 2068 6572 6520 7765  npoint - here we
-00001290: 276c 6c20 7573 6520 2444 5f7b 4c61 7d24  'll use $D_{La}$
-000012a0: 2074 6f20 6361 6c63 756c 6174 6520 7265   to calculate re
-000012b0: 6c61 7469 7665 2070 6172 7469 7469 6f6e  lative partition
-000012c0: 696e 6720 6f66 2074 6865 206f 7468 6572  ing of the other
-000012d0: 5c6e 5261 7265 2045 6172 7468 2045 6c65  \nRare Earth Ele
-000012e0: 6d65 6e74 732c 2061 6c74 686f 7567 6820  ments, although 
-000012f0: 796f 7520 6d61 7920 6861 7665 206e 6f74  you may have not
-00001300: 6963 6564 2069 7420 6973 206e 6f74 2064  iced it is not d
-00001310: 6566 696e 6564 2061 626f 7665 2e5c 6e54  efined above.\nT
-00001320: 6872 6f75 6768 2061 2068 616e 6479 2072  hrough a handy r
-00001330: 656c 6174 696f 6e73 6869 702c 2077 6520  elationship, we 
-00001340: 6361 6e20 6573 7469 6d61 7465 2024 445f  can estimate $D_
-00001350: 7b4c 617d 245c 6e62 6173 6564 206f 6e20  {La}$\nbased on 
-00001360: 7468 6520 6561 7369 6572 206d 6561 7375  the easier measu
-00001370: 7265 6420 2444 5f7b 4361 7d24 2c20 2444  red $D_{Ca}$, $D
-00001380: 5f7b 4e61 7d24 2061 6e64 2074 656d 7065  _{Na}$ and tempe
-00001390: 7261 7475 7265 205b 2372 6566 5f32 5d5f  rature [#ref_2]_
-000013a0: 3a5c 6e5c 6e5c 6e22 0d0a 2020 2020 2020  :\n\n\n"..      
-000013b0: 5d0d 0a20 2020 207d 2c0d 0a20 2020 207b  ]..    },..    {
-000013c0: 0d0a 2020 2020 2020 2263 656c 6c5f 7479  ..      "cell_ty
-000013d0: 7065 223a 2022 636f 6465 222c 0d0a 2020  pe": "code",..  
-000013e0: 2020 2020 2265 7865 6375 7469 6f6e 5f63      "execution_c
-000013f0: 6f75 6e74 223a 206e 756c 6c2c 0d0a 2020  ount": null,..  
-00001400: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
-00001410: 7b0d 0a20 2020 2020 2020 2022 636f 6c6c  {..        "coll
-00001420: 6170 7365 6422 3a20 6661 6c73 650d 0a20  apsed": false.. 
-00001430: 2020 2020 207d 2c0d 0a20 2020 2020 2022       },..      "
-00001440: 6f75 7470 7574 7322 3a20 5b5d 2c0d 0a20  outputs": [],.. 
-00001450: 2020 2020 2022 736f 7572 6365 223a 205b       "source": [
-00001460: 0d0a 2020 2020 2020 2020 2244 5f4c 6120  ..        "D_La 
-00001470: 3d20 2844 5f43 6120 2a2a 2032 202f 2044  = (D_Ca ** 2 / D
-00001480: 5f4e 6129 202a 206e 702e 6578 7028 2835  _Na) * np.exp((5
-00001490: 3239 202f 2054 6b29 202d 2033 2e37 3035  29 / Tk) - 3.705
-000014a0: 295c 6e44 5f4c 6120 2023 2030 2e34 3830  )\nD_La  # 0.480
-000014b0: 3835 220d 0a20 2020 2020 205d 0d0a 2020  85"..      ]..  
-000014c0: 2020 7d2c 0d0a 2020 2020 7b0d 0a20 2020    },..    {..   
-000014d0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
-000014e0: 226d 6172 6b64 6f77 6e22 2c0d 0a20 2020  "markdown",..   
-000014f0: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-00001500: 7d2c 0d0a 2020 2020 2020 2273 6f75 7263  },..      "sourc
-00001510: 6522 3a20 5b0d 0a20 2020 2020 2020 2022  e": [..        "
-00001520: 4e6f 7720 2444 5f7b 4c61 7d24 2069 7320  Now $D_{La}$ is 
-00001530: 6465 6669 6e65 642c 2077 6520 6361 6e20  defined, we can 
-00001540: 7573 6520 6974 2061 7320 6120 7265 6665  use it as a refe
-00001550: 7265 6e63 6520 666f 7220 7468 6520 6f74  rence for the ot
-00001560: 6865 7220 5245 453a 5c6e 5c6e 5c6e 220d  her REE:\n\n\n".
-00001570: 0a20 2020 2020 205d 0d0a 2020 2020 7d2c  .      ]..    },
-00001580: 0d0a 2020 2020 7b0d 0a20 2020 2020 2022  ..    {..      "
-00001590: 6365 6c6c 5f74 7970 6522 3a20 2263 6f64  cell_type": "cod
-000015a0: 6522 2c0d 0a20 2020 2020 2022 6578 6563  e",..      "exec
-000015b0: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
-000015c0: 6c6c 2c0d 0a20 2020 2020 2022 6d65 7461  ll,..      "meta
-000015d0: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
-000015e0: 2020 2263 6f6c 6c61 7073 6564 223a 2066    "collapsed": f
-000015f0: 616c 7365 0d0a 2020 2020 2020 7d2c 0d0a  alse..      },..
-00001600: 2020 2020 2020 226f 7574 7075 7473 223a        "outputs":
-00001610: 205b 5d2c 0d0a 2020 2020 2020 2273 6f75   [],..      "sou
-00001620: 7263 6522 3a20 5b0d 0a20 2020 2020 2020  rce": [..       
-00001630: 2022 7369 7465 336c 6162 656c 7320 3d20   "site3labels = 
-00001640: 5245 4528 6472 6f70 506d 3d54 7275 6529  REE(dropPm=True)
-00001650: 5c6e 2320 6765 7420 7468 6520 5368 616e  \n# get the Shan
-00001660: 6e6f 6e20 696f 6e69 6320 7261 6469 6920  non ionic radii 
-00001670: 666f 7220 7468 6520 656c 656d 656e 7473  for the elements
-00001680: 2069 6e20 7468 6520 332b 2073 6974 655c   in the 3+ site\
-00001690: 6e73 6974 6533 7261 6469 6920 3d20 5b67  nsite3radii = [g
-000016a0: 6574 5f69 6f6e 6963 5f72 6164 6969 2878  et_ionic_radii(x
-000016b0: 2c20 6368 6172 6765 3d33 2c20 636f 6f72  , charge=3, coor
-000016c0: 6469 6e61 7469 6f6e 3d38 2920 666f 7220  dination=8) for 
-000016d0: 7820 696e 2052 4545 2864 726f 7050 6d3d  x in REE(dropPm=
-000016e0: 5472 7565 295d 5c6e 7369 7465 3344 7320  True)]\nsite3Ds 
-000016f0: 3d20 445f 4c61 202a 206e 702e 6172 7261  = D_La * np.arra
-00001700: 7928 5c6e 2020 2020 5b73 7472 6169 6e5f  y(\n    [strain_
-00001710: 636f 6566 6669 6369 656e 7428 724c 612c  coefficient(rLa,
-00001720: 2072 782c 2072 303d 7230 332c 2045 3d45   rx, r0=r03, E=E
-00001730: 5f33 2c20 543d 546b 2920 666f 7220 7278  _3, T=Tk) for rx
-00001740: 2069 6e20 7369 7465 3372 6164 6969 5d5c   in site3radii]\
-00001750: 6e29 5c6e 2320 706c 6f74 2074 6865 2072  n)\n# plot the r
-00001760: 656c 6174 6976 6520 7061 7269 7469 6f6e  elative parition
-00001770: 696e 6720 6375 7276 6520 666f 7220 6361  ing curve for ca
-00001780: 7469 6f6e 7320 696e 2074 6865 2033 2b20  tions in the 3+ 
-00001790: 7369 7465 5c6e 6178 2e73 6361 7474 6572  site\nax.scatter
-000017a0: 2873 6974 6533 7261 6469 692c 2073 6974  (site3radii, sit
-000017b0: 6533 4473 2c20 636f 6c6f 723d 5c22 7075  e3Ds, color=\"pu
-000017c0: 7270 6c65 5c22 2c20 6c61 6265 6c3d 5c22  rple\", label=\"
-000017d0: 2458 5e7b 332b 7d24 2043 6174 696f 6e73  $X^{3+}$ Cations
-000017e0: 5c22 295c 6e23 2070 6c6f 7420 7468 6520  \")\n# plot the 
-000017f0: 7265 6c61 7469 7665 2070 6172 6974 696f  relative paritio
-00001800: 6e69 6e67 2063 7572 7665 2066 6f72 2074  ning curve for t
-00001810: 6865 2073 6974 655c 6e63 7572 7665 3344  he site\ncurve3D
-00001820: 7320 3d20 445f 4c61 202a 2073 7472 6169  s = D_La * strai
-00001830: 6e5f 636f 6566 6669 6369 656e 7428 724c  n_coefficient(rL
-00001840: 612c 2078 732c 2072 303d 7230 332c 2045  a, xs, r0=r03, E
-00001850: 3d45 5f33 2c20 543d 546b 295c 6e61 782e  =E_3, T=Tk)\nax.
-00001860: 706c 6f74 2878 732c 2063 7572 7665 3344  plot(xs, curve3D
-00001870: 732c 2063 6f6c 6f72 3d5c 2230 2e35 5c22  s, color=\"0.5\"
-00001880: 2c20 6c73 3d5c 222d 2d5c 2229 5c6e 2320  , ls=\"--\")\n# 
-00001890: 6164 6420 7468 6520 656c 656d 656e 7420  add the element 
-000018a0: 6c61 6265 6c73 206e 6578 7420 746f 2074  labels next to t
-000018b0: 6865 2070 6f69 6e74 735c 6e66 6f72 206c  he points\nfor l
-000018c0: 2c20 722c 2064 2069 6e20 7a69 7028 7369  , r, d in zip(si
-000018d0: 7465 336c 6162 656c 732c 2073 6974 6533  te3labels, site3
-000018e0: 7261 6469 692c 2073 6974 6533 4473 293a  radii, site3Ds):
-000018f0: 5c6e 2020 2020 6178 2e61 6e6e 6f74 6174  \n    ax.annotat
-00001900: 6528 5c6e 2020 2020 2020 2020 6c2c 2078  e(\n        l, x
-00001910: 793d 2872 2c20 6429 2c20 7879 636f 6f72  y=(r, d), xycoor
-00001920: 6473 3d5c 2264 6174 615c 222c 2068 613d  ds=\"data\", ha=
-00001930: 5c22 7269 6768 745c 222c 2076 613d 5c22  \"right\", va=\"
-00001940: 626f 7474 6f6d 5c22 2c20 666f 6e74 7369  bottom\", fontsi
-00001950: 7a65 3d66 6f6e 7473 697a 655c 6e20 2020  ze=fontsize\n   
-00001960: 2029 5c6e 6178 2e73 6574 5f79 7363 616c   )\nax.set_yscal
-00001970: 6528 5c22 6c6f 675c 2229 5c6e 6178 2e73  e(\"log\")\nax.s
-00001980: 6574 5f79 6c61 6265 6c28 5c22 2444 5f58  et_ylabel(\"$D_X
-00001990: 245c 2229 5c6e 6178 2e73 6574 5f78 6c61  $\")\nax.set_xla
-000019a0: 6265 6c28 5c22 5261 6469 6920 2824 5c5c  bel(\"Radii ($\\
-000019b0: 4141 2429 5c22 295c 6e66 6967 220d 0a20  AA$)\")\nfig".. 
-000019c0: 2020 2020 205d 0d0a 2020 2020 7d2c 0d0a       ]..    },..
-000019d0: 2020 2020 7b0d 0a20 2020 2020 2022 6365      {..      "ce
-000019e0: 6c6c 5f74 7970 6522 3a20 226d 6172 6b64  ll_type": "markd
-000019f0: 6f77 6e22 2c0d 0a20 2020 2020 2022 6d65  own",..      "me
-00001a00: 7461 6461 7461 223a 207b 7d2c 0d0a 2020  tadata": {},..  
-00001a10: 2020 2020 2273 6f75 7263 6522 3a20 5b0d      "source": [.
-00001a20: 0a20 2020 2020 2020 2022 4173 2065 7572  .        "As eur
-00001a30: 6f70 6975 6d20 6973 2063 6f6d 6d6f 6e6c  opium is commonl
-00001a40: 7920 7072 6573 656e 7420 6173 2061 206d  y present as a m
-00001a50: 6978 7475 7265 206f 6620 626f 7468 2024  ixture of both $
-00001a60: 4575 5e7b 322b 7d24 5c6e 616e 6420 2445  Eu^{2+}$\nand $E
-00001a70: 755e 7b33 2b7d 242c 2074 6865 2065 6666  u^{3+}$, the eff
-00001a80: 6563 7469 7665 2070 6172 7469 7469 6f6e  ective partition
-00001a90: 696e 6720 6f66 2045 7520 7769 6c6c 2062  ing of Eu will b
-00001aa0: 6520 696e 7465 726d 6564 6961 7465 5c6e  e intermediate\n
-00001ab0: 6265 7477 6565 6e20 7468 6174 206f 6620  between that of 
-00001ac0: 2444 5f7b 4575 5e7b 322b 7d7d 2461 6e64  $D_{Eu^{2+}}$and
-00001ad0: 2024 445f 7b45 755e 7b33 2b7d 7d24 2e20   $D_{Eu^{3+}}$. 
-00001ae0: 5573 696e 6720 6120 3630 3a34 3020 6d69  Using a 60:40 mi
-00001af0: 7874 7572 655c 6e6f 6620 2445 755e 7b33  xture\nof $Eu^{3
-00001b00: 2b7d 2420 3a20 2445 755e 7b32 2b7d 2420  +}$ : $Eu^{2+}$ 
-00001b10: 6173 2061 6e20 6578 616d 706c 652c 2074  as an example, t
-00001b20: 6869 7320 6566 6665 6374 6976 6520 7061  his effective pa
-00001b30: 7274 6974 696f 6e5c 6e63 6f65 6666 6963  rtition\ncoeffic
-00001b40: 6965 6e74 2063 616e 2062 6520 6361 6c63  ient can be calc
-00001b50: 756c 6174 6564 3a5c 6e5c 6e5c 6e22 0d0a  ulated:\n\n\n"..
-00001b60: 2020 2020 2020 5d0d 0a20 2020 207d 2c0d        ]..    },.
-00001b70: 0a20 2020 207b 0d0a 2020 2020 2020 2263  .    {..      "c
-00001b80: 656c 6c5f 7479 7065 223a 2022 636f 6465  ell_type": "code
-00001b90: 222c 0d0a 2020 2020 2020 2265 7865 6375  ",..      "execu
-00001ba0: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
-00001bb0: 6c2c 0d0a 2020 2020 2020 226d 6574 6164  l,..      "metad
-00001bc0: 6174 6122 3a20 7b0d 0a20 2020 2020 2020  ata": {..       
-00001bd0: 2022 636f 6c6c 6170 7365 6422 3a20 6661   "collapsed": fa
-00001be0: 6c73 650d 0a20 2020 2020 207d 2c0d 0a20  lse..      },.. 
-00001bf0: 2020 2020 2022 6f75 7470 7574 7322 3a20       "outputs": 
-00001c00: 5b5d 2c0d 0a20 2020 2020 2022 736f 7572  [],..      "sour
-00001c10: 6365 223a 205b 0d0a 2020 2020 2020 2020  ce": [..        
-00001c20: 2258 5f45 7533 203d 2030 2e36 5c6e 2320  "X_Eu3 = 0.6\n# 
-00001c30: 6361 6c63 756c 6174 6520 445f 4575 3320  calculate D_Eu3 
-00001c40: 7265 6c61 7469 7665 2074 6f20 445f 4c61  relative to D_La
-00001c50: 5c6e 445f 4575 3320 3d20 445f 4c61 202a  \nD_Eu3 = D_La *
-00001c60: 2073 7472 6169 6e5f 636f 6566 6669 6369   strain_coeffici
-00001c70: 656e 7428 5c6e 2020 2020 724c 612c 2067  ent(\n    rLa, g
-00001c80: 6574 5f69 6f6e 6963 5f72 6164 6969 285c  et_ionic_radii(\
-00001c90: 2245 755c 222c 2063 6861 7267 653d 332c  "Eu\", charge=3,
-00001ca0: 2063 6f6f 7264 696e 6174 696f 6e3d 3829   coordination=8)
-00001cb0: 2c20 7230 3d72 3033 2c20 453d 455f 332c  , r0=r03, E=E_3,
-00001cc0: 2054 3d54 6b5c 6e29 5c6e 2320 6361 6c63   T=Tk\n)\n# calc
-00001cd0: 756c 6174 6520 445f 4575 3220 7265 6c61  ulate D_Eu2 rela
-00001ce0: 7469 7665 2074 6f20 445f 4361 5c6e 445f  tive to D_Ca\nD_
-00001cf0: 4575 3220 3d20 445f 4361 202a 2073 7472  Eu2 = D_Ca * str
-00001d00: 6169 6e5f 636f 6566 6669 6369 656e 7428  ain_coefficient(
-00001d10: 5c6e 2020 2020 7243 612c 2067 6574 5f69  \n    rCa, get_i
-00001d20: 6f6e 6963 5f72 6164 6969 285c 2245 755c  onic_radii(\"Eu\
-00001d30: 222c 2063 6861 7267 653d 322c 2063 6f6f  ", charge=2, coo
-00001d40: 7264 696e 6174 696f 6e3d 3829 2c20 7230  rdination=8), r0
-00001d50: 3d72 3032 2c20 453d 455f 322c 2054 3d54  =r02, E=E_2, T=T
-00001d60: 6b5c 6e29 5c6e 2320 6361 6c63 756c 6174  k\n)\n# calculat
-00001d70: 6520 7468 6520 6566 6665 6374 6976 6520  e the effective 
-00001d80: 7061 7269 7469 6f6e 2063 6f65 6666 6963  parition coeffic
-00001d90: 6965 6e74 5c6e 445f 4575 203d 2028 3120  ient\nD_Eu = (1 
-00001da0: 2d20 585f 4575 3329 202a 2044 5f45 7532  - X_Eu3) * D_Eu2
-00001db0: 202b 2058 5f45 7533 202a 2044 5f45 7533   + X_Eu3 * D_Eu3
-00001dc0: 5c6e 2320 7368 6f77 2074 6865 2065 6666  \n# show the eff
-00001dd0: 6563 7469 7665 2070 6172 7469 7469 6f6e  ective partition
-00001de0: 2063 6f65 6666 6963 6965 6e74 2072 656c   coefficient rel
-00001df0: 6174 6976 6520 746f 2074 6865 2032 2b20  ative to the 2+ 
-00001e00: 616e 6420 332b 2065 6e64 6d65 6d62 6572  and 3+ endmember
-00001e10: 735c 6e72 6164 6969 2c20 6473 203d 2028  s\nradii, ds = (
-00001e20: 5c6e 2020 2020 5b67 6574 5f69 6f6e 6963  \n    [get_ionic
-00001e30: 5f72 6164 6969 285c 2245 755c 222c 2063  _radii(\"Eu\", c
-00001e40: 6861 7267 653d 632c 2063 6f6f 7264 696e  harge=c, coordin
-00001e50: 6174 696f 6e3d 3829 2066 6f72 2063 2069  ation=8) for c i
-00001e60: 6e20 5b33 2c20 332c 2032 2c20 325d 5d2c  n [3, 3, 2, 2]],
-00001e70: 5c6e 2020 2020 5b44 5f45 7533 2c20 445f  \n    [D_Eu3, D_
-00001e80: 4575 2c20 445f 4575 2c20 445f 4575 325d  Eu, D_Eu, D_Eu2]
-00001e90: 2c5c 6e29 5c6e 6178 2e70 6c6f 7428 5c6e  ,\n)\nax.plot(\n
-00001ea0: 2020 2020 7261 6469 692c 2064 732c 206c      radii, ds, l
-00001eb0: 733d 5c22 2d2d 5c22 2c20 636f 6c6f 723d  s=\"--\", color=
-00001ec0: 5c22 302e 395c 222c 206d 6172 6b65 723d  \"0.9\", marker=
-00001ed0: 5c22 445c 222c 206c 6162 656c 3d5c 2245  \"D\", label=\"E
-00001ee0: 6666 6563 7469 7665 2024 445f 7b45 757d  ffective $D_{Eu}
-00001ef0: 245c 222c 207a 6f72 6465 723d 2d31 5c6e  $\", zorder=-1\n
-00001f00: 295c 6e61 782e 6c65 6765 6e64 286c 6f63  )\nax.legend(loc
-00001f10: 3d5c 2275 7070 6572 206c 6566 745c 222c  =\"upper left\",
-00001f20: 2062 626f 785f 746f 5f61 6e63 686f 723d   bbox_to_anchor=
-00001f30: 2831 2e30 352c 2031 292c 2066 7261 6d65  (1.05, 1), frame
-00001f40: 6f6e 3d46 616c 7365 2c20 6661 6365 636f  on=False, faceco
-00001f50: 6c6f 723d 4e6f 6e65 295c 6e66 6967 220d  lor=None)\nfig".
-00001f60: 0a20 2020 2020 205d 0d0a 2020 2020 7d2c  .      ]..    },
-00001f70: 0d0a 2020 2020 7b0d 0a20 2020 2020 2022  ..    {..      "
-00001f80: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-00001f90: 6b64 6f77 6e22 2c0d 0a20 2020 2020 2022  kdown",..      "
-00001fa0: 6d65 7461 6461 7461 223a 207b 7d2c 0d0a  metadata": {},..
-00001fb0: 2020 2020 2020 2273 6f75 7263 6522 3a20        "source": 
-00001fc0: 5b0d 0a20 2020 2020 2020 2022 2e2e 205b  [..        ".. [
-00001fd0: 2372 6566 5f31 5d20 426c 756e 6479 2c20  #ref_1] Blundy, 
-00001fe0: 4a2e 2c20 576f 6f64 2c20 422e 2c20 3139  J., Wood, B., 19
-00001ff0: 3934 2e20 5072 6564 6963 7469 6f6e 206f  94. Prediction o
-00002000: 6620 6372 7973 7461 6c5c 7532 3031 336d  f crystal\u2013m
-00002010: 656c 7420 7061 7274 6974 696f 6e20 636f  elt partition co
-00002020: 6566 6669 6369 656e 7473 5c6e 2020 2020  efficients\n    
-00002030: 2020 2020 2020 2020 6672 6f6d 2065 6c61          from ela
-00002040: 7374 6963 206d 6f64 756c 692e 204e 6174  stic moduli. Nat
-00002050: 7572 6520 3337 322c 2034 3532 2e5c 6e20  ure 372, 452.\n 
-00002060: 2020 2020 2020 2020 2020 2064 6f69 3a20             doi: 
-00002070: 6031 302e 3130 3338 2f33 3732 3435 3241  `10.1038/372452A
-00002080: 3020 3c68 7474 7073 3a2f 2f64 6f69 2e6f  0 <https://doi.o
-00002090: 7267 2f31 302e 3130 3338 2f33 3732 3435  rg/10.1038/37245
-000020a0: 3241 303e 605f 5f5c 6e5c 6e2e 2e20 5b23  2A0>`__\n\n.. [#
-000020b0: 7265 665f 325d 2044 6f68 6d65 6e2c 2052  ref_2] Dohmen, R
-000020c0: 2e2c 2042 6c75 6e64 792c 204a 2e2c 2032  ., Blundy, J., 2
-000020d0: 3031 342e 2041 2070 7265 6469 6374 6976  014. A predictiv
-000020e0: 6520 7468 6572 6d6f 6479 6e61 6d69 6320  e thermodynamic 
-000020f0: 6d6f 6465 6c20 666f 7220 656c 656d 656e  model for elemen
-00002100: 7420 7061 7274 6974 696f 6e69 6e67 5c6e  t partitioning\n
-00002110: 2020 2020 2020 2020 2020 2020 6265 7477              betw
-00002120: 6565 6e20 706c 6167 696f 636c 6173 6520  een plagioclase 
-00002130: 616e 6420 6d65 6c74 2061 7320 6120 6675  and melt as a fu
-00002140: 6e63 7469 6f6e 206f 6620 7072 6573 7375  nction of pressu
-00002150: 7265 2c20 7465 6d70 6572 6174 7572 6520  re, temperature 
-00002160: 616e 6420 636f 6d70 6f73 6974 696f 6e2e  and composition.
-00002170: 5c6e 2020 2020 2020 2020 2020 2020 416d  \n            Am
-00002180: 6572 6963 616e 204a 6f75 726e 616c 206f  erican Journal o
-00002190: 6620 5363 6965 6e63 6520 3331 342c 2031  f Science 314, 1
-000021a0: 3331 395c 7532 3031 3331 3337 322e 5c6e  319\u20131372.\n
-000021b0: 2020 2020 2020 2020 2020 2020 646f 693a              doi:
-000021c0: 2060 3130 2e32 3437 352f 3039 2e32 3031   `10.2475/09.201
-000021d0: 342e 3034 203c 6874 7470 733a 2f2f 646f  4.04 <https://do
-000021e0: 692e 6f72 672f 3130 2e32 3437 352f 3039  i.org/10.2475/09
-000021f0: 2e32 3031 342e 3034 3e60 5f5f 5c6e 5c6e  .2014.04>`__\n\n
-00002200: 2e2e 2073 6565 616c 736f 3a3a 5c6e 5c6e  .. seealso::\n\n
-00002210: 2020 4578 616d 706c 6573 3a5c 6e20 2020    Examples:\n   
-00002220: 2060 5368 616e 6e6f 6e20 5261 6469 6920   `Shannon Radii 
-00002230: 3c2e 2e2f 696e 6465 7865 732f 7368 616e  <../indexes/shan
-00002240: 6e6f 6e2e 6874 6d6c 3e60 5f5f 2c5c 6e20  non.html>`__,\n 
-00002250: 2020 2060 5245 4520 5261 6469 6920 506c     `REE Radii Pl
-00002260: 6f74 203c 2e2e 2f70 6c6f 7474 696e 672f  ot <../plotting/
-00002270: 5245 455f 765f 7261 6469 692e 6874 6d6c  REE_v_radii.html
-00002280: 3e60 5f5f 5c6e 5c6e 2020 4675 6e63 7469  >`__\n\n  Functi
-00002290: 6f6e 733a 5c6e 2020 2020 3a66 756e 633a  ons:\n    :func:
-000022a0: 607e 7079 726f 6c69 7465 2e6d 696e 6572  `~pyrolite.miner
-000022b0: 616c 2e6c 6174 7469 6365 2e73 7472 6169  al.lattice.strai
-000022c0: 6e5f 636f 6566 6669 6369 656e 7460 2c5c  n_coefficient`,\
-000022d0: 6e20 2020 203a 6675 6e63 3a60 7e70 7972  n    :func:`~pyr
-000022e0: 6f6c 6974 652e 6d69 6e65 7261 6c2e 6c61  olite.mineral.la
-000022f0: 7474 6963 652e 796f 756e 6773 5f6d 6f64  ttice.youngs_mod
-00002300: 756c 7573 5f61 7070 726f 7869 6d61 7469  ulus_approximati
-00002310: 6f6e 602c 5c6e 2020 2020 3a66 756e 633a  on`,\n    :func:
-00002320: 607e 7079 726f 6c69 7465 2e67 656f 6368  `~pyrolite.geoch
-00002330: 656d 2e67 6574 5f69 6f6e 6963 5f72 6164  em.get_ionic_rad
-00002340: 6969 605c 6e5c 6e22 0d0a 2020 2020 2020  ii`\n\n"..      
-00002350: 5d0d 0a20 2020 207d 0d0a 2020 5d2c 0d0a  ]..    }..  ],..
-00002360: 2020 226d 6574 6164 6174 6122 3a20 7b0d    "metadata": {.
-00002370: 0a20 2020 2022 6b65 726e 656c 7370 6563  .    "kernelspec
-00002380: 223a 207b 0d0a 2020 2020 2020 2264 6973  ": {..      "dis
-00002390: 706c 6179 5f6e 616d 6522 3a20 2250 7974  play_name": "Pyt
-000023a0: 686f 6e20 3322 2c0d 0a20 2020 2020 2022  hon 3",..      "
-000023b0: 6c61 6e67 7561 6765 223a 2022 7079 7468  language": "pyth
-000023c0: 6f6e 222c 0d0a 2020 2020 2020 226e 616d  on",..      "nam
-000023d0: 6522 3a20 2270 7974 686f 6e33 220d 0a20  e": "python3".. 
-000023e0: 2020 207d 2c0d 0a20 2020 2022 6c61 6e67     },..    "lang
-000023f0: 7561 6765 5f69 6e66 6f22 3a20 7b0d 0a20  uage_info": {.. 
-00002400: 2020 2020 2022 636f 6465 6d69 7272 6f72       "codemirror
-00002410: 5f6d 6f64 6522 3a20 7b0d 0a20 2020 2020  _mode": {..     
-00002420: 2020 2022 6e61 6d65 223a 2022 6970 7974     "name": "ipyt
-00002430: 686f 6e22 2c0d 0a20 2020 2020 2020 2022  hon",..        "
-00002440: 7665 7273 696f 6e22 3a20 330d 0a20 2020  version": 3..   
-00002450: 2020 207d 2c0d 0a20 2020 2020 2022 6669     },..      "fi
-00002460: 6c65 5f65 7874 656e 7369 6f6e 223a 2022  le_extension": "
-00002470: 2e70 7922 2c0d 0a20 2020 2020 2022 6d69  .py",..      "mi
-00002480: 6d65 7479 7065 223a 2022 7465 7874 2f78  metype": "text/x
-00002490: 2d70 7974 686f 6e22 2c0d 0a20 2020 2020  -python",..     
-000024a0: 2022 6e61 6d65 223a 2022 7079 7468 6f6e   "name": "python
-000024b0: 222c 0d0a 2020 2020 2020 226e 6263 6f6e  ",..      "nbcon
-000024c0: 7665 7274 5f65 7870 6f72 7465 7222 3a20  vert_exporter": 
-000024d0: 2270 7974 686f 6e22 2c0d 0a20 2020 2020  "python",..     
-000024e0: 2022 7079 676d 656e 7473 5f6c 6578 6572   "pygments_lexer
-000024f0: 223a 2022 6970 7974 686f 6e33 222c 0d0a  ": "ipython3",..
-00002500: 2020 2020 2020 2276 6572 7369 6f6e 223a        "version":
-00002510: 2022 332e 372e 3422 0d0a 2020 2020 7d0d   "3.7.4"..    }.
-00002520: 0a20 207d 2c0d 0a20 2022 6e62 666f 726d  .  },..  "nbform
-00002530: 6174 223a 2034 2c0d 0a20 2022 6e62 666f  at": 4,..  "nbfo
-00002540: 726d 6174 5f6d 696e 6f72 223a 2030 0d0a  rmat_minor": 0..
-00002550: 7d                                       }
+00000000: 2222 220d 0a53 7562 6d6f 6475 6c65 2066  """..Submodule f
+00000010: 6f72 2063 616c 6375 6174 696e 6720 7265  or calcuating re
+00000020: 6c61 7469 7665 2069 6f6e 2070 6172 6974  lative ion parit
+00000030: 696f 6e69 6e67 2062 6173 6564 206f 6e20  ioning based on 
+00000040: 7468 6520 6c61 7474 6963 6520 7374 7261  the lattice stra
+00000050: 696e 206d 6f64 656c 205b 2372 6566 5f31  in model [#ref_1
+00000060: 5d5f 205b 2372 6566 5f32 5d5f 205b 2372  ]_ [#ref_2]_ [#r
+00000070: 6566 5f33 5d5f 2e0d 0a0d 0a54 6f64 6f0d  ef_3]_.....Todo.
+00000080: 0a2d 2d2d 2d2d 2d0d 0a0d 0a20 2020 202a  .------....    *
+00000090: 2042 756c 6b20 6d6f 6475 6c75 7320 616e   Bulk modulus an
+000000a0: 6420 596f 756e 6773 206d 6f64 756c 7573  d Youngs modulus
+000000b0: 2061 7070 726f 7869 6d61 7469 6f6e 7320   approximations 
+000000c0: 5b23 7265 665f 335d 5f20 5b23 7265 665f  [#ref_3]_ [#ref_
+000000d0: 345d 5f20 205b 2372 6566 5f35 5d5f 2e0d  4]_  [#ref_5]_..
+000000e0: 0a0d 0a52 6566 6572 656e 6365 730d 0a2d  ...References..-
+000000f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020  -----------..   
+00000100: 202e 2e20 5b23 7265 665f 315d 2042 7269   .. [#ref_1] Bri
+00000110: 6365 2c20 4a2e 432e 2c20 3139 3735 2e20  ce, J.C., 1975. 
+00000120: 536f 6d65 2074 6865 726d 6f64 796e 616d  Some thermodynam
+00000130: 6963 2061 7370 6563 7473 206f 6620 7468  ic aspects of th
+00000140: 6520 6772 6f77 7468 206f 6620 7374 7261  e growth of stra
+00000150: 696e 6564 2063 7279 7374 616c 732e 0d0a  ined crystals...
+00000160: 2020 2020 2020 2020 2020 2020 4a6f 7572              Jour
+00000170: 6e61 6c20 6f66 2043 7279 7374 616c 2047  nal of Crystal G
+00000180: 726f 7774 6820 3238 2c20 3234 39e2 8093  rowth 28, 249...
+00000190: 3235 332e 0d0a 2020 2020 2020 2020 2020  253...          
+000001a0: 2020 646f 693a 207b 6272 6963 6531 3937    doi: {brice197
+000001b0: 357d 0d0a 2020 2020 2e2e 205b 2372 6566  5}..    .. [#ref
+000001c0: 5f32 5d20 426c 756e 6479 2c20 4a2e 2c20  _2] Blundy, J., 
+000001d0: 576f 6f64 2c20 422e 2c20 3139 3934 2e20  Wood, B., 1994. 
+000001e0: 5072 6564 6963 7469 6f6e 206f 6620 6372  Prediction of cr
+000001f0: 7973 7461 6ce2 8093 6d65 6c74 2070 6172  ystal...melt par
+00000200: 7469 7469 6f6e 2063 6f65 6666 6963 6965  tition coefficie
+00000210: 6e74 7320 6672 6f6d 2065 6c61 7374 6963  nts from elastic
+00000220: 206d 6f64 756c 692e 0d0a 2020 2020 2020   moduli...      
+00000230: 2020 2020 2020 4e61 7475 7265 2033 3732        Nature 372
+00000240: 2c20 3435 322e 0d0a 2020 2020 2020 2020  , 452...        
+00000250: 2020 2020 646f 693a 207b 626c 756e 6479      doi: {blundy
+00000260: 3139 3934 7d0d 0a20 2020 202e 2e20 5b23  1994}..    .. [#
+00000270: 7265 665f 335d 2057 6f6f 642c 2042 2e4a  ref_3] Wood, B.J
+00000280: 2e2c 2042 6c75 6e64 792c 204a 2e44 2e2c  ., Blundy, J.D.,
+00000290: 2032 3031 342e 2054 7261 6365 2045 6c65   2014. Trace Ele
+000002a0: 6d65 6e74 2050 6172 7469 7469 6f6e 696e  ment Partitionin
+000002b0: 673a 2054 6865 2049 6e66 6c75 656e 6365  g: The Influence
+000002c0: 7320 6f66 2049 6f6e 6963 0d0a 2020 2020  s of Ionic..    
+000002d0: 2020 2020 2020 2020 5261 6469 7573 2c20          Radius, 
+000002e0: 4361 7469 6f6e 2043 6861 7267 652c 2050  Cation Charge, P
+000002f0: 7265 7373 7572 652c 2061 6e64 2054 656d  ressure, and Tem
+00000300: 7065 7261 7475 7265 2e20 5472 6561 7469  perature. Treati
+00000310: 7365 206f 6e20 4765 6f63 6865 6d69 7374  se on Geochemist
+00000320: 7279 0d0a 2020 2020 2020 2020 2020 2020  ry..            
+00000330: 2853 6563 6f6e 6420 4564 6974 696f 6e29  (Second Edition)
+00000340: 2033 2c20 3432 31e2 8093 3434 382e 0d0a   3, 421...448...
+00000350: 2020 2020 2020 2020 2020 2020 646f 693a              doi:
+00000360: 207b 776f 6f64 3230 3134 7d0d 0a20 2020   {wood2014}..   
+00000370: 202e 2e20 5b23 7265 665f 345d 2041 6e64   .. [#ref_4] And
+00000380: 6572 736f 6e2c 2044 2e4c 2e2c 2041 6e64  erson, D.L., And
+00000390: 6572 736f 6e2c 204f 2e4c 2e2c 2031 3937  erson, O.L., 197
+000003a0: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
+000003b0: 4272 6965 6620 7265 706f 7274 3a20 5468  Brief report: Th
+000003c0: 6520 6275 6c6b 206d 6f64 756c 7573 2d76  e bulk modulus-v
+000003d0: 6f6c 756d 6520 7265 6c61 7469 6f6e 7368  olume relationsh
+000003e0: 6970 2066 6f72 206f 7869 6465 732e 0d0a  ip for oxides...
+000003f0: 2020 2020 2020 2020 2020 2020 4a6f 7572              Jour
+00000400: 6e61 6c20 6f66 2047 656f 7068 7973 6963  nal of Geophysic
+00000410: 616c 2052 6573 6561 7263 6820 2831 3839  al Research (189
+00000420: 362d 3139 3737 2920 3735 2c20 3334 3934  6-1977) 75, 3494
+00000430: e280 9333 3530 302e 0d0a 2020 2020 2020  ...3500...      
+00000440: 2020 2020 2020 646f 693a 207b 616e 6465        doi: {ande
+00000450: 7273 6f6e 3139 3730 7d0d 0a20 2020 202e  rson1970}..    .
+00000460: 2e20 5b23 7265 665f 355d 2048 617a 656e  . [#ref_5] Hazen
+00000470: 2c20 522e 4d2e 2c20 4669 6e67 6572 2c20  , R.M., Finger, 
+00000480: 4c2e 572e 2c20 3139 3739 2e20 4275 6c6b  L.W., 1979. Bulk
+00000490: 206d 6f64 756c 7573 e280 9476 6f6c 756d   modulus...volum
+000004a0: 6520 7265 6c61 7469 6f6e 7368 6970 2066  e relationship f
+000004b0: 6f72 2063 6174 696f 6e2d 616e 696f 6e20  or cation-anion 
+000004c0: 706f 6c79 6865 6472 612e 0d0a 2020 2020  polyhedra...    
+000004d0: 2020 2020 2020 2020 4a6f 7572 6e61 6c20          Journal 
+000004e0: 6f66 2047 656f 7068 7973 6963 616c 2052  of Geophysical R
+000004f0: 6573 6561 7263 683a 2053 6f6c 6964 2045  esearch: Solid E
+00000500: 6172 7468 2038 342c 2036 3732 33e2 8093  arth 84, 6723...
+00000510: 3637 3238 2e0d 0a20 2020 2020 2020 2020  6728...         
+00000520: 2020 2064 6f69 3a20 7b68 617a 656e 3139     doi: {hazen19
+00000530: 3739 7d0d 0a0d 0a22 2222 0d0a 696d 706f  79}...."""..impo
+00000540: 7274 206e 756d 7079 2061 7320 6e70 0d0a  rt numpy as np..
+00000550: 0d0a 6672 6f6d 202e 2e75 7469 6c2e 6c6f  ..from ..util.lo
+00000560: 6720 696d 706f 7274 2048 616e 646c 650d  g import Handle.
+00000570: 0a66 726f 6d20 2e2e 7574 696c 2e6d 6574  .from ..util.met
+00000580: 6120 696d 706f 7274 2073 7068 696e 785f  a import sphinx_
+00000590: 646f 695f 6c69 6e6b 2c20 7570 6461 7465  doi_link, update
+000005a0: 5f64 6f63 7374 7269 6e67 5f72 6566 6572  _docstring_refer
+000005b0: 656e 6365 730d 0a0d 0a6c 6f67 6765 7220  ences....logger 
+000005c0: 3d20 4861 6e64 6c65 285f 5f6e 616d 655f  = Handle(__name_
+000005d0: 5f29 0d0a 0d0a 0d0a 4075 7064 6174 655f  _)......@update_
+000005e0: 646f 6373 7472 696e 675f 7265 6665 7265  docstring_refere
+000005f0: 6e63 6573 0d0a 6465 6620 7374 7261 696e  nces..def strain
+00000600: 5f63 6f65 6666 6963 6965 6e74 2872 692c  _coefficient(ri,
+00000610: 2072 782c 2072 303d 4e6f 6e65 2c20 453d   rx, r0=None, E=
+00000620: 4e6f 6e65 2c20 543d 3239 382e 3135 2c20  None, T=298.15, 
+00000630: 7a3d 4e6f 6e65 2c20 2a2a 6b77 6172 6773  z=None, **kwargs
+00000640: 293a 0d0a 2020 2020 7222 2222 0d0a 2020  ):..    r"""..  
+00000650: 2020 4361 6c63 756c 6174 6520 7468 6520    Calculate the 
+00000660: 6c61 7474 6963 6520 7374 7261 696e 2061  lattice strain a
+00000670: 7373 6f63 6961 7465 6420 7769 7468 2061  ssociated with a
+00000680: 6e20 696f 6e69 6320 7375 6273 7469 7475  n ionic substitu
+00000690: 7469 6f6e 205b 2372 6566 5f31 5d5f 205b  tion [#ref_1]_ [
+000006a0: 2372 6566 5f32 5d5f 2e0d 0a0d 0a20 2020  #ref_2]_.....   
+000006b0: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+000006c0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020   -----------..  
+000006d0: 2020 7269 203a 203a 636c 6173 733a 6066    ri : :class:`f
+000006e0: 6c6f 6174 600d 0a20 2020 2020 2020 2049  loat`..        I
+000006f0: 6f6e 6963 2072 6164 6975 7320 746f 2063  onic radius to c
+00000700: 616c 6375 6c61 7465 2073 7472 6169 6e20  alculate strain 
+00000710: 7265 6c61 7469 7665 2074 6f2c 2069 6e20  relative to, in 
+00000720: 616e 6773 7472 6f6d 7320 28c3 8529 2e0d  angstroms (..)..
+00000730: 0a20 2020 2072 6a20 3a20 3a63 6c61 7373  .    rj : :class
+00000740: 3a60 666c 6f61 7460 0d0a 2020 2020 2020  :`float`..      
+00000750: 2020 496f 6e69 6320 7261 6469 7573 2074    Ionic radius t
+00000760: 6f20 6361 6c63 756c 6174 6520 7374 7261  o calculate stra
+00000770: 696e 2066 6f72 2c20 696e 2061 6e67 7374  in for, in angst
+00000780: 726f 6d73 2028 c385 292e 0d0a 2020 2020  roms (..)...    
+00000790: 7230 203a 203a 636c 6173 733a 6066 6c6f  r0 : :class:`flo
+000007a0: 6174 602c 203a 636f 6465 3a60 4e6f 6e65  at`, :code:`None
+000007b0: 600d 0a20 2020 2020 2020 2046 6963 7469  `..        Ficti
+000007c0: 7665 2069 6465 616c 2069 6f6e 6963 2072  ve ideal ionic r
+000007d0: 6164 6969 2066 6f72 2074 6865 2073 6974  adii for the sit
+000007e0: 652e 2054 6865 2076 616c 7565 2066 6f72  e. The value for
+000007f0: 203a 636f 6465 3a60 7269 6020 7769 6c6c   :code:`ri` will
+00000800: 2062 6520 7573 6564 2069 6e20 6974 7320   be used in its 
+00000810: 706c 6163 650d 0a20 2020 2020 2020 2069  place..        i
+00000820: 6620 6e6f 6e65 2069 7320 6769 7665 6e2c  f none is given,
+00000830: 2061 6e64 2061 2077 6172 6e69 6e67 2069   and a warning i
+00000840: 7373 7565 642e 0d0a 2020 2020 4520 3a20  ssued...    E : 
+00000850: 3a63 6c61 7373 3a60 666c 6f61 7460 2c20  :class:`float`, 
+00000860: 3a63 6f64 653a 604e 6f6e 6560 0d0a 2020  :code:`None`..  
+00000870: 2020 2020 2020 596f 756e 6727 7320 6d6f        Young's mo
+00000880: 6475 6c75 7320 2873 7469 6666 6e65 7373  dulus (stiffness
+00000890: 2920 666f 7220 7468 6520 7369 7465 2c20  ) for the site, 
+000008a0: 696e 2070 6173 6361 6c73 2028 5061 292e  in pascals (Pa).
+000008b0: 2057 696c 6c20 6265 2065 7374 696d 6174   Will be estimat
+000008c0: 6564 2075 7369 6e67 0d0a 2020 2020 2020  ed using..      
+000008d0: 2020 3a66 756e 633a 6079 6f75 6e67 735f    :func:`youngs_
+000008e0: 6d6f 6475 6c75 735f 6170 7072 6f78 696d  modulus_approxim
+000008f0: 6174 696f 6e60 2069 6620 6e6f 6e65 2069  ation` if none i
+00000900: 7320 6769 7665 6e2e 0d0a 2020 2020 5420  s given...    T 
+00000910: 3a20 3a63 6c61 7373 3a60 666c 6f61 7460  : :class:`float`
+00000920: 0d0a 2020 2020 2020 2020 5465 6d70 6572  ..        Temper
+00000930: 6174 7572 652c 2069 6e20 4b65 6c76 696e  ature, in Kelvin
+00000940: 2028 4b29 2e0d 0a20 2020 207a 203a 203a   (K)...    z : :
+00000950: 636c 6173 733a 6069 6e74 600d 0a20 2020  class:`int`..   
+00000960: 2020 2020 204f 7074 696f 6e61 6c20 7370       Optional sp
+00000970: 6563 6966 6963 6174 696f 6e20 6f66 2063  ecification of c
+00000980: 6174 696f 6e69 6320 7661 6c65 6e63 652c  ationic valence,
+00000990: 2066 6f72 2063 616c 6375 6174 696f 6e20   for calcuation 
+000009a0: 6f66 2061 7070 726f 7869 6d61 7465 0d0a  of approximate..
+000009b0: 2020 2020 2020 2020 596f 756e 6727 7320          Young's 
+000009c0: 6d6f 6475 6c75 7320 7573 696e 6720 3a66  modulus using :f
+000009d0: 756e 633a 6079 6f75 6e67 735f 6d6f 6475  unc:`youngs_modu
+000009e0: 6c75 735f 6170 7072 6f78 696d 6174 696f  lus_approximatio
+000009f0: 6e60 2c0d 0a20 2020 2020 2020 2077 6865  n`,..        whe
+00000a00: 7265 2074 6865 206d 6f64 756c 7573 2069  re the modulus i
+00000a10: 7320 6e6f 7420 7370 6563 6966 6965 642e  s not specified.
+00000a20: 0d0a 0d0a 2020 2020 5265 7475 726e 730d  ....    Returns.
+00000a30: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20  .    --------.. 
+00000a40: 2020 203a 636c 6173 733a 6066 6c6f 6174     :class:`float
+00000a50: 600d 0a20 2020 2020 2020 2054 6865 2073  `..        The s
+00000a60: 7472 6169 6e20 636f 6566 6669 6365 6e74  train coefficent
+00000a70: 203a 6d61 7468 3a60 655e 7b5c 6672 6163   :math:`e^{\frac
+00000a80: 7b2d 5c44 656c 7461 2047 5f7b 7374 7261  {-\Delta G_{stra
+00000a90: 696e 7d7d 7b52 547d 7d60 2e0d 0a0d 0a20  in}}{RT}}`..... 
+00000aa0: 2020 204e 6f74 6573 0d0a 2020 2020 2d2d     Notes..    --
+00000ab0: 2d2d 2d2d 0d0a 0d0a 2020 2020 2020 2020  ----....        
+00000ac0: 5468 6520 6c61 7474 6963 6520 7374 7261  The lattice stra
+00000ad0: 696e 206d 6f64 656c 2072 656c 6174 6573  in model relates
+00000ae0: 2063 6861 6e67 6573 2069 6e20 7061 7269   changes in pari
+00000af0: 7469 6f6e 696e 6720 746f 2064 6966 6665  tioning to diffe
+00000b00: 7265 6e63 6573 2069 6e0d 0a20 2020 2020  rences in..     
+00000b10: 2020 2069 6f6e 6963 2072 6164 6969 2066     ionic radii f
+00000b20: 6f72 2069 6f6e 7320 6f66 2061 2067 6976  or ions of a giv
+00000b30: 656e 2063 6174 696f 6e69 6320 6368 6172  en cationic char
+00000b40: 6765 2c20 616e 6420 666f 7220 6120 666f  ge, and for a fo
+00000b50: 7220 6120 7370 6563 6966 6963 2073 6974  r a specific sit
+00000b60: 650d 0a20 2020 2020 2020 2028 7769 7468  e..        (with
+00000b70: 2059 6f75 6e67 2773 206d 6f64 756c 7573   Young's modulus
+00000b80: 203a 6d61 7468 3a60 4560 292e 2054 6869   :math:`E`). Thi
+00000b90: 7320 6973 2063 616c 6375 6174 6564 2075  s is calcuated u
+00000ba0: 7369 6e67 2074 6865 2077 6f72 6b0d 0a20  sing the work.. 
+00000bb0: 2020 2020 2020 2064 6f6e 6520 746f 2065         done to e
+00000bc0: 7870 616e 6420 6120 7370 6865 7269 6361  xpand a spherica
+00000bd0: 6c20 7368 656c 6c20 6365 6e74 7265 6420  l shell centred 
+00000be0: 6f6e 2074 6865 206c 6174 7469 6365 2073  on the lattice s
+00000bf0: 6974 652c 0d0a 2020 2020 2020 2020 7768  ite,..        wh
+00000c00: 6963 6820 616c 7465 7273 2074 6865 203a  ich alters the :
+00000c10: 6d61 7468 3a60 5c44 656c 7461 2047 6020  math:`\Delta G` 
+00000c20: 666f 7220 7468 6520 666f 726d 6174 696f  for the formatio
+00000c30: 6e20 6f66 2074 6865 206d 696e 6572 616c  n of the mineral
+00000c40: 2e0d 0a20 2020 2020 2020 2054 6869 7320  ...        This 
+00000c50: 6361 6e20 6265 2072 656c 6174 6564 2074  can be related t
+00000c60: 6f20 6368 616e 6765 7320 696e 2070 6172  o changes in par
+00000c70: 7469 7469 6f6e 2063 6f65 6666 6963 6965  tition coefficie
+00000c80: 6e74 7320 7573 696e 6720 7468 6520 666f  nts using the fo
+00000c90: 6c6c 6f77 696e 670d 0a20 2020 2020 2020  llowing..       
+00000ca0: 205b 2372 6566 5f32 5d5f 3a0d 0a0d 0a20   [#ref_2]_:.... 
+00000cb0: 2020 2020 2020 202e 2e20 6d61 7468 3a3a         .. math::
+00000cc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00000cd0: 445f 7b6a 5e7b 6e2b 7d7d 203d 2044 5f7b  D_{j^{n+}} = D_{
+00000ce0: 415e 7b6e 2b7d 7d20 5c63 646f 7420 655e  A^{n+}} \cdot e^
+00000cf0: 7b5c 6672 6163 7b2d 345c 7069 2045 204e  {\frac{-4\pi E N
+00000d00: 205c 4269 6728 5c66 7261 637b 725f 7b30   \Big(\frac{r_{0
+00000d10: 7d7d 7b32 7d28 725f 6a20 2d20 725f 3029  }}{2}(r_j - r_0)
+00000d20: 5e32 202b 205c 6672 6163 7b31 7d7b 337d  ^2 + \frac{1}{3}
+00000d30: 2872 5f6a 202d 2072 5f30 295e 335c 4269  (r_j - r_0)^3\Bi
+00000d40: 6729 7d7b 5254 7d7d 0d0a 0d0a 2020 2020  g)}{RT}}....    
+00000d50: 2020 2020 5768 6572 6520 3a6d 6174 683a      Where :math:
+00000d60: 6044 5f7b 415e 7b6e 2b7d 7d60 2069 7320  `D_{A^{n+}}` is 
+00000d70: 7468 6520 7061 7274 6974 696f 6e20 636f  the partition co
+00000d80: 6566 6669 6369 656e 7420 666f 7220 7468  efficient for th
+00000d90: 6520 6964 6561 6c20 696f 6e20 412c 2061  e ideal ion A, a
+00000da0: 6e64 0d0a 2020 2020 2020 2020 4e20 6973  nd..        N is
+00000db0: 2041 7661 6761 6472 6f27 7320 6e75 6d62   Avagadro's numb
+00000dc0: 6572 2028 362e 3032 3365 3233 2061 746f  er (6.023e23 ato
+00000dd0: 6d73 2f6d 6f6c 292e 2054 6869 7320 6361  ms/mol). This ca
+00000de0: 6e20 616c 736f 0d0a 2020 2020 2020 2020  n also..        
+00000df0: 6265 2063 616c 6375 6174 6564 2072 656c  be calcuated rel
+00000e00: 6174 6976 6520 746f 2061 6e20 2769 6465  ative to an 'ide
+00000e10: 616c 2720 6669 6374 6976 6520 696f 6e20  al' fictive ion 
+00000e20: 7768 6963 6820 6861 7320 6120 6d61 7869  which has a maxi
+00000e30: 6d75 6d20 3a6d 6174 683a 6044 600d 0a20  mum :math:`D`.. 
+00000e40: 2020 2020 2020 2077 6865 7265 2074 6869         where thi
+00000e50: 7320 6461 7461 2061 7265 2061 7661 696c  s data are avail
+00000e60: 6162 6c65 2e20 5468 6973 2072 656c 6174  able. This relat
+00000e70: 696f 6e73 6869 7020 6172 6973 6573 2076  ionship arises v
+00000e80: 6961 2069 2920 7468 6520 696e 7465 6772  ia i) the integr
+00000e90: 6174 696f 6e0d 0a20 2020 2020 2020 2074  ation..        t
+00000ea0: 6f20 6361 6c63 7561 7465 2074 6865 2073  o calcuate the s
+00000eb0: 7472 6169 6e20 656e 6572 6779 206d 656e  train energy men
+00000ec0: 7469 6f6e 6564 2061 626f 7665 0d0a 2020  tioned above..  
+00000ed0: 2020 2020 2020 283a 6d61 7468 3a60 345c        (:math:`4\
+00000ee0: 7069 2045 2028 5c66 7261 637b 725f 7b30  pi E (\frac{r_{0
+00000ef0: 7d7d 7b32 7d28 725f 6a20 2d20 725f 3029  }}{2}(r_j - r_0)
+00000f00: 5e32 202b 205c 6672 6163 7b31 7d7b 337d  ^2 + \frac{1}{3}
+00000f10: 2872 5f6a 202d 2072 5f30 295e 3329 6029  (r_j - r_0)^3)`)
+00000f20: 2c0d 0a20 2020 2020 2020 2061 6e64 2069  ,..        and i
+00000f30: 6929 2074 6865 2061 7373 756d 7074 696f  i) the assumptio
+00000f40: 6e20 7468 6174 2074 6865 2063 6861 6e67  n that the chang
+00000f50: 6573 2069 6e20 3a6d 6174 683a 605c 4465  es in :math:`\De
+00000f60: 6c74 6120 4760 206f 6363 7572 206f 6e6c  lta G` occur onl
+00000f70: 7920 746f 2073 697a 650d 0a20 2020 2020  y to size..     
+00000f80: 2020 2064 6966 6665 7265 6e63 6573 2c20     differences, 
+00000f90: 616e 6420 7468 6520 6469 6666 6572 656e  and the differen
+00000fa0: 6365 2069 7320 6164 6469 7469 7665 2e20  ce is additive. 
+00000fb0: 5468 6520 2773 6567 7265 6761 7469 6f6e  The 'segregation
+00000fc0: 2063 6f65 6666 6963 6965 6e74 270d 0a20   coefficient'.. 
+00000fd0: 2020 2020 2020 203a 6d61 7468 3a60 4b5f         :math:`K_
+00000fe0: 6a60 2063 616e 2062 6520 6578 7072 6573  j` can be expres
+00000ff0: 7365 6420 7265 6c61 7469 7665 2074 6f20  sed relative to 
+00001000: 7468 6520 6e6f 6e2d 646f 7065 6420 6571  the non-doped eq
+00001010: 7569 6c69 6269 7275 6d20 636f 6e73 7461  uilibirum consta
+00001020: 6e74 0d0a 2020 2020 2020 2020 3a6d 6174  nt..        :mat
+00001030: 683a 604b 5f30 6020 5b23 7265 665f 315d  h:`K_0` [#ref_1]
+00001040: 5f3a 0d0a 0d0a 2020 2020 2020 2020 2e2e  _:....        ..
+00001050: 206d 6174 683a 3a0d 0a0d 0a20 2020 2020   math::....     
+00001060: 2020 2020 2020 205c 6265 6769 6e7b 616c         \begin{al
+00001070: 6967 6e7d 0d0a 2020 2020 2020 2020 2020  ign}..          
+00001080: 2020 4b5f 6a20 263d 2065 5e7b 5c66 7261    K_j &= e^{\fra
+00001090: 637b 2d5c 4465 6c74 6120 475f 3020 2d5c  c{-\Delta G_0 -\
+000010a0: 4465 6c74 6120 475f 7b73 7472 6169 6e7d  Delta G_{strain}
+000010b0: 7d7b 5254 7d7d 5c5c 0d0a 2020 2020 2020  }{RT}}\\..      
+000010c0: 2020 2020 2020 2020 2020 263d 2065 5e7b            &= e^{
+000010d0: 5c66 7261 637b 2d5c 4465 6c74 6120 475f  \frac{-\Delta G_
+000010e0: 307d 7b52 547d 7d20 5c63 646f 7420 655e  0}{RT}} \cdot e^
+000010f0: 7b5c 6672 6163 7b2d 5c44 656c 7461 2047  {\frac{-\Delta G
+00001100: 5f7b 7374 7261 696e 7d7d 7b52 547d 7d5c  _{strain}}{RT}}\
+00001110: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
+00001120: 2020 2026 3d20 4b5f 3020 5c63 646f 7420     &= K_0 \cdot 
+00001130: 655e 7b5c 6672 6163 7b2d 5c44 656c 7461  e^{\frac{-\Delta
+00001140: 2047 5f7b 7374 7261 696e 7d7d 7b52 547d   G_{strain}}{RT}
+00001150: 7d5c 5c0d 0a20 2020 2020 2020 2020 2020  }\\..           
+00001160: 205c 656e 647b 616c 6967 6e7d 0d0a 0d0a   \end{align}....
+00001170: 2020 2020 2020 2020 5468 6520 6d6f 6465          The mode
+00001180: 6c20 6173 7375 6d65 7320 7468 6174 2074  l assumes that t
+00001190: 6865 2063 7279 7374 616c 2069 7320 656c  he crystal is el
+000011a0: 6173 7469 6361 6c6c 7920 6973 6f74 726f  astically isotro
+000011b0: 7069 632e 0d0a 0d0a 2020 2020 2222 220d  pic.....    """.
+000011c0: 0a20 2020 206e 203d 2036 2e30 3233 202a  .    n = 6.023 *
+000011d0: 2031 302a 2a32 330d 0a20 2020 2069 6620   10**23..    if 
+000011e0: 7230 2069 7320 4e6f 6e65 3a0d 0a20 2020  r0 is None:..   
+000011f0: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
+00001200: 2822 5573 6520 6669 6374 6976 6520 6964  ("Use fictive id
+00001210: 6561 6c20 6361 7469 6f6e 2072 6164 6969  eal cation radii
+00001220: 2077 6865 7265 2070 6f73 7369 626c 652e   where possible.
+00001230: 2229 0d0a 2020 2020 2020 2020 7230 203d  ")..        r0 =
+00001240: 2072 690d 0a20 2020 2072 692c 2072 782c   ri..    ri, rx,
+00001250: 2072 3020 3d20 7269 202f 2031 302a 2a31   r0 = ri / 10**1
+00001260: 302c 2072 7820 2f20 3130 2a2a 3130 2c20  0, rx / 10**10, 
+00001270: 7230 202f 2031 302a 2a31 3020 2023 2063  r0 / 10**10  # c
+00001280: 6f6e 7665 7274 2074 6f20 6d65 7465 7273  onvert to meters
+00001290: 0d0a 2020 2020 4520 3d20 4520 6f72 2079  ..    E = E or y
+000012a0: 6f75 6e67 735f 6d6f 6475 6c75 735f 6170  oungs_modulus_ap
+000012b0: 7072 6f78 696d 6174 696f 6e28 7a2c 2072  proximation(z, r
+000012c0: 3029 2020 2320 7573 6520 4520 6966 2064  0)  # use E if d
+000012d0: 6566 696e 6564 2c20 656c 7365 2074 7279  efined, else try
+000012e0: 2074 6f20 6361 6c63 0d0a 2020 2020 636f   to calc..    co
+000012f0: 6566 6620 3d20 342e 3020 2a20 6e70 2e70  eff = 4.0 * np.p
+00001300: 6920 2a20 450d 0a0d 0a20 2020 2072 7465  i * E....    rte
+00001310: 726d 203d 2028 7230 202f 2032 2e30 2920  rm = (r0 / 2.0) 
+00001320: 2a20 2872 6920 2d20 7278 2920 2a2a 2032  * (ri - rx) ** 2
+00001330: 202d 2028 312e 3020 2f20 3329 202a 2028   - (1.0 / 3) * (
+00001340: 7269 202d 2072 7829 202a 2a20 330d 0a20  ri - rx) ** 3.. 
+00001350: 2020 2072 6574 7572 6e20 6e70 2e65 7870     return np.exp
+00001360: 2863 6f65 6666 202a 2072 7465 726d 202a  (coeff * rterm *
+00001370: 2028 2d6e 202f 2028 382e 3331 3420 2a20   (-n / (8.314 * 
+00001380: 5429 2929 0d0a 0d0a 0d0a 4075 7064 6174  T)))......@updat
+00001390: 655f 646f 6373 7472 696e 675f 7265 6665  e_docstring_refe
+000013a0: 7265 6e63 6573 0d0a 6465 6620 796f 756e  rences..def youn
+000013b0: 6773 5f6d 6f64 756c 7573 5f61 7070 726f  gs_modulus_appro
+000013c0: 7869 6d61 7469 6f6e 287a 2c20 7229 3a0d  ximation(z, r):.
+000013d0: 0a20 2020 2072 2222 220d 0a20 2020 2059  .    r"""..    Y
+000013e0: 6f75 6e67 2773 206d 6f64 756c 7573 2061  oung's modulus a
+000013f0: 7070 726f 7869 6d61 7469 6f6e 2066 6f72  pproximation for
+00001400: 2063 6174 696f 6e69 6320 7369 7465 7320   cationic sites 
+00001410: 696e 2073 696c 6963 6174 6573 0d0a 2020  in silicates..  
+00001420: 2020 616e 6420 6f78 6964 6573 205b 2372    and oxides [#r
+00001430: 6566 5f31 5d5f 205b 2372 6566 5f32 5d5f  ef_1]_ [#ref_2]_
+00001440: 205b 2372 6566 5f33 5d5f 2e0d 0a0d 0a20   [#ref_3]_..... 
+00001450: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+00001460: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+00001470: 2020 207a 203a 203a 636c 6173 733a 6069     z : :class:`i
+00001480: 6e74 6567 6572 600d 0a20 2020 2020 2020  nteger`..       
+00001490: 2043 6174 696f 6e69 6320 7661 6c65 6e63   Cationic valenc
+000014a0: 652e 0d0a 2020 2020 7220 3a20 3a63 6c61  e...    r : :cla
+000014b0: 7373 3a60 666c 6f61 7460 0d0a 2020 2020  ss:`float`..    
+000014c0: 2020 2020 496f 6e69 6320 7261 6469 7573      Ionic radius
+000014d0: 206f 6620 7468 6520 6361 7469 6f6e 2028   of the cation (
+000014e0: c385 292e 0d0a 0d0a 2020 2020 5265 7475  ..).....    Retu
+000014f0: 726e 730d 0a20 2020 202d 2d2d 2d2d 2d2d  rns..    -------
+00001500: 2d0d 0a20 2020 2045 203a 203a 636c 6173  -..    E : :clas
+00001510: 733a 6066 6c6f 6174 600d 0a20 2020 2020  s:`float`..     
+00001520: 2020 2059 6f75 6e67 2773 206d 6f64 756c     Young's modul
+00001530: 7573 2066 6f72 2074 6865 2063 6174 696f  us for the catio
+00001540: 6e69 6320 7369 7465 2c20 696e 2050 6173  nic site, in Pas
+00001550: 6361 6c73 2028 5061 290d 0a20 2020 204e  cals (Pa)..    N
+00001560: 6f74 6573 0d0a 2020 2020 2d2d 2d2d 2d2d  otes..    ------
+00001570: 0d0a 2020 2020 5468 6520 6275 6c6b 206d  ..    The bulk m
+00001580: 6f64 756c 7573 203a 6d61 7468 3a60 4b60  odulus :math:`K`
+00001590: 2066 6f72 2061 6e20 616e 2069 6f6e 6963   for an an ionic
+000015a0: 2063 7279 7374 616c 2069 7320 6573 696d   crystal is esim
+000015b0: 6174 6564 2075 7369 6e67 205b 2372 6566  ated using [#ref
+000015c0: 5f31 5d5f 3a0d 0a0d 0a20 2020 202e 2e20  _1]_:....    .. 
+000015d0: 6d61 7468 3a3a 0d0a 0d0a 2020 2020 2020  math::....      
+000015e0: 2020 4b20 3d20 5c66 7261 637b 4120 5a5f    K = \frac{A Z_
+000015f0: 6120 5a5f 6320 655e 3220 286e 2d31 297d  a Z_c e^2 (n-1)}
+00001600: 7b39 2064 5f30 2056 5f30 7d0d 0a0d 0a20  {9 d_0 V_0}.... 
+00001610: 2020 2057 6865 7265 203a 6d61 7468 3a60     Where :math:`
+00001620: 4160 2069 7320 7468 6520 4d61 6465 6c75  A` is the Madelu
+00001630: 6e67 2063 6f6e 7374 616e 742c 203a 6d61  ng constant, :ma
+00001640: 7468 3a60 5a5f 6360 2061 6e64 203a 6d61  th:`Z_c` and :ma
+00001650: 7468 3a60 5a5f 6160 2061 7265 2074 6865  th:`Z_a` are the
+00001660: 0d0a 2020 2020 616e 696f 6e20 616e 6420  ..    anion and 
+00001670: 6361 7469 6f6e 2076 616c 656e 6365 732c  cation valences,
+00001680: 203a 6d61 7468 3a60 6560 2069 7320 7468   :math:`e` is th
+00001690: 6520 6368 6172 6765 206f 6e20 7468 6520  e charge on the 
+000016a0: 656c 6563 7472 6f6e 2c0d 0a20 2020 203a  electron,..    :
+000016b0: 6d61 7468 3a60 6e60 2069 7320 7468 6520  math:`n` is the 
+000016c0: 426f 726e 2070 6f77 6572 206c 6177 2063  Born power law c
+000016d0: 6f65 6666 6963 656e 742c 2061 6e64 203a  oefficent, and :
+000016e0: 6d61 7468 3a60 645f 3060 2069 7320 7468  math:`d_0` is th
+000016f0: 6520 6361 7469 6f6e 2d61 6e69 6f6e 0d0a  e cation-anion..
+00001700: 2020 2020 6469 7374 616e 6365 205b 2372      distance [#r
+00001710: 6566 5f31 5d5f 2e20 5573 696e 6720 7468  ef_1]_. Using th
+00001720: 6520 5368 616e 6e6f 6e20 696f 6e69 6320  e Shannon ionic 
+00001730: 7261 6469 7573 2066 6f72 206f 7879 6765  radius for oxyge
+00001740: 6e20 2831 2e33 3820 c385 292c 0d0a 2020  n (1.38 ..),..  
+00001750: 2020 7468 6973 2069 7320 6170 7072 6f78    this is approx
+00001760: 696d 6174 6564 2066 6f72 2063 6174 696f  imated for catio
+00001770: 6e73 2063 6f6f 7264 696e 6174 6564 2062  ns coordinated b
+00001780: 7920 6f78 7967 656e 2069 6e20 7369 6c69  y oxygen in sili
+00001790: 6361 7465 7320 616e 6420 6f78 6964 6573  cates and oxides
+000017a0: 0d0a 2020 2020 7573 696e 6720 7468 6520  ..    using the 
+000017b0: 666f 6c6c 6f77 696e 6720 7265 6c61 7469  following relati
+000017c0: 6f6e 7368 6970 205b 2372 6566 5f32 5d5f  onship [#ref_2]_
+000017d0: 3a0d 0a0d 0a20 2020 202e 2e20 6d61 7468  :....    .. math
+000017e0: 3a3a 0d0a 0d0a 2020 2020 2020 2020 4b20  ::....        K 
+000017f0: 3d20 3735 3020 5a5f 6320 645e 7b2d 337d  = 750 Z_c d^{-3}
+00001800: 0d0a 0d0a 2020 2020 5768 6572 6520 3a6d  ....    Where :m
+00001810: 6174 683a 6064 6020 6973 2074 6865 2063  ath:`d` is the c
+00001820: 6174 696f 6e2d 616e 696f 6e20 6469 7374  ation-anion dist
+00001830: 616e 6365 2028 c385 292c 203a 6d61 7468  ance (..), :math
+00001840: 3a60 5a5f 6360 2069 7320 7468 650d 0a20  :`Z_c` is the.. 
+00001850: 2020 2063 6174 696f 6e69 6320 7661 6c65     cationic vale
+00001860: 6e63 6520 2861 6e64 203a 6d61 7468 3a60  nce (and :math:`
+00001870: 4b60 2069 7320 696e 2047 5061 292e 2054  K` is in GPa). T
+00001880: 6865 2059 6f75 6e67 2773 206d 6f64 756c  he Young's modul
+00001890: 7573 203a 6d61 7468 3a60 4560 2069 730d  us :math:`E` is.
+000018a0: 0a20 2020 2074 6865 6e20 6361 6c63 756c  .    then calcul
+000018b0: 6174 6564 2074 6872 6f75 6768 2074 6865  ated through the
+000018c0: 2072 656c 6174 696f 6e73 6869 7020 5b23   relationship [#
+000018d0: 7265 665f 335d 5f3a 0d0a 0d0a 2020 2020  ref_3]_:....    
+000018e0: 2e2e 206d 6174 683a 3a0d 0a0d 0a20 2020  .. math::....   
+000018f0: 2020 2020 2045 203d 2033 204b 2028 3120       E = 3 K (1 
+00001900: 2d20 3220 5c73 6967 6d61 290d 0a0d 0a20  - 2 \sigma).... 
+00001910: 2020 2057 6865 7265 203a 6d61 7468 3a60     Where :math:`
+00001920: 5c73 6967 6d61 6020 6973 2050 6f69 7373  \sigma` is Poiss
+00001930: 6f6e 2773 2072 6174 696f 2c20 7768 6963  on's ratio, whic
+00001940: 6820 696e 2074 6865 2063 6173 6520 6f66  h in the case of
+00001950: 206d 696e 6572 616c 7320 6361 6e20 6265   minerals can be
+00001960: 0d0a 2020 2020 6170 7072 6f69 6d78 6174  ..    approimxat
+00001970: 6564 2062 7920 302e 3235 205b 2372 6566  ed by 0.25 [#ref
+00001980: 5f33 5d5f 2c20 616e 6420 6865 6e63 653a  _3]_, and hence:
+00001990: 0d0a 0d0a 2020 2020 2e2e 206d 6174 683a  ....    .. math:
+000019a0: 3a0d 0a0d 0a20 2020 2020 2020 205c 6265  :....        \be
+000019b0: 6769 6e7b 616c 6967 6e7d 0d0a 2020 2020  gin{align}..    
+000019c0: 2020 2020 2020 2020 4520 265c 6170 7072          E &\appr
+000019d0: 6f78 2031 2e35 204b 5c5c 0d0a 2020 2020  ox 1.5 K\\..    
+000019e0: 2020 2020 2020 2020 4520 265c 6170 7072          E &\appr
+000019f0: 6f78 2031 3032 3520 5a5f 6320 645e 7b2d  ox 1025 Z_c d^{-
+00001a00: 337d 0d0a 2020 2020 2020 2020 5c65 6e64  3}..        \end
+00001a10: 7b61 6c69 676e 7d0d 0a0d 0a20 2020 2054  {align}....    T
+00001a20: 6f64 6f0d 0a20 2020 202d 2d2d 2d2d 0d0a  odo..    -----..
+00001a30: 0d0a 2020 2020 2020 2020 2a20 4164 6420  ..        * Add 
+00001a40: 6c69 6e6b 7320 746f 2064 6f63 7374 7269  links to docstri
+00001a50: 6e67 0d0a 0d0a 2020 2020 2222 220d 0a20  ng....    """.. 
+00001a60: 2020 2061 7373 6572 7420 287a 2069 7320     assert (z is 
+00001a70: 6e6f 7420 4e6f 6e65 2920 616e 6420 280d  not None) and (.
+00001a80: 0a20 2020 2020 2020 2072 2069 7320 6e6f  .        r is no
+00001a90: 7420 4e6f 6e65 0d0a 2020 2020 292c 2022  t None..    ), "
+00001aa0: 4e65 6564 2063 6861 7267 6520 616e 6420  Need charge and 
+00001ab0: 7261 6469 6920 746f 2061 7070 726f 7869  radii to approxi
+00001ac0: 6d61 7465 2059 6f75 6e67 2773 204d 6f64  mate Young's Mod
+00001ad0: 756c 7573 220d 0a20 2020 2064 203d 2072  ulus"..    d = r
+00001ae0: 202b 2031 2e33 380d 0a20 2020 2045 203d   + 1.38..    E =
+00001af0: 2031 2e35 202a 2037 3530 202a 2028 7a20   1.5 * 750 * (z 
+00001b00: 2f20 642a 2a33 2920 2a20 3130 2a2a 390d  / d**3) * 10**9.
+00001b10: 0a20 2020 2072 6574 7572 6e20 450d 0a0d  .    return E...
+00001b20: 0a0d 0a5f 5f64 6f63 5f5f 203d 205f 5f64  ...__doc__ = __d
+00001b30: 6f63 5f5f 2e66 6f72 6d61 7428 0d0a 2020  oc__.format(..  
+00001b40: 2020 6272 6963 6531 3937 353d 7370 6869    brice1975=sphi
+00001b50: 6e78 5f64 6f69 5f6c 696e 6b28 2231 302e  nx_doi_link("10.
+00001b60: 3130 3136 2f30 3032 322d 3032 3438 2837  1016/0022-0248(7
+00001b70: 3529 3930 3234 312d 3922 292c 0d0a 2020  5)90241-9"),..  
+00001b80: 2020 626c 756e 6479 3139 3934 3d73 7068    blundy1994=sph
+00001b90: 696e 785f 646f 695f 6c69 6e6b 2822 3130  inx_doi_link("10
+00001ba0: 2e31 3033 382f 3337 3234 3532 6130 2229  .1038/372452a0")
+00001bb0: 2c0d 0a20 2020 2061 6e64 6572 736f 6e31  ,..    anderson1
+00001bc0: 3937 303d 7370 6869 6e78 5f64 6f69 5f6c  970=sphinx_doi_l
+00001bd0: 696e 6b28 2231 302e 3130 3239 2f4a 4230  ink("10.1029/JB0
+00001be0: 3735 6930 3137 7030 3334 3934 2229 2c0d  75i017p03494"),.
+00001bf0: 0a20 2020 2068 617a 656e 3139 3739 3d73  .    hazen1979=s
+00001c00: 7068 696e 785f 646f 695f 6c69 6e6b 2822  phinx_doi_link("
+00001c10: 3130 2e31 3032 392f 4a42 3038 3469 4231  10.1029/JB084iB1
+00001c20: 3270 3036 3732 3322 292c 0d0a 2020 2020  2p06723"),..    
+00001c30: 776f 6f64 3230 3134 3d73 7068 696e 785f  wood2014=sphinx_
+00001c40: 646f 695f 6c69 6e6b 2822 3130 2e31 3031  doi_link("10.101
+00001c50: 362f 4239 3738 2d30 2d30 382d 3039 3539  6/B978-0-08-0959
+00001c60: 3735 2d37 2e30 3032 3039 2d36 2229 2c0d  75-7.00209-6"),.
+00001c70: 0a29 0d0a 5f5f 646f 635f 5f20 3d20 7374  .)..__doc__ = st
+00001c80: 7228 5f5f 646f 635f 5f29 2e72 6570 6c61  r(__doc__).repla
+00001c90: 6365 2822 7265 6622 2c20 5f5f 6e61 6d65  ce("ref", __name
+00001ca0: 5f5f 290d 0a0d 0a23 2061 6464 2072 6566  __)....# add ref
+00001cb0: 6572 656e 6365 7320 666f 7220 7468 6520  erences for the 
+00001cc0: 6c61 7474 6963 6520 7374 7261 696e 206d  lattice strain m
+00001cd0: 6f64 656c 2c20 6e65 6564 7320 746f 2062  odel, needs to b
+00001ce0: 6520 646f 6e65 2068 6572 6520 6475 6520  e done here due 
+00001cf0: 746f 206e 6573 7465 6420 7b7d 0d0a 2320  to nested {}..# 
+00001d00: 696e 2074 6865 206d 6174 6820 626c 6f63  in the math bloc
+00001d10: 6b73 0d0a 7363 5f72 6566 203d 2072 2222  ks..sc_ref = r""
+00001d20: 2252 6566 6572 656e 6365 730d 0a20 2020  "References..   
+00001d30: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+00001d40: 202e 2e20 5b23 7265 665f 315d 2042 7269   .. [#ref_1] Bri
+00001d50: 6365 2c20 4a2e 432e 2c20 3139 3735 2e20  ce, J.C., 1975. 
+00001d60: 536f 6d65 2074 6865 726d 6f64 796e 616d  Some thermodynam
+00001d70: 6963 2061 7370 6563 7473 206f 6620 7468  ic aspects of th
+00001d80: 6520 6772 6f77 7468 206f 6620 7374 7261  e growth of stra
+00001d90: 696e 6564 2063 7279 7374 616c 732e 0d0a  ined crystals...
+00001da0: 2020 2020 2020 2020 2020 2020 4a6f 7572              Jour
+00001db0: 6e61 6c20 6f66 2043 7279 7374 616c 2047  nal of Crystal G
+00001dc0: 726f 7774 6820 3238 2c20 3234 39e2 8093  rowth 28, 249...
+00001dd0: 3235 332e 0d0a 2020 2020 2020 2020 2020  253...          
+00001de0: 2020 646f 693a 207b 6272 6963 6531 3937    doi: {brice197
+00001df0: 357d 0d0a 2020 2020 2e2e 205b 2372 6566  5}..    .. [#ref
+00001e00: 5f32 5d20 426c 756e 6479 2c20 4a2e 2c20  _2] Blundy, J., 
+00001e10: 576f 6f64 2c20 422e 2c20 3139 3934 2e20  Wood, B., 1994. 
+00001e20: 5072 6564 6963 7469 6f6e 206f 6620 6372  Prediction of cr
+00001e30: 7973 7461 6ce2 8093 6d65 6c74 2070 6172  ystal...melt par
+00001e40: 7469 7469 6f6e 2063 6f65 6666 6963 6965  tition coefficie
+00001e50: 6e74 7320 6672 6f6d 2065 6c61 7374 6963  nts from elastic
+00001e60: 206d 6f64 756c 692e 0d0a 2020 2020 2020   moduli...      
+00001e70: 2020 2020 2020 4e61 7475 7265 2033 3732        Nature 372
+00001e80: 2c20 3435 322e 0d0a 2020 2020 2020 2020  , 452...        
+00001e90: 2020 2020 646f 693a 207b 626c 756e 6479      doi: {blundy
+00001ea0: 3139 3934 7d0d 0a20 2020 2022 2222 2e66  1994}..    """.f
+00001eb0: 6f72 6d61 7428 0d0a 2020 2020 6272 6963  ormat(..    bric
+00001ec0: 6531 3937 353d 7370 6869 6e78 5f64 6f69  e1975=sphinx_doi
+00001ed0: 5f6c 696e 6b28 2231 302e 3130 3136 2f30  _link("10.1016/0
+00001ee0: 3032 322d 3032 3438 2837 3529 3930 3234  022-0248(75)9024
+00001ef0: 312d 3922 292c 0d0a 2020 2020 626c 756e  1-9"),..    blun
+00001f00: 6479 3139 3934 3d73 7068 696e 785f 646f  dy1994=sphinx_do
+00001f10: 695f 6c69 6e6b 2822 3130 2e31 3033 382f  i_link("10.1038/
+00001f20: 3337 3234 3532 6130 2229 2c0d 0a29 0d0a  372452a0"),..)..
+00001f30: 7363 5f72 6566 203d 2073 635f 7265 662e  sc_ref = sc_ref.
+00001f40: 7265 706c 6163 6528 0d0a 2020 2020 2272  replace(..    "r
+00001f50: 6566 222c 2073 7472 6169 6e5f 636f 6566  ef", strain_coef
+00001f60: 6669 6369 656e 742e 5f5f 6d6f 6475 6c65  ficient.__module
+00001f70: 5f5f 202b 2022 2e22 202b 2073 7472 6169  __ + "." + strai
+00001f80: 6e5f 636f 6566 6669 6369 656e 742e 5f5f  n_coefficient.__
+00001f90: 6e61 6d65 5f5f 0d0a 290d 0a73 7472 6169  name__..)..strai
+00001fa0: 6e5f 636f 6566 6669 6369 656e 742e 5f5f  n_coefficient.__
+00001fb0: 646f 635f 5f20 3d20 7374 7261 696e 5f63  doc__ = strain_c
+00001fc0: 6f65 6666 6963 6965 6e74 2e5f 5f64 6f63  oefficient.__doc
+00001fd0: 5f5f 202b 2073 635f 7265 660d 0a0d 0a62  __ + sc_ref....b
+00001fe0: 6d5f 7265 6620 3d20 7222 2222 5265 6665  m_ref = r"""Refe
+00001ff0: 7265 6e63 6573 0d0a 2020 2020 2d2d 2d2d  rences..    ----
+00002000: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+00002010: 202e 2e20 5b23 7265 665f 315d 2041 6e64   .. [#ref_1] And
+00002020: 6572 736f 6e2c 2044 2e4c 2e2c 2041 6e64  erson, D.L., And
+00002030: 6572 736f 6e2c 204f 2e4c 2e2c 2031 3937  erson, O.L., 197
+00002040: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
+00002050: 2020 2020 4272 6965 6620 7265 706f 7274      Brief report
+00002060: 3a20 5468 6520 6275 6c6b 206d 6f64 756c  : The bulk modul
+00002070: 7573 2d76 6f6c 756d 6520 7265 6c61 7469  us-volume relati
+00002080: 6f6e 7368 6970 2066 6f72 206f 7869 6465  onship for oxide
+00002090: 732e 0d0a 2020 2020 2020 2020 2020 2020  s...            
+000020a0: 2020 2020 4a6f 7572 6e61 6c20 6f66 2047      Journal of G
+000020b0: 656f 7068 7973 6963 616c 2052 6573 6561  eophysical Resea
+000020c0: 7263 6820 2831 3839 362d 3139 3737 2920  rch (1896-1977) 
+000020d0: 3735 2c20 3334 3934 e280 9333 3530 302e  75, 3494...3500.
+000020e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000020f0: 2020 646f 693a 207b 616e 6465 7273 6f6e    doi: {anderson
+00002100: 3139 3730 7d0d 0a20 2020 2020 2020 202e  1970}..        .
+00002110: 2e20 5b23 7265 665f 325d 2048 617a 656e  . [#ref_2] Hazen
+00002120: 2c20 522e 4d2e 2c20 4669 6e67 6572 2c20  , R.M., Finger, 
+00002130: 4c2e 572e 2c20 3139 3739 2e20 4275 6c6b  L.W., 1979. Bulk
+00002140: 206d 6f64 756c 7573 e280 9476 6f6c 756d   modulus...volum
+00002150: 6520 7265 6c61 7469 6f6e 7368 6970 2066  e relationship f
+00002160: 6f72 0d0a 2020 2020 2020 2020 2020 2020  or..            
+00002170: 2020 2020 6361 7469 6f6e 2d61 6e69 6f6e      cation-anion
+00002180: 2070 6f6c 7968 6564 7261 2e20 4a6f 7572   polyhedra. Jour
+00002190: 6e61 6c20 6f66 2047 656f 7068 7973 6963  nal of Geophysic
+000021a0: 616c 2052 6573 6561 7263 683a 2053 6f6c  al Research: Sol
+000021b0: 6964 2045 6172 7468 2038 342c 0d0a 2020  id Earth 84,..  
+000021c0: 2020 2020 2020 2020 2020 2020 2020 3637                67
+000021d0: 3233 e280 9336 3732 382e 0d0a 2020 2020  23...6728...    
+000021e0: 2020 2020 2020 2020 2020 2020 646f 693a              doi:
+000021f0: 207b 6861 7a65 6e31 3937 397d 0d0a 2020   {hazen1979}..  
+00002200: 2020 2020 2020 2e2e 205b 2372 6566 5f33        .. [#ref_3
+00002210: 5d20 576f 6f64 2c20 422e 4a2e 2c20 426c  ] Wood, B.J., Bl
+00002220: 756e 6479 2c20 4a2e 442e 2c20 3230 3134  undy, J.D., 2014
+00002230: 2e20 5472 6163 6520 456c 656d 656e 7420  . Trace Element 
+00002240: 5061 7274 6974 696f 6e69 6e67 3a20 5468  Partitioning: Th
+00002250: 6520 496e 666c 7565 6e63 6573 206f 6620  e Influences of 
+00002260: 496f 6e69 630d 0a20 2020 2020 2020 2020  Ionic..         
+00002270: 2020 2020 2020 2052 6164 6975 732c 2043         Radius, C
+00002280: 6174 696f 6e20 4368 6172 6765 2c20 5072  ation Charge, Pr
+00002290: 6573 7375 7265 2c20 616e 6420 5465 6d70  essure, and Temp
+000022a0: 6572 6174 7572 652e 2054 7265 6174 6973  erature. Treatis
+000022b0: 6520 6f6e 2047 656f 6368 656d 6973 7472  e on Geochemistr
+000022c0: 790d 0a20 2020 2020 2020 2020 2020 2020  y..             
+000022d0: 2020 2028 5365 636f 6e64 2045 6469 7469     (Second Editi
+000022e0: 6f6e 2920 332c 2034 3231 e280 9334 3438  on) 3, 421...448
+000022f0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00002300: 2020 2064 6f69 3a20 7b77 6f6f 6432 3031     doi: {wood201
+00002310: 347d 0d0a 2020 2020 2222 222e 666f 726d  4}..    """.form
+00002320: 6174 280d 0a20 2020 2061 6e64 6572 736f  at(..    anderso
+00002330: 6e31 3937 303d 7370 6869 6e78 5f64 6f69  n1970=sphinx_doi
+00002340: 5f6c 696e 6b28 2231 302e 3130 3239 2f4a  _link("10.1029/J
+00002350: 4230 3735 6930 3137 7030 3334 3934 2229  B075i017p03494")
+00002360: 2c0d 0a20 2020 2068 617a 656e 3139 3739  ,..    hazen1979
+00002370: 3d73 7068 696e 785f 646f 695f 6c69 6e6b  =sphinx_doi_link
+00002380: 2822 3130 2e31 3032 392f 4a42 3038 3469  ("10.1029/JB084i
+00002390: 4231 3270 3036 3732 3322 292c 0d0a 2020  B12p06723"),..  
+000023a0: 2020 776f 6f64 3230 3134 3d73 7068 696e    wood2014=sphin
+000023b0: 785f 646f 695f 6c69 6e6b 2822 3130 2e31  x_doi_link("10.1
+000023c0: 3031 362f 4239 3738 2d30 2d30 382d 3039  016/B978-0-08-09
+000023d0: 3539 3735 2d37 2e30 3032 3039 2d36 2229  5975-7.00209-6")
+000023e0: 2c0d 0a29 0d0a 626d 5f72 6566 203d 2062  ,..)..bm_ref = b
+000023f0: 6d5f 7265 662e 7265 706c 6163 6528 0d0a  m_ref.replace(..
+00002400: 2020 2020 2272 6566 222c 0d0a 2020 2020      "ref",..    
+00002410: 796f 756e 6773 5f6d 6f64 756c 7573 5f61  youngs_modulus_a
+00002420: 7070 726f 7869 6d61 7469 6f6e 2e5f 5f6d  pproximation.__m
+00002430: 6f64 756c 655f 5f0d 0a20 2020 202b 2022  odule__..    + "
+00002440: 2e22 0d0a 2020 2020 2b20 796f 756e 6773  ."..    + youngs
+00002450: 5f6d 6f64 756c 7573 5f61 7070 726f 7869  _modulus_approxi
+00002460: 6d61 7469 6f6e 2e5f 5f6e 616d 655f 5f2c  mation.__name__,
+00002470: 0d0a 290d 0a79 6f75 6e67 735f 6d6f 6475  ..)..youngs_modu
+00002480: 6c75 735f 6170 7072 6f78 696d 6174 696f  lus_approximatio
+00002490: 6e2e 5f5f 646f 635f 5f20 3d20 796f 756e  n.__doc__ = youn
+000024a0: 6773 5f6d 6f64 756c 7573 5f61 7070 726f  gs_modulus_appro
+000024b0: 7869 6d61 7469 6f6e 2e5f 5f64 6f63 5f5f  ximation.__doc__
+000024c0: 202b 2062 6d5f 7265 660d 0a               + bm_ref..
```

### Comparing `pyrolite-0.3.3.post0/docs/source/examples/geochem/mineral_lattice.rst` & `pyrolite-0.3.4/pyrolite/geochem/magma.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,297 +1,235 @@
-.. rst-class:: sphx-glr-example-title
-
-.. _sphx_glr_examples_geochem_mineral_lattice.py:
-
-
-Lattice Strain Calculations
-------------------------------
-
-.. note::
-
-    This example follows that given during a Institute of Advanced Studies Masterclass
-    with Jon Blundy at the University of Western Australia on the 29\ :sup:`th` April
-    2019, and is used here with permission.
-
-
-Pyrolite includes a function for calculating relative lattice strain [#ref_1]_, which
-together with the tables of Shannon ionic radii and Young's modulus approximations for
-silicate and oxide cationic sites enable relatively simple calculation of ionic
-partitioning in common rock forming minerals.
-
-This example below uses previously characterised calcium and sodium partition
-coefficients between plagioclase (:math:`CaAl_2Si_2O_8 - NaAlSi_3O8`) and silicate melt
-to estimate partitioning for other cations based on their ionic radii.
-
-A model parameterised using sodium and calcium partition coefficients [#ref_2]_ is then
-used to estimate the partitioning for lanthanum into the trivalent site (largely
-occupied by :math:`Al^{3+}`), and extended to other trivalent cations (here, the Rare
-Earth Elements). The final section of the example highlights the mechanism which
-generates plagioclase's hallmark 'europium anomaly', and the effects of variable
-europium oxidation state on bulk europium partitioning.
-
-
-.. code-block:: default
-
-    import numpy as np
-    import matplotlib.pyplot as plt
-    from pyrolite.geochem.ind import REE, get_ionic_radii
-    from pyrolite.mineral.lattice import strain_coefficient
-
-
-
-
-
-
-
-
-First, we need to define some of the necessary parameters including temperature, the Young's
-moduli for the :math:`X^{2+}` and :math:`X^{3+}` sites in plagioclase (:math:`E_2`,
-:math:`E_3`), and some reference partition coefficients and radii for calcium and
-sodium:
-
-
-.. code-block:: default
-
-    D_Na = 1.35  # Partition coefficient Plag-Melt
-    D_Ca = 4.1  # Partition coefficient Plag-Melt
-    Tc = 900  # Temperature, °C
-    Tk = Tc + 273.15  # Temperature, K
-    E_2 = 120 * 10 ** 9  # Youngs modulus for 2+ site, Pa
-    E_3 = 135 * 10 ** 9  # Youngs modulus for 3+ site, Pa
-    r02, r03 = 1.196, 1.294  # fictive ideal cation radii for these sites
-    rCa = get_ionic_radii("Ca", charge=2, coordination=8)
-    rLa = get_ionic_radii("La", charge=3, coordination=8)
-
-
-
-
-
-
-
-We can calculate and plot the partitioning of :math:`X^{2+}` cations relative to
-:math:`Ca^{2+}` at a given temperature using their radii and the lattice strain function:
-
-
-
-.. code-block:: default
-
-    fontsize = 8
-    fig, ax = plt.subplots(1)
-
-    site2labels = ["Na", "Ca", "Eu", "Sr"]
-    # get the Shannon ionic radii for the elements in the 2+ site
-    site2radii = [
-        get_ionic_radii("Na", charge=1, coordination=8),
-        *[get_ionic_radii(el, charge=2, coordination=8) for el in ["Ca", "Eu", "Sr"]],
-    ]
-    # plot the relative paritioning curve for cations in the 2+ site
-    site2Ds = D_Ca * np.array(
-        [strain_coefficient(rCa, rx, r0=r02, E=E_2, T=Tk) for rx in site2radii]
-    )
-    ax.scatter(site2radii, site2Ds, color="g", label="$X^{2+}$ Cations")
-    # create an index of radii, and plot the relative paritioning curve for the site
-    xs = np.linspace(0.9, 1.3, 200)
-    curve2Ds = D_Ca * strain_coefficient(rCa, xs, r0=r02, E=E_2, T=Tk)
-    ax.plot(xs, curve2Ds, color="0.5", ls="--")
-    # add the element labels next to the points
-    for l, r, d in zip(site2labels, site2radii, site2Ds):
-        ax.annotate(
-            l, xy=(r, d), xycoords="data", ha="left", va="bottom", fontsize=fontsize
-        )
-    fig
-
-
-
-.. image:: /examples/geochem/images/sphx_glr_mineral_lattice_001.png
-    :class: sphx-glr-single-img
-
-
-.. rst-class:: sphx-glr-script-out
-
- Out:
-
- .. code-block:: none
-
-
-    <Figure size 640x480 with 1 Axes>
-
-
-
-When it comes to estimating the partitioning of :math:`X^{3+}` cations, we'll need a reference
-point - here we'll use :math:`D_{La}` to calculate relative partitioning of the other
-Rare Earth Elements, although you may have noticed it is not defined above.
-Through a handy relationship, we can estimate :math:`D_{La}`
-based on the easier measured :math:`D_{Ca}`, :math:`D_{Na}` and temperature [#ref_2]_:
-
-
-
-.. code-block:: default
-
-    D_La = (D_Ca ** 2 / D_Na) * np.exp((529 / Tk) - 3.705)
-    D_La  # 0.48085
-
-
-
-
-.. rst-class:: sphx-glr-script-out
-
- Out:
-
- .. code-block:: none
-
-
-    0.48084614946362086
-
-
-
-Now :math:`D_{La}` is defined, we can use it as a reference for the other REE:
-
-
-
-.. code-block:: default
-
-    site3labels = REE(dropPm=True)
-    # get the Shannon ionic radii for the elements in the 3+ site
-    site3radii = [get_ionic_radii(x, charge=3, coordination=8) for x in REE(dropPm=True)]
-    site3Ds = D_La * np.array(
-        [strain_coefficient(rLa, rx, r0=r03, E=E_3, T=Tk) for rx in site3radii]
-    )
-    # plot the relative paritioning curve for cations in the 3+ site
-    ax.scatter(site3radii, site3Ds, color="purple", label="$X^{3+}$ Cations")
-    # plot the relative paritioning curve for the site
-    curve3Ds = D_La * strain_coefficient(rLa, xs, r0=r03, E=E_3, T=Tk)
-    ax.plot(xs, curve3Ds, color="0.5", ls="--")
-    # add the element labels next to the points
-    for l, r, d in zip(site3labels, site3radii, site3Ds):
-        ax.annotate(
-            l, xy=(r, d), xycoords="data", ha="right", va="bottom", fontsize=fontsize
-        )
-    ax.set_yscale("log")
-    ax.set_ylabel("$D_X$")
-    ax.set_xlabel("Radii ($\AA$)")
-    fig
-
-
-
-.. image:: /examples/geochem/images/sphx_glr_mineral_lattice_002.png
-    :class: sphx-glr-single-img
-
-
-.. rst-class:: sphx-glr-script-out
-
- Out:
-
- .. code-block:: none
-
-
-    <Figure size 640x480 with 1 Axes>
-
-
-
-As europium is commonly present as a mixture of both :math:`Eu^{2+}`
-and :math:`Eu^{3+}`, the effective partitioning of Eu will be intermediate
-between that of :math:`D_{Eu^{2+}}`and :math:`D_{Eu^{3+}}`. Using a 60:40 mixture
-of :math:`Eu^{3+}` : :math:`Eu^{2+}` as an example, this effective partition
-coefficient can be calculated:
-
-
-
-.. code-block:: default
-
-    X_Eu3 = 0.6
-    # calculate D_Eu3 relative to D_La
-    D_Eu3 = D_La * strain_coefficient(
-        rLa, get_ionic_radii("Eu", charge=3, coordination=8), r0=r03, E=E_3, T=Tk
-    )
-    # calculate D_Eu2 relative to D_Ca
-    D_Eu2 = D_Ca * strain_coefficient(
-        rCa, get_ionic_radii("Eu", charge=2, coordination=8), r0=r02, E=E_2, T=Tk
-    )
-    # calculate the effective parition coefficient
-    D_Eu = (1 - X_Eu3) * D_Eu2 + X_Eu3 * D_Eu3
-    # show the effective partition coefficient relative to the 2+ and 3+ endmembers
-    radii, ds = (
-        [get_ionic_radii("Eu", charge=c, coordination=8) for c in [3, 3, 2, 2]],
-        [D_Eu3, D_Eu, D_Eu, D_Eu2],
-    )
-    ax.plot(
-        radii, ds, ls="--", color="0.9", marker="D", label="Effective $D_{Eu}$", zorder=-1
-    )
-    ax.legend(loc="upper left", bbox_to_anchor=(1.05, 1), frameon=False, facecolor=None)
-    fig
-
-
-
-.. image:: /examples/geochem/images/sphx_glr_mineral_lattice_003.png
-    :class: sphx-glr-single-img
-
-
-.. rst-class:: sphx-glr-script-out
-
- Out:
-
- .. code-block:: none
-
-
-    <Figure size 640x480 with 1 Axes>
-
-
-
-.. [#ref_1] Blundy, J., Wood, B., 1994. Prediction of crystal–melt partition coefficients
-            from elastic moduli. Nature 372, 452.
-            doi: `10.1038/372452A0 <https://doi.org/10.1038/372452A0>`__
-
-.. [#ref_2] Dohmen, R., Blundy, J., 2014. A predictive thermodynamic model for element partitioning
-            between plagioclase and melt as a function of pressure, temperature and composition.
-            American Journal of Science 314, 1319–1372.
-            doi: `10.2475/09.2014.04 <https://doi.org/10.2475/09.2014.04>`__
-
-.. seealso::
-
-  Examples:
-    `Shannon Radii <../indexes/shannon.html>`__,
-    `REE Radii Plot <../plotting/REE_v_radii.html>`__
-
-  Functions:
-    :func:`~pyrolite.mineral.lattice.strain_coefficient`,
-    :func:`~pyrolite.mineral.lattice.youngs_modulus_approximation`,
-    :func:`~pyrolite.geochem.get_ionic_radii`
-
-
-.. rst-class:: sphx-glr-timing
-
-   **Total running time of the script:** ( 0 minutes  1.104 seconds)
-
-
-.. _sphx_glr_download_examples_geochem_mineral_lattice.py:
-
-
-.. only :: html
-
- .. container:: sphx-glr-footer
-    :class: sphx-glr-footer-example
-
-
-  .. container:: binder-badge
-
-    .. image:: https://mybinder.org/badge_logo.svg
-      :target: https://mybinder.org/v2/gh/morganjwilliams/pyrolite/develop?filepath=docs/source/examples/geochem/mineral_lattice.ipynb
-      :width: 150 px
-
-
-  .. container:: sphx-glr-download sphx-glr-download-python
-
-     :download:`Download Python source code: mineral_lattice.py <mineral_lattice.py>`
-
-
-
-  .. container:: sphx-glr-download sphx-glr-download-jupyter
-
-     :download:`Download Jupyter notebook: mineral_lattice.ipynb <mineral_lattice.ipynb>`
-
-
-.. only:: html
-
- .. rst-class:: sphx-glr-signature
-
-    `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
+"""
+Submodule for calculating and modelling melt chemistry. Includes common
+functions for predicting and accounting for melt evolution.
+"""
+import numpy as np
+import periodictable as pt
+
+from ..util.log import Handle
+from ..util.meta import update_docstring_references
+from ..util.units import scale
+from .ind import _common_elements, _common_oxides
+from .transform import to_molecular
+
+logger = Handle(__name__)
+
+
+@update_docstring_references
+def FeAt8MgO(FeOT: float, MgO: float) -> float:
+    """
+    To account for differences in the slopes and curvature of liquid lines of descent
+    as a function of parental magma composition [#ref_1]_ [#ref_2]_ (after [#ref_3]_).
+
+    Parameters
+    -------------
+    FeOT : :class:`float`
+        Iron oxide content.
+    MgO : :class:`float`
+        Magnesium oxide content.
+
+    References
+    -----------
+    .. [#ref_1] Castillo PR, Klein E, Bender J, et al (2000).
+        Petrology and Sr, Nd, and Pb isotope geochemistry of
+        mid-ocean ridge basalt glasses from the 11°45’N to 15°00’N
+        segment of the East Pacific Rise.
+        Geochemistry, Geophysics, Geosystems 1:1.
+        doi: `10.1029/1999GC000024 <https://dx.doi.org/10.1029/1999GC000024>`__
+
+    .. [#ref_2] Klein EM, Langmuir CH (1987).
+        Global correlations of ocean ridge basalt chemistry with
+        axial depth and crustal thickness.
+        Journal of Geophysical Research: Solid Earth 92:8089–8115.
+        doi: `10.1029/JB092iB08p08089 <https://dx.doi.org/10.1029/JB092iB08p08089>`__
+
+    .. [#ref_3] Langmuir CH, Bender JF (1984).
+        The geochemistry of oceanic basalts in the vicinity
+        of transform faults: Observations and implications.
+        Earth and Planetary Science Letters 69:107–127.
+        doi: `10.1016/0012-821X(84)90077-3 <https://dx.doi.org/10.1016/0012-821X(84)90077-3>`__
+    """
+    Fe8 = 1.825 - 1.529 * (FeOT - 0.03261 * MgO**2 + 0.2619) / (
+        MgO - 0.04467 * MgO**2 - 6.67
+    )
+    return Fe8
+
+
+@update_docstring_references
+def NaAt8MgO(Na2O: float, MgO: float) -> float:
+    """
+    To account for differences in the slopes and curvature of liquid lines of descent
+    as a function of parental magma composition [#ref_1]_ [#ref_2]_ (after [#ref_3]_).
+
+    Parameters
+    -------------
+    Na2O : :class:`float`
+        Iron oxide content.
+    MgO : :class:`float`
+        Magnesium oxide content.
+
+    References
+    -----------
+    .. [#ref_1] Castillo PR, Klein E, Bender J, et al (2000).
+        Petrology and Sr, Nd, and Pb isotope geochemistry of
+        mid-ocean ridge basalt glasses from the 11°45’N to 15°00’N
+        segment of the East Pacific Rise.
+        Geochemistry, Geophysics, Geosystems 1:1.
+        doi: `10.1029/1999GC000024 <https://dx.doi.org/10.1029/1999GC000024>`__
+
+    .. [#ref_2] Klein EM, Langmuir CH (1987).
+        Global correlations of ocean ridge basalt chemistry with
+        axial depth and crustal thickness.
+        Journal of Geophysical Research: Solid Earth 92:8089–8115.
+        doi: `10.1029/JB092iB08p08089 <https://dx.doi.org/10.1029/JB092iB08p08089>`__
+
+    .. [#ref_3] Langmuir CH, Bender JF (1984).
+        The geochemistry of oceanic basalts in the vicinity
+        of transform faults: Observations and implications.
+        Earth and Planetary Science Letters 69:107–127.
+        doi: `10.1016/0012-821X(84)90077-3 <https://dx.doi.org/10.1016/0012-821X(84)90077-3>`__
+    """
+    Na8 = 0.6074 - 3.523 * (Na2O + 0.00529 * MgO**2 - 0.9495) / (
+        MgO - 0.05297 * MgO**2 - 8.133
+    )
+    return Na8
+
+
+@update_docstring_references
+def SCSS(df, T, P, kelvin=False, grid=None, outunit="wt%"):
+    r"""
+    Obtain the sulfur content at sulfate and sulfide saturation [#ref_1]_ [#ref_2]_.
+
+    Parameters
+    -------------
+    df : :class:`pandas.DataFrame`
+        Dataframe of compositions.
+    T : :class:`float` | :class:`numpy.ndarray`
+        Temperature
+    P : :class:`float` | :class:`numpy.ndarray`
+        Pressure (kbar)
+    kelvin : :class:`bool`
+        Whether temperature values are in kelvin (:code:`True`) or celsuis (:code:`False`)
+    grid : :code:`None`, :code:`'geotherm'`, :code:`'grid'`
+        Whether to consider temperature and pressure as a geotherm (:code:`geotherm`),
+        or independently (as a grid, :code:`grid`).
+
+    Returns
+    -------
+    sulfate, sulfide : :class:`numpy.ndarray`, :class:`numpy.ndarray`
+        Arrays of mass fraction sulfate and sulfide abundances at saturation.
+
+    Notes
+    ------
+
+    For anhydrite-saturated systems, the sulfur content at sulfate saturation is given
+    by the following:
+
+    .. math::
+
+        \begin{align}
+        ln(X_S) = &10.07
+        - 1.151 \cdot (10^4 / T_K)
+        + 0.104 \cdot P_{kbar}\\
+        &- 7.1 \cdot X_{SiO_2}
+        - 14.02 \cdot X_{MgO}
+        - 14.164 \cdot X_{Al_2O_3}\\
+        \end{align}
+
+    For sulfide-liquid saturated systems, the sulfur content at sulfide saturation is
+    given by the following:
+
+    .. math::
+
+        \begin{align}
+        ln(X_S) = &{-1.76}
+        - 0.474 \cdot (10^4 / T_K)
+        + 0.021 \cdot P_{kbar}\\
+        &+ 5.559 \cdot X_{FeO}
+        + 2.565 \cdot X_{TiO_2}
+        + 2.709 \cdot X_{CaO}\\
+        &- 3.192 \cdot X_{SiO_2}
+        - 3.049 \cdot X_{H_2O}\\
+        \end{align}
+
+    References
+    -----------
+    .. [#ref_1] Li, C., and Ripley, E.M. (2009).
+        Sulfur Contents at Sulfide-Liquid or Anhydrite Saturation in Silicate Melts:
+        Empirical Equations and Example Applications. Economic Geology 104, 405–412.
+        doi: `gsecongeo.104.3.405 <https://doi.org/10.2113/gsecongeo.104.3.405>`__
+
+    .. [#ref_2] Smythe, D.J., Wood, B.J., and Kiseeva, E.S. (2017).
+        The S content of silicate melts at sulfide saturation:
+        New experiments and a model incorporating the effects of sulfide composition.
+        American Mineralogist 102, 795–803.
+        doi: `10.2138/am-2017-5800CCBY <https://doi.org/10.2138/am-2017-5800CCBY>`__
+
+    Todo
+    -----
+    * Produce an updated version based on log-regressions?
+    * Add updates from Smythe et al. (2017)?
+    """
+    T, P = np.array(T, dtype="float"), np.array(P, dtype="float")
+    if not kelvin:
+        T = T + 273.15
+
+    C = np.ones(df.index.size)
+    assert grid in [None, "geotherm", "grid"]
+    if grid == "grid":
+        cc, tt, pp = np.meshgrid(C, T, P, indexing="ij")
+    elif grid == "geotherm":
+        assert T.shape == P.shape
+        cc = C[:, np.newaxis]
+        tt = T[np.newaxis, :]
+        pp = P[np.newaxis, :]
+    elif grid is None:
+        _dims = C.size, T.size, P.size
+        maxdim = max(_dims)
+        assert all([x == maxdim or x == 1 for x in _dims])
+        cc, tt, pp = C, T, P
+
+    comp = list(set(df.columns) & (_common_elements | _common_oxides))
+    moldf = to_molecular(df.loc[:, comp], renorm=True) / 100.0  # mole-fraction
+    molsum = to_molecular(df.loc[:, comp], renorm=False).sum(axis=1)
+
+    def gridify(ser):
+        """
+        Create a parameter grid from a pandas series to facilitate
+        array-addition of each component.
+        """
+        arr = ser.replace(np.nan, 0).values
+        if grid == "grid":
+            return arr[:, np.newaxis, np.newaxis]
+        elif grid == "geotherm":
+            return arr[:, np.newaxis]
+        elif grid is None:
+            return arr
+
+    ln_sulfate = 10.07 * cc - 1.151 * 10**4 / tt + 0.104 * pp
+    for chem, D in [("SiO2", -7.1), ("MgO", -14.02), ("Al2O3", -14.164)]:
+        if chem in moldf.columns:
+            ln_sulfate += gridify(moldf[chem]) * D * cc
+
+    ln_sulfide = -1.76 * cc - 0.474 * 10**4 / tt + 0.021 * pp
+
+    for chem, D in [
+        ("FeO", 5.559),
+        ("TiO2", 2.565),
+        ("CaO", 2.709),
+        ("SiO2", -3.192),
+        ("H2O", -3.049),
+    ]:
+        if chem in moldf.columns:
+            ln_sulfide += gridify(moldf[chem]) * D * cc
+
+    sulfate, sulfide = np.exp(ln_sulfate), np.exp(ln_sulfide)
+
+    _s = gridify(molsum * pt.S.mass) * scale("wt%", outunit)
+    _so4 = gridify(molsum * pt.formula("SO4").mass) * scale("wt%", outunit)
+    sulfide *= _s
+    sulfate *= _so4
+
+    if sulfate.size == 1:  # 0D
+        return sulfate.flatten()[0], sulfide.flatten()[0]
+    else:  # 2D
+        return sulfate, sulfide
```

### Comparing `pyrolite-0.3.3.post0/pyrolite/__init__.py` & `pyrolite-0.3.4/pyrolite/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,7 +40,10 @@
         for r in replace:
             n = n.replace(r, "")
         setattr(extensions, n, m)
 
 
 # _export_pyrolite_mplstyle() should be called in .plot import regardless
 matplotlib.style.use("pyrolite")
+
+from . import _version
+__version__ = _version.get_versions()['version']
```

### Comparing `pyrolite-0.3.3.post0/pyrolite/comp/__init__.py` & `pyrolite-0.3.4/pyrolite/comp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/comp/aggregate.py` & `pyrolite-0.3.4/pyrolite/comp/aggregate.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/comp/codata.py` & `pyrolite-0.3.4/pyrolite/comp/codata.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,15 @@
 
     indicies = np.arange(1, p + 1)[::-1]
     for ix in indicies:  # we have to recurse from p back down to #2
         if ix == p:
             S = 1
         else:
             # vector - the product of sin components
-            S = np.product(np.sin(θ[:, ix:]), axis=1)
+            S = np.prod(np.sin(θ[:, ix:]), axis=1)
             # where this evaluates to zero, the composition is all in the first component
             S[np.isclose(S, 0.0)] = 1.0
 
         ratios = _ys[:, ix] / S
         # where this looks like it could be slightly higher than 1
         # np.arcos will return np.nan, so we can filter these.
         ratios[np.isclose(ratios, 1.0)] = 1.0
```

### Comparing `pyrolite-0.3.3.post0/pyrolite/comp/impute.py` & `pyrolite-0.3.4/pyrolite/comp/impute.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/Aitchison/__init__.py` & `pyrolite-0.3.4/pyrolite/data/Aitchison/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/Aitchison/boxite.csv` & `pyrolite-0.3.4/pyrolite/data/Aitchison/boxite.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/Aitchison/coxite.csv` & `pyrolite-0.3.4/pyrolite/data/Aitchison/coxite.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/Aitchison/hongite.csv` & `pyrolite-0.3.4/pyrolite/data/Aitchison/hongite.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/Aitchison/kongite.csv` & `pyrolite-0.3.4/pyrolite/data/Aitchison/kongite.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/_config/pyrolite.mplstyle` & `pyrolite-0.3.4/pyrolite/data/_config/pyrolite.mplstyle`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/geochemdb.json` & `pyrolite-0.3.4/pyrolite/data/geochem/geochemdb.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/ARS_Condie1993.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/ARS_Condie1993.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/BCC_McLennan2001.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/BCC_McLennan2001.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/BCC_RudnickGao2003.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/BCC_RudnickGao2003.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/BCC_RudnickGao2014.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/BCC_RudnickGao2014.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/CH_McDonoughSun1995.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/CH_McDonoughSun1995.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/CH_PalmeONeill2014.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/CH_PalmeONeill2014.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/CH_REE_ONeill2016.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/CH_REE_ONeill2016.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/CH_SunMcDonough1989.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/CH_SunMcDonough1989.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/DDMM_WorkmanHart2005.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/DDMM_WorkmanHart2005.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/DMM_WorkmanHart2005.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/DMM_WorkmanHart2005.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/DMORB_Gale2013.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/DMORB_Gale2013.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/DM_SaltersStrake2004.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/DM_SaltersStrake2004.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/EDMM_WorkmanHart2005.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/EDMM_WorkmanHart2005.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/EMORB_Gale2013.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/EMORB_Gale2013.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/EMORB_SunMcDonough1989.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/EMORB_SunMcDonough1989.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/EUS_Bau2018.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/EUS_Bau2018.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/GLOSS2_Plank2014.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/GLOSS2_Plank2014.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/GLOSS_Plank2014.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/GLOSS_Plank2014.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/LCC_McLennan2001.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/LCC_McLennan2001.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/LCC_RudnickGao2003.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/LCC_RudnickGao2003.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/LCC_RudnickGao2014.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/LCC_RudnickGao2014.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/MCC_RudnickGao2014.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/MCC_RudnickGao2014.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/MORB_Gale2013.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/MORB_Gale2013.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/MUQ_Kamber2005.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/MUQ_Kamber2005.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/NASC_Gromet1984.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/NASC_Gromet1984.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/NMORB_Gale2013.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/NMORB_Gale2013.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/NMORB_SunMcDonough1989.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/NMORB_SunMcDonough1989.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/OIB_SunMcDonough1989.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/OIB_SunMcDonough1989.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PAAS_Pourmand2012.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PAAS_Pourmand2012.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PAAS_TaylorMcLennan1985.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PAAS_TaylorMcLennan1985.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PHS_Condie1993.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PHS_Condie1993.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PM_PalmeONeill2014.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PM_PalmeONeill2014.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PM_SunMcDonough1989.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PM_SunMcDonough1989.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PRS_Condie1993.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PRS_Condie1993.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/PY_McDonoughSun1995.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/PY_McDonoughSun1995.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/UCC_McLennan2001.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/UCC_McLennan2001.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/UCC_RudnickGao2003.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/UCC_RudnickGao2003.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp/UCC_RudnickGao2014.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp/UCC_RudnickGao2014.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refcomp_template.csv` & `pyrolite-0.3.4/pyrolite/data/geochem/refcomp_template.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/geochem/refdb.json` & `pyrolite-0.3.4/pyrolite/data/geochem/refdb.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/mineral/mindb.json` & `pyrolite-0.3.4/pyrolite/data/mineral/mindb.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/mineral/mins.csv` & `pyrolite-0.3.4/pyrolite/data/mineral/mins.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/FeldsparTernary/config.json` & `pyrolite-0.3.4/pyrolite/data/models/FeldsparTernary/config.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/JensenPlot/config.json` & `pyrolite-0.3.4/pyrolite/data/models/JensenPlot/config.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/QAP/config.json` & `pyrolite-0.3.4/pyrolite/data/models/QAP/config.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/SpinelFeBivariate/config.json` & `pyrolite-0.3.4/pyrolite/data/models/SpinelFeBivariate/config.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/SpinelTrivalentTernary/config.json` & `pyrolite-0.3.4/pyrolite/data/models/SpinelTrivalentTernary/config.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/TAS/config.json` & `pyrolite-0.3.4/pyrolite/data/models/TAS/config.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/TAS/config_lemaitre.json` & `pyrolite-0.3.4/pyrolite/data/models/TAS/config_lemaitre.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/TAS/config_lemaitre_combined.json` & `pyrolite-0.3.4/pyrolite/data/models/TAS/config_lemaitre_combined.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/TAS.clsf.gz` & `pyrolite-0.3.4/pyrolite/data/models/TAS.clsf.gz`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/USDASoilTexture/config.json` & `pyrolite-0.3.4/pyrolite/data/models/USDASoilTexture/config.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/sandstones/config_herron.json` & `pyrolite-0.3.4/pyrolite/data/models/sandstones/config_herron.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/models/sandstones/config_pettijohn.json` & `pyrolite-0.3.4/pyrolite/data/models/sandstones/config_pettijohn.json`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/radii/shannon.csv` & `pyrolite-0.3.4/pyrolite/data/radii/shannon.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/radii/whittaker_muntus.csv` & `pyrolite-0.3.4/pyrolite/data/radii/whittaker_muntus.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/testing/CIPW_Verma_Test.csv` & `pyrolite-0.3.4/pyrolite/data/testing/CIPW_Verma_Test.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/timescale/geotimescale_201807.csv` & `pyrolite-0.3.4/pyrolite/data/timescale/geotimescale_201807.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/timescale/geotimescale_202003.csv` & `pyrolite-0.3.4/pyrolite/data/timescale/geotimescale_202003.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/timescale/geotimescale_202210.csv` & `pyrolite-0.3.4/pyrolite/data/timescale/geotimescale_202210.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/data/timescale/timecolors.csv` & `pyrolite-0.3.4/pyrolite/data/timescale/timecolors.csv`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/__init__.py` & `pyrolite-0.3.4/pyrolite/geochem/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/alteration.py` & `pyrolite-0.3.4/pyrolite/geochem/alteration.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/ind.py` & `pyrolite-0.3.4/pyrolite/geochem/ind.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/ions.py` & `pyrolite-0.3.4/pyrolite/geochem/ions.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/isotope/__init__.py` & `pyrolite-0.3.4/pyrolite/geochem/isotope/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/isotope/count.py` & `pyrolite-0.3.4/pyrolite/geochem/isotope/count.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/norm.py` & `pyrolite-0.3.4/pyrolite/geochem/norm.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/parse.py` & `pyrolite-0.3.4/pyrolite/geochem/parse.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/quality/__init__.py` & `pyrolite-0.3.4/pyrolite/geochem/quality/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/geochem/transform.py` & `pyrolite-0.3.4/pyrolite/geochem/transform.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/mineral/mindb.py` & `pyrolite-0.3.4/pyrolite/mineral/mindb.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/mineral/normative.py` & `pyrolite-0.3.4/pyrolite/mineral/normative.py`

 * *Files 2% similar despite different names*

```diff
@@ -663,14 +663,16 @@
 
     # convert to a single set of oxides and gas traces
     df = df.pyrochem.convert_chemistry(to=majors + minors_trace, renorm=False).fillna(0)
 
     df["SO3"] = SO3
     df["S"] = S
 
+    minors_trace.append("SO3")
+
     ############################################################################
     # Normalization
     # Adjust majors wt% to 100% then adjust again to account for trace components
     ############################################################################
     # Rounding to 3 dp
     df[majors] = df[majors].round(rounding)
 
@@ -774,15 +776,15 @@
     minerals["Fe-Hy"]["mass"] = df["MW_FeO_corr"] + pt.formula("SiO2").mass
     minerals["Fe-Ol"]["mass"] = (2 * df["MW_FeO_corr"]) + pt.formula("SiO2").mass
     minerals["Mt"]["mass"] = df["MW_FeO_corr"] + pt.formula("Fe2O3").mass
     minerals["Il"]["mass"] = df["MW_FeO_corr"] + pt.formula("TiO2").mass
     minerals["An"]["mass"] = df["MW_CaO_corr"] + pt.formula("Al2O3 (SiO2)2").mass
     minerals["Mg-Di"]["mass"] = df["MW_CaO_corr"] + pt.formula("MgO (SiO2)2").mass
     minerals["Wo"]["mass"] = df["MW_CaO_corr"] + pt.formula("SiO2").mass
-    minerals["Cs"]["mass"] = 2 * df["MW_CaO_corr"] + pt.formula("SiO2").mass
+    minerals["Cs"]["mass"] = (2 * df["MW_CaO_corr"]) + pt.formula("SiO2").mass
     minerals["Tn"]["mass"] = df["MW_CaO_corr"] + pt.formula("TiO2 SiO2").mass
     minerals["Pf"]["mass"] = df["MW_CaO_corr"] + pt.formula("TiO2").mass
     minerals["CaF2-Ap"]["mass"] = (
         3 * df["MW_CaO_corr"]
         + (1 / 3) * df["MW_Ca_corr"]
         + (2 / 3) * pt.F.mass
         + pt.formula("P2O5").mass
@@ -823,15 +825,15 @@
         df["CaO"] >= (3 + 1 / 3) * df["P2O5"], df["P2O5"], df["CaO"] / (3 + 1 / 3)
     ).T
 
     df["CaO_"] = np.where(
         df["CaO"] >= (3 + 1 / 3) * df["P2O5"], df["CaO"] - (3 + 1 / 3) * df["Ap"], 0
     ).T
 
-    df["P2O5"] = np.where(
+    df["P2O5_"] = np.where(
         df["CaO"] < (3 + 1 / 3) * df["P2O5"], df["P2O5"] - df["Ap"], 0
     ).T
 
     df["CaO"] = df["CaO_"]
 
     # apatite options where F in present
 
@@ -847,93 +849,103 @@
 
     df["Ap"] = np.where(
         df["ap_option"] == 3, df["CaF2-Ap"] + df["CaO-Ap"], df["Ap"].T
     ).T
 
     df["F"] = np.where(df["ap_option"] == 3, 0, df["F"]).T
 
-    df["FREE_P2O5"] = df["P2O5"]
+    df["FREE_P2O5"] = df["P2O5_"]
 
     df["FREEO_12b"] = np.where(df["ap_option"] == 2, 1 / 3 * df["Ap"], 0).T
     df["FREEO_12c"] = np.where(df["ap_option"] == 3, df["F"] / 2, 0).T
 
     # Normative Fluorite
     df["Fr"] = np.where(df["CaO"] >= df["F"] / 2, df["F"] / 2, df["CaO"]).T
 
-    df["CaO"] = np.where(df["CaO"] >= df["F"] / 2, df["CaO"] - df["Fr"], 0).T
+    df["CaO_"] = np.where(df["CaO"] >= df["F"] / 2, df["CaO"] - df["Fr"], 0).T
 
-    df["F"] = np.where(df["CaO"] >= df["F"] / 2, df["F"], df["F"] - (2 * df["Fr"])).T
+    df["F"] = np.where(df["CaO"] >= df["F"] / 2, 0, df["F"] - (2 * df["Fr"])).T
 
+    df["CaO"] = df["CaO_"]
     df["FREEO_13"] = df["Fr"]
     df["FREE_F"] = df["F"]
 
     # Normative halite
-    df["Hl"] = np.where(df["Na2O"] >= 2 * df["Cl"], df["Cl"], df["Na2O"] / 2).T
+    df["Hl"] = np.where(df["Na2O"] >= (2 * df["Cl"]), df["Cl"], df["Na2O"]/2).T
+
+    df["Na2O_"] = np.where(df["Na2O"] >= (2 * df["Cl"]), df["Na2O"] - df["Hl"]/2, 0).T
 
-    df["Na2O"] = np.where(df["Na2O"] >= 2 * df["Cl"], df["Na2O"] - df["Hl"] / 2, 0).T
+    df["Cl"] = np.where(df["Na2O"] >= (2 * df["Cl"]), 0, df["Cl"] - df["Hl"]).T
 
-    df["Cl"] = np.where(df["Na2O"] >= 2 * df["Cl"], df["Cl"], df["Cl"] - df["Hl"]).T
+    df["Na2O"] = df["Na2O_"]
 
     df["FREE_Cl"] = df["Cl"]
     df["FREEO_14"] = df["Hl"] / 2
 
     # Normative thenardite
-    df["Th"] = np.where((df["SO3"] > 0) & (df["Na2O"] >= df["SO3"]), df["SO3"], 0).T
     df["Th"] = np.where(
-        (df["SO3"] > 0) & (df["Na2O"] < df["SO3"]), df["Na2O"], df["Th"]
+        df["Na2O"] >= df["SO3"], df["SO3"], df["Na2O"]
     ).T
 
     df["Na2O_"] = np.where(
-        (df["SO3"] > 0) & (df["Na2O"] >= df["SO3"]), df["Na2O"] - df["Th"], df["Na2O"]
+        df["Na2O"] >= df["SO3"], df["Na2O"] - df["Th"], 0
     ).T
 
-    df["Na2O"] = np.where((df["SO3"] > 0) & (df["Na2O"] < df["SO3"]), 0, df["Na2O_"]).T
-
     df["SO3"] = np.where(
-        (df["SO3"] > 0) & (df["Na2O"] < df["SO3"]), df["SO3"] - df["Th"], df["SO3"]
+        df["Na2O"] >= df["SO3"], 0, df["SO3"] - df["Th"]
     ).T
 
+    df["Na2O"] = df["Na2O_"]
+
     df["FREE_SO3"] = df["SO3"]
 
     # Normative Pyrite
-    df["Pr"] = np.where(df["FeO"] >= 2 * df["S"], df["S"] / 2, df["S"]).T
+    df["Pr"] = np.where(df["FeO"] >= 2 * df["S"], df["S"] / 2, df["FeO"]).T
 
     df["FeO_"] = np.where(df["FeO"] >= 2 * df["S"], df["FeO"] - df["Pr"], 0).T
 
-    df["FeO"] = np.where(df["S"] > 0, df["FeO_"], df["FeO"]).T
+    df["S"] = np.where(df["FeO"] >= 2 * df["S"], 0, df["S"] - 2*df['Pr']).T
 
-    df["FREE_S"] = np.where(df["FeO"] >= 2 * df["S"], 0, df["S"]).T
+    df["FeO"] = df["FeO_"]
 
+    df['FREE_S'] = df['S']
     df["FREEO_16"] = df["Pr"]
 
     # Normative sodium carbonate (cancrinite) or calcite
 
     df["Nc"] = np.where(df["Na2O"] >= df["CO2"], df["CO2"], df["Na2O"]).T
 
-    df["Na2O"] = np.where(df["Na2O"] >= df["CO2"], df["Na2O"] - df["Nc"], df["Na2O"]).T
+    df["Na2O_"] = np.where(df["Na2O"] >= df["CO2"], df["Na2O"] - df["Nc"], 0).T
+
+    df["CO2"] = np.where(df["Na2O"] >= df["CO2"], 0, df["CO2"] - df["Nc"]).T
 
-    df["CO2"] = np.where(df["Na2O"] >= df["CO2"], df["CO2"], df["CO2"] - df["Nc"]).T
+    df['Na2O'] = df['Na2O_']
 
     df["Cc"] = np.where(df["CaO"] >= df["CO2"], df["CO2"], df["CaO"]).T
 
-    df["CaO"] = np.where(df["Na2O"] >= df["CO2"], df["CaO"] - df["Cc"], df["CaO"]).T
+    df["CaO_"] = np.where(df["CaO"] >= df["CO2"], df["CaO"] - df["Cc"], 0).T
 
-    df["CO2"] = np.where(df["Na2O"] >= df["CO2"], df["CO2"], df["CO2"] - df["Cc"]).T
+    df["CO2"] = np.where(df["CaO"] >= df["CO2"], 0, df["CO2"] - df["Cc"]).T
+
+    df['CaO'] = df['CaO_']
 
     df["FREECO2"] = df["CO2"]
 
     # Normative Chromite
     df["Cm"] = np.where(df["FeO"] >= df["Cr2O3"], df["Cr2O3"], df["FeO"]).T
 
-    df["FeO"] = np.where(df["FeO"] >= df["Cr2O3"], df["FeO"] - df["Cm"], 0).T
+    df["FeO_"] = np.where(df["FeO"] >= df["Cr2O3"], df["FeO"] - df["Cm"], 0).T
+    
     df["Cr2O3"] = np.where(
         df["FeO"] >= df["Cr2O3"], df["Cr2O3"] - df["Cm"], df["Cr2O3"]
     ).T
 
-    df["FREE_CR2O3"] = df["Cm"]
+    df["FeO"] = df["FeO_"]
+
+    df["FREE_CR2O3"] = df["Cr2O3"]
 
     # Normative Ilmenite
     df["Il"] = np.where(df["FeO"] >= df["TiO2"], df["TiO2"], df["FeO"]).T
 
     df["FeO_"] = np.where(df["FeO"] >= df["TiO2"], df["FeO"] - df["Il"], 0).T
 
     df["TiO2_"] = np.where(df["FeO"] >= df["TiO2"], 0, df["TiO2"] - df["Il"]).T
@@ -1068,15 +1080,15 @@
     df["deficit"] = df["D"] > 0
 
     # Normative Olivine / Hypersthene
     df["Ol_"] = np.where((df["D"] < df["Hy_p"] / 2), df["D"], df["Hy_p"] / 2).T
 
     df["Hy"] = np.where((df["D"] < df["Hy_p"] / 2), df["Hy_p"] - 2 * df["D"], 0).T
 
-    df["D1"] = df["D"] - df["Hy_p"] / 2
+    df["D1"] = df["D"] - (df["Hy_p"] / 2)
 
     df["Ol"] = np.where((df["deficit"]), df["Ol_"], 0).T
 
     df["Hy"] = np.where((df["deficit"]), df["Hy"], df["Hy_p"]).T
 
     df["deficit"] = df["D1"] > 0
 
@@ -1089,17 +1101,17 @@
 
     df["Tn"] = np.where((df["deficit"]), df["Tn"], df["Tn_p"]).T
     df["Pf"] = np.where((df["deficit"]), df["Pf_"], 0).T
 
     df["deficit"] = df["D2"] > 0
 
     # Normative Nepheline / Albite
-    df["Ne_"] = np.where((df["D2"] < 4 * df["Ab_p"]), df["D2"] / 4, df["Ab_p"]).T
+    df["Ne_"] = np.where(df["D2"] < 4 * df["Ab_p"], df["D2"] / 4, df["Ab_p"]).T
 
-    df["Ab"] = np.where((df["D2"] < 4 * df["Ab_p"]), df["Ab_p"] - df["D2"] / 4, 0).T
+    df["Ab"] = np.where(df["D2"] < 4 * df["Ab_p"], df["Ab_p"] - df["D2"] / 4, 0).T
 
     df["D3"] = df["D2"] - 4 * df["Ab_p"]
 
     df["Ne"] = np.where((df["deficit"]), df["Ne_"], 0).T
     df["Ab"] = np.where((df["deficit"]), df["Ab"], df["Ab_p"]).T
 
     df["deficit"] = df["D3"] > 0
@@ -1290,8 +1302,8 @@
             FREE.rename(
                 columns={
                     c: "FREE_" + c for c in FREE.columns if "FREE" not in c.upper()
                 }
             )
         )
 
-    return pd.concat(outputs, axis=1).round(rounding)
+    return pd.concat(outputs, axis=1).round(rounding)
```

### Comparing `pyrolite-0.3.3.post0/pyrolite/mineral/sites.py` & `pyrolite-0.3.4/pyrolite/mineral/sites.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/mineral/template.py` & `pyrolite-0.3.4/pyrolite/mineral/template.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/mineral/transform.py` & `pyrolite-0.3.4/pyrolite/mineral/transform.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/__init__.py` & `pyrolite-0.3.4/pyrolite/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/biplot.py` & `pyrolite-0.3.4/pyrolite/plot/biplot.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/color.py` & `pyrolite-0.3.4/pyrolite/plot/color.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/density/__init__.py` & `pyrolite-0.3.4/pyrolite/plot/density/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/density/grid.py` & `pyrolite-0.3.4/pyrolite/plot/density/grid.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/density/ternary.py` & `pyrolite-0.3.4/pyrolite/plot/density/ternary.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/parallel.py` & `pyrolite-0.3.4/pyrolite/plot/parallel.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/spider.py` & `pyrolite-0.3.4/pyrolite/plot/spider.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/stem.py` & `pyrolite-0.3.4/pyrolite/plot/stem.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/QAP.py` & `pyrolite-0.3.4/pyrolite/plot/templates/QAP.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/TAS.py` & `pyrolite-0.3.4/pyrolite/plot/templates/TAS.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/USDA_soil_texture.py` & `pyrolite-0.3.4/pyrolite/plot/templates/USDA_soil_texture.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/__init__.py` & `pyrolite-0.3.4/pyrolite/plot/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/components.py` & `pyrolite-0.3.4/pyrolite/plot/templates/components.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/feldspar.py` & `pyrolite-0.3.4/pyrolite/plot/templates/feldspar.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/jensen.py` & `pyrolite-0.3.4/pyrolite/plot/templates/jensen.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/pearce.py` & `pyrolite-0.3.4/pyrolite/plot/templates/pearce.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/sandstones.py` & `pyrolite-0.3.4/pyrolite/plot/templates/sandstones.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/plot/templates/spinel.py` & `pyrolite-0.3.4/pyrolite/plot/templates/spinel.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/classification.py` & `pyrolite-0.3.4/pyrolite/util/classification.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/database.py` & `pyrolite-0.3.4/pyrolite/util/database.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/distributions.py` & `pyrolite-0.3.4/pyrolite/util/distributions.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/env.py` & `pyrolite-0.3.4/pyrolite/util/env.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/general.py` & `pyrolite-0.3.4/pyrolite/util/general.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/lambdas/__init__.py` & `pyrolite-0.3.4/pyrolite/util/lambdas/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/lambdas/eval.py` & `pyrolite-0.3.4/pyrolite/util/lambdas/eval.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/lambdas/oneill.py` & `pyrolite-0.3.4/pyrolite/util/lambdas/oneill.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/lambdas/opt.py` & `pyrolite-0.3.4/pyrolite/util/lambdas/opt.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/lambdas/params.py` & `pyrolite-0.3.4/pyrolite/util/lambdas/params.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/lambdas/plot.py` & `pyrolite-0.3.4/pyrolite/util/lambdas/plot.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/lambdas/transform.py` & `pyrolite-0.3.4/pyrolite/util/lambdas/transform.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/log.py` & `pyrolite-0.3.4/pyrolite/util/log.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/math.py` & `pyrolite-0.3.4/pyrolite/util/math.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/meta.py` & `pyrolite-0.3.4/pyrolite/util/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     subfolder : :class:`str`
         Subfolder within the module data folder.
 
     Returns
     -------
     :class:`pathlib.Path`
     """
-    pth = (
-        Path(importlib.machinery.PathFinder().find_spec(module).origin).parent / "data"
-    )
+    pth = Path(importlib.util.find_spec(module).origin).parent / "data"
     if subfolder:
         pth /= subfolder
     return pth
 
 
 def pyrolite_datafolder(subfolder=None):
     """
```

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/missing.py` & `pyrolite-0.3.4/pyrolite/util/missing.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/multip.py` & `pyrolite-0.3.4/pyrolite/util/multip.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/pd.py` & `pyrolite-0.3.4/pyrolite/util/pd.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/__init__.py` & `pyrolite-0.3.4/pyrolite/util/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/axes.py` & `pyrolite-0.3.4/pyrolite/util/plot/axes.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/density.py` & `pyrolite-0.3.4/pyrolite/util/plot/density.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/export.py` & `pyrolite-0.3.4/pyrolite/util/plot/export.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/grid.py` & `pyrolite-0.3.4/pyrolite/util/plot/grid.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/helpers.py` & `pyrolite-0.3.4/pyrolite/util/plot/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/interpolation.py` & `pyrolite-0.3.4/pyrolite/util/plot/interpolation.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/legend.py` & `pyrolite-0.3.4/pyrolite/util/plot/legend.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/style.py` & `pyrolite-0.3.4/pyrolite/util/plot/style.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/plot/transform.py` & `pyrolite-0.3.4/pyrolite/util/plot/transform.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/resampling.py` & `pyrolite-0.3.4/pyrolite/util/resampling.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/skl/helpers.py` & `pyrolite-0.3.4/pyrolite/util/skl/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/skl/impute.py` & `pyrolite-0.3.4/pyrolite/util/skl/impute.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/skl/pipeline.py` & `pyrolite-0.3.4/pyrolite/util/skl/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/skl/select.py` & `pyrolite-0.3.4/pyrolite/util/skl/select.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/skl/transform.py` & `pyrolite-0.3.4/pyrolite/util/skl/transform.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/skl/vis.py` & `pyrolite-0.3.4/pyrolite/util/skl/vis.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/spatial.py` & `pyrolite-0.3.4/pyrolite/util/spatial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """
 Baisc spatial utility functions.
 """
 import itertools
 
 import numpy as np
-from psutil import virtual_memory  # memory check
+
+try:
+    from psutil import virtual_memory  # memory check
+except ImportError:
+    virtual_memory = None
 
 from .log import Handle
 
 logger = Handle(__name__)
 
 
 def _get_sqare_grid_segment_indicies(size, segments):
@@ -172,22 +176,24 @@
             f = _vicenty_GC_distance
 
     if matrix:
         # if matrix mode we need to turn these 1d arrays into 2d
         # but, with large arrays it'll spit out a memory error
         # so instead we can try to build it numerically
         size = np.max([a.shape[0] for a in [φ1, φ2, λ1, λ2]])
-        mem = virtual_memory().total  # total physical memory available
         estimated_matrix_size = np.array([[1.0]], dtype=dtype).nbytes * size**2
         logger.debug(
             "Attempting to build {}x{} array of size {:.2f} Gb.".format(
                 size, size, estimated_matrix_size / 1024**3
             )
         )
-        if estimated_matrix_size > (mem * max_memory_fraction):
+
+        infeasible = estimated_matrix_size > (virtual_memory().total * max_memory_fraction) if virtual_memory is not None else False
+
+        if infeasible:
             logger.warn(
                 "Angle array for segmented distance matrix larger than maximum memory "
                 "fraction, computing mean global distances instead."
             )
             angle = np.zeros((size, 1))
             # compute sum-distances for each lat-long pair
             for ix, (_φ1, _λ1) in enumerate(np.vstack([φ1, λ1])):
```

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/synthetic.py` & `pyrolite-0.3.4/pyrolite/util/synthetic.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/text.py` & `pyrolite-0.3.4/pyrolite/util/text.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/time.py` & `pyrolite-0.3.4/pyrolite/util/time.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/units.py` & `pyrolite-0.3.4/pyrolite/util/units.py`

 * *Files identical despite different names*

### Comparing `pyrolite-0.3.3.post0/pyrolite/util/web.py` & `pyrolite-0.3.4/pyrolite/util/web.py`

 * *Files identical despite different names*

