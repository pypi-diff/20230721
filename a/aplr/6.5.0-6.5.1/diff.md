# Comparing `tmp/aplr-6.5.0.tar.gz` & `tmp/aplr-6.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aplr-6.5.0.tar", last modified: Fri Jul 14 20:09:12 2023, max compression
+gzip compressed data, was "aplr-6.5.1.tar", last modified: Fri Jul 21 18:19:07 2023, max compression
```

## Comparing `aplr-6.5.0.tar` & `aplr-6.5.1.tar`

### file list

```diff
@@ -1,2036 +1,2036 @@
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.333572 aplr-6.5.0/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1113 2022-05-12 19:01:46.000000 aplr-6.5.0/LICENSE
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      152 2023-07-14 16:07:35.000000 aplr-6.5.0/MANIFEST.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      614 2023-07-14 20:09:12.333572 aplr-6.5.0/PKG-INFO
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1175 2023-05-24 16:05:01.000000 aplr-6.5.0/README.md
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.917570 aplr-6.5.0/aplr/
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)       19 2022-05-09 14:53:50.000000 aplr-6.5.0/aplr/__init__.py
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    13640 2023-07-04 15:26:35.000000 aplr-6.5.0/aplr/aplr.py
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.917570 aplr-6.5.0/aplr.egg-info/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      614 2023-07-14 20:09:11.000000 aplr-6.5.0/aplr.egg-info/PKG-INFO
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   112326 2023-07-14 20:09:11.000000 aplr-6.5.0/aplr.egg-info/SOURCES.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)        1 2023-07-14 20:09:11.000000 aplr-6.5.0/aplr.egg-info/dependency_links.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       12 2023-07-14 20:09:11.000000 aplr-6.5.0/aplr.egg-info/requires.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       14 2023-07-14 20:09:11.000000 aplr-6.5.0/aplr.egg-info/top_level.txt
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.921570 aplr-6.5.0/cpp/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12294 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/APLRClassifier.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    74406 2023-07-14 17:14:55.000000 aplr-6.5.0/cpp/APLRRegressor.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.905570 aplr-6.5.0/cpp/build/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.905570 aplr-6.5.0/cpp/build/CMakeFiles/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.905570 aplr-6.5.0/cpp/build/CMakeFiles/3.16.3/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.921570 aplr-6.5.0/cpp/build/CMakeFiles/3.16.3/CompilerIdCXX/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20091 2022-05-12 20:45:33.000000 aplr-6.5.0/cpp/build/CMakeFiles/3.16.3/CompilerIdCXX/CMakeCXXCompilerId.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      321 2023-05-24 16:05:01.000000 aplr-6.5.0/cpp/constants.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18214 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/functions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1825 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/main.cpp
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    19771 2023-07-04 15:26:35.000000 aplr-6.5.0/cpp/pythonbinding.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28325 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/term.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2033 2023-07-14 17:03:30.000000 aplr-6.5.0/cpp/test ALRRegressor cauchy group_mse validation.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1903 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor cauchy.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3465 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor custom loss and validation.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3084 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor custom loss.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2623 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor gamma custom_link.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2281 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor gamma custom_validation.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1951 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor gamma gini weighted.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1951 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor gamma gini.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1949 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor gamma rank unweighted.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1949 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor gamma rank.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1941 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor gamma.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1987 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor group_mse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1990 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor int constr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1980 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor inversegaussian.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1975 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor logit.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1910 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor mae.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2055 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor monotonic.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2021 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor negative_binomial.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1974 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor poisson.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2011 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor poissongamma.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1893 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor quantile.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2436 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor rank.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1937 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor weibull.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2484 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test ALRRegressor.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4205 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test APLRClassifier multi_class other_params.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4178 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test APLRClassifier multi_class.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2991 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test APLRClassifier two_class other_params.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2931 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test APLRClassifier two_class val_index.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2872 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test APLRClassifier two_class.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5005 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test functions.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4067 2023-07-14 16:07:35.000000 aplr-6.5.0/cpp/test term.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.913570 aplr-6.5.0/dependencies/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.929570 aplr-6.5.0/dependencies/eigen-3.4.0/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      292 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/.gitignore
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.905570 aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.929570 aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab/issue_templates/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2744 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab/issue_templates/Bug Report.md
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      201 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab/issue_templates/Feature Request.md
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.929570 aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab/merge_request_templates/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1394 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab/merge_request_templates/Merge Request Template.md
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      571 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab-ci.yml
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/.hgeol
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24767 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11362 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.APACHE
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1517 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.BSD
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35147 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.GPL
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26530 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.LGPL
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2193 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.MINPACK
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16726 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.MPL2
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      779 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.README
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      584 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/CTestConfig.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/CTestCustom.cmake.in
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.937570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1161 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Cholesky
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1900 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/CholmodSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12799 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Core
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      122 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Dense
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       35 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Eigen
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1777 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Eigenvalues
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1940 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Geometry
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      829 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Householder
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2083 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/IterativeLinearSolvers
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      894 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Jacobi
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1389 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/KLUSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1268 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/LU
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      991 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/MetisSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2451 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/OrderingMethods
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1751 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/PaStiXSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1116 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/PardisoSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1272 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/QR
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      900 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/QtAlignedMalloc
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1162 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SPQRSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1584 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SVD
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      888 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Sparse
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1235 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SparseCholesky
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2240 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SparseCore
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1814 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SparseLU
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1195 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SparseQR
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      797 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/StdDeque
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      726 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/StdList
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      803 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/StdVector
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2243 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SuperLUSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1382 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/UmfPackSupport
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.909570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.937570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Cholesky/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24934 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LDLT.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18760 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LLT.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3974 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.937570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/CholmodSupport/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25441 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.949570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19214 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ArithmeticSequence.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16782 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Array.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8217 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ArrayBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7018 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ArrayWrapper.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2738 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Assign.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    41673 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/AssignEvaluator.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    12488 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Assign_MKL.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14075 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/BandMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18648 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Block.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4429 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/BooleanRedux.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5981 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CommaInitializer.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6990 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ConditionEstimator.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    63841 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CoreEvaluators.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4745 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CoreIterators.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7909 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseBinaryOp.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    36282 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8256 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseTernaryOp.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3937 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5551 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    31529 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DenseBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24484 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25360 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DenseStorage.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9870 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Diagonal.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14670 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      988 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DiagonalProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11654 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Dot.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5841 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/EigenBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4909 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5759 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Fuzzy.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21679 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/GeneralProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    38812 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/GenericPacketMath.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11543 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/GlobalFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8238 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/IO.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9620 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/IndexedView.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3503 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Inverse.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7256 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Map.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11281 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/MapBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    60784 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/MathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7156 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/MathFunctionsImpl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24343 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Matrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23856 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/MatrixBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2520 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/NestByValue.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3620 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/NoAlias.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12884 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/NumTraits.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9207 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/PartialReduxEvaluator.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20748 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/PermutationMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    49193 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/PlainObjectBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7336 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Product.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    53832 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ProductEvaluators.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7756 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Random.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19195 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Redux.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17821 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Ref.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5656 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Replicate.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17033 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Reshaped.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4284 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ReturnByValue.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7522 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Reverse.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6143 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Select.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14999 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/SelfAdjointView.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1697 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6837 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Solve.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9368 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/SolveTriangular.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6170 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/SolverBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8700 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/StableNorm.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21641 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/StlIterators.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4212 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Stride.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2765 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Swap.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17606 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Transpose.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13567 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Transpositions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    38277 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/TriangularMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3488 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/VectorBlock.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35168 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/VectorwiseOp.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11997 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Visitor.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.905570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.949570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15223 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/Complex.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8102 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    64608 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2564 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.949570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17160 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/Complex.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13344 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    87891 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2134 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.953570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16540 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2323 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   119355 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9490 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24820 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)   102394 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.953570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/CUDA/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17317 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/CUDA/Complex.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.953570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26903 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/BFloat16.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5251 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    67696 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3770 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35534 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/Half.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1746 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/Settings.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3746 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.953570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2695 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    57047 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2256 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.905570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/HIP/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.953570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      691 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.953570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17541 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/Complex.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16159 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    33615 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.957570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22503 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/Complex.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6815 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3083 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   189525 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    51286 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.957570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14251 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/Complex.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6765 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    64465 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3650 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.957570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1194 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21200 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1351 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.957570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7428 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12539 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    27786 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21856 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2626 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.957570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16728 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/Complex.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8024 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    36894 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.961570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6686 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20921 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/BinaryFunctors.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8334 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/NullaryFunctors.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4998 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/StlFunctors.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      607 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/TernaryFunctors.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40146 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/UnaryFunctors.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.961570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   108448 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20104 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15948 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6936 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5106 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21724 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6368 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5582 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/Parallelizer.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21354 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11570 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9958 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5209 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6164 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4126 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20987 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13867 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14722 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10571 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14678 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6707 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5882 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.965570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    23156 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/BlasUtil.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19876 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/ConfigureVectorization.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21931 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/Constants.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     4892 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15555 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6696 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/IndexedViewHelper.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10949 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/IntegralConstant.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     4268 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/MKL_support.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    52909 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/Macros.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    46661 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/Memory.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    29336 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/Meta.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       85 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/NonMPL2.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1024 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1432 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/ReshapedHelper.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10676 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/StaticAssert.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12003 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/SymbolicIndex.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35762 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/XprHelper.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.969570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12559 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17274 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4178 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22970 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17176 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9716 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14349 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5575 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23640 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21078 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3650 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35182 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4104 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22764 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.969570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18939 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/AlignedBox.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8403 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/AngleAxis.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3624 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/EulerAngles.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20726 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Homogeneous.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11962 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Hyperplane.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8955 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9812 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    34367 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Quaternion.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6862 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Rotation2D.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8063 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/RotationBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6724 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Scaling.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    61930 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Transform.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7664 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Translation.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6190 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Umeyama.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.969570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/arch/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5945 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.969570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Householder/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4784 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Householder/BlockHouseholder.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5365 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Householder/Householder.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23611 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Householder/HouseholderSequence.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.973570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6771 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6850 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8887 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15036 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14940 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13379 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7349 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4212 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.973570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Jacobi/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16383 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Jacobi/Jacobi.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.973570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/KLUSupport/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11555 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/KLUSupport/KLUSupport.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.973570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3439 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/Determinant.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    32383 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/FullPivLU.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15727 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/InverseImpl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22069 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/PartialPivLU.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3555 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.973570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/arch/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13693 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/arch/InverseSize4.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.973570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/MetisSupport/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4588 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.973570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16105 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Amd.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    61681 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5248 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.973570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/PaStiXSupport/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22249 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.977570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/PardisoSupport/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20092 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.977570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25498 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4662 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23429 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26768 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14641 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/HouseholderQR.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2993 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.977570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SPQRSupport/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11826 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.977570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    54214 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/BDCSVD.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    32988 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/JacobiSVD.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5099 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14743 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/SVDBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15957 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.977570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24216 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5830 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.985570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10670 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8743 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13166 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2191 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11368 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseAssign.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24360 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6485 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13606 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25524 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4757 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13256 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5808 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3080 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDot.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1107 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12589 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMap.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    57475 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17451 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7329 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7593 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1699 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15600 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseRef.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25889 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4424 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSolverBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8704 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3175 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6437 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6827 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14832 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseVector.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8127 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseView.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9657 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.989570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    33316 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4303 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7602 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4974 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12837 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2049 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6712 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6584 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3681 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10217 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4181 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5723 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8485 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9028 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4979 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4545 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2889 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.989570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseQR/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29167 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseQR/SparseQR.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.989570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/StlSupport/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4730 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdDeque.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4155 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdList.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5338 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdVector.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2809 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/StlSupport/details.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.989570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SuperLUSupport/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    34324 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.989570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/UmfPackSupport/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24456 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.993570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2913 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/Image.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2742 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/Kernel.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1748 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/RealSvd2x2.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30560 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/blas.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7834 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/lapack.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)  1058369 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/lapacke.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      474 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/lapacke_mangling.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.993570 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14060 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21431 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    59020 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/BlockMethods.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4828 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6089 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12283 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/IndexedViewMethods.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6387 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3350 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6915 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/ReshapedMethods.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1145 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/INSTALL
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      288 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/README.md
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.005571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3932 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/BenchSparseUtil.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4486 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/BenchTimer.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2529 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/BenchUtil.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2008 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/README.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28983 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/analyze-blocking-sizes.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1421 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/basicbench.cxxlist
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1107 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/basicbenchmark.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1674 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/basicbenchmark.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6313 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchBlasGemm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3548 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchCholesky.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5788 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchEigenSolver.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2806 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchFFT.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3598 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchGeometry.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5193 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchVecAdd.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11435 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_gemm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1352 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_move_semantics.cpp
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)      618 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_multi_compilers.sh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11622 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_norm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2159 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_reverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      320 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_sum.cpp
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)      651 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_unrolling
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22259 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmark-blocking-sizes.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      790 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmark.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      835 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmarkSlice.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      640 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmarkX.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      605 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmarkXcwise.cpp
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1209 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmark_suite
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.009570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2782 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18109 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/COPYING
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6447 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/README
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.013570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3374 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_aat_product.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3354 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_ata_product.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3670 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_atv_product.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3371 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_axpby.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3340 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_axpy.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3202 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_cholesky.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3460 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_ger.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5598 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_hessenberg.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3151 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_lu_decomp.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3598 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_lu_solve.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3886 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3982 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product_bis.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3989 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_vector_product.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3188 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_partial_lu.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3019 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_rot.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3691 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_symv.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3664 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_syr2.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3425 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_trisolve.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4061 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_trisolve_matrix.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3907 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_trmm.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      464 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/basic_actions.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.013570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      918 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindACML.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1290 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindATLAS.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      781 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindBLAZE.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1058 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindBlitz.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      634 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindCBLAS.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      336 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindGMM.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1232 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindMKL.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      787 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindMTL4.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      604 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindOPENBLAS.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2372 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      798 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindTvmet.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1315 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.017571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      869 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1368 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/action_settings.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2224 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/gnuplot_common_settings.hh
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     2092 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/go_mean
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5306 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/mean.cxx
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1850 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/mk_gnuplot_script.sh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      929 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/mk_mean_script.sh
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1742 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/mk_new_gnuplot.sh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      974 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/perlib_plot_settings.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3425 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/regularize.cxx
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5112 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/smooth.cxx
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1687 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/smooth_all.sh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.017571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4827 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/bench.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1916 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/bench_parameter.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6748 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/btl.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.017571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1478 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_function.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2295 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_matrix.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1416 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_vector.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.017571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2278 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/bench_static.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1948 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2222 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/static_size_generator.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.021571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2305 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2522 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/STL_timer.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1994 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2938 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3534 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     3534 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_timer.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2927 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5294 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/x86_timer.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.021571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1658 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/size_lin_log.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1646 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/size_log.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2745 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/utilities.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2214 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/xy_file.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.909570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.021571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1468 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35158 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2891 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4811 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface_impl.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1634 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/c_interface_base.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2960 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/main.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.021571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/STL/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       37 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/STL/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5802 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/STL/STL_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1828 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/STL/main.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.021571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blaze/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      475 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blaze/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4122 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blaze/blaze_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1636 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blaze/main.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.025570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      378 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5364 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4129 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/blitz_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1962 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/btl_blitz.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1393 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/btl_tiny_blitz.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3100 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/tiny_blitz_interface.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.025570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      768 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1664 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5151 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/eigen2_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1799 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_adv.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1205 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_linear.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1384 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_matmat.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1456 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_vecmat.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.025570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3207 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1664 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8187 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/eigen3_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1799 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_adv.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1285 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_linear.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1378 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_matmat.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1447 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_vecmat.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.025570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/gmm/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      116 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/gmm/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5364 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4174 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/gmm/gmm_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2113 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/gmm/main.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.029570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      153 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/.kdbgrc.main
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      123 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1943 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/main.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5364 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4210 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_interface.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.029570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2130 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      671 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_linear.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      624 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_matmat.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      624 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_vecmat.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3190 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/tensor_interface.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.029570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      131 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1460 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/main.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3017 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/tvmet_interface.hh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.029570 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/ublas/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/ublas/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1785 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/ublas/main.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4341 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/ublas/ublas_interface.hh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3269 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/check_cache_queries.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6416 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/dense_solvers.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7243 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/eig33.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3307 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/geometry.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.033571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6574 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/changesets.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      193 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1382 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm_common.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm_settings.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      114 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm_square_settings.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      193 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1381 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv_common.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       79 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv_settings.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       88 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv_square_settings.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      205 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemvt.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2466 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/lazy_gemm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      132 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/lazy_gemm_settings.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      298 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/llt.cpp
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     2693 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/make_plot.sh
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.041571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3813 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/chart_footer.html
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14775 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/chart_header.html
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       25 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/footer.html
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      884 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/header.html
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   151723 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/s1.js
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   241320 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/s2.js
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     4090 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/run.sh
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     2031 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/runall.sh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      217 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/trmv_lo.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/trmv_lot.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      217 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/trmv_up.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/trmv_upt.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3232 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/product_threshold.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6006 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/quat_slerp.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1097 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/quatmul.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6260 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_cholesky.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5101 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_dense_product.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3011 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_lu.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8999 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_product.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3393 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_randomsetter.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13761 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_setter.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2347 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_transpose.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6114 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_trisolver.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.041571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3061 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3975 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/sp_solver.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1856 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/spbench.dtd
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3301 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/spbenchsolver.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18167 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/spbenchsolver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3825 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/spbenchstyle.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2831 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/test_sparseLU.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6096 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/spmv.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.045571 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1496 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/README
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1585 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/benchmark.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6834 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/benchmark_main.cc
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1389 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/contraction_benchmarks_cpu.cc
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)      729 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/eigen_sycl_bench.sh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      647 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/eigen_sycl_bench_contract.sh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20459 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6264 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_cpu.cc
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3381 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_fp16_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3373 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6273 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_sycl.cc
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11331 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_contract_sycl_bench.cc
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1203 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/bench/vdw_new.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.049571 aplr-6.5.0/dependencies/eigen-3.4.0/blas/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3614 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/BandTriangularSolver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1730 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1608 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/GeneralRank1Update.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2036 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/PackedSelfadjointProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3165 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/PackedTriangularMatrixVector.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3191 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/PackedTriangularSolverVector.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      183 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/README.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2168 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/Rank2Update.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4672 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/common.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      647 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/complex_double.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      646 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/complex_single.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1507 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/double.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.053571 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15108 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/chbmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13026 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/chpmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2310 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/complexdots.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18945 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/ctbmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      117 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/d_cnjg.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      657 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/datatypes.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4968 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/drotm.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6193 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/drotmg.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10188 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/dsbmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8075 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/dspmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11657 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/dtbmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2976 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/lsame.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      105 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/r_cnjg.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4902 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/srotm.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6056 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/srotmg.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10210 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/ssbmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8051 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/sspmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11643 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/stbmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15144 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/zhbmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13060 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/zhpmv.c
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18973 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/ztbmv.c
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.053571 aplr-6.5.0/dependencies/eigen-3.4.0/blas/fortran/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      979 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/fortran/complexdots.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5646 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/level1_cplx_impl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3892 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/level1_impl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4267 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/level1_real_impl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12223 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/level2_cplx_impl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25172 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/level2_impl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10499 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/level2_real_impl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    38043 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/level3_impl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      763 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/single.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.065571 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      948 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    32110 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat1.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1546 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat2.dat
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   116657 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat2.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1046 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat3.dat
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   131550 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat3.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    44820 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat1.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1466 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat2.dat
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   112335 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat2.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      882 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat3.dat
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   104262 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat3.f
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1016 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/runblastest.sh
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    43389 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat1.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1466 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat2.dat
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   112251 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat2.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      882 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat3.dat
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   104172 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat3.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    32115 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat1.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1546 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat2.dat
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   117003 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat2.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1046 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat3.dat
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   131995 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat3.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      389 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/blas/xerbla.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.069571 aplr-6.5.0/dependencies/eigen-3.4.0/ci/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6736 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/ci/CTest2JUnit.xsl
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4910 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/ci/README.md
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5024 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/ci/build.gitlab-ci.yml
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3490 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/ci/smoketests.gitlab-ci.yml
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10349 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/ci/test.gitlab-ci.yml
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.077571 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2171 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/ComputeCppCompilerChecks.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      475 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/ComputeCppIRMap.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      802 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/Eigen3Config.cmake.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1397 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/Eigen3ConfigLegacy.cmake.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2779 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenConfigureTesting.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1562 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenDetermineOSVersion.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1814 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenDetermineVSServicePack.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2321 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenSmokeTestList.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29205 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenTesting.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1196 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenUninstall.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      517 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindAdolc.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    42828 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindBLAS.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13179 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindBLASEXT.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2413 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindCHOLMOD.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16685 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindComputeCpp.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2636 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindEigen2.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3509 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindEigen3.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2783 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindFFTW.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2943 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindGLEW.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      524 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindGMP.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4992 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindGSL.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      846 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindGoogleHash.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11729 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindHWLOC.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1281 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindKLU.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9734 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindLAPACK.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2632 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindMPFR.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3524 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindMPREAL.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8969 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindMetis.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23160 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindPASTIX.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14417 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindPTSCOTCH.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12034 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindSCOTCH.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1142 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindSPQR.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2482 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindStandardMathLibrary.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2261 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindSuperLU.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5111 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindTriSYCL.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1662 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindUMFPACK.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      910 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/RegexUtils.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      177 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/cmake/UseEigen3.cmake
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.909570 aplr-6.5.0/dependencies/eigen-3.4.0/debug/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.077571 aplr-6.5.0/dependencies/eigen-3.4.0/debug/gdb/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       22 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/debug/gdb/__init__.py
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9617 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/debug/gdb/printers.py
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.077571 aplr-6.5.0/dependencies/eigen-3.4.0/debug/msvc/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11661 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/debug/msvc/eigen.natvis
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7566 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/debug/msvc/eigen_autoexp_part.dat
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.077571 aplr-6.5.0/dependencies/eigen-3.4.0/demos/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      278 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/CMakeLists.txt
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.077571 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mandelbrot/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      462 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mandelbrot/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      336 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mandelbrot/README
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7509 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mandelbrot/mandelbrot.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1888 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mandelbrot/mandelbrot.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.077571 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      262 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/README
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4158 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3346 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1616 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/example.c
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.081571 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      695 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      403 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/README
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5981 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/camera.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3435 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/camera.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3974 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/gpuhelper.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7177 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/gpuhelper.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3927 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/icosphere.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      869 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/icosphere.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19192 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/quaternion_demo.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2635 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/quaternion_demo.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1756 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/trackball.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      943 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/trackball.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.101571 aplr-6.5.0/dependencies/eigen-3.4.0/doc/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11165 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/AsciiQuickReference.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2425 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/B01_Experimental.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4935 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6332 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/ClassHierarchy.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18692 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/CoeffwiseMathFunctionsTable.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4423 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/CustomizingEigen_CustomScalar.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1337 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/CustomizingEigen_InheritingMatrix.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3658 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/CustomizingEigen_NullaryExpr.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3658 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/CustomizingEigen_Plugins.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5021 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/DenseDecompositionBenchmark.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    86035 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/Doxyfile.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8355 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/Eigen_Silly_Professor_64x64.png
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1906 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/FixedSizeVectorizable.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13458 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/FunctionsTakingEigenTypes.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5429 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/HiPerformance.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3797 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/InplaceDecomposition.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30585 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/InsideEigenExample.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3150 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/LeastSquares.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6761 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/Manual.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      758 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/MatrixfreeSolverExample.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5610 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/NewExpressionType.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1929 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/Overview.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1166 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/PassingByValue.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7018 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/Pitfalls.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14277 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/PreprocessorDirectives.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29844 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/QuickReference.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6578 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/QuickStartGuide.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19902 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/SparseLinearSystems.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8312 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/SparseQuickReference.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3923 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/StlContainers.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4119 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/StorageOrders.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7026 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/StructHavingEigenMembers.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6157 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TemplateKeyword.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10269 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicAliasing.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5285 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicAssertions.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1914 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicCMakeGuide.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      173 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicEigenExpressionTemplates.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6314 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicLazyEvaluation.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9068 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicLinearAlgebraDecompositions.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3749 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicMultithreading.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      137 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicResizing.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      145 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicScalarTypes.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       97 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicVectorization.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6900 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialAdvancedInitialization.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8523 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialArrayClass.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8288 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialBlockOperations.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9731 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialGeometry.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11860 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialLinearAlgebra.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3988 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialMapClass.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9865 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialMatrixArithmetic.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13680 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialMatrixClass.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12006 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialReductionsVisitorsBroadcasting.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2981 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialReshape.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2142 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialSTL.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8209 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialSlicingIndexing.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20483 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialSparse.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       89 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialSparse_example_details.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8737 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/UnalignedArrayAssert.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6633 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/UsingBlasLapackBackends.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6113 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/UsingIntelMKL.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1855 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/UsingNVCC.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2924 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/WrongStackAlignment.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8006 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigen_navtree_hacks.js
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4584 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy.css
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      680 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy_footer.html.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2521 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy_header.html.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5337 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy_layout.xml.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1095 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy_tabs.css
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.113571 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       34 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/.krazy
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      607 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      766 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/CustomizingEigen_Inheritance.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      189 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Cwise_erf.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      190 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Cwise_erfc.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      192 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Cwise_lgamma.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      282 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/DenseBase_middleCols_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      282 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/DenseBase_middleRows_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      283 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/DenseBase_template_int_middleCols.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      283 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/DenseBase_template_int_middleRows.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      206 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/QuickStart_example.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      305 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/QuickStart_example2_dynamic.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      289 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/QuickStart_example2_fixed.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      677 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TemplateKeyword_flexible.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      508 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TemplateKeyword_simple.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1589 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialInplaceLU.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      622 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgComputeTwice.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      371 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgExComputeSolveError.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      381 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      356 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgExSolveLDLT.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      348 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgInverseDeterminant.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      600 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgRankRevealing.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      405 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgSVDSolve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      534 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      377 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgSetThreshold.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      466 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_accessors.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      400 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_addition.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      410 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      444 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      591 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      237 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_mult.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      523 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      390 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_colrow.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      448 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_corner.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      413 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_print_block.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      348 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_vector.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      401 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_PartialLU_solve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      440 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      356 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      361 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      247 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      502 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      513 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      675 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      447 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      244 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      531 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      680 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_simple_example_dynamic_size.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      282 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_simple_example_fixed_size.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      737 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_Block.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      526 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_CwiseBinaryOp.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      561 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_CwiseUnaryOp.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      371 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      697 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_FixedBlock.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      467 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_FixedReshaped.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      673 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_FixedVectorBlock.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      545 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_Reshaped.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      775 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_VectorBlock.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      418 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/function_taking_eigenbase.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      594 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/function_taking_ref.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      366 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      145 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.entry
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      948 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.evaluator
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      591 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.expression
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      146 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.main
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       85 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.preamble
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      605 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.traits
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1320 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4275 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/matrixfree_cg.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2455 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/nullary_indexing.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      471 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_add_sub.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      393 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_dot_cross.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      612 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_matrix_mul.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      529 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_redux_basic.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      353 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_scalar_mul_div.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      343 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_matrix_coefficient_accessors.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      489 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_matrix_resize.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_matrix_resize_fixed_size.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       86 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/ftv2node.png
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/ftv2pnode.png
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.177571 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       34 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/.krazy
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      210 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/AngleAxis_mimic_euler.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Array_initializer_list_23_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       63 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Array_initializer_list_vector_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      102 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Array_variadic_ctor_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      394 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/BiCGSTAB_simple.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      407 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/BiCGSTAB_step_by_step.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1624 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      324 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/ColPivHouseholderQR_solve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      792 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/ComplexEigenSolver_compute.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      216 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      194 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      301 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/ComplexSchur_compute.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      263 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/ComplexSchur_matrixT.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      221 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/ComplexSchur_matrixU.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_abs.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       46 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_abs2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_acos.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       85 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_arg.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      232 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_array_power_array.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_asin.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       65 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_atan.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_boolean_and.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      105 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_boolean_not.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_boolean_or.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       63 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_boolean_xor.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       92 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_ceil.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       58 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_cos.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_cosh.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       44 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_cube.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_equal_equal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       43 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_exp.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       93 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_floor.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       51 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_greater.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_greater_equal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       47 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_inverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      104 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_isFinite.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      101 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_isInf.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      101 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_isNaN.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       51 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_less.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_less_equal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       43 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_log.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       47 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_log10.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       54 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_max.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       54 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_min.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       39 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_minus.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_minus_equal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_not_equal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       39 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_plus.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_plus_equal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       53 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_pow.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      141 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_product.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       49 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_quotient.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       92 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_rint.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       93 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_round.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       85 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_scalar_power_array.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_sign.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       58 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_sin.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_sinh.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_slash_equal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       44 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_sqrt.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       46 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_square.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       58 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_tan.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_tanh.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Cwise_times_equal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      117 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/DenseBase_LinSpaced.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      420 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/DenseBase_LinSpacedInt.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      139 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/DenseBase_LinSpaced_seq_deprecated.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/DenseBase_setLinSpaced.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      368 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/DirectionWise_hnormalized.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      186 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/DirectionWise_replicate.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      179 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/DirectionWise_replicate_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      800 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      361 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_compute.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      176 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_eigenvalues.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      181 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_eigenvectors.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      430 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      325 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/FullPivHouseholderQR_solve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      369 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/FullPivLU_image.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      317 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/FullPivLU_kernel.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      413 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/FullPivLU_solve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      456 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/GeneralizedEigenSolver.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      339 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/HessenbergDecomposition_compute.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      391 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/HessenbergDecomposition_matrixH.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      482 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      300 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/HouseholderQR_householderQ.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      357 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/HouseholderQR_solve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1316 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      603 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/IOFormat.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      614 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/JacobiSVD_basic.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      236 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Jacobi_makeGivens.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      293 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Jacobi_makeJacobi.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      519 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/LLT_example.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      456 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/LLT_solve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      192 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/LeastSquaresNormalEquations.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      177 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/LeastSquaresQR.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      164 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Map_general_stride.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      199 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Map_inner_stride.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      138 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Map_outer_stride.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      183 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Map_placement_new.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       93 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Map_simple.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_adjoint.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      523 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_all.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      207 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_applyOnTheLeft.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      292 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_applyOnTheRight.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       70 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_array.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      234 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_array_const.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       56 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_asDiagonal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      244 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_block_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      250 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_block_int_int_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      271 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      274 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      242 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_bottomRows_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      119 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cast.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       82 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_col.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      287 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_colwise.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      471 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_colwise_iterator_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      410 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      318 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       80 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseAbs.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       81 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseAbs2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       95 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseArg.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      276 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseEqual.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       87 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseInverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseMax.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseMin.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      286 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseNotEqual.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      153 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseProduct.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       65 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseQuotient.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       80 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseSign.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       50 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseSqrt.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      188 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_diagonal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      270 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_diagonal_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      274 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_diagonal_template_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      160 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_eigenvalues.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      226 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_end_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      467 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_eval.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      274 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      377 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_hnormalized.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      487 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_homogeneous.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       50 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_identity.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       42 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_identity_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      145 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_inverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      241 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isDiagonal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      235 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isIdentity.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      216 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isOnes.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      293 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isOrthogonal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      231 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isUnitary.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      215 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isZero.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      236 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_leftCols_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      129 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_noalias.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       75 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_ones.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       77 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_ones_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       37 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_ones_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      132 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_operatorNorm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      171 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_prod.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       42 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_random.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       37 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_random_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       39 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_random_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      170 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_replicate.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      163 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_replicate_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      291 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_auto.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      178 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_fixed.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      160 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      287 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_to_vector.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      407 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      239 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_rightCols_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       82 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_row.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      281 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_rowwise.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      244 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_segment_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      115 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_select.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      361 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_selfadjointView.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      290 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_set.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       83 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_setIdentity.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       72 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_setOnes.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       72 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_setRandom.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       72 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_setZero.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      226 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_start_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      248 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_bottomRows.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      230 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_end.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      264 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      274 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      301 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      277 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      304 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      265 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      292 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      268 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      295 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      242 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_leftCols.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      245 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_rightCols.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      244 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_segment.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      230 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_start.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      239 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_topRows.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      262 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      265 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      233 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_topRows_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      414 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_transpose.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      573 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_triangularView.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       71 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_zero.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       73 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_zero_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       37 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_zero_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      157 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_Map_stride.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_initializer_list_23_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       40 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_initializer_list_vector_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      111 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_resize_NoChange_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      235 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_resize_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      111 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_resize_int_NoChange.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      407 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_resize_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_setConstant_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_setConstant_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_setIdentity_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_setOnes_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       48 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_setOnes_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       47 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_setRandom_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       50 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_setRandom_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_setZero_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       48 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_setZero_int_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      104 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Matrix_variadic_ctor_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      372 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/PartialPivLU_solve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      263 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_count.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      176 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_maxCoeff.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      176 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_minCoeff.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_norm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_prod.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_squaredNorm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      164 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_sum.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      819 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/RealQZ_compute.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      429 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      343 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/RealSchur_compute.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      362 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      816 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      826 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      365 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      396 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      193 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      426 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      363 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      184 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointView_eigenvalues.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      157 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointView_operatorNorm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      167 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Slicing_arrayexpr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      369 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Slicing_custom_padding_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      190 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Slicing_rawarray_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      164 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Slicing_stdvector_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      411 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SparseMatrix_coeffs.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      267 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_block.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      270 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_block_correct.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      591 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_cwise.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       76 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      230 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       86 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult3.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      102 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult4.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      109 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult5.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      525 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicStorageOrders_example.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      520 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Triangular_solve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      445 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      392 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_compute.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      550 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      552 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_diagonal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      303 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_householderCoefficients.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      394 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_packedMatrix.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      132 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      168 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      266 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      272 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      878 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      332 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      299 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_Map_rowmajor.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      896 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_Map_using.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      171 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      299 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      611 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_SlicingCol.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_SlicingVec.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       70 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_commainit_01.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      113 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_commainit_01b.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      215 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_commainit_02.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      117 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_range_for_loop_1d_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      148 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_range_for_loop_2d_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      249 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_reshaped_vs_resize_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      372 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_reshaped_vs_resize_2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      146 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_matrix_inverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      318 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_multiple_rhs.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      368 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      256 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_singular.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      273 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_triangular.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      159 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_triangular_inplace.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      203 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_std_sort.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      218 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_std_sort_rows_cxx11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      461 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/VectorwiseOp_homogeneous.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      536 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Vectorwise_reverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      732 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/class_FullPivLU.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      555 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/compile_snippet.cpp.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      468 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/tut_arithmetic_redux_minmax.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      188 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      277 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      174 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_inplace.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      193 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/tut_matrix_assignment_resizing.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.177571 aplr-6.5.0/dependencies/eigen-3.4.0/doc/special_examples/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1114 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/special_examples/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1184 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1576 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example_details.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      336 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/special_examples/random_cpp11.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2544 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/doc/tutorial.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      254 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/eigen3.pc.in
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.185571 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2423 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      245 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/bdcsvd_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      233 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      233 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      261 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      262 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/block_on_const_type_actually_const_0.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      262 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/block_on_const_type_actually_const_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      257 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/colpivqr_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      245 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/const_qualified_block_method_retval_0.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      240 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/const_qualified_block_method_retval_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      239 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/const_qualified_diagonal_method_retval.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      241 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/const_qualified_transpose_method_retval.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      271 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      296 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/cwiseunaryview_on_const_type_actually_const.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      228 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      250 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/diagonal_on_const_type_actually_const.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      276 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/eigensolver_cplx.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      259 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/eigensolver_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      156 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/failtest_sanity_check.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      247 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/fullpivlu_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      258 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/fullpivqr_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      183 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/initializer_list_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      222 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/initializer_list_2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      248 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/jacobisvd_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      250 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/ldlt_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      248 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/llt_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      224 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      246 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      270 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      314 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      321 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      249 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/map_on_const_type_actually_const_0.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      241 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/map_on_const_type_actually_const_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      250 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/partialpivlu_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      251 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/qr_int.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      263 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/ref_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      213 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/ref_2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      231 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/ref_3.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      227 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/ref_4.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      238 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/ref_5.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      241 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      266 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/selfadjointview_on_const_type_actually_const.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      302 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/sparse_ref_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      238 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/sparse_ref_2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      271 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/sparse_ref_3.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      235 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/sparse_ref_4.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      285 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/sparse_ref_5.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      290 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/sparse_storage_mismatch.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      217 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/swap_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      211 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/swap_2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      213 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/ternary_1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      225 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/ternary_2.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      254 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/transpose_on_const_type_actually_const.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      238 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      265 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/failtest/triangularview_on_const_type_actually_const.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.193571 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10876 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2205 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/cholesky.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2831 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clacgv.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2340 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/cladiv.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6295 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clarf.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23424 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clarfb.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5344 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clarfg.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10450 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clarft.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      578 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/complex_double.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      577 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/complex_single.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2969 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dladiv.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5259 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlamch.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2514 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlapy2.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2737 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlapy3.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6167 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlarf.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22749 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlarfb.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4946 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlarfg.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10222 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlarft.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      562 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/double.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1282 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dsecnd_NONE.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1826 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/eigenvalues.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2957 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilaclc.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2997 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilaclr.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2952 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/iladlc.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3000 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/iladlr.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2941 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilaslc.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2988 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilaslr.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2962 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilazlc.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3010 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilazlr.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      877 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/lapack_common.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2655 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/lu.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1258 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/second_NONE.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      561 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/single.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2897 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/sladiv.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5261 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slamch.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2490 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slapy2.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2701 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slapy3.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6117 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slarf.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22727 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slarfb.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4908 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slarfg.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10183 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slarft.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4891 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/svd.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2839 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlacgv.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2364 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zladiv.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6278 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlarf.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23498 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlarfb.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5359 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlarfg.f
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10453 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlarft.f
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.197571 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      328 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/CMakeLists.txt
--rwxr-xr-x   0 mathiaso  (1000) mathiaso  (1001)      577 2021-08-18 18:41:58.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/buildtests.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1569 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/cdashtesting.cmake.in
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)      670 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/check.in
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)       44 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/debug.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6384 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/eigen_gen_credits.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      738 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/eigen_gen_docs
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      323 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/eigen_gen_split_test_help.cmake
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1009 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/eigen_monitor_perf.sh
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)       46 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/release.in
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2368 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/scripts/relicense.py
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      216 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/signature_of_eigen3_matrix_library
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.233572 aplr-6.5.0/dependencies/eigen-3.4.0/test/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5707 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/AnnoyingScalar.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14452 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1079 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/MovableScalar.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      605 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/SafeScalar.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8668 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/adjoint.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    27758 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/array_cwise.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12883 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/array_for_matrix.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      961 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/array_of_string.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2342 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/array_replicate.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6383 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/array_reverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2432 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/bandmatrix.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13366 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/basicstuff.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4443 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/bdcsvd.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17931 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/bfloat16_float.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1473 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/bicgstab.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6413 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/blasutil.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14816 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/block.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5731 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/boostmultiprec.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      174 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/bug1213.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      147 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/bug1213.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      279 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/bug1213_main.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18340 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/cholesky.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3377 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/cholmod_support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3150 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/commainitializer.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1543 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/conjugate_gradient.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5369 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/conservative_resize.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2562 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/constructor.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6448 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/corners.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2016 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/ctorleak.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5062 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/denseLM.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7256 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/dense_storage.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2275 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/determinant.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4115 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/diagonal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6686 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/diagonal_matrix_variadic_ctor.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7531 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/diagonalmatrices.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2229 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/dontalign.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4760 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/dynalloc.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2196 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/eigen2support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6221 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/eigensolver_complex.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4046 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/eigensolver_generalized_real.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9459 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/eigensolver_generic.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11419 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/eigensolver_selfadjoint.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/evaluator_common.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21038 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/evaluators.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1916 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/exceptions.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5256 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/fastmath.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1874 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/first_aligned.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18093 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_alignedbox.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3562 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_eulerangles.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5470 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_homogeneous.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7304 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_hyperplane.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4838 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_orthomethods.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4974 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_parametrizedline.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11568 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_quaternion.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26366 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_transformations.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16082 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/gpu_basic.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5456 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/gpu_common.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14524 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/half_float.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2404 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/hessenberg.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6286 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/householder.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2623 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/incomplete_cholesky.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19424 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/indexed_view.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12744 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/initializer_list_construction.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3880 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/inplace_decomposition.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5793 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/integer_types.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4701 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/inverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1833 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/io.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1368 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/is_same_dense.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2733 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/jacobi.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5877 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/jacobisvd.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      955 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/klu_support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6130 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/linearstructure.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1499 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/lscg.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9075 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/lu.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    33109 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/main.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7943 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/mapped_matrix.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7471 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/mapstaticmethods.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11369 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/mapstride.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7339 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/meta.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      751 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/metis_support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1789 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/miscmatrices.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17824 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/mixingtypes.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      635 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/mpl2only.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1208 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/nestbyvalue.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4377 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/nesting_ops.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8700 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/nomalloc.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12806 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/nullary.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3212 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/num_dimensions.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9042 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/numext.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    55436 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/packetmath.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9016 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/packetmath_test_shared.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      955 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/pardiso_support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1902 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/pastix_support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7031 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/permutationmatrices.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3120 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/prec_inverse_4x4.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11880 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15711 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_extra.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5395 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_large.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4447 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_mmtr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10988 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_notemporary.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3510 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_selfadjoint.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12656 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_small.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6133 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_symm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7856 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_syrk.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6921 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_trmm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4250 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_trmv.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6102 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/product_trsolve.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4673 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/qr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13867 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/qr_colpivoting.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5600 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/qr_fullpivoting.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4621 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/qtvector.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4373 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/rand.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7174 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/random_without_cast_overflow.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3102 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/real_qz.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8239 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/redux.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14363 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/ref.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10706 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/reshape.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1105 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/resize.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5668 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/rvalue_types.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3569 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/schur_complex.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3964 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/schur_real.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2419 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/selfadjoint.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2564 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/simplicial_cholesky.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2038 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sizeof.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2639 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sizeoverflow.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2133 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/smallvectors.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1716 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/solverbase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6216 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4740 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparseLM.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29343 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_basic.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12153 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_block.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9997 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_permutations.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25557 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_product.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6125 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_ref.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24396 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_solver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5142 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_solvers.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5087 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_vector.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1791 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparselu.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4587 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/sparseqr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1762 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/special_numbers.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   159516 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/split_test_helper.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1841 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/spqr_support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10379 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/stable_norm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4260 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/stddeque.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4738 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/stddeque_overload.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4232 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/stdlist.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5852 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/stdlist_overload.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5116 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/stdvector.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5014 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/stdvector_overload.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19411 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/stl_iterators.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      956 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/superlu_support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19317 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/svd_common.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4050 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/svd_fill.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2940 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/swap.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2742 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/symbolic_index.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11918 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/triangular.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2024 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/type_alias.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5859 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/umeyama.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1171 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/umfpack_support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2565 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/unalignedcount.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1716 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/upperbidiagonalization.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20351 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/vectorization_logic.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11489 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/vectorwiseop.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6384 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/visitor.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3734 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/test/zerosized.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.233572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      293 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/CMakeLists.txt
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.237572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4422 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/AdolcForward
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6349 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/AlignedVector3
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      884 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/ArpackSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1181 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/AutoDiff
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5523 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/BVH
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      603 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CMakeLists.txt
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.241572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      307 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4187 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/Tensor
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1267 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/TensorSymmetry
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2087 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/ThreadPool
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.913570 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.265572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    62365 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/README.md
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21269 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12448 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10323 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    57932 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    60851 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    42150 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19707 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15665 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    45320 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2675 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      225 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    63402 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23586 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    89042 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    70687 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18803 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    48686 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    27527 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8642 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13146 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4896 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      215 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3427 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12837 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40367 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15203 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7674 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17751 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8556 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40005 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26655 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16115 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24345 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14486 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8782 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8320 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15269 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10920 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1316 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4068 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1267 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2560 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28066 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25692 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9094 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2730 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9041 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7769 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3642 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14191 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8104 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    43284 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28764 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11474 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12385 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    44395 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      221 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40719 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30074 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14793 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16938 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20091 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25279 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18256 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5481 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13513 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10152 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9432 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7552 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30089 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.265572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10857 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9086 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13021 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.265572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21046 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.269572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2113 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9121 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17075 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9366 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      774 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1209 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11482 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1680 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      715 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.269572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22752 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4115 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8155 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/EmulateArray.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4174 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1126 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/EulerAngles
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13948 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/FFT
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1561 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/IterativeSolvers
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      944 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/KroneckerProduct
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1238 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/LevenbergMarquardt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7656 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/MPRealSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17919 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/MatrixFunctions
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      592 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/MoreVectorization
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5963 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/NonLinearOptimization
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1779 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/NumericalDiff
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19072 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/OpenGLSupport
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4749 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/Polynomials
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      930 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/Skyline
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1360 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/SparseExtra
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2951 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/SpecialFunctions
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      996 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/Splines
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.913570 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.269572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3150 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    29107 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9029 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.269572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12976 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/BVAlgorithms.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9166 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/KdBVH.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.269572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29075 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.273572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      174 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15367 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerAngles.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11620 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerSystem.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.273572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9223 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_fftw_impl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13231 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.273572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5324 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17769 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10209 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/GMRES.h
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    14794 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IDRS.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2520 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5360 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IterationController.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12397 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/MINRES.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5853 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/Scaling.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.273572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10250 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.277572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2194 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2443 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6648 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5039 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6805 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13297 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.277572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16624 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22671 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17557 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23422 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14212 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2107 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.277572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3035 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.281572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19837 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22135 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1864 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/chkder.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1915 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/covar.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3297 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2225 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9111 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3264 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1081 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3083 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1362 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.281572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4020 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.281572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8076 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/Companion.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15683 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4806 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.281572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11365 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    31105 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7837 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10853 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineProduct.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7966 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineStorage.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3153 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineUtil.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.281572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4260 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40316 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13744 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8416 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MarketIO.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7568 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12423 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/RandomSetter.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.289572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10015 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2724 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12641 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2544 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    69632 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4006 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2489 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7694 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3087 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11700 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2899 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    58539 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3713 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.913570 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.289572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1492 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      398 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.289572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1549 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      415 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.289572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10864 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.289572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2258 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1283 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.289572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18307 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/Spline.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16505 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFitting.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4312 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFwd.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1876 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/README.txt
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.289572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/bench/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3906 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/bench/bench_svd.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.289572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      114 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      878 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/Overview.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      345 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/SYCL.dox
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5283 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/eigendoxy_layout.xml.in
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.293572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2108 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/BVH_Example.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      736 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1847 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/EulerAngles.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2522 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/FFT.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      356 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixExponential.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      469 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixFunction.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      375 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixLogarithm.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      364 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixPower.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      424 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixPower_optimal.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      508 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixSine.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      524 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixSinh.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      434 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixSquareRoot.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2392 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/PolynomialSolver1.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      635 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/PolynomialUtils1.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.293572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1409 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2551 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/CwiseMul.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.293572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/snippets/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1137 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/snippets/CMakeLists.txt
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.325572 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7190 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/BVH.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15348 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/CMakeLists.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9623 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/EulerAngles.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       47 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/FFT.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9233 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/FFTW.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    64597 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/NonLinearOptimization.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2862 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/NumericalDiff.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2366 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/alignedvector3.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10992 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/autodiff.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2943 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/autodiff_scalar.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16409 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/bessel_functions.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3990 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_eventcount.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1839 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_maxsizevector.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18740 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_meta.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5039 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_non_blocking_thread_pool.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7024 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_runqueue.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9150 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8886 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9949 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9707 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_assign.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22378 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_access.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    31888 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_eval.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15858 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_io.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5708 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9209 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcasting.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15767 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_builtins_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2420 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_cast_float16_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5526 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_casts.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13050 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26158 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1991 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_comparisons.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2871 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6636 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4624 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8411 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1660 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_const.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7350 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    47521 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23176 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contraction.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5381 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20033 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2518 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_index.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3211 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6806 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13495 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_device.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3210 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_device_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2578 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_dimension.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      999 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_empty.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30675 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_executor.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14224 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_expr.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13705 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_fft.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7252 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_fixed_size.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2167 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3461 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2266 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_generator.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5732 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_generator_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    58446 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5942 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_ifft.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3890 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_op_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    36037 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    62111 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18652 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_index_list.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2109 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5101 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4129 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_intdiv.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3277 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_io.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1639 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4730 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      950 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_lvalue.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7962 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_map.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      993 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_math.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3877 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_math_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1501 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_mixed_indices.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18215 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17549 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1734 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_move.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1789 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_notification.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2893 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_complex.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2430 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_const_values.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21223 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_float16_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3766 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_strings.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2652 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_padding.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5677 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_padding_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5499 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_patch.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9385 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_patch_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2513 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2355 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3568 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15346 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5410 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    42176 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6722 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_ref.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5285 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9283 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1486 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_roundings.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2978 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2576 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_gpu.cu
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6376 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7692 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4265 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9624 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_simple.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3024 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_striding.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7074 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_striding_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1896 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_sugar.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14828 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    59079 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_symmetry.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4237 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_local.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25491 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_pool.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5129 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_trace.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5757 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_uint128.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4592 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11972 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1279 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/dgmres.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3822 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/forward_adolc.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1245 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/gmres.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      942 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/idrs.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9075 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/kronecker_product.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    55504 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/levenberg_marquardt.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4417 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_exponential.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7447 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_function.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2106 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_functions.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7178 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_power.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1050 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_square_root.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1658 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/minres.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2439 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/mpreal_support.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18637 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/openglsupport.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7486 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/polynomialsolver.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3582 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/polynomialutils.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8414 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/sparse_extra.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22854 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/special_functions.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6372 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/special_packetmath.cpp
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8529 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/splines.cpp
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.325572 aplr-6.5.0/dependencies/pybind11/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1684 2022-05-09 14:53:50.000000 aplr-6.5.0/dependencies/pybind11/LICENSE.txt
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      414 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/__init__.py
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1544 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/__main__.py
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      228 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/_version.py
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1226 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/commands.py
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.913570 aplr-6.5.0/dependencies/pybind11/include/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.329572 aplr-6.5.0/dependencies/pybind11/include/pybind11/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23959 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7069 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    65660 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8458 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      120 2023-07-14 06:11:46.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/common.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2096 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.329572 aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28518 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    52930 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5491 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17869 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26305 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    42613 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1625 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.333572 aplr-6.5.0/dependencies/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    31450 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18140 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      316 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13471 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4731 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5002 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8262 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8862 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    79416 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9103 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2734 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/options.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   126420 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    94641 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.333572 aplr-6.5.0/dependencies/pybind11/include/pybind11/stl/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4185 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15337 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29747 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/include/pybind11/stl_bind.h
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 06:11:46.000000 aplr-6.5.0/dependencies/pybind11/py.typed
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17650 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/setup_helpers.py
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.913570 aplr-6.5.0/dependencies/pybind11/share/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:11.913570 aplr-6.5.0/dependencies/pybind11/share/cmake/
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.333572 aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11190 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/FindPythonLibsNew.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14033 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11Common.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7781 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11Config.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1403 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11ConfigVersion.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8960 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11NewTools.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4184 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11Targets.cmake
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8361 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11Tools.cmake
-drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 20:09:12.333572 aplr-6.5.0/dependencies/pybind11/share/pkgconfig/
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      171 2023-07-14 16:07:35.000000 aplr-6.5.0/dependencies/pybind11/share/pkgconfig/pybind11.pc
--rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       38 2023-07-14 20:09:12.333572 aplr-6.5.0/setup.cfg
--rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1236 2023-07-14 17:14:55.000000 aplr-6.5.0/setup.py
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.819042 aplr-6.5.1/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1113 2022-05-12 19:01:46.000000 aplr-6.5.1/LICENSE
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      152 2023-07-14 16:07:35.000000 aplr-6.5.1/MANIFEST.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      614 2023-07-21 18:19:07.819042 aplr-6.5.1/PKG-INFO
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1175 2023-05-24 16:05:01.000000 aplr-6.5.1/README.md
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.383040 aplr-6.5.1/aplr/
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)       19 2022-05-09 14:53:50.000000 aplr-6.5.1/aplr/__init__.py
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    13640 2023-07-04 15:26:35.000000 aplr-6.5.1/aplr/aplr.py
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.383040 aplr-6.5.1/aplr.egg-info/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      614 2023-07-21 18:19:07.000000 aplr-6.5.1/aplr.egg-info/PKG-INFO
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   112326 2023-07-21 18:19:07.000000 aplr-6.5.1/aplr.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)        1 2023-07-21 18:19:07.000000 aplr-6.5.1/aplr.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       12 2023-07-21 18:19:07.000000 aplr-6.5.1/aplr.egg-info/requires.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       14 2023-07-21 18:19:07.000000 aplr-6.5.1/aplr.egg-info/top_level.txt
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.391040 aplr-6.5.1/cpp/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12294 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/APLRClassifier.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    75771 2023-07-21 18:16:31.000000 aplr-6.5.1/cpp/APLRRegressor.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.371040 aplr-6.5.1/cpp/build/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.371040 aplr-6.5.1/cpp/build/CMakeFiles/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.371040 aplr-6.5.1/cpp/build/CMakeFiles/3.16.3/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.391040 aplr-6.5.1/cpp/build/CMakeFiles/3.16.3/CompilerIdCXX/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20091 2022-05-12 20:45:33.000000 aplr-6.5.1/cpp/build/CMakeFiles/3.16.3/CompilerIdCXX/CMakeCXXCompilerId.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      321 2023-05-24 16:05:01.000000 aplr-6.5.1/cpp/constants.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18214 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/functions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1825 2023-07-21 13:48:26.000000 aplr-6.5.1/cpp/main.cpp
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    19771 2023-07-04 15:26:35.000000 aplr-6.5.1/cpp/pythonbinding.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28325 2023-07-21 13:46:32.000000 aplr-6.5.1/cpp/term.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2033 2023-07-21 10:28:34.000000 aplr-6.5.1/cpp/test ALRRegressor cauchy group_mse validation.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1903 2023-07-21 16:21:44.000000 aplr-6.5.1/cpp/test ALRRegressor cauchy.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3465 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor custom loss and validation.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3084 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor custom loss.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2623 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor gamma custom_link.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2281 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor gamma custom_validation.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1951 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor gamma gini weighted.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1951 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor gamma gini.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1949 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor gamma rank unweighted.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1949 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor gamma rank.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1941 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor gamma.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1987 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor group_mse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1990 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor int constr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1980 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor inversegaussian.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1975 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor logit.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1910 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor mae.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2055 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor monotonic.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2021 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor negative_binomial.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1974 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor poisson.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2011 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor poissongamma.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1893 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor quantile.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2436 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor rank.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1937 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor weibull.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2484 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test ALRRegressor.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4205 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test APLRClassifier multi_class other_params.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4178 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test APLRClassifier multi_class.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2991 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test APLRClassifier two_class other_params.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2931 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test APLRClassifier two_class val_index.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2872 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test APLRClassifier two_class.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5005 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test functions.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4067 2023-07-14 16:07:35.000000 aplr-6.5.1/cpp/test term.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.383040 aplr-6.5.1/dependencies/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.395040 aplr-6.5.1/dependencies/eigen-3.4.0/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      292 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/.gitignore
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.375040 aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.399040 aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab/issue_templates/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2744 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab/issue_templates/Bug Report.md
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      201 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab/issue_templates/Feature Request.md
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.399040 aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab/merge_request_templates/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1394 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab/merge_request_templates/Merge Request Template.md
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      571 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab-ci.yml
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/.hgeol
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24767 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11362 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.APACHE
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1517 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.BSD
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35147 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.GPL
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26530 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.LGPL
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2193 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.MINPACK
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16726 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.MPL2
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      779 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.README
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      584 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/CTestConfig.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/CTestCustom.cmake.in
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.403040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1161 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Cholesky
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1900 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/CholmodSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12799 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Core
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      122 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Dense
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       35 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Eigen
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1777 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Eigenvalues
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1940 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Geometry
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      829 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Householder
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2083 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/IterativeLinearSolvers
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      894 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Jacobi
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1389 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/KLUSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1268 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/LU
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      991 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/MetisSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2451 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/OrderingMethods
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1751 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/PaStiXSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1116 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/PardisoSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1272 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/QR
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      900 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/QtAlignedMalloc
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1162 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SPQRSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1584 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SVD
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      888 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Sparse
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1235 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SparseCholesky
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2240 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SparseCore
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1814 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SparseLU
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1195 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SparseQR
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      797 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/StdDeque
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      726 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/StdList
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      803 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/StdVector
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2243 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SuperLUSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1382 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/UmfPackSupport
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.375040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.403040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Cholesky/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24934 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LDLT.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18760 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LLT.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3974 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.403040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/CholmodSupport/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25441 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.415040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19214 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ArithmeticSequence.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16782 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Array.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8217 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ArrayBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7018 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ArrayWrapper.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2738 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Assign.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    41673 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/AssignEvaluator.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    12488 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Assign_MKL.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14075 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/BandMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18648 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Block.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4429 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/BooleanRedux.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5981 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CommaInitializer.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6990 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ConditionEstimator.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    63841 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CoreEvaluators.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4745 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CoreIterators.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7909 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseBinaryOp.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    36282 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseNullaryOp.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8256 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseTernaryOp.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3937 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseUnaryOp.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5551 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseUnaryView.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    31529 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DenseBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24484 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DenseCoeffsBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25360 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DenseStorage.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9870 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Diagonal.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14670 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DiagonalMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      988 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DiagonalProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11654 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Dot.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5841 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/EigenBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4909 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ForceAlignedAccess.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5759 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Fuzzy.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21679 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/GeneralProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    38812 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/GenericPacketMath.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11543 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/GlobalFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8238 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/IO.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9620 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/IndexedView.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3503 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Inverse.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7256 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Map.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11281 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/MapBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    60784 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/MathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7156 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/MathFunctionsImpl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24343 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Matrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23856 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/MatrixBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2520 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/NestByValue.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3620 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/NoAlias.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12884 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/NumTraits.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9207 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20748 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/PermutationMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    49193 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/PlainObjectBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7336 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Product.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    53832 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ProductEvaluators.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7756 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Random.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19195 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Redux.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17821 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Ref.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5656 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Replicate.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17033 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Reshaped.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4284 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ReturnByValue.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7522 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Reverse.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6143 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Select.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14999 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/SelfAdjointView.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1697 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6837 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Solve.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9368 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/SolveTriangular.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6170 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/SolverBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8700 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/StableNorm.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21641 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/StlIterators.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4212 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Stride.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2765 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Swap.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17606 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Transpose.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13567 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Transpositions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    38277 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/TriangularMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3488 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/VectorBlock.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35168 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/VectorwiseOp.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11997 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Visitor.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.375040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.415040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15223 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/Complex.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8102 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    64608 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2564 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.419040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17160 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13344 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    87891 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2134 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.419040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16540 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2323 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   119355 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9490 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24820 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)   102394 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.419040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/CUDA/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17317 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/CUDA/Complex.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.419040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26903 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5251 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    67696 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3770 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35534 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/Half.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1746 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/Settings.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3746 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.419040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2695 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    57047 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2256 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.375040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/HIP/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.419040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      691 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.419040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17541 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/Complex.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16159 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    33615 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.423040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22503 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/Complex.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6815 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3083 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   189525 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    51286 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.423040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14251 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/Complex.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6765 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    64465 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3650 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.423040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1194 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21200 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1351 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.423040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7428 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12539 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    27786 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21856 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2626 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.423040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16728 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8024 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    36894 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.423040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6686 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20921 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8334 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4998 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/StlFunctors.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      607 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40146 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.427040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   108448 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20104 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15948 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6936 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5106 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21724 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6368 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5582 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/Parallelizer.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21354 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11570 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9958 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5209 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6164 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4126 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20987 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13867 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14722 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10571 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14678 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6707 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5882 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.431040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    23156 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/BlasUtil.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19876 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21931 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/Constants.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     4892 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15555 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6696 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10949 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/IntegralConstant.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     4268 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/MKL_support.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    52909 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/Macros.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    46661 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/Memory.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    29336 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/Meta.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       85 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/NonMPL2.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1024 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1432 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/ReshapedHelper.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10676 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/StaticAssert.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12003 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/SymbolicIndex.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35762 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/XprHelper.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.431040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12559 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17274 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4178 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22970 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17176 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9716 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14349 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5575 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23640 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealQZ.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21078 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3650 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35182 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4104 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22764 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.435040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18939 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/AlignedBox.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8403 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/AngleAxis.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3624 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/EulerAngles.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20726 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Homogeneous.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11962 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Hyperplane.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8955 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/OrthoMethods.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9812 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/ParametrizedLine.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    34367 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Quaternion.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6862 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Rotation2D.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8063 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/RotationBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6724 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Scaling.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    61930 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Transform.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7664 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Translation.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6190 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Umeyama.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.435040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/arch/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5945 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.435040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Householder/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4784 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Householder/BlockHouseholder.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5365 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Householder/Householder.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23611 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Householder/HouseholderSequence.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.439040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6771 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6850 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8887 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15036 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14940 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13379 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7349 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4212 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.439040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Jacobi/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16383 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Jacobi/Jacobi.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.439040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/KLUSupport/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11555 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/KLUSupport/KLUSupport.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.439040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3439 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/Determinant.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    32383 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/FullPivLU.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15727 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/InverseImpl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22069 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/PartialPivLU.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3555 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.439040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/arch/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13693 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/arch/InverseSize4.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.439040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/MetisSupport/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4588 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.439040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16105 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Amd.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    61681 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5248 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.439040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/PaStiXSupport/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22249 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.439040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/PardisoSupport/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20092 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.443040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25498 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4662 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23429 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26768 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14641 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/HouseholderQR.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2993 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.443040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SPQRSupport/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11826 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.443040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    54214 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/BDCSVD.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    32988 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/JacobiSVD.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5099 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14743 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/SVDBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15957 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.443040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24216 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5830 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.451040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10670 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/AmbiVector.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8743 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/CompressedStorage.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13166 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2191 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11368 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseAssign.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24360 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseBlock.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6485 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseColEtree.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13606 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25524 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4757 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13256 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5808 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3080 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDot.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1107 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12589 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMap.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    57475 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17451 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7329 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparsePermutation.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7593 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1699 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseRedux.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15600 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseRef.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25889 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4424 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8704 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3175 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseTranspose.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6437 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6827 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseUtil.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14832 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseVector.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8127 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseView.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9657 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.455040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    33316 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4303 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7602 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4974 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12837 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2049 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6712 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6584 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3681 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10217 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4181 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5723 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8485 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9028 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4979 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4545 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2889 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.455040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseQR/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29167 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseQR/SparseQR.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.455040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/StlSupport/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4730 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdDeque.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4155 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdList.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5338 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdVector.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2809 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/StlSupport/details.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.455040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SuperLUSupport/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    34324 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.455040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/UmfPackSupport/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24456 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.459040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2913 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/Image.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2742 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/Kernel.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1748 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/RealSvd2x2.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30560 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/blas.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7834 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/lapack.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)  1058369 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/lapacke.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      474 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/lapacke_mangling.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.459040 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14060 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21431 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    59020 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/BlockMethods.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4828 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6089 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12283 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/IndexedViewMethods.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6387 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3350 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6915 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/ReshapedMethods.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1145 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/INSTALL
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      288 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/README.md
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.467040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3932 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/BenchSparseUtil.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4486 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/BenchTimer.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2529 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/BenchUtil.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2008 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/README.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28983 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/analyze-blocking-sizes.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1421 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/basicbench.cxxlist
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1107 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/basicbenchmark.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1674 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/basicbenchmark.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6313 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchBlasGemm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3548 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchCholesky.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5788 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchEigenSolver.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2806 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchFFT.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3598 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchGeometry.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5193 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchVecAdd.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11435 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_gemm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1352 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_move_semantics.cpp
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)      618 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_multi_compilers.sh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11622 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_norm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2159 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_reverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      320 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_sum.cpp
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)      651 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_unrolling
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22259 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmark-blocking-sizes.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      790 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmark.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      835 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmarkSlice.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      640 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmarkX.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      605 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmarkXcwise.cpp
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1209 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmark_suite
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.467040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2782 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18109 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/COPYING
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6447 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/README
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.471040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3374 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_aat_product.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3354 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_ata_product.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3670 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_atv_product.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3371 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_axpby.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3340 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_axpy.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3202 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_cholesky.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3460 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_ger.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5598 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_hessenberg.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3151 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_lu_decomp.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3598 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_lu_solve.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3886 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3982 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product_bis.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3989 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_vector_product.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3188 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_partial_lu.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3019 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_rot.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3691 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_symv.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3664 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_syr2.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3425 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_trisolve.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4061 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_trisolve_matrix.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3907 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_trmm.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      464 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/basic_actions.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.475040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      918 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindACML.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1290 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindATLAS.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      781 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindBLAZE.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1058 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindBlitz.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      634 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindCBLAS.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      336 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindGMM.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1232 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindMKL.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      787 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindMTL4.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      604 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindOPENBLAS.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2372 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      798 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindTvmet.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1315 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.479040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      869 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1368 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/action_settings.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2224 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/gnuplot_common_settings.hh
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     2092 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/go_mean
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5306 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/mean.cxx
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1850 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/mk_gnuplot_script.sh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      929 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/mk_mean_script.sh
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1742 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/mk_new_gnuplot.sh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      974 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/perlib_plot_settings.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3425 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/regularize.cxx
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5112 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/smooth.cxx
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1687 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/smooth_all.sh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.479040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4827 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/bench.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1916 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/bench_parameter.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6748 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/btl.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.479040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1478 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_function.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2295 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_matrix.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1416 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_vector.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.479040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2278 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/bench_static.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1948 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2222 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/static_size_generator.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.479040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2305 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2522 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/STL_timer.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1994 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2938 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3534 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     3534 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_timer.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2927 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5294 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/x86_timer.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.483040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1658 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/size_lin_log.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1646 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/size_log.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2745 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/utilities.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2214 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/xy_file.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.379040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.483040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1468 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    35158 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2891 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4811 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface_impl.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1634 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/c_interface_base.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2960 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/main.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.483040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/STL/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       37 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/STL/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5802 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/STL/STL_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1828 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/STL/main.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.483040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blaze/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      475 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blaze/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4122 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blaze/blaze_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1636 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blaze/main.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.487040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      378 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5364 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4129 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/blitz_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1962 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/btl_blitz.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1393 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/btl_tiny_blitz.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3100 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/tiny_blitz_interface.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.487040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      768 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1664 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5151 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/eigen2_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1799 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_adv.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1205 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_linear.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1384 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_matmat.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1456 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_vecmat.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.487040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3207 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1664 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8187 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/eigen3_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1799 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_adv.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1285 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_linear.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1378 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_matmat.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1447 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_vecmat.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.487040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/gmm/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      116 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/gmm/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5364 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4174 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/gmm/gmm_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2113 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/gmm/main.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.491040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      153 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/.kdbgrc.main
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      123 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1943 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/main.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5364 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4210 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_interface.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.491040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2130 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      671 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_linear.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      624 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_matmat.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      624 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_vecmat.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3190 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/tensor_interface.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.491040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      131 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1460 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/main.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3017 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/tvmet_interface.hh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.491040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/ublas/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/ublas/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1785 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/ublas/main.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4341 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/ublas/ublas_interface.hh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3269 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/check_cache_queries.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6416 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/dense_solvers.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7243 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/eig33.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3307 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/geometry.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.495041 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6574 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/changesets.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      193 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1382 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm_common.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm_settings.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      114 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm_square_settings.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      193 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1381 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv_common.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       79 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv_settings.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       88 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv_square_settings.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      205 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemvt.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2466 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/lazy_gemm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      132 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/lazy_gemm_settings.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      298 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/llt.cpp
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     2693 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/make_plot.sh
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.499040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3813 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/chart_footer.html
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14775 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/chart_header.html
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       25 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/footer.html
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      884 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/header.html
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   151723 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/s1.js
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   241320 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/s2.js
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     4090 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/run.sh
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     2031 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/runall.sh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      217 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/trmv_lo.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/trmv_lot.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      217 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/trmv_up.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/trmv_upt.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3232 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/product_threshold.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6006 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/quat_slerp.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1097 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/quatmul.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6260 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_cholesky.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5101 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_dense_product.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3011 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_lu.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8999 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_product.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3393 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_randomsetter.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13761 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_setter.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2347 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_transpose.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6114 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_trisolver.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.499040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3061 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3975 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/sp_solver.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1856 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/spbench.dtd
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3301 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/spbenchsolver.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18167 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/spbenchsolver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3825 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/spbenchstyle.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2831 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/test_sparseLU.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6096 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/spmv.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.503040 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1496 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/README
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1585 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/benchmark.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6834 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/benchmark_main.cc
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1389 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/contraction_benchmarks_cpu.cc
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)      729 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/eigen_sycl_bench.sh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      647 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/eigen_sycl_bench_contract.sh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20459 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6264 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_cpu.cc
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3381 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_fp16_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3373 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6273 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_sycl.cc
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11331 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_contract_sycl_bench.cc
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1203 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/bench/vdw_new.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.507041 aplr-6.5.1/dependencies/eigen-3.4.0/blas/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3614 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/BandTriangularSolver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1730 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1608 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/GeneralRank1Update.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2036 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/PackedSelfadjointProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3165 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/PackedTriangularMatrixVector.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3191 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/PackedTriangularSolverVector.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      183 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/README.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2168 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/Rank2Update.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4672 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/common.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      647 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/complex_double.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      646 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/complex_single.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1507 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/double.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.515040 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15108 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/chbmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13026 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/chpmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2310 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/complexdots.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18945 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/ctbmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      117 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/d_cnjg.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      657 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/datatypes.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4968 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/drotm.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6193 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/drotmg.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10188 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/dsbmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8075 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/dspmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11657 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/dtbmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2976 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/lsame.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      105 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/r_cnjg.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4902 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/srotm.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6056 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/srotmg.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10210 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/ssbmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8051 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/sspmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11643 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/stbmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15144 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/zhbmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13060 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/zhpmv.c
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18973 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/ztbmv.c
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.515040 aplr-6.5.1/dependencies/eigen-3.4.0/blas/fortran/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      979 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/fortran/complexdots.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5646 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/level1_cplx_impl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3892 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/level1_impl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4267 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/level1_real_impl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12223 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/level2_cplx_impl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25172 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/level2_impl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10499 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/level2_real_impl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    38043 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/level3_impl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      763 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/single.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.531041 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      948 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    32110 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat1.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1546 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat2.dat
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   116657 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat2.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1046 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat3.dat
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   131550 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat3.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    44820 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat1.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1466 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat2.dat
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   112335 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat2.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      882 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat3.dat
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   104262 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat3.f
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1016 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/runblastest.sh
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    43389 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat1.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1466 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat2.dat
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   112251 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat2.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      882 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat3.dat
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   104172 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat3.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    32115 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat1.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1546 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat2.dat
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   117003 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat2.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1046 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat3.dat
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   131995 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat3.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      389 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/blas/xerbla.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.535041 aplr-6.5.1/dependencies/eigen-3.4.0/ci/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6736 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/ci/CTest2JUnit.xsl
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4910 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/ci/README.md
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5024 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/ci/build.gitlab-ci.yml
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3490 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/ci/smoketests.gitlab-ci.yml
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10349 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/ci/test.gitlab-ci.yml
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.543041 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2171 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/ComputeCppCompilerChecks.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      475 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/ComputeCppIRMap.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      802 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/Eigen3Config.cmake.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1397 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/Eigen3ConfigLegacy.cmake.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2779 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenConfigureTesting.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1562 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenDetermineOSVersion.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1814 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenDetermineVSServicePack.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2321 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenSmokeTestList.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29205 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenTesting.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1196 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenUninstall.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      517 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindAdolc.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    42828 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindBLAS.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13179 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindBLASEXT.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2413 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindCHOLMOD.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16685 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindComputeCpp.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2636 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindEigen2.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3509 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindEigen3.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2783 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindFFTW.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2943 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindGLEW.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      524 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindGMP.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4992 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindGSL.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      846 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindGoogleHash.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11729 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindHWLOC.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1281 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindKLU.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9734 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindLAPACK.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2632 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindMPFR.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3524 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindMPREAL.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8969 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindMetis.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23160 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindPASTIX.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14417 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindPTSCOTCH.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12034 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindSCOTCH.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1142 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindSPQR.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2482 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindStandardMathLibrary.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2261 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindSuperLU.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5111 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindTriSYCL.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1662 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindUMFPACK.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      910 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/RegexUtils.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      177 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/cmake/UseEigen3.cmake
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.379040 aplr-6.5.1/dependencies/eigen-3.4.0/debug/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.543041 aplr-6.5.1/dependencies/eigen-3.4.0/debug/gdb/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       22 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/debug/gdb/__init__.py
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9617 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/debug/gdb/printers.py
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.543041 aplr-6.5.1/dependencies/eigen-3.4.0/debug/msvc/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11661 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/debug/msvc/eigen.natvis
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7566 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/debug/msvc/eigen_autoexp_part.dat
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.543041 aplr-6.5.1/dependencies/eigen-3.4.0/demos/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      278 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/CMakeLists.txt
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.543041 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mandelbrot/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      462 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mandelbrot/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      336 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mandelbrot/README
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7509 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mandelbrot/mandelbrot.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1888 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mandelbrot/mandelbrot.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.543041 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      262 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/README
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4158 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3346 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1616 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/example.c
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.547041 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      695 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      403 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/README
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5981 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/camera.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3435 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/camera.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3974 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/gpuhelper.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7177 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/gpuhelper.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3927 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/icosphere.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      869 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/icosphere.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19192 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/quaternion_demo.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2635 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/quaternion_demo.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1756 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/trackball.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      943 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/trackball.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.563041 aplr-6.5.1/dependencies/eigen-3.4.0/doc/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11165 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/AsciiQuickReference.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2425 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/B01_Experimental.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4935 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6332 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/ClassHierarchy.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18692 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/CoeffwiseMathFunctionsTable.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4423 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/CustomizingEigen_CustomScalar.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1337 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/CustomizingEigen_InheritingMatrix.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3658 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/CustomizingEigen_NullaryExpr.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3658 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/CustomizingEigen_Plugins.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5021 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/DenseDecompositionBenchmark.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    86035 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/Doxyfile.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8355 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/Eigen_Silly_Professor_64x64.png
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1906 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/FixedSizeVectorizable.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13458 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/FunctionsTakingEigenTypes.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5429 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/HiPerformance.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3797 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/InplaceDecomposition.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30585 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/InsideEigenExample.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3150 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/LeastSquares.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6761 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/Manual.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      758 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/MatrixfreeSolverExample.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5610 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/NewExpressionType.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1929 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/Overview.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1166 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/PassingByValue.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7018 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/Pitfalls.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14277 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/PreprocessorDirectives.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29844 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/QuickReference.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6578 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/QuickStartGuide.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19902 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/SparseLinearSystems.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8312 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/SparseQuickReference.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3923 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/StlContainers.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4119 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/StorageOrders.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7026 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/StructHavingEigenMembers.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6157 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TemplateKeyword.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10269 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicAliasing.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5285 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicAssertions.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1914 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicCMakeGuide.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      173 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicEigenExpressionTemplates.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6314 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicLazyEvaluation.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9068 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicLinearAlgebraDecompositions.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3749 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicMultithreading.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      137 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicResizing.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      145 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicScalarTypes.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       97 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicVectorization.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6900 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialAdvancedInitialization.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8523 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialArrayClass.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8288 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialBlockOperations.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9731 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialGeometry.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11860 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialLinearAlgebra.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3988 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialMapClass.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9865 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialMatrixArithmetic.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13680 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialMatrixClass.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12006 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialReductionsVisitorsBroadcasting.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2981 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialReshape.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2142 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialSTL.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8209 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialSlicingIndexing.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20483 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialSparse.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       89 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialSparse_example_details.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8737 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/UnalignedArrayAssert.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6633 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/UsingBlasLapackBackends.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6113 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/UsingIntelMKL.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1855 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/UsingNVCC.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2924 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/WrongStackAlignment.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8006 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigen_navtree_hacks.js
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4584 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy.css
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      680 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy_footer.html.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2521 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy_header.html.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5337 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy_layout.xml.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1095 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy_tabs.css
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.579041 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       34 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/.krazy
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      607 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      766 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/CustomizingEigen_Inheritance.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      189 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Cwise_erf.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      190 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Cwise_erfc.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      192 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Cwise_lgamma.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      282 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/DenseBase_middleCols_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      282 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/DenseBase_middleRows_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      283 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/DenseBase_template_int_middleCols.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      283 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/DenseBase_template_int_middleRows.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      206 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/QuickStart_example.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      305 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/QuickStart_example2_dynamic.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      289 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/QuickStart_example2_fixed.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      677 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TemplateKeyword_flexible.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      508 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TemplateKeyword_simple.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1589 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialInplaceLU.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      622 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgComputeTwice.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      371 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgExComputeSolveError.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      381 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      356 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgExSolveLDLT.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      348 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgInverseDeterminant.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      600 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgRankRevealing.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      405 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgSVDSolve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      534 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      377 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgSetThreshold.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      466 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_accessors.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      400 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_addition.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      410 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      444 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      591 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      237 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_mult.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      523 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      390 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_colrow.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      448 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_corner.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      413 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_print_block.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      348 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_vector.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      401 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_PartialLU_solve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      440 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      356 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      361 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      247 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      502 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      513 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      675 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      447 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      244 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      531 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      680 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_simple_example_dynamic_size.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      282 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_simple_example_fixed_size.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      737 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_Block.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      526 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_CwiseBinaryOp.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      561 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_CwiseUnaryOp.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      371 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      697 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_FixedBlock.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      467 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_FixedReshaped.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      673 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_FixedVectorBlock.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      545 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_Reshaped.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      775 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_VectorBlock.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      418 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/function_taking_eigenbase.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      594 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/function_taking_ref.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      366 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      145 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.entry
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      948 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.evaluator
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      591 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.expression
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      146 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.main
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       85 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.preamble
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      605 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.traits
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1320 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4275 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/matrixfree_cg.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2455 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/nullary_indexing.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      471 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_add_sub.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      393 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_dot_cross.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      612 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_matrix_mul.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      529 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_redux_basic.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      353 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_scalar_mul_div.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      343 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_matrix_coefficient_accessors.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      489 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_matrix_resize.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_matrix_resize_fixed_size.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       86 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/ftv2node.png
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/ftv2pnode.png
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.635041 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       34 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/.krazy
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      210 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/AngleAxis_mimic_euler.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Array_initializer_list_23_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       63 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Array_initializer_list_vector_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      102 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Array_variadic_ctor_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      394 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/BiCGSTAB_simple.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      407 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/BiCGSTAB_step_by_step.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1624 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      324 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/ColPivHouseholderQR_solve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      792 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/ComplexEigenSolver_compute.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      216 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      194 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      301 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/ComplexSchur_compute.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      263 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/ComplexSchur_matrixT.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      221 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/ComplexSchur_matrixU.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_abs.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       46 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_abs2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_acos.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       85 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_arg.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      232 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_array_power_array.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_asin.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       65 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_atan.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_boolean_and.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      105 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_boolean_not.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_boolean_or.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       63 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_boolean_xor.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       92 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_ceil.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       58 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_cos.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_cosh.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       44 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_cube.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_equal_equal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       43 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_exp.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       93 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_floor.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       51 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_greater.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_greater_equal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       47 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_inverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      104 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_isFinite.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      101 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_isInf.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      101 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_isNaN.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       51 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_less.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_less_equal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       43 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_log.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       47 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_log10.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       54 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_max.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       54 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_min.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       39 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_minus.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_minus_equal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_not_equal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       39 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_plus.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_plus_equal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       53 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_pow.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      141 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_product.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       49 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_quotient.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       92 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_rint.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       93 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_round.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       85 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_scalar_power_array.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_sign.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       58 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_sin.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_sinh.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_slash_equal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       44 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_sqrt.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       46 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_square.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       58 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_tan.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       64 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_tanh.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Cwise_times_equal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      117 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/DenseBase_LinSpaced.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      420 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/DenseBase_LinSpacedInt.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      139 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/DenseBase_LinSpaced_seq_deprecated.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/DenseBase_setLinSpaced.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      368 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/DirectionWise_hnormalized.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      186 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/DirectionWise_replicate.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      179 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/DirectionWise_replicate_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      800 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      361 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_compute.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      176 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_eigenvalues.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      181 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_eigenvectors.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      430 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      325 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/FullPivHouseholderQR_solve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      369 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/FullPivLU_image.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      317 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/FullPivLU_kernel.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      413 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/FullPivLU_solve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      456 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/GeneralizedEigenSolver.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      339 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/HessenbergDecomposition_compute.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      391 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/HessenbergDecomposition_matrixH.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      482 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      300 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/HouseholderQR_householderQ.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      357 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/HouseholderQR_solve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1316 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      603 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/IOFormat.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      614 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/JacobiSVD_basic.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      236 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Jacobi_makeGivens.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      293 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Jacobi_makeJacobi.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      519 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/LLT_example.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      456 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/LLT_solve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      192 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/LeastSquaresNormalEquations.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      177 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/LeastSquaresQR.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      164 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Map_general_stride.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      199 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Map_inner_stride.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      138 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Map_outer_stride.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      183 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Map_placement_new.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       93 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Map_simple.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_adjoint.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      523 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_all.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      207 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_applyOnTheLeft.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      292 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_applyOnTheRight.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       70 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_array.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      234 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_array_const.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       56 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_asDiagonal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      244 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_block_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      250 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_block_int_int_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      271 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      274 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      242 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_bottomRows_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      119 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cast.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       82 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_col.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      287 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_colwise.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      471 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_colwise_iterator_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      410 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      318 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       80 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseAbs.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       81 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseAbs2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       95 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseArg.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      276 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseEqual.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       87 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseInverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseMax.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseMin.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      286 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseNotEqual.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      153 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseProduct.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       65 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseQuotient.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       80 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseSign.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       50 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_cwiseSqrt.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      188 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_diagonal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      270 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_diagonal_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      274 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_diagonal_template_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      160 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_eigenvalues.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      226 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_end_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      467 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_eval.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      274 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      377 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_hnormalized.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      487 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_homogeneous.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       50 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_identity.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       42 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_identity_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      145 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_inverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      241 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isDiagonal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      235 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isIdentity.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      216 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isOnes.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      293 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isOrthogonal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      231 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isUnitary.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      215 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_isZero.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      236 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_leftCols_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      129 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_noalias.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       75 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_ones.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       77 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_ones_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       37 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_ones_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      132 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_operatorNorm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      171 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_prod.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       42 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_random.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       37 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_random_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       39 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_random_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      170 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_replicate.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      163 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_replicate_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      291 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_auto.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      178 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_fixed.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      160 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      287 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_to_vector.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      407 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_reverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      239 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_rightCols_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       82 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_row.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      281 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_rowwise.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      244 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_segment_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      115 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_select.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      361 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_selfadjointView.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      290 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_set.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       83 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_setIdentity.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       72 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_setOnes.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       72 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_setRandom.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       72 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_setZero.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      226 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_start_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      248 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_bottomRows.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      230 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_end.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      264 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      274 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      301 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      277 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      304 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      265 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      292 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      268 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      295 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      242 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_leftCols.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      245 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_rightCols.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      244 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_segment.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      230 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_start.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      239 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_template_int_topRows.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      262 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      265 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      233 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_topRows_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      414 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_transpose.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      573 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_triangularView.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       71 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_zero.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       73 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_zero_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       37 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_zero_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      157 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_Map_stride.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       60 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_initializer_list_23_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       40 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_initializer_list_vector_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      111 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_resize_NoChange_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      235 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_resize_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      111 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_resize_int_NoChange.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      407 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_resize_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_setConstant_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       55 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_setConstant_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       52 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_setIdentity_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_setOnes_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       48 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_setOnes_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       47 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_setRandom_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       50 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_setRandom_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       45 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_setZero_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       48 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_setZero_int_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      104 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Matrix_variadic_ctor_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      372 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/PartialPivLU_solve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      263 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_count.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      176 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_maxCoeff.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      176 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_minCoeff.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_norm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      169 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_prod.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_squaredNorm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      164 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/PartialRedux_sum.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      819 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/RealQZ_compute.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      429 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      343 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/RealSchur_compute.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      362 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      816 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      826 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      365 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      396 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      193 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      426 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      363 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      184 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointView_eigenvalues.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      157 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointView_operatorNorm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      167 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Slicing_arrayexpr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      369 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Slicing_custom_padding_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      190 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Slicing_rawarray_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      164 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Slicing_stdvector_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      411 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SparseMatrix_coeffs.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      267 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_block.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      270 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_block_correct.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      591 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_cwise.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       76 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      230 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       86 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult3.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      102 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult4.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      109 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_mult5.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      525 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicStorageOrders_example.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      520 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Triangular_solve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      445 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      392 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_compute.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      550 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      552 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_diagonal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      303 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_householderCoefficients.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      394 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_packedMatrix.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      132 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      168 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      266 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      272 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      878 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      332 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      299 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_Map_rowmajor.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      896 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_Map_using.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      171 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      299 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      611 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_SlicingCol.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      180 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_SlicingVec.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       70 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_commainit_01.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      113 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_commainit_01b.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      215 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_commainit_02.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      117 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_range_for_loop_1d_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      148 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_range_for_loop_2d_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      249 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_reshaped_vs_resize_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      372 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_reshaped_vs_resize_2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      146 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_matrix_inverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      318 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_multiple_rhs.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      368 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      256 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_singular.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      273 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_triangular.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      159 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_solve_triangular_inplace.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      203 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_std_sort.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      218 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_std_sort_rows_cxx11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      461 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/VectorwiseOp_homogeneous.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      536 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Vectorwise_reverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      732 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/class_FullPivLU.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      555 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/compile_snippet.cpp.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      468 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/tut_arithmetic_redux_minmax.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      188 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      277 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      174 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_inplace.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      193 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/tut_matrix_assignment_resizing.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.635041 aplr-6.5.1/dependencies/eigen-3.4.0/doc/special_examples/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1114 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/special_examples/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1184 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1576 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example_details.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      336 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/special_examples/random_cpp11.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2544 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/doc/tutorial.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      254 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/eigen3.pc.in
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.655041 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2423 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      245 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/bdcsvd_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      233 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      233 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      261 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      262 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/block_on_const_type_actually_const_0.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      262 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/block_on_const_type_actually_const_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      257 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/colpivqr_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      245 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/const_qualified_block_method_retval_0.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      240 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/const_qualified_block_method_retval_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      239 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/const_qualified_diagonal_method_retval.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      241 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/const_qualified_transpose_method_retval.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      271 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      296 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/cwiseunaryview_on_const_type_actually_const.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      228 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      250 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/diagonal_on_const_type_actually_const.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      276 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/eigensolver_cplx.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      259 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/eigensolver_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      156 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/failtest_sanity_check.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      247 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/fullpivlu_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      258 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/fullpivqr_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      183 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/initializer_list_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      222 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/initializer_list_2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      248 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/jacobisvd_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      250 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/ldlt_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      248 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/llt_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      224 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      246 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      270 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      314 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      321 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      249 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/map_on_const_type_actually_const_0.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      241 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/map_on_const_type_actually_const_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      250 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/partialpivlu_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      251 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/qr_int.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      263 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/ref_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      213 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/ref_2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      231 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/ref_3.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      227 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/ref_4.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      238 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/ref_5.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      241 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      266 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/selfadjointview_on_const_type_actually_const.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      302 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/sparse_ref_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      238 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/sparse_ref_2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      271 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/sparse_ref_3.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      235 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/sparse_ref_4.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      285 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/sparse_ref_5.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      290 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/sparse_storage_mismatch.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      217 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/swap_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      211 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/swap_2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      213 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/ternary_1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      225 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/ternary_2.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      229 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      254 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/transpose_on_const_type_actually_const.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      238 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      265 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/failtest/triangularview_on_const_type_actually_const.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.663041 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10876 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2205 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/cholesky.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2831 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clacgv.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2340 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/cladiv.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6295 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clarf.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23424 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clarfb.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5344 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clarfg.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10450 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clarft.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      578 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/complex_double.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      577 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/complex_single.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2969 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dladiv.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5259 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlamch.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2514 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlapy2.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2737 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlapy3.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6167 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlarf.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22749 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlarfb.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4946 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlarfg.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10222 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlarft.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      562 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/double.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1282 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dsecnd_NONE.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1826 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/eigenvalues.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2957 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilaclc.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2997 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilaclr.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2952 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/iladlc.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3000 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/iladlr.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2941 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilaslc.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2988 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilaslr.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2962 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilazlc.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3010 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilazlr.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      877 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/lapack_common.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2655 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/lu.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1258 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/second_NONE.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      561 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/single.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2897 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/sladiv.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5261 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slamch.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2490 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slapy2.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2701 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slapy3.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6117 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slarf.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22727 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slarfb.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4908 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slarfg.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10183 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slarft.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4891 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/svd.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2839 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlacgv.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2364 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zladiv.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6278 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlarf.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23498 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlarfb.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5359 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlarfg.f
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10453 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlarft.f
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.667041 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      328 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/CMakeLists.txt
+-rwxr-xr-x   0 mathiaso  (1000) mathiaso  (1001)      577 2021-08-18 18:41:58.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/buildtests.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1569 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/cdashtesting.cmake.in
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)      670 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/check.in
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)       44 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/debug.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6384 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/eigen_gen_credits.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      738 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/eigen_gen_docs
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      323 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/eigen_gen_split_test_help.cmake
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1009 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/eigen_monitor_perf.sh
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)       46 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/release.in
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2368 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/scripts/relicense.py
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      216 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/signature_of_eigen3_matrix_library
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.703042 aplr-6.5.1/dependencies/eigen-3.4.0/test/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5707 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/AnnoyingScalar.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14452 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1079 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/MovableScalar.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      605 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/SafeScalar.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8668 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/adjoint.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    27758 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/array_cwise.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12883 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/array_for_matrix.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      961 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/array_of_string.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2342 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/array_replicate.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6383 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/array_reverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2432 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/bandmatrix.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13366 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/basicstuff.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4443 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/bdcsvd.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17931 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/bfloat16_float.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1473 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/bicgstab.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6413 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/blasutil.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14816 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/block.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5731 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/boostmultiprec.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      174 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/bug1213.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      147 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/bug1213.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      279 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/bug1213_main.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18340 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/cholesky.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3377 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/cholmod_support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3150 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/commainitializer.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1543 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/conjugate_gradient.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5369 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/conservative_resize.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2562 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/constructor.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6448 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/corners.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2016 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/ctorleak.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5062 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/denseLM.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7256 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/dense_storage.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2275 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/determinant.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4115 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/diagonal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6686 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/diagonal_matrix_variadic_ctor.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7531 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/diagonalmatrices.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2229 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/dontalign.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4760 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/dynalloc.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2196 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/eigen2support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6221 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/eigensolver_complex.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4046 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/eigensolver_generalized_real.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9459 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/eigensolver_generic.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11419 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/eigensolver_selfadjoint.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/evaluator_common.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21038 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/evaluators.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1916 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/exceptions.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5256 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/fastmath.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1874 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/first_aligned.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18093 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_alignedbox.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3562 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_eulerangles.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5470 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_homogeneous.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7304 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_hyperplane.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4838 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_orthomethods.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4974 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_parametrizedline.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11568 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_quaternion.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26366 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_transformations.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16082 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/gpu_basic.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5456 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/gpu_common.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14524 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/half_float.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2404 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/hessenberg.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6286 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/householder.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2623 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/incomplete_cholesky.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19424 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/indexed_view.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12744 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/initializer_list_construction.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3880 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/inplace_decomposition.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5793 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/integer_types.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4701 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/inverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1833 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/io.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1368 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/is_same_dense.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2733 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/jacobi.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5877 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/jacobisvd.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      955 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/klu_support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6130 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/linearstructure.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1499 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/lscg.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9075 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/lu.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    33109 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/main.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7943 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/mapped_matrix.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7471 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/mapstaticmethods.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11369 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/mapstride.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7339 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/meta.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      751 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/metis_support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1789 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/miscmatrices.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17824 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/mixingtypes.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      635 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/mpl2only.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1208 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/nestbyvalue.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4377 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/nesting_ops.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8700 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/nomalloc.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12806 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/nullary.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3212 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/num_dimensions.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9042 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/numext.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    55436 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/packetmath.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9016 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/packetmath_test_shared.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      955 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/pardiso_support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1902 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/pastix_support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7031 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/permutationmatrices.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3120 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/prec_inverse_4x4.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11880 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15711 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_extra.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5395 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_large.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4447 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_mmtr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10988 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_notemporary.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3510 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_selfadjoint.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12656 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_small.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6133 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_symm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7856 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_syrk.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6921 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_trmm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4250 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_trmv.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6102 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/product_trsolve.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4673 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/qr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13867 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/qr_colpivoting.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5600 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/qr_fullpivoting.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4621 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/qtvector.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4373 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/rand.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7174 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/random_without_cast_overflow.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3102 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/real_qz.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8239 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/redux.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14363 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/ref.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10706 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/reshape.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1105 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/resize.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5668 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/rvalue_types.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3569 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/schur_complex.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3964 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/schur_real.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2419 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/selfadjoint.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2564 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/simplicial_cholesky.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2038 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sizeof.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2639 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sizeoverflow.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2133 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/smallvectors.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1716 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/solverbase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6216 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4740 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparseLM.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29343 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_basic.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12153 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_block.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9997 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_permutations.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25557 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_product.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6125 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_ref.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24396 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_solver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5142 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_solvers.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5087 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_vector.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1791 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparselu.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4587 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/sparseqr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1762 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/special_numbers.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   159516 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/split_test_helper.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1841 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/spqr_support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10379 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/stable_norm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4260 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/stddeque.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4738 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/stddeque_overload.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4232 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/stdlist.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5852 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/stdlist_overload.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5116 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/stdvector.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5014 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/stdvector_overload.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19411 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/stl_iterators.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      956 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/superlu_support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19317 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/svd_common.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4050 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/svd_fill.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2940 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/swap.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2742 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/symbolic_index.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11918 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/triangular.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2024 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/type_alias.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5859 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/umeyama.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1171 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/umfpack_support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2565 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/unalignedcount.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1716 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/upperbidiagonalization.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20351 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/vectorization_logic.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11489 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/vectorwiseop.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6384 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/visitor.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3734 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/test/zerosized.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.703042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      293 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/CMakeLists.txt
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.707042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4422 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/AdolcForward
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6349 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/AlignedVector3
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      884 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/ArpackSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1181 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/AutoDiff
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5523 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/BVH
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      603 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CMakeLists.txt
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.707042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      307 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4187 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/Tensor
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1267 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/TensorSymmetry
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2087 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/ThreadPool
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.379040 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.731042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    62365 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/README.md
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21269 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12448 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10323 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    57932 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    60851 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    42150 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19707 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15665 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    45320 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2675 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      225 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    63402 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23586 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    89042 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    70687 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18803 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    48686 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    27527 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8642 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13146 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4896 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      215 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3427 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12837 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40367 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15203 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7674 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17751 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8556 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40005 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26655 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16115 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    24345 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14486 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8782 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8320 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15269 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10920 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1316 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4068 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1267 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2560 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28066 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25692 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9094 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2730 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9041 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7769 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3642 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14191 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8104 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    43284 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28764 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11474 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12385 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    44395 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      221 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40719 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30074 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14793 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16938 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20091 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25279 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18256 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5481 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13513 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10152 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9432 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7552 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30089 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.731042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10857 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9086 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13021 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.731042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21046 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.735042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2113 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9121 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17075 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9366 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      774 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1209 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11482 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1680 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      715 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.735042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22752 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4115 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8155 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/EmulateArray.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4174 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1126 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/EulerAngles
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13948 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/FFT
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1561 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/IterativeSolvers
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      944 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/KroneckerProduct
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1238 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/LevenbergMarquardt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7656 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/MPRealSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17919 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/MatrixFunctions
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      592 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/MoreVectorization
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5963 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/NonLinearOptimization
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1779 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/NumericalDiff
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19072 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/OpenGLSupport
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4749 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/Polynomials
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      930 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/Skyline
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1360 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/SparseExtra
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2951 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/SpecialFunctions
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      996 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/Splines
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.383040 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.735042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3150 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    29107 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9029 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.735042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12976 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/BVAlgorithms.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9166 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/KdBVH.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.735042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29075 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.735042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      174 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15367 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerAngles.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11620 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerSystem.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.735042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9223 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_fftw_impl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13231 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.739042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5324 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17769 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10209 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/GMRES.h
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)    14794 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IDRS.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2520 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5360 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IterationController.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12397 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/MINRES.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5853 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/Scaling.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.739042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10250 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.739042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2194 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2443 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6648 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5039 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6805 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13297 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.743042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16624 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22671 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17557 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23422 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14212 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2107 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.743042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3035 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.743042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    19837 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22135 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1864 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/chkder.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1915 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/covar.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3297 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2225 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9111 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3264 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1081 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3083 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1362 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.743042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4020 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.743042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8076 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/Companion.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15683 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4806 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.751042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11365 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    31105 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7837 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10853 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineProduct.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7966 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineStorage.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3153 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineUtil.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.751042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4260 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    40316 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13744 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8416 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MarketIO.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7568 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12423 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/RandomSetter.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.755042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10015 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2724 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    12641 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2544 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    69632 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4006 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2489 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7694 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3087 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11700 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2899 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    58539 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3713 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.383040 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.755042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1492 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      398 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.755042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1549 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      415 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.755042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10864 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.759042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2258 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1283 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.759042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18307 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/Spline.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16505 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFitting.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4312 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFwd.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1876 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/README.txt
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.759042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/bench/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3906 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/bench/bench_svd.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.759042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      114 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      878 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/Overview.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      345 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/SYCL.dox
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5283 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/eigendoxy_layout.xml.in
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.763042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2108 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/BVH_Example.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      736 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1847 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/EulerAngles.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2522 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/FFT.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      356 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixExponential.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      469 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixFunction.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      375 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixLogarithm.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      364 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixPower.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      424 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixPower_optimal.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      508 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixSine.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      524 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixSinh.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      434 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixSquareRoot.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2392 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/PolynomialSolver1.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      635 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/PolynomialUtils1.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.763042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1409 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2551 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/CwiseMul.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.763042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/snippets/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1137 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/snippets/CMakeLists.txt
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.795042 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7190 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/BVH.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15348 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/CMakeLists.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9623 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/EulerAngles.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       47 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/FFT.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9233 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/FFTW.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    64597 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/NonLinearOptimization.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2862 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/NumericalDiff.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2366 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/alignedvector3.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    10992 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/autodiff.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2943 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/autodiff_scalar.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    16409 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/bessel_functions.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3990 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_eventcount.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1839 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_maxsizevector.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18740 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_meta.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5039 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_non_blocking_thread_pool.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7024 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_runqueue.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9150 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8886 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9949 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9707 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_assign.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22378 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_access.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    31888 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_eval.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15858 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_io.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5708 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9209 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcasting.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15767 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_builtins_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2420 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_cast_float16_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5526 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_casts.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13050 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26158 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1991 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_comparisons.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2871 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6636 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4624 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8411 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1660 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_const.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7350 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    47521 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23176 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contraction.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5381 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    20033 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2518 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_index.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3211 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6806 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13495 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_device.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3210 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_device_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2578 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_dimension.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      999 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_empty.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    30675 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_executor.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14224 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_expr.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13705 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_fft.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7252 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_fixed_size.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2167 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3461 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2266 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_generator.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5732 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_generator_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    58446 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5942 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_ifft.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3890 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_op_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    36037 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    62111 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18652 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_index_list.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2109 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5101 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4129 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_intdiv.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3277 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_io.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1639 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4730 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      950 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_lvalue.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7962 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_map.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      993 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_math.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3877 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_math_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1501 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_mixed_indices.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18215 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17549 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1734 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_move.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1789 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_notification.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2893 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_complex.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2430 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_const_values.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    21223 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_float16_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3766 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_strings.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2652 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_padding.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5677 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_padding_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5499 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_patch.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9385 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_patch_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2513 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2355 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3568 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15346 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5410 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    42176 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6722 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_ref.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5285 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9283 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1486 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_roundings.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2978 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2576 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_gpu.cu
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6376 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7692 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4265 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9624 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_simple.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3024 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_striding.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7074 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_striding_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1896 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_sugar.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14828 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    59079 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_symmetry.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4237 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_local.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    25491 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_pool.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5129 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_trace.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5757 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_uint128.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4592 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11972 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1279 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/dgmres.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3822 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/forward_adolc.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1245 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/gmres.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      942 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/idrs.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9075 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/kronecker_product.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    55504 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/levenberg_marquardt.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4417 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_exponential.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7447 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_function.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2106 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_functions.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7178 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_power.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1050 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_square_root.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1658 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/minres.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2439 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/mpreal_support.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18637 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/openglsupport.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7486 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/polynomialsolver.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     3582 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/polynomialutils.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8414 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/sparse_extra.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    22854 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/special_functions.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     6372 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/special_packetmath.cpp
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8529 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/splines.cpp
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.795042 aplr-6.5.1/dependencies/pybind11/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1684 2022-05-09 14:53:50.000000 aplr-6.5.1/dependencies/pybind11/LICENSE.txt
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      414 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/__init__.py
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1544 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/__main__.py
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      228 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/_version.py
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1226 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/commands.py
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.383040 aplr-6.5.1/dependencies/pybind11/include/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.807042 aplr-6.5.1/dependencies/pybind11/include/pybind11/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    23959 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7069 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    65660 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8458 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      120 2023-07-14 06:11:46.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2096 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.811042 aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    28518 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    52930 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5491 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17869 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    26305 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    42613 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1625 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.811042 aplr-6.5.1/dependencies/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    31450 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    18140 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      316 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    13471 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4731 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     5002 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8262 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8862 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    79416 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     9103 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     2734 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)   126420 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    94641 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.819042 aplr-6.5.1/dependencies/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4185 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    15337 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    29747 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/include/pybind11/stl_bind.h
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-14 06:11:46.000000 aplr-6.5.1/dependencies/pybind11/py.typed
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    17650 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/setup_helpers.py
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.383040 aplr-6.5.1/dependencies/pybind11/share/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.383040 aplr-6.5.1/dependencies/pybind11/share/cmake/
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.819042 aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    11190 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/FindPythonLibsNew.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)    14033 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11Common.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     7781 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11Config.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     1403 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11ConfigVersion.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8960 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11NewTools.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     4184 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11Targets.cmake
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)     8361 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11Tools.cmake
+drwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)        0 2023-07-21 18:19:07.819042 aplr-6.5.1/dependencies/pybind11/share/pkgconfig/
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)      171 2023-07-14 16:07:35.000000 aplr-6.5.1/dependencies/pybind11/share/pkgconfig/pybind11.pc
+-rw-rw-r--   0 mathiaso  (1000) mathiaso  (1001)       38 2023-07-21 18:19:07.819042 aplr-6.5.1/setup.cfg
+-rwxrwxr-x   0 mathiaso  (1000) mathiaso  (1001)     1236 2023-07-21 18:16:31.000000 aplr-6.5.1/setup.py
```

### Comparing `aplr-6.5.0/LICENSE` & `aplr-6.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/PKG-INFO` & `aplr-6.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 6.5.0
+Version: 6.5.1
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Description: Build predictive and interpretable parametric regression or classification machine learning models in Python based on the Automatic Piecewise Linear Regression methodology developed by Mathias von Ottenbreit.
 Platform: Windows
