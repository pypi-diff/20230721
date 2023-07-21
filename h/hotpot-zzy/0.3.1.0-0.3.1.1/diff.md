# Comparing `tmp/hotpot-zzy-0.3.1.0.tar.gz` & `tmp/hotpot-zzy-0.3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-udfycxsw/hotpot-zzy-0.3.1.0.tar", last modified: Fri Jul 21 09:06:27 2023, max compression
+gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-_ius_yh1/hotpot-zzy-0.3.1.1.tar", last modified: Fri Jul 21 11:27:49 2023, max compression
```

## Comparing `hotpot-zzy-0.3.1.0.tar` & `hotpot-zzy-0.3.1.1.tar`

### file list

```diff
@@ -1,154 +1,157 @@
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1070 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/LICENSE
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       59 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/MANIFEST.in
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      553 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8988 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/README.rst
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      437 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    40231 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/_io.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    27190 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   128862 2023-07-21 08:30:02.000000 hotpot-zzy-0.3.1.0/hotpot/cheminfo.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/data/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       65 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/atom_single_point.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1874 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/deepmd_script.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/data/force_field/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/data/force_field/UFF/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     4606 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/data/force_field/aMaterials/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1701 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/force_field/aMaterials/SiC.tersoff
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       82 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/force_field/contents.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      328 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/data/goptions.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/periodic_table.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.110679 hotpot-zzy-0.3.1.0/hotpot/data/solvents/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      946 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,1-trichloroethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1039 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      760 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,2-trichloroethene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-dichloroethene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2525 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-diethoxypropane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1410 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-dimethoxymethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      943 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dichloroethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dichloroethene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1688 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dimethoxyethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1518 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,4-dioxane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-butanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1865 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-pentanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1307 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-propanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2,2-dimethoxypropane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-butanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1684 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-ethoxyethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1406 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methoxyethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1595 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methyl-1-propanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1716 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/3-methyl-1-butanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      649 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/DCM.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1300 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/DMF.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1115 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/DMSO.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1597 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/N,N-dimethylacetamide.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1712 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/N-methylpyrrolidone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1417 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/THF.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      936 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1118 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      751 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetonitrile.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1328 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/benzene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2053 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/butylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      666 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/carbon_tetrachloride.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1334 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/chlorobenzene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      656 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/chloroform.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2164 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/cumene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/cyclohexane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1588 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/diethylether.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2243 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/diisopropylamine.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1025 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethyl_formate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1495 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethyleneglycol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      748 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/formamide.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      657 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/formic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2327 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/heptane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2047 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/hexane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2057 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isobutyl_acetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2608 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isooctane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1308 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1778 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2148 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropylether.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/meta-xylene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      747 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1707 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methoxybenzene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1965 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylbutylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2175 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylcyclohexane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1407 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylethylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylisobutylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1690 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylisopropylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1610 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/morpholine.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      844 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/nitromethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1891 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ortho-xylene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/para-xylene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1769 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/pentane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1775 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/propylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1236 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/pyridine.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1609 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/sulfolane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/t-butylmethylether.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2283 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/tetralin.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1607 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/toluene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/trichloroacetic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/trifluoroacetic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      465 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/water.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      182 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/units.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.110679 hotpot-zzy-0.3.1.0/hotpot/tanks/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      205 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    12075 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/cc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8913 2023-07-14 06:27:13.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/deepmd.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      149 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/features.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.110679 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      269 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     7862 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/base.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8553 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/gcmc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     9615 2023-07-14 06:27:13.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/materials.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.110679 hotpot-zzy-0.3.1.0/hotpot/tanks/qm/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      128 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/qm/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    22275 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/qm/gaussian.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    33955 2023-07-21 07:55:46.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/quantum.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2838 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tmo.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2805 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tools.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.114679 hotpot-zzy-0.3.1.0/hotpot/utils/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/utils/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     3979 2023-07-03 10:51:41.000000 hotpot-zzy-0.3.1.0/hotpot/utils/library.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1462 2023-07-14 06:27:13.000000 hotpot-zzy-0.3.1.0/hotpot/utils/manage_machine.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      478 2023-07-21 07:51:57.000000 hotpot-zzy-0.3.1.0/hotpot/utils/ob2netwx.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      642 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.114679 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      553 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     4648 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       44 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/top_level.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      885 2023-07-21 09:05:56.000000 hotpot-zzy-0.3.1.0/pyproject.toml
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/setup.cfg
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.114679 hotpot-zzy-0.3.1.0/test/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.098680 hotpot-zzy-0.3.1.0/test/examples/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.114679 hotpot-zzy-0.3.1.0/test/examples/struct/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   363848 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/0.log
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      843 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/Cs-VOHSAM-5.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      228 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/Li-ZADQAA-8-L.gjf
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    51433 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/aCarbon.xyz
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   973096 2023-07-18 02:31:26.000000 hotpot-zzy-0.3.1.0/test/examples/struct/abnormal_output.log
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    14953 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/cage.cif
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    12564 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/mol.mol2
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.098680 hotpot-zzy-0.3.1.0/test/output/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/test/output/gaussrun/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 03:26:46.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2547573.d2e
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 03:26:46.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2547573.int
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   524288 2023-07-20 03:29:53.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2547573.skr
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 04:22:47.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2599402.d2e
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 04:22:47.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2599402.int
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   524288 2023-07-20 04:31:40.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2599402.skr
--rw-rw-r--   0 zz1       (1005) zz1       (1008)  4124672 2023-07-20 06:26:05.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/checkpoint.chk
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      701 2023-07-20 05:59:22.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/input.gjf
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   706878 2023-07-20 06:26:05.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/output.log
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/test/output/mol_write/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     6740 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/output/mol_write/mol.gjf
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    13403 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/output/mol_write/mol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      617 2023-07-18 02:44:49.000000 hotpot-zzy-0.3.1.0/test/test_cheminfo.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      503 2023-07-19 13:02:24.000000 hotpot-zzy-0.3.1.0/test/test_gaussian.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      782 2023-07-20 03:26:42.000000 hotpot-zzy-0.3.1.0/test/test_quantum.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.569331 hotpot-zzy-0.3.1.1/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1070 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/LICENSE
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       59 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/MANIFEST.in
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8841 2023-07-21 11:27:49.565331 hotpot-zzy-0.3.1.1/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8384 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/README.md
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8988 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/README.rst
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.525332 hotpot-zzy-0.3.1.1/hotpot/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      437 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/hotpot/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    40231 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/hotpot/_io.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    27190 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/hotpot/bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   128862 2023-07-21 08:30:02.000000 hotpot-zzy-0.3.1.1/hotpot/cheminfo.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.529332 hotpot-zzy-0.3.1.1/hotpot/data/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       65 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/atom_single_point.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1874 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/deepmd_script.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.529332 hotpot-zzy-0.3.1.1/hotpot/data/force_field/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.529332 hotpot-zzy-0.3.1.1/hotpot/data/force_field/UFF/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4606 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.529332 hotpot-zzy-0.3.1.1/hotpot/data/force_field/aMaterials/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1701 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       82 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/force_field/contents.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      328 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/hotpot/data/goptions.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/periodic_table.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.537331 hotpot-zzy-0.3.1.1/hotpot/data/solvents/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      946 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1,1-trichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1039 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      760 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1,2-trichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2525 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1-diethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1410 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1-dimethoxymethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      943 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,2-dichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,2-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1688 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,2-dimethoxyethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1518 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,4-dioxane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1865 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1-pentanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1307 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/2,2-dimethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1684 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-ethoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1406 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-methoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1595 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-methyl-1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1716 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/3-methyl-1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      649 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/DCM.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1300 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/DMF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1115 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/DMSO.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1597 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/N,N-dimethylacetamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1712 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/N-methylpyrrolidone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1417 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/THF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      936 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/acetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1118 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/acetone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      751 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/acetonitrile.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1328 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/benzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2053 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/butylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      666 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/carbon_tetrachloride.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1334 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/chlorobenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      656 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/chloroform.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2164 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/cumene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/cyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1588 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/diethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2243 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/diisopropylamine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1025 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/ethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/ethyl_formate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1495 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/ethylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/ethyleneglycol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      748 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/formamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      657 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/formic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2327 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/heptane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2047 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/hexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2057 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/isobutyl_acetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2608 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/isooctane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1308 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/isopropanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1778 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/isopropylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2148 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/isopropylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/meta-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      747 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/methanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1707 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/methoxybenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1965 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylbutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2175 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylcyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1407 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylethylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylisobutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1690 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylisopropylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1610 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/morpholine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      844 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/nitromethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1891 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/ortho-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/para-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1769 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/pentane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1775 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/propylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1236 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/pyridine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1609 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/sulfolane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/t-butylmethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2283 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/tetralin.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1607 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/toluene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/trichloroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/trifluoroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      465 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/solvents/water.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      182 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/data/units.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.537331 hotpot-zzy-0.3.1.1/hotpot/tanks/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      205 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    12075 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/cc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8913 2023-07-14 06:27:13.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/deepmd.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      149 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/features.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.537331 hotpot-zzy-0.3.1.1/hotpot/tanks/lmp/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      269 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/lmp/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7862 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/lmp/base.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8553 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/lmp/gcmc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     9615 2023-07-14 06:27:13.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/lmp/materials.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.537331 hotpot-zzy-0.3.1.1/hotpot/tanks/qm/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      128 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/qm/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    22275 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/qm/gaussian.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    33955 2023-07-21 07:55:46.000000 hotpot-zzy-0.3.1.1/hotpot/tanks/quantum.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2838 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/tmo.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2805 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/tools.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.541331 hotpot-zzy-0.3.1.1/hotpot/utils/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/utils/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     3979 2023-07-03 10:51:41.000000 hotpot-zzy-0.3.1.1/hotpot/utils/library.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1462 2023-07-14 06:27:13.000000 hotpot-zzy-0.3.1.1/hotpot/utils/manage_machine.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      478 2023-07-21 07:51:57.000000 hotpot-zzy-0.3.1.1/hotpot/utils/ob2netwx.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      642 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.541331 hotpot-zzy-0.3.1.1/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8841 2023-07-21 11:27:49.000000 hotpot-zzy-0.3.1.1/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4684 2023-07-21 11:27:49.000000 hotpot-zzy-0.3.1.1/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-07-21 11:27:49.000000 hotpot-zzy-0.3.1.1/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       44 2023-07-21 11:27:49.000000 hotpot-zzy-0.3.1.1/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       12 2023-07-21 11:27:49.000000 hotpot-zzy-0.3.1.1/hotpot_zzy.egg-info/top_level.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      884 2023-07-21 11:27:05.000000 hotpot-zzy-0.3.1.1/pyproject.toml
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-07-21 11:27:49.569331 hotpot-zzy-0.3.1.1/setup.cfg
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1061 2023-07-21 11:26:21.000000 hotpot-zzy-0.3.1.1/setup.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.541331 hotpot-zzy-0.3.1.1/test/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      129 2023-07-17 02:23:08.000000 hotpot-zzy-0.3.1.1/test/__init__.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.521332 hotpot-zzy-0.3.1.1/test/examples/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.545331 hotpot-zzy-0.3.1.1/test/examples/struct/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   363848 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/test/examples/struct/0.log
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      843 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/test/examples/struct/Cs-VOHSAM-5.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      228 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/test/examples/struct/Li-ZADQAA-8-L.gjf
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    51433 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/test/examples/struct/aCarbon.xyz
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   973096 2023-07-18 02:31:26.000000 hotpot-zzy-0.3.1.1/test/examples/struct/abnormal_output.log
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    14953 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/test/examples/struct/cage.cif
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    12564 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/test/examples/struct/mol.mol2
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.521332 hotpot-zzy-0.3.1.1/test/output/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.565331 hotpot-zzy-0.3.1.1/test/output/gaussrun/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 03:26:46.000000 hotpot-zzy-0.3.1.1/test/output/gaussrun/Gau-2547573.d2e
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 03:26:46.000000 hotpot-zzy-0.3.1.1/test/output/gaussrun/Gau-2547573.int
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   524288 2023-07-20 03:29:53.000000 hotpot-zzy-0.3.1.1/test/output/gaussrun/Gau-2547573.skr
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 04:22:47.000000 hotpot-zzy-0.3.1.1/test/output/gaussrun/Gau-2599402.d2e
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 04:22:47.000000 hotpot-zzy-0.3.1.1/test/output/gaussrun/Gau-2599402.int
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   524288 2023-07-20 04:31:40.000000 hotpot-zzy-0.3.1.1/test/output/gaussrun/Gau-2599402.skr
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)  4124672 2023-07-20 06:26:05.000000 hotpot-zzy-0.3.1.1/test/output/gaussrun/checkpoint.chk
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      701 2023-07-20 05:59:22.000000 hotpot-zzy-0.3.1.1/test/output/gaussrun/input.gjf
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   706878 2023-07-20 06:26:05.000000 hotpot-zzy-0.3.1.1/test/output/gaussrun/output.log
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 11:27:49.565331 hotpot-zzy-0.3.1.1/test/output/mol_write/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     6740 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/test/output/mol_write/mol.gjf
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    13403 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.1/test/output/mol_write/mol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      617 2023-07-18 02:44:49.000000 hotpot-zzy-0.3.1.1/test/test_cheminfo.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      503 2023-07-19 13:02:24.000000 hotpot-zzy-0.3.1.1/test/test_gaussian.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      782 2023-07-20 03:26:42.000000 hotpot-zzy-0.3.1.1/test/test_quantum.py
```

### Comparing `hotpot-zzy-0.3.1.0/LICENSE` & `hotpot-zzy-0.3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/README.rst` & `hotpot-zzy-0.3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/_io.py` & `hotpot-zzy-0.3.1.1/hotpot/_io.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/bundle.py` & `hotpot-zzy-0.3.1.1/hotpot/bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/cheminfo.py` & `hotpot-zzy-0.3.1.1/hotpot/cheminfo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/deepmd_script.json` & `hotpot-zzy-0.3.1.1/hotpot/data/deepmd_script.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.3.1.1/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.3.1.1/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/periodic_table.json` & `hotpot-zzy-0.3.1.1/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,1-trichloroethane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1,1-trichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,1-trifluroethanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1,1-trifluroethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,2-trichloroethene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1,2-trichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-dichloroethene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-diethoxypropane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1-diethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-dimethoxymethane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,1-dimethoxymethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dichloroethane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,2-dichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dichloroethene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,2-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dimethoxyethane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,2-dimethoxyethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,4-dioxane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1,4-dioxane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-butanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-pentanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1-pentanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-propanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2,2-dimethoxypropane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/2,2-dimethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-butanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-ethoxyethanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-ethoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methoxyethanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-methoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methyl-1-propanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-methyl-1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methyltetrahydrofuran.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/2-methyltetrahydrofuran.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/3-methyl-1-butanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/3-methyl-1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/DCM.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/DCM.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/DMF.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/DMF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/DMSO.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/DMSO.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/N,N-dimethylacetamide.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/N,N-dimethylacetamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/N-methylpyrrolidone.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/N-methylpyrrolidone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/THF.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/THF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetic_acid.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/acetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetone.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/acetone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetonitrile.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/acetonitrile.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/benzene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/benzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/butylacetate.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/butylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/carbon_tetrachloride.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/carbon_tetrachloride.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/chlorobenzene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/chlorobenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/chloroform.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/chloroform.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/cumene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/cumene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/cyclohexane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/cyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/diethylether.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/diethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/diisopropylamine.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/diisopropylamine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/ethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethyl_formate.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/ethyl_formate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethylacetate.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/ethylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethyleneglycol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/ethyleneglycol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/formamide.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/formamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/formic_acid.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/formic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/heptane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/heptane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/hexane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/hexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isobutyl_acetate.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/isobutyl_acetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isooctane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/isooctane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/isopropanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropylacetate.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/isopropylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropylether.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/isopropylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/meta-xylene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/meta-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methanol.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/methanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methoxybenzene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/methoxybenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylacetate.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylbutylketone.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylbutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylcyclohexane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylcyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylethylketone.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylethylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylisobutylketone.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylisobutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylisopropylketone.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/methylisopropylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/morpholine.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/morpholine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/nitromethane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/nitromethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ortho-xylene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/ortho-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/para-xylene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/para-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/pentane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/pentane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/propylacetate.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/propylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/pyridine.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/pyridine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/sulfolane.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/sulfolane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/t-butylmethylether.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/t-butylmethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/tetralin.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/tetralin.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/toluene.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/toluene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/trichloroacetic_acid.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/trichloroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/data/solvents/trifluoroacetic_acid.mol2` & `hotpot-zzy-0.3.1.1/hotpot/data/solvents/trifluoroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/tanks/cc.py` & `hotpot-zzy-0.3.1.1/hotpot/tanks/cc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/tanks/deepmd.py` & `hotpot-zzy-0.3.1.1/hotpot/tanks/deepmd.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.3.1.1/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.3.1.1/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.3.1.1/hotpot/tanks/lmp/materials.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/tanks/qm/gaussian.py` & `hotpot-zzy-0.3.1.1/hotpot/tanks/qm/gaussian.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/tanks/quantum.py` & `hotpot-zzy-0.3.1.1/hotpot/tanks/quantum.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/tmo.py` & `hotpot-zzy-0.3.1.1/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/tools.py` & `hotpot-zzy-0.3.1.1/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/utils/library.py` & `hotpot-zzy-0.3.1.1/hotpot/utils/library.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/utils/manage_machine.py` & `hotpot-zzy-0.3.1.1/hotpot/utils/manage_machine.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot/utils/units_convert.py` & `hotpot-zzy-0.3.1.1/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/SOURCES.txt` & `hotpot-zzy-0.3.1.1/hotpot_zzy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
 MANIFEST.in
+README.md
 README.rst
 pyproject.toml
+setup.py
 hotpot/__init__.py
 hotpot/_io.py
 hotpot/bundle.py
 hotpot/cheminfo.py
 hotpot/tmo.py
 hotpot/tools.py
 hotpot/data/atom_single_point.json
@@ -107,14 +109,15 @@
 hotpot/utils/ob2netwx.py
 hotpot/utils/units_convert.py
 hotpot_zzy.egg-info/PKG-INFO
 hotpot_zzy.egg-info/SOURCES.txt
 hotpot_zzy.egg-info/dependency_links.txt
 hotpot_zzy.egg-info/requires.txt
 hotpot_zzy.egg-info/top_level.txt
+test/__init__.py
 test/test_cheminfo.py
 test/test_gaussian.py
 test/test_quantum.py
 test/examples/struct/0.log
 test/examples/struct/Cs-VOHSAM-5.mol2
 test/examples/struct/Li-ZADQAA-8-L.gjf
 test/examples/struct/aCarbon.xyz
```

### Comparing `hotpot-zzy-0.3.1.0/pyproject.toml` & `hotpot-zzy-0.3.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hotpot-zzy"
-version = "0.3.1.0"
-readme = "RAEDME.rst"
+version = "0.3.1.1"
+readme = "README.md"
 authors = [
     { name = "Zhiyuan Zhang", email = "ZhiyuanZhang_scu@163.com" },
     { name = "Yue Dong", email = "1320801310@qq.com" },
     { name = "Yuqing Qiu", email = "2022223070045@stu.scu.edu.cn" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `hotpot-zzy-0.3.1.0/test/examples/struct/0.log` & `hotpot-zzy-0.3.1.1/test/examples/struct/0.log`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/examples/struct/Cs-VOHSAM-5.mol2` & `hotpot-zzy-0.3.1.1/test/examples/struct/Cs-VOHSAM-5.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/examples/struct/aCarbon.xyz` & `hotpot-zzy-0.3.1.1/test/examples/struct/aCarbon.xyz`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/examples/struct/abnormal_output.log` & `hotpot-zzy-0.3.1.1/test/examples/struct/abnormal_output.log`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/examples/struct/cage.cif` & `hotpot-zzy-0.3.1.1/test/examples/struct/cage.cif`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/examples/struct/mol.mol2` & `hotpot-zzy-0.3.1.1/test/examples/struct/mol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/output/gaussrun/checkpoint.chk` & `hotpot-zzy-0.3.1.1/test/output/gaussrun/checkpoint.chk`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/output/gaussrun/input.gjf` & `hotpot-zzy-0.3.1.1/test/output/gaussrun/input.gjf`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/output/gaussrun/output.log` & `hotpot-zzy-0.3.1.1/test/output/gaussrun/output.log`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/output/mol_write/mol.gjf` & `hotpot-zzy-0.3.1.1/test/output/mol_write/mol.gjf`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/output/mol_write/mol.mol2` & `hotpot-zzy-0.3.1.1/test/output/mol_write/mol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/test_cheminfo.py` & `hotpot-zzy-0.3.1.1/test/test_cheminfo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.1.0/test/test_quantum.py` & `hotpot-zzy-0.3.1.1/test/test_quantum.py`

 * *Files identical despite different names*