```

### Comparing `aplr-6.5.0/README.md` & `aplr-6.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/aplr/aplr.py` & `aplr-6.5.1/aplr/aplr.py`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/aplr.egg-info/PKG-INFO` & `aplr-6.5.1/aplr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 6.5.0
+Version: 6.5.1
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Description: Build predictive and interpretable parametric regression or classification machine learning models in Python based on the Automatic Piecewise Linear Regression methodology developed by Mathias von Ottenbreit.
 Platform: Windows
```

### Comparing `aplr-6.5.0/aplr.egg-info/SOURCES.txt` & `aplr-6.5.1/aplr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/APLRClassifier.h` & `aplr-6.5.1/cpp/APLRClassifier.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/APLRRegressor.h` & `aplr-6.5.1/cpp/APLRRegressor.h`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,16 @@
     void calculate_and_validate_validation_error(size_t boosting_step);
     void calculate_validation_error(size_t boosting_step, const VectorXd &predictions);
     void update_term_eligibility();
     void print_summary_after_boosting_step(size_t boosting_step);
     void update_coefficients_for_all_steps();
     void print_final_summary();
     void find_optimal_m_and_update_model_accordingly();
+    void remove_redundant_terms();
+    void remove_unused_terms();
     void name_terms(const MatrixXd &X, const std::vector<std::string> &X_names);
     void calculate_feature_importance_on_validation_set();
     void find_min_and_max_training_predictions_or_responses();
     void cleanup_after_fit();
     void validate_that_model_can_be_used(const MatrixXd &X);
     void throw_error_if_loss_function_does_not_exist();
     void throw_error_if_link_function_does_not_exist();
@@ -241,14 +243,16 @@
     define_training_and_validation_sets(X,y,sample_weight,validation_set_indexes,group);
     scale_training_observations_if_using_log_link_function();
     initialize(prioritized_predictors_indexes, monotonic_constraints, interaction_constraints);
     execute_boosting_steps();
     update_coefficients_for_all_steps();
     print_final_summary();
     find_optimal_m_and_update_model_accordingly();
+    remove_redundant_terms();
+    remove_unused_terms();
     revert_scaling_if_using_log_link_function();
     name_terms(X, X_names);
     calculate_feature_importance_on_validation_set();
     find_min_and_max_training_predictions_or_responses();
     cleanup_after_fit();
 }
 
@@ -1321,16 +1325,50 @@
     validation_error_steps.minCoeff(&best_boosting_step_index);
     intercept=intercept_steps[best_boosting_step_index];
     for (size_t i = 0; i < terms.size(); ++i)
     {
         terms[i].coefficient = terms[i].coefficient_steps[best_boosting_step_index];
     }
     m_optimal=best_boosting_step_index+1; 
+}
+
+void APLRRegressor::remove_redundant_terms()
+{
+    for(size_t i = 0; i < terms.size(); ++i)
+    {        
+        for(size_t j = 0; j < terms.size(); ++j)
+        {
+            bool term_is_used{!is_approximately_zero(terms[i].coefficient)};
+            bool other_term_is_used{!is_approximately_zero(terms[j].coefficient)};
+            if(i!=j && term_is_used && other_term_is_used && terms[i].equals_not_comparing_given_terms(terms[i],terms[j]))
+            {
+                VectorXd values_i{terms[i].calculate(X_train)};
+                VectorXd values_j{terms[j].calculate(X_train)};
+                bool terms_are_similar{values_i==values_j};
+                if(terms_are_similar)
+                {
+                    if(terms[i].get_interaction_level()>terms[j].get_interaction_level())
+                    {
+                        terms[j].coefficient+=terms[i].coefficient;
+                        terms[i].coefficient=0;
+                        break;
+                    }
+                    else
+                    {
+                        terms[i].coefficient+=terms[j].coefficient;
+                        terms[j].coefficient=0;
+                    }
+                }
+            }
+        }
+    }
+}
 
-    //Removing unused terms
+void APLRRegressor::remove_unused_terms()
+{
     std::vector<Term> terms_new;
     terms_new.reserve(terms.size());
     for (size_t i = 0; i < terms.size(); ++i)
     {
         bool term_is_used{!is_approximately_zero(terms[i].coefficient)};
         if(term_is_used)
             terms_new.push_back(terms[i]);
```

### Comparing `aplr-6.5.0/cpp/build/CMakeFiles/3.16.3/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `aplr-6.5.1/cpp/build/CMakeFiles/3.16.3/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/functions.h` & `aplr-6.5.1/cpp/functions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/main.cpp` & `aplr-6.5.1/cpp/main.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/pythonbinding.cpp` & `aplr-6.5.1/cpp/pythonbinding.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/term.h` & `aplr-6.5.1/cpp/term.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor cauchy group_mse validation.cpp` & `aplr-6.5.1/cpp/test ALRRegressor cauchy group_mse validation.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor cauchy.cpp` & `aplr-6.5.1/cpp/test ALRRegressor cauchy.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor custom loss and validation.cpp` & `aplr-6.5.1/cpp/test ALRRegressor custom loss and validation.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor custom loss.cpp` & `aplr-6.5.1/cpp/test ALRRegressor custom loss.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor gamma custom_link.cpp` & `aplr-6.5.1/cpp/test ALRRegressor gamma custom_link.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor gamma custom_validation.cpp` & `aplr-6.5.1/cpp/test ALRRegressor gamma custom_validation.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor gamma gini weighted.cpp` & `aplr-6.5.1/cpp/test ALRRegressor gamma gini weighted.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor gamma gini.cpp` & `aplr-6.5.1/cpp/test ALRRegressor gamma gini.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor gamma rank unweighted.cpp` & `aplr-6.5.1/cpp/test ALRRegressor gamma rank unweighted.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor gamma rank.cpp` & `aplr-6.5.1/cpp/test ALRRegressor gamma rank.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor gamma.cpp` & `aplr-6.5.1/cpp/test ALRRegressor gamma.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor group_mse.cpp` & `aplr-6.5.1/cpp/test ALRRegressor group_mse.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor int constr.cpp` & `aplr-6.5.1/cpp/test ALRRegressor int constr.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor inversegaussian.cpp` & `aplr-6.5.1/cpp/test ALRRegressor inversegaussian.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor logit.cpp` & `aplr-6.5.1/cpp/test ALRRegressor logit.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor mae.cpp` & `aplr-6.5.1/cpp/test ALRRegressor mae.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor monotonic.cpp` & `aplr-6.5.1/cpp/test ALRRegressor monotonic.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor negative_binomial.cpp` & `aplr-6.5.1/cpp/test ALRRegressor negative_binomial.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor poisson.cpp` & `aplr-6.5.1/cpp/test ALRRegressor poisson.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor poissongamma.cpp` & `aplr-6.5.1/cpp/test ALRRegressor poissongamma.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor quantile.cpp` & `aplr-6.5.1/cpp/test ALRRegressor quantile.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor rank.cpp` & `aplr-6.5.1/cpp/test ALRRegressor rank.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor weibull.cpp` & `aplr-6.5.1/cpp/test ALRRegressor weibull.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test ALRRegressor.cpp` & `aplr-6.5.1/cpp/test ALRRegressor.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test APLRClassifier multi_class other_params.cpp` & `aplr-6.5.1/cpp/test APLRClassifier multi_class other_params.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test APLRClassifier multi_class.cpp` & `aplr-6.5.1/cpp/test APLRClassifier multi_class.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test APLRClassifier two_class other_params.cpp` & `aplr-6.5.1/cpp/test APLRClassifier two_class other_params.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test APLRClassifier two_class val_index.cpp` & `aplr-6.5.1/cpp/test APLRClassifier two_class val_index.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test APLRClassifier two_class.cpp` & `aplr-6.5.1/cpp/test APLRClassifier two_class.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test functions.cpp` & `aplr-6.5.1/cpp/test functions.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/cpp/test term.cpp` & `aplr-6.5.1/cpp/test term.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab/issue_templates/Bug Report.md` & `aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab/issue_templates/Bug Report.md`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab/merge_request_templates/Merge Request Template.md` & `aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab/merge_request_templates/Merge Request Template.md`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/.gitlab-ci.yml` & `aplr-6.5.1/dependencies/eigen-3.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.APACHE` & `aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.APACHE`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.BSD` & `aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.BSD`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.GPL` & `aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.LGPL` & `aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.MINPACK` & `aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.MINPACK`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.MPL2` & `aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.MPL2`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/COPYING.README` & `aplr-6.5.1/dependencies/eigen-3.4.0/COPYING.README`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/CTestConfig.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/CTestConfig.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Cholesky` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/CholmodSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Core` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Core`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Eigenvalues` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Geometry` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Householder` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/IterativeLinearSolvers` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Jacobi` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/KLUSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/LU` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/LU`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/MetisSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/OrderingMethods` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/PaStiXSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/PardisoSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/QR` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/QR`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/QtAlignedMalloc` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SPQRSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SVD` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/Sparse` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SparseCholesky` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SparseCore` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SparseLU` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SparseQR` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/StdDeque` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/StdList` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/StdVector` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/SuperLUSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/UmfPackSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LDLT.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LLT.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LLT_LAPACKE.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/CholmodSupport/CholmodSupport.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ArithmeticSequence.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Array.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ArrayBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ArrayWrapper.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Assign.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/AssignEvaluator.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Assign_MKL.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/BandMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Block.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/BooleanRedux.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CommaInitializer.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ConditionEstimator.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CoreEvaluators.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CoreIterators.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseBinaryOp.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseNullaryOp.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseTernaryOp.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseUnaryOp.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseUnaryView.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DenseBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DenseCoeffsBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DenseStorage.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Diagonal.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DiagonalMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/DiagonalProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Dot.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/EigenBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ForceAlignedAccess.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Fuzzy.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/GeneralProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/GenericPacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/GlobalFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/IO.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/IndexedView.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Inverse.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Map.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/MapBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/MathFunctionsImpl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Matrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/MatrixBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/NestByValue.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/NoAlias.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/NumTraits.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/PartialReduxEvaluator.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/PermutationMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/PlainObjectBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Product.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ProductEvaluators.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Random.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Redux.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Ref.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Replicate.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Reshaped.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/ReturnByValue.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Reverse.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Select.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/SelfAdjointView.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/SelfCwiseBinaryOp.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Solve.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/SolveTriangular.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/SolverBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/StableNorm.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/StlIterators.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Stride.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Swap.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Transpose.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Transpositions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/TriangularMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/VectorBlock.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/VectorwiseOp.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/Visitor.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/Complex.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/TypeCasting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/Complex.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/Complex.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/CUDA/Complex.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/BFloat16.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/ConjHelper.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/Half.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/Settings.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/TypeCasting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/TypeCasting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/Complex.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/Complex.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/TypeCasting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/Complex.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/TypeCasting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/TypeCasting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/Complex.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/PacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/AssignmentFunctors.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/BinaryFunctors.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/NullaryFunctors.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/StlFunctors.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/TernaryFunctors.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/functors/UnaryFunctors.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/Parallelizer.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointRank2Update.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/BlasUtil.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/ConfigureVectorization.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/Constants.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/DisableStupidWarnings.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/ForwardDeclarations.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/IndexedViewHelper.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/IntegralConstant.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/MKL_support.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/Macros.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/Memory.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/Meta.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/ReenableStupidWarnings.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/ReshapedHelper.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/StaticAssert.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/SymbolicIndex.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Core/util/XprHelper.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/EigenSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealQZ.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/Tridiagonalization.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/AlignedBox.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/AngleAxis.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/EulerAngles.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Homogeneous.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Hyperplane.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/OrthoMethods.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/ParametrizedLine.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Quaternion.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Rotation2D.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/RotationBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Scaling.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Transform.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Translation.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/Umeyama.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Householder/BlockHouseholder.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Householder/Householder.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Householder/HouseholderSequence.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/Jacobi/Jacobi.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/KLUSupport/KLUSupport.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/Determinant.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/FullPivLU.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/InverseImpl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/PartialPivLU.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/LU/arch/InverseSize4.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/MetisSupport/MetisSupport.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Amd.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Ordering.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/PardisoSupport/PardisoSupport.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/FullPivHouseholderQR.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/HouseholderQR.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/BDCSVD.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/JacobiSVD.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/SVDBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SVD/UpperBidiagonalization.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/AmbiVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/CompressedStorage.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/MappedSparseMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseAssign.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseBlock.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseColEtree.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCompressedBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDenseProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDot.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseFuzzy.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMap.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrixBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparsePermutation.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseRedux.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseRef.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSolverBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseTranspose.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseTriangularView.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseUtil.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseView.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseCore/TriangularSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLUImpl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Memory.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Structs.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Utils.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pivotL.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pruneL.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SparseQR/SparseQR.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdDeque.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdList.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/StlSupport/details.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/Image.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/Kernel.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/RealSvd2x2.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/blas.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/lapack.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/misc/lapacke.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/BlockMethods.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/IndexedViewMethods.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/Eigen/src/plugins/ReshapedMethods.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/INSTALL` & `aplr-6.5.1/dependencies/eigen-3.4.0/INSTALL`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/BenchSparseUtil.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/BenchSparseUtil.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/BenchTimer.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/BenchTimer.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/BenchUtil.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/BenchUtil.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/README.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/README.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/analyze-blocking-sizes.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/analyze-blocking-sizes.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/basicbench.cxxlist` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/basicbench.cxxlist`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/basicbenchmark.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/basicbenchmark.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/basicbenchmark.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/basicbenchmark.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchBlasGemm.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchBlasGemm.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchCholesky.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchCholesky.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchEigenSolver.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchEigenSolver.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchFFT.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchFFT.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchGeometry.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchGeometry.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchVecAdd.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchVecAdd.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_gemm.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_gemm.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_move_semantics.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_move_semantics.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_multi_compilers.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_multi_compilers.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_norm.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_norm.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_reverse.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_reverse.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/bench_unrolling` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/bench_unrolling`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmark-blocking-sizes.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmark-blocking-sizes.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmark.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmark.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmarkSlice.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmarkSlice.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmarkX.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmarkX.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmarkXcwise.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmarkXcwise.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/benchmark_suite` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/benchmark_suite`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/COPYING` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/COPYING`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/README` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/README`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_aat_product.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_aat_product.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_ata_product.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_ata_product.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_atv_product.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_atv_product.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_axpby.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_axpby.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_axpy.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_axpy.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_cholesky.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_cholesky.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_ger.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_ger.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_hessenberg.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_hessenberg.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_lu_decomp.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_lu_decomp.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_lu_solve.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_lu_solve.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product_bis.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product_bis.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_vector_product.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_matrix_vector_product.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_partial_lu.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_partial_lu.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_rot.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_rot.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_symv.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_symv.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_syr2.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_syr2.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_trisolve.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_trisolve.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_trisolve_matrix.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_trisolve_matrix.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/actions/action_trmm.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/actions/action_trmm.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindACML.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindACML.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindATLAS.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindATLAS.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindBLAZE.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindBLAZE.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindBlitz.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindBlitz.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindCBLAS.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindCBLAS.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindMKL.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindMKL.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindMTL4.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindMTL4.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindOPENBLAS.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindOPENBLAS.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindPackageHandleStandardArgs.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/FindTvmet.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/FindTvmet.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/action_settings.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/action_settings.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/gnuplot_common_settings.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/gnuplot_common_settings.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/go_mean` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/go_mean`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/mean.cxx` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/mean.cxx`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/mk_gnuplot_script.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/mk_gnuplot_script.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/mk_mean_script.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/mk_mean_script.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/mk_new_gnuplot.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/mk_new_gnuplot.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/perlib_plot_settings.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/perlib_plot_settings.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/regularize.cxx` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/regularize.cxx`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/smooth.cxx` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/smooth.cxx`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/data/smooth_all.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/data/smooth_all.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/bench.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/bench.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/bench_parameter.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/bench_parameter.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/btl.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/btl.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_function.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_function.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_matrix.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_matrix.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_vector.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/init/init_vector.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/bench_static.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/bench_static.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/intel_bench_fixed_size.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/intel_bench_fixed_size.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/static_size_generator.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/static/static_size_generator.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/STL_perf_analyzer.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/STL_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/STL_timer.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/STL_timer.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_timer.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/portable_timer.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/x86_perf_analyzer.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/x86_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/x86_timer.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/timers/x86_timer.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/size_lin_log.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/size_lin_log.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/size_log.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/size_log.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/utilities.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/utilities.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/xy_file.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/generic_bench/utils/xy_file.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface_impl.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface_impl.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/c_interface_base.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/c_interface_base.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/main.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/BLAS/main.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/STL/STL_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/STL/STL_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/STL/main.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/STL/main.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blaze/blaze_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blaze/blaze_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blaze/main.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blaze/main.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/blitz_LU_solve_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/blitz_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/blitz_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/blitz_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/btl_blitz.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/btl_blitz.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/btl_tiny_blitz.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/btl_tiny_blitz.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/blitz/tiny_blitz_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/blitz/tiny_blitz_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/eigen2_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/eigen2_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_adv.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_adv.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_linear.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_matmat.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_vecmat.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen2/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/eigen3_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/eigen3_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_adv.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_adv.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_linear.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_matmat.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_vecmat.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/eigen3/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/gmm/gmm_LU_solve_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/gmm/gmm_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/gmm/gmm_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/gmm/gmm_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/gmm/main.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/gmm/main.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/main.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/main.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_linear.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_matmat.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_vecmat.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tensors/tensor_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tensors/tensor_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/main.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/main.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/tvmet_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/tvmet/tvmet_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/ublas/main.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/ublas/main.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/btl/libs/ublas/ublas_interface.hh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/btl/libs/ublas/ublas_interface.hh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/check_cache_queries.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/check_cache_queries.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/dense_solvers.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/dense_solvers.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/eig33.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/eig33.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/geometry.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/geometry.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/changesets.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/changesets.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm_common.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemm_common.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv_common.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/gemv_common.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/lazy_gemm.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/lazy_gemm.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/make_plot.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/make_plot.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/chart_footer.html` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/chart_footer.html`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/chart_header.html` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/chart_header.html`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/header.html` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/header.html`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/s1.js` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/s1.js`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/s2.js` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/resources/s2.js`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/run.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/run.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/perf_monitoring/runall.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/perf_monitoring/runall.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/product_threshold.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/product_threshold.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/quat_slerp.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/quat_slerp.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/quatmul.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/quatmul.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_cholesky.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_dense_product.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_dense_product.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_lu.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_lu.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_product.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_product.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_randomsetter.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_randomsetter.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_setter.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_setter.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_transpose.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_transpose.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/sparse_trisolver.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/sparse_trisolver.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/sp_solver.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/sp_solver.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/spbench.dtd` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/spbench.dtd`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/spbenchsolver.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/spbenchsolver.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/spbenchsolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/spbenchsolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/spbenchstyle.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/spbenchstyle.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/spbench/test_sparseLU.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/spbench/test_sparseLU.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/spmv.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/spmv.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/README` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/README`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/benchmark.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/benchmark.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/benchmark_main.cc` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/benchmark_main.cc`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/contraction_benchmarks_cpu.cc` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/contraction_benchmarks_cpu.cc`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/eigen_sycl_bench.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/eigen_sycl_bench.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/eigen_sycl_bench_contract.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/eigen_sycl_bench_contract.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_cpu.cc` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_cpu.cc`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_fp16_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_fp16_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_sycl.cc` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_benchmarks_sycl.cc`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/tensors/tensor_contract_sycl_bench.cc` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/tensors/tensor_contract_sycl_bench.cc`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/bench/vdw_new.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/bench/vdw_new.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/BandTriangularSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/BandTriangularSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/GeneralRank1Update.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/GeneralRank1Update.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/PackedSelfadjointProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/PackedSelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/PackedTriangularMatrixVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/PackedTriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/PackedTriangularSolverVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/PackedTriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/Rank2Update.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/Rank2Update.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/common.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/common.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/complex_double.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/complex_double.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/complex_single.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/complex_single.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/double.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/double.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/chbmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/chbmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/chpmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/chpmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/complexdots.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/complexdots.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/ctbmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/ctbmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/datatypes.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/datatypes.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/drotm.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/drotm.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/drotmg.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/drotmg.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/dsbmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/dsbmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/dspmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/dspmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/dtbmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/dtbmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/lsame.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/lsame.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/srotm.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/srotm.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/srotmg.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/srotmg.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/ssbmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/ssbmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/sspmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/sspmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/stbmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/stbmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/zhbmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/zhbmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/zhpmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/zhpmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/f2c/ztbmv.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/f2c/ztbmv.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/fortran/complexdots.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/fortran/complexdots.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/level1_cplx_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/level1_cplx_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/level1_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/level1_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/level1_real_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/level1_real_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/level2_cplx_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/level2_cplx_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/level2_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/level2_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/level2_real_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/level2_real_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/level3_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/level3_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/single.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/single.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat1.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat1.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat2.dat` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat2.dat`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat2.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat2.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat3.dat` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat3.dat`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/cblat3.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/cblat3.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat1.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat1.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat2.dat` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat2.dat`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat2.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat2.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat3.dat` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat3.dat`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/dblat3.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/dblat3.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/runblastest.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/runblastest.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat1.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat1.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat2.dat` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat2.dat`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat2.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat2.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat3.dat` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat3.dat`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/sblat3.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/sblat3.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat1.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat1.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat2.dat` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat2.dat`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat2.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat2.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat3.dat` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat3.dat`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/blas/testing/zblat3.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/blas/testing/zblat3.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/ci/CTest2JUnit.xsl` & `aplr-6.5.1/dependencies/eigen-3.4.0/ci/CTest2JUnit.xsl`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/ci/README.md` & `aplr-6.5.1/dependencies/eigen-3.4.0/ci/README.md`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/ci/build.gitlab-ci.yml` & `aplr-6.5.1/dependencies/eigen-3.4.0/ci/build.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/ci/smoketests.gitlab-ci.yml` & `aplr-6.5.1/dependencies/eigen-3.4.0/ci/smoketests.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/ci/test.gitlab-ci.yml` & `aplr-6.5.1/dependencies/eigen-3.4.0/ci/test.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/ComputeCppCompilerChecks.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/ComputeCppCompilerChecks.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/Eigen3Config.cmake.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/Eigen3Config.cmake.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/Eigen3ConfigLegacy.cmake.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/Eigen3ConfigLegacy.cmake.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenConfigureTesting.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenConfigureTesting.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenDetermineOSVersion.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenDetermineOSVersion.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenDetermineVSServicePack.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenDetermineVSServicePack.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenSmokeTestList.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenSmokeTestList.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenTesting.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenTesting.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/EigenUninstall.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/EigenUninstall.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindAdolc.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindAdolc.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindBLAS.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindBLAS.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindBLASEXT.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindBLASEXT.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindCHOLMOD.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindCHOLMOD.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindComputeCpp.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindComputeCpp.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindEigen2.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindEigen2.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindEigen3.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindFFTW.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindFFTW.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindGLEW.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindGLEW.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindGMP.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindGSL.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindGSL.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindGoogleHash.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindGoogleHash.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindHWLOC.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindHWLOC.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindKLU.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindKLU.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindLAPACK.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindLAPACK.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindMPFR.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindMPFR.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindMPREAL.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindMPREAL.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindMetis.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindMetis.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindPASTIX.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindPASTIX.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindPTSCOTCH.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindPTSCOTCH.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindSCOTCH.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindSCOTCH.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindSPQR.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindSPQR.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindStandardMathLibrary.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindStandardMathLibrary.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindSuperLU.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindSuperLU.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindTriSYCL.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindTriSYCL.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/FindUMFPACK.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/FindUMFPACK.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/cmake/RegexUtils.cmake` & `aplr-6.5.1/dependencies/eigen-3.4.0/cmake/RegexUtils.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/debug/gdb/printers.py` & `aplr-6.5.1/dependencies/eigen-3.4.0/debug/gdb/printers.py`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/debug/msvc/eigen.natvis` & `aplr-6.5.1/dependencies/eigen-3.4.0/debug/msvc/eigen.natvis`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/debug/msvc/eigen_autoexp_part.dat` & `aplr-6.5.1/dependencies/eigen-3.4.0/debug/msvc/eigen_autoexp_part.dat`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/mandelbrot/mandelbrot.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/mandelbrot/mandelbrot.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/mandelbrot/mandelbrot.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/mandelbrot/mandelbrot.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/example.c` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/mix_eigen_and_c/example.c`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/camera.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/camera.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/camera.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/camera.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/gpuhelper.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/gpuhelper.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/gpuhelper.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/gpuhelper.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/icosphere.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/icosphere.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/icosphere.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/icosphere.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/quaternion_demo.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/quaternion_demo.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/quaternion_demo.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/quaternion_demo.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/trackball.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/trackball.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/demos/opengl/trackball.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/demos/opengl/trackball.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/AsciiQuickReference.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/AsciiQuickReference.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/B01_Experimental.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/B01_Experimental.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/ClassHierarchy.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/ClassHierarchy.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/CoeffwiseMathFunctionsTable.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/CoeffwiseMathFunctionsTable.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/CustomizingEigen_CustomScalar.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/CustomizingEigen_CustomScalar.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/CustomizingEigen_InheritingMatrix.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/CustomizingEigen_InheritingMatrix.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/CustomizingEigen_NullaryExpr.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/CustomizingEigen_NullaryExpr.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/CustomizingEigen_Plugins.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/CustomizingEigen_Plugins.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/DenseDecompositionBenchmark.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/DenseDecompositionBenchmark.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/Doxyfile.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/Eigen_Silly_Professor_64x64.png` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/Eigen_Silly_Professor_64x64.png`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/FixedSizeVectorizable.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/FixedSizeVectorizable.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/FunctionsTakingEigenTypes.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/FunctionsTakingEigenTypes.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/HiPerformance.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/HiPerformance.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/InplaceDecomposition.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/InplaceDecomposition.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/InsideEigenExample.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/InsideEigenExample.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/LeastSquares.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/LeastSquares.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/Manual.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/Manual.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/MatrixfreeSolverExample.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/MatrixfreeSolverExample.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/NewExpressionType.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/NewExpressionType.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/Overview.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/Overview.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/PassingByValue.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/PassingByValue.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/Pitfalls.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/Pitfalls.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/PreprocessorDirectives.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/PreprocessorDirectives.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/QuickReference.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/QuickReference.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/QuickStartGuide.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/QuickStartGuide.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/SparseLinearSystems.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/SparseLinearSystems.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/SparseQuickReference.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/SparseQuickReference.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/StlContainers.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/StlContainers.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/StorageOrders.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/StorageOrders.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/StructHavingEigenMembers.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/StructHavingEigenMembers.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TemplateKeyword.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TemplateKeyword.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicAliasing.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicAliasing.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicAssertions.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicAssertions.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicCMakeGuide.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicCMakeGuide.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicLazyEvaluation.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicLazyEvaluation.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicLinearAlgebraDecompositions.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicLinearAlgebraDecompositions.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TopicMultithreading.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TopicMultithreading.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialAdvancedInitialization.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialAdvancedInitialization.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialArrayClass.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialArrayClass.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialBlockOperations.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialBlockOperations.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialGeometry.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialGeometry.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialLinearAlgebra.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialLinearAlgebra.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialMapClass.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialMapClass.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialMatrixArithmetic.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialMatrixArithmetic.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialMatrixClass.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialMatrixClass.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialReductionsVisitorsBroadcasting.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialReductionsVisitorsBroadcasting.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialReshape.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialReshape.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialSTL.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialSTL.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialSlicingIndexing.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialSlicingIndexing.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/TutorialSparse.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/TutorialSparse.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/UnalignedArrayAssert.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/UnalignedArrayAssert.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/UsingBlasLapackBackends.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/UsingBlasLapackBackends.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/UsingIntelMKL.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/UsingIntelMKL.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/UsingNVCC.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/UsingNVCC.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/WrongStackAlignment.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/WrongStackAlignment.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigen_navtree_hacks.js` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigen_navtree_hacks.js`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy.css` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy.css`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy_footer.html.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy_footer.html.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy_header.html.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy_header.html.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy_layout.xml.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy_layout.xml.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/eigendoxy_tabs.css` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/eigendoxy_tabs.css`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/CustomizingEigen_Inheritance.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/CustomizingEigen_Inheritance.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TemplateKeyword_flexible.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TemplateKeyword_flexible.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialInplaceLU.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialInplaceLU.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgComputeTwice.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgComputeTwice.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgRankRevealing.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgRankRevealing.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_block_assignment.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_block_assignment.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/Tutorial_simple_example_dynamic_size.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/Tutorial_simple_example_dynamic_size.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_Block.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_Block.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_CwiseBinaryOp.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_CwiseBinaryOp.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_CwiseUnaryOp.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_CwiseUnaryOp.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_FixedBlock.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_FixedBlock.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_FixedVectorBlock.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_FixedVectorBlock.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_Reshaped.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_Reshaped.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/class_VectorBlock.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/class_VectorBlock.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/function_taking_ref.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/function_taking_ref.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.evaluator` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.evaluator`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.expression` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.expression`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.traits` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant.cpp.traits`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/make_circulant2.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/make_circulant2.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/matrixfree_cg.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/matrixfree_cg.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/nullary_indexing.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/nullary_indexing.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_matrix_mul.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_matrix_mul.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_redux_basic.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/examples/tut_arithmetic_redux_basic.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/ComplexEigenSolver_compute.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/ComplexEigenSolver_compute.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/HouseholderSequence_HouseholderSequence.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/HouseholderSequence_HouseholderSequence.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/IOFormat.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/IOFormat.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/JacobiSVD_basic.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/JacobiSVD_basic.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/LLT_example.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/LLT_example.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_all.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_all.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_triangularView.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/MatrixBase_triangularView.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/RealQZ_compute.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/RealQZ_compute.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_cwise.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicAliasing_cwise.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/TopicStorageOrders_example.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/TopicStorageOrders_example.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Triangular_solve.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Triangular_solve.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_decomposeInPlace.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_decomposeInPlace.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_diagonal.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tridiagonalization_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_Map_using.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_Map_using.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Tutorial_SlicingCol.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Tutorial_SlicingCol.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/Vectorwise_reverse.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/Vectorwise_reverse.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/class_FullPivLU.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/class_FullPivLU.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/snippets/compile_snippet.cpp.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/snippets/compile_snippet.cpp.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/special_examples/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/special_examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example_details.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example_details.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/doc/tutorial.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/doc/tutorial.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/failtest/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/failtest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/cholesky.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/cholesky.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clacgv.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clacgv.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/cladiv.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/cladiv.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clarf.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clarf.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clarfb.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clarfb.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clarfg.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clarfg.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/clarft.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/clarft.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/complex_double.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/complex_double.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/complex_single.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/complex_single.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dladiv.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dladiv.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlamch.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlamch.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlapy2.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlapy2.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlapy3.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlapy3.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlarf.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlarf.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlarfb.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlarfb.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlarfg.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlarfg.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dlarft.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dlarft.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/double.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/double.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/dsecnd_NONE.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/dsecnd_NONE.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/eigenvalues.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/eigenvalues.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilaclc.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilaclc.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilaclr.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilaclr.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/iladlc.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/iladlc.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/iladlr.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/iladlr.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilaslc.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilaslc.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilaslr.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilaslr.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilazlc.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilazlc.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/ilazlr.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/ilazlr.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/lapack_common.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/lapack_common.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/lu.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/lu.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/second_NONE.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/second_NONE.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/single.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/single.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/sladiv.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/sladiv.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slamch.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slamch.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slapy2.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slapy2.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slapy3.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slapy3.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slarf.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slarf.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slarfb.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slarfb.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slarfg.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slarfg.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/slarft.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/slarft.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/svd.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/svd.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlacgv.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlacgv.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zladiv.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zladiv.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlarf.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlarf.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlarfb.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlarfb.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlarfg.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlarfg.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/lapack/zlarft.f` & `aplr-6.5.1/dependencies/eigen-3.4.0/lapack/zlarft.f`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/scripts/buildtests.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/scripts/buildtests.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/scripts/cdashtesting.cmake.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/scripts/cdashtesting.cmake.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/scripts/check.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/scripts/check.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/scripts/eigen_gen_credits.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/scripts/eigen_gen_credits.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/scripts/eigen_gen_docs` & `aplr-6.5.1/dependencies/eigen-3.4.0/scripts/eigen_gen_docs`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/scripts/eigen_monitor_perf.sh` & `aplr-6.5.1/dependencies/eigen-3.4.0/scripts/eigen_monitor_perf.sh`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/scripts/relicense.py` & `aplr-6.5.1/dependencies/eigen-3.4.0/scripts/relicense.py`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/AnnoyingScalar.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/AnnoyingScalar.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/MovableScalar.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/MovableScalar.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/SafeScalar.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/SafeScalar.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/adjoint.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/adjoint.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/array_cwise.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/array_cwise.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/array_for_matrix.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/array_for_matrix.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/array_of_string.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/array_of_string.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/array_replicate.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/array_replicate.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/array_reverse.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/array_reverse.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/bandmatrix.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/bandmatrix.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/basicstuff.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/basicstuff.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/bdcsvd.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/bdcsvd.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/bfloat16_float.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/bfloat16_float.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/bicgstab.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/bicgstab.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/blasutil.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/blasutil.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/block.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/block.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/boostmultiprec.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/boostmultiprec.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/cholesky.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/cholesky.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/cholmod_support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/cholmod_support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/commainitializer.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/commainitializer.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/conjugate_gradient.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/conjugate_gradient.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/conservative_resize.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/conservative_resize.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/constructor.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/constructor.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/corners.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/corners.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/ctorleak.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/ctorleak.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/denseLM.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/denseLM.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/dense_storage.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/dense_storage.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/determinant.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/determinant.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/diagonal.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/diagonal.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/diagonal_matrix_variadic_ctor.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/diagonal_matrix_variadic_ctor.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/diagonalmatrices.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/diagonalmatrices.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/dontalign.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/dontalign.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/dynalloc.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/dynalloc.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/eigen2support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/eigen2support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/eigensolver_complex.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/eigensolver_complex.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/eigensolver_generalized_real.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/eigensolver_generalized_real.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/eigensolver_generic.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/eigensolver_generic.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/eigensolver_selfadjoint.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/eigensolver_selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/evaluators.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/evaluators.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/exceptions.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/exceptions.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/fastmath.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/fastmath.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/first_aligned.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/first_aligned.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_alignedbox.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_alignedbox.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_eulerangles.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_eulerangles.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_homogeneous.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_homogeneous.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_hyperplane.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_hyperplane.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_orthomethods.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_orthomethods.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_parametrizedline.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_parametrizedline.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_quaternion.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_quaternion.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/geo_transformations.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/geo_transformations.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/gpu_basic.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/gpu_basic.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/gpu_common.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/gpu_common.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/half_float.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/half_float.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/hessenberg.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/hessenberg.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/householder.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/householder.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/incomplete_cholesky.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/incomplete_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/indexed_view.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/indexed_view.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/initializer_list_construction.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/initializer_list_construction.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/inplace_decomposition.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/inplace_decomposition.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/integer_types.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/integer_types.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/inverse.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/inverse.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/io.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/io.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/is_same_dense.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/is_same_dense.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/jacobi.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/jacobi.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/jacobisvd.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/jacobisvd.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/klu_support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/klu_support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/linearstructure.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/linearstructure.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/lscg.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/lscg.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/lu.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/lu.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/main.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/main.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/mapped_matrix.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/mapped_matrix.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/mapstaticmethods.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/mapstaticmethods.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/mapstride.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/mapstride.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/meta.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/meta.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/metis_support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/metis_support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/miscmatrices.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/miscmatrices.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/mixingtypes.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/mixingtypes.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/mpl2only.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/mpl2only.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/nestbyvalue.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/nestbyvalue.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/nesting_ops.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/nesting_ops.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/nomalloc.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/nomalloc.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/nullary.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/nullary.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/num_dimensions.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/num_dimensions.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/numext.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/numext.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/packetmath.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/packetmath.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/packetmath_test_shared.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/packetmath_test_shared.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/pardiso_support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/pardiso_support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/pastix_support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/pastix_support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/permutationmatrices.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/permutationmatrices.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/prec_inverse_4x4.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/prec_inverse_4x4.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_extra.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_extra.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_large.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_large.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_mmtr.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_mmtr.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_notemporary.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_notemporary.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_selfadjoint.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_small.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_small.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_symm.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_symm.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_syrk.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_syrk.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_trmm.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_trmm.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_trmv.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_trmv.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/product_trsolve.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/product_trsolve.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/qr.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/qr.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/qr_colpivoting.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/qr_colpivoting.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/qr_fullpivoting.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/qr_fullpivoting.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/qtvector.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/qtvector.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/rand.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/rand.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/random_without_cast_overflow.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/random_without_cast_overflow.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/real_qz.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/real_qz.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/redux.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/redux.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/ref.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/ref.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/reshape.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/reshape.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/resize.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/resize.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/rvalue_types.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/rvalue_types.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/schur_complex.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/schur_complex.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/schur_real.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/schur_real.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/selfadjoint.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/simplicial_cholesky.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/simplicial_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sizeof.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sizeof.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sizeoverflow.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sizeoverflow.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/smallvectors.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/smallvectors.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/solverbase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/solverbase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparseLM.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparseLM.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_basic.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_basic.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_block.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_block.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_permutations.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_permutations.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_product.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_product.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_ref.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_ref.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_solver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_solver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_solvers.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_solvers.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparse_vector.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparse_vector.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparselu.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparselu.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/sparseqr.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/sparseqr.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/special_numbers.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/special_numbers.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/split_test_helper.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/split_test_helper.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/spqr_support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/spqr_support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/stable_norm.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/stable_norm.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/stddeque.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/stddeque.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/stddeque_overload.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/stddeque_overload.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/stdlist.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/stdlist.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/stdlist_overload.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/stdlist_overload.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/stdvector.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/stdvector.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/stdvector_overload.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/stdvector_overload.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/stl_iterators.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/stl_iterators.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/superlu_support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/superlu_support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/svd_common.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/svd_common.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/svd_fill.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/svd_fill.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/swap.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/swap.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/symbolic_index.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/symbolic_index.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/triangular.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/triangular.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/type_alias.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/type_alias.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/umeyama.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/umeyama.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/umfpack_support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/umfpack_support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/unalignedcount.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/unalignedcount.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/upperbidiagonalization.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/upperbidiagonalization.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/vectorization_logic.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/vectorization_logic.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/vectorwiseop.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/vectorwiseop.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/visitor.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/visitor.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/test/zerosized.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/test/zerosized.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/AdolcForward` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/AdolcForward`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/AlignedVector3` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/AlignedVector3`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/ArpackSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/ArpackSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/AutoDiff` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/AutoDiff`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/BVH` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/BVH`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/Tensor` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/Tensor`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/TensorSymmetry` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/TensorSymmetry`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/ThreadPool` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/ThreadPool`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/README.md` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/README.md`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/Tensor.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/Tensor.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Meta.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Meta.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/EmulateArray.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/EmulateArray.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/EulerAngles` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/EulerAngles`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/FFT` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/FFT`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/IterativeSolvers` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/IterativeSolvers`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/KroneckerProduct` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/KroneckerProduct`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/LevenbergMarquardt` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/LevenbergMarquardt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/MPRealSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/MPRealSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/MatrixFunctions` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/MatrixFunctions`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/MoreVectorization` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/MoreVectorization`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/NonLinearOptimization` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/NonLinearOptimization`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/NumericalDiff` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/NumericalDiff`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/OpenGLSupport` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/OpenGLSupport`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/Polynomials` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/Polynomials`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/Skyline` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/Skyline`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/SparseExtra` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/SparseExtra`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/SpecialFunctions` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/SpecialFunctions`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/Splines` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/Splines`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/BVAlgorithms.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/BVAlgorithms.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/KdBVH.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/BVH/KdBVH.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerAngles.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerSystem.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerSystem.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_fftw_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_fftw_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_kissfft_impl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_kissfft_impl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/DGMRES.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/DGMRES.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/GMRES.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/GMRES.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IDRS.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IDRS.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IterationController.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IterationController.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/MINRES.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/MINRES.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/Scaling.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/Scaling.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/StemFunction.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/StemFunction.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/MathFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/chkder.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/chkder.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/covar.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/covar.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/dogleg.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/dogleg.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/lmpar.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/lmpar.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1updt.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1updt.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/Companion.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/Companion.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialSolver.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialSolver.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialUtils.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialUtils.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineProduct.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineProduct.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineStorage.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineStorage.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineUtil.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineUtil.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MarketIO.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MarketIO.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/RandomSetter.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/RandomSetter.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/Spline.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/Spline.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFitting.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFitting.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFwd.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFwd.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/README.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/README.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/bench/bench_svd.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/bench/bench_svd.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/Overview.dox` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/Overview.dox`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/eigendoxy_layout.xml.in` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/eigendoxy_layout.xml.in`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/BVH_Example.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/BVH_Example.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/EulerAngles.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/EulerAngles.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/FFT.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/FFT.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixSinh.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/MatrixSinh.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/PolynomialSolver1.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/PolynomialSolver1.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/PolynomialUtils1.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/PolynomialUtils1.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/CwiseMul.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/examples/SYCL/CwiseMul.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/doc/snippets/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/doc/snippets/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/BVH.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/BVH.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/CMakeLists.txt` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/EulerAngles.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/EulerAngles.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/FFTW.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/FFTW.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/NonLinearOptimization.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/NonLinearOptimization.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/NumericalDiff.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/NumericalDiff.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/alignedvector3.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/alignedvector3.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/autodiff.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/autodiff.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/autodiff_scalar.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/autodiff_scalar.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/bessel_functions.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/bessel_functions.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_eventcount.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_eventcount.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_maxsizevector.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_maxsizevector.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_meta.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_meta.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_non_blocking_thread_pool.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_non_blocking_thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_runqueue.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_runqueue.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_assign.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_assign.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_access.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_access.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_eval.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_eval.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_io.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_block_io.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcast_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcast_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcasting.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcasting.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_builtins_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_builtins_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_cast_float16_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_cast_float16_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_casts.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_casts.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_comparisons.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_comparisons.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_const.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_const.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contraction.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_contraction.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_index.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_index.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_device.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_device.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_device_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_device_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_dimension.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_dimension.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_empty.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_empty.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_executor.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_executor.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_expr.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_expr.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_fft.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_fft.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_fixed_size.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_fixed_size.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_generator.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_generator.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_generator_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_generator_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_ifft.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_ifft.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_op_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_op_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_index_list.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_index_list.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_intdiv.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_intdiv.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_io.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_io.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_lvalue.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_lvalue.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_map.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_map.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_math.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_math.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_math_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_math_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_mixed_indices.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_mixed_indices.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_move.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_move.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_notification.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_notification.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_complex.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_complex.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_const_values.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_const_values.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_float16_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_float16_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_strings.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_of_strings.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_padding.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_padding.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_padding_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_padding_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_patch.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_patch.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_patch_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_patch_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_random_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_ref.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_ref.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_roundings.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_roundings.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_gpu.cu` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_gpu.cu`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_simple.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_simple.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_striding.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_striding.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_striding_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_striding_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_sugar.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_sugar.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_symmetry.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_symmetry.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_local.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_local.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_pool.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_trace.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_trace.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_uint128.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_uint128.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/dgmres.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/dgmres.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/forward_adolc.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/forward_adolc.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/gmres.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/gmres.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/idrs.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/idrs.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/kronecker_product.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/kronecker_product.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/levenberg_marquardt.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/levenberg_marquardt.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_exponential.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_exponential.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_function.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_function.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_functions.h` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_functions.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_power.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_power.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/matrix_square_root.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/matrix_square_root.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/minres.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/minres.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/mpreal_support.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/mpreal_support.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/openglsupport.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/openglsupport.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/polynomialsolver.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/polynomialsolver.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/polynomialutils.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/polynomialutils.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/sparse_extra.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/sparse_extra.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/special_functions.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/special_functions.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/special_packetmath.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/special_packetmath.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/eigen-3.4.0/unsupported/test/splines.cpp` & `aplr-6.5.1/dependencies/eigen-3.4.0/unsupported/test/splines.cpp`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/LICENSE.txt` & `aplr-6.5.1/dependencies/pybind11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/__main__.py` & `aplr-6.5.1/dependencies/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/commands.py` & `aplr-6.5.1/dependencies/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/attr.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/buffer_info.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/cast.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/chrono.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/complex.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/class.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/common.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/descr.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/init.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/internals.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/type_caster_base.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/detail/typeid.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/eigen/matrix.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/eigen/tensor.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/embed.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/eval.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/functional.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/gil.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/iostream.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/numpy.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/operators.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/options.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/pybind11.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/pytypes.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/stl/filesystem.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/stl.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/include/pybind11/stl_bind.h` & `aplr-6.5.1/dependencies/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/setup_helpers.py` & `aplr-6.5.1/dependencies/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/FindPythonLibsNew.cmake` & `aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11Common.cmake` & `aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11Config.cmake` & `aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11Config.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11ConfigVersion.cmake` & `aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11ConfigVersion.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11NewTools.cmake` & `aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11Targets.cmake` & `aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11Targets.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/dependencies/pybind11/share/cmake/pybind11/pybind11Tools.cmake` & `aplr-6.5.1/dependencies/pybind11/share/cmake/pybind11/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `aplr-6.5.0/setup.py` & `aplr-6.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     include_dirs=['cpp','dependencies/eigen-3.4.0','dependencies/pybind11/include'],
     language='c++',
     extra_compile_args=extra_compile_args,
     )
 
 setuptools.setup(
     name='aplr',
-    version='6.5.0',
+    version='6.5.1',
     description='Automatic Piecewise Linear Regression',
     ext_modules=[sfc_module],
     author="Mathias von Ottenbreit",
     author_email="ottenbreitdatascience@gmail.com",
     long_description="Build predictive and interpretable parametric regression or classification machine learning models in Python based on the Automatic Piecewise Linear Regression methodology developed by Mathias von Ottenbreit.",
     long_description_content_type="text/markdown",
     packages=['aplr'],
```

