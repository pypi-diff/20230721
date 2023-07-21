# Comparing `tmp/hotpot-zzy-0.3.0.9.tar.gz` & `tmp/hotpot-zzy-0.3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotpot-zzy-0.3.0.9.tar", last modified: Fri Jul  7 05:50:26 2023, max compression
+gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-udfycxsw/hotpot-zzy-0.3.1.0.tar", last modified: Fri Jul 21 09:06:27 2023, max compression
```

## Comparing `hotpot-zzy-0.3.0.9.tar` & `hotpot-zzy-0.3.1.0.tar`

### file list

```diff
@@ -1,127 +1,154 @@
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.309484 hotpot-zzy-0.3.0.9/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1070 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/LICENSE
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)       17 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/MANIFEST.in
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      449 2023-07-07 05:50:26.308484 hotpot-zzy-0.3.0.9/PKG-INFO
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     6643 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/README.md
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.095516 hotpot-zzy-0.3.0.9/hotpot/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      419 2023-07-07 05:38:01.000000 hotpot-zzy-0.3.0.9/hotpot/__init__.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)    36575 2023-07-04 06:09:00.000000 hotpot-zzy-0.3.0.9/hotpot/_io.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)    25800 2023-07-04 07:52:05.000000 hotpot-zzy-0.3.0.9/hotpot/bundle.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)   112109 2023-07-06 06:16:21.000000 hotpot-zzy-0.3.0.9/hotpot/cheminfo.py
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.146257 hotpot-zzy-0.3.0.9/hotpot/data/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)       65 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/atom_single_point.json
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1874 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/deepmd_script.json
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.160364 hotpot-zzy-0.3.0.9/hotpot/data/force_field/
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.177362 hotpot-zzy-0.3.0.9/hotpot/data/force_field/UFF/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     4606 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/force_field/UFF/LJ.json
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.195362 hotpot-zzy-0.3.0.9/hotpot/data/force_field/aMaterials/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1701 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/force_field/aMaterials/SiC.tersoff
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)       82 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/force_field/contents.json
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)   231681 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/periodic_table.json
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.097163 hotpot-zzy-0.3.0.9/hotpot/data/solvents/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      946 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,1-trichloroethane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1039 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      760 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,2-trichloroethene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-dichloroethene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2525 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-diethoxypropane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1410 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-dimethoxymethane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      943 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dichloroethane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dichloroethene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1688 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dimethoxyethane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1518 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,4-dioxane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-butanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1865 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-pentanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1307 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-propanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2,2-dimethoxypropane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-butanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1684 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-ethoxyethanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1406 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methoxyethanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1595 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methyl-1-propanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1716 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/3-methyl-1-butanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      649 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/DCM.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1300 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/DMF.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1115 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/DMSO.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1597 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/N,N-dimethylacetamide.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1712 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/N-methylpyrrolidone.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1417 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/THF.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      936 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetic_acid.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1118 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetone.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      751 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetonitrile.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1328 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/benzene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2053 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/butylacetate.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      666 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/carbon_tetrachloride.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1334 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/chlorobenzene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      656 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/chloroform.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2164 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/cumene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/cyclohexane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1588 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/diethylether.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2243 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/diisopropylamine.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1025 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethyl_formate.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1495 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethylacetate.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethyleneglycol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      748 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/formamide.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      657 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/formic_acid.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2327 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/heptane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2047 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/hexane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2057 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isobutyl_acetate.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2608 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isooctane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1308 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1778 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropylacetate.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2148 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropylether.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/meta-xylene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      747 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methanol.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1707 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methoxybenzene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylacetate.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1965 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylbutylketone.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2175 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylcyclohexane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1407 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylethylketone.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylisobutylketone.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1690 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylisopropylketone.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1610 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/morpholine.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      844 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/nitromethane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1891 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ortho-xylene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/para-xylene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1769 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/pentane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1775 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/propylacetate.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1236 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/pyridine.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1609 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/sulfolane.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/t-butylmethylether.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2283 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/tetralin.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1607 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/toluene.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/trichloroacetic_acid.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/trifluoroacetic_acid.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      465 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/water.mol2
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      182 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/units.json
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.145492 hotpot-zzy-0.3.0.9/hotpot/tanks/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      205 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/__init__.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)    10283 2023-07-06 05:53:15.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/cc.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     8140 2023-07-06 01:38:16.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/deepmd.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      149 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/features.py
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.193897 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      269 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/__init__.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     7862 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/base.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     8553 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/gcmc.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     9158 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/materials.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)    16656 2023-07-06 09:21:59.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/quantum.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2838 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tmo.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2805 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tools.py
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.232231 hotpot-zzy-0.3.0.9/hotpot/utils/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/utils/__init__.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     3979 2023-07-03 10:51:41.000000 hotpot-zzy-0.3.0.9/hotpot/utils/library.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1403 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/utils/manage_machine.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      642 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/utils/units_convert.py
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.269851 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      449 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/PKG-INFO
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     3941 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/SOURCES.txt
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)        1 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/dependency_links.txt
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)       44 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/requires.txt
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)        7 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/top_level.txt
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      731 2023-07-07 05:38:01.000000 hotpot-zzy-0.3.0.9/pyproject.toml
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)       38 2023-07-07 05:50:26.309484 hotpot-zzy-0.3.0.9/setup.cfg
-drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.299484 hotpot-zzy-0.3.0.9/test/
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)      533 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/test/test_amorphous_maker.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1812 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/test/test_bundle.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     3095 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/test/test_chemif.py
--rwxrwxrwx   0 zzy       (1000) zzy       (1000)     6853 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/test/test_lmp.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1070 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/LICENSE
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       59 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/MANIFEST.in
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      553 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8988 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/README.rst
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      437 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    40231 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/_io.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    27190 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   128862 2023-07-21 08:30:02.000000 hotpot-zzy-0.3.1.0/hotpot/cheminfo.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/data/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       65 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/atom_single_point.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1874 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/deepmd_script.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/data/force_field/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/data/force_field/UFF/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4606 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.102680 hotpot-zzy-0.3.1.0/hotpot/data/force_field/aMaterials/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1701 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       82 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/force_field/contents.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      328 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/data/goptions.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/periodic_table.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.110679 hotpot-zzy-0.3.1.0/hotpot/data/solvents/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      946 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,1-trichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1039 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      760 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,2-trichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2525 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-diethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1410 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-dimethoxymethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      943 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1688 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dimethoxyethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1518 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,4-dioxane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1865 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-pentanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1307 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2,2-dimethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1684 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-ethoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1406 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1595 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methyl-1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1716 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/3-methyl-1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      649 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/DCM.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1300 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/DMF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1115 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/DMSO.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1597 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/N,N-dimethylacetamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1712 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/N-methylpyrrolidone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1417 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/THF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      936 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1118 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      751 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetonitrile.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1328 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/benzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2053 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/butylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      666 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/carbon_tetrachloride.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1334 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/chlorobenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      656 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/chloroform.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2164 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/cumene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/cyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1588 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/diethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2243 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/diisopropylamine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1025 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethyl_formate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1495 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethyleneglycol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      748 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/formamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      657 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/formic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2327 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/heptane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2047 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/hexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2057 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isobutyl_acetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2608 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isooctane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1308 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1778 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2148 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/meta-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      747 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1707 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methoxybenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1965 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylbutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2175 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylcyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1407 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylethylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylisobutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1690 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylisopropylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1610 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/morpholine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      844 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/nitromethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1891 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/ortho-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/para-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1769 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/pentane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1775 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/propylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1236 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/pyridine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1609 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/sulfolane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/t-butylmethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2283 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/tetralin.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1607 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/toluene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/trichloroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/trifluoroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      465 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/solvents/water.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      182 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/data/units.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.110679 hotpot-zzy-0.3.1.0/hotpot/tanks/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      205 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    12075 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/cc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8913 2023-07-14 06:27:13.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/deepmd.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      149 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/features.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.110679 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      269 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7862 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/base.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8553 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/gcmc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     9615 2023-07-14 06:27:13.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/materials.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.110679 hotpot-zzy-0.3.1.0/hotpot/tanks/qm/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      128 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/qm/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    22275 2023-07-21 07:51:58.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/qm/gaussian.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    33955 2023-07-21 07:55:46.000000 hotpot-zzy-0.3.1.0/hotpot/tanks/quantum.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2838 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tmo.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2805 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/tools.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.114679 hotpot-zzy-0.3.1.0/hotpot/utils/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/utils/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     3979 2023-07-03 10:51:41.000000 hotpot-zzy-0.3.1.0/hotpot/utils/library.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1462 2023-07-14 06:27:13.000000 hotpot-zzy-0.3.1.0/hotpot/utils/manage_machine.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      478 2023-07-21 07:51:57.000000 hotpot-zzy-0.3.1.0/hotpot/utils/ob2netwx.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      642 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.114679 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      553 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4648 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       44 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-07-21 09:06:27.000000 hotpot-zzy-0.3.1.0/hotpot_zzy.egg-info/top_level.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      885 2023-07-21 09:05:56.000000 hotpot-zzy-0.3.1.0/pyproject.toml
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/setup.cfg
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.114679 hotpot-zzy-0.3.1.0/test/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.098680 hotpot-zzy-0.3.1.0/test/examples/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.114679 hotpot-zzy-0.3.1.0/test/examples/struct/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   363848 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/0.log
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      843 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/Cs-VOHSAM-5.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      228 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/Li-ZADQAA-8-L.gjf
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    51433 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/aCarbon.xyz
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   973096 2023-07-18 02:31:26.000000 hotpot-zzy-0.3.1.0/test/examples/struct/abnormal_output.log
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    14953 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/cage.cif
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    12564 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/examples/struct/mol.mol2
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.098680 hotpot-zzy-0.3.1.0/test/output/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/test/output/gaussrun/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 03:26:46.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2547573.d2e
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 03:26:46.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2547573.int
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   524288 2023-07-20 03:29:53.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2547573.skr
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 04:22:47.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2599402.d2e
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        0 2023-07-20 04:22:47.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2599402.int
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   524288 2023-07-20 04:31:40.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/Gau-2599402.skr
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)  4124672 2023-07-20 06:26:05.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/checkpoint.chk
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      701 2023-07-20 05:59:22.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/input.gjf
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   706878 2023-07-20 06:26:05.000000 hotpot-zzy-0.3.1.0/test/output/gaussrun/output.log
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-21 09:06:27.122679 hotpot-zzy-0.3.1.0/test/output/mol_write/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     6740 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/output/mol_write/mol.gjf
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    13403 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.1.0/test/output/mol_write/mol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      617 2023-07-18 02:44:49.000000 hotpot-zzy-0.3.1.0/test/test_cheminfo.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      503 2023-07-19 13:02:24.000000 hotpot-zzy-0.3.1.0/test/test_gaussian.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      782 2023-07-20 03:26:42.000000 hotpot-zzy-0.3.1.0/test/test_quantum.py
```

### Comparing `hotpot-zzy-0.3.0.9/LICENSE` & `hotpot-zzy-0.3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/_io.py` & `hotpot-zzy-0.3.1.0/hotpot/_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,979 +1,1046 @@
-"""
-python v3.7.9
-@Project: hotpot
-@File   : _io.py
-@Author : Zhiyuan Zhang
-@Date   : 2023/3/14
-@Time   : 4:18
-"""
-import os
-import re
-from pathlib import Path
-from os import PathLike
-from typing import *
-from abc import ABCMeta, abstractmethod
-from copy import copy
-import io
-from io import IOBase
-from openbabel import pybel
-import cclib
-import numpy as np
-
-import hotpot.cheminfo as ci
-from hotpot.tanks.deepmd import DeepSystem
-
-"""
-Notes:
-This module contain Classes to IO between the Molecule object and various file formats.
-the main classes are:
-    - Reader: from Formatted files to Molecule, called by the Molecule.read() method.
-    - Writer: from Molecule to formatted files, called by the Molecule.write() method.
-    - Dumper: from Molecule to formatted Literals(str or bytes), called by the Molecule.dump() method.
-    - Parser: from formatted Literals to the Molecule obj, called by the Molecule.parse() method.
-all of them are inherit from the _IOBase class.
-
-For the implementation of dump and parse:
-    - some third-part package are used, like openbabel, cclib and so on.
-    - there are some self own IO function be defined too.
-    - the user also custom and register to the Dumper and Parser too.
-
-When implementing the IO: 
-    1) the IO class will firstly check whether a custom IO function is defined and register, if the IO function 
-        are defined and registered, the IO are implemented by the registered.
-    2) else, the IO class will try to call, in turn, try to call some third-part packages,
-    3) finally, if all third-part packages fail to complement IO, Raise the IOError !!!
-
-Following the steps to customise your IO function:
-    1) determine which IO operation(read, write, dump or parse) you want to define， import the relevant IO class
-        into your own python modules.
-    2) define the IO function which customises your IO implementation, the custom function should meet the base
-        requirements demand by the corresponding IO class. When the IO functions are defined, applying the
-        `IOClass`.register decorator to register the IO function into the `IOClass`, the `IOClass`.register should
-        pass some args. This is a example:
-        --------------------------------- Example ------------------------------------
-        Examples:
-        # importing the relevant IO classes
-        from hotpot.io import Dumper, Reader
-        
-        # define and register a read function
-        # the fmt defined the format key to handle the custom IO function
-        # the types defined where the IO function will be applied, pre: preprocess, io: main io, post: postprocess
-        @Reader.register(fmt='the/format/key', types='pre|io|post')
-        def my_read_func(*arg, **kwargs)  # the args should meet the Reader demand
-            ...
-            
-        # define and register a dump function
-        def my_dump_func(*arg, **kwargs) # the args should meet the Dumper demand
-            ...
-        ---------------------------------- END ---------------------------------------
-"""
-
-
-# Define custom Exceptions
-class IOEarlyStop(BaseException):
-    """ monitor the situation that the IO should early stop and return None and the IO result """
-
-
-# Define the IO function types
-IOFuncPrefix = Literal['pre', 'io', 'post']
-IOStream = Union[IOBase, str, bytes]
-
-
-def _parse_lmp_data_script(script: str):
-    """ Parse the LAMMPS data script to two dict, header and body"""
-    # Define_body_title
-    bt_name = (
-        # atom-property sections
-        'Atoms', 'Velocities', 'Masses', 'Ellipsoids', 'Lines', 'Triangles', 'Bodies',
-        # molecular topology sections
-        'Bonds', 'Angles', 'Dihedrals', 'Impropers',
-        # force field sections
-        'Pair Coeffs', 'PairIJ Coeffs', 'Bond Coeffs', 'Angle Coeffs', 'Dihedral Coeffs', 'Improper Coeffs',
-        # class 2 force field sections
-        'BondBond Coeffs', 'BondAngle Coeffs', 'MiddleBondTorsion Coeffs', 'EndBondTorsion Coeffs',
-        'AngleTorsion Coeffs', 'AngleAngleTorsion Coeffs', 'BondBond13 Coeffs', 'AngleAngle Coeffs'
-    )
-
-    # Compile the body and header pattern
-    header_title = re.compile(r'[a-z]+')
-    header_int = re.compile(r'[0-9]+')
-    header_float = re.compile(r'-?[0-9]+\.[0-9]*')
-
-    lines = script.split('\n')
-    body_split_point = [i for i, lin in enumerate(lines) if lin in bt_name] + [len(lines)]
-
-    # Extract header info
-    headers = {}
-    for line in lines[1:body_split_point[0]]:
-        line = line.strip()
-        if line:
-            ht = ' '.join(header_title.findall(line))
-            hvs = line[:line.find(ht)].strip()  # header values
-            header_values = []
-            for hv in re.split(r'\s+', hvs):
-                if header_int.fullmatch(hv):
-                    header_values.append(int(hv))
-                elif header_float.fullmatch(hv):
-                    header_values.append(float(hv))
-                else:
-                    raise ValueError('the header line not match well')
-
-            headers[ht] = header_values
-
-    # Extract bodies info
-    bodies = {}
-    for sl_idx, el_idx in zip(body_split_point[:-1], body_split_point[1:]):
-        bt = lines[sl_idx].strip()  # body title
-        bc = [line.strip() for line in lines[sl_idx+1: el_idx] if line.strip()]  # body content
-        bodies[bt] = bc
-
-    return lines[0], headers, bodies
-
-
-class Register:
-    """
-    Register the IO function for Dumper, Parser or so on
-    """
-    def __init__(self):
-        # these dicts are container to store the custom io functions
-        # the keys of the dict are serve as the handle to get the mapped io functions(the values)
-        self.pre_methods = {}
-        self.io_methods = {}
-        self.post_methods = {}
-
-    def __repr__(self):
-        return f"Register:\n" + \
-               f"pre_method:\n" + \
-               f"\n\t".join([n for n in self.pre_methods]) + "\n\n" + \
-               f"io methods:\n" + \
-               f"\n\t".join([n for n in self.io_methods]) + '\n\n' + \
-               f"post methods:\n" + \
-               f"\n\t".join([n for n in self.post_methods])
-
-    def __call__(self, io_cls: type, fmt: str, prefix: IOFuncPrefix):
-        """
-        To register any function as a dumper or a postprocess to convert mol to formats
-        Args:
-            fmt:
-            prefix:
-
-        Returns:
-
-        """
-
-        def decorator(func: Callable):
-
-            if prefix == 'pre':
-                self.pre_methods[fmt] = func
-            elif prefix == 'io':
-                self.io_methods[fmt] = func
-            elif prefix == 'post':
-                self.post_methods[fmt] = func
-            else:
-                raise TypeError('the type of register is not supported')
-
-            return func
-
-        return decorator
-
-    def pre(self, fmt: str):
-        return self.pre_methods.get(fmt)
-
-    def io(self, fmt: str):
-        return self.io_methods.get(fmt)
-
-    def post(self, fmt: str):
-        return self.post_methods.get(fmt)
-
-
-# Retrieve the IO class by its format name
-def retrieve_format(fmt: str = None):
-    return _MoleculeIO.registered_format().get(fmt)
-
-
-# Get all registered format name
-def registered_format_name():
-    return tuple(_MoleculeIO.registered_format().keys())
-
-
-# TODO: deprecated in the later version
-class _MoleculeIO(ABCMeta):
-    """    Metaclass for registration of IO class format """
-    _registered_format = {}
-
-    def __new__(mcs, name, bases, namespace, **kwargs):
-        # Get the format keywords
-        fmt = namespace.get('format')(mcs)
-
-        if not fmt:
-            return super(_MoleculeIO, mcs).__new__(mcs, name, bases, namespace, **kwargs)
-        elif not isinstance(fmt, str):
-            raise TypeError('the defined format should be a string')
-        elif fmt in mcs._registered_format:
-            raise ValueError(f'the format {fmt} have been defined before')
-        else:
-            cls = super(_MoleculeIO, mcs).__new__(mcs, name, bases, namespace, **kwargs)
-            mcs._registered_format[fmt] = cls
-            return cls
-
-    @classmethod
-    def registered_format(mcs):
-        return copy(mcs._registered_format)
-
-
-class MetaIO(type):
-    """
-    The Meta class to specify how to construct the IO class
-    This Meta class is defined to register IO function conveniently.
-
-    The IO functions are divided into three categories:
-        - preprocess: do something before performing any of IO operation, with prefix '_pre'
-        - io: performing the IO operation, with prefix '_io'
-        - postprocess: do something after preforming IO operation, with prefix '_post'
-
-    This Meta class offer two approach to defined and register the IO functions:
-        - Define inside the IO class (IOClass)
-        - Define outside the IO class and decorate the defined function by IOClass.register function
-
-    To define inside the IOClass, one should name the IO function with the pattern:
-        def _prefix_keys():
-            ...
-    where, the prefix is one of 'pre', 'io' or 'post'; the keys is the handle name to retrieve the
-    IO functions.
-
-    To define outside the IOClass, one should applied the class method register as the decorator of the
-    IO functions, specified the prefix and the handle name as the decorator arguments, like:
-        @IOClass.register(fmt='keys', types='prefix')
-        def outside_io_func(*args, **kwargs):
-            ...
-    where the IOClass is one of Reader, Writer, Dumper, Parser or other custom IOClass, the 'key' and 'prefix'
-    should be replace to the handle name and prefix you specified.
-    """
-
-    def __new__(mcs, name: str, bases: tuple, namespace: dict, **kwargs):
-        """ If the subclasses contain methods with the prefix of '_pre', '_io' or '_post'
-        they are seen as the IO function, that the preprocess, io or postprocess functions, respectively
-        """
-        _register = Register()
-
-        for attr_name, attr in namespace.items():
-
-            # Make sure the io function is a Callable obj
-            if not isinstance(attr, Callable):
-                continue
-
-            split_names = attr_name.split('_')
-
-            # the custom IO function should with prefix: '_pre', '_io' and '_post'
-            # the handle keys of these function are follow the above prefix and separate be '_'
-            # for example:
-            #     def _pre_gjf(*args, **kwargs):
-            #         ...
-            # this is a preprocess IO function with a handle key: 'gjf' to retrieve the function.
-            if len(split_names) <= 2:
-                continue
-
-            io_type = split_names[1]
-
-            # Register the io functions:
-            # if a define methods with the prefix '_pre', '_io' or '_post'
-            # these methods are seen as preprocess, io or postprocess functions, respectively
-            if io_type == 'pre':
-                _register.pre_methods['_'.join(split_names[2:])] = attr
-            if io_type == 'io':
-                _register.io_methods['_'.join(split_names[2:])] = attr
-            if io_type == 'post':
-                _register.post_methods['_'.join(split_names[2:])] = attr
-
-        namespace[f'_register'] = _register
-
-        return type(name, bases, namespace, **kwargs)
-
-
-class IOBase:
-    """ The base IO class """
-    # Initialize the register function, which is a callable obj embed in IO classes
-    # When to register new IO function, apply the register function as decorator
-
-    # _register = None
-
-    def __init__(self, fmt: str, source: Union['ci.Molecule', IOStream], *args, **kwargs):
-        """"""
-        self.fmt = fmt
-        self.src = source
-
-        self.args = args
-        self.kwargs = kwargs
-
-        # override this methods to check the
-        self.result = self._checks()
-
-    def __call__(self):
-        """ Call for the performing of IO """
-        try:
-            self._pre()
-            # For dumper, the obj is Literal str or bytes obj
-            # For parser, the obj is Molecule obj
-            io_func = self._get_io()
-            if io_func:  # If a custom io function have been defined, run custom functions
-                obj = io_func(self)
-            else:  # else get the general io function define in class
-                obj = self._io()
-
-            return self._post(obj)
-
-        except IOEarlyStop:
-            return None
-
-    @abstractmethod
-    def _checks(self) -> Dict[str, Any]:
-        """
-        This method should be overriden when definition of new IO class
-        The purpose of this class is to check the regulation of initialized arguments.
-        If not any arguments should be checked, return None directly.
-        """
-        raise NotImplemented()
-
-    def _get_pre(self) -> Callable:
-        return self.register.pre(self.fmt)
-
-    def _get_io(self) -> Callable:
-        return self.register.io(self.fmt)
-
-    def _get_post(self) -> Callable:
-        return self.register.post(self.fmt)
-
-    def _pre(self, *args, **kwargs):
-        """ Regulate the method of preprocess """
-        pre_func = self._get_pre()
-        if pre_func:
-            pre_func(self)
-
-    @abstractmethod
-    def _io(self, *args, **kwargs):
-        """ Regulate the main io method """
-        raise NotImplemented
-
-    def _post(self, obj, *args, **kwargs):
-        """ Regulate the method of postprocess """
-        post_func = self._get_post()
-        if post_func:
-            return post_func(self, obj)
-        else:
-            return obj
-
-    @property
-    def register(self) -> Register:
-        return getattr(self, f'_register')
-
-
-class Dumper(IOBase, metaclass=MetaIO):
-    """
-    Dump the Molecule information into specific format.
-    The output in general is the string or bytes
-    """
-
-    _pybel_fmt_convert = {
-    }
-
-    def _process_lmpdat_bonds(self, bond_contents: list):
-        """"""
-        uni_bonds = tuple(self.src.unique_bonds)
-        bonds = self.src.bonds
-        sep = re.compile(r'\s+')
-        for i, bc in enumerate(bond_contents):
-            split_bc = sep.split(bc)
-            split_bc[1] = str(uni_bonds.index(bonds[i]) + 1)
-            bond_contents[i] = '  '.join(split_bc)
-
-        return bond_contents
-
-    def _io(self):
-        """ Performing the IO operation, convert the Molecule obj to Literal obj """
-        # Try to dump by openbabel.pybel
-        type_err_pattern = re.compile(
-            r"write\(\) got an unexpected keyword argument '\w+'"
-        )
-        pb_mol = pybel.Molecule(self.src.ob_mol)
-        kwargs = copy(self.kwargs)
-
-        while kwargs:
-            try:
-                return pb_mol.write(self._pybel_fmt_convert.get(self.fmt, self.fmt), **kwargs)
-
-            except TypeError as error:
-                if type_err_pattern.match(str(error)):
-                    pop_kwargs = str(error).split()[-1].strip("'")
-                    kwargs.pop(pop_kwargs)
-                else:
-                    raise error
-
-            except ValueError:
-                print(IOError(f'the cheminfo.Molecule obj cannot dump to Literal'))
-                return None
-
-        return pb_mol.write(self._pybel_fmt_convert.get(self.fmt, self.fmt))
-
-    def _checks(self) -> Dict[str, Any]:
-        if not isinstance(self.src, ci.Molecule):
-            raise TypeError(f'the dumped object should be hotpot.cheminfo.Molecule, instead of {type(self.src)}')
-
-        return {}
-
-    def _pre_cif(self):
-        """
-        pre-process for Molecule object to convert to cif file.
-        if the hotpot object do not place in a Crystal, create a P1 compact Crystal for it
-        """
-        crystal = self.src.crystal()
-        if not isinstance(crystal, ci.Crystal) or (
-                np.logical_not(crystal.vector >= 0.).any() and np.logical_not(crystal.vector < 0.).any()
-        ):
-            self.src.compact_crystal(inplace=True)
-
-        if self.src.crystal().space_group:
-            self.src.crystal().space_group = 'P1'
-
-    def _pre_gjf(self):
-        """ Assign the Molecule charge before to dump to gjf file """
-        if not self.src.has_3d:
-            self.src.build_3d()
-
-        self.src.assign_atoms_formal_charge()
-        self.src.identifier = self.src.formula
-
-    def _io_dpmd_sys(self):
-        """ convert molecule information to numpy arrays """
-        return DeepSystem(self.src)
-
-    def _io_lmpmol(self):
-        """
-        write a molecule script
-        default values: coordinates, velocities, atom IDs and types
-        additional attributes for atomic: Bonds
-        additional attributes for full: Bonds + molecular + charge
-        """
-
-        def bonds(m):
-            """ Add bond body """
-            bond_str = 'Bonds' + '\n\n'  # bond body title
-
-            # the formula of bond_type key: atom1[bond_type]atom2
-            uni_bonds = tuple(m.unique_bonds)  # store bonds type
-            for j, bond in enumerate(m.bonds, 1):
-
-                bt_id = uni_bonds.index(bond) + 1
-                bond_str += f'{j} {bt_id} {bond.ob_atom1_id + 1} {bond.ob_atom2_id + 1}\n'
-
-            bond_str += '\n'
-
-            return bond_str
-
-        def charge():
-            """ Retrieve atom charge information """
-            charge_str = '\n' + 'Charges' + '\n\n'
-
-            for ic, a in enumerate(atoms_list, 1):  # ID of charge, atom
-                if isinstance(a, ci.Atom):
-                    charge_str += f'{ic} {a.partial_charge}\n'
-                else:
-                    assert isinstance(a, ci.PseudoAtom)
-                    charge_str += f'{ic} {a.charge}\n'
-
-            charge_str += '\n'
-
-            return charge_str
-
-        mol = self.src
-        kwargs = self.kwargs  # keywords arguments
-
-        # default values: coordinates, velocities, atom IDs and types;
-        # additional attributes for atomic: None;
-        # additional attributes for full: molecular + charge
-        atom_style = kwargs.get('atom_style', 'atomic')   # default atom_style is atomic
-        mol_name = kwargs.get('mol_name', mol.smiles)
-
-        # combine real atoms with pseudo atoms in a list
-        atoms_list = []
-        for m_a in mol.atoms:
-            atoms_list.append(m_a)
-
-        if mol.pseudo_atoms:   # determine if there are pseudo_atoms
-            for pse_a in mol.pseudo_atoms:
-                atoms_list.append(pse_a)
-
-        # title information
-        title = f"Create by hotpot package, convert from {mol_name}"
-        script = title + '\n\n'   # write the molecular script for lammps
-
-        # TODO: some header information missing
-        # Header partition
-        # add atom header
-        num_atoms = len(atoms_list)
-        num_atoms_str = f'{num_atoms}  atoms'
-        script += num_atoms_str + '\n'
-
-        # add bond header
-        num_bonds = len(mol.bonds)
-        num_bonds_str = f'{num_bonds}  bonds'
-        script += num_bonds_str + '\n'
-
-        # Add new blank line to end the header partition
-        script += '\n'
-
-        # Body partition
-        # Coords body
-        script += 'Coords' + '\n\n'
-        for i, atom in enumerate(atoms_list, 1):
-            script += f'{i}' + '  ' + '  '.join(map(str, atom.coordinates)) + '\n'
-        script += '\n'
-
-        # Types body
-        script += 'Types' + '\n\n'
-
-        dict_types = {}
-        for i, atom in enumerate(atoms_list, 1):
-            atom_type = dict_types.setdefault(atom.symbol, len(dict_types)+1)
-            script += f'{i} {atom_type}  # {atom.symbol}\n'
-
-        script += '\n'
-
-        # additional attributes
-        # to atomic style, only basis information (ID，Coords, types, velocitier)
-        if atom_style == 'atomic':
-            if num_bonds:
-                script += bonds(mol)
-
-        # to full style, basis information + molecular + charge
-        elif atom_style == 'full':
-            if num_bonds:
-                script += bonds(mol)
-            script += charge()
-
-        return script
-
-    def _post_gjf(self, script):
-        """ postprocess the dumped Gaussian 16 .gjf script to add the link0 and route context """
-        # To count the insert lines
-        inserted_lines = 0
-
-        # separate keyword arguments:
-        link0 = self.kwargs['link0']
-        route = self.kwargs['route']
-        custom_charge = self.kwargs.get('charge')
-        custom_spin = self.kwargs.get('spin')
-
-        lines = script.splitlines()
-
-        # Write link0 command
-        if isinstance(link0, str):
-            lines[0] = f'%{link0}'
-        elif isinstance(link0, list):
-            for i, stc in enumerate(link0):  # stc=sentence
-                assert isinstance(stc, str)
-                if not i:  # For the first line of link0, replace the original line in raw script
-                    lines[0] = f'%{stc}'
-                else:  # For the other lines, insert into after the 1st line
-                    inserted_lines += 1
-                    lines.insert(inserted_lines, f'%{stc}')
-        else:
-            raise TypeError('the link0 should be string or list of string')
-
-        # Write route command
-        if isinstance(route, str):
-            lines[1+inserted_lines] = f'# {route}'
-        elif isinstance(route, list):
-            for i, stc in enumerate(route):
-                assert isinstance(stc, str)
-                if not i:  # For the first line of link0, replace the the original line in raw script
-                    lines[1+inserted_lines] = f'#{stc}'
-                else:  # For the other lines, insert into after the original route line.
-                    inserted_lines += 1
-                    lines.insert(inserted_lines+1, f'%{stc}')
-        else:
-            raise TypeError('the route should be string or list of string')
-
-        charge, spin = lines[5+inserted_lines].split()
-        if custom_charge:
-            charge = str(custom_charge)
-        if custom_spin:
-            spin = str(custom_spin)
-
-        lines[5+inserted_lines] = f'{charge} {spin}'
-
-        script = '\n'.join(lines)
-
-        # End black line
-        script += '\n\n'
-
-        return script
-
-    def _post_lmpdat(self, script: str):
-        """ post-process for LAMMPS data file """
-
-        title, headers, bodies = _parse_lmp_data_script(script)
-        script = title + '\n'
-
-        for ht, hvs in headers.items():
-            if ht == 'bond types':  # header title, header values
-                hvs[0] = len(self.src.unique_bonds)
-
-            script += ' '.join(map(str, hvs)) + ' ' + ht + '\n'
-
-        script += '\n' * 3
-
-        for bt, bcs in bodies.items():  # body title, body contents
-            if bt == 'Bonds':
-                bcs = self._process_lmpdat_bonds(bcs)
-
-            if bcs:  # if the body contents exist
-                script += bt + '\n' * 2
-                script += '\n'.join(bcs)
-                script += '\n' * 3
-
-        return script
-
-
-class Parser(IOBase, metaclass=MetaIO):
-    """ Parse the str or bytes obj to Molecule obj """
-    _pybel_fmt_convert = {
-        'g16log': 'g16'
-    }
-
-    def _open_source_to_string_lines(self, *which_allowed: str, output_type: Literal['lines', 'script'] = 'lines'):
-        """
-        Open the source file to string lines
-        Args:
-            which_allowed: which types of source are allowed to process to string lines
-
-        Returns:
-            (List of string|string)
-        """
-        src_type = self.result.get('src_type')
-        if src_type not in which_allowed:
-            raise RuntimeError(f'the source type {type(self.src)} have not been supported')
-        else:
-            if src_type == 'str':
-                script = self.src
-
-            elif src_type == 'path':
-                with open(self.src) as file:
-                    try:
-                        script = file.read()
-                    # If the file pointed by the path is not a text file
-                    # such as a bytes file
-                    except UnicodeDecodeError:
-                        raise IOEarlyStop()
-
-            elif src_type == 'IOString':
-                script = self.src.read()
-
-            else:
-                raise RuntimeError(f'the source type {type(self.src)} have not been supported')
-
-            if output_type == 'lines':
-                return script.split('\n')
-            elif output_type == 'script':
-                return script
-            else:
-                raise ValueError('the arg output_type given a wrong values, lines or script allow only')
-
-    def _checks(self) -> Dict[str, Any]:
-        if not isinstance(self.src, (IOBase, str, bytes, PathLike)):
-            raise TypeError(f'the parsed object should be IOBase, str or bytes, instead of {type(self.src)}')
-
-        if isinstance(self.src, str):
-            if os.path.exists(self.src):
-                return {'src_type': 'path'}
-            else:
-                return {'src_type': 'str'}
-
-        if isinstance(self.src, PathLike):
-            return {'src_type': 'path'}
-
-        if isinstance(self.src, bytes):
-            return {'src_type': 'bytes'}
-        if isinstance(self.src, io.StringIO):
-            return {'src_type': 'StringIO'}
-        if isinstance(self.src, io.BytesIO):
-            return {'src_type': 'BytesIO'}
-        if isinstance(self.src, io.FileIO):
-            return {'src_type': 'FileIO'}
-        print(f'the get source type is {type(self.src)}')
-        return {'src_type': type(self.src)}
-
-    def _ob_io(self):
-        """ IO by openbabel.pybel """
-        # Get the source type name
-        src_type = self.result.get('src_type')
-        try:
-            if src_type == 'str':
-                pybel_mol = pybel.readstring(self._pybel_fmt_convert.get(self.fmt, self.fmt), self.src)
-            elif src_type == 'path':
-                pybel_mol = next(pybel.readfile(self._pybel_fmt_convert.get(self.fmt, self.fmt), str(self.src)))
-            elif src_type == 'IOString':
-                pybel_mol = pybel.readstring(self._pybel_fmt_convert.get(self.fmt, self.fmt), self.src.read())
-            else:
-                raise RuntimeError(f'the source type {type(self.src)} have not been supported')
-
-            obj = ci.Molecule(pybel_mol.OBMol)
-
-        except RuntimeError:
-            obj = None
-
-        return obj
-
-    def _cclib_io(self, obj):
-        """ IO by cclib package """
-        src_type = self.result.get('src_type')
-
-        try:
-            if src_type == 'str':
-                data = cclib.ccopen(io.StringIO(self.src)).parse()
-            elif src_type == 'path':
-                data = cclib.ccopen(self.src).parse()
-            elif src_type == 'IOString':
-                data = cclib.ccopen(self.src).parse()
-            else:
-                raise RuntimeError(f'the source type {type(self.src)} have not been supported in cclib')
-
-        except (RuntimeError, AttributeError):
-            data = None
-
-        if data:
-            if not obj:
-                # if get information about the atoms species
-                if hasattr(data, 'atomnos'):
-                    atoms_attrs = [{'atomic_number': an} for an in getattr(data, 'atomnos')]
-                    obj = ci.Molecule(atoms=atoms_attrs)
-                else:
-                    print(IOError(f'the parsing of {self.src} is not successful!'))
-                    return obj  # Return None
-
-            # if get information about the coordination collections
-            if hasattr(data, 'atomcoords'):
-                obj.set(all_coordinates=getattr(data, 'atomcoords'))
-
-            # if get information about the energy (SCF energies) vector
-            if hasattr(data, 'scfenergies'):
-                obj.set(all_energy=getattr(data, 'scfenergies'))
-
-        return obj
-
-    def _io(self, *args, **kwargs):
-        """ Standard IO process """
-        # Try parse the log file by openbabel.pybel file firstly
-        return self._ob_io()
-
-    # Start to the prefix IO functions
-
-    # preprocess for g16log file
-    # This preprocess is used to judge whether a Error happened when perform g16 calculate
-    def _pre_g16log(self):
-        """ g16log preprocess to judge whether some Error happened """
-        def is_convergence_failure():
-            if 'Convergence failure -- run terminated.' in script:
-                return True
-            return False
-
-        def is_hessian_no_longer_linear_valid():
-            march_pattern = re.compile(r'Error termination via Lnk1e in (/.+)*/l103\.exe')
-
-            if any (march_pattern.match(line.strip()) for line in script.splitlines()[-5:]):
-                return True
-            return False
-
-        script = self._open_source_to_string_lines('str', 'path', "IOString", output_type='script')
-
-        # Check whether a failure have happened when calculation.
-        if is_convergence_failure():
-            raise IOEarlyStop('Gaussian16 SCF cannot convergence!')
-        if is_hessian_no_longer_linear_valid():
-            raise IOEarlyStop('Gaussian16 Hessian no longer linear valid')
-
-    # Parse the XYZ file
-    def _io_xyz(self):
-        """ Parse the XYZ file """
-        src_type = self.result['src_type']
-        if src_type != 'path':
-            return self._io()
-        else:
-            from ase import io
-            from openbabel import openbabel as ob
-            data_generator = io.iread(self.src)
-
-            # atomic_numbers, coordinates, cell_params
-            atomic_numbers, all_coordinates, cell_matrix = [], [], None
-            for data in data_generator:
-                atomic_numbers.append(data.numbers)
-                all_coordinates.append(data.positions)
-                if cell_matrix is None:
-                    cell_matrix = data.cell.array
-
-            atomic_numbers = np.stack(atomic_numbers)
-            all_coordinates = np.stack(all_coordinates)
-
-            number_min = atomic_numbers.min(axis=0)
-            number_max = atomic_numbers.max(axis=0)
-
-            # the values in same columns should be same.
-            assert all(number_max == number_min)
-
-            obj = ci.Molecule()
-            obj.quick_build_atoms(number_min)
-
-            obj.set(all_coordinates=all_coordinates)
-            obj.set(crystal=cell_matrix)
-            obj.conformer_select(0)
-
-            return obj
-
-    # postprocess for g16log file
-    def _post_g16log(self, obj: 'ci.Molecule'):
-        """
-        post process for g16log format, to extract:
-            1) Mulliken charge
-            2) Spin densities
-        """
-        def extract_charges_spin():
-            """ Extract charges and spin information from g16.log file """
-            # Get the line index of Mulliken charges
-            head_lines = [i for i, line in enumerate(lines) if line.strip() == 'Mulliken charges and spin densities:']
-            if not head_lines:
-                head_lines = [i for i, line in enumerate(lines) if line.strip() == 'Mulliken charges:']
-                charge_only = True
-            else:
-                charge_only = False
-
-            # Skip the first charge&spin sheet, it can't find corresponding coordinates
-            if not head_lines:
-                raise IOEarlyStop
-            elif len(head_lines) == obj.conformer_counts + 1:
-                head_lines = head_lines[1:]
-
-            # Extract the Mulliken charge and spin densities
-            charges, spin_densities = [], []  # changes(cgs) spin_densities(sds)
-            for i in head_lines:
-                # Enhance inspection
-                col_heads = lines[i + 1].strip().split()
-                if charge_only:
-                    assert len(col_heads) == 1 and col_heads[0] == '1'
-                else:
-                    assert len(col_heads) == 2 and col_heads[0] == '1' and col_heads
-
-                HEAD_LINES_NUM = 2
-                cg, sd = [], []  # change, spin_density
-
-                while True:
-                    split_line = lines[i + HEAD_LINES_NUM].strip().split()
-                    if charge_only and len(split_line) == 3:
-                        row, syb, c = split_line  # row number, symbol, charges
-                        s = 0.0  # spin density
-                    elif not charge_only and len(split_line) == 4:
-                        row, syb, c, s = split_line  # row number, symbol, charges, spin density
-                    else:
-                        break
-
-                    try:
-                        row, c, s = int(row), float(c), float(s)
-                        # check the sheet row number
-                        if row != HEAD_LINES_NUM - 1:
-                            break
-
-                    # Inspect the types of values
-                    except ValueError:
-                        break
-
-                    # record the charge and spin density
-                    cg.append(c)
-                    sd.append(s)
-                    HEAD_LINES_NUM += 1
-
-                # store the extracted
-                if cg and sd:
-                    if len(cg) == len(sd) == len(obj.atoms):
-                        charges.append(cg)
-                        spin_densities.append(sd)
-                    else:
-                        raise ValueError('the number of charges do not match to the number of atoms')
-                else:
-                    raise ValueError('get a empty charge and spin list, check the input!!')
-
-            obj.set(all_atom_charges=np.array(charges))
-            obj.set(all_atom_spin_densities=np.array(spin_densities))
-                
-        def extract_force_matrix():
-            # Define the format of force sheet
-            # the Force sheet like this:
-            #  -------------------------------------------------------------------
-            #  Center     Atomic                   Forces (Hartrees/Bohr)
-            #  Number     Number              X              Y              Z
-            #  -------------------------------------------------------------------
-            #       1        8           0.039901671    0.000402574    0.014942530
-            #       2        8           0.017381613    0.001609531    0.006381231
-            #       3        6          -0.092853735   -0.025654844   -0.005885898
-            #       4        6           0.067801154    0.024130172   -0.022794721
-            #       5        8          -0.023702905    0.005486251   -0.004938175
-            #       6        8          -0.006359715   -0.008543465    0.010350815
-            #       7       55          -0.002168084    0.002569781    0.001944217
-            #  -------------------------------------------------------------------
-            force_head1 = re.compile(r'\s*Center\s+Atomic\s+Forces\s\(Hartrees/Bohr\)\s*')
-            force_head2 = re.compile(r'\s*Number\s+Number\s+X\s+Y\s+Z\s*')
-            sheet_line = re.compile(r'\s*----+\s*')
-
-            HEAD_LINES_NUM = 3  # the offset line to write the header
-
-            head_lines = [i for i, line in enumerate(lines) if force_head1.match(line)]
-
-            all_forces = []
-            for i in head_lines:
-                # enhance the inspection of Force sheet head
-                assert force_head2.match(lines[i + 1])
-                assert sheet_line.match(lines[i + 2])
-
-                rows = 0
-                forces = []
-                while True:
-
-                    if sheet_line.match(lines[i + HEAD_LINES_NUM + rows]):
-                        if len(forces) == obj.atom_counts:
-                            all_forces.append(forces)
-                            break
-                        else:
-                            raise ValueError('the number of force vector do not match the number of atoms')
-
-                    ac, an, x, y, z = map(
-                        lambda v: int(v[1]) if v[0] < 2 else float(v[1]),
-                        enumerate(lines[i + HEAD_LINES_NUM + rows].split())
-                    )
-
-                    # Enhance the inspection
-                    assert ac == rows + 1
-                    if obj.atoms[rows].atomic_number != an:
-                        raise ValueError('the atomic number do not match')
-
-                    forces.append([x, y, z])
-
-                    rows += 1
-
-            try:
-                obj.set(all_forces=np.array(all_forces))
-            except ValueError:
-                return
-
-        obj = self._cclib_io(obj)  # Try to supplementary Molecule data by cclib
-
-        lines = self._open_source_to_string_lines('str', 'path', 'IOString')
-
-        try:  # TODO: For now, this is the case, the spin densities may lost in some case  # the units is Hartree/Bohr
-            extract_charges_spin()
-            extract_force_matrix()
-        except IndexError:
-            raise IOEarlyStop
-
-        # assign the first conformer for the molecule
-        obj.conformer_select(0)
-
-        return obj
-
-
+"""
+python v3.7.9
+@Project: hotpot
+@File   : _io.py
+@Author : Zhiyuan Zhang
+@Date   : 2023/3/14
+@Time   : 4:18
+"""
+import os
+import re
+from pathlib import Path
+from os import PathLike
+from typing import *
+from abc import ABCMeta, abstractmethod
+from copy import copy
+import io
+from io import IOBase
+from openbabel import pybel
+import cclib
+import numpy as np
+
+import hotpot.cheminfo as ci
+from hotpot.tanks.deepmd import DeepSystem
+
+"""
+Notes:
+This module contain Classes to IO between the Molecule object and various file formats.
+the main classes are:
+    - Reader: from Formatted files to Molecule, called by the Molecule.read() method.
+    - Writer: from Molecule to formatted files, called by the Molecule.write() method.
+    - Dumper: from Molecule to formatted Literals(str or bytes), called by the Molecule.dump() method.
+    - Parser: from formatted Literals to the Molecule obj, called by the Molecule.parse() method.
+all of them are inherit from the _IOBase class.
+
+For the implementation of dump and parse:
+    - some third-part package are used, like openbabel, cclib and so on.
+    - there are some self own IO function be defined too.
+    - the user also custom and register to the Dumper and Parser too.
+
+When implementing the IO: 
+    1) the IO class will firstly check whether a custom IO function is defined and register, if the IO function 
+        are defined and registered, the IO are implemented by the registered.
+    2) else, the IO class will try to call, in turn, try to call some third-part packages,
+    3) finally, if all third-part packages fail to complement IO, Raise the IOError !!!
+
+Following the steps to customise your IO function:
+    1) determine which IO operation(read, write, dump or parse) you want to define， import the relevant IO class
+        into your own python modules.
+    2) define the IO function which customises your IO implementation, the custom function should meet the base
+        requirements demand by the corresponding IO class. When the IO functions are defined, applying the
+        `IOClass`.register decorator to register the IO function into the `IOClass`, the `IOClass`.register should
+        pass some args. This is a example:
+        --------------------------------- Example ------------------------------------
+        Examples:
+        # importing the relevant IO classes
+        from hotpot.io import Dumper, Reader
+        
+        # define and register a read function
+        # the fmt defined the format key to handle the custom IO function
+        # the types defined where the IO function will be applied, pre: preprocess, io: main io, post: postprocess
+        @Reader.register(fmt='the/format/key', types='pre|io|post')
+        def my_read_func(*arg, **kwargs)  # the args should meet the Reader demand
+            ...
+            
+        # define and register a dump function
+        def my_dump_func(*arg, **kwargs) # the args should meet the Dumper demand
+            ...
+        ---------------------------------- END ---------------------------------------
+"""
+
+
+# Define custom Exceptions
+class IOEarlyStop(BaseException):
+    """ monitor the situation that the IO should early stop and return None and the IO result """
+
+
+# Define the IO function types
+IOFuncPrefix = Literal['pre', 'io', 'post']
+IOStream = Union[IOBase, str, bytes]
+
+
+def _parse_lmp_data_script(script: str):
+    """ Parse the LAMMPS data script to two dict, header and body"""
+    # Define_body_title
+    bt_name = (
+        # atom-property sections
+        'Atoms', 'Velocities', 'Masses', 'Ellipsoids', 'Lines', 'Triangles', 'Bodies',
+        # molecular topology sections
+        'Bonds', 'Angles', 'Dihedrals', 'Impropers',
+        # force field sections
+        'Pair Coeffs', 'PairIJ Coeffs', 'Bond Coeffs', 'Angle Coeffs', 'Dihedral Coeffs', 'Improper Coeffs',
+        # class 2 force field sections
+        'BondBond Coeffs', 'BondAngle Coeffs', 'MiddleBondTorsion Coeffs', 'EndBondTorsion Coeffs',
+        'AngleTorsion Coeffs', 'AngleAngleTorsion Coeffs', 'BondBond13 Coeffs', 'AngleAngle Coeffs'
+    )
+
+    # Compile the body and header pattern
+    header_title = re.compile(r'[a-z]+')
+    header_int = re.compile(r'[0-9]+')
+    header_float = re.compile(r'-?[0-9]+\.[0-9]*')
+
+    lines = script.split('\n')
+    body_split_point = [i for i, lin in enumerate(lines) if lin in bt_name] + [len(lines)]
+
+    # Extract header info
+    headers = {}
+    for line in lines[1:body_split_point[0]]:
+        line = line.strip()
+        if line:
+            ht = ' '.join(header_title.findall(line))
+            hvs = line[:line.find(ht)].strip()  # header values
+            header_values = []
+            for hv in re.split(r'\s+', hvs):
+                if header_int.fullmatch(hv):
+                    header_values.append(int(hv))
+                elif header_float.fullmatch(hv):
+                    header_values.append(float(hv))
+                else:
+                    raise ValueError('the header line not match well')
+
+            headers[ht] = header_values
+
+    # Extract bodies info
+    bodies = {}
+    for sl_idx, el_idx in zip(body_split_point[:-1], body_split_point[1:]):
+        bt = lines[sl_idx].strip()  # body title
+        bc = [line.strip() for line in lines[sl_idx+1: el_idx] if line.strip()]  # body content
+        bodies[bt] = bc
+
+    return lines[0], headers, bodies
+
+
+class Register:
+    """
+    Register the IO function for Dumper, Parser or so on
+    """
+    def __init__(self):
+        # these dicts are container to store the custom io functions
+        # the keys of the dict are serve as the handle to get the mapped io functions(the values)
+        self.pre_methods = {}
+        self.io_methods = {}
+        self.post_methods = {}
+
+    def __repr__(self):
+        return f"Register:\n" + \
+               f"pre_method:\n" + \
+               f"\n\t".join([n for n in self.pre_methods]) + "\n\n" + \
+               f"io methods:\n" + \
+               f"\n\t".join([n for n in self.io_methods]) + '\n\n' + \
+               f"post methods:\n" + \
+               f"\n\t".join([n for n in self.post_methods])
+
+    def __call__(self, io_cls: type, fmt: str, prefix: IOFuncPrefix):
+        """
+        To register any function as a dumper or a postprocess to convert mol to formats
+        Args:
+            fmt:
+            prefix:
+
+        Returns:
+
+        """
+
+        def decorator(func: Callable):
+
+            if prefix == 'pre':
+                self.pre_methods[fmt] = func
+            elif prefix == 'io':
+                self.io_methods[fmt] = func
+            elif prefix == 'post':
+                self.post_methods[fmt] = func
+            else:
+                raise TypeError('the type of register is not supported')
+
+            return func
+
+        return decorator
+
+    def pre(self, fmt: str):
+        return self.pre_methods.get(fmt)
+
+    def io(self, fmt: str):
+        return self.io_methods.get(fmt)
+
+    def post(self, fmt: str):
+        return self.post_methods.get(fmt)
+
+
+# Retrieve the IO class by its format name
+def retrieve_format(fmt: str = None):
+    return _MoleculeIO.registered_format().get(fmt)
+
+
+# Get all registered format name
+def registered_format_name():
+    return tuple(_MoleculeIO.registered_format().keys())
+
+
+# TODO: deprecated in the later version
+class _MoleculeIO(ABCMeta):
+    """    Metaclass for registration of IO class format """
+    _registered_format = {}
+
+    def __new__(mcs, name, bases, namespace, **kwargs):
+        # Get the format keywords
+        fmt = namespace.get('format')(mcs)
+
+        if not fmt:
+            return super(_MoleculeIO, mcs).__new__(mcs, name, bases, namespace, **kwargs)
+        elif not isinstance(fmt, str):
+            raise TypeError('the defined format should be a string')
+        elif fmt in mcs._registered_format:
+            raise ValueError(f'the format {fmt} have been defined before')
+        else:
+            cls = super(_MoleculeIO, mcs).__new__(mcs, name, bases, namespace, **kwargs)
+            mcs._registered_format[fmt] = cls
+            return cls
+
+    @classmethod
+    def registered_format(mcs):
+        return copy(mcs._registered_format)
+
+
+class MetaIO(type):
+    """
+    The Meta class to specify how to construct the IO class
+    This Meta class is defined to register IO function conveniently.
+
+    The IO functions are divided into three categories:
+        - preprocess: do something before performing any of IO operation, with prefix '_pre'
+        - io: performing the IO operation, with prefix '_io'
+        - postprocess: do something after preforming IO operation, with prefix '_post'
+
+    This Meta class offer two approach to defined and register the IO functions:
+        - Define inside the IO class (IOClass)
+        - Define outside the IO class and decorate the defined function by IOClass.register function
+
+    To define inside the IOClass, one should name the IO function with the pattern:
+        def _prefix_keys():
+            ...
+    where, the prefix is one of 'pre', 'io' or 'post'; the keys is the handle name to retrieve the
+    IO functions.
+
+    To define outside the IOClass, one should applied the class method register as the decorator of the
+    IO functions, specified the prefix and the handle name as the decorator arguments, like:
+        @IOClass.register(fmt='keys', types='prefix')
+        def outside_io_func(*args, **kwargs):
+            ...
+    where the IOClass is one of Reader, Writer, Dumper, Parser or other custom IOClass, the 'key' and 'prefix'
+    should be replace to the handle name and prefix you specified.
+    """
+
+    def __new__(mcs, name: str, bases: tuple, namespace: dict, **kwargs):
+        """ If the subclasses contain methods with the prefix of '_pre', '_io' or '_post'
+        they are seen as the IO function, that the preprocess, io or postprocess functions, respectively
+        """
+        _register = Register()
+
+        for attr_name, attr in namespace.items():
+
+            # Make sure the io function is a Callable obj
+            if not isinstance(attr, Callable):
+                continue
+
+            split_names = attr_name.split('_')
+
+            # the custom IO function should with prefix: '_pre', '_io' and '_post'
+            # the handle keys of these function are follow the above prefix and separate be '_'
+            # for example:
+            #     def _pre_gjf(*args, **kwargs):
+            #         ...
+            # this is a preprocess IO function with a handle key: 'gjf' to retrieve the function.
+            if len(split_names) <= 2:
+                continue
+
+            io_type = split_names[1]
+
+            # Register the io functions:
+            # if a define methods with the prefix '_pre', '_io' or '_post'
+            # these methods are seen as preprocess, io or postprocess functions, respectively
+            if io_type == 'pre':
+                _register.pre_methods['_'.join(split_names[2:])] = attr
+            if io_type == 'io':
+                _register.io_methods['_'.join(split_names[2:])] = attr
+            if io_type == 'post':
+                _register.post_methods['_'.join(split_names[2:])] = attr
+
+        namespace[f'_register'] = _register
+
+        return type(name, bases, namespace, **kwargs)
+
+
+class IOBase:
+    """ The base IO class """
+    # Initialize the register function, which is a callable obj embed in IO classes
+    # When to register new IO function, apply the register function as decorator
+
+    # _register = None
+
+    def __init__(self, fmt: str, source: Union['ci.Molecule', IOStream], *args, **kwargs):
+        """"""
+        self.fmt = fmt
+        self.src = source
+
+        self.args = args
+        self.kwargs = kwargs
+
+        # override this methods to check the
+        self.result = self._checks()
+
+    def __call__(self):
+        """ Call for the performing of IO """
+        try:
+            self._pre()
+            # For dumper, the obj is Literal str or bytes obj
+            # For parser, the obj is Molecule obj
+            io_func = self._get_io()
+            if io_func:  # If a custom io function have been defined, run custom functions
+                obj = io_func(self)
+            else:  # else get the general io function define in class
+                obj = self._io()
+
+            return self._post(obj)
+
+        except IOEarlyStop:
+            return None
+
+    @abstractmethod
+    def _checks(self) -> Dict[str, Any]:
+        """
+        This method should be overriden when definition of new IO class
+        The purpose of this class is to check the regulation of initialized arguments.
+        If not any arguments should be checked, return None directly.
+        """
+        raise NotImplemented()
+
+    def _get_pre(self) -> Callable:
+        return self.register.pre(self.fmt)
+
+    def _get_io(self) -> Callable:
+        return self.register.io(self.fmt)
+
+    def _get_post(self) -> Callable:
+        return self.register.post(self.fmt)
+
+    def _pre(self, *args, **kwargs):
+        """ Regulate the method of preprocess """
+        pre_func = self._get_pre()
+        if pre_func:
+            pre_func(self)
+
+    @abstractmethod
+    def _io(self, *args, **kwargs):
+        """ Regulate the main io method """
+        raise NotImplemented
+
+    def _post(self, obj, *args, **kwargs):
+        """ Regulate the method of postprocess """
+        post_func = self._get_post()
+        if post_func:
+            return post_func(self, obj)
+        else:
+            return obj
+
+    @property
+    def register(self) -> Register:
+        return getattr(self, f'_register')
+
+
+class Dumper(IOBase, metaclass=MetaIO):
+    """
+    Dump the Molecule information into specific format.
+    The output in general is the string or bytes
+    """
+
+    _pybel_fmt_convert = {
+    }
+
+    def _preprocess_for_gjf(self):
+        """ Perform preprocess for  conversion of all gaussian input """
+        if not self.src.has_3d:
+            self.src.build_3d()
+
+        self.src.assign_atoms_formal_charge()
+        self.src.identifier = self.src.formula
+
+    def _postprocess_for_gjf_head(self, script) -> (List[str], int):
+        """ Postprocess the context before the Molecular specification partition """
+        # To count the insert lines
+        inserted_lines = 0
+
+        # separate keyword arguments:
+        link0 = self.kwargs['link0']
+        route = self.kwargs['route']
+        custom_charge = self.kwargs.get('charge')
+        custom_spin = self.kwargs.get('spin')
+
+        lines = script.splitlines()
+
+        # Write link0 command
+        if isinstance(link0, str):
+            lines[0] = f'%{link0}'
+        elif isinstance(link0, list):
+            for i, stc in enumerate(link0):  # stc=sentence
+                assert isinstance(stc, str)
+                if not i:  # For the first line of link0, replace the original line in raw script
+                    lines[0] = f'%{stc}'
+                else:  # For the other lines, insert into after the 1st line
+                    inserted_lines += 1
+                    lines.insert(inserted_lines, f'%{stc}')
+        else:
+            raise TypeError('the link0 should be string or list of string')
+
+        # Write route command
+        if isinstance(route, str):
+            lines[1+inserted_lines] = f'# {route}'
+        elif isinstance(route, list):
+            for i, stc in enumerate(route):
+                assert isinstance(stc, str)
+                if not i:  # For the first line of link0, replace the original line in raw script
+                    lines[1+inserted_lines] = f'#{stc}'
+                else:  # For the other lines, insert into after the original route line.
+                    inserted_lines += 1
+                    lines.insert(inserted_lines+1, f'%{stc}')
+        else:
+            raise TypeError('the route should be string or list of string')
+
+        charge, spin = lines[5+inserted_lines].split()
+        if custom_charge:
+            charge = str(custom_charge)
+        if custom_spin:
+            spin = str(custom_spin)
+
+        lines[5+inserted_lines] = f'{charge} {spin}'
+
+        return lines, 6 + inserted_lines
+
+    def _process_lmpdat_bonds(self, bond_contents: list):
+        """"""
+        uni_bonds = tuple(self.src.unique_bonds)
+        bonds = self.src.bonds
+        sep = re.compile(r'\s+')
+        for i, bc in enumerate(bond_contents):
+            split_bc = sep.split(bc)
+            split_bc[1] = str(uni_bonds.index(bonds[i]) + 1)
+            bond_contents[i] = '  '.join(split_bc)
+
+        return bond_contents
+
+    def _io(self):
+        """ Performing the IO operation, convert the Molecule obj to Literal obj """
+        # Try to dump by openbabel.pybel
+        type_err_pattern = re.compile(
+            r"write\(\) got an unexpected keyword argument '\w+'"
+        )
+        pb_mol = pybel.Molecule(self.src.ob_mol)
+        kwargs = copy(self.kwargs)
+
+        while kwargs:
+            try:
+                return pb_mol.write(self._pybel_fmt_convert.get(self.fmt, self.fmt), **kwargs)
+
+            except TypeError as error:
+                if type_err_pattern.match(str(error)):
+                    pop_kwargs = str(error).split()[-1].strip("'")
+                    kwargs.pop(pop_kwargs)
+                else:
+                    raise error
+
+            except ValueError:
+                print(IOError(f'the cheminfo.Molecule obj cannot dump to Literal'))
+                return None
+
+        return pb_mol.write(self._pybel_fmt_convert.get(self.fmt, self.fmt))
+
+    def _checks(self) -> Dict[str, Any]:
+        if not isinstance(self.src, ci.Molecule):
+            raise TypeError(f'the dumped object should be hotpot.cheminfo.Molecule, instead of {type(self.src)}')
+
+        return {}
+
+    def _pre_cif(self):
+        """
+        pre-process for Molecule object to convert to cif file.
+        if the hotpot object do not place in a Crystal, create a P1 compact Crystal for it
+        """
+        crystal = self.src.crystal()
+        if not isinstance(crystal, ci.Crystal) or (
+                np.logical_not(crystal.vector >= 0.).any() and np.logical_not(crystal.vector < 0.).any()
+        ):
+            self.src.compact_crystal(inplace=True)
+
+        if self.src.crystal().space_group:
+            self.src.crystal().space_group = 'P1'
+
+    def _pre_gjf(self):
+        """ Assign the Molecule charge before to dump to gjf file """
+        self._preprocess_for_gjf()
+
+    def _pre_gzmat(self):
+        self._preprocess_for_gjf()
+
+    def _io_dpmd_sys(self):
+        """ convert molecule information to numpy arrays """
+        return DeepSystem(self.src)
+
+    def _io_lmpmol(self):
+        """
+        write a molecule script
+        default values: coordinates, velocities, atom IDs and types
+        additional attributes for atomic: Bonds
+        additional attributes for full: Bonds + molecular + charge
+        """
+
+        def bonds(m):
+            """ Add bond body """
+            bond_str = 'Bonds' + '\n\n'  # bond body title
+
+            # the formula of bond_type key: atom1[bond_type]atom2
+            uni_bonds = tuple(m.unique_bonds)  # store bonds type
+            for j, bond in enumerate(m.bonds, 1):
+
+                bt_id = uni_bonds.index(bond) + 1
+                bond_str += f'{j} {bt_id} {bond.ob_atom1_id + 1} {bond.ob_atom2_id + 1}\n'
+
+            bond_str += '\n'
+
+            return bond_str
+
+        def charge():
+            """ Retrieve atom charge information """
+            charge_str = '\n' + 'Charges' + '\n\n'
+
+            for ic, a in enumerate(atoms_list, 1):  # ID of charge, atom
+                if isinstance(a, ci.Atom):
+                    charge_str += f'{ic} {a.partial_charge}\n'
+                else:
+                    assert isinstance(a, ci.PseudoAtom)
+                    charge_str += f'{ic} {a.charge}\n'
+
+            charge_str += '\n'
+
+            return charge_str
+
+        mol = self.src
+        kwargs = self.kwargs  # keywords arguments
+
+        # default values: coordinates, velocities, atom IDs and types;
+        # additional attributes for atomic: None;
+        # additional attributes for full: molecular + charge
+        atom_style = kwargs.get('atom_style', 'atomic')   # default atom_style is atomic
+        mol_name = kwargs.get('mol_name', mol.smiles)
+
+        # combine real atoms with pseudo atoms in a list
+        atoms_list = []
+        for m_a in mol.atoms:
+            atoms_list.append(m_a)
+
+        if mol.pseudo_atoms:   # determine if there are pseudo_atoms
+            for pse_a in mol.pseudo_atoms:
+                atoms_list.append(pse_a)
+
+        # title information
+        title = f"Create by hotpot package, convert from {mol_name}"
+        script = title + '\n\n'   # write the molecular script for lammps
+
+        # TODO: some header information missing
+        # Header partition
+        # add atom header
+        num_atoms = len(atoms_list)
+        num_atoms_str = f'{num_atoms}  atoms'
+        script += num_atoms_str + '\n'
+
+        # add bond header
+        num_bonds = len(mol.bonds)
+        num_bonds_str = f'{num_bonds}  bonds'
+        script += num_bonds_str + '\n'
+
+        # Add new blank line to end the header partition
+        script += '\n'
+
+        # Body partition
+        # Coords body
+        script += 'Coords' + '\n\n'
+        for i, atom in enumerate(atoms_list, 1):
+            script += f'{i}' + '  ' + '  '.join(map(str, atom.coordinates)) + '\n'
+        script += '\n'
+
+        # Types body
+        script += 'Types' + '\n\n'
+
+        dict_types = {}
+        for i, atom in enumerate(atoms_list, 1):
+            atom_type = dict_types.setdefault(atom.symbol, len(dict_types)+1)
+            script += f'{i} {atom_type}  # {atom.symbol}\n'
+
+        script += '\n'
+
+        # additional attributes
+        # to atomic style, only basis information (ID，Coords, types, velocitier)
+        if atom_style == 'atomic':
+            if num_bonds:
+                script += bonds(mol)
+
+        # to full style, basis information + molecular + charge
+        elif atom_style == 'full':
+            if num_bonds:
+                script += bonds(mol)
+            script += charge()
+
+        return script
+
+    def _post_gjf(self, script):
+        """ postprocess the dumped Gaussian 16 .gjf script to add the link0 and route context """
+        lines, _ = self._postprocess_for_gjf_head(script)
+        script = '\n'.join(lines)
+
+        # End black line
+        script += '\n\n'
+
+        return script
+
+    def _post_gzmat(self, script):
+        """ postprocess the dumped Gaussian 16 .gjf script to add the link0 and route content with Z-matrix """
+        lines, current_line = self._postprocess_for_gjf_head(script)
+        zmat = re.compile('\s+')
+
+        # Extract the symbol of atoms, bonds, angles and torsions
+        z_counts, atoms, var = 0, self.src.atoms, {}
+        while lines[current_line + z_counts].strip() != 'Variables:':
+            items = zmat.split(lines[current_line + z_counts])
+
+            assert items[0] == atoms[z_counts].symbol
+
+            if len(items) == 1:
+                assert not z_counts
+            elif len(items) == 3:
+                assert z_counts == 1
+                var[items[2]] = self.src.bond(z_counts, int(items[1])-1)
+            elif len(items) == 5:
+                assert z_counts == 2
+                var[items[2]] = self.src.bond(z_counts, int(items[1])-1)
+                var[items[4]] = self.src.angle(z_counts, int(items[1])-1, int(items[3])-1)
+            elif len(items) == 7:
+                var[items[2]] = self.src.bond(z_counts, int(items[1])-1)
+                var[items[4]] = self.src.angle(z_counts, int(items[1])-1, int(items[3])-1)
+                var[items[6]] = self.src.torsion(z_counts, int(items[1])-1, int(items[3])-1, int(items[5])-1)
+            else:
+                raise ValueError('Get an error string from Z-matrix')
+
+            z_counts += 1  # Next line
+
+        current_line += z_counts + 1  # update the current line
+        while lines[current_line].strip():
+            key, _ = lines[current_line].split('= ')
+            lines[current_line] += f" {var[key]['scan_step']}" if var[key]["scan_step"] else ''
+
+            current_line += 1
+
+        script = '\n'.join(lines)
+        # End black line
+        script += '\n\n'
+
+        return script
+
+    def _post_lmpdat(self, script: str):
+        """ post-process for LAMMPS data file """
+
+        title, headers, bodies = _parse_lmp_data_script(script)
+        script = title + '\n'
+
+        for ht, hvs in headers.items():
+            if ht == 'bond types':  # header title, header values
+                hvs[0] = len(self.src.unique_bonds)
+
+            script += ' '.join(map(str, hvs)) + ' ' + ht + '\n'
+
+        script += '\n' * 3
+
+        for bt, bcs in bodies.items():  # body title, body contents
+            if bt == 'Bonds':
+                bcs = self._process_lmpdat_bonds(bcs)
+
+            if bcs:  # if the body contents exist
+                script += bt + '\n' * 2
+                script += '\n'.join(bcs)
+                script += '\n' * 3
+
+        return script
+
+
+class Parser(IOBase, metaclass=MetaIO):
+    """ Parse the str or bytes obj to Molecule obj """
+    _pybel_fmt_convert = {
+        'g16log': 'g16'
+    }
+
+    def _open_source_to_string_lines(self, *which_allowed: str, output_type: Literal['lines', 'script'] = 'lines'):
+        """
+        Open the source file to string lines
+        Args:
+            which_allowed: which types of source are allowed to process to string lines
+
+        Returns:
+            (List of string|string)
+        """
+        src_type = self.result.get('src_type')
+        if src_type not in which_allowed:
+            raise RuntimeError(f'the source type {type(self.src)} have not been supported')
+        else:
+            if src_type == 'str':
+                script = self.src
+
+            elif src_type == 'path':
+                with open(self.src) as file:
+                    try:
+                        script = file.read()
+                    # If the file pointed by the path is not a text file
+                    # such as a bytes file
+                    except UnicodeDecodeError:
+                        raise IOEarlyStop()
+
+            elif src_type == 'IOString':
+                script = self.src.read()
+
+            else:
+                raise RuntimeError(f'the source type {type(self.src)} have not been supported')
+
+            if output_type == 'lines':
+                return script.split('\n')
+            elif output_type == 'script':
+                return script
+            else:
+                raise ValueError('the arg output_type given a wrong values, lines or script allow only')
+
+    def _checks(self) -> Dict[str, Any]:
+        if not isinstance(self.src, (IOBase, str, bytes, PathLike)):
+            raise TypeError(f'the parsed object should be IOBase, str or bytes, instead of {type(self.src)}')
+
+        if isinstance(self.src, str):
+            if os.path.exists(self.src):
+                return {'src_type': 'path'}
+            else:
+                return {'src_type': 'str'}
+
+        if isinstance(self.src, PathLike):
+            return {'src_type': 'path'}
+
+        if isinstance(self.src, bytes):
+            return {'src_type': 'bytes'}
+        if isinstance(self.src, io.StringIO):
+            return {'src_type': 'StringIO'}
+        if isinstance(self.src, io.BytesIO):
+            return {'src_type': 'BytesIO'}
+        if isinstance(self.src, io.FileIO):
+            return {'src_type': 'FileIO'}
+        print(f'the get source type is {type(self.src)}')
+        return {'src_type': type(self.src)}
+
+    def _ob_io(self):
+        """ IO by openbabel.pybel """
+        # Get the source type name
+        src_type = self.result.get('src_type')
+        try:
+            if src_type == 'str':
+                pybel_mol = pybel.readstring(self._pybel_fmt_convert.get(self.fmt, self.fmt), self.src)
+            elif src_type == 'path':
+                pybel_mol = next(pybel.readfile(self._pybel_fmt_convert.get(self.fmt, self.fmt), str(self.src)))
+            elif src_type == 'IOString':
+                pybel_mol = pybel.readstring(self._pybel_fmt_convert.get(self.fmt, self.fmt), self.src.read())
+            else:
+                raise RuntimeError(f'the source type {type(self.src)} have not been supported')
+
+            obj = ci.Molecule(pybel_mol.OBMol)
+
+        except RuntimeError:
+            obj = None
+
+        return obj
+
+    def _cclib_io(self, obj):
+        """ IO by cclib package """
+        src_type = self.result.get('src_type')
+
+        try:
+            if src_type == 'str':
+                data = cclib.ccopen(io.StringIO(self.src)).parse()
+            elif src_type == 'path':
+                data = cclib.ccopen(self.src).parse()
+            elif src_type == 'IOString':
+                data = cclib.ccopen(self.src).parse()
+            else:
+                raise RuntimeError(f'the source type {type(self.src)} have not been supported in cclib')
+
+        except (RuntimeError, AttributeError):
+            data = None
+
+        if data:
+            if not obj:
+                # when get information about the atoms species
+                if hasattr(data, 'atomnos'):
+                    atoms_attrs = [{'atomic_number': an} for an in getattr(data, 'atomnos')]
+                    obj = ci.Molecule(atoms=atoms_attrs)
+                else:
+                    print(IOError(f'the parsing of {self.src} is not successful!'))
+                    return obj  # Return None
+
+            # if get information about the coordination collections
+            if hasattr(data, 'atomcoords'):
+                obj.set(all_coordinates=getattr(data, 'atomcoords'))
+
+            # if get information about the energy (SCF energies) vector
+            if hasattr(data, 'scfenergies'):
+                obj.set(all_energy=getattr(data, 'scfenergies'))
+
+        return obj
+
+    def _io(self, *args, **kwargs):
+        """ Standard IO process """
+        # Try parse the log file by openbabel.pybel file firstly
+        return self._ob_io()
+
+    # Start to the prefix IO functions
+
+    # preprocess for g16log file
+    # This preprocess is used to judge whether a Error happened when perform g16 calculate
+    def _pre_g16log(self):
+        """ g16log preprocess to judge whether some Error happened """
+        def is_convergence_failure():
+            if 'Convergence failure -- run terminated.' in script:
+                return True
+            return False
+
+        def is_hessian_no_longer_linear_valid():
+            march_pattern = re.compile(r'Error termination via Lnk1e in (/.+)*/l103\.exe')
+
+            if any(march_pattern.match(line.strip()) for line in script.splitlines()[-5:]):
+                return True
+            return False
+
+        script = self._open_source_to_string_lines('str', 'path', "IOString", output_type='script')
+
+        try:
+            # Check whether a failure have happened when calculation.
+            if is_convergence_failure():
+                raise IOEarlyStop('Gaussian16 SCF cannot convergence!')
+            if is_hessian_no_longer_linear_valid():
+                raise IOEarlyStop('Gaussian16 Hessian no longer linear valid')
+
+        except IOEarlyStop as error:
+            if self.kwargs.get('force'):
+                print(error)
+            else:
+                raise error
+
+    # Parse the XYZ file
+    def _io_xyz(self):
+        """ Parse the XYZ file """
+        src_type = self.result['src_type']
+        if src_type != 'path':
+            return self._io()
+        else:
+            from ase import io
+            from openbabel import openbabel as ob
+            data_generator = io.iread(self.src)
+
+            # atomic_numbers, coordinates, cell_params
+            atomic_numbers, all_coordinates, cell_matrix = [], [], None
+            for data in data_generator:
+                atomic_numbers.append(data.numbers)
+                all_coordinates.append(data.positions)
+                if cell_matrix is None:
+                    cell_matrix = data.cell.array
+
+            atomic_numbers = np.stack(atomic_numbers)
+            all_coordinates = np.stack(all_coordinates)
+
+            number_min = atomic_numbers.min(axis=0)
+            number_max = atomic_numbers.max(axis=0)
+
+            # the values in same columns should be same.
+            assert all(number_max == number_min)
+
+            obj = ci.Molecule()
+            obj.quick_build_atoms(number_min)
+
+            obj.set(all_coordinates=all_coordinates)
+            obj.set(crystal=cell_matrix)
+            obj.conformer_select(0)
+
+            return obj
+
+    # postprocess for g16log file
+    def _post_g16log(self, obj: 'ci.Molecule'):
+        """
+        post process for g16log format, to extract:
+            1) Mulliken charge
+            2) Spin densities
+        """
+        def extract_charges_spin():
+            """ Extract charges and spin information from g16.log file """
+            # Get the line index of Mulliken charges
+            head_lines = [i for i, line in enumerate(lines) if line.strip() == 'Mulliken charges and spin densities:']
+            if not head_lines:
+                head_lines = [i for i, line in enumerate(lines) if line.strip() == 'Mulliken charges:']
+                charge_only = True
+            else:
+                charge_only = False
+
+            # Skip the first charge&spin sheet, it can't find corresponding coordinates
+            if not head_lines:
+                raise IOEarlyStop
+            elif len(head_lines) == obj.conformer_counts + 1:
+                head_lines = head_lines[1:]
+
+            # Extract the Mulliken charge and spin densities
+            charges, spin_densities = [], []  # changes(cgs) spin_densities(sds)
+            for i in head_lines:
+                # Enhance inspection
+                col_heads = lines[i + 1].strip().split()
+                if charge_only:
+                    assert len(col_heads) == 1 and col_heads[0] == '1'
+                else:
+                    assert len(col_heads) == 2 and col_heads[0] == '1' and col_heads
+
+                HEAD_LINES_NUM = 2
+                cg, sd = [], []  # change, spin_density
+
+                while True:
+                    split_line = lines[i + HEAD_LINES_NUM].strip().split()
+                    if charge_only and len(split_line) == 3:
+                        row, syb, c = split_line  # row number, symbol, charges
+                        s = 0.0  # spin density
+                    elif not charge_only and len(split_line) == 4:
+                        row, syb, c, s = split_line  # row number, symbol, charges, spin density
+                    else:
+                        break
+
+                    try:
+                        row, c, s = int(row), float(c), float(s)
+                        # check the sheet row number
+                        if row != HEAD_LINES_NUM - 1:
+                            break
+
+                    # Inspect the types of values
+                    except ValueError:
+                        break
+
+                    # record the charge and spin density
+                    cg.append(c)
+                    sd.append(s)
+                    HEAD_LINES_NUM += 1
+
+                # store the extracted
+                if cg and sd:
+                    if len(cg) == len(sd) == len(obj.atoms):
+                        charges.append(cg)
+                        spin_densities.append(sd)
+                    else:
+                        raise ValueError('the number of charges do not match to the number of atoms')
+                else:
+                    raise ValueError('get a empty charge and spin list, check the input!!')
+
+            obj.set(all_atom_charges=np.array(charges))
+            obj.set(all_atom_spin_densities=np.array(spin_densities))
+                
+        def extract_force_matrix():
+            # Define the format of force sheet
+            # the Force sheet like this:
+            #  -------------------------------------------------------------------
+            #  Center     Atomic                   Forces (Hartrees/Bohr)
+            #  Number     Number              X              Y              Z
+            #  -------------------------------------------------------------------
+            #       1        8           0.039901671    0.000402574    0.014942530
+            #       2        8           0.017381613    0.001609531    0.006381231
+            #       3        6          -0.092853735   -0.025654844   -0.005885898
+            #       4        6           0.067801154    0.024130172   -0.022794721
+            #       5        8          -0.023702905    0.005486251   -0.004938175
+            #       6        8          -0.006359715   -0.008543465    0.010350815
+            #       7       55          -0.002168084    0.002569781    0.001944217
+            #  -------------------------------------------------------------------
+            force_head1 = re.compile(r'\s*Center\s+Atomic\s+Forces\s\(Hartrees/Bohr\)\s*')
+            force_head2 = re.compile(r'\s*Number\s+Number\s+X\s+Y\s+Z\s*')
+            sheet_line = re.compile(r'\s*----+\s*')
+
+            HEAD_LINES_NUM = 3  # the offset line to write the header
+
+            head_lines = [i for i, line in enumerate(lines) if force_head1.match(line)]
+
+            all_forces = []
+            for i in head_lines:
+                # enhance the inspection of Force sheet head
+                assert force_head2.match(lines[i + 1])
+                assert sheet_line.match(lines[i + 2])
+
+                rows = 0
+                forces = []
+                while True:
+
+                    if sheet_line.match(lines[i + HEAD_LINES_NUM + rows]):
+                        if len(forces) == obj.atom_counts:
+                            all_forces.append(forces)
+                            break
+                        else:
+                            raise ValueError('the number of force vector do not match the number of atoms')
+
+                    ac, an, x, y, z = map(
+                        lambda v: int(v[1]) if v[0] < 2 else float(v[1]),
+                        enumerate(lines[i + HEAD_LINES_NUM + rows].split())
+                    )
+
+                    # Enhance the inspection
+                    assert ac == rows + 1
+                    if obj.atoms[rows].atomic_number != an:
+                        raise ValueError('the atomic number do not match')
+
+                    forces.append([x, y, z])
+
+                    rows += 1
+
+            try:
+                obj.set(all_forces=np.array(all_forces))
+            except ValueError:
+                return
+
+        obj = self._cclib_io(obj)  # Try to supplementary Molecule data by cclib
+
+        lines = self._open_source_to_string_lines('str', 'path', 'IOString')
+
+        try:  # TODO: For now, this is the case, the spin densities may lost in some case  # the units is Hartree/Bohr
+            extract_charges_spin()
+        except IOEarlyStop:
+            if self.kwargs.get('must_have_charge'):
+                raise IOEarlyStop
+
+        try:
+            extract_force_matrix()
+        except IndexError:
+            raise IOEarlyStop
+
+        # assign the first conformer for the molecule
+        obj.conformer_select(0)
+
+        return obj
+
+
```

### Comparing `hotpot-zzy-0.3.0.9/hotpot/bundle.py` & `hotpot-zzy-0.3.1.0/hotpot/bundle.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,649 +1,668 @@
-"""
-python v3.7.9
-@Project: hotpot
-@File   : bundle.py
-@Author : Zhiyuan Zhang
-@Date   : 2023/3/22
-@Time   : 3:18
-"""
-import copy
-import os
-import random
-import time
-from os import PathLike
-from typing import *
-from pathlib import Path
-import numpy as np
-from tqdm import tqdm
-from openbabel import pybel as pb
-import hotpot.cheminfo as ci
-from hotpot.tools import check_path
-import multiprocessing as mp
-
-feature_formats = {
-    'basic': ['atomic_number', 's', 'p', 'f']
-}
-
-# the dict to store all defined bundle classes
-_bundle_classes = {}
-
-
-def register_bundles(bundle: Type):
-    """ register the bundle to _bundle_classes """
-    _bundle_classes[bundle.__name__] = bundle
-    return bundle
-
-
-@register_bundles
-class MolBundle:
-    """ The basic class for all molecular bundle """
-
-    def __init__(self, mols: Union[Sequence[ci.Molecule], Generator[ci.Molecule, None, None]] = None):
-        self._data = {'mols': mols}
-
-    def __repr__(self):
-        class_name = self.__class__.__name__
-        return f"{class_name}(generator)" if isinstance(self.mols, Generator) else f"{class_name}({self.mols})"
-
-    def __iter__(self):
-        return iter(self.mols)
-
-    def __add__(self, other: Union['MolBundle', ci.Molecule]):
-        """"""
-        if isinstance(other, MolBundle):
-            return MolBundle(self.to_list() + other.to_list())
-        elif isinstance(other, ci.Molecule):
-            return MolBundle(self.to_list() + [other])
-        else:
-            raise TypeError('the MolBundle is only allowed to add with Molecule or MolBundle object')
-
-    def __len__(self):
-        return len(self.mols)
-
-    def __getitem__(self, item: int):
-        return self.mols[item]
-
-    def __get_all_unique_attrs(self, attr_name: str):
-        """ Given a Molecule attr_name, get all unique values of the attributes among all Molecule in the MolBundle"""
-        if self.is_generator:
-            self.to_list()
-
-        dict_attrs = {}
-        for i, mol in enumerate(self):
-            list_indices = dict_attrs.setdefault(getattr(mol, attr_name), [])
-            list_indices.append(i)
-
-        if not dict_attrs:
-            return 0
-        if len(dict_attrs) == 1:
-            return getattr(self.mols[0], attr_name)
-        else:
-            return dict_attrs
-
-    @property
-    def atom_counts(self) -> Dict[int, List[int]]:
-        """
-        Notes:
-            if the Bundle is a generator, convert to a list of Molecule first.
-        Returns:
-            returns a dict with the key is the number of the atoms and the key is the indices of Molecules
-        """
-        return self.__get_all_unique_attrs('atom_counts')
-
-    @property
-    def atomic_numbers(self):
-        return self.__get_all_unique_attrs('atomic_numbers')
-
-    def choice(
-            self, size: int = 1, replace: bool = True,
-            p: Union[Sequence, float, Callable] = None,
-            get_remain: bool = False
-    ) -> Union['MolBundle', tuple['MolBundle', 'MolBundle']]:
-        """
-         Generate new MolBundle with a list of random Molecule objects from the current MolBundle
-        Args:
-            size: the size of generating MolBundle, that the number of contained Molecule objects
-            replace: whether allow to choice a Molecule object multiply times. It must be noted that
-             if this MolBundle is a generator or the get_remain arg has been specified, this arg
-             would not work.
-            p: If the current MolBundle is a Generator it should be a float or a Callable object
-             which arg is the generated molecule. If the current MolBundle is a Sequence, the p
-             should bea sequence with same size as the number of Molecule objects in current
-             MolBundle, specify the probability of each Molecule to be chosen.
-            get_remain: whether to get the remain Molecule object, if the current MolBundle is a Generator
-             this arg would not work
-
-        Return:
-            MolBundle contained specified-number molecules
-        """
-        def choice_from_generator():
-            """ Generator molecule according to specified probability """
-            if isinstance(p, float):
-                for mol in self:
-                    if random.choices([0, 1], [1-p, p]):
-                        yield mol
-
-            if isinstance(p, Callable):
-                for mol in self:
-                    if p(mol):
-                        yield mol
-
-        # if the MolBundle is a generator, the derivative one is still generator
-        if self.is_generator:
-            if isinstance(p, (float, Callable)):
-                return MolBundle(choice_from_generator())
-            else:
-                raise TypeError('When the MolBundle is a generator, the p should be a float or Callable object')
-
-        elif get_remain:  # get remain molecules as the second return
-            mol_indices = np.arange(len(self))
-            chosen_idx = np.random.choice(mol_indices, size=int(len(self) * p))
-            remain_idx = np.setdiff1d(mol_indices, chosen_idx)
-
-            chosen_mol = np.array(self.mols)[chosen_idx].tolist()
-            remain_mol = np.array(self.mols)[remain_idx].tolist()
-
-            return self.__class__(chosen_mol), self.__class__(remain_mol)
-
-        else:
-            return self.__class__(np.random.choice(self.mols, size=size, replace=replace, p=p))
-
-    @property
-    def data(self):
-        return self._data
-
-    @data.setter
-    def data(self, data):
-        if isinstance(data, dict):
-            self._data = data
-        else:
-            raise TypeError(f'the {self.__class__.__name__}.data must be a dict')
-
-    @classmethod
-    def read_from(
-            cls, fmt: str,
-            dir_or_strings: Union[str, PathLike, Iterable[str]],
-            match_pattern: str = '*',
-            generate: bool = False,
-            ranges: Union[Sequence[int], range] = None,
-            condition: Callable = None,
-            num_proc: int = None
-    ):
-        """
-        Read Molecule objects from a directory.
-
-        Args:
-            fmt(str): read file with the specified-format method.
-            dir_or_strings(str|PathLike): the directory all file put, or a sequence of string
-            match_pattern(str): the file name pattern
-            generate(bool): read file to a generator of Molecule object
-            ranges(Sequence[int]|range): A list or range of integers representing the indices of
-                the input files to read. Defaults to None.
-            condition(Callable): A callable object that takes two arguments (the path of the input file
-                and the corresponding Molecule object) and returns a boolean value indicating whether to include the
-                Molecule object in the output. Defaults to None.
-            num_proc: the number of process to read
-
-        Returns:
-            List(Molecule) or Generator(Molecule)
-        """
-        def read_mol(pm: Path, conn):
-
-            try:
-                mol = ci.Molecule.read_from(pm, fmt)
-
-                # the OBMol, OBAtom, OBBond are C++ objects wrapped by SWIG,
-                # they can't be pickle, so pop them from Molecule and convert their info to .mol2 string
-                pmol = pb.Molecule(mol.ob_mol_pop())
-                script = pmol.write('mol2')  # Write to the mol2 script to allow it to pickle
-
-                # communicate with the main process
-                conn.send((mol, script, pm))
-
-            except AttributeError:
-                conn.send((None, None, pm))
-
-            except StopIteration:
-                conn.send((None, None, pm))
-
-        def mol_generator():
-            nonlocal dir_or_strings
-            for i, path_mol in enumerate(generate_path_or_string()):
-
-                if not ranges or i in ranges:
-                    try:
-                        mol = ci.Molecule.read_from(path_mol, fmt)
-                    except StopIteration:
-                        mol = None
-                else:
-                    continue
-
-                if mol and (not condition or condition(path_mol, mol)):
-                    yield mol
-
-        def mol_mp_generator():
-            mols_info = []
-
-            parent_conn, child_conn = mp.Pipe()
-            ps = []  # list of Process: Queue pairs
-
-            for i, source in enumerate(generate_path_or_string()):
-
-                # if the number of process more than num_proc, get the read molecule info and stop to start new process
-                while len(ps) >= num_proc:
-                    for p in ps:
-                        if not p.is_alive():
-                            mols_info.append(parent_conn.recv())
-                            p.terminate()
-                            ps.remove(p)
-
-                # When received some Molecule info, reorganize these info and yield
-                while mols_info:
-                    mol, script, pf = mols_info.pop()  # hotpot Molecule, mol2_script, path_file of Molecule
-
-                    # If you get a valid Molecule info, re-wrap to be hotpot Molecule
-                    if mol and script:
-                        pmol = pb.readstring('mol2', script)  # pybel Molecule object
-                        mol.ob_mol_rewrap(pmol.OBMol)  # re-wrap OBMol by hotpot Molecule
-
-                        # if the reorganized Molecule is expected, yield
-                        if not condition or condition(mol, pf):
-                            yield mol
-
-                # Start new process to read Molecule from file
-                if not ranges or i in ranges:
-                    p = mp.Process(target=read_mol, args=(source, child_conn))
-                    p.start()
-                    ps.append(p)
-
-            # After all path_file have pass into process to read
-            while ps:
-                for p in ps:
-                    if not p.is_alive():
-                        mols_info.append(parent_conn.recv())
-                        p.terminate()
-                        ps.remove(p)
-
-            for mol, script, pf in mols_info:
-                # if get a valid Molecule info, re-wrap to be hotpot Molecule
-                if mol and script:
-                    pmol = pb.readstring('mol2', script)  # pybel Molecule object
-                    mol.ob_mol_rewrap(pmol.OBMol)  # re-wrap OBMol by hotpot Molecule
-
-                    # if the reorganized Molecule is expected, yield
-                    if not condition or condition(mol, pf):
-                        yield mol
-
-        def generate_path_or_string():
-            """"""
-            if isinstance(dir_or_strings, Path):
-                for path in dir_or_strings.glob(match_pattern):
-                    yield path
-
-            elif isinstance(dir_or_strings, Iterable):
-                for string in dir_or_strings:
-                    yield string
-
-            else:
-                raise TypeError(f'the dir_or_strings is required to be a Path or str, get {type(dir_or_strings)}')
-
-        if isinstance(dir_or_strings, str):
-            dir_or_strings = Path(dir_or_strings)
-        elif not isinstance(dir_or_strings, PathLike) and not isinstance(dir_or_strings, Iterable):
-            raise TypeError(
-                f'the read_dir should be a str, PathLike or iterable str, instead of {type(dir_or_strings)}'
-            )
-
-        generator = mol_mp_generator() if num_proc else mol_generator()
-
-        if generate:
-            return cls(generator)
-        else:
-            return cls([m for m in tqdm(generator, 'reading molecules')])
-
-    def gcmc_for_isotherm(
-            self, *guest: 'ci.Molecule', force_field: Union[str, PathLike] = None,
-            work_dir: Union[str, PathLike] = None, T: float = 298.15,
-            Ps: Sequence[float] = (1.0,), procs: int = 1, named_identifier: bool = False,
-            **kwargs
-    ):
-        """
-        Run gcmc to determine the adsorption of guest,
-        Args:
-            self: the framework as the sorbent of guest molecule
-            guest(Molecule): the guest molecule to be adsorbed into the framework
-            force_field(str|PathLike): the path to force field file or the self-existent force file contained
-             in force field directory (in the case, a str should be given as a relative path from the root of
-             force field root to the specified self-existent force filed). By default, the force field is UFF
-             which in the relative path 'UFF/LJ.json' for the force field path.
-            work_dir: the user-specified dir to store the result of GCMC and log file.
-            T: the environmental temperature (default, 298.15 K)
-            Ps(Sequence[float]): A sequence of relative pressure related to the saturation vapor in the environmental temperature.
-            procs(int): the number of processes, default 1.
-            named_identifier: Whether to name the dir by the identifier of frames
-        """
-        if isinstance(work_dir, str):
-            work_dir = Path(work_dir)
-
-        # Assemble keywords arguments for multiprocess
-        processes = []
-        for i, frame in enumerate(self.mols, 1):
-
-            # When the running proc more than the specified values, waiting for terminate
-            while len(processes) >= procs:
-                for p in processes:
-                    if not p.is_alive():
-                        processes.pop(processes.index(p))
-                        p.terminate()
-
-                time.sleep(10)
-
-            if named_identifier:
-                sub_work_dir = work_dir.joinpath(frame.identifier)
-            else:
-                idt_map = self._data.setdefault('identifier_map', {})
-                idt_map[i] = frame.identifier
-                sub_work_dir = work_dir.joinpath('mol_' + str(i))
-
-            if not sub_work_dir.exists():
-                sub_work_dir.mkdir()
-
-            kwargs.update({
-                'force_field': force_field,
-                'work_dir': sub_work_dir,
-                'T': T, 'Ps': Ps
-            })
-
-            p = mp.Process(target=frame.gcmc_for_isotherm, args=guest, kwargs=kwargs)
-
-            p.start()
-            processes.append(p)
-
-        for p in processes:
-            p.join()
-            p.terminate()
-
-        return self._data.get('identifier_map')
-
-    def graph_representation(self, *feature_names) -> Generator[Union[str, np.ndarray, np.ndarray], None, None]:
-        """ Transform molecules to their graph representation """
-        for mol in self.mols:
-            yield mol.graph_representation(*feature_names)
-
-    def gaussian(
-            self, g16root: Union[str, PathLike], dir_out: Union[str, PathLike],
-            link0: Union[str, List[str]], route: Union[str, List[str]],
-            dir_err: Optional[Union[str, PathLike]] = None,
-            dir_chk: Optional[Union[str, PathLike]] = None,
-            clean_conformers: bool = True,
-            perturb_kwargs: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
-            *args, **kwargs
-    ) -> None:
-        """
-        Run Gaussian16 calculations for Molecule objects stored in the MolBundle.
-        These Molecules are allowed to be perturbed their atoms' coordinates before submit to Gaussian 16
-
-        Args:
-            g16root (Union[str, PathLike]): The path to the Gaussian16 root directory.
-            dir_out (Union[str, PathLike]): The path to the directory to output the log files.
-            link0 (Union[str, List[str]]): The link0 information for Gaussian16 calculations.
-            route (Union[str, List[str]]): The route information for Gaussian16 calculations.
-            dir_err (Optional[Union[str, PathLike]], optional): The path to the directory to output the error files.
-                Defaults to None.
-            dir_chk (Optional[Union[str, PathLike]], optional): The path to the directory to store the .chk files.
-                Defaults to None.
-            clean_conformers (bool, optional): A flag indicating whether to clean the configuration before perturbing
-                the molecule or lattice. Defaults to True.
-            perturb_kwargs (Optional[Union[Dict[str, Any], List[Dict[str, Any]]]], optional): The parameters for
-                perturbing the molecule or lattice. Defaults to None.
-            *args: Additional positional arguments.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            None
-        """
-        # Check and process paths
-        g16root: Path = check_path(g16root, file_or_dir='dir')
-        dir_out: Path = check_path(dir_out, mkdir=True)
-        dir_err: Optional[Path] = check_path(dir_err, mkdir=True)
-        dir_chk: Optional[Path] = check_path(dir_chk, mkdir=True)
-
-        for mol in self.mols:
-            assert isinstance(mol, ci.Molecule)
-
-            # Clean before perturb conformers
-            if clean_conformers:
-                mol.clean_conformers()
-
-            # Assign the dirs
-            # assign the dir to put out.log files for the mol
-            dir_out_mol = dir_out.joinpath(mol.identifier)
-            if not dir_out_mol.exists():
-                dir_out_mol.mkdir()
-
-            # assign the dir to put err.log files for the mol
-            if dir_err:
-                dir_err_mol = dir_err.joinpath(mol.identifier)
-                if not dir_err_mol.exists():
-                    dir_err_mol.mkdir()
-            else:
-                dir_err_mol = None
-
-            # Performing the molecule or lattice perturb
-            if isinstance(perturb_kwargs, Dict):
-                perturb_kwargs = [perturb_kwargs]  # Wrap it into a list
-
-            if isinstance(perturb_kwargs, List) and all(isinstance(pk, dict) for pk in perturb_kwargs):
-                for pk in perturb_kwargs:
-                    pk['inplace'] = True  # Force to inplace
-                    mol.perturb_atoms_coordinates(**pk)
-            elif perturb_kwargs is not None:
-                ValueError('The perturb_kwargs should be a dict or list of dict')
-
-            # Running the gaussian16
-            for config_idx in range(mol.conformer_counts):
-                mol.conformer_select(config_idx)
-
-                # Reorganize the arguments for each conformer
-                path_out = dir_out_mol.joinpath(f'{config_idx}.log')
-                path_err = dir_err_mol.joinpath(f'{config_idx}.err') if dir_err else None
-
-                if dir_chk:  # for dir_chk
-                    dir_chk_mol = dir_chk.joinpath(mol.identifier)
-                    dir_chk_mol.mkdir(exist_ok=True)
-
-                    if isinstance(link0, str):
-                        link0_cfg = [f'chk={str(dir_chk_mol)}/{config_idx}.chk', link0]
-                    elif isinstance(link0, list):
-                        link0_cfg = copy.copy(link0)
-                        link0_cfg.insert(0, f'chk={str(dir_chk_mol)}/{config_idx}.chk')
-                    else:
-                        TypeError('the link0 should be str or list of str!')
-                else:
-                    link0_cfg = link0
-
-                mol.gaussian(
-                    g16root=g16root,
-                    link0=link0_cfg,
-                    route=route,
-                    path_log_file=str(path_out.absolute()),
-                    path_err_file=str(path_err) if path_err else None,
-                    *args, **kwargs
-                )
-
-    @property
-    def is_generator(self):
-        """ To judge weather the object is a Molecule generator """
-        return isinstance(self.mols, Generator)
-
-    @property
-    def mols(self):
-        return self._data.get('mols', [])
-
-    @mols.setter
-    def mols(self, mols):
-        self._data['mols'] = mols
-
-    @staticmethod
-    def registered_bundle_names():
-        """ Return all registered bundle names """
-        return list(_bundle_classes.keys())
-
-    def to(self, bundle_name: str):
-        """ Convert this bundle to other bundle type """
-        return _bundle_classes[bundle_name](self.mols)
-
-    def to_list(self) -> List[ci.Molecule]:
-        """ Convert the molecule container (self.mol) to list """
-        if isinstance(self.mols, Generator):
-            self.mols = list(self)
-
-        return self.mols
-
-    def unique_mols(self, mode: Literal['smiles', 'similarity'] = 'smiles'):
-        """
-        get a new Bundle with all unique Molecule objects
-        Args:
-            mode: the standard to identify whether two molecule to be regard as identical
-
-        Returns:
-            A new Bundle with all the unique Molecule objects
-        """
-        clone = copy.copy(self)
-        clone.data = copy.copy(self.data)
-        if mode == 'smiles':
-            clone.mols = ({m.smiles: m for m in self.mols}.values())
-            return clone
-        elif mode == 'similarity':
-            dict_mols = {}
-            for mol in self.mols:
-                mols_with_same_atom_num = dict_mols.setdefault(mol.atom_counts, [])
-                mols_with_same_atom_num.append(mol)
-
-            new_mols = []
-            for _, mols_with_same_atom_num in dict_mols.items():
-                uni_mols = []
-                for mol in mols_with_same_atom_num:
-                    if mol not in uni_mols:
-                        uni_mols.append(mol)
-
-                new_mols.extend(uni_mols)
-
-            clone.mols = new_mols
-
-            return clone
-
-
-@register_bundles
-class DeepModelBundle(MolBundle):
-    """ Specific MolBundle to carry out the tasks in DeepModeling packages """
-
-    def merge_conformers(self):
-        """
-        Get the sum of conformers for all molecule in the mol bundle "self.mols"
-        This method can only be successfully executed
-        when all molecules in the molecular bundle can be added to each other
-        Returns:
-            a Molecule object with all conformers in the self.mols
-        """
-        atomic_numbers = self.atomic_numbers
-
-        if isinstance(atomic_numbers, tuple):
-            return sum(self.mols[1:], start=self.mols[0])
-        elif isinstance(atomic_numbers, dict):
-            mol_array = np.array(self.mols)
-            return self.__class__([mol_array[i].sum() for ans, i in self.atomic_numbers.items()])
-
-    def merge_atoms_same_mols(self) -> 'DeepModelBundle':
-        """ Merge Molecules with same atoms to a MixSameAtomMol """
-        bundle: DeepModelBundle = self.to_mix_mols()
-        atom_counts = bundle.atom_counts
-
-        if isinstance(atom_counts, tuple):
-            return sum(bundle.mols[1:], start=bundle.mols[0])
-        elif isinstance(atom_counts, dict):
-            mol_array = np.array(bundle.mols)
-            return self.__class__([mol_array[i].sum() for ans, i in atom_counts.items()])
-
-    def to_dpmd_sys(
-            self, system_dir: Union[str, os.PathLike],
-            validate_ratio: float,
-            mode: Literal['std', 'att'] = 'std',
-            split_mode: Optional[Literal['inside', 'outside']] = None
-    ):
-        """"""
-        def to_files(mb: MolBundle, save_root: Path):
-            for c, m in enumerate(mb):  # c: counts, m: molecule
-                mol_save_root = \
-                    save_root.joinpath(str(m.atom_counts)) if mode == 'att' else system_dir.joinpath(str(c))
-                if not mol_save_root.exists():
-                    mol_save_root.mkdir()
-
-                m.to_dpmd_sys(mol_save_root, mode)
-
-        if split_mode and split_mode not in ['inside', 'outside']:
-            raise ValueError("the split_mode must be 'inside' or 'outside'")
-
-        if not 0.0 < validate_ratio < 1.0:
-            raise ValueError('the validate_ratio must be from 0.0 to 1.0')
-
-        # Organize dirs
-        if not isinstance(system_dir, Path):
-            system_dir = Path(system_dir)
-        training_dir = system_dir.joinpath('training_data')
-        validate_dir = system_dir.joinpath('validate_data')
-        if not training_dir.exists():
-            training_dir.mkdir()
-        if not validate_dir.exists():
-            validate_dir.mkdir()
-
-        if mode == 'att':
-            bundle = self.merge_atoms_same_mols()
-            if not split_mode:
-                split_mode = 'inside'
-
-        elif mode == 'std':
-            bundle = copy.copy(self)
-            if not split_mode:
-                split_mode = 'outside'
-
-        else:
-            raise ValueError("the mode is only allowed to be 'att' or 'std'!")
-
-        if split_mode == 'inside':
-            for i, mol in enumerate(bundle):
-                mol_training_dir = \
-                    training_dir.joinpath(str(mol.atom_counts)) if mode == 'att' else system_dir.joinpath(str(i))
-                mol_validate_dir = \
-                    validate_dir.joinpath(str(mol.atom_counts)) if mode == 'att' else system_dir.joinpath(str(i))
-
-                if not mol_training_dir.exists():
-                    mol_training_dir.mkdir()
-                if not mol_validate_dir.exists():
-                    mol_validate_dir.mkdir()
-
-                mol.to_dpmd_sys(mol_training_dir, mode, validate_ratio, mol_validate_dir)
-
-        elif split_mode == 'outside':
-            validate_bundle, training_bundle = bundle.choice(p=validate_ratio, get_remain=True)
-
-            # Save to files
-            to_files(training_bundle, training_dir)
-            to_files(validate_bundle, validate_dir)
-
-    def to_mix_mols(self):
-        """
-        Return a new MolBundle, in which Molecule objects in container are converted to MixSameAtomMol
-        Returns:
-            MolBundle(MixSameAtomMol)
-        """
-        return self.__class__([m.to_mix_mol() if not isinstance(m, ci.MixSameAtomMol) else m for m in self])
-
-    def to_mols(self):
-        """
-        Return a new MolBundle, in which MixSameAtomMol objects in container are converted to Molecule
-        Returns:
-            MolBundle(Molecule)
-        """
-        return self.__class__([m.to_mol() if isinstance(m, ci.MixSameAtomMol) else m for m in self])
-
+"""
+python v3.7.9
+@Project: hotpot
+@File   : bundle.py
+@Author : Zhiyuan Zhang
+@Date   : 2023/3/22
+@Time   : 3:18
+"""
+import copy
+import os
+import random
+import time
+from os import PathLike
+from typing import *
+from pathlib import Path
+import numpy as np
+from tqdm import tqdm
+from openbabel import pybel as pb
+import hotpot.cheminfo as ci
+from hotpot.tools import check_path
+import multiprocessing as mp
+
+feature_formats = {
+    'basic': ['atomic_number', 's', 'p', 'f']
+}
+
+# the dict to store all defined bundle classes
+_bundle_classes = {}
+
+
+def register_bundles(bundle: Type):
+    """ register the bundle to _bundle_classes """
+    _bundle_classes[bundle.__name__] = bundle
+    return bundle
+
+
+@register_bundles
+class MolBundle:
+    """ The basic class for all molecular bundle """
+
+    def __init__(self, mols: Union[Sequence[ci.Molecule], Generator[ci.Molecule, None, None]] = None):
+        self._data = {'mols': mols}
+
+    def __repr__(self):
+        class_name = self.__class__.__name__
+        return f"{class_name}(generator)" if isinstance(self.mols, Generator) else f"{class_name}({self.mols})"
+
+    def __iter__(self):
+        return iter(self.mols)
+
+    def __add__(self, other: Union['MolBundle', ci.Molecule]):
+        """"""
+        if isinstance(other, MolBundle):
+            return MolBundle(self.to_list() + other.to_list())
+        elif isinstance(other, ci.Molecule):
+            return MolBundle(self.to_list() + [other])
+        else:
+            raise TypeError('the MolBundle is only allowed to add with Molecule or MolBundle object')
+
+    def __len__(self):
+        return len(self.mols)
+
+    def __getitem__(self, item: int):
+        return self.mols[item]
+
+    def __get_all_unique_attrs(self, attr_name: str):
+        """ Given a Molecule attr_name, get all unique values of the attributes among all Molecule in the MolBundle"""
+        if self.is_generator:
+            self.to_list()
+
+        dict_attrs = {}
+        for i, mol in enumerate(self):
+            list_indices = dict_attrs.setdefault(getattr(mol, attr_name), [])
+            list_indices.append(i)
+
+        if not dict_attrs:
+            return 0
+        if len(dict_attrs) == 1:
+            return getattr(self.mols[0], attr_name)
+        else:
+            return dict_attrs
+
+    @property
+    def atom_counts(self) -> Dict[int, List[int]]:
+        """
+        Notes:
+            if the Bundle is a generator, convert to a list of Molecule first.
+        Returns:
+            returns a dict with the key is the number of the atoms and the key is the indices of Molecules
+        """
+        return self.__get_all_unique_attrs('atom_counts')
+
+    @property
+    def atomic_numbers(self):
+        return self.__get_all_unique_attrs('atomic_numbers')
+
+    def choice(
+            self, size: int = 1, replace: bool = True,
+            p: Union[Sequence, float, Callable] = None,
+            get_remain: bool = False
+    ) -> Union['MolBundle', tuple['MolBundle', 'MolBundle']]:
+        """
+         Generate new MolBundle with a list of random Molecule objects from the current MolBundle
+        Args:
+            size: the size of generating MolBundle, that the number of contained Molecule objects
+            replace: whether allow to choice a Molecule object multiply times. It must be noted that
+             if this MolBundle is a generator or the get_remain arg has been specified, this arg
+             would not work.
+            p: If the current MolBundle is a Generator it should be a float or a Callable object
+             which arg is the generated molecule. If the current MolBundle is a Sequence, the p
+             should bea sequence with same size as the number of Molecule objects in current
+             MolBundle, specify the probability of each Molecule to be chosen.
+            get_remain: whether to get the remain Molecule object, if the current MolBundle is a Generator
+             this arg would not work
+
+        Return:
+            MolBundle contained specified-number molecules
+        """
+        def choice_from_generator():
+            """ Generator molecule according to specified probability """
+            if isinstance(p, float):
+                for mol in self:
+                    if random.choices([0, 1], [1-p, p]):
+                        yield mol
+
+            if isinstance(p, Callable):
+                for mol in self:
+                    if p(mol):
+                        yield mol
+
+        # if the MolBundle is a generator, the derivative one is still generator
+        if self.is_generator:
+            if isinstance(p, (float, Callable)):
+                return MolBundle(choice_from_generator())
+            else:
+                raise TypeError('When the MolBundle is a generator, the p should be a float or Callable object')
+
+        elif get_remain:  # get remain molecules as the second return
+            mol_indices = np.arange(len(self))
+            chosen_idx = np.random.choice(mol_indices, size=int(len(self) * p))
+            remain_idx = np.setdiff1d(mol_indices, chosen_idx)
+
+            chosen_mol = np.array(self.mols)[chosen_idx].tolist()
+            remain_mol = np.array(self.mols)[remain_idx].tolist()
+
+            return self.__class__(chosen_mol), self.__class__(remain_mol)
+
+        else:
+            return self.__class__(np.random.choice(self.mols, size=size, replace=replace, p=p))
+
+    def collect_identical(self, inplace: bool = False) -> 'MolBundle':
+        """ Merge the molecules with same graph structures to one """
+        dict_umol = {}
+        for mol in self.mols:
+            list_umol = dict_umol.setdefault(mol.atom_counts, [])
+
+            if not list_umol:
+                list_umol.append(mol)
+            if all(umol != mol for umol in list_umol):
+                list_umol.append(mol)
+
+        if inplace:
+            self.mols = [umol for list_umol in dict_umol.values() for umol in list_umol]
+        else:
+            return self.__class__([umol for list_umol in dict_umol.values() for umol in list_umol])
+
+    @property
+    def data(self):
+        return self._data
+
+    @data.setter
+    def data(self, data):
+        if isinstance(data, dict):
+            self._data = data
+        else:
+            raise TypeError(f'the {self.__class__.__name__}.data must be a dict')
+
+    @classmethod
+    def read_from(
+            cls, fmt: str,
+            dir_or_strings: Union[str, PathLike, Iterable[str]],
+            match_pattern: str = '*',
+            generate: bool = False,
+            ranges: Union[Sequence[int], range] = None,
+            condition: Callable = None,
+            num_proc: int = None
+    ):
+        """
+        Read Molecule objects from a directory.
+
+        Args:
+            fmt(str): read file with the specified-format method.
+            dir_or_strings(str|PathLike): the directory all file put, or a sequence of string
+            match_pattern(str): the file name pattern
+            generate(bool): read file to a generator of Molecule object
+            ranges(Sequence[int]|range): A list or range of integers representing the indices of
+                the input files to read. Defaults to None.
+            condition(Callable): A callable object that takes two arguments (the path of the input file
+                and the corresponding Molecule object) and returns a boolean value indicating whether to include the
+                Molecule object in the output. Defaults to None.
+            num_proc: the number of process to read
+
+        Returns:
+            List(Molecule) or Generator(Molecule)
+        """
+        def read_mol(pm: Path, conn):
+
+            try:
+                mol = ci.Molecule.read_from(pm, fmt)
+
+                # the OBMol, OBAtom, OBBond are C++ objects wrapped by SWIG,
+                # they can't be pickle, so pop them from Molecule and convert their info to .mol2 string
+                pmol = pb.Molecule(mol.ob_mol_pop())
+                script = pmol.write('mol2')  # Write to the mol2 script to allow it to pickle
+
+                # communicate with the main process
+                conn.send((mol, script, pm))
+
+            except AttributeError:
+                conn.send((None, None, pm))
+
+            except StopIteration:
+                conn.send((None, None, pm))
+
+        def mol_generator():
+            nonlocal dir_or_strings
+            for i, path_mol in enumerate(generate_path_or_string()):
+
+                if not ranges or i in ranges:
+                    try:
+                        mol = ci.Molecule.read_from(path_mol, fmt)
+                    except StopIteration:
+                        mol = None
+                else:
+                    continue
+
+                if mol and (not condition or condition(path_mol, mol)):
+                    yield mol
+
+        def mol_mp_generator():
+            mols_info = []
+
+            parent_conn, child_conn = mp.Pipe()
+            ps = []  # list of Process: Queue pairs
+
+            for i, source in enumerate(generate_path_or_string()):
+
+                # if the number of process more than num_proc, get the read molecule info and stop to start new process
+                while len(ps) >= num_proc:
+                    for p in ps:
+                        if not p.is_alive():
+                            mols_info.append(parent_conn.recv())
+                            p.terminate()
+                            ps.remove(p)
+
+                # When received some Molecule info, reorganize these info and yield
+                while mols_info:
+                    mol, script, pf = mols_info.pop()  # hotpot Molecule, mol2_script, path_file of Molecule
+
+                    # If you get a valid Molecule info, re-wrap to be hotpot Molecule
+                    if mol and script:
+                        pmol = pb.readstring('mol2', script)  # pybel Molecule object
+                        mol.ob_mol_rewrap(pmol.OBMol)  # re-wrap OBMol by hotpot Molecule
+
+                        # if the reorganized Molecule is expected, yield
+                        if not condition or condition(mol, pf):
+                            yield mol
+
+                # Start new process to read Molecule from file
+                if not ranges or i in ranges:
+                    p = mp.Process(target=read_mol, args=(source, child_conn))
+                    p.start()
+                    ps.append(p)
+
+            # After all path_file have pass into process to read
+            while ps:
+                for p in ps:
+                    if not p.is_alive():
+                        mols_info.append(parent_conn.recv())
+                        p.terminate()
+                        ps.remove(p)
+
+            for mol, script, pf in mols_info:
+                # if get a valid Molecule info, re-wrap to be hotpot Molecule
+                if mol and script:
+                    pmol = pb.readstring('mol2', script)  # pybel Molecule object
+                    mol.ob_mol_rewrap(pmol.OBMol)  # re-wrap OBMol by hotpot Molecule
+
+                    # if the reorganized Molecule is expected, yield
+                    if not condition or condition(mol, pf):
+                        yield mol
+
+        def generate_path_or_string():
+            """"""
+            if isinstance(dir_or_strings, Path):
+                for path in dir_or_strings.glob(match_pattern):
+                    yield path
+
+            elif isinstance(dir_or_strings, Iterable):
+                for string in dir_or_strings:
+                    yield string
+
+            else:
+                raise TypeError(f'the dir_or_strings is required to be a Path or str, get {type(dir_or_strings)}')
+
+        if isinstance(dir_or_strings, str):
+            dir_or_strings = Path(dir_or_strings)
+        elif not isinstance(dir_or_strings, PathLike) and not isinstance(dir_or_strings, Iterable):
+            raise TypeError(
+                f'the read_dir should be a str, PathLike or iterable str, instead of {type(dir_or_strings)}'
+            )
+
+        generator = mol_mp_generator() if num_proc else mol_generator()
+
+        if generate:
+            return cls(generator)
+        else:
+            return cls([m for m in tqdm(generator, 'reading molecules')])
+
+    def gcmc_for_isotherm(
+            self, *guest: 'ci.Molecule', force_field: Union[str, PathLike] = None,
+            work_dir: Union[str, PathLike] = None, T: float = 298.15,
+            Ps: Sequence[float] = (1.0,), procs: int = 1, named_identifier: bool = False,
+            **kwargs
+    ):
+        """
+        Run gcmc to determine the adsorption of guest,
+        Args:
+            self: the framework as the sorbent of guest molecule
+            guest(Molecule): the guest molecule to be adsorbed into the framework
+            force_field(str|PathLike): the path to force field file or the self-existent force file contained
+             in force field directory (in the case, a str should be given as a relative path from the root of
+             force field root to the specified self-existent force filed). By default, the force field is UFF
+             which in the relative path 'UFF/LJ.json' for the force field path.
+            work_dir: the user-specified dir to store the result of GCMC and log file.
+            T: the environmental temperature (default, 298.15 K)
+            Ps(Sequence[float]): A sequence of relative pressure related to the saturation vapor in the environmental temperature.
+            procs(int): the number of processes, default 1.
+            named_identifier: Whether to name the dir by the identifier of frames
+        """
+        if isinstance(work_dir, str):
+            work_dir = Path(work_dir)
+
+        # Assemble keywords arguments for multiprocess
+        processes = []
+        for i, frame in enumerate(self.mols, 1):
+
+            # When the running proc more than the specified values, waiting for terminate
+            while len(processes) >= procs:
+                for p in processes:
+                    if not p.is_alive():
+                        processes.pop(processes.index(p))
+                        p.terminate()
+
+                time.sleep(10)
+
+            if named_identifier:
+                sub_work_dir = work_dir.joinpath(frame.identifier)
+            else:
+                idt_map = self._data.setdefault('identifier_map', {})
+                idt_map[i] = frame.identifier
+                sub_work_dir = work_dir.joinpath('mol_' + str(i))
+
+            if not sub_work_dir.exists():
+                sub_work_dir.mkdir()
+
+            kwargs.update({
+                'force_field': force_field,
+                'work_dir': sub_work_dir,
+                'T': T, 'Ps': Ps
+            })
+
+            p = mp.Process(target=frame.gcmc_for_isotherm, args=guest, kwargs=kwargs)
+
+            p.start()
+            processes.append(p)
+
+        for p in processes:
+            p.join()
+            p.terminate()
+
+        return self._data.get('identifier_map')
+
+    def graph_representation(self, *feature_names) -> Generator[Union[str, np.ndarray, np.ndarray], None, None]:
+        """ Transform molecules to their graph representation """
+        for mol in self.mols:
+            yield mol.graph_representation(*feature_names)
+
+    def gaussian(
+            self, g16root: Union[str, PathLike], dir_out: Union[str, PathLike],
+            link0: Union[str, List[str]], route: Union[str, List[str]],
+            dir_err: Optional[Union[str, PathLike]] = None,
+            dir_chk: Optional[Union[str, PathLike]] = None,
+            clean_conformers: bool = True,
+            perturb_kwargs: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
+            *args, **kwargs
+    ) -> None:
+        """
+        Run Gaussian16 calculations for Molecule objects stored in the MolBundle.
+        These Molecules are allowed to be perturbed their atoms' coordinates before submit to Gaussian 16
+
+        Args:
+            g16root (Union[str, PathLike]): The path to the Gaussian16 root directory.
+            dir_out (Union[str, PathLike]): The path to the directory to output the log files.
+            link0 (Union[str, List[str]]): The link0 information for Gaussian16 calculations.
+            route (Union[str, List[str]]): The route information for Gaussian16 calculations.
+            dir_err (Optional[Union[str, PathLike]], optional): The path to the directory to output the error files.
+                Defaults to None.
+            dir_chk (Optional[Union[str, PathLike]], optional): The path to the directory to store the .chk files.
+                Defaults to None.
+            clean_conformers (bool, optional): A flag indicating whether to clean the configuration before perturbing
+                the molecule or lattice. Defaults to True.
+            perturb_kwargs (Optional[Union[Dict[str, Any], List[Dict[str, Any]]]], optional): The parameters for
+                perturbing the molecule or lattice. Defaults to None.
+            *args: Additional positional arguments.
+            **kwargs: Additional keyword arguments.
+
+        Returns:
+            None
+        """
+        # Check and process paths
+        g16root: Path = check_path(g16root, file_or_dir='dir')
+        dir_out: Path = check_path(dir_out, mkdir=True)
+        dir_err: Optional[Path] = check_path(dir_err, mkdir=True)
+        dir_chk: Optional[Path] = check_path(dir_chk, mkdir=True)
+
+        for mol in self.mols:
+            assert isinstance(mol, ci.Molecule)
+
+            # Clean before perturb conformers
+            if clean_conformers:
+                mol.clean_conformers()
+
+            # Assign the dirs
+            # assign the dir to put out.log files for the mol
+            dir_out_mol = dir_out.joinpath(mol.identifier)
+            if not dir_out_mol.exists():
+                dir_out_mol.mkdir()
+
+            # assign the dir to put err.log files for the mol
+            if dir_err:
+                dir_err_mol = dir_err.joinpath(mol.identifier)
+                if not dir_err_mol.exists():
+                    dir_err_mol.mkdir()
+            else:
+                dir_err_mol = None
+
+            # Performing the molecule or lattice perturb
+            if isinstance(perturb_kwargs, Dict):
+                perturb_kwargs = [perturb_kwargs]  # Wrap it into a list
+
+            if isinstance(perturb_kwargs, List) and all(isinstance(pk, dict) for pk in perturb_kwargs):
+                for pk in perturb_kwargs:
+                    pk['inplace'] = True  # Force to inplace
+                    mol.perturb_atoms_coordinates(**pk)
+            elif perturb_kwargs is not None:
+                ValueError('The perturb_kwargs should be a dict or list of dict')
+
+            # Running the gaussian16
+            for config_idx in range(mol.conformer_counts):
+                mol.conformer_select(config_idx)
+
+                # Reorganize the arguments for each conformer
+                path_out = dir_out_mol.joinpath(f'{config_idx}.log')
+                path_err = dir_err_mol.joinpath(f'{config_idx}.err') if dir_err else None
+
+                if dir_chk:  # for dir_chk
+                    dir_chk_mol = dir_chk.joinpath(mol.identifier)
+                    dir_chk_mol.mkdir(exist_ok=True)
+
+                    if isinstance(link0, str):
+                        link0_cfg = [f'chk={str(dir_chk_mol)}/{config_idx}.chk', link0]
+                    elif isinstance(link0, list):
+                        link0_cfg = copy.copy(link0)
+                        link0_cfg.insert(0, f'chk={str(dir_chk_mol)}/{config_idx}.chk')
+                    else:
+                        TypeError('the link0 should be str or list of str!')
+                else:
+                    link0_cfg = link0
+
+                mol.gaussian(
+                    g16root=g16root,
+                    link0=link0_cfg,
+                    route=route,
+                    path_log_file=str(path_out.absolute()),
+                    path_err_file=str(path_err) if path_err else None,
+                    *args, **kwargs
+                )
+
+    @property
+    def is_generator(self):
+        """ To judge weather the object is a Molecule generator """
+        return isinstance(self.mols, Generator)
+
+    @property
+    def mols(self):
+        return self._data.get('mols', [])
+
+    @mols.setter
+    def mols(self, mols):
+        self._data['mols'] = mols
+
+    @staticmethod
+    def registered_bundle_names():
+        """ Return all registered bundle names """
+        return list(_bundle_classes.keys())
+
+    def to(self, bundle_name: str):
+        """ Convert this bundle to other bundle type """
+        return _bundle_classes[bundle_name](self.mols)
+
+    def to_list(self) -> List[ci.Molecule]:
+        """ Convert the molecule container (self.mol) to list """
+        if isinstance(self.mols, Generator):
+            self.mols = list(self)
+
+        return self.mols
+
+    def unique_mols(self, mode: Literal['smiles', 'similarity'] = 'smiles'):
+        """
+        get a new Bundle with all unique Molecule objects
+        Args:
+            mode: the standard to identify whether two molecule to be regard as identical
+
+        Returns:
+            A new Bundle with all the unique Molecule objects
+        """
+        clone = copy.copy(self)
+        clone.data = copy.copy(self.data)
+        if mode == 'smiles':
+            clone.mols = ({m.smiles: m for m in self.mols}.values())
+            return clone
+        elif mode == 'similarity':
+            dict_mols = {}
+            for mol in self.mols:
+                mols_with_same_atom_num = dict_mols.setdefault(mol.atom_counts, [])
+                mols_with_same_atom_num.append(mol)
+
+            new_mols = []
+            for _, mols_with_same_atom_num in dict_mols.items():
+                uni_mols = []
+                for mol in mols_with_same_atom_num:
+                    if mol not in uni_mols:
+                        uni_mols.append(mol)
+
+                new_mols.extend(uni_mols)
+
+            clone.mols = new_mols
+
+            return clone
+
+
+@register_bundles
+class DeepModelBundle(MolBundle):
+    """ Specific MolBundle to carry out the tasks in DeepModeling packages """
+
+    def merge_conformers(self):
+        """
+        Get the sum of conformers for all molecule in the mol bundle "self.mols"
+        This method can only be successfully executed
+        when all molecules in the molecular bundle can be added to each other
+        Returns:
+            a Molecule object with all conformers in the self.mols
+        """
+        atomic_numbers = self.atomic_numbers
+
+        if isinstance(atomic_numbers, tuple):
+            return sum(self.mols[1:], start=self.mols[0])
+        elif isinstance(atomic_numbers, dict):
+            mol_array = np.array(self.mols)
+            return self.__class__([mol_array[i].sum() for ans, i in self.atomic_numbers.items()])
+
+    def merge_atoms_same_mols(self) -> 'DeepModelBundle':
+        """ Merge Molecules with same atoms to a MixSameAtomMol """
+        bundle: DeepModelBundle = self.to_mix_mols()
+        atom_counts = bundle.atom_counts
+
+        if isinstance(atom_counts, tuple):
+            return sum(bundle.mols[1:], start=bundle.mols[0])
+        elif isinstance(atom_counts, dict):
+            mol_array = np.array(bundle.mols)
+            return self.__class__([mol_array[i].sum() for ans, i in atom_counts.items()])
+
+    def to_dpmd_sys(
+            self, system_dir: Union[str, os.PathLike],
+            validate_ratio: float,
+            mode: Literal['std', 'att'] = 'std',
+            split_mode: Optional[Literal['inside', 'outside']] = None
+    ):
+        """"""
+        def to_files(mb: MolBundle, save_root: Path):
+            for c, m in enumerate(mb):  # c: counts, m: molecule
+                mol_save_root = \
+                    save_root.joinpath(str(m.atom_counts)) if mode == 'att' else save_root.joinpath(str(c))
+                if not mol_save_root.exists():
+                    mol_save_root.mkdir()
+
+                m.to_dpmd_sys(mol_save_root, mode)
+
+        if split_mode and split_mode not in ['inside', 'outside']:
+            raise ValueError("the split_mode must be 'inside' or 'outside'")
+
+        if not 0.0 < validate_ratio < 1.0:
+            raise ValueError('the validate_ratio must be from 0.0 to 1.0')
+
+        # Organize dirs
+        if not isinstance(system_dir, Path):
+            system_dir = Path(system_dir)
+        if not system_dir.exists():
+            system_dir.mkdir()
+
+        training_dir = system_dir.joinpath('training_data')
+        validate_dir = system_dir.joinpath('validate_data')
+        if not training_dir.exists():
+            training_dir.mkdir()
+        if not validate_dir.exists():
+            validate_dir.mkdir()
+
+        if mode == 'att':
+            bundle = self.merge_atoms_same_mols()
+            if not split_mode:
+                split_mode = 'inside'
+
+        elif mode == 'std':
+            bundle = self.merge_conformers()
+            if not split_mode:
+                split_mode = 'outside'
+
+        else:
+            raise ValueError("the mode is only allowed to be 'att' or 'std'!")
+
+        if split_mode == 'inside':
+            for i, mol in enumerate(bundle):
+                mol_training_dir = \
+                    training_dir.joinpath(str(mol.atom_counts)) if mode == 'att' else system_dir.joinpath(str(i))
+                mol_validate_dir = \
+                    validate_dir.joinpath(str(mol.atom_counts)) if mode == 'att' else system_dir.joinpath(str(i))
+
+                if not mol_training_dir.exists():
+                    mol_training_dir.mkdir()
+                if not mol_validate_dir.exists():
+                    mol_validate_dir.mkdir()
+
+                mol.to_dpmd_sys(mol_training_dir, mode, validate_ratio, mol_validate_dir)
+
+        elif split_mode == 'outside':
+            validate_bundle, training_bundle = bundle.choice(p=validate_ratio, get_remain=True)
+
+            # Save to files
+            to_files(training_bundle, training_dir)
+            to_files(validate_bundle, validate_dir)
+
+    def to_mix_mols(self):
+        """
+        Return a new MolBundle, in which Molecule objects in container are converted to MixSameAtomMol
+        Returns:
+            MolBundle(MixSameAtomMol)
+        """
+        return self.__class__([m.to_mix_mol() if not isinstance(m, ci.MixSameAtomMol) else m for m in self])
+
+    def to_mols(self):
+        """
+        Return a new MolBundle, in which MixSameAtomMol objects in container are converted to Molecule
+        Returns:
+            MolBundle(Molecule)
+        """
+        return self.__class__([m.to_mol() if isinstance(m, ci.MixSameAtomMol) else m for m in self])
+
```

### Comparing `hotpot-zzy-0.3.0.9/hotpot/cheminfo.py` & `hotpot-zzy-0.3.1.0/hotpot/cheminfo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,3057 +1,3414 @@
-"""
-python v3.9.0
-@Project: hotpot
-@File   : cheminfo.py
-@Author : Zhiyuan Zhang
-@Date   : 2023/3/14
-@Time   : 4:09
-"""
-import copy
-import json
-import os
-import re
-from abc import ABC, abstractmethod
-from io import IOBase
-from os import PathLike
-from os.path import join as opj
-from pathlib import Path
-from typing import *
-from itertools import product
-
-import numpy as np
-from openbabel import openbabel as ob, pybel as pb
-from rdkit import Chem
-from rdkit.Chem import Draw
-
-from hotpot import data_root
-from hotpot.tanks import lmp
-from hotpot.tanks.quantum import Gaussian, GaussianRunError
-from hotpot.utils.library import library as _lib  # The chemical library
-
-
-# Define Exceptions
-class OperateOBMolFail(BaseException):
-    """ Raise for any fail that trys to operate the OBMol """
-
-
-class AddAtomFail(OperateOBMolFail):
-    """ Raise when add an atom into Molecule fail """
-
-
-class AddBondFail(OperateOBMolFail):
-    """ Raise when add a bond into Molecule fail """
-
-
-# periodic_table = json.load(open(opj(data_root, 'periodic_table.json'), encoding='utf-8'))
-periodic_table = _lib.get('PeriodicTable')  # hotpot.utils.library.PeriodicTabel
-
-_stable_charges = {
-    "H": 1,  "He": 0,
-    "Li": 1, "Be": 2, "B": 3,  "C": 4,  "N": -3,  "O": -2,  "F": -1,  "Ne": 0,
-    "Na": 1, "Mg": 2, "Al": 3, "Si": 4, "P": -3,  "S": -2,  "Cl": -1, "Ar": 0,
-    "K": 1,  "Ca": 2, "Ga": 3, "Ge": 4, "As": -3, "Se": -2, "Br": -1, "Kr": 0,
-    "Rb": 1, "Sr": 2, "In": 3, "Sn": 2, "Sb": -3, "Te": -2, "I": -1,  "Xe": 0,
-    "Cs": 1, "Ba": 2, "Tl": 3, "Pb": 2, "Bi": 3,  "Po": -2, "At": -1, "Rn": 0,
-    "Fr": 1, "Ra": 2, "Nh": 8, "Fl": 8, "Mc": 8,  "Lv": 8,  "Ts": 8,  "Og": 8,
-
-    "Sc": 3, "Ti": 4, "V": 5,  "Cr": 3, "Mn": 2,  "Fe": 3,  "Co": 3,  "Ni": 2, "Cu": 2, "Zn": 2,
-    "Y": 3,  "Zr": 4, "Nb": 5, "Mo": 6, "Tc": 7,  "Ru": 4,  "Rh": 3,  "Pd": 2, "Ag": 1, "Cd": 2,
-    "Lu": 3, "Hf": 4, "Ta": 5, "W": 6,  "Re": 7,  "Os": 4,  "Ir": 3,  "Pt": 2, "Au": 1, "Hg": 2,
-    "Lr": 3, "Rf": 4, "Db": 5, "Sg": 6, "Bh": 7,  "Hs": 8,  "Mt": 8,  "Ds": 8, "Rg": 8, "Cn": 8,
-
-    "La": 3, "Ce": 4, "Pr": 3, "Nd": 3, "Pm": 3,  "Sm": 3,  "Eu": 2,  "Gd": 3, "Tb": 3, "Dy": 3, "Ho": 3, "Er": 3, "Tm": 3, "Yb": 3,
-    "Ac": 3, "Th": 4, "Pa": 5, "U": 6,  "Np": 6,  "Pu": 6,  "Am": 6,  "Cm": 6, "Bk": 6, "Cf": 6, "Es": 6, "Fm": 6, "Md": 6, "No": 6,
-}
-
-
-_bond_type = {
-    'Unknown': 0,
-    'Single': 1,
-    'Double': 2,
-    'Triple': 3,
-    'Aromatic': 5,
-}
-
-_type_bond = {
-    0: 'Unknown',
-    1: 'Single',
-    2: 'Double',
-    3: 'Triple',
-    5: 'Aromatic'
-}
-
-_ob_data_dict = {
-    0: 'UndefinedData', 1: 'PairData', 2: 'EnergyData', 3: 'CommentData',
-    4: 'ConformerData', 5: 'ExternalBondData', 6: 'RotamerList', 7: 'VirtualBondData',
-    8: 'RingData', 9: 'TorsionData', 10: 'AngleData', 11: 'SerialNums',
-    12: 'UnitCell', 13: 'SpinData', 14: 'ChargeData', 15: 'SymmetryData',
-    16: 'ChiralData', 17: 'OccupationData', 18: 'DensityData', 19: 'ElectronicData',
-    20: 'VibrationData', 21: 'RotationData', 22: 'NuclearData', 23: 'SetData',
-    24: 'GridData', 25: 'VectorData', 26: 'MatrixData', 27: 'StereoData',
-    28: 'DOSData', 29: 'ElectronicTransitionData', 16384: 'CustomData0', 16385: 'CustomData1',
-    16386: 'CustomData2', 16387: 'CustomData3', 16388: 'CustomData4', 16389: 'CustomData5',
-    16390: 'CustomData6', 16391: 'CustomData7', 16392: 'CustomData8', 16393: 'CustomData9',
-    16394: 'CustomData10', 16395: 'CustomData11', 16396: 'CustomData12', 16397: 'CustomData13',
-    19398: 'CustomData14', 16399: 'CustomData15'
-}
-
-
-class Wrapper(ABC):
-    """
-    A wrapper of chemical information and data.
-    The _set_attrs method is used to set any keyword attribute, the attribute names, in the wrapper context, are defined
-    by the keys from returned dict of _attr_setters; the values of the returned dict of _attr_setters are a collection
-    of specific private method to wrapper and call openbabel method to set the attributes in openbabel object.
-    """
-    _data = {}  # all attributes of wrappers are stored into
-
-    @property
-    def _ob_obj(self) -> Union[ob.OBMol, ob.OBAtom, ob.OBBond, ob.OBAngle, ob.OBUnitCell]:
-        return self._data.get('ob_obj')
-
-    @property
-    def _protected_data(self):
-        """
-        the protected attr in data which could not be replaced by call methods:
-            - update_attr_data()
-        """
-        return ('ob_obj',)
-
-    def _set_attrs(self, **kwargs):
-        """    Set any atomic attributes by name    """
-        attr_setters = self._attr_setters
-        for name, value in kwargs.items():
-            setter = attr_setters.get(name)
-
-            if setter:  # if the attribute is exist in the object.
-                assert isinstance(setter, Callable)
-                setter(value)
-
-            else:
-                raise NameError(
-                    f'the {name} is cannot be set by {self.__class__.__name__}.set(), '
-                    f'the legal attrs include: {self._attr_setters.keys()}'
-                )
-
-    @property
-    @abstractmethod
-    def _attr_setters(self) -> Dict[str, Callable]:
-        raise NotImplemented
-
-    def _get_ob_comment_data(self, data_name: str):
-        """ Retrieve OBCommentData according to specific data_name """
-        comment = self._ob_obj.GetData(data_name)
-        if comment:
-            comment = ob.toCommentData(comment)
-            return comment.GetData()
-        return None
-
-    @property
-    def data(self) -> dict:
-        """ Get the clone of attributes data dict """
-        return copy.copy(self._data)
-
-    def kwargs_setters(self):
-        list_setters = [f'{k}: {s.__doc__}' for k, s in self._attr_setters.items()]
-        print("\n".join(list_setters))
-
-    def remove_ob_data(self, data_name: str):
-        """ Remove specific OBData item by given data_name """
-        self._ob_obj.DeleteData(data_name)
-
-    def replace_attr_data(self, data: Dict):
-        """ Replace the core data dict directly """
-        self._data = data
-
-    def set_ob_comment_data(self, attr_name: str, value: str):
-        """ Set the OBCommentData for ob_obj """
-        comment_data = ob.OBCommentData()
-
-        comment_data.SetAttribute(attr_name)
-        comment_data.SetData(value)
-
-        self._ob_obj.CloneData(comment_data)
-
-    @property
-    def setter_keys(self):
-        return list(self._attr_setters.keys())
-
-    @property
-    def temp_label(self):
-        """ Retrieve the temp label """
-        return self._get_ob_comment_data('temp_label')
-
-    def update_attr_data(self, data: dict):
-        """ update the attribute data by give dict """
-        for data_attr in self._protected_data:
-            if data.get(data_attr):
-                data.pop(data_attr)
-
-        self._data.update(data)
-
-
-class Molecule(Wrapper, ABC):
-    """"""
-    # All Molecule attribute's items relating to molecule conformers
-    conformer_items = (
-        # the items are ranked by the number of values for each atom, for example:
-        #   - the all_atom_charges and atom_spin_densities have 1 value for each atom, so they are placed in the second
-        #     item (with the index 1)
-        #   - the coordinates have 3 values for each atom, i.e., [x, y, z], so it is placed in the forth
-        #     item (with the index 3）
-        # For the molecular attributes, which have only one value for each conformer and represent the attribute
-        # of whole molecule, they are place in the first item (with the index 0)
-        ('all_energy', 'identifier_array'),
-        ('all_atom_charges', 'all_atom_spin_densities'),
-        (),
-        ('all_coordinates', 'all_forces')
-    )
-
-    def __init__(self, ob_mol: ob.OBMol = None, _data: dict = None, **kwargs):
-        if _data:
-            self._data: dict = _data
-        else:
-            self._data: dict = {
-                'ob_obj': ob_mol if ob_mol else ob.OBMol()
-            }
-        self._set_attrs(**kwargs)
-        self._load_atoms()
-        self._load_bonds()
-
-    def __repr__(self):
-        return f'Mol({self.ob_mol.GetSpacedFormula()})'
-
-    def __add__(self, other: ['Molecule']):
-        """
-        Two Molecule objects could add to a new one to merge all of their conformers.
-        All of information about the conformer will be merged to one.
-        the other information will reserve the one in the left item
-        Args:
-            other: the right item
-
-        Returns:
-            Molecule
-        """
-        # When other obj is a Molecule or a child of Molecule
-        if isinstance(other, Molecule):
-            # If this one is compatible to the other
-            if self.iadd_accessible(other):
-                clone = self.copy()
-                clone += other
-
-                return clone
-
-            # If the other one is compatible to this one
-            if other.iadd_accessible(self):
-                clone = other.copy()
-                clone += self
-
-                return clone
-
-            # If they are compatible, but are Molecule or child of Molecule
-            return bd.MolBundle([self, other])
-
-        # if isinstance(other, MixSameAtomMol):
-        #     return self.to_mix_mol() + other
-
-        # When other obj is a MolBundle
-        if isinstance(other, bd.MolBundle):
-            return other.__class__([self] + other.mols)
-
-        else:
-            raise TypeError('the Molecule only add with Molecule or MolBundle')
-
-    def __iadd__(self, other):
-        """
-        Self add with other Molecule object with consist atoms list,
-        The attributes or information about conformers will merge with the other,
-        other attributes or information will be reserved
-        Args:
-            other: the merged Molecule object
-
-        Returns:
-            None
-        """
-        if not isinstance(other, Molecule):
-            raise TypeError('the Molecule object is only allowed to add with other Molecule')
-
-        # Check whether left and right Molecules have consist atom list
-        if not self.iadd_accessible(other):
-            raise AttributeError(
-                'the self addition cannot be performed among molecules with different atoms list!'
-            )
-
-        return self._merge_conformer_attr(other)
-
-    def __iter__(self):
-        """ Return self with different conformers """
-
-        def conformer_generator():
-            for i in range(self.conformer_counts):
-                self.conformer_select(i)
-                yield self
-
-        return iter(conformer_generator())
-
-    def __next__(self):
-        config_idx = self._data.get('config_idx', 0)
-        try:
-            self.conformer_select(config_idx)
-            self._data['config_idx'] = config_idx + 1
-            return self
-        except IndexError:
-            raise StopIteration
-
-    def __eq__(self, other):
-        """ if two molecule with 1.0 similarity in 2FP fingerprint they are identical """
-        if self.similarity(other) == 1.0:
-            return True
-        return False
-
-    def _add_temp_atom_labels(self):
-        """
-        Add temp atom label, These label will assist in the implementation of certain functions,
-        say Molecule.components. These label should be deleted after the assisted functions have
-        been fulfilled, by call method _delete_temp_atom_labels(self)
-        """
-        for i, atom in enumerate(self.atoms):
-            atom.set_ob_comment_data('temp_label', str(i))
-
-    @staticmethod
-    def _assign_coordinates(the_mol: 'Molecule', coordinates: np.ndarray):
-        """ Assign coordinates for all atoms in the Molecule """
-        if len(the_mol.atoms) != coordinates.shape[-2]:
-            raise AttributeError('the coordinate matrix do not match the number of atoms')
-
-        for new_mol_atom, new_atom_coord in zip(the_mol.atoms, coordinates):
-            new_mol_atom.coordinates = new_atom_coord
-
-    @property
-    def _attr_setters(self) -> Dict[str, Callable]:
-        return {
-            'atoms.partial_charge': self._set_atoms_partial_charge,
-            "identifier": self._set_identifier,
-            "energy": self._set_energy,
-            'all_energy': self._set_all_energy,
-            'charge': self._set_mol_charge,
-            'all_atom_charges': self._set_all_atom_charges,
-            'all_atom_spin_densities': self._set_all_atom_spin_densities,
-            'spin': self._set_spin_multiplicity,
-            'atoms': self._set_atoms,
-            'mol_orbital_energies': self._set_mol_orbital_energies,
-            'coordinates': self._set_coordinates,
-            'all_coordinates': self._set_all_coordinates,
-            'all_forces': self._set_all_forces,
-            'forces': self._set_forces,
-            'crystal': self.create_crystal_by_matrix
-        }
-
-    def _create_ob_unit_cell(self):
-        """ Create New OBUnitCell for the Molecule """
-        ob_unit_cell = ob.OBUnitCell()
-        self.ob_mol.CloneData(ob_unit_cell)
-
-    def _delete_atom_temp_label(self):
-        """ Remove temp label of all label """
-        for a in self.atoms:
-            a.remove_ob_data('temp_label')
-
-    def _get_critical_params(self, name: str):
-        critical_params = self._data.get('critical_params')
-        if critical_params is None:
-            critical_params = json.load(open(opj(data_root, 'thermo', 'critical.json'))).get(self.smiles)
-            if critical_params:
-                self._data['critical_params'] = critical_params
-                return critical_params[name]
-            else:
-                self._data['critical_params'] = False
-                return False
-
-        else:
-            return critical_params[name]
-
-    def _pert_mol_generate(self, coordinates: Union[Sequence, np.ndarray]):
-        """
-        Generate new molecule obj according to new given coordinate
-        Args:
-            coordinates: New coordinates matrix
-
-        Returns:
-            Molecule, copy of this molecule with new coordinates
-        """
-        clone_mol = self.copy()
-        self._assign_coordinates(clone_mol, coordinates)
-        return clone_mol
-
-    def _load_atoms(self) -> Dict[int, 'Atom']:
-        """
-        Construct atoms dict according to the OBAtom in the OBMol,
-        where the keys of the dict are the ob_id of OBAtom and the values are the the constructed Atom objects
-        the constructed dict would be place into the _data dict
-        Returns:
-            the atoms dict
-        """
-        atoms: Dict[int, Atom] = self._data.get('atoms', {})
-
-        new_atoms = {}
-        for new_ob_id, oba in enumerate(ob.OBMolAtomIter(self.ob_mol)):
-            atom = atoms.get(oba.GetId(), Atom(oba, mol=self))
-            oba.SetId(new_ob_id)
-            new_atoms[new_ob_id] = atom
-
-        self._data['atoms'] = new_atoms
-
-        return new_atoms
-
-    def _load_bonds(self) -> Dict[int, 'Bond']:
-        """
-        Construct bonds dict according to the OBBond in the OBMol,
-        where the keys of the dict are the ob_id of OBBond and the values are the the constructed Bond objects
-        the constructed dict would be place into the _data dict
-        Returns:
-            dict of bonds
-        """
-        bonds: Dict = self._data.get('bonds', {})  # Get the stored bonds
-
-        new_bonds = {}
-        for new_ob_id, obb in enumerate(ob.OBMolBondIter(self.ob_mol)):
-            bond = bonds.get(obb.GetId(), Bond(obb, self))  # Get old bond by old id
-            obb.SetId(new_ob_id)  # Specify new id
-            new_bonds[new_ob_id] = bond
-
-        self._data['bonds'] = new_bonds
-
-        return new_bonds
-
-    @staticmethod
-    def _melt_quench(
-            elements: Dict[str, float], force_field: Union[str, os.PathLike], mol: "Molecule" = None,
-            density: float = 1.0, a: float = 25., b: float = 25., c: float = 25.,
-            alpha: float = 90., beta: float = 90., gamma: float = 90., time_step: float = 0.0001,
-            origin_temp: float = 298.15, melt_temp: float = 4000., highest_temp: float = 10000.,
-            ff_args: Sequence = (), path_writefile: Optional[str] = None, path_dump_to: Optional[str] = None,
-            dump_every: int = 100,
-    ):
-        """ to perform the melt-quench by call lmp.AmorphousMaker """
-        am = lmp.AmorphousMaker(elements, force_field, density, a, b, c, alpha, beta, gamma)
-        mol = am.melt_quench(
-            *ff_args, mol=mol, path_writefile=path_writefile, path_dump_to=path_dump_to, origin_temp=origin_temp,
-            melt_temp=melt_temp, highest_temp=highest_temp, time_step=time_step, dump_every=dump_every
-        )
-
-        return mol
-
-    def _merge_conformer_attr(self, other: 'Molecule'):
-        """ Merge attributes, relate to molecule conformer, in other Molecule into this Molecule """
-
-        def merge_attr(attr_name: str):
-            """ Merge single conformer attr """
-            left_attr = getattr(self, attr_name)
-            right_attr = getattr(other, attr_name)
-
-            if isinstance(left_attr, np.ndarray) and isinstance(right_attr, np.ndarray):
-                self._data[attr_name] = np.concatenate([left_attr, right_attr])
-            elif not (  # If the left and right values are not both empty, raise Attributes error.
-                    (left_attr is None) or (isinstance(left_attr, np.ndarray) and (not left_attr.all())) and
-                    (right_attr is None) or (isinstance(right_attr, np.ndarray) and (not right_attr.all()))
-            ):
-                raise AttributeError(
-                    f'the conformer relational attribute {attr_name} is different in:\n'
-                    f'  - {self}_identifier: {self.identifier}\n'
-                    f'  - {other}_identifier: {other.identifier}'
-                    'they cannot to perform addition operation'
-                )
-
-        for i, items in enumerate(self.conformer_items):
-            for item in items:
-                merge_attr(item)
-
-        return self
-
-    def _preserve_atoms_data(self):
-        """
-        Preserve atoms data dict before destroy them.
-        Though the atoms are destroyed, their core ob_atom will be prevented,
-        The reserve data will match with the core ob_atoms
-        """
-        # Link the old atoms data dict with new atoms by temp labels
-        self._add_temp_atom_labels()
-        return {a.temp_label: a.data for a in self.atoms}
-
-    @property
-    def _protected_data(self):
-        return 'ob_obj', 'atoms', 'bonds', 'angles'
-
-    def _reorder_atom_ob_id(self):
-        """ Reorder the ob id of atoms """
-        new_atom_dict = {}
-        for ob_id, atom in enumerate(self.atoms):
-            atom.ob_atom.SetId(ob_id)
-            new_atom_dict[ob_id] = atom
-
-        self._data['atoms'] = new_atom_dict
-
-    def _reorder_bond_ob_id(self):
-        new_atom_dict = {}
-        for ob_id, bond in enumerate(self.bonds):
-            bond.ob_bond.SetId(ob_id)
-            new_atom_dict[ob_id] = bond
-
-        self._data['bonds'] = new_atom_dict
-
-    def _reorganize_atom_indices(self):
-        """ reorganize or rearrange the indices for all atoms """
-        for i, ob_atom in enumerate(ob.OBMolAtomIter(self.ob_mol)):
-            ob_atom.SetId(i)
-
-    def _set_atoms(self, atoms_kwargs: List[Dict[str, Any]]):
-        """ add a list of atoms by a list atoms attributes dict """
-        for atom_kwarg in atoms_kwargs:
-            a = Atom(**atom_kwarg)
-            self.add_atom(a)
-
-    def _set_atoms_partial_charge(self, partial_charges: [np.ndarray, Sequence[float]]):
-        """ Set partial charges for all atoms in the molecule """
-        if not isinstance(partial_charges, (np.ndarray, Sequence[int])):
-            raise TypeError(
-                f'the `partial_charges` should be np.ndarray or Sequence of float, not {type(partial_charges)}'
-            )
-
-        if self.atom_counts != len(partial_charges):
-            raise ValueError('the given partial charges should have same numbers with the number of atoms')
-
-        for atom, partial_charge in zip(self.atoms, partial_charges):
-            atom.partial_charge = partial_charge
-
-    def _set_all_coordinates(self, all_coordinates: np.ndarray):
-        """
-        Assign the coordinates collection directly
-        Args:
-            all_coordinates: numpy array with the shape (M, N, 3), where the M is the number of coordinates
-            in the collection, the N is the number of atoms of the molecule.
-
-        Returns:
-            None
-        """
-        if not isinstance(all_coordinates, np.ndarray):
-            raise ValueError(
-                f'the given all_coordinates must be a numpy.ndarray class, instead of {type(all_coordinates)}')
-
-        if all_coordinates.shape[-1] != 3:
-            raise ValueError(f'the coordinate must be 3 dimension, instead of {all_coordinates.shape[-1]}')
-
-        if len(all_coordinates.shape) == 2:
-            # if only give a group of coordinates
-            all_coordinates = all_coordinates.reshape((-1, all_coordinates.shape[-2], 3))
-        elif len(all_coordinates.shape) != 3:
-            raise ValueError(
-                f'the shape of given all_coordinates should with length 2 or 3, now is {len(all_coordinates.shape)}'
-            )
-
-        self._data['all_coordinates'] = all_coordinates
-
-    def _set_coordinates(self, coordinates: np.ndarray):
-        """ Assign the coordinates for all atoms in the molecule """
-        assert isinstance(coordinates, np.ndarray)
-        assert coordinates.shape == (self.atom_counts, 3)
-
-        for a, c in zip(self.atoms, coordinates):
-            a.coordinates = c
-
-    def _set_atom_charges(self, charge: Union[Sequence, np.ndarray]):
-        """ Set partial charge for each atoms in the mol """
-        if not isinstance(charge, (Sequence, np.ndarray)):
-            raise TypeError(f'the charge should be a sequence or np.ndarray, got {type(charge)}')
-
-        if isinstance(charge, np.ndarray):
-            charge = charge.flatten()
-
-        if len(charge) != self.atom_counts:
-            raise ValueError('the number of charges do not match with the atom charge')
-
-        for atom, ch in zip(self.atoms, charge):
-            atom.partial_charge = ch
-
-    def _set_all_atom_charges(self, charges: np.ndarray):
-        """
-        set groups of charges for each atoms in the mol, and each group of charges are corresponding to a
-        conformer of the mol
-        Args:
-            charges: group of atoms with the shape of (C, N), where the C is the number of the conformer
-             and the N is the number of the atom in the molecule
-        """
-        if not isinstance(charges, np.ndarray):
-            raise TypeError('the arg charges should be np.ndarray')
-
-        if len(charges.shape) != 2 and charges.shape[1] != self.atom_counts:
-            raise ValueError('the shape of the arg: charge should be (number_of_conformer, number_of_atoms),'
-                             f'got the value with shape {charges.shape}')
-
-        self._data['all_atom_charges'] = charges
-
-    def _set_all_atom_spin_densities(self, group_spd: np.ndarray) -> None:
-        """
-        assign groups of spin densities for all atom in molecule, each group is corresponding to a conformer
-        Args:
-            group_spd(np.ndarray): group of spin densities, the numpy array with the (C, N) shape,
-             where the C is the number of conformer, the N is the number of atoms
-        """
-        if not isinstance(group_spd, np.ndarray):
-            raise TypeError('the arg group_spd should be np.ndarray')
-
-        if len(group_spd.shape) != 2 and group_spd.shape[1] != self.atom_counts:
-            raise ValueError('the shape of the arg: group_spd should be (number_of_conformer, number_of_atoms),'
-                             f'got the value with shape {group_spd.shape}')
-
-        self._data['all_atom_spin_densities'] = group_spd
-
-    def _set_atom_spin_densities(self, spd: Union[Sequence, np.ndarray]):
-        """ assign the spin density for each of atoms in the mol """
-        if not isinstance(spd, (Sequence, np.ndarray)):
-            raise TypeError(f'the charge should be a sequence or np.ndarray, got {type(spd)}')
-
-        if isinstance(spd, np.ndarray):
-            spd = spd.flatten()
-
-        if len(spd) != self.atom_counts:
-            raise ValueError('the number of charges do not match with the atom charge')
-
-        for atom, sp in zip(self.atoms, spd):
-            atom.spin_density = sp
-
-    def _set_forces(self, forces: np.ndarray):
-        """ Set the force vectors for each atoms in the molecule """
-        if not isinstance(forces, np.ndarray):
-            raise TypeError('the forces should be np.ndarray')
-
-        if len(forces.shape) != 2:
-            raise ValueError('the length of shape of forces should be 2')
-
-        if forces.shape[-2] != self.atom_counts:
-            raise ValueError('the give forces do not match to the number of atoms')
-
-        for atom, force_vector in zip(self.atoms, forces):
-            atom.force_vector = force_vector
-
-    def _set_all_forces(self, all_forces: np.ndarray):
-        """ Store the force matrix into the attribute dict """
-        if not isinstance(all_forces, np.ndarray):
-            raise TypeError('the all_forces should be np.ndarray')
-
-        if len(all_forces.shape) != 3:
-            raise ValueError('the length of shape of all_forces should be 3')
-
-        if all_forces.shape[-2] != self.atom_counts:
-            raise ValueError('the give all_forces do not match to the number of atoms')
-
-        self._data['all_forces'] = all_forces
-
-    def _set_mol_charge(self, charge: int):
-        self.ob_mol.SetTotalCharge(charge)
-
-    def _set_mol_orbital_energies(self, orbital_energies: list[np.ndarray]):
-        self._data['mol_orbital_energies'] = orbital_energies[0]
-
-    def _set_energy(self, energy: float):
-        """ set the energy """
-        self.ob_mol.SetEnergy(energy)
-
-    def _set_all_energy(self, all_energy: Union[float, np.ndarray]):
-        """ set the energy for all conformers """
-        if isinstance(all_energy, float):
-            self._data['all_energy'] = np.array([all_energy])
-        else:
-            all_energy = all_energy.flatten()
-            self._data['all_energy'] = all_energy
-
-    def _set_identifier(self, identifier):
-        self.ob_mol.SetTitle(identifier)
-
-    def _set_spin_multiplicity(self, spin):
-        self.ob_mol.SetTotalSpinMultiplicity(spin)
-
-    @staticmethod
-    def _transfer_preserve_data_to_new_atoms(tgt_mol: 'Molecule', preserve_data: Dict, rm_temp_label: bool = False):
-        """
-        Transfer preserve data dict to new target Molecule object
-        Args:
-            tgt_mol: The target Molecule
-            preserve_data(dict): the old atoms data dict
-            rm_temp_label: whether to remove temp label after data have been transferred.
-        """
-        for atom in tgt_mol.atoms:
-            temp_label = atom.temp_label
-            if temp_label:
-                atom.update_attr_data(preserve_data[temp_label])
-
-                if rm_temp_label:
-                    atom.remove_ob_data('temp_label')
-
-    @property
-    def acentric_factor(self):
-        return self._get_critical_params('acentric_factor')
-
-    def add_atom(self, atom: Union["Atom", str, int], **atom_attrs) -> 'Atom':
-        """
-        Add a new atom out of the molecule into the molecule.
-        Args:
-            atom(Atom|str|int):
-
-        atom_kwargs(kwargs for this added atom):
-            atomic_number(int): set atomic number
-            symbol(str): set atomic symbol
-            coordinates(Sequence, numpy.ndarray): coordinates of the atom
-            partial_charge:
-            label:
-            spin_density:
-
-        Returns:
-            the copy of atom in the molecule
-        """
-        oba = ob.OBAtom()  # Initialize a new OBAtom
-        data = None
-        if isinstance(atom, str):
-            oba.SetAtomicNum(ob.GetAtomicNum(atom))
-        elif isinstance(atom, int):
-            oba.SetAtomicNum(atom)
-        elif isinstance(atom, Atom):
-            oba.SetAtomicNum(atom.atomic_number)
-            data = atom.data  # Copy the give atoms data
-
-        # add OBAtom to the OBMol
-        success = self.ob_mol.AddAtom(oba)
-
-        if success:
-            atom = self.atoms[-1]  # Retrieve the added atom
-
-            if data:
-                atom.update_attr_data(data)  # replicant the old atom's data to the new
-
-            atom.set(**atom_attrs)  # Set attributes by kwargs
-
-            return atom
-
-        else:
-            raise AddAtomFail(f'Add the atom {atom} into Molecule fail')
-
-    @property
-    def all_atoms_with_unique_symbol(self):
-        return self.atoms_with_unique_symbol + \
-            self.pseudo_atoms_with_unique_symbol
-
-    def add_bond(
-            self,
-            atom1: Union[str, int, 'Atom'],
-            atom2: Union[str, int, 'Atom'],
-            bond_type: Union[str, int],
-    ):
-        """ Add a new bond into the molecule """
-        inputs = (atom1, atom2)
-        atoms: List[Atom] = []
-        for a in inputs:
-            if isinstance(a, int):
-                atoms.append(self.atoms_dict[a])
-            if isinstance(a, Atom):
-                atoms.append(a)
-            if isinstance(a, str):
-                atoms.append(self.atom(a))
-
-        # Represent the bond type by int, refer to _bond_type dict
-        bond_type = bond_type if isinstance(bond_type, int) else _bond_type[bond_type]
-
-        # Try to add new OBMol
-        # 'openbabel' has an odd behave that `index` of the `OBAtom` with various origin in the `OBMol`.
-        # the `Id` of `OBAtom` from 0; but the `Idx` of `OBAtom` from 1.
-        # To meet the convention, the `Id` is selected to be the unique `index` to specify `Atom`.
-        # However, when try to add a `OBBond` to link each two `OBAtoms`, the `Idx` is the only method
-        # to specify the atoms, so our `index` in `Atom` are added 1 to match the 'Idx'
-        success = self.ob_mol.AddBond(atoms[0].ob_idx, atoms[1].ob_idx, bond_type)
-
-        if success:
-            return self.bonds[-1]  # the new atoms should place in the terminal of the bond list
-
-        elif atoms[0].ob_id not in self.atom_indices:
-            raise KeyError("the start atom1 doesn't exist in molecule")
-
-        elif atoms[1].ob_id not in self.atom_indices:
-            raise KeyError("the end atom2 doesn't exist in molecule")
-
-        else:
-            raise RuntimeError('add bond not successful!')
-
-    def add_hydrogens(
-            self,
-            polar_only: bool = False,
-            correct_for_ph: bool = False,
-            ph: float = 1.0,
-            balance_hydrogen: bool = True,
-    ):
-        """
-        add hydrogens for the molecule
-        Args:
-            ph: add hydrogen in which PH environment
-            polar_only: Whether to add hydrogens only to polar atoms (i.e., not to C atoms)
-            correct_for_ph: Correct for pH by applying the OpenBabel::OBPhModel transformations
-            balance_hydrogen: whether to balance the bond valance of heavy atom to their valence
-        """
-        self.ob_mol.AddHydrogens(polar_only, correct_for_ph, ph)
-        self._load_atoms()
-        self._load_bonds()
-
-        if balance_hydrogen:
-            for atom in self.atoms:
-                atom.balance_hydrogen()
-
-    def add_pseudo_atom(self, symbol: str, mass: float, coordinates: Union[Sequence, np.ndarray], **kwargs):
-        """ Add pseudo atom into the molecule """
-        list_pseudo_atom = self._data.setdefault('pseudo_atoms', [])
-        pa = PseudoAtom(symbol, mass, coordinates, mol=self, molecule=self, **kwargs)
-        list_pseudo_atom.append(pa)
-
-    @property
-    def all_coordinates(self) -> np.ndarray:
-        """
-        Get the collections of the matrix of all atoms coordinates,
-        each matrix represents a conformer.
-        The return array with shape of (C, N, 3),
-        where the C is the number of conformers, the N is the number of atoms
-        """
-        all_coordinates = self._data.get('all_coordinates')
-        if isinstance(all_coordinates, np.ndarray):
-            return all_coordinates
-        else:
-            return self.coordinates.reshape((-1, self.atom_counts, 3))
-
-    @property
-    def all_energy(self):
-        return self._data.get('all_energy')
-
-    @property
-    def angles(self):
-        return [Angle(self, a_idx) for a_idx in ob.OBMolAngleIter(self.ob_mol)]
-
-    def assign_bond_types(self):
-        self.ob_mol.PerceiveBondOrders()
-
-    def atom(self, id_label: Union[int, str]) -> 'Atom':
-        """ get atom by label or idx """
-        if isinstance(id_label, str):
-
-            if not self.is_labels_unique:
-                raise AttributeError(
-                    'the label is not unique, cannot get atom by label. try to get atom by ob_id '
-                    'or normalize the label before'
-                )
-
-            for atom in self.atoms:
-                if atom.label == id_label:
-                    return atom
-            raise KeyError(f'No atom with label {id_label}')
-
-        elif isinstance(id_label, int):
-            return self.atoms_dict[id_label]
-        else:
-            raise TypeError(f'the given idx_label is expected to be int or string, but given {type(id_label)}')
-
-    @property
-    def atom_counts(self):
-        return self.ob_mol.NumAtoms()
-
-    @property
-    def atomic_numbers(self) -> Tuple[int]:
-        return tuple(a.atomic_number for a in self.atoms)
-
-    @property
-    def atomic_numbers_array(self) -> np.ndarray:
-        """ conformer corresponding attributes with array shape (number_of_atoms, number_of_conformers) """
-        return np.array(self.atomic_numbers).reshape(1, -1).repeat(self.conformer_counts, axis=0)
-
-    @property
-    def atomic_symbols(self):
-        return tuple(a.symbol for a in self.atoms)
-
-    @property
-    def atoms(self) -> List['Atom']:
-        """
-        Generate dict of Atom objects into the data repository.
-        Return list of Atom objects with the order their index.
-        """
-        atoms = self._load_atoms()
-        return list(atoms.values())
-
-    @property
-    def atoms_dict(self) -> Dict[int, 'Atom']:
-        return self._load_atoms()
-
-    @property
-    def atoms_with_unique_symbol(self):
-        uni_atoms, uni_symbol = [], set()
-        for a in self.pseudo_atoms:
-            if a.symbol not in uni_symbol:
-                uni_atoms.append(a)
-                uni_symbol.add(a.symbol)
-
-        return uni_atoms
-
-    @property
-    def pseudo_atoms_with_unique_symbol(self):
-        uni_patoms, uni_psymbol = [], set()
-        for a in self.atoms:
-            if a.symbol not in uni_psymbol:
-                uni_patoms.append(a)
-                uni_psymbol.add(a.symbol)
-
-        return uni_patoms
-
-    @property
-    def all_atoms(self):
-        return self.atoms + self.pseudo_atoms
-
-    @property
-    def atom_charges(self) -> np.ndarray:
-        """ Return all atoms charges as a numpy array """
-        return np.array([a.partial_charge for a in self.atoms])
-
-    @property
-    def all_atom_charges(self) -> np.ndarray:
-        """ Return all atoms charges as a numpy array for every conformers """
-        all_atom_charges = self._data.get('all_atom_charges')
-        if isinstance(all_atom_charges, np.ndarray):
-            return all_atom_charges
-        return self.atom_charges.reshape((-1, self.atom_counts))
-
-    @property
-    def atom_indices(self) -> list[int]:
-        return [a.ob_id for a in self.atoms]
-
-    @property
-    def atom_labels(self) -> list[str]:
-        return [a.label for a in self.atoms]
-
-    @property
-    def atom_spin_densities(self) -> np.ndarray:
-        return np.array([a.spin_density for a in self.atoms])
-
-    @property
-    def all_atom_spin_densities(self):
-        all_atom_spin_densities = self._data.get('all_atom_spin_densities')
-        if all_atom_spin_densities is not None:
-            return all_atom_spin_densities
-        return self.atom_spin_densities.reshape((-1, self.atom_counts))
-
-    def assign_atoms_formal_charge(self):
-        """ Assign the formal charges for all atoms in the molecule """
-        self.add_hydrogens(balance_hydrogen=False)
-
-        for atom in self.atoms:
-            if atom.is_polar_hydrogen:
-                atom.formal_charge = 1
-            elif atom.is_hydrogen or atom.is_carbon:
-                atom.formal_charge = 0
-            elif atom.is_metal:
-                atom.formal_charge = _stable_charges[atom.symbol]
-            elif atom.symbol == 'S':
-                if not [a for a in atom.neighbours if a.symbol == 'O']:
-                    atom.formal_charge = atom.covalent_valence - 2
-                else:
-                    atom.formal_charge = 0
-            elif atom.symbol == 'P':
-                if not [a for a in atom.neighbours if a.symbol == 'O']:
-                    atom.formal_charge = atom.covalent_valence - 2
-                else:
-                    atom.formal_charge = 0
-            elif [a for a in atom.neighbours if a.is_polar_hydrogen]:
-                atom.formal_charge = -(len([a for a in atom.neighbours if a.is_polar_hydrogen]))
-            else:
-                atom.formal_charge = atom.covalent_valence - atom.stable_valence
-
-    def balance_hydrogens(self):
-        """ Add or remove hydrogens for make or heave atom to achieve the stable valence """
-        for a in self.heavy_atoms():
-            a.balance_hydrogen()
-
-    def bond(self, atom1: Union[int, str], atom2: Union[int, str], miss_raise: bool = False) -> 'Bond':
-        """
-        Return the Bond by given atom index labels in the bond ends
-        if the bond is missing in the molecule, return None if given miss_raise is False else raise a KeyError
-        Args:
-            atom1(int|str): index or label of atom in one of the bond end
-            atom2(int|str): index or label of atom in the other end of the bond
-            miss_raise(bool): Whether to raise error when can't find the bond
-
-        Returns:
-            Bond
-
-        Raises:
-            KeyError: when can't find the bond, and the miss_raise passing True
-
-        """
-        atom1: Atom = self.atom(atom1)
-        atom2: Atom = self.atom(atom2)
-        ob_bond = self.ob_mol.GetBond(atom1.ob_atom, atom2.ob_atom)
-
-        if ob_bond:
-            return Bond(ob_bond, self)
-
-    @property
-    def bond_pair_keys(self):
-        return [b.pair_key for b in self.bonds]
-
-    @property
-    def bonds(self):
-        bonds = self._load_bonds()
-        return list(bonds.values())
-
-    @property
-    def bonds_dict(self) -> Dict[int, 'Bond']:
-        return self._load_bonds()
-
-    def build_2d(self):
-        """ build 2d conformer """
-        pmol = pb.Molecule(self.ob_mol)
-        pmol.make2D()
-
-    def build_3d(self, force_field: str = 'UFF', steps: int = 500):
-        """ build 3D coordinates for the molecule """
-        # Preserve atoms data before building
-        preserve_data = self._preserve_atoms_data()
-
-        # Destroy atoms and bonds wrappers
-        self._data['atoms'] = {}
-        self._data['bonds'] = {}
-
-        # Build 3d conformer
-        pymol = pb.Molecule(self.ob_mol)
-        pymol.make3D(force_field, steps)
-
-        # Reload atoms and bonds
-        self._load_atoms()
-        self._load_bonds()
-
-        # Transfer preserve data to new
-        self._transfer_preserve_data_to_new_atoms(self, preserve_data)
-        # Delete temp label
-        self._delete_atom_temp_label()
-
-        # Remove redundant hydrogen or supply the lack hydrogens
-        self.balance_hydrogens()
-
-    def build_bonds(self):
-        self.ob_mol.ConnectTheDots()
-
-    @property
-    def center_of_masses(self):
-        return (self.masses * self.coordinates.T).T.sum(axis=0) / self.masses.sum()
-
-    @property
-    def center_of_shape(self):
-        return self.coordinates.mean(axis=0)
-
-    @property
-    def charge(self):
-        return self.ob_mol.GetTotalCharge()
-
-    @charge.setter
-    def charge(self, charge):
-        self._set_mol_charge(charge)
-
-    def clean_bonds(self):
-        """ Remove all bonds """
-        # Iterate directly will fail.
-        ob_bonds = [ob_bond for ob_bond in ob.OBMolBondIter(self.ob_mol)]
-        for ob_bond in ob_bonds:
-            self.ob_mol.DeleteBond(ob_bond)
-
-    def clean_conformers(self, pop: bool = False):
-        """ clean all config save inside the molecule """
-        try:
-            all_coordinates = self._data.pop('all_coordinates')
-        except KeyError:
-            all_coordinates = None
-
-        if pop:
-            return all_coordinates
-
-    @property
-    def components(self):
-        """ get all fragments don't link each by any bonds """
-        # Add temp label for each atom first
-        preserve_data = self._preserve_atoms_data()
-
-        components = [self.__class__(obc) for obc in self.ob_mol.Separate()]
-
-        # Transfer the parent data attr to the children
-        for c in components:
-            for a in c.atoms:
-                a.update_attr_data(preserve_data[a.temp_label])
-                a.remove_ob_data('temp_label')
-
-        # remove temp labels of all atoms
-        self._delete_atom_temp_label()
-
-        return components
-
-    @property
-    def conformer_counts(self) -> int:
-        """ The number of conformers in the molecule """
-        all_coordinates = self._data.get('all_coordinates')
-        if isinstance(all_coordinates, np.ndarray):
-            return all_coordinates.shape[0]
-        else:
-            return 1
-
-    def conformer_select(self, conf_idx: int):
-        """ select specific conformer by index """
-
-        def assign_numpy_attrs(attrs_name: str, setter: Callable):
-            attrs = self._data.get(attrs_name)
-            if isinstance(attrs, np.ndarray):
-                try:
-                    attr = attrs[conf_idx]
-                except IndexError:
-                    attr = None
-            else:
-                attr = None
-
-            if isinstance(attr, np.ndarray) or attr:
-                setter(attr)
-
-        all_coordinates = self._data.get('all_coordinates')
-        if all_coordinates is None and conf_idx:
-            raise IndexError('Only one conformer here!')
-
-        # assign the coordinates for the molecule
-        coordinates = all_coordinates[conf_idx]
-        self._assign_coordinates(self, coordinates)
-
-        assign_numpy_attrs('all_energy', self._set_energy)
-
-        assign_numpy_attrs('all_atom_charges', self._set_atom_charges)
-
-        assign_numpy_attrs('all_atom_spin_densities', self._set_atom_spin_densities)
-
-        assign_numpy_attrs('all_forces', self._set_forces)
-
-    @property
-    def coordinates(self) -> np.ndarray:
-        """
-        Get the matrix of all atoms coordinates,
-        where the row index point to the atom index;
-        the column index point to the (x, y, z)
-        """
-        return np.array([atom.coordinates for atom in self.atoms], dtype=np.float64)
-
-    def copy(self) -> 'Molecule':
-        """ Get a clone of this Molecule """
-        clone = self.__class__(self.ob_copy())
-        clone._load_atoms()
-        clone._load_bonds()
-
-        # Copy the Molecule's attr data to the clone one
-        clone.update_attr_data(self.data)
-        # Copy the Atoms' attr data to the clone ones
-        for atom in clone.atoms:
-            atom.update_attr_data(self.atoms_dict[atom.ob_id].data)
-            atom.molecule = clone
-        # Copy the Bonds' attr data to the lone ones
-        for bond in clone.bonds:
-            bond.update_attr_data(self.bonds_dict[bond.ob_id].data)
-            bond.molecule = clone
-
-        return clone
-
-    def compact_crystal(self, inplace=False):
-        """"""
-        mol = self if inplace else self.copy()
-        lattice_params = np.concatenate((self.xyz_diff, [90., 90., 90.]))
-
-        mol.make_crystal(*lattice_params)
-
-        return mol
-
-    def create_crystal_by_vectors(
-            self,
-            va: Union[Sequence, np.ndarray],
-            vb: Union[Sequence, np.ndarray],
-            vc: Union[Sequence, np.ndarray]
-    ):
-        """ Create a new crystal with specified cell vectors for the Molecule """
-        self._create_ob_unit_cell()
-        self.crystal().set_vectors(va, vb, vc)
-
-    def create_crystal_by_matrix(self, matrix: np.ndarray):
-        """ Create a new crystal with specified cell matrix for the molecule """
-        if not (np.logical_not(matrix >= 0.).any() and np.logical_not(matrix < 0.).any()) and np.linalg.det(matrix):
-            self._create_ob_unit_cell()
-            self.crystal().set_matrix(matrix)
-            # self.crystal().space_group = 'P1'
-
-    @classmethod
-    def create_aCryst_by_mq(
-            cls, elements: Dict[str, float], force_field: Union[str, os.PathLike],
-            density: float = 1.0, a: float = 25., b: float = 25., c: float = 25.,
-            alpha: float = 90., beta: float = 90., gamma: float = 90., time_step: float = 0.0001,
-            origin_temp: float = 298.15, melt_temp: float = 4000., highest_temp: float = 10000.,
-            ff_args: Sequence = (), path_writefile: Optional[str] = None, path_dump_to: Optional[str] = None,
-            dump_every: int = 100
-    ):
-        """
-        Create a Amorphous crystal materials by Melt-Quench process.
-        This process is performed by LAMMPS package, make sure the LAMMPS is accessible.
-        A suitable force field is required for the process are performed correctly.
-        Args:
-            elements(dict[str, float]): Dict of elements and their composition ratio
-            force_field(str, os.PathLike): The name of force filed or the path to load a force filed. The name
-             of the force filed is refer to the relative path to the 'hotpot_root/data/force_field'.
-            density: the demand density for the created amorphous crystal
-            a: the length of a vector in the crystal
-            b: the length of b vector in the crystal
-            c: the length of c vector in the crystal
-            alpha: alpha angle of crystal param.
-            beta: beta angle of crystal param.
-            gamma: gamma angle of crystal param
-            time_step: time interval between path integrals when performing melt-quench
-            origin_temp: the initial temperature before melt
-            melt_temp: the round melting point to the materials
-            highest_temp: the highest temperature to liquefy the materials
-            ff_args: the arguments the force file requried, refering the LAMMPS pair_coeff:
-             "pair_coeff I J args" url: https://docs.lammps.org/pair_coeff.html
-            path_writefile: the path to write the final material (screenshot) to file, if not specify, not save.
-            path_dump_to:  the path to save the trajectory of the melt-quench process, if not specify not save.
-            dump_every: the step interval between each dump operations
-
-        Returns:
-            Molecule, a created amorphous material
-        """
-        return cls._melt_quench(
-            elements=elements, force_field=force_field, density=density,
-            a=a, b=b, c=c, alpha=alpha, beta=beta, gamma=gamma, time_step=time_step,
-            origin_temp=origin_temp, melt_temp=melt_temp, highest_temp=highest_temp,
-            ff_args=ff_args, path_writefile=path_writefile, path_dump_to=path_dump_to,
-            dump_every=dump_every
-        )
-
-    @property
-    def critical_pressure(self):
-        return self._get_critical_params('pressure')
-
-    @property
-    def critical_temperature(self):
-        return self._get_critical_params('temperature')
-
-    def crystal(self):
-        """ Get the Crystal containing the Molecule """
-        cell_index = ob.UnitCell  # Get the index the UnitCell data save
-        cell_data = self.ob_mol.GetData(cell_index)
-
-        if cell_data:
-            ob_unit_cell = ob.toUnitCell(cell_data)
-            return Crystal(ob_unit_cell, molecule=self)
-        else:
-            return None
-
-    def dump(self, fmt: str, *args, **kwargs) -> Union[str, bytes, dict, 'DeepSystem']:
-        """"""
-        dumper = Dumper(fmt=fmt, source=self, *args, **kwargs)
-        return dumper()
-
-    @property
-    def elements(self) -> list[str]:
-        return re.findall(r'[A-Z][a-z]*', self.formula)
-
-    @property
-    def energy(self):
-        """ Return energy with kcal/mol as default """
-        return self.ob_mol.GetEnergy()
-
-    def feature_matrix(self, *feature_names: Sequence) -> np.ndarray:
-        """ Retrieve the feature matrix (collections of feature vector for atoms),
-         The default feature is `atomic_orbital`, if the feature names not be specified, the `atomic_orbital` will be
-         retrieved.
-         Args:
-             feature_names: the feature names are offered in hotpot/data/periodic_table.json
-         """
-        if not feature_names:
-            feature_names = ('atomic_orbital',)
-
-        # Matrix with shape (atom_numbers, feature_length)
-        return np.stack([atom.element_features(*feature_names) for atom in self.atoms])
-
-    def fingerprint(self, fptype: Literal['FP2', 'FP3', 'FP4', 'MACCS'] = 'FP2'):
-        """
-        Calculate the molecular fingerprint for this molecule, the supporting fingerprint include:
-
-        1. "FP2": The FP2 fingerprint is a path-based fingerprint that encodes the presence of linear
-        fragments up to 7 atoms long. It is a 1024-bit fingerprint and is commonly used for substructure
-        searches and similarity calculations.
-
-        2. "FP3": The FP3 fingerprint is designed for searching 3D conformations, such as those found
-        in protein-ligand complexes. It encodes the presence of particular pharmacophoric features,
-        such as hydrogen bond donors, acceptors, and hydrophobic regions.
-
-        3. "FP4": The FP4 fingerprint is a circular fingerprint based on the Morgan algorithm. It
-        captures information about the local environment of each atom in the molecule, up to a certain
-        radius. It is useful for similarity calculations and machine learning tasks.
-
-        4. "MACCS": The MACCS fingerprint is a 166-bit structural key-based fingerprint. It represents
-        the presence of specific substructures or functional groups defined by the MACCS keys. It is
-        commonly used for similarity calculations and substructure searches.
-
-        Return:
-            the Fingerprint object in pybel module
-        """
-        return pb.Molecule(self.ob_mol).calcfp(fptype)
-
-    @property
-    def forces(self):
-        """ return the all force vectors for all atoms in the molecule """
-        return np.vstack((atom.force_vector for atom in self.atoms))
-
-    @property
-    def all_forces(self):
-        """ the force matrix for all conformer """
-        force_matrix = self._data.get("all_forces")
-        if isinstance(force_matrix, np.ndarray):
-            return force_matrix
-        return self.forces
-
-    @property
-    def formula(self) -> str:
-        return self.ob_mol.GetSpacedFormula()
-
-    def gaussian(
-            self,
-            g16root: Union[str, PathLike],
-            link0: Union[str, List[str]],
-            route: Union[str, List[str]],
-            path_log_file: Union[str, PathLike] = None,
-            path_err_file: Union[str, PathLike] = None,
-            inplace_attrs: bool = False,
-            *args, **kwargs
-    ) -> (Union[None, str], str):
-        """
-        calculation by Gaussian.
-        for running the method normally, MAKE SURE THE Gaussian16 HAVE BEEN INSTALLED AND ALL ENV VAR SET RITHT !!
-        Args:
-            g16root: the dir Gaussian16 software installed
-            link0: the link0 command in gjf script
-            route: the route command in gjf script
-            path_log_file: Optional, the path to save the out.log file. If not given, the logfile won't be write
-             to disk
-            path_err_file: optional, the path to save the error log file. If not given, the err file won't be write
-             to disk
-            inplace_attrs: Whether to inplace self attribute according to the results from attributes
-            *args:
-            **kwargs:
-
-        Returns:
-            the standard output of g16 log file(string), the standard output of g16 err file(string)
-        """
-        # For 2d molecule, build its confomer by universal force field first
-        if not self.has_3d:
-            self.build_3d()
-
-        # TODO: Preserve for restart when encounter a Gaussian error.
-        chk_path = None
-        if isinstance(link0, List):
-            for l0 in link0:
-                if re.match(r'%chk=.+\.chk', l0):
-                    chk_path = l0[5:]
-                    break
-
-        # Make the input gjf script
-        script = self.dump('gjf', *args, link0=link0, route=route, **kwargs)
-
-        # Run Gaussian16
-        with Gaussian(g16root) as gaussian:
-
-            try:
-                stdout, stderr = gaussian.run(script)
-
-                # save the calculate result into the molecule data dict
-                self._data['gaussian_output'] = stdout
-                self._data['gaussian_parse_data'] = gaussian.parse_log(stdout)
-
-                # Inplace the self attribute according to the result from gaussian
-                if inplace_attrs:
-                    self._set_attrs(**gaussian.molecule_setter_dict(stdout))
-
-                # Save log file when the path_log_file has been specified
-                if path_log_file:
-                    with open(path_log_file, 'w') as writer:
-                        writer.write(stdout)
-
-                # return results and error info
-                return stdout, stderr
-
-            # If got an error message, save the error and stdout file, before raise the error
-            except GaussianRunError:
-                stdout, stderr = gaussian.stdout, gaussian.stderr
-
-                # Save error file
-                if not path_err_file:
-                    path_err_file = Path(f'{self.formula}.err')
-                with open(path_err_file, 'w') as writer:
-                    writer.write(stderr)
-
-                # Save log file
-                if not path_log_file:
-                    path_log_file = Path(f'{self.formula}.log')
-                with open(path_log_file, 'w') as writer:
-                    writer.write(stdout)
-
-                raise GaussianRunError(stderr)
-
-    def gcmc(
-            self, *guest: 'Molecule', force_field: Union[str, os.PathLike] = None,
-            work_dir: Union[str, os.PathLike] = None, T: float = 298.15, P: float = 1.0, **kwargs
-    ):
-        """
-        Run gcmc to determine the adsorption of guest,
-        Args:
-            self: the framework as the sorbent of guest molecule
-            guest(Molecule): the guest molecule to be adsorbed into the framework
-            force_field(str|PathLike): the path to force field file or the self-existent force file contained
-             in force field directory (in the case, a str should be given as a relative path from the root of
-             force field root to the specified self-existent force filed). By default, the force field is UFF
-             which in the relative path 'UFF/LJ.json' for the force field path.
-            work_dir: the user-specified dir to store the result of GCMC and log file.
-            T: the environmental temperature (default, 298.15 K)
-            P: the relative pressure related to the saturation vapor in the environmental temperature.
-        """
-        from tanks.lmp.gcmc import LjGCMC
-        gcmc = LjGCMC(self, force_field, *guest, work_dir=work_dir, T=T, P=P, **kwargs)
-        return gcmc.run()
-
-    def gcmc_for_isotherm(
-            self, *guest: 'Molecule', force_field: Union[str, os.PathLike] = None,
-            work_dir: Union[str, os.PathLike] = None, T: float = 298.15,
-            Ps: Sequence[float] = (1.0,), **kwargs
-    ):
-        """
-        Run gcmc to determine the adsorption of guest,
-        Args:
-            self: the framework as the sorbent of guest molecule
-            guest(Molecule): the guest molecule to be adsorbed into the framework
-            force_field(str|PathLike): the path to force field file or the self-existent force file contained
-             in force field directory (in the case, a str should be given as a relative path from the root of
-             force field root to the specified self-existent force filed). By default, the force field is UFF
-             which in the relative path 'UFF/LJ.json' for the force field path.
-            work_dir: the user-specified dir to store the result of GCMC and log file.
-            T: the environmental temperature (default, 298.15 K)
-            Ps(Sequence[float]): A sequence of relative pressure related to the saturation vapor in the environmental temperature.
-        """
-        if isinstance(work_dir, str):
-            work_dir = Path(work_dir)
-
-        if not work_dir.exists():
-            work_dir.mkdir()
-
-        for P in Ps:
-            sub_work_dir = work_dir.joinpath('press_' + str(P))
-            if not sub_work_dir.exists():
-                sub_work_dir.mkdir()
-
-            self.gcmc(*guest, force_field=force_field, work_dir=sub_work_dir, T=T, P=P, **kwargs)
-
-    def generate_metal_ligand_pair(
-            self, metal_symbol: str,
-            acceptor_atoms: Sequence = ('O',),
-            opti_force_field: str = 'UFF',
-            opti_before_gen: bool = False,
-            opti_step: int = 500
-    ) -> Generator['Molecule', None, None]:
-        """
-        This method could work if the molecule is an organic ligand, or raise AttributeError.
-        Generate metal-ligand pair by link metal with acceptor atoms in the organic ligand.
-
-        Args:
-            metal_symbol: which metal element link to the ligand
-            acceptor_atoms: which elements to be acceptor atom to link to metal
-            opti_force_field: which force field could be used to optimize the configuration of ligand and M-L pair.
-            opti_before_gen: whether to optimize the ligand conformer before generate pair
-            opti_step: the step to optimize the 3d conformer
-
-        Return:
-            A generator for M-L pair
-        """
-        ligand = self.copy()
-
-        if opti_before_gen:
-            ligand.build_3d(force_field=opti_force_field, steps=opti_step)
-
-        for atom in ligand.atoms:
-            if atom.symbol in acceptor_atoms:
-                # copy the ligand as the embryo of metal-ligand pairs
-                pair = ligand.copy()
-
-                # Replace the correspondent atom in the pair embryo, i.e., the accepting atom
-                acc_atom = pair.atom(atom.ob_id)
-
-                # assign the initial coordinates, if the pair has 3d conformer
-                # the sum of vector of relative position relate to the accepting atom
-                if pair.has_3d:
-                    sum_relative_coordinates = sum([c for _, c in acc_atom.neighbours_position])
-                    metal_init_coordinates = acc_atom.coordinates_array - sum_relative_coordinates
-
-                    # add metal atom into the acceptor_ligand
-                    added_metal = pair.add_atom(metal_symbol, coordinates=metal_init_coordinates)
-
-                else:  # If the pair has not 3d conformer, add the metal directly
-                    added_metal = pair.add_atom(metal_symbol)
-
-                # add the coordinating bond between metal atom and acceptor atoms
-                pair.add_bond(added_metal, acc_atom, 0)
-
-                # localize optimization of M-L pair by classical force field, if the pair has 3d
-                if pair.has_3d:
-                    pair.localed_optimize(opti_force_field)
-                else:
-                    pair.add_hydrogens()  # Add hydrogens
-
-                pair.identifier = pair.smiles
-                yield pair
-
-    def generate_pairs_bundle(
-            self, metal_symbol: str,
-            acceptor_atoms: Sequence = ('O',),
-            opti_force_field: str = 'UFF',
-            opti_before_gen: bool = False,
-            opti_step: int = 500
-    ) -> 'PairBundle':
-        """
-        Generate metal-ligand pairs by bind this ligand with proposed, and put this ligand, metal and all pairs,
-        which are assembled by the ligand and metal, into a PairBundle objects.
-        Args:
-            metal_symbol(str): the symbol of proposed metal
-            acceptor_atoms(Sequence): the atoms to form bond with the proposed metal, the default is Oxygen
-            opti_force_field(str): the force field to optimize the conformer of this ligand and the generated
-             pairs.
-            opti_before_gen: whether to optimize the ligand conformer before generate pair.
-            opti_step: the step to optimize the 3d conformer
-
-        Returns:
-            PairBundle with this ligand, proposed metal and the pairs
-        """
-        return PairBundle(
-            metal=Atom(symbol=metal_symbol),
-            ligand=self,
-            pairs=list(self.generate_metal_ligand_pair(
-                metal_symbol,
-                acceptor_atoms,
-                opti_force_field,
-                opti_before_gen
-            )),
-        )
-
-    def graph_representation(self, *feature_names):
-        return self.identifier, self.feature_matrix(*feature_names), self.link_matrix
-
-    def heavy_atoms(self):
-        """ Get the atoms except for hydrogens """
-        return [a for a in self.atoms if a.is_heavy]
-
-    @property
-    def has_3d(self):
-        """ Whether atoms in the molecule have 3d coordinates """
-        return self.ob_mol.Has3D()
-
-    @property
-    def has_hydrogen_added(self):
-        """ Have hydrogens been added to the molecule by call Molecule.add_hydrogen()? """
-        return self.ob_mol.HasHydrogensAdded()
-
-    @property
-    def has_unknown_bond(self):
-        return any(not b.type for b in self.bonds)
-
-    @property
-    def hydrogens(self):
-        return [a for a in self.atoms if a.is_hydrogen]
-
-    @property
-    def identifier(self):
-        return self.ob_mol.GetTitle()
-
-    @identifier.setter
-    def identifier(self, value):
-        self.ob_mol.SetTitle(value)
-
-    @property
-    def identifier_array(self) -> np.ndarray:
-        """ numpy.array of identifiers has the same number of items with the number of conformers """
-        idt_array = self._data.get('identifier_array')
-        if not isinstance(idt_array, np.ndarray):
-            idt_array = []
-            for i, c in enumerate(self.all_coordinates):
-                idt_array.append(f'{self.identifier}_c{i}')
-            self._data['identifier_array'] = idt_array = np.array(idt_array)
-
-        return idt_array
-
-    def iadd_accessible(self, other):
-        if self.atomic_numbers == other.atomic_numbers:
-            return True
-        return False
-
-    @property
-    def inchi(self):
-        return self.dump('inchi').strip()
-
-    @property
-    def is_disorder(self):
-        """ To judge whether this Molecule has disorder bonds """
-        if self.has_3d:
-            if any(not (0.85 < b.length/b.ideal_length < 1.15) for b in self.bonds):
-                return True
-        return False
-
-    @property
-    def is_labels_unique(self):
-        """ Determine whether all atom labels are unique """
-        return len(set(self.labels)) == self.atom_counts
-
-    @property
-    def is_organic(self):
-        """ To judge whether the molecule is organic, an organic compound is with carbon atoms and without metal """
-        if any(a.is_metal for a in self.atoms):
-            return False
-        elif any(a.symbol == 'C' for a in self.atoms):
-            return True
-
-        return False
-
-    def ob_copy(self):
-        """ Return a clone of OBMol of the Molecule """
-        return ob.OBMol(self.ob_mol)
-
-    @property
-    def ob_mol(self):
-        return self._data['ob_obj']
-
-    def ob_mol_pop(self):
-        data: dict = self._data
-
-        atoms: Dict[int, Atom] = data.get('atoms')
-        if atoms:
-            for ob_id, atom in atoms.items():
-                atom.ob_atom_pop()
-
-        bonds: Dict[int, Bond] = data.get('bonds')
-        if bonds:
-            for ob_idx, bond in bonds.items():
-                bond.ob_bond_pop()
-
-        return self._data.pop('ob_obj')
-
-    def ob_mol_rewrap(self, ob_mol: ob.OBMol):
-        if not isinstance(ob_mol, ob.OBMol):
-            raise TypeError('the ob_mol should be OBMol object')
-
-        atoms = self._data.get('atoms')
-        bonds = self._data.get('bonds')
-
-        if any(oba.GetId() not in atoms for oba in ob.OBMolAtomIter(ob_mol)):
-            raise ValueError('the atom number between the wrapper and the core OBMol is not match')
-        if any(obb.GetId() not in bonds for obb in ob.OBMolBondIter(ob_mol)):
-            raise ValueError('the bond number between the wrapper and the core OBMol is not match')
-
-        self._data['ob_obj'] = ob_mol
-        for ob_atom in ob.OBMolAtomIter(ob_mol):
-            atom = atoms.get(ob_atom.GetId())
-            atom.ob_atom_rewrap(ob_atom)
-
-        for ob_bond in ob.OBMolBondIter(ob_mol):
-            bond = bonds.get(ob_bond.GetId())
-            bond.ob_bond_rewrap(ob_bond)
-
-    @property
-    def labels(self):
-        return [a.label for a in self.atoms]
-
-    @property
-    def lmp(self):
-        """ handle to operate the Lammps object """
-        return self._data.get('lmp')
-
-    def lmp_close(self):
-        pop_lmp = self._data.pop('lmp')
-        pop_lmp.close()
-
-    def lmp_setup(self, **kwargs):
-        self._data['lmp'] = lmp.HpLammps(self, **kwargs)
-
-    @property
-    def link_matrix(self):
-        return np.array([[b.ob_atom1_id, b.ob_atom2_id] for b in self.bonds]).T
-
-    def localed_optimize(self, force_field: str = 'UFF', steps: int = 500):
-        """ Locally optimize the coordinates. seeing openbabel.pybel package """
-        pymol = pb.Molecule(self.ob_mol)
-        pymol.localopt(force_field, steps)
-        self.balance_hydrogens()
-
-    def make_crystal(self, a: float, b: float, c: float, alpha: float, beta: float, gamma: float) -> 'Crystal':
-        """ Put this molecule into the specified crystal """
-        ob_unit_cell = ob.OBUnitCell()
-
-        self.ob_mol.CloneData(ob_unit_cell)
-        self.crystal().ob_unit_cell.SetData(a, b, c, alpha, beta, gamma)
-        self.crystal().ob_unit_cell.SetSpaceGroup('P1')
-
-        return self.crystal()
-
-    @property
-    def masses(self) -> np.ndarray:
-        return np.array([a.mass for a in self.atoms])
-
-    def melt_quench(
-            self, elements: Dict[str, float], force_field: Union[str, os.PathLike],
-            density: float = 1.0, a: float = 25., b: float = 25., c: float = 25.,
-            alpha: float = 90., beta: float = 90., gamma: float = 90., time_step: float = 0.0001,
-            origin_temp: float = 298.15, melt_temp: float = 4000., highest_temp: float = 10000.,
-            ff_args: Sequence = (), path_writefile: Optional[str] = None, path_dump_to: Optional[str] = None,
-            dump_every: int = 100
-    ):
-        """
-        Create an Amorphous crystal materials by performing Melt-Quench process for this materials.
-        This process is performed by LAMMPS package, make sure the LAMMPS is accessible.
-        A suitable force field is required for the process are performed correctly.
-        Args:
-            elements(dict[str, float]): Dict of elements and their composition ratio
-            force_field(str, os.PathLike): The name of force filed or the path to load a force filed. The name
-             of the force filed is refer to the relative path to the 'hotpot_root/data/force_field'.
-            density: the demand density for the created amorphous crystal
-            a: the length of a vector in the crystal
-            b: the length of b vector in the crystal
-            c: the length of c vector in the crystal
-            alpha: alpha angle of crystal param.
-            beta: beta angle of crystal param.
-            gamma: gamma angle of crystal param
-            time_step: time interval between path integrals when performing melt-quench
-            origin_temp: the initial temperature before melt
-            melt_temp: the round melting point to the materials
-            highest_temp: the highest temperature to liquefy the materials
-            ff_args: the arguments the force file requried, refering the LAMMPS pair_coeff:
-             "pair_coeff I J args" url: https://docs.lammps.org/pair_coeff.html
-            path_writefile: the path to write the final material (screenshot) to file, if not specify, not save.
-            path_dump_to:  the path to save the trajectory of the melt-quench process, if not specify not save.
-            dump_every: the step interval between each dump operations
-
-        Returns:
-            Molecule, a created amorphous material
-        """
-        return self._melt_quench(
-            elements=elements, force_field=force_field, density=density,
-            a=a, b=b, c=c, alpha=alpha, beta=beta, gamma=gamma, time_step=time_step,
-            origin_temp=origin_temp, melt_temp=melt_temp, highest_temp=highest_temp,
-            ff_args=ff_args, path_writefile=path_writefile, path_dump_to=path_dump_to,
-            dump_every=dump_every, mol=self
-        )
-
-    @property
-    def metals(self) -> List['Atom']:
-        return [a for a in self.atoms if a.is_metal]
-
-    @property
-    def mol_orbital_energies(self):
-        energies = self._data.get('mol_orbital_energies')
-        if energies:
-            return energies
-        else:
-            return None
-
-    def normalize_labels(self):
-        """ Reorder the atoms labels in the molecule """
-        element_counts = {}
-        for atom in self.atoms:
-            count = element_counts.get(atom.symbol, 0)
-            count += 1
-            element_counts[atom.symbol] = count
-            atom.label = f'{atom.symbol}{count}'
-
-    def perturb_atoms_coordinates(
-            self,
-            random_style='uniform',
-            mol_distance=0.5,
-            freeze_dim: Sequence[int] = (),
-            max_generate_num: int = 10,
-            inplace: bool = False
-    ) -> Generator["Molecule", None, None]:
-        """
-        Perturb the coordinate of atom in the molecule
-        generate new mol
-        Args:
-            random_style: how to sample, 'uniform' or 'normal'
-            mol_distance: the max distance of perturbation in 'uniform'; the square variance in 'normal'
-            freeze_dim: tuple of int or str, 0 = x, 1 = y, 2 = z
-            max_generate_num: the maximum of generated molecule
-            inplace
-
-        Returns:
-            Generator of perturbed molecule
-        """
-        dim_transform = {'x': 0, 'y': 1, 'z': 2}
-
-        coordinates_shape = (self.atom_counts, 3)  # the shape of coordinates matrix (atom counts, 3 dimension)
-        origin_coordinates = self.coordinates
-
-        def coordinates_generator():
-            """ Generating """
-            for _ in range(max_generate_num):
-                if random_style == 'uniform':
-                    perturb_matrix = np.float64(np.random.uniform(-mol_distance, mol_distance, coordinates_shape))
-                elif random_style == 'normal':
-                    perturb_matrix = np.float64(np.random.normal(0, mol_distance, coordinates_shape))
-                else:
-                    raise ValueError('the perturb style is not defined!')
-
-                if freeze_dim:
-                    dim = [
-                        i if (isinstance(i, int) and 0 <= i <= 3) else dim_transform[i]
-                        for i in freeze_dim
-                    ]
-
-                    perturb_matrix[:, dim] = 0.
-
-                new_coord = origin_coordinates + perturb_matrix
-
-                yield new_coord
-
-        if inplace:
-            origin_all_coordinates = self._data.get('all_coordinates')
-            new_all_coordinates = np.array([c for c in coordinates_generator()])
-
-            if origin_all_coordinates is not None:
-                self._data['all_coordinates'] = np.concatenate([origin_all_coordinates, new_all_coordinates])
-            else:
-                self._data['all_coordinates'] = np.concatenate(
-                    [np.reshape(origin_coordinates, (1,) + origin_coordinates.shape), new_all_coordinates]
-                )
-
-        else:
-            return (self._pert_mol_generate(c) for c in coordinates_generator())
-
-    def perturb_cell_params(self):
-        """ To perturb parameters, i.e., a, b, c, alpha, beta, gamma """
-
-    @property
-    def pseudo_atoms(self):
-        return self._data.get('pseudo_atoms', [])
-
-    def quick_build_atoms(self, atomic_numbers: np.ndarray):
-        """
-        This method to quick build atoms according an array of atomic numbers.
-        The method bypass to calling more time-consumed method: add_atom().
-        However, the method only assign the elements or atomic number for atoms,
-        more fine attributes like coordinates, can't be specified.
-        Args:
-            atomic_numbers(np.ndarray): 1-D numpy array to add new atoms into the molecule
-
-        Returns:
-            None
-        """
-        if not isinstance(atomic_numbers, (np.ndarray, Sequence)):
-            raise TypeError('the atomic_numbers should be np.ndarray or Sequence')
-        if isinstance(atomic_numbers, np.ndarray) and len(atomic_numbers.shape) != 1:
-            raise ValueError('the numpy array must be 1-D')
-
-        for atomic_number in atomic_numbers:
-            ob_atom = ob.OBAtom()
-            ob_atom.SetAtomicNum(int(atomic_number))
-            self.ob_mol.AddAtom(ob_atom)
-
-    @classmethod
-    def read_from(cls, source: Union[str, PathLike, IOBase], fmt=None, *args, **kwargs) -> 'Molecule':
-        """
-        read source to the Molecule obj by call _io.Parser class
-        Args:
-            source(str, PathLike, IOBase): the formatted source
-            fmt:
-            *args:
-            **kwargs:
-
-        Returns:
-
-        """
-        if not fmt:
-            if isinstance(source, str):
-                source = Path(source)
-
-            if isinstance(source, Path):
-                fmt = source.suffix.strip('.')
-            else:
-                raise ValueError(f'the arguments should be specified for {type(source)} source')
-
-        mol = Parser(fmt, source, *args, **kwargs)()  # initialize parser object and call self
-
-        # Specify the mol identifier if it's None
-        if isinstance(mol, Molecule) and not mol.identifier:
-            mol.identifier = str(source)
-
-        return mol
-
-    def register_critical_params(self, name: str, temperature: float, pressure: float, acentric: float):
-        """ Register new critical parameters into the critical parameters sheet """
-        data = json.load(open(opj(data_root, 'thermo', 'critical.json')))
-        data[self.smiles] = {'name': name, 'temperature': temperature, 'pressure': pressure, 'acentric': acentric}
-        with open(opj(data_root, 'thermo', 'critical.json'), 'w') as writer:
-            json.dump(data, writer, indent=True)
-
-    def remove_atoms(self, *atoms: Union[int, str, 'Atom'], remove_hydrogens: bool = False) -> None:
-        """
-        Remove atom according to given atom index, label or the atoms self.
-        Args:
-            atoms(int|str|Atom): the index, label or self of Removed atom
-            remove_hydrogens(bool): remove the hydrogens connecting in the atoms synchronously.
-
-        Returns:
-            None
-        """
-        for atom in atoms:
-
-            # Check and locate the atom
-            if isinstance(atom, int):
-                atom = self.atoms_dict[atom]
-            elif isinstance(atom, str):
-                atom = self.atom(atom)
-            elif isinstance(atom, Atom):
-                if not (atom.molecule is self):
-                    raise AttributeError('the given atom not in the molecule')
-            else:
-                raise TypeError('the given atom should be int, str or Atom')
-
-            # remove connecting hydrogens
-            if remove_hydrogens:
-                for nh in atom.neighbours_hydrogen:
-                    self.ob_mol.DeleteAtom(nh.ob_atom)
-
-            # Removing the atom
-            self.ob_mol.DeleteAtom(atom.ob_atom)
-            atom._data['mol'] = None
-
-        # Reload atoms
-        self._load_atoms()
-        self._load_bonds()
-
-    def remove_bonds(self, *bonds: 'Bond'):
-        """ Remove the bonds in the molecule """
-        for bond in bonds:
-            successful = self.ob_mol.DeleteBond(bond.ob_bond)
-            if not successful:
-                raise RuntimeError(f'Fail to remove {bonds}')
-
-        self._load_bonds()
-
-    def remove_hydrogens(self):
-        self.ob_mol.DeleteHydrogens()
-
-    def remove_metals(self):
-        """ remove all of metal atoms in the molecule """
-        self.remove_atoms(*self.metals)
-
-    def remove_solvents(self, remove_disorder: bool = True, remove_isolate_atoms: bool = True):
-        """ remove all solvents in the molecule """
-        self.normalize_labels()
-        for i, ligand in enumerate(self.retrieve_ligands()):
-            if remove_disorder and ligand.is_disorder:  # remove disorder molecular structures first
-                self.remove_atoms(*ligand.atom_labels, remove_hydrogens=False)
-            elif remove_isolate_atoms and len(ligand.atoms) == 1:
-                self.remove_atoms(*ligand.atom_labels, remove_hydrogens=False)
-            elif _lib.get('Solvents').is_solvent(ligand):  # To judge if the ligand is solvents
-                self.remove_atoms(*ligand.atom_labels, remove_hydrogens=False)
-
-    def retrieve_ligands(self) -> List['Molecule']:
-        """ Retrieve all ligand molecule from this """
-        clone = self.copy()
-        clone.remove_metals()
-
-        return clone.components
-
-    def retrieve_metal_ligand_pairs(self) -> List['Molecule']:
-        """ Retrieve all clone of metal-ligand pairs in the molecule """
-        if not self.is_labels_unique:
-            self.normalize_labels()
-
-        ml_pairs = []
-        for metal, ligand in product(self.metals, self.retrieve_ligands()):
-            if set(metal.neighbours_label) & set(ligand.atom_labels):
-                pair = self.copy()
-
-                # Remove all the atoms is not the metal and not on the ligand
-                other_atoms = [a for a in pair.atoms if a.label != metal.label and a.label not in ligand.atom_labels]
-                pair.remove_atoms(*other_atoms, remove_hydrogens=False)
-
-                ml_pairs.append(pair)
-
-        return ml_pairs
-
-    @property
-    def rotatable_bonds_number(self):
-        return self.ob_mol.NumRotors()
-
-    def save_2d_img(self, file_path: Union[str, os.PathLike], **kwargs):
-        """
-        Export 2d image to file
-        Args:
-            file_path:
-            **kwargs: other keywords arguments for 2d image make and save
-
-        Keyword Args:
-
-        """
-        img = self.to_2d_img(**kwargs)
-        img.save(file_path)
-
-    def set(self, **kwargs):
-        """ Set the attributes directly """
-        self._set_attrs(**kwargs)
-
-    def set_label(self, ob_id: int, label: str):
-        self.atoms_dict[ob_id].label = label
-
-    def similarity(self, other: 'Molecule', fptype: Literal['FP2', 'FP3', 'FP4', 'MACCS'] = 'FP2') -> int:
-        """
-        Compare the similarity with other molecule, based on specified fingerprint
-        Args:
-            other(Molecule): the other Molecule
-            fptype(str): the fingerprint type to perform comparison of similarity
-
-        Return:
-            the similarity(int)
-        """
-        return self.fingerprint(fptype) | other.fingerprint(fptype)
-
-    def smarts(self):
-        """ Get the SMARTS string """
-        return Chem.MolToSmarts(self.to_rdmol())
-
-    @property
-    def smiles(self):
-        """ Get the canonical smiles """
-        return self.dump('can').split()[0]
-
-    @property
-    def spin(self):
-        return self.ob_mol.GetTotalSpinMultiplicity()
-
-    @spin.setter
-    def spin(self, spin: int):
-        self._set_spin_multiplicity(spin)
-
-    def thermo_init(self, **kwargs):
-        """
-        If certain substance don't retrieve information from current database, some required thermodynamical
-        parameters should pass into equation_of_state to initialization
-        Keyword Args:
-            T: the ambient temperature for thermodynamical system
-            P: the ambient pressure for thermodynamical system
-            V: the volume of thermodynamical system
-            Tc: the critical temperature of the molecule
-            Pc: the critical pressure of the molecule
-            omega: acentric factor of the molecule
-
-        Returns:
-            Thermo class
-        """
-        from tmo import Thermo
-        self._data['thermo'] = Thermo(self, **kwargs)
-        return self._data['thermo']
-
-    @property
-    def thermo(self):
-        return self._data.get('thermo')
-
-    def thermo_close(self):
-        _ = self._data.pop('thermo')
-        del _
-
-    def to_2d_img(self, **kwargs):
-        """
-        Get a 2D image objects for the molecule
-        Keyword Args:
-            kekulize: whether to applying Kekulize style to aromatical rings
-
-        Returns:
-
-        """
-        clone = self.copy()
-        clone.build_2d()
-        return Draw.MolToImage(clone.to_rdmol(), **kwargs)
-
-    def to_dpmd_sys(
-            self, system_dir: Union[str, os.PathLike],
-            mode: Literal['std', 'att'] = 'std',
-            validate_ratio: float = None,
-            validate_dir: Union[str, Path] = None
-    ):
-        """
-        convert to DeePMD-Kit System, there are two system mode, that `standard` (std) and `attention` (att)
-            1) standard: https://docs.deepmodeling.com/projects/deepmd/en/master/data/system.html
-            2) attention: https://docs.deepmodeling.com/projects/deepmd/en/master/model/train-se-atten.html#data-format
-
-        Args:
-            system_dir: the dir for all system data store, if the validate_dir has been given, this is the dir of
-             training system
-            mode: the system mode, choose from att or std
-            validate_ratio(float): the ratio of validate data set.
-            validate_dir(str|Path): if validate_ratio has been specified, this must be given
-        """
-        system: DeepSystem = self.dump('dpmd_sys')
-        system(system_dir, mode, validate_ratio, validate_dir)
-
-    def to_mix_mol(self):
-        """ Convert this Molecule object to MixSaveAtomMol """
-        return MixSameAtomMol(_data=self._data)
-
-    def to_rdmol(self):
-        """ convert hotpot Molecule object to RdKit mol object """
-        return Chem.MolFromMol2Block(self.dump('mol2'))
-
-    @property
-    def unique_all_atoms(self) -> List[Union['Atom', 'PseudoAtom']]:
-        return self.unique_atoms + self.unique_pseudo_atoms
-
-    @property
-    def unique_atoms(self):
-        uni = []
-        for a in self.atoms:
-            if a not in uni:
-                uni.append(a)
-        return uni
-
-    @property
-    def unique_bonds(self):
-        uni = []
-        for b in self.bonds:
-            if b not in uni:
-                uni.append(b)
-        return uni
-
-    @property
-    def unique_bond_pairs(self) -> List[Tuple[int, int, int]]:
-        """ Retrieve unique bond pair in the molecule, i.e. a bond with same atoms element combination and bond type """
-        return [b.pair_key for b in self.unique_bonds]
-
-    @property
-    def unique_pseudo_atoms(self) -> List['PseudoAtom']:
-        uni = []
-        for pa in self.pseudo_atoms:
-            if pa not in uni:
-                uni.append(pa)
-        return uni
-
-    @property
-    def weight(self):
-        return self.ob_mol.GetExactMass()
-
-    def writefile(self, fmt: str, path_file, retrieve_script=False, *args, **kwargs):
-        """Write the Molecule Info into a file with specific format(fmt)"""
-        script = self.dump(fmt=fmt, *args, **kwargs)
-        if isinstance(script, str):
-            mode = 'w'
-        elif isinstance(script, bytes):
-            mode = 'wb'
-        else:
-            raise IOError(f'the {type(script)} type for script is not supported to write into file')
-
-        with open(path_file, mode) as writer:
-            writer.write(script)
-
-        if retrieve_script:
-            return script
-
-    @property
-    def xyz_min(self) -> np.ndarray:
-        """ Return the minimum of x coordinates wreathing all atoms """
-        return self.coordinates.min(axis=0)
-
-    @property
-    def xyz_max(self) -> np.ndarray:
-        return self.coordinates.max(axis=0)
-
-    @property
-    def xyz_diff(self):
-        return self.xyz_max - self.xyz_min
-
-
-class MixSameAtomMol(Molecule):
-    """ the only difference to the Molecule class is the method of their addition  """
-
-    def __repr__(self):
-        return f'MixMol({self.formula})'
-
-    def _merge_conformer_attr(self, other: 'Molecule'):
-        """"""
-        # merge the MixSameAtomMol-specific conformer attributes
-        left_atomic_numbers: Dict[Tuple[int], int] = self.atomic_numbers
-        right_atomic_numbers: Union[Dict[Tuple[int], int], Tuple[int]] = other.atomic_numbers
-
-        # If the right atomic_number is a tuple convert it to dict.
-        if isinstance(right_atomic_numbers, tuple):
-            right_atomic_numbers = {right_atomic_numbers: other.conformer_counts}
-
-        for atomic_numbers, conformer_counts in right_atomic_numbers.items():
-            left_atomic_numbers[atomic_numbers] = left_atomic_numbers.get(atomic_numbers, 0) + conformer_counts
-
-        self._set_atomic_numbers(left_atomic_numbers)
-
-        # ##### the super method ######
-        # Merge the basic conformer attributes
-        super(MixSameAtomMol, self)._merge_conformer_attr(other)
-
-        return self
-
-    def _set_atomic_numbers(self, atomic_numbers: Dict[Tuple[int], int]):
-        """ Set all atoms' atomic numbers and their corresponding number of conformers """
-        self.update_attr_data({'atomic_numbers': atomic_numbers})
-
-    @property
-    def atomic_numbers(self) -> Dict[Tuple[int], int]:
-        """ get each conformer atomic numbers """
-        atomic_numbers = self.data.get('atomic_numbers')
-        if not atomic_numbers:
-            atomic_numbers = {super(MixSameAtomMol, self).atomic_numbers: self.conformer_counts}
-            self._set_atomic_numbers(atomic_numbers)
-
-        return atomic_numbers
-
-    @property
-    def atomic_number_counts(self):
-        """ the counts of series of atomic_numbers """
-        return len(self.atomic_numbers)
-
-    @property
-    def atomic_numbers_array(self) -> np.ndarray:
-        """ the conformer corresponding attributes with array shape (counts_of_atoms, counts_of_conformers) """
-        atomic_numbers_array = []
-        for atomic_numbers, conformer_counts in self.atomic_numbers.items():
-            atomic_numbers_array.append(np.array(atomic_numbers).reshape(1, -1).repeat(conformer_counts, axis=0))
-
-        return np.concatenate(atomic_numbers_array)
-
-    def iadd_accessible(self, other):
-        if self.atom_counts == other.atom_counts:
-            return True
-        return False
-
-    def to_mol(self):
-        """ Convert this MixSameAtomMol object to Molecule """
-        if self.atomic_number_counts > 1:
-            raise AttributeError(
-                'Cannot convert the MixSameAtomMol with multipy atomic_number series to Molecule object\n'
-                f'atomic_number_counts = {self.atomic_number_counts}'
-            )
-
-        return Molecule(_data=self.data)
-
-
-class Atom(Wrapper, ABC):
-    """ The Atom wrapper for OBAtom class in openbabel """
-
-    def __init__(
-            self,
-            ob_atom: ob.OBAtom = None,
-            **kwargs
-    ):
-        # Contain all data to reappear this Atom
-        self._data: Dict[str, Any] = {
-            'ob_obj': ob_atom if ob_atom else ob.OBAtom(),
-        }
-
-        self._set_attrs(**kwargs)
-
-    def __eq__(self, other):
-        if isinstance(other, Atom):
-            return self.ob_atom == other.ob_atom
-
-    def __hash__(self):
-        return hash(f'Atom({self.atomic_number})')
-
-    @property
-    def ob_atom(self):
-        return self._data['ob_obj']
-
-    @ob_atom.setter
-    def ob_atom(self, oba):
-        self._data['ob_obj'] = oba
-
-    def ob_atom_pop(self):
-        return self._data.pop('ob_obj')
-
-    def ob_atom_rewrap(self, ob_atom):
-        self._data['ob_obj'] = ob_atom
-
-    def __repr__(self):
-        return f"Atom({self.label if self.label else self.symbol})"
-
-    def _assign_formal_charge(self):
-        """ assign formal charge for this atom, the formal charge equal its valence minus its covalent valence """
-        if self.is_polar_hydrogen:
-            self.formal_charge = 1
-        elif self.is_hydrogen or self.is_carbon:
-            self.formal_charge = 0
-        elif self.is_metal:
-            self.formal_charge = _stable_charges[self.symbol]
-        else:
-            self.formal_charge = -len([a for a in self.neighbours if a.is_polar_hydrogen])
-
-    @property
-    def _attr_setters(self) -> Dict[str, Callable]:
-        return {
-            '_mol': self._set_molecule,
-            'mol': self._set_molecule,
-            'molecule': self._set_molecule,
-            'atomic_number': self._set_atomic_number,
-            'symbol': self._set_atomic_symbol,
-            'coordinates': self._set_coordinate,
-            'formal_charge': self._set_formal_charge,
-            'partial_charge': self._set_partial_charge,
-            'label': self._set_label,
-            'ob_id': self._set_ob_id,
-            'spin_density': self._set_spin_density
-        }
-
-    def _set_atomic_number(self, atomic_number: int):
-        self.ob_atom.SetAtomicNum(int(atomic_number))
-
-    def _set_atomic_symbol(self, symbol):
-        self.ob_atom.SetAtomicNum(ob.GetAtomicNum(symbol))
-
-    def _set_coordinate(self, coordinates):
-        self.ob_atom.SetVector(*coordinates)
-
-    def _set_force_vector(self, force_vector: Union[Sequence, np.ndarray]):
-        if isinstance(force_vector, Sequence):
-            if all(isinstance(f, float) for f in force_vector):
-                force_vector = np.array(force_vector)
-            else:
-                ValueError('the give force_vector must float vector with dimension 3')
-        elif isinstance(force_vector, np.ndarray):
-            force_vector = force_vector.flatten()
-        else:
-            raise TypeError('the force vector should be Sequence or np.ndarray')
-
-        self._data['force_vector'] = force_vector
-
-    def _set_formal_charge(self, charge: float):
-        self.ob_atom.SetFormalCharge(charge)
-
-    def _set_ob_id(self, ob_id):
-        self.ob_atom.SetId(ob_id)
-
-    def _set_label(self, label):
-        label_data = ob.OBCommentData()
-
-        label_data.SetAttribute('label')
-        label_data.SetData(label)
-
-        self.ob_atom.CloneData(label_data)
-
-    def _set_molecule(self, molecule: Molecule):
-        self._data['mol'] = molecule
-
-    def _set_partial_charge(self, charge):
-        self.ob_atom.SetPartialCharge(charge)
-
-    def _set_spin_density(self, spin_density: float):
-        self._data['spin_density'] = spin_density
-
-    @property
-    def atom_type(self):
-        """ Some atom have specific type, such as Carbon with sp1, sp2 and sp3, marked as C1, C2 and C3 """
-        return self.ob_atom.GetType()
-
-    def add_atom(self, symbol: str, bond_type=1, **atom_attrs):
-        """ add atom to link with this atom """
-        new_atom = self.molecule.add_atom(symbol, **atom_attrs)
-        self.molecule.add_bond(self, new_atom, bond_type)
-
-    def add_hydrogen(self):
-        """ add hydrogen to the atom """
-        self.add_atom('H')
-
-    @property
-    def atomic_number(self):
-        return self.ob_atom.GetAtomicNum()
-
-    def balance_hydrogen(self):
-        """ Remove or add hydrogens link with this atom, if the bond valence is not equal to the atomic valence """
-        if self.is_heavy and not self.is_metal:  # Do not add or remove hydrogens to the metal, H or inert elements
-            while self.valence > self.stable_valence and self.neighbours_hydrogen:
-                self.molecule.remove_atoms(self.neighbours_hydrogen[0])
-
-            # add hydrogen, if the bond valence less than the atomic valence
-            while self.valence < self.stable_valence:
-                self.add_hydrogen()
-
-    @property
-    def bonds(self):
-        """ Get all bonds link with the atoms """
-        return [self.molecule.bonds_dict[obb.GetId()] for obb in ob.OBAtomBondIter(self.ob_atom)]
-
-    @property
-    def coordinates(self) -> (float, float, float):
-        return self.ob_atom.GetX(), self.ob_atom.GetY(), self.ob_atom.GetZ()
-
-    @coordinates.setter
-    def coordinates(self, value):
-        self._set_coordinate(value)
-
-    @property
-    def coordinates_array(self) -> np.ndarray:
-        """ the array of coordinates """
-        return np.array(self.coordinates)
-
-    def copy(self):
-        """ Make a copy of self """
-        # Extract old data
-        data = self.data
-        data.pop('ob_obj')  # Remove the old OBAtom
-        # Remove molecule if the parent atom in a molecule
-        if self.molecule:
-            data.pop('mol')
-
-        # Copy the information contained in OBAtom
-        new_attrs = {
-            "atomic_number": self.atomic_number,
-            "coordinates": self.coordinates,
-            'partial_charge': self.partial_charge,
-        }
-
-        new_attrs.update(**data)
-
-        return Atom(**new_attrs)
-
-    @property
-    def covalent_valence(self):
-        """ the number of covalent electrons for this atoms """
-        return sum(b.type if b.is_covalent else 0 for b in self.bonds)
-
-    def element_features(self, *feature_names) -> np.ndarray:
-        """ Retrieve the feature vector """
-        atom_feature = periodic_table[self.symbol]
-
-        features = []
-        for feature_name in feature_names:
-            if feature_name == 'atomic_orbital':
-                features.extend(self._atomic_orbital_feature().values())
-            elif feature_name == 'atomic_number':
-                features.append(self.atomic_number)
-            else:
-                features.append(atom_feature[feature_name])
-
-        return np.array(features)
-
-    def _atomic_orbital_feature(self, outermost_layer=True, nonexistent_orbit=0):
-        """    Calculating the feature about atomic orbital structures    """
-        _atomic_orbital_structure_max = {
-            "1s": 2,
-            "2s": 2, "2p": 6,
-            "3s": 2, "3p": 6,
-            "4s": 2, "3d": 10, "4p": 6,
-            "5s": 2, "4d": 10, "5p": 6,
-            "6s": 2, "4f": 14, "5d": 10, "6p": 6,
-            "7s": 2, "5f": 14, "6d": 10, "7p": 6
-        }
-        atomic_orbital_structure = {
-            "1s": 0,
-            "2s": 0, "2p": 0,
-            "3s": 0, "3p": 0,
-            "4s": 0, "3d": 0, "4p": 0,
-            "5s": 0, "4d": 0, "5p": 0,
-            "6s": 0, "4f": 0, "5d": 0, "6p": 0,
-            "7s": 0, "5f": 0, "6d": 0, "7p": 0
-        }
-
-        # Calculating atomic orbital structure
-        residual_electron = self.atomic_number
-        n_osl = 0  # Principal quantum number (n) of open shell layers (osl)
-        for orbital_name, men in _atomic_orbital_structure_max.items():  # max electron number (men)
-
-            # Update Principal quantum number (n)
-            if orbital_name[1] == "s":
-                n_osl = int(orbital_name[0])
-
-            # Filled atomic orbital
-            if residual_electron - men >= 0:
-                residual_electron = residual_electron - men
-                atomic_orbital_structure[orbital_name] = men
-            else:
-                atomic_orbital_structure[orbital_name] = residual_electron
-                break
-
-        # Readout and return outermost electron structure
-        atom_orbital_feature = {"atomic_number": self.atomic_number, "n_osl": n_osl}
-        if outermost_layer:
-            diff_max_n = {"s": 0, "p": 0, "d": -1, "f": -2}
-            for layer, diff in diff_max_n.items():  # Angular momentum quantum number (l)
-                electron_number = atomic_orbital_structure.get(f"{n_osl + diff}{layer}", nonexistent_orbit)
-                atom_orbital_feature[layer] = electron_number
-        else:
-            atom_orbital_feature.update(atomic_orbital_structure)
-
-        # return whole electron structure directly
-        return atom_orbital_feature
-
-    @property
-    def force_vector(self):
-        return self._data.get('force_vector', np.zeros(3, dtype=float))
-
-    @force_vector.setter
-    def force_vector(self, force_vector: Union[Sequence, np.ndarray]):
-        self._set_force_vector(force_vector)
-
-    @property
-    def formal_charge(self) -> float:
-        return self.ob_atom.GetFormalCharge()
-
-    @formal_charge.setter
-    def formal_charge(self, value: float):
-        self.ob_atom.SetFormalCharge(value)
-
-    @property
-    def has_unknown_bond(self) -> bool:
-        return any(not b.type for b in self.bonds)
-
-    @property
-    def hybridization(self):
-        """ The hybridization of this atom:
-        1 for sp, 2 for sp2, 3 for sp3, 4 for sq. planar, 5 for trig. bipy, 6 for octahedral """
-        return self.ob_atom.GetHyb()
-
-    @property
-    def kwargs_attributes(self):
-        return tuple(self._attr_setters.keys())
-
-    @property
-    def ob_id(self):
-        return self.ob_atom.GetId()
-
-    @property
-    def ob_idx(self):
-        return self.ob_atom.GetIdx()
-
-    @property
-    def is_aromatic(self):
-        return self.ob_atom.IsAromatic()
-
-    @property
-    def is_carbon(self):
-        return self.atomic_number == 6
-
-    @property
-    def is_chiral(self):
-        return self.ob_atom.IsChiral()
-
-    @property
-    def is_hydrogen(self):
-        return self.ob_atom.GetAtomicNum() == 1
-
-    @property
-    def is_heavy(self):
-        """ Whether the atom is heavy atom """
-        return not self.is_hydrogen
-
-    @property
-    def is_polar_hydrogen(self) -> bool:
-        """ Is this atom a hydrogen connected to a polar atom """
-        return self.ob_atom.IsPolarHydrogen()
-
-    @property
-    def is_metal(self):
-        return self.ob_atom.IsMetal()
-
-    @property
-    def label(self):
-        label_data = self.ob_atom.GetData('label')
-
-        if label_data:
-            label_data = ob.toCommentData(label_data)
-            return label_data.GetValue()
-        else:
-            return self.symbol
-
-    @label.setter
-    def label(self, value):
-        self._set_label(value)
-
-    @property
-    def link_degree(self) -> int:
-        """ the degree of the atom in their parent molecule """
-        return self.ob_atom.GetTotalDegree()
-
-    @property
-    def mass(self):
-        return self.ob_atom.GetAtomicMass()
-
-    @property
-    def max_bonds(self):
-        """ the max allowed bond order"""
-        return ob.GetMaxBonds(self.atomic_number)
-
-    @property
-    def molecule(self) -> Molecule:
-        return self._data.get('mol')
-
-    @molecule.setter
-    def molecule(self, mol: 'Molecule'):
-        self._data['mol'] = mol
-
-    @property
-    def neighbours_hydrogen(self) -> List['Atom']:
-        """ return all neigh hydrogen atoms """
-        return [a for a in self.neighbours if a.is_hydrogen]
-
-    @property
-    def electronegativity(self):
-        return ob.GetElectroNeg(self.atomic_number)
-
-    @property
-    def neighbours(self) -> List['Atom']:
-        """ Get all atoms bond with this atom in same molecule """
-        if self.molecule:
-            _ = self.molecule.atoms  # update the atoms dict
-            return [self.molecule.atoms_dict[ob_atom.GetId()] for ob_atom in ob.OBAtomAtomIter(self.ob_atom)]
-        else:
-            return []
-
-    @property
-    def neighbours_label(self) -> List[str]:
-        """ return all neighbours labels """
-        return [a.label for a in self.neighbours]
-
-    @property
-    def neighbours_position(self) -> Generator[Tuple[Union['Atom', np.ndarray]], None, None]:
-        """ Retrieve the relative position of neigh atoms, assign this atom as the origin """
-        for neigh_atom in self.neighbours:
-            yield neigh_atom, neigh_atom.coordinates_array - self.coordinates_array
-
-    @property
-    def partial_charge(self):
-        return self.ob_atom.GetPartialCharge()
-
-    @partial_charge.setter
-    def partial_charge(self, value: float):
-        # This is necessary to take effect to the assignment.
-        # the reason is unknown
-        self.ob_atom.GetPartialCharge()
-        self._set_partial_charge(value)
-
-    def remove_hydrogen(self):
-        """ remove the first atom linking with the atoms """
-        hydrogens = self.neighbours_hydrogen
-        if hydrogens:
-            self.molecule.remove_atoms(hydrogens[0])
-
-    def remove_hydrogens(self):
-        """ Remove all hydrogens linking with the atom"""
-        hydrogens = self.neighbours_hydrogen
-        self.molecule.remove_atoms(*hydrogens)
-
-    def replace_attr_data(self, data: Dict):
-        """ Replace the core data dict directly """
-        self._data = data
-
-    def set(self, **kwargs):
-        """
-        Set atom attributes by kwargs
-        Kwargs:
-            atomic_number(int): set atomic number
-            symbol(str): set atomic symbol
-            coordinates(Sequence, numpy.ndarray): coordinates of the atom
-            partial_charge:
-            label:
-            spin_density:
-        """
-        self._set_attrs(**kwargs)  # set attributes
-
-    @property
-    def spin_density(self):
-        return self._data.get('spin_density', 0.0)
-
-    @spin_density.setter
-    def spin_density(self, spin_density: float):
-        self._set_spin_density(spin_density)
-
-    @property
-    def stable_valence(self) -> int:
-        if self.is_metal:
-            return 0
-        elif self.symbol == 'S':
-            if not [a for a in self.neighbours if a.symbol == 'O']:
-                return 2
-            elif self.covalent_valence <= 2:
-                return 2
-            elif self.covalent_valence <= 4:
-                return 4
-            else:
-                return 6
-        elif self.symbol == 'S':
-            if not [a for a in self.neighbours if a.symbol == 'O']:
-                return 3
-            elif self.covalent_valence == 0:
-                return 0
-            elif self.covalent_valence == 1:
-                return 1
-            elif self.covalent_valence <= 3:
-                return 3
-            else:
-                return 5
-        else:
-            return abs(_stable_charges[self.symbol])
-
-    @property
-    def symbol(self) -> str:
-        return ob.GetSymbol(self.atomic_number)
-
-    @property
-    def valence(self) -> int:
-        # if self.has_unknown_bond:
-        #     raise AttributeError('Cannot calculate the bond valence, because of the existence of unknown bonds')
-        return sum(b.type if b.type else 0 if b.is_covalent else 1 for b in self.bonds)
-
-
-class PseudoAtom(Wrapper, ABC):
-    """ A data wrapper for pseudo atom """
-
-    def __init__(self, symbol: str, mass: float, coordinates: Union[Sequence, np.ndarray], **kwargs):
-        if isinstance(coordinates, Sequence):
-            coordinates = np.array(coordinates)
-
-        assert isinstance(coordinates, np.ndarray) and coordinates.shape == (3,)
-
-        self._data = dict(symbol=symbol, mass=mass, coordinates=coordinates, **kwargs)
-
-    def __eq__(self, other):
-        if isinstance(other, PseudoAtom):
-            return self.symbol == other.symbol
-        return False
-
-    def __hash__(self):
-        return hash(f'PseudoAtom({self.symbol})')
-
-    def _attr_setters(self) -> Dict[str, Callable]:
-        return {}
-
-    def __repr__(self):
-        return f'PseudoAtom({self.symbol})'
-
-    def __dir__(self) -> Iterable[str]:
-        return list(self._data.keys())
-
-    def __getattr__(self, item):
-        return self._data.get(item, 0.)
-
-
-class Bond(Wrapper, ABC):
-    """"""
-
-    def __init__(self, ob_bond: ob.OBBond, _mol: Molecule):
-        self._data = {
-            'ob_obj': ob_bond,
-            'mol': _mol
-        }
-
-    def __repr__(self):
-        return f"Bond({self.atoms[0].label}, {self.atoms[1].label}, {self.type_name})"
-
-    def __eq__(self, other: 'Bond'):
-        if isinstance(other, Bond):
-            return self.pair_key == other.pair_key
-
-    def __hash__(self):
-        return hash(self.pair_key)
-
-    @property
-    def ob_bond(self):
-        return self._data['ob_obj']
-
-    def ob_bond_pop(self):
-        return self._data.pop('ob_obj')
-
-    def ob_bond_rewrap(self, ob_bond):
-        self._data['ob_obj'] = ob_bond
-
-    @property
-    def _attr_setters(self) -> Dict[str, Callable]:
-        return {
-        }
-
-    @property
-    def atom1(self) -> Atom:
-        return self.molecule.atoms_dict[self.ob_atom1_id]
-
-    @property
-    def atom2(self) -> Atom:
-        return self.molecule.atoms_dict[self.ob_atom2_id]
-
-    @property
-    def atomic_number1(self):
-        return self.ob_bond.GetBeginAtom().GetAtomicNum()
-
-    @property
-    def atomic_number2(self):
-        return self.ob_bond.GetEndAtom().GetAtomicNum()
-
-    @property
-    def atoms(self):
-        return self.atom1, self.atom2
-
-    @property
-    def begin_end_ob_id(self) -> (int, int):
-        return self.ob_bond.GetBeginAtom().GetId(), self.ob_bond.GetEndAtom().GetId()
-
-    @property
-    def begin_end_atomic_number(self):
-        return self.ob_bond.GetBeginAtom().GetAtomicNum(), self.ob_bond.GetEndAtom().GetAtomicNum()
-
-    @property
-    def is_covalent(self) -> bool:
-        return not self.ob_atom1.IsMetal() and not self.ob_atom2.IsMetal()
-
-    @property
-    def ideal_length(self):
-        return self.ob_bond.GetEquibLength()
-
-    @property
-    def ob_id(self):
-        return self.ob_bond.GetId()
-
-    @property
-    def ob_idx(self):
-        return self.ob_bond.GetIdx()
-
-    @property
-    def ob_atom1(self):
-        return self.ob_bond.GetBeginAtom()
-
-    @property
-    def ob_atom2(self):
-        return self.ob_bond.GetEndAtom()
-
-    @property
-    def ob_atom1_id(self):
-        return self.ob_atom1.GetId()
-
-    @property
-    def ob_atom2_id(self):
-        return self.ob_atom2.GetId()
-
-    @property
-    def pair_key(self):
-        """ Get the bond pair key, a string that show combination of element of end atoms and bond type,
-        where, the atomic symbol with lower atomic number is placed in the first, the higher in the last"""
-        if self.atomic_number1 <= self.atomic_number2:
-            return self.atomic_number1, self.type, self.atomic_number2
-        return self.atomic_number2, self.type, self.atomic_number1
-
-    @property
-    def length(self):
-        return self.ob_bond.GetLength()
-
-    @property
-    def molecule(self):
-        return self._data['mol']
-
-    @molecule.setter
-    def molecule(self, mol: Molecule):
-        self._data['mol'] = mol
-
-    @property
-    def type_name(self):
-        return _type_bond[self.type]
-
-    @property
-    def type(self):
-        return self.ob_bond.GetBondOrder()
-
-
-class Angle:
-    """ Data wrapper of angle in molecule """
-
-    def __init__(self, mol: 'Molecule', atoms_ob_id: tuple):
-        self._data = {
-            'mol': mol,
-            'atoms_ob_id': atoms_ob_id
-        }
-
-    def __repr__(self):
-        a, b, c = self.atoms
-        return f'Angle({a.label}, {b.label}, {c.label}, {round(self.degree, 2)}°)'
-
-    @property
-    def molecule(self):
-        return self._data.get('mol')
-
-    @molecule.setter
-    def molecule(self, mol: Molecule):
-        self._data['mol'] = mol
-
-    @property
-    def atoms(self):
-        mas = self.molecule.atoms  # atom in the molecule
-        return [mas[i] for i in self.atoms_ob_id]
-
-    @property
-    def atoms_ob_id(self):
-        return self._data.get('atoms_ob_id')
-
-    @property
-    def degree(self):
-        ob_atoms = [a.ob_atom for a in self.atoms]
-        return self.molecule.ob_mol.GetAngle(*ob_atoms)
-
-
-class Torsion:
-    """"""
-
-
-class Crystal(Wrapper, ABC):
-    """"""
-    _lattice_type = (
-        'Undefined', 'Triclinic', 'Monoclinic', 'Orthorhombic', 'Tetragonal', 'Rhombohedral', 'Hexagonal', 'Cubic'
-    )
-
-    def __init__(self, ob_unitcell: ob.OBUnitCell = None, **kwargs):
-
-        self._data: Dict[str, Any] = {
-            'OBUnitCell': ob_unitcell if ob_unitcell else ob.OBUnitCell(),
-        }
-
-        self._set_attrs(**kwargs)
-
-    def __repr__(self):
-        return f'Crystal({self.lattice_type}, {self.space_group}, {self.molecule})'
-
-    @property
-    def ob_unit_cell(self) -> ob.OBUnitCell:
-        return self._data.get('OBUnitCell')
-
-    @staticmethod
-    def _matrix_to_params(matrix: np.ndarray):
-        """ Covert the cell matrix to cell parameters: a, b, c, alpha, beta, gamma """
-        va, vb, vc = matrix
-        a = sum(va ** 2) ** 0.5
-        b = sum(vb ** 2) ** 0.5
-        c = sum(vc ** 2) ** 0.5
-
-        alpha = np.arccos(np.dot(va, vb) / (a * b)) / np.pi * 180
-        beta = np.arccos(np.dot(va, vc) / (a * c)) / np.pi * 180
-        gamma = np.arccos(np.dot(vb, vc) / (b * c)) / np.pi * 180
-
-        return a, b, c, alpha, beta, gamma
-
-    def _set_molecule(self, molecule: Molecule):
-        if molecule.crystal and isinstance(molecule.crystal, Crystal):
-            print(AttributeError("the Molecule have been stored in a Crystal, "
-                                 "can't save the same Molecule into two Crystals"))
-        else:
-            self._data['mol'] = molecule
-
-    def _set_space_group(self, space_group: str):
-        self.ob_unit_cell.SetSpaceGroup(space_group)
-
-    @property
-    def _attr_setters(self) -> Dict[str, Callable]:
-        return {
-            'mol': self._set_molecule,
-            'molecule': self._set_molecule,
-            'space_group': self._set_space_group
-        }
-
-    @property
-    def lattice_type(self) -> str:
-        return self._lattice_type[self.ob_unit_cell.GetLatticeType()]
-
-    @property
-    def lattice_params(self) -> np.ndarray[2, 3]:
-        a = self.ob_unit_cell.GetA()
-        b = self.ob_unit_cell.GetB()
-        c = self.ob_unit_cell.GetC()
-        alpha = self.ob_unit_cell.GetAlpha()
-        beta = self.ob_unit_cell.GetBeta()
-        gamma = self.ob_unit_cell.GetGamma()
-        return np.array([[a, b, c], [alpha, beta, gamma]])
-
-    @property
-    def molecule(self) -> Molecule:
-        return self._data.get('mol')
-
-    @molecule.setter
-    def molecule(self, mol: Molecule):
-        self._data['mol'] = mol
-
-    @property
-    def pack_molecule(self) -> Molecule:
-        mol = self.molecule  # Get the contained Molecule
-
-        if not mol:  # If get None
-            print(RuntimeWarning("the crystal doesn't contain any Molecule!"))
-
-        pack_mol = mol.copy()
-        self.ob_unit_cell.FillUnitCell(pack_mol.ob_mol)  # Full the crystal
-        pack_mol._reorganize_atom_indices()  # Rearrange the atom indices.
-
-        return pack_mol
-
-    def set_lattice(
-            self,
-            a: float, b: float, c: float,
-            alpha: float, beta: float, gamma: float
-    ):
-        self.ob_unit_cell.SetData(a, b, c, alpha, beta, gamma)
-
-    def set_vectors(
-            self,
-            va: Union[np.ndarray, Sequence],
-            vb: Union[np.ndarray, Sequence],
-            vc: Union[np.ndarray, Sequence]
-    ):
-        """"""
-        vectors = [va, vb, vc]
-        matrix = np.array(vectors)
-        self.set_matrix(matrix)
-
-    def set_matrix(self, matrix: np.ndarray):
-        """ Set cell matrix for the crystal """
-        if matrix.shape != (3, 3):
-            raise AttributeError('the shape of cell_vectors should be [3, 3]')
-
-        cell_params = map(float, self._matrix_to_params(matrix))
-
-        self.ob_unit_cell.SetData(*cell_params)
-
-    @property
-    def space_group(self):
-        space_group = self.ob_unit_cell.GetSpaceGroup()
-        if space_group:
-            return space_group.GetHMName()
-        else:
-            return None
-
-    @space_group.setter
-    def space_group(self, value: str):
-        self._set_space_group(value)
-
-    @property
-    def volume(self):
-        return self.ob_unit_cell.GetCellVolume()
-
-    @property
-    def vector(self):
-        v1, v2, v3 = self.ob_unit_cell.GetCellVectors()
-        return np.array([
-            [v1.GetX(), v1.GetY(), v1.GetZ()],
-            [v2.GetX(), v2.GetY(), v2.GetZ()],
-            [v3.GetX(), v3.GetY(), v3.GetZ()]
-        ])
-
-    def zeo_plus_plus(self):
-        """ TODO: complete the method after define the Crystal and ZeoPlusPlus tank """
-
-
-import hotpot.bundle as bd
-from hotpot._io import Dumper, Parser
-from hotpot.tanks.cc import PairBundle
-from hotpot.tanks.deepmd import DeepSystem
+"""
+python v3.9.0
+@Project: hotpot
+@File   : cheminfo.py
+@Author : Zhiyuan Zhang
+@Date   : 2023/3/14
+@Time   : 4:09
+"""
+import copy
+import json
+import os
+import re
+from abc import ABC, abstractmethod
+from io import IOBase
+from os import PathLike
+from os.path import join as opj
+from pathlib import Path
+from typing import *
+from itertools import product
+
+import numpy as np
+from openbabel import openbabel as ob, pybel as pb
+from rdkit import Chem
+from rdkit.Chem import Draw
+
+from hotpot import data_root
+from hotpot.tanks import lmp
+from hotpot.tanks.quantum import Gaussian, GaussianRunError, GaussRun, GaussErrorHandle
+from hotpot.utils.library import library as _lib  # The chemical library
+
+
+# Define Exceptions
+class OperateOBMolFail(BaseException):
+    """ Raise for any fail that trys to operate the OBMol """
+
+
+class AddAtomFail(OperateOBMolFail):
+    """ Raise when add an atom into Molecule fail """
+
+
+class AddBondFail(OperateOBMolFail):
+    """ Raise when add a bond into Molecule fail """
+
+
+# periodic_table = json.load(open(opj(data_root, 'periodic_table.json'), encoding='utf-8'))
+periodic_table = _lib.get('PeriodicTable')  # hotpot.utils.library.PeriodicTabel
+
+_stable_charges = {
+    "H": 1,  "He": 0,
+    "Li": 1, "Be": 2, "B": 3,  "C": 4,  "N": -3,  "O": -2,  "F": -1,  "Ne": 0,
+    "Na": 1, "Mg": 2, "Al": 3, "Si": 4, "P": -3,  "S": -2,  "Cl": -1, "Ar": 0,
+    "K": 1,  "Ca": 2, "Ga": 3, "Ge": 4, "As": -3, "Se": -2, "Br": -1, "Kr": 0,
+    "Rb": 1, "Sr": 2, "In": 3, "Sn": 2, "Sb": -3, "Te": -2, "I": -1,  "Xe": 0,
+    "Cs": 1, "Ba": 2, "Tl": 3, "Pb": 2, "Bi": 3,  "Po": -2, "At": -1, "Rn": 0,
+    "Fr": 1, "Ra": 2, "Nh": 8, "Fl": 8, "Mc": 8,  "Lv": 8,  "Ts": 8,  "Og": 8,
+
+    "Sc": 3, "Ti": 4, "V": 5,  "Cr": 3, "Mn": 2,  "Fe": 3,  "Co": 3,  "Ni": 2, "Cu": 2, "Zn": 2,
+    "Y": 3,  "Zr": 4, "Nb": 5, "Mo": 6, "Tc": 7,  "Ru": 4,  "Rh": 3,  "Pd": 2, "Ag": 1, "Cd": 2,
+    "Lu": 3, "Hf": 4, "Ta": 5, "W": 6,  "Re": 7,  "Os": 4,  "Ir": 3,  "Pt": 2, "Au": 1, "Hg": 2,
+    "Lr": 3, "Rf": 4, "Db": 5, "Sg": 6, "Bh": 7,  "Hs": 8,  "Mt": 8,  "Ds": 8, "Rg": 8, "Cn": 8,
+
+    "La": 3, "Ce": 4, "Pr": 3, "Nd": 3, "Pm": 3,  "Sm": 3,  "Eu": 2,  "Gd": 3, "Tb": 3, "Dy": 3, "Ho": 3, "Er": 3, "Tm": 3, "Yb": 3,
+    "Ac": 3, "Th": 4, "Pa": 5, "U": 6,  "Np": 6,  "Pu": 6,  "Am": 6,  "Cm": 6, "Bk": 6, "Cf": 6, "Es": 6, "Fm": 6, "Md": 6, "No": 6,
+}
+
+
+_bond_type = {
+    'Unknown': 0,
+    'Single': 1,
+    'Double': 2,
+    'Triple': 3,
+    'Aromatic': 5,
+}
+
+_type_bond = {
+    0: 'Unknown',
+    1: 'Single',
+    2: 'Double',
+    3: 'Triple',
+    5: 'Aromatic'
+}
+
+_ob_data_dict = {
+    0: 'UndefinedData', 1: 'PairData', 2: 'EnergyData', 3: 'CommentData',
+    4: 'ConformerData', 5: 'ExternalBondData', 6: 'RotamerList', 7: 'VirtualBondData',
+    8: 'RingData', 9: 'TorsionData', 10: 'AngleData', 11: 'SerialNums',
+    12: 'UnitCell', 13: 'SpinData', 14: 'ChargeData', 15: 'SymmetryData',
+    16: 'ChiralData', 17: 'OccupationData', 18: 'DensityData', 19: 'ElectronicData',
+    20: 'VibrationData', 21: 'RotationData', 22: 'NuclearData', 23: 'SetData',
+    24: 'GridData', 25: 'VectorData', 26: 'MatrixData', 27: 'StereoData',
+    28: 'DOSData', 29: 'ElectronicTransitionData', 16384: 'CustomData0', 16385: 'CustomData1',
+    16386: 'CustomData2', 16387: 'CustomData3', 16388: 'CustomData4', 16389: 'CustomData5',
+    16390: 'CustomData6', 16391: 'CustomData7', 16392: 'CustomData8', 16393: 'CustomData9',
+    16394: 'CustomData10', 16395: 'CustomData11', 16396: 'CustomData12', 16397: 'CustomData13',
+    19398: 'CustomData14', 16399: 'CustomData15'
+}
+
+
+class Wrapper(ABC):
+    """
+    A wrapper of chemical information and data.
+    The _set_attrs method is used to set any keyword attribute, the attribute names, in the wrapper context, are defined
+    by the keys from returned dict of _attr_setters; the values of the returned dict of _attr_setters are a collection
+    of specific private method to wrapper and call openbabel method to set the attributes in openbabel object.
+    """
+    _data = {}  # all attributes of wrappers are stored into
+
+    @property
+    def _ob_obj(self) -> Union[ob.OBMol, ob.OBAtom, ob.OBBond, ob.OBAngle, ob.OBUnitCell]:
+        return self._data.get('ob_obj')
+
+    @property
+    def _protected_data(self):
+        """
+        the protected attr in data which could not be replaced by call methods:
+            - update_attr_data()
+        """
+        return ('ob_obj',)
+
+    def _set_attrs(self, **kwargs):
+        """    Set any atomic attributes by name    """
+        attr_setters = self._attr_setters
+        for name, value in kwargs.items():
+            setter = attr_setters.get(name)
+
+            if setter:  # if the attribute is exist in the object.
+                assert isinstance(setter, Callable)
+                setter(value)
+
+            else:
+                raise NameError(
+                    f'the {name} is cannot be set by {self.__class__.__name__}.set(), '
+                    f'the legal attrs include: {self._attr_setters.keys()}'
+                )
+
+    @property
+    @abstractmethod
+    def _attr_setters(self) -> Dict[str, Callable]:
+        raise NotImplemented
+
+    def _get_ob_comment_data(self, data_name: str):
+        """ Retrieve OBCommentData according to specific data_name """
+        comment = self._ob_obj.GetData(data_name)
+        if comment:
+            comment = ob.toCommentData(comment)
+            return comment.GetData()
+        return None
+
+    @property
+    def data(self) -> dict:
+        """ Get the clone of attributes data dict """
+        return copy.copy(self._data)
+
+    def kwargs_setters(self):
+        list_setters = [f'{k}: {s.__doc__}' for k, s in self._attr_setters.items()]
+        print("\n".join(list_setters))
+
+    def remove_ob_data(self, data_name: str):
+        """ Remove specific OBData item by given data_name """
+        self._ob_obj.DeleteData(data_name)
+
+    def replace_attr_data(self, data: Dict):
+        """ Replace the core data dict directly """
+        self._data = data
+
+    def set_ob_comment_data(self, attr_name: str, value: str):
+        """ Set the OBCommentData for ob_obj """
+        comment_data = ob.OBCommentData()
+
+        comment_data.SetAttribute(attr_name)
+        comment_data.SetData(value)
+
+        self._ob_obj.CloneData(comment_data)
+
+    @property
+    def setter_keys(self):
+        return list(self._attr_setters.keys())
+
+    @property
+    def temp_label(self):
+        """ Retrieve the temp label """
+        return self._get_ob_comment_data('temp_label')
+
+    def update_attr_data(self, data: dict):
+        """ update the attribute data by give dict """
+        for data_attr in self._protected_data:
+            if data.get(data_attr):
+                data.pop(data_attr)
+
+        self._data.update(data)
+
+
+class MolLinker:
+    """ This class offer methods to link to parent molecule object and retrieve associated value from the molecule """
+    class LinkerKey:
+        def __init__(self, *ob_atoms: ob.OBAtom):
+            self.ob_atoms = ob_atoms
+
+        def __repr__(self):
+            return str(self.key)
+
+        def __eq__(self, other: 'MolLinker.LinkerKey'):
+            return self.key == other.key or self.key == other.key[::-1]
+
+        def __hash__(self):
+            return hash(self.key)
+
+        @property
+        def key(self):
+            return tuple(aba.GetId() for aba in self.ob_atoms)
+
+    def __init__(self, mol: 'Molecule', *ob_ids: int):
+        """"""
+        self.mol = mol
+        self.ob_atoms = tuple(mol.atoms_dict[obi].ob_atom for obi in ob_ids)
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}({", ".join([a.label for a in self.atoms])}; {self._degree})'
+
+    def __eq__(self, other: 'Torsion'):
+        return self.linker_key == other.linker_key
+
+    def __getitem__(self, item):
+        return self.data.get(item, {})
+
+    def __setitem__(self, key, value):
+        self.update_attr_data({key: value})
+
+    @property
+    @abstractmethod
+    def _degree(self) -> float:
+        raise NotImplementedError('')
+
+    @property
+    def atoms(self) -> List['Atom']:
+        return [self.mol.atoms_dict[obi] for obi in self.atoms_ob_id]
+
+    @property
+    def atoms_ob_id(self):
+        return tuple(oba.GetId() for oba in self.ob_atoms)
+
+    @property
+    def data(self) -> Dict:
+        data: Dict[MolLinker.LinkerKey, Dict[Hashable, Any]] = self.mol.data.get(self.__class__.__name__, {})
+        return data.setdefault(self.linker_key, {})
+
+    @property
+    def linker_key(self) -> LinkerKey:
+        return self.LinkerKey(*self.ob_atoms)
+
+    def update_attr_data(self, update_data: Dict):
+        all_angle_data: Dict[MolLinker.LinkerKey, Dict[Hashable, Any]] = self.mol.data.get(self.__class__.__name__, {})
+        data: Dict[Hashable, Any] = all_angle_data.setdefault(self.linker_key, {})
+        data.update(update_data)
+
+        self.mol.update_attr_data({self.__class__.__name__: all_angle_data})
+
+
+class Molecule(Wrapper, ABC):
+    """"""
+    # All Molecule attribute's items relating to molecule conformers
+    conformer_items = (
+        # the items are ranked by the number of values for each atom, for example:
+        #   - the all_atom_charges and atom_spin_densities have 1 value for each atom, so they are placed in the second
+        #     item (with the index 1)
+        #   - the coordinates have 3 values for each atom, i.e., [x, y, z], so it is placed in the forth
+        #     item (with the index 3）
+        # For the molecular attributes, which have only one value for each conformer and represent the attribute
+        # of whole molecule, they are place in the first item (with the index 0)
+        ('all_energy', 'identifier_array'),
+        ('all_atom_charges', 'all_atom_spin_densities'),
+        (),
+        ('all_coordinates', 'all_forces')
+    )
+
+    def __init__(self, ob_mol: ob.OBMol = None, _data: dict = None, **kwargs):
+        if _data:
+            self._data: dict = _data
+        else:
+            self._data: dict = {
+                'ob_obj': ob_mol if ob_mol else ob.OBMol()
+            }
+        self._set_attrs(**kwargs)
+        self._load_atoms()
+        self._load_bonds()
+
+    def __repr__(self):
+        return f'Mol({self.ob_mol.GetSpacedFormula()})'
+
+    def __add__(self, other: ['Molecule']):
+        """
+        Two Molecule objects could add to a new one to merge all of their conformers.
+        All information about the conformer will be merged to one.
+        the other information will reserve the one in the left item
+        Args:
+            other: the right item
+
+        Returns:
+            Molecule
+        """
+        # When other obj is a Molecule or a child of Molecule
+        if isinstance(other, Molecule):
+            # If this one is compatible to the other
+            if self.iadd_accessible(other):
+                clone = self.copy()
+                clone += other
+
+                return clone
+
+            # If the other one is compatible to this one
+            if other.iadd_accessible(self):
+                clone = other.copy()
+                clone += self
+
+                return clone
+
+            # If they are compatible, but are Molecule or child of Molecule
+            return bd.MolBundle([self, other])
+
+        # if isinstance(other, MixSameAtomMol):
+        #     return self.to_mix_mol() + other
+
+        # When other obj is a MolBundle
+        if isinstance(other, bd.MolBundle):
+            return other.__class__([self] + other.mols)
+
+        else:
+            raise TypeError('the Molecule only add with Molecule or MolBundle')
+
+    def __iadd__(self, other):
+        """
+        Self add with other Molecule object with consist atoms list,
+        The attributes or information about conformers will merge with the other,
+        other attributes or information will be reserved
+        Args:
+            other: the merged Molecule object
+
+        Returns:
+            None
+        """
+        if not isinstance(other, Molecule):
+            raise TypeError('the Molecule object is only allowed to add with other Molecule')
+
+        # Check whether left and right Molecules have consist atom list
+        if not self.iadd_accessible(other):
+            raise AttributeError(
+                'the self addition cannot be performed among molecules with different atoms list!'
+            )
+
+        return self._merge_conformer_attr(other)
+
+    def __iter__(self):
+        """ Return self with different conformers """
+
+        def conformer_generator():
+            for i in range(self.conformer_counts):
+                self.conformer_select(i)
+                yield self
+
+        return iter(conformer_generator())
+
+    def __next__(self):
+        config_idx = self._data.get('config_idx', 0)
+        try:
+            self.conformer_select(config_idx)
+            self._data['config_idx'] = config_idx + 1
+            return self
+        except IndexError:
+            raise StopIteration
+
+    def __eq__(self, other):
+        """ if two molecule with 1.0 similarity in 2FP fingerprint they are identical """
+        if self.similarity(other) == 1.0:
+            return True
+        return False
+
+    def _add_temp_atom_labels(self):
+        """
+        Add temp atom label, These label will assist in the implementation of certain functions,
+        say Molecule.components. These label should be deleted after the assisted functions have
+        been fulfilled, by call method _delete_temp_atom_labels(self)
+        """
+        for i, atom in enumerate(self.atoms):
+            atom.set_ob_comment_data('temp_label', str(i))
+
+    @staticmethod
+    def _assign_coordinates(the_mol: 'Molecule', coordinates: np.ndarray):
+        """ Assign coordinates for all atoms in the Molecule """
+        if len(the_mol.atoms) != coordinates.shape[-2]:
+            raise AttributeError('the coordinate matrix do not match the number of atoms')
+
+        for new_mol_atom, new_atom_coord in zip(the_mol.atoms, coordinates):
+            new_mol_atom.coordinates = new_atom_coord
+
+    @property
+    def _attr_setters(self) -> Dict[str, Callable]:
+        return {
+            'atoms.partial_charge': self._set_atoms_partial_charge,
+            "identifier": self._set_identifier,
+            "energy": self._set_energy,
+            'all_energy': self._set_all_energy,
+            'charge': self._set_mol_charge,
+            'all_atom_charges': self._set_all_atom_charges,
+            'all_atom_spin_densities': self._set_all_atom_spin_densities,
+            'spin': self._set_spin_multiplicity,
+            'atoms': self._set_atoms,
+            'mol_orbital_energies': self._set_mol_orbital_energies,
+            'coordinates': self._set_coordinates,
+            'all_coordinates': self._set_all_coordinates,
+            'all_forces': self._set_all_forces,
+            'forces': self._set_forces,
+            'crystal': self.create_crystal_by_matrix
+        }
+
+    def _create_ob_unit_cell(self):
+        """ Create New OBUnitCell for the Molecule """
+        ob_unit_cell = ob.OBUnitCell()
+        self.ob_mol.CloneData(ob_unit_cell)
+
+    def _delete_atoms_temp_label(self):
+        """ Remove temp label of all atoms """
+        for a in self.atoms:
+            a.remove_ob_data('temp_label')
+
+    def _delete_bonds_temp_label(self):
+        """ Remove temp label of all bonds """
+        for b in self.bonds:
+            b.remove_ob_data('temp_label')
+
+    def _get_critical_params(self, name: str):
+        critical_params = self._data.get('critical_params')
+        if critical_params is None:
+            critical_params = json.load(open(opj(data_root, 'thermo', 'critical.json'))).get(self.smiles)
+            if critical_params:
+                self._data['critical_params'] = critical_params
+                return critical_params[name]
+            else:
+                self._data['critical_params'] = False
+                return False
+
+        else:
+            return critical_params[name]
+
+    def _has_atom_temp_label(self):
+        return any(atom.temp_label for atom in self.atoms)
+
+    def _pert_mol_generate(self, coordinates: Union[Sequence, np.ndarray]):
+        """
+        Generate new molecule obj according to new given coordinate
+        Args:
+            coordinates: New coordinates matrix
+
+        Returns:
+            Molecule, copy of this molecule with new coordinates
+        """
+        clone_mol = self.copy()
+        self._assign_coordinates(clone_mol, coordinates)
+        return clone_mol
+
+    def _load_atoms(self) -> Dict[int, 'Atom']:
+        """
+        Construct atoms dict according to the OBAtom in the OBMol,
+        where the keys of the dict are the ob_id of OBAtom and the values are the the constructed Atom objects
+        the constructed dict would be place into the _data dict
+        Returns:
+            the atoms dict
+        """
+        atoms: Dict[int, Atom] = self._data.get('atoms', {})
+
+        new_atoms = {}
+        for new_ob_id, oba in enumerate(ob.OBMolAtomIter(self.ob_mol)):
+            atom = atoms.get(oba.GetId(), Atom(oba, mol=self))
+            oba.SetId(new_ob_id)
+            new_atoms[new_ob_id] = atom
+
+        self._data['atoms'] = new_atoms
+
+        return new_atoms
+
+    def _load_bonds(self) -> Dict[int, 'Bond']:
+        """
+        Construct bonds dict according to the OBBond in the OBMol,
+        where the keys of the dict are the ob_id of OBBond and the values are the the constructed Bond objects
+        the constructed dict would be place into the _data dict
+        Returns:
+            dict of bonds
+        """
+        bonds: Dict = self._data.get('bonds', {})  # Get the stored bonds
+
+        new_bonds = {}
+        for new_ob_id, obb in enumerate(ob.OBMolBondIter(self.ob_mol)):
+            bond = bonds.get(obb.GetId(), Bond(obb, self))  # Get old bond by old id
+            obb.SetId(new_ob_id)  # Specify new id
+            new_bonds[new_ob_id] = bond
+
+        self._data['bonds'] = new_bonds
+
+        return new_bonds
+
+    @staticmethod
+    def _melt_quench(
+            elements: Dict[str, float], force_field: Union[str, os.PathLike], mol: "Molecule" = None,
+            density: float = 1.0, a: float = 25., b: float = 25., c: float = 25.,
+            alpha: float = 90., beta: float = 90., gamma: float = 90., time_step: float = 0.0001,
+            origin_temp: float = 298.15, melt_temp: float = 4000., highest_temp: float = 10000.,
+            ff_args: Sequence = (), path_writefile: Optional[str] = None, path_dump_to: Optional[str] = None,
+            dump_every: int = 100,
+    ):
+        """ to perform the melt-quench by call lmp.AmorphousMaker """
+        am = lmp.AmorphousMaker(elements, force_field, density, a, b, c, alpha, beta, gamma)
+        mol = am.melt_quench(
+            *ff_args, mol=mol, path_writefile=path_writefile, path_dump_to=path_dump_to, origin_temp=origin_temp,
+            melt_temp=melt_temp, highest_temp=highest_temp, time_step=time_step, dump_every=dump_every
+        )
+
+        return mol
+
+    def _merge_conformer_attr(self, other: 'Molecule'):
+        """ Merge attributes, relate to molecule conformer, in other Molecule into this Molecule """
+
+        def merge_attr(attr_name: str):
+            """ Merge single conformer attr """
+            left_attr = getattr(self, attr_name)
+            right_attr = getattr(other, attr_name)
+
+            if isinstance(left_attr, np.ndarray) and isinstance(right_attr, np.ndarray):
+                self._data[attr_name] = np.concatenate([left_attr, right_attr])
+            elif not (  # If the left and right values are not both empty, raise Attributes error.
+                    (left_attr is None) or (isinstance(left_attr, np.ndarray) and (not left_attr.all())) and
+                    (right_attr is None) or (isinstance(right_attr, np.ndarray) and (not right_attr.all()))
+            ):
+                raise AttributeError(
+                    f'the conformer relational attribute {attr_name} is different in:\n'
+                    f'  - {self}_identifier: {self.identifier}\n'
+                    f'  - {other}_identifier: {other.identifier}'
+                    'they cannot to perform addition operation'
+                )
+
+        for i, items in enumerate(self.conformer_items):
+            for item in items:
+                merge_attr(item)
+
+        return self
+
+    def _preserve_atoms_data(self):
+        """
+        Preserve atoms data dict before destroy them.
+        Though the atoms are destroyed, their core ob_atom will be prevented,
+        The reserve data will match with the core ob_atoms
+        """
+        # Link the old atoms data dict with new atoms by temp labels
+        self._add_temp_atom_labels()
+        return {a.temp_label: a.data for a in self.atoms}
+
+    def _preserve_bonds_data(self):
+        """"""
+        if not self._has_atom_temp_label():
+            self._add_temp_atom_labels()
+
+        return {(b.atom1.temp_label, b.atom2.temp_label): b.data for b in self.bonds}
+
+    def _preserve_angles_data(self):
+        if not self._has_atom_temp_label():
+            self._add_temp_atom_labels()
+
+        return {tuple(atom.temp_label for atom in angle.atoms): angle.data for angle in self.angles}
+
+    def _preserve_torsion_data(self):
+        if not self._has_atom_temp_label():
+            self._add_temp_atom_labels()
+
+        return {tuple(atom.temp_label for atom in torsion.atoms): torsion.data for torsion in self.torsions}
+
+    @property
+    def _protected_data(self):
+        return 'ob_obj', 'atoms', 'bonds', 'angles'
+
+    def _reorder_atom_ob_id(self):
+        """ Reorder the ob id of atoms """
+        new_atom_dict = {}
+        for ob_id, atom in enumerate(self.atoms):
+            atom.ob_atom.SetId(ob_id)
+            new_atom_dict[ob_id] = atom
+
+        self._data['atoms'] = new_atom_dict
+
+    def _reorder_bond_ob_id(self):
+        new_atom_dict = {}
+        for ob_id, bond in enumerate(self.bonds):
+            bond.ob_bond.SetId(ob_id)
+            new_atom_dict[ob_id] = bond
+
+        self._data['bonds'] = new_atom_dict
+
+    def _reorganize_atom_indices(self):
+        """ reorganize or rearrange the indices for all atoms """
+        for i, ob_atom in enumerate(ob.OBMolAtomIter(self.ob_mol)):
+            ob_atom.SetId(i)
+
+    def _set_atoms(self, atoms_kwargs: List[Dict[str, Any]]):
+        """ add a list of atoms by a list atoms attributes dict """
+        for atom_kwarg in atoms_kwargs:
+            a = Atom(**atom_kwarg)
+            self.add_atom(a)
+
+    def _set_atoms_partial_charge(self, partial_charges: [np.ndarray, Sequence[float]]):
+        """ Set partial charges for all atoms in the molecule """
+        if not isinstance(partial_charges, (np.ndarray, Sequence[int])):
+            raise TypeError(
+                f'the `partial_charges` should be np.ndarray or Sequence of float, not {type(partial_charges)}'
+            )
+
+        if self.atom_counts != len(partial_charges):
+            raise ValueError('the given partial charges should have same numbers with the number of atoms')
+
+        for atom, partial_charge in zip(self.atoms, partial_charges):
+            atom.partial_charge = partial_charge
+
+    def _set_all_coordinates(self, all_coordinates: np.ndarray):
+        """
+        Assign the coordinates collection directly
+        Args:
+            all_coordinates: numpy array with the shape (M, N, 3), where the M is the number of coordinates
+            in the collection, the N is the number of atoms of the molecule.
+
+        Returns:
+            None
+        """
+        if not isinstance(all_coordinates, np.ndarray):
+            raise ValueError(
+                f'the given all_coordinates must be a numpy.ndarray class, instead of {type(all_coordinates)}')
+
+        if all_coordinates.shape[-1] != 3:
+            raise ValueError(f'the coordinate must be 3 dimension, instead of {all_coordinates.shape[-1]}')
+
+        if len(all_coordinates.shape) == 2:
+            # if only give a group of coordinates
+            all_coordinates = all_coordinates.reshape((-1, all_coordinates.shape[-2], 3))
+        elif len(all_coordinates.shape) != 3:
+            raise ValueError(
+                f'the shape of given all_coordinates should with length 2 or 3, now is {len(all_coordinates.shape)}'
+            )
+
+        self._data['all_coordinates'] = all_coordinates
+
+    def _set_coordinates(self, coordinates: np.ndarray):
+        """ Assign the coordinates for all atoms in the molecule """
+        assert isinstance(coordinates, np.ndarray)
+        assert coordinates.shape == (self.atom_counts, 3)
+
+        for a, c in zip(self.atoms, coordinates):
+            a.coordinates = c
+
+    def _set_atom_charges(self, charge: Union[Sequence, np.ndarray]):
+        """ Set partial charge for each atoms in the mol """
+        if not isinstance(charge, (Sequence, np.ndarray)):
+            raise TypeError(f'the charge should be a sequence or np.ndarray, got {type(charge)}')
+
+        if isinstance(charge, np.ndarray):
+            charge = charge.flatten()
+
+        if len(charge) != self.atom_counts:
+            raise ValueError('the number of charges do not match with the atom charge')
+
+        for atom, ch in zip(self.atoms, charge):
+            atom.partial_charge = ch
+
+    def _set_all_atom_charges(self, charges: np.ndarray):
+        """
+        set groups of charges for each atoms in the mol, and each group of charges are corresponding to a
+        conformer of the mol
+        Args:
+            charges: group of atoms with the shape of (C, N), where the C is the number of the conformer
+             and the N is the number of the atom in the molecule
+        """
+        if not isinstance(charges, np.ndarray):
+            raise TypeError('the arg charges should be np.ndarray')
+
+        if len(charges.shape) != 2 and charges.shape[1] != self.atom_counts:
+            raise ValueError('the shape of the arg: charge should be (number_of_conformer, number_of_atoms),'
+                             f'got the value with shape {charges.shape}')
+
+        self._data['all_atom_charges'] = charges
+
+    def _set_all_atom_spin_densities(self, group_spd: np.ndarray) -> None:
+        """
+        assign groups of spin densities for all atom in molecule, each group is corresponding to a conformer
+        Args:
+            group_spd(np.ndarray): group of spin densities, the numpy array with the (C, N) shape,
+             where the C is the number of conformer, the N is the number of atoms
+        """
+        if not isinstance(group_spd, np.ndarray):
+            raise TypeError('the arg group_spd should be np.ndarray')
+
+        if len(group_spd.shape) != 2 and group_spd.shape[1] != self.atom_counts:
+            raise ValueError('the shape of the arg: group_spd should be (number_of_conformer, number_of_atoms),'
+                             f'got the value with shape {group_spd.shape}')
+
+        self._data['all_atom_spin_densities'] = group_spd
+
+    def _set_atom_spin_densities(self, spd: Union[Sequence, np.ndarray]):
+        """ assign the spin density for each of atoms in the mol """
+        if not isinstance(spd, (Sequence, np.ndarray)):
+            raise TypeError(f'the charge should be a sequence or np.ndarray, got {type(spd)}')
+
+        if isinstance(spd, np.ndarray):
+            spd = spd.flatten()
+
+        if len(spd) != self.atom_counts:
+            raise ValueError('the number of charges do not match with the atom charge')
+
+        for atom, sp in zip(self.atoms, spd):
+            atom.spin_density = sp
+
+    def _set_forces(self, forces: np.ndarray):
+        """ Set the force vectors for each atoms in the molecule """
+        if not isinstance(forces, np.ndarray):
+            raise TypeError('the forces should be np.ndarray')
+
+        if len(forces.shape) != 2:
+            raise ValueError('the length of shape of forces should be 2')
+
+        if forces.shape[-2] != self.atom_counts:
+            raise ValueError('the give forces do not match to the number of atoms')
+
+        for atom, force_vector in zip(self.atoms, forces):
+            atom.force_vector = force_vector
+
+    def _set_all_forces(self, all_forces: np.ndarray):
+        """ Store the force matrix into the attribute dict """
+        if not isinstance(all_forces, np.ndarray):
+            raise TypeError('the all_forces should be np.ndarray')
+
+        if len(all_forces.shape) != 3:
+            raise ValueError('the length of shape of all_forces should be 3')
+
+        if all_forces.shape[-2] != self.atom_counts:
+            raise ValueError('the give all_forces do not match to the number of atoms')
+
+        self._data['all_forces'] = all_forces
+
+    def _set_mol_charge(self, charge: int):
+        self.ob_mol.SetTotalCharge(charge)
+
+    def _set_mol_orbital_energies(self, orbital_energies: list[np.ndarray]):
+        self._data['mol_orbital_energies'] = orbital_energies[0]
+
+    def _set_energy(self, energy: float):
+        """ set the energy """
+        self.ob_mol.SetEnergy(energy)
+
+    def _set_all_energy(self, all_energy: Union[float, np.ndarray]):
+        """ set the energy for all conformers """
+        if isinstance(all_energy, float):
+            self._data['all_energy'] = np.array([all_energy])
+        else:
+            all_energy = all_energy.flatten()
+            self._data['all_energy'] = all_energy
+
+    def _set_identifier(self, identifier):
+        self.ob_mol.SetTitle(identifier)
+
+    def _set_spin_multiplicity(self, spin):
+        self.ob_mol.SetTotalSpinMultiplicity(spin)
+
+    @staticmethod
+    def _transfer_preserve_data_to_new_atoms(tgt_mol: 'Molecule', preserve_data: Dict, rm_temp_label: bool = False):
+        """
+        Transfer preserve data dict to new target Molecule atoms
+        Args:
+            tgt_mol: The target Molecule
+            preserve_data(dict): the old atoms data dict
+            rm_temp_label: whether to remove temp label after data have been transferred.
+        """
+        for atom in tgt_mol.atoms:
+            temp_label = atom.temp_label
+            if temp_label:
+                atom.update_attr_data(preserve_data[temp_label])
+
+                if rm_temp_label:
+                    atom.remove_ob_data('temp_label')
+
+    @staticmethod
+    def _transfer_preserve_data_to_new_bonds(tgt_mol: 'Molecule', preserve_data: Dict):
+        """
+        Transfer preserve data dict to new target Molecule bonds
+        Args:
+            tgt_mol: The target Molecule
+            preserve_data(dict): the old atoms data dict
+        """
+        for bond in tgt_mol.bonds:
+            temp_label = (bond.atom1.temp_label, bond.atom2.temp_label)
+            if all(temp_label):
+                try:
+                    bond.update_attr_data(preserve_data[temp_label])
+                except KeyError:
+                    bond.update_attr_data(preserve_data[temp_label[::-1]])
+
+    @staticmethod
+    def _transfer_preserve_data_to_new_angles(tgt_mol: 'Molecule', preserve_data: Dict):
+        for angle in tgt_mol.angles:
+            temp_label = tuple(atom.temp_label for atom in angle.atoms)
+            if all(temp_label):
+                try:
+                    angle.update_attr_data(preserve_data[temp_label])
+                except KeyError:
+                    angle.update_attr_data(preserve_data[temp_label[::-1]])
+
+    @staticmethod
+    def _transfer_preserve_data_to_new_torsions(tgt_mol: 'Molecule', preserve_data: Dict):
+        for torsion in tgt_mol.torsions:
+            temp_label = tuple(atom.temp_label for atom in torsion.atoms)
+            if all(temp_label):
+                try:
+                    torsion.update_attr_data(preserve_data[temp_label])
+                except KeyError:
+                    torsion.update_attr_data(preserve_data[temp_label[::-1]])
+
+    @property
+    def acentric_factor(self):
+        return self._get_critical_params('acentric_factor')
+
+    def add_atom(self, atom: Union["Atom", str, int], **atom_attrs) -> 'Atom':
+        """
+        Add a new atom out of the molecule into the molecule.
+        Args:
+            atom(Atom|str|int):
+
+        atom_kwargs(kwargs for this added atom):
+            atomic_number(int): set atomic number
+            symbol(str): set atomic symbol
+            coordinates(Sequence, numpy.ndarray): coordinates of the atom
+            partial_charge:
+            label:
+            spin_density:
+
+        Returns:
+            the copy of atom in the molecule
+        """
+        oba = ob.OBAtom()  # Initialize a new OBAtom
+        data = None
+        if isinstance(atom, str):
+            oba.SetAtomicNum(ob.GetAtomicNum(atom))
+        elif isinstance(atom, int):
+            oba.SetAtomicNum(atom)
+        elif isinstance(atom, Atom):
+            oba.SetAtomicNum(atom.atomic_number)
+            data = atom.data  # Copy the give atoms data
+
+        # add OBAtom to the OBMol
+        success = self.ob_mol.AddAtom(oba)
+
+        if success:
+            atom = self.atoms[-1]  # Retrieve the added atom
+
+            if data:
+                atom.update_attr_data(data)  # replicant the old atom's data to the new
+
+            atom.set(**atom_attrs)  # Set attributes by kwargs
+
+            return atom
+
+        else:
+            raise AddAtomFail(f'Add the atom {atom} into Molecule fail')
+
+    @property
+    def all_atoms_with_unique_symbol(self):
+        return self.atoms_with_unique_symbol + \
+            self.pseudo_atoms_with_unique_symbol
+
+    def add_bond(
+            self,
+            atom1: Union[str, int, 'Atom'],
+            atom2: Union[str, int, 'Atom'],
+            bond_type: Union[str, int],
+    ):
+        """ Add a new bond into the molecule """
+        inputs = (atom1, atom2)
+        atoms: List[Atom] = []
+        for a in inputs:
+            if isinstance(a, int):
+                atoms.append(self.atoms_dict[a])
+            if isinstance(a, Atom):
+                atoms.append(a)
+            if isinstance(a, str):
+                atoms.append(self.atom(a))
+
+        # Represent the bond type by int, refer to _bond_type dict
+        bond_type = bond_type if isinstance(bond_type, int) else _bond_type[bond_type]
+
+        # Try to add new OBMol
+        # 'openbabel' has an odd behave that `index` of the `OBAtom` with various origin in the `OBMol`.
+        # the `Id` of `OBAtom` from 0; but the `Idx` of `OBAtom` from 1.
+        # To meet the convention, the `Id` is selected to be the unique `index` to specify `Atom`.
+        # However, when try to add a `OBBond` to link each two `OBAtoms`, the `Idx` is the only method
+        # to specify the atoms, so our `index` in `Atom` are added 1 to match the 'Idx'
+        success = self.ob_mol.AddBond(atoms[0].ob_idx, atoms[1].ob_idx, bond_type)
+
+        if success:
+            return self.bonds[-1]  # the new atoms should place in the terminal of the bond list
+
+        elif atoms[0].ob_id not in self.atom_indices:
+            raise KeyError("the start atom1 doesn't exist in molecule")
+
+        elif atoms[1].ob_id not in self.atom_indices:
+            raise KeyError("the end atom2 doesn't exist in molecule")
+
+        else:
+            raise RuntimeError('add bond not successful!')
+
+    def add_hydrogens(
+            self,
+            polar_only: bool = False,
+            correct_for_ph: bool = False,
+            ph: float = 1.0,
+            balance_hydrogen: bool = True,
+    ):
+        """
+        add hydrogens for the molecule
+        Args:
+            ph: add hydrogen in which PH environment
+            polar_only: Whether to add hydrogens only to polar atoms (i.e., not to C atoms)
+            correct_for_ph: Correct for pH by applying the OpenBabel::OBPhModel transformations
+            balance_hydrogen: whether to balance the bond valance of heavy atom to their valence
+        """
+        self.ob_mol.AddHydrogens(polar_only, correct_for_ph, ph)
+        self._load_atoms()
+        self._load_bonds()
+
+        if balance_hydrogen:
+            for atom in self.atoms:
+                atom.balance_hydrogen()
+
+    def add_pseudo_atom(self, symbol: str, mass: float, coordinates: Union[Sequence, np.ndarray], **kwargs):
+        """ Add pseudo atom into the molecule """
+        list_pseudo_atom = self._data.setdefault('pseudo_atoms', [])
+        pa = PseudoAtom(symbol, mass, coordinates, mol=self, molecule=self, **kwargs)
+        list_pseudo_atom.append(pa)
+
+    @property
+    def all_coordinates(self) -> np.ndarray:
+        """
+        Get the collections of the matrix of all atoms coordinates,
+        each matrix represents a conformer.
+        The return array with shape of (C, N, 3),
+        where the C is the number of conformers, the N is the number of atoms
+        """
+        all_coordinates = self._data.get('all_coordinates')
+        if isinstance(all_coordinates, np.ndarray):
+            return all_coordinates
+        else:
+            return self.coordinates.reshape((-1, self.atom_counts, 3))
+
+    @property
+    def all_energy(self):
+        return self._data.get('all_energy')
+
+    @property
+    def angles(self):
+        return [Angle(self, *a_idx) for a_idx in ob.OBMolAngleIter(self.ob_mol)]
+
+    def assign_bond_types(self):
+        self.ob_mol.PerceiveBondOrders()
+
+    def atom(self, id_label: Union[int, str]) -> 'Atom':
+        """ get atom by label or idx """
+        if isinstance(id_label, str):
+
+            if not self.is_labels_unique:
+                raise AttributeError(
+                    'the label is not unique, cannot get atom by label. try to get atom by ob_id '
+                    'or normalize the label before'
+                )
+
+            for atom in self.atoms:
+                if atom.label == id_label:
+                    return atom
+            raise KeyError(f'No atom with label {id_label}')
+
+        elif isinstance(id_label, int):
+            return self.atoms_dict[id_label]
+        else:
+            raise TypeError(f'the given idx_label is expected to be int or string, but given {type(id_label)}')
+
+    @property
+    def atom_counts(self):
+        return self.ob_mol.NumAtoms()
+
+    @property
+    def atomic_numbers(self) -> Tuple[int]:
+        return tuple(a.atomic_number for a in self.atoms)
+
+    @property
+    def atomic_numbers_array(self) -> np.ndarray:
+        """ conformer corresponding attributes with array shape (number_of_atoms, number_of_conformers) """
+        return np.array(self.atomic_numbers).reshape(1, -1).repeat(self.conformer_counts, axis=0)
+
+    @property
+    def atomic_symbols(self):
+        return tuple(a.symbol for a in self.atoms)
+
+    @property
+    def atoms(self) -> List['Atom']:
+        """
+        Generate dict of Atom objects into the data repository.
+        Return list of Atom objects with the order their index.
+        """
+        atoms = self._load_atoms()
+        return list(atoms.values())
+
+    @property
+    def atoms_dict(self) -> Dict[int, 'Atom']:
+        return self._load_atoms()
+
+    @property
+    def atoms_with_unique_symbol(self):
+        uni_atoms, uni_symbol = [], set()
+        for a in self.pseudo_atoms:
+            if a.symbol not in uni_symbol:
+                uni_atoms.append(a)
+                uni_symbol.add(a.symbol)
+
+        return uni_atoms
+
+    @property
+    def pseudo_atoms_with_unique_symbol(self):
+        uni_patoms, uni_psymbol = [], set()
+        for a in self.atoms:
+            if a.symbol not in uni_psymbol:
+                uni_patoms.append(a)
+                uni_psymbol.add(a.symbol)
+
+        return uni_patoms
+
+    @property
+    def all_atoms(self):
+        return self.atoms + self.pseudo_atoms
+
+    @property
+    def atom_charges(self) -> np.ndarray:
+        """ Return all atoms charges as a numpy array """
+        return np.array([a.partial_charge for a in self.atoms])
+
+    @property
+    def all_atom_charges(self) -> np.ndarray:
+        """ Return all atoms charges as a numpy array for every conformers """
+        all_atom_charges = self._data.get('all_atom_charges')
+        if isinstance(all_atom_charges, np.ndarray):
+            return all_atom_charges
+        return self.atom_charges.reshape((-1, self.atom_counts))
+
+    @property
+    def atom_indices(self) -> list[int]:
+        return [a.ob_id for a in self.atoms]
+
+    @property
+    def atom_labels(self) -> list[str]:
+        return [a.label for a in self.atoms]
+
+    @property
+    def atom_spin_densities(self) -> np.ndarray:
+        return np.array([a.spin_density for a in self.atoms])
+
+    @property
+    def all_atom_spin_densities(self):
+        all_atom_spin_densities = self._data.get('all_atom_spin_densities')
+        if all_atom_spin_densities is not None:
+            return all_atom_spin_densities
+        return self.atom_spin_densities.reshape((-1, self.atom_counts))
+
+    def assign_atoms_formal_charge(self):
+        """ Assign the formal charges for all atoms in the molecule """
+        self.add_hydrogens(balance_hydrogen=False)
+
+        for atom in self.atoms:
+            if atom.is_polar_hydrogen:
+                atom.formal_charge = 1
+            elif atom.is_hydrogen or atom.is_carbon:
+                atom.formal_charge = 0
+            elif atom.is_metal:
+                atom.formal_charge = _stable_charges[atom.symbol]
+            elif [a for a in atom.neighbours if a.is_polar_hydrogen]:
+                atom.formal_charge = -(len([a for a in atom.neighbours if a.is_polar_hydrogen]))
+            elif atom.symbol in ['S', 'P']:
+                if not [a for a in atom.neighbours if a.symbol == 'O']:
+                    atom.formal_charge = atom.covalent_valence - (2 if atom.symbol == 'S' else 3)
+                else:
+                    atom.formal_charge = 0
+            else:
+                atom.formal_charge = atom.covalent_valence - atom.stable_valence
+
+    def balance_hydrogens(self):
+        """ Add or remove hydrogens for make or heave atom to achieve the stable valence """
+        for a in self.heavy_atoms():
+            a.balance_hydrogen()
+
+    def angle(self, a: Union[str, int], v: Union[str, int], b: Union[str, int]) -> 'Angle':
+        """
+        Get a Angle from Molecule by ob_id or atom label
+        Args:
+            a: the ob_id or atom label of the first end atom
+            v: the ob_id or atom label of the vertex atom
+            b: the ob_id or atom label of the second end atom
+
+        Returns:
+            Angle
+        """
+        a: Atom = self.atom(a)
+        v: Atom = self.atom(v)
+        b: Atom = self.atom(b)
+
+        assert self.bond(a.ob_id, v.ob_id)
+        assert self.bond(v.ob_id, b.ob_id)
+
+        return Angle(self, v.ob_id, a.ob_id, b.ob_id)
+
+    def torsion(self, a: Union[str, int], b: Union[str, int], c: Union[str, int], d: Union[str, int]) -> 'Torsion':
+        """
+        Get a Torsion from Molecule by ob_id or atom label
+        Args:
+            a: the ob_id or atom label of the first end atom
+            b: the ob_id or atom label of the first internal atom
+            c: the ob_id or atom label of the second internal atom
+            d: the ob_id or atom label of the second internal atom
+
+        Returns:
+            Torsion
+        """
+        a: Atom = self.atom(a)
+        b: Atom = self.atom(b)
+        c: Atom = self.atom(c)
+        d: Atom = self.atom(d)
+
+        # Todo: The reason why these assert can't successful is still uncertain,
+        # Todo: Refer to the rule of Z-Matrix in Gaussian16
+        # assert self.bond(a.ob_id, b.ob_id)
+        # assert self.bond(b.ob_id, c.ob_id)
+        # assert self.bond(c.ob_id, d.ob_id)
+
+        return Torsion(self, a.ob_id, b.ob_id, c.ob_id, d.ob_id)
+
+    def bond(self, atom1: Union[int, str], atom2: Union[int, str]) -> 'Bond':
+        """
+        Return the Bond by given atom index labels in the bond ends
+        if the bond is missing in the molecule, return None if given miss_raise is False else raise a KeyError
+        Args:
+            atom1(int|str): index or label of atom in one of the bond end
+            atom2(int|str): index or label of atom in the other end of the bond
+
+        Returns:
+            Bond
+
+        Raises:
+            KeyError: when can't find the bond, and the miss_raise passing True
+
+        """
+        atom1: Atom = self.atom(atom1)
+        atom2: Atom = self.atom(atom2)
+        ob_bond = self.ob_mol.GetBond(atom1.ob_atom, atom2.ob_atom)
+
+        if ob_bond:
+            return self.bonds_dict[ob_bond.GetId()]
+
+    @property
+    def bond_pair_keys(self):
+        return [b.pair_key for b in self.bonds]
+
+    @property
+    def bonds(self):
+        bonds = self._load_bonds()
+        return list(bonds.values())
+
+    @property
+    def bonds_dict(self) -> Dict[int, 'Bond']:
+        return self._load_bonds()
+
+    def build_2d(self):
+        """ build 2d conformer """
+        pmol = pb.Molecule(self.ob_mol)
+        pmol.make2D()
+
+    def build_3d(self, force_field: str = 'UFF', steps: int = 500):
+        """ build 3D coordinates for the molecule """
+        # Preserve atoms data before building
+        preserve_atoms_data = self._preserve_atoms_data()
+        preserve_bonds_data = self._preserve_bonds_data()
+        preserve_angles_data = self._preserve_angles_data()
+        preserve_torsion_data = self._preserve_torsion_data()
+
+        # Destroy atoms and bonds wrappers
+        self._data['atoms'] = {}
+        self._data['bonds'] = {}
+
+        # Build 3d conformer
+        pymol = pb.Molecule(self.ob_mol)
+        pymol.make3D(force_field, steps)
+
+        # Reload atoms and bonds
+        self._load_atoms()
+        self._load_bonds()
+
+        # Transfer preserve data to new
+        self._transfer_preserve_data_to_new_atoms(self, preserve_atoms_data)
+        self._transfer_preserve_data_to_new_bonds(self, preserve_bonds_data)
+        self._transfer_preserve_data_to_new_angles(self, preserve_angles_data)
+        self._transfer_preserve_data_to_new_torsions(self, preserve_torsion_data)
+
+        # Delete temp label
+        self._delete_atoms_temp_label()
+
+        # Remove redundant hydrogen or supply the lack hydrogens
+        self.balance_hydrogens()
+
+    def build_bonds(self):
+        self.ob_mol.ConnectTheDots()
+
+    @property
+    def center_of_masses(self):
+        return (self.masses * self.coordinates.T).T.sum(axis=0) / self.masses.sum()
+
+    @property
+    def center_of_shape(self):
+        return self.coordinates.mean(axis=0)
+
+    @property
+    def charge(self):
+        return self.ob_mol.GetTotalCharge()
+
+    @charge.setter
+    def charge(self, charge):
+        self._set_mol_charge(charge)
+
+    def clean_bonds(self):
+        """ Remove all bonds """
+        # Iterate directly will fail.
+        ob_bonds = [ob_bond for ob_bond in ob.OBMolBondIter(self.ob_mol)]
+        for ob_bond in ob_bonds:
+            self.ob_mol.DeleteBond(ob_bond)
+
+    def clean_conformers(self, pop: bool = False):
+        """ clean all config save inside the molecule """
+        try:
+            all_coordinates = self._data.pop('all_coordinates')
+        except KeyError:
+            all_coordinates = None
+
+        if pop:
+            return all_coordinates
+
+    @property
+    def components(self):
+        """ get all fragments don't link each by any bonds """
+        # Add temp label for each atom first
+        preserve_data = self._preserve_atoms_data()
+
+        components = [self.__class__(obc) for obc in self.ob_mol.Separate()]
+
+        # Transfer the parent data attr to the children
+        for c in components:
+            for a in c.atoms:
+                a.update_attr_data(preserve_data[a.temp_label])
+                a.remove_ob_data('temp_label')
+
+        # remove temp labels of all atoms
+        self._delete_atoms_temp_label()
+
+        return components
+
+    @property
+    def conformer_counts(self) -> int:
+        """ The number of conformers in the molecule """
+        all_coordinates = self._data.get('all_coordinates')
+        if isinstance(all_coordinates, np.ndarray):
+            return all_coordinates.shape[0]
+        else:
+            return 1
+
+    def conformer_select(self, conf_idx: int):
+        """ select specific conformer by index """
+
+        def assign_numpy_attrs(attrs_name: str, setter: Callable):
+            attrs = self._data.get(attrs_name)
+            if isinstance(attrs, np.ndarray):
+                try:
+                    attr = attrs[conf_idx]
+                except IndexError:
+                    attr = None
+            else:
+                attr = None
+
+            if isinstance(attr, np.ndarray) or attr:
+                setter(attr)
+
+        all_coordinates = self._data.get('all_coordinates')
+        if all_coordinates is None and conf_idx:
+            raise IndexError('Only one conformer here!')
+
+        # assign the coordinates for the molecule
+        coordinates = all_coordinates[conf_idx]
+        self._assign_coordinates(self, coordinates)
+
+        assign_numpy_attrs('all_energy', self._set_energy)
+
+        assign_numpy_attrs('all_atom_charges', self._set_atom_charges)
+
+        assign_numpy_attrs('all_atom_spin_densities', self._set_atom_spin_densities)
+
+        assign_numpy_attrs('all_forces', self._set_forces)
+
+    @property
+    def coordinates(self) -> np.ndarray:
+        """
+        Get the matrix of all atoms coordinates,
+        where the row index point to the atom index;
+        the column index point to the (x, y, z)
+        """
+        return np.array([atom.coordinates for atom in self.atoms], dtype=np.float64)
+
+    def copy(self) -> 'Molecule':
+        """ Get a clone of this Molecule """
+        clone = self.__class__(self.ob_copy())
+        clone._load_atoms()
+        clone._load_bonds()
+
+        # Copy the Molecule's attr data to the clone one
+        clone.update_attr_data(self.data)
+        # Copy the Atoms' attr data to the clone ones
+        for atom in clone.atoms:
+            atom.update_attr_data(self.atoms_dict[atom.ob_id].data)
+            atom.molecule = clone
+        # Copy the Bonds' attr data to the lone ones
+        for bond in clone.bonds:
+            bond.update_attr_data(self.bonds_dict[bond.ob_id].data)
+            bond.molecule = clone
+
+        return clone
+
+    def compact_crystal(self, inplace=False):
+        """"""
+        mol = self if inplace else self.copy()
+        lattice_params = np.concatenate((self.xyz_diff, [90., 90., 90.]))
+
+        mol.make_crystal(*lattice_params)
+
+        return mol
+
+    def create_crystal_by_vectors(
+            self,
+            va: Union[Sequence, np.ndarray],
+            vb: Union[Sequence, np.ndarray],
+            vc: Union[Sequence, np.ndarray]
+    ):
+        """ Create a new crystal with specified cell vectors for the Molecule """
+        self._create_ob_unit_cell()
+        self.crystal().set_vectors(va, vb, vc)
+
+    def create_crystal_by_matrix(self, matrix: np.ndarray):
+        """ Create a new crystal with specified cell matrix for the molecule """
+        if not (np.logical_not(matrix >= 0.).any() and np.logical_not(matrix < 0.).any()) and np.linalg.det(matrix):
+            self._create_ob_unit_cell()
+            self.crystal().set_matrix(matrix)
+            # self.crystal().space_group = 'P1'
+
+    @classmethod
+    def create_aCryst_by_mq(
+            cls, elements: Dict[str, float], force_field: Union[str, os.PathLike],
+            density: float = 1.0, a: float = 25., b: float = 25., c: float = 25.,
+            alpha: float = 90., beta: float = 90., gamma: float = 90., time_step: float = 0.0001,
+            origin_temp: float = 298.15, melt_temp: float = 4000., highest_temp: float = 10000.,
+            ff_args: Sequence = (), path_writefile: Optional[str] = None, path_dump_to: Optional[str] = None,
+            dump_every: int = 100
+    ):
+        """
+        Create a Amorphous crystal materials by Melt-Quench process.
+        This process is performed by LAMMPS package, make sure the LAMMPS is accessible.
+        A suitable force field is required for the process are performed correctly.
+        Args:
+            elements(dict[str, float]): Dict of elements and their composition ratio
+            force_field(str, os.PathLike): The name of force filed or the path to load a force filed. The name
+             of the force filed is refer to the relative path to the 'hotpot_root/data/force_field'.
+            density: the demand density for the created amorphous crystal
+            a: the length of a vector in the crystal
+            b: the length of b vector in the crystal
+            c: the length of c vector in the crystal
+            alpha: alpha angle of crystal param.
+            beta: beta angle of crystal param.
+            gamma: gamma angle of crystal param
+            time_step: time interval between path integrals when performing melt-quench
+            origin_temp: the initial temperature before melt
+            melt_temp: the round melting point to the materials
+            highest_temp: the highest temperature to liquefy the materials
+            ff_args: the arguments the force file requried, refering the LAMMPS pair_coeff:
+             "pair_coeff I J args" url: https://docs.lammps.org/pair_coeff.html
+            path_writefile: the path to write the final material (screenshot) to file, if not specify, not save.
+            path_dump_to:  the path to save the trajectory of the melt-quench process, if not specify not save.
+            dump_every: the step interval between each dump operations
+
+        Returns:
+            Molecule, a created amorphous material
+        """
+        return cls._melt_quench(
+            elements=elements, force_field=force_field, density=density,
+            a=a, b=b, c=c, alpha=alpha, beta=beta, gamma=gamma, time_step=time_step,
+            origin_temp=origin_temp, melt_temp=melt_temp, highest_temp=highest_temp,
+            ff_args=ff_args, path_writefile=path_writefile, path_dump_to=path_dump_to,
+            dump_every=dump_every
+        )
+
+    @property
+    def critical_pressure(self):
+        return self._get_critical_params('pressure')
+
+    @property
+    def critical_temperature(self):
+        return self._get_critical_params('temperature')
+
+    def crystal(self):
+        """ Get the Crystal containing the Molecule """
+        cell_index = ob.UnitCell  # Get the index the UnitCell data save
+        cell_data = self.ob_mol.GetData(cell_index)
+
+        if cell_data:
+            ob_unit_cell = ob.toUnitCell(cell_data)
+            return Crystal(ob_unit_cell, molecule=self)
+        else:
+            return None
+
+    def dump(self, fmt: str, *args, **kwargs) -> Union[str, bytes, dict, 'DeepSystem']:
+        """"""
+        dumper = Dumper(fmt=fmt, source=self, *args, **kwargs)
+        return dumper()
+
+    @property
+    def elements(self) -> list[str]:
+        return re.findall(r'[A-Z][a-z]*', self.formula)
+
+    @property
+    def energy(self):
+        """ Return energy with kcal/mol as default """
+        return self.ob_mol.GetEnergy()
+
+    def feature_matrix(self, *feature_names: Sequence) -> np.ndarray:
+        """ Retrieve the feature matrix (collections of feature vector for atoms),
+         The default feature is `atomic_orbital`, if the feature names not be specified, the `atomic_orbital` will be
+         retrieved.
+         Args:
+             feature_names: the feature names are offered in hotpot/data/periodic_table.json
+         """
+        if not feature_names:
+            feature_names = ('atomic_orbital',)
+
+        # Matrix with shape (atom_numbers, feature_length)
+        return np.stack([atom.element_features(*feature_names) for atom in self.atoms])
+
+    def fingerprint(self, fptype: Literal['FP2', 'FP3', 'FP4', 'MACCS'] = 'FP2'):
+        """
+        Calculate the molecular fingerprint for this molecule, the supporting fingerprint include:
+
+        1. "FP2": The FP2 fingerprint is a path-based fingerprint that encodes the presence of linear
+        fragments up to 7 atoms long. It is a 1024-bit fingerprint and is commonly used for substructure
+        searches and similarity calculations.
+
+        2. "FP3": The FP3 fingerprint is designed for searching 3D conformations, such as those found
+        in protein-ligand complexes. It encodes the presence of particular pharmacophoric features,
+        such as hydrogen bond donors, acceptors, and hydrophobic regions.
+
+        3. "FP4": The FP4 fingerprint is a circular fingerprint based on the Morgan algorithm. It
+        captures information about the local environment of each atom in the molecule, up to a certain
+        radius. It is useful for similarity calculations and machine learning tasks.
+
+        4. "MACCS": The MACCS fingerprint is a 166-bit structural key-based fingerprint. It represents
+        the presence of specific substructures or functional groups defined by the MACCS keys. It is
+        commonly used for similarity calculations and substructure searches.
+
+        Return:
+            the Fingerprint object in pybel module
+        """
+        return pb.Molecule(self.ob_mol).calcfp(fptype)
+
+    @property
+    def forces(self):
+        """ return the all force vectors for all atoms in the molecule """
+        return np.vstack((atom.force_vector for atom in self.atoms))
+
+    @property
+    def all_forces(self):
+        """ the force matrix for all conformer """
+        force_matrix = self._data.get("all_forces")
+        if isinstance(force_matrix, np.ndarray):
+            return force_matrix
+        return self.forces
+
+    @property
+    def formula(self) -> str:
+        return self.ob_mol.GetSpacedFormula()
+
+    def gaussian(
+            self,
+            g16root: Union[str, PathLike],
+            link0: Union[str, List[str]],
+            route: Union[str, List[str]],
+            path_log_file: Union[str, PathLike] = None,
+            path_err_file: Union[str, PathLike] = None,
+            path_chk_file: Union[str, PathLike] = None,
+            path_rwf_file: Union[str, PathLike] = None,
+            inplace_attrs: bool = False,
+            debugger: Union[str, GaussErrorHandle] = 'auto',
+            *args, **kwargs
+    ) -> (Union[None, str], str):
+        """
+        calculation by Gaussian.
+        for running the method normally, MAKE SURE THE Gaussian16 HAVE BEEN INSTALLED AND ALL ENV VAR SET RITHT !!
+        Args:
+            g16root: the dir Gaussian16 software installed
+            link0: the link0 command in gjf script
+            route: the route command in gjf script
+            path_log_file: Optional, the path to save the out.log file. If not given, the logfile would be written
+             to the work dir
+            path_err_file: Optional, the path to save the error log file. If not given, the err file would be written
+             to the work dir
+            path_chk_file: Optional, the path to the checkpoint file. If not given the chk file would be written
+             to the work dir
+            path_rwf_file: Optional, the path to the read-write file. If not given the rwf file would be written
+             to the work dir
+            inplace_attrs: Whether to inplace self attribute according to the results from attributes.
+            debugger: define the method to handle the Gaussian error, like l9999, l103 or l502 ...,
+             the default method is the 'auto', which just to handle some common error case. More elaborate
+             debugger could be handmade by inherit from `GaussErrorHandle` abstract class. For detail, seeing
+             the documentation.
+            *args:
+            **kwargs:
+
+        Returns:
+            the standard output of g16 log file(string), the standard output of g16 err file(string)
+        """
+        # For 2d molecule, build its confomer by universal force field first
+        if not self.has_3d:
+            self.build_3d()
+
+        # Specify the temporary file
+        if not path_chk_file:
+            path_chk_file = Path.cwd().joinpath('checkpoint.chk')
+        else:
+            path_chk_file = Path(path_chk_file)
+
+        if not path_rwf_file:
+            path_rwf_file = Path.cwd().joinpath('readwrite.rwf')
+        else:
+            path_rwf_file = Path(path_rwf_file)
+
+        if isinstance(link0, str):
+            link0 = [link0]
+
+        link0 = link0 + [f'rwf={str(path_rwf_file)}', 'NoSave', f'chk={str(path_chk_file)}']
+
+        # Make the input gjf script
+        script = self.dump('gjf', *args, link0=link0, route=route, **kwargs)
+
+        gauss = Gaussian(g16root)
+        gauss.path_rwf = path_rwf_file
+        gauss.path_chk = path_chk_file
+
+        grun = GaussRun(gauss, debugger)
+        gauss = grun(script)
+
+        if not gauss.stderr:
+            # save the calculate result into the molecule data dict
+            self._data['gaussian_output'] = gauss.stdout
+            self._data['gaussian_parse_data'] = gauss.parse_log()
+
+            # Inplace the self attribute according to the result from gaussian
+            if inplace_attrs:
+                self._set_attrs(**gauss.molecule_setter_dict())
+
+            # Save log file when the path_log_file has been specified
+            if path_log_file:
+                with open(path_log_file, 'w') as writer:
+                    writer.write(gauss.stdout)
+
+            # return results and error info
+            return gauss.stdout, gauss.stderr
+
+        # If got an error message, save the error and stdout file, before raise the error
+        else:
+            # Save error file
+            if not path_err_file:
+                path_err_file = Path(f'{self.formula}.err')
+            with open(path_err_file, 'w') as writer:
+                writer.write(gauss.stderr)
+
+            # Save log file
+            if not path_log_file:
+                path_log_file = Path(f'{self.formula}.log')
+            with open(path_log_file, 'w') as writer:
+                writer.write(gauss.stdout)
+
+            raise GaussianRunError(gauss.stderr)
+
+    def gcmc(
+            self, *guest: 'Molecule', force_field: Union[str, os.PathLike] = None,
+            work_dir: Union[str, os.PathLike] = None, T: float = 298.15, P: float = 1.0, **kwargs
+    ):
+        """
+        Run gcmc to determine the adsorption of guest,
+        Args:
+            self: the framework as the sorbent of guest molecule
+            guest(Molecule): the guest molecule to be adsorbed into the framework
+            force_field(str|PathLike): the path to force field file or the self-existent force file contained
+             in force field directory (in the case, a str should be given as a relative path from the root of
+             force field root to the specified self-existent force filed). By default, the force field is UFF
+             which in the relative path 'UFF/LJ.json' for the force field path.
+            work_dir: the user-specified dir to store the result of GCMC and log file.
+            T: the environmental temperature (default, 298.15 K)
+            P: the relative pressure related to the saturation vapor in the environmental temperature.
+        """
+        from tanks.lmp.gcmc import LjGCMC
+        gcmc = LjGCMC(self, force_field, *guest, work_dir=work_dir, T=T, P=P, **kwargs)
+        return gcmc.run()
+
+    def gcmc_for_isotherm(
+            self, *guest: 'Molecule', force_field: Union[str, os.PathLike] = None,
+            work_dir: Union[str, os.PathLike] = None, T: float = 298.15,
+            Ps: Sequence[float] = (1.0,), **kwargs
+    ):
+        """
+        Run gcmc to determine the adsorption of guest,
+        Args:
+            self: the framework as the sorbent of guest molecule
+            guest(Molecule): the guest molecule to be adsorbed into the framework
+            force_field(str|PathLike): the path to force field file or the self-existent force file contained
+             in force field directory (in the case, a str should be given as a relative path from the root of
+             force field root to the specified self-existent force filed). By default, the force field is UFF
+             which in the relative path 'UFF/LJ.json' for the force field path.
+            work_dir: the user-specified dir to store the result of GCMC and log file.
+            T: the environmental temperature (default, 298.15 K)
+            Ps(Sequence[float]): A sequence of relative pressure related to the saturation vapor in the environmental temperature.
+        """
+        if isinstance(work_dir, str):
+            work_dir = Path(work_dir)
+
+        if not work_dir.exists():
+            work_dir.mkdir()
+
+        for P in Ps:
+            sub_work_dir = work_dir.joinpath('press_' + str(P))
+            if not sub_work_dir.exists():
+                sub_work_dir.mkdir()
+
+            self.gcmc(*guest, force_field=force_field, work_dir=sub_work_dir, T=T, P=P, **kwargs)
+
+    def generate_metal_ligand_pair(
+            self, metal_symbol: str,
+            acceptor_atoms: Sequence = ('O',),
+            opti_force_field: str = 'UFF',
+            opti_before_gen: bool = False,
+            opti_step: int = 500
+    ) -> Generator['Molecule', None, None]:
+        """
+        This method could work if the molecule is an organic ligand, or raise AttributeError.
+        Generate metal-ligand pair by link metal with acceptor atoms in the organic ligand.
+
+        Args:
+            metal_symbol: which metal element link to the ligand
+            acceptor_atoms: which elements to be acceptor atom to link to metal
+            opti_force_field: which force field could be used to optimize the configuration of ligand and M-L pair.
+            opti_before_gen: whether to optimize the ligand conformer before generate pair
+            opti_step: the step to optimize the 3d conformer
+
+        Return:
+            A generator for M-L pair
+        """
+        ligand = self.copy()
+
+        if opti_before_gen:
+            ligand.build_3d(force_field=opti_force_field, steps=opti_step)
+
+        for atom in ligand.atoms:
+            if atom.symbol in acceptor_atoms:
+                # copy the ligand as the embryo of metal-ligand pairs
+                pair = ligand.copy()
+
+                # Replace the correspondent atom in the pair embryo, i.e., the accepting atom
+                acc_atom = pair.atom(atom.ob_id)
+
+                # assign the initial coordinates, if the pair has 3d conformer
+                # the sum of vector of relative position relate to the accepting atom
+                if pair.has_3d:
+                    sum_relative_coordinates = sum([c for _, c in acc_atom.neighbours_position])
+                    metal_init_coordinates = acc_atom.coordinates_array - sum_relative_coordinates
+
+                    # add metal atom into the acceptor_ligand
+                    added_metal = pair.add_atom(metal_symbol, coordinates=metal_init_coordinates)
+
+                else:  # If the pair has not 3d conformer, add the metal directly
+                    added_metal = pair.add_atom(metal_symbol)
+
+                # add the coordinating bond between metal atom and acceptor atoms
+                pair.add_bond(added_metal, acc_atom, 1)
+
+                # localize optimization of M-L pair by classical force field, if the pair has 3d
+                if pair.has_3d:
+                    pair.localed_optimize(opti_force_field)
+                else:
+                    pair.add_hydrogens()  # Add hydrogens
+
+                pair.identifier = pair.smiles
+                yield pair
+
+    def generate_pairs_bundle(
+            self, metal_symbol: str,
+            acceptor_atoms: Sequence = ('O',),
+            opti_force_field: str = 'UFF',
+            opti_before_gen: bool = False,
+            opti_step: int = 500
+    ) -> 'PairBundle':
+        """
+        Generate metal-ligand pairs by bind this ligand with proposed, and put this ligand, metal and all pairs,
+        which are assembled by the ligand and metal, into a PairBundle objects.
+        Args:
+            metal_symbol(str): the symbol of proposed metal
+            acceptor_atoms(Sequence): the atoms to form bond with the proposed metal, the default is Oxygen
+            opti_force_field(str): the force field to optimize the conformer of this ligand and the generated
+             pairs.
+            opti_before_gen: whether to optimize the ligand conformer before generate pair.
+            opti_step: the step to optimize the 3d conformer
+
+        Returns:
+            PairBundle with this ligand, proposed metal and the pairs
+        """
+        return PairBundle(
+            metal=Atom(symbol=metal_symbol),
+            ligand=self,
+            pairs=list(self.generate_metal_ligand_pair(
+                metal_symbol,
+                acceptor_atoms,
+                opti_force_field,
+                opti_before_gen
+            )),
+        )
+
+    def graph_representation(self, *feature_names):
+        return self.identifier, self.feature_matrix(*feature_names), self.link_matrix
+
+    def heavy_atoms(self):
+        """ Get the atoms except for hydrogens """
+        return [a for a in self.atoms if a.is_heavy]
+
+    @property
+    def has_3d(self):
+        """ Whether atoms in the molecule have 3d coordinates """
+        return self.ob_mol.Has3D()
+
+    @property
+    def has_hydrogen_added(self):
+        """ Have hydrogens been added to the molecule by call Molecule.add_hydrogen()? """
+        return self.ob_mol.HasHydrogensAdded()
+
+    @property
+    def has_unknown_bond(self):
+        return any(not b.type for b in self.bonds)
+
+    @property
+    def hydrogens(self):
+        return [a for a in self.atoms if a.is_hydrogen]
+
+    @property
+    def identifier(self):
+        return self.ob_mol.GetTitle()
+
+    @identifier.setter
+    def identifier(self, value):
+        self.ob_mol.SetTitle(value)
+
+    @property
+    def identifier_array(self) -> np.ndarray:
+        """ numpy.array of identifiers has the same number of items with the number of conformers """
+        idt_array = self._data.get('identifier_array')
+        if not isinstance(idt_array, np.ndarray):
+            idt_array = []
+            for i, c in enumerate(self.all_coordinates):
+                idt_array.append(f'{self.identifier}_c{i}')
+            self._data['identifier_array'] = idt_array = np.array(idt_array)
+
+        return idt_array
+
+    def iadd_accessible(self, other):
+        if self.atomic_numbers == other.atomic_numbers:
+            return True
+        return False
+
+    @property
+    def inchi(self):
+        return self.dump('inchi').strip()
+
+    @property
+    def is_disorder(self):
+        """ To judge whether this Molecule has disorder bonds """
+        if self.has_3d:
+            if any(not (0.85 < b.length/b.ideal_length < 1.15) for b in self.bonds):
+                return True
+        return False
+
+    @property
+    def is_labels_unique(self):
+        """ Determine whether all atom labels are unique """
+        return len(set(self.labels)) == self.atom_counts
+
+    @property
+    def is_organic(self):
+        """ To judge whether the molecule is organic, an organic compound is with carbon atoms and without metal """
+        if any(a.is_metal for a in self.atoms):
+            return False
+        elif any(a.symbol == 'C' for a in self.atoms):
+            return True
+
+        return False
+
+    def ob_copy(self):
+        """ Return a clone of OBMol of the Molecule """
+        return ob.OBMol(self.ob_mol)
+
+    @property
+    def ob_mol(self):
+        return self._data['ob_obj']
+
+    def ob_mol_pop(self):
+        data: dict = self._data
+
+        atoms: Dict[int, Atom] = data.get('atoms')
+        if atoms:
+            for ob_id, atom in atoms.items():
+                atom.ob_atom_pop()
+
+        bonds: Dict[int, Bond] = data.get('bonds')
+        if bonds:
+            for ob_idx, bond in bonds.items():
+                bond.ob_bond_pop()
+
+        return self._data.pop('ob_obj')
+
+    def ob_mol_rewrap(self, ob_mol: ob.OBMol):
+        if not isinstance(ob_mol, ob.OBMol):
+            raise TypeError('the ob_mol should be OBMol object')
+
+        atoms = self._data.get('atoms')
+        bonds = self._data.get('bonds')
+
+        if any(oba.GetId() not in atoms for oba in ob.OBMolAtomIter(ob_mol)):
+            raise ValueError('the atom number between the wrapper and the core OBMol is not match')
+        if any(obb.GetId() not in bonds for obb in ob.OBMolBondIter(ob_mol)):
+            raise ValueError('the bond number between the wrapper and the core OBMol is not match')
+
+        self._data['ob_obj'] = ob_mol
+        for ob_atom in ob.OBMolAtomIter(ob_mol):
+            atom = atoms.get(ob_atom.GetId())
+            atom.ob_atom_rewrap(ob_atom)
+
+        for ob_bond in ob.OBMolBondIter(ob_mol):
+            bond = bonds.get(ob_bond.GetId())
+            bond.ob_bond_rewrap(ob_bond)
+
+    @property
+    def labels(self):
+        return [a.label for a in self.atoms]
+
+    @property
+    def lmp(self):
+        """ handle to operate the Lammps object """
+        return self._data.get('lmp')
+
+    def lmp_close(self):
+        pop_lmp = self._data.pop('lmp')
+        pop_lmp.close()
+
+    def lmp_setup(self, **kwargs):
+        self._data['lmp'] = lmp.HpLammps(self, **kwargs)
+
+    @property
+    def link_matrix(self):
+        return np.array([[b.ob_atom1_id, b.ob_atom2_id] for b in self.bonds]).T
+
+    def localed_optimize(self, force_field: str = 'UFF', steps: int = 500):
+        """ Locally optimize the coordinates. seeing openbabel.pybel package """
+        pymol = pb.Molecule(self.ob_mol)
+        pymol.localopt(force_field, steps)
+        self.balance_hydrogens()
+
+    def make_crystal(self, a: float, b: float, c: float, alpha: float, beta: float, gamma: float) -> 'Crystal':
+        """ Put this molecule into the specified crystal """
+        ob_unit_cell = ob.OBUnitCell()
+
+        self.ob_mol.CloneData(ob_unit_cell)
+        self.crystal().ob_unit_cell.SetData(a, b, c, alpha, beta, gamma)
+        self.crystal().ob_unit_cell.SetSpaceGroup('P1')
+
+        return self.crystal()
+
+    @property
+    def masses(self) -> np.ndarray:
+        return np.array([a.mass for a in self.atoms])
+
+    def melt_quench(
+            self, elements: Dict[str, float], force_field: Union[str, os.PathLike],
+            density: float = 1.0, a: float = 25., b: float = 25., c: float = 25.,
+            alpha: float = 90., beta: float = 90., gamma: float = 90., time_step: float = 0.0001,
+            origin_temp: float = 298.15, melt_temp: float = 4000., highest_temp: float = 10000.,
+            ff_args: Sequence = (), path_writefile: Optional[str] = None, path_dump_to: Optional[str] = None,
+            dump_every: int = 100
+    ):
+        """
+        Create an Amorphous crystal materials by performing Melt-Quench process for this materials.
+        This process is performed by LAMMPS package, make sure the LAMMPS is accessible.
+        A suitable force field is required for the process are performed correctly.
+        Args:
+            elements(dict[str, float]): Dict of elements and their composition ratio
+            force_field(str, os.PathLike): The name of force filed or the path to load a force filed. The name
+             of the force filed is refer to the relative path to the 'hotpot_root/data/force_field'.
+            density: the demand density for the created amorphous crystal
+            a: the length of a vector in the crystal
+            b: the length of b vector in the crystal
+            c: the length of c vector in the crystal
+            alpha: alpha angle of crystal param.
+            beta: beta angle of crystal param.
+            gamma: gamma angle of crystal param
+            time_step: time interval between path integrals when performing melt-quench
+            origin_temp: the initial temperature before melt
+            melt_temp: the round melting point to the materials
+            highest_temp: the highest temperature to liquefy the materials
+            ff_args: the arguments the force file requried, refering the LAMMPS pair_coeff:
+             "pair_coeff I J args" url: https://docs.lammps.org/pair_coeff.html
+            path_writefile: the path to write the final material (screenshot) to file, if not specify, not save.
+            path_dump_to:  the path to save the trajectory of the melt-quench process, if not specify not save.
+            dump_every: the step interval between each dump operations
+
+        Returns:
+            Molecule, a created amorphous material
+        """
+        return self._melt_quench(
+            elements=elements, force_field=force_field, density=density,
+            a=a, b=b, c=c, alpha=alpha, beta=beta, gamma=gamma, time_step=time_step,
+            origin_temp=origin_temp, melt_temp=melt_temp, highest_temp=highest_temp,
+            ff_args=ff_args, path_writefile=path_writefile, path_dump_to=path_dump_to,
+            dump_every=dump_every, mol=self
+        )
+
+    @property
+    def metals(self) -> List['Atom']:
+        return [a for a in self.atoms if a.is_metal]
+
+    @property
+    def mol_orbital_energies(self):
+        energies = self._data.get('mol_orbital_energies')
+        if energies:
+            return energies
+        else:
+            return None
+
+    def normalize_labels(self):
+        """ Reorder the atoms labels in the molecule """
+        element_counts = {}
+        for atom in self.atoms:
+            count = element_counts.get(atom.symbol, 0)
+            count += 1
+            element_counts[atom.symbol] = count
+            atom.label = f'{atom.symbol}{count}'
+
+    def perturb_atoms_coordinates(
+            self,
+            random_style='uniform',
+            mol_distance=0.5,
+            freeze_dim: Sequence[int] = (),
+            max_generate_num: int = 10,
+            inplace: bool = False
+    ) -> Generator["Molecule", None, None]:
+        """
+        Perturb the coordinate of atom in the molecule
+        generate new mol
+        Args:
+            random_style: how to sample, 'uniform' or 'normal'
+            mol_distance: the max distance of perturbation in 'uniform'; the square variance in 'normal'
+            freeze_dim: tuple of int or str, 0 = x, 1 = y, 2 = z
+            max_generate_num: the maximum of generated molecule
+            inplace
+
+        Returns:
+            Generator of perturbed molecule
+        """
+        dim_transform = {'x': 0, 'y': 1, 'z': 2}
+
+        coordinates_shape = (self.atom_counts, 3)  # the shape of coordinates matrix (atom counts, 3 dimension)
+        origin_coordinates = self.coordinates
+
+        def coordinates_generator():
+            """ Generating """
+            for _ in range(max_generate_num):
+                if random_style == 'uniform':
+                    perturb_matrix = np.float64(np.random.uniform(-mol_distance, mol_distance, coordinates_shape))
+                elif random_style == 'normal':
+                    perturb_matrix = np.float64(np.random.normal(0, mol_distance, coordinates_shape))
+                else:
+                    raise ValueError('the perturb style is not defined!')
+
+                if freeze_dim:
+                    dim = [
+                        i if (isinstance(i, int) and 0 <= i <= 3) else dim_transform[i]
+                        for i in freeze_dim
+                    ]
+
+                    perturb_matrix[:, dim] = 0.
+
+                new_coord = origin_coordinates + perturb_matrix
+
+                yield new_coord
+
+        if inplace:
+            origin_all_coordinates = self._data.get('all_coordinates')
+            new_all_coordinates = np.array([c for c in coordinates_generator()])
+
+            if origin_all_coordinates is not None:
+                self._data['all_coordinates'] = np.concatenate([origin_all_coordinates, new_all_coordinates])
+            else:
+                self._data['all_coordinates'] = np.concatenate(
+                    [np.reshape(origin_coordinates, (1,) + origin_coordinates.shape), new_all_coordinates]
+                )
+
+        else:
+            return (self._pert_mol_generate(c) for c in coordinates_generator())
+
+    def perturb_cell_params(self):
+        """ To perturb parameters, i.e., a, b, c, alpha, beta, gamma """
+
+    @property
+    def pseudo_atoms(self):
+        return self._data.get('pseudo_atoms', [])
+
+    def quick_build_atoms(self, atomic_numbers: np.ndarray):
+        """
+        This method to quick build atoms according an array of atomic numbers.
+        The method bypass to calling more time-consumed method: add_atom().
+        However, the method only assign the elements or atomic number for atoms,
+        more fine attributes like coordinates, can't be specified.
+        Args:
+            atomic_numbers(np.ndarray): 1-D numpy array to add new atoms into the molecule
+
+        Returns:
+            None
+        """
+        if not isinstance(atomic_numbers, (np.ndarray, Sequence)):
+            raise TypeError('the atomic_numbers should be np.ndarray or Sequence')
+        if isinstance(atomic_numbers, np.ndarray) and len(atomic_numbers.shape) != 1:
+            raise ValueError('the numpy array must be 1-D')
+
+        for atomic_number in atomic_numbers:
+            ob_atom = ob.OBAtom()
+            ob_atom.SetAtomicNum(int(atomic_number))
+            self.ob_mol.AddAtom(ob_atom)
+
+    @classmethod
+    def read_from(cls, source: Union[str, PathLike, IOBase], fmt=None, *args, **kwargs) -> 'Molecule':
+        """
+        read source to the Molecule obj by call _io.Parser class
+        Args:
+            source(str, PathLike, IOBase): the formatted source
+            fmt:
+            *args:
+            **kwargs:
+
+        Returns:
+
+        """
+        if not fmt:
+            if isinstance(source, str):
+                source = Path(source)
+
+            if isinstance(source, Path):
+                fmt = source.suffix.strip('.')
+            else:
+                raise ValueError(f'the arguments should be specified for {type(source)} source')
+
+        mol = Parser(fmt, source, *args, **kwargs)()  # initialize parser object and call self
+
+        # Specify the mol identifier if it's None
+        if isinstance(mol, Molecule) and not mol.identifier:
+            mol.identifier = str(source)
+
+        return mol
+
+    def register_critical_params(self, name: str, temperature: float, pressure: float, acentric: float):
+        """ Register new critical parameters into the critical parameters sheet """
+        data = json.load(open(opj(data_root, 'thermo', 'critical.json')))
+        data[self.smiles] = {'name': name, 'temperature': temperature, 'pressure': pressure, 'acentric': acentric}
+        with open(opj(data_root, 'thermo', 'critical.json'), 'w') as writer:
+            json.dump(data, writer, indent=True)
+
+    def remove_atoms(self, *atoms: Union[int, str, 'Atom'], remove_hydrogens: bool = False) -> None:
+        """
+        Remove atom according to given atom index, label or the atoms self.
+        Args:
+            atoms(int|str|Atom): the index, label or self of Removed atom
+            remove_hydrogens(bool): remove the hydrogens connecting in the atoms synchronously.
+
+        Returns:
+            None
+        """
+        for atom in atoms:
+
+            # Check and locate the atom
+            if isinstance(atom, int):
+                atom = self.atoms_dict[atom]
+            elif isinstance(atom, str):
+                atom = self.atom(atom)
+            elif isinstance(atom, Atom):
+                if not (atom.molecule is self):
+                    raise AttributeError('the given atom not in the molecule')
+            else:
+                raise TypeError('the given atom should be int, str or Atom')
+
+            # remove connecting hydrogens
+            if remove_hydrogens:
+                for nh in atom.neighbours_hydrogen:
+                    self.ob_mol.DeleteAtom(nh.ob_atom)
+
+            # Removing the atom
+            self.ob_mol.DeleteAtom(atom.ob_atom)
+            atom._data['mol'] = None
+
+        # Reload atoms
+        self._load_atoms()
+        self._load_bonds()
+
+    def remove_bonds(self, *bonds: 'Bond'):
+        """ Remove the bonds in the molecule """
+        for bond in bonds:
+            successful = self.ob_mol.DeleteBond(bond.ob_bond)
+            if not successful:
+                raise RuntimeError(f'Fail to remove {bonds}')
+
+        self._load_bonds()
+
+    def remove_hydrogens(self):
+        self.ob_mol.DeleteHydrogens()
+
+    def remove_metals(self):
+        """ remove all of metal atoms in the molecule """
+        self.remove_atoms(*self.metals)
+
+    def remove_solvents(self, remove_disorder: bool = True, remove_isolate_atoms: bool = True):
+        """ remove all solvents in the molecule """
+        self.normalize_labels()
+        for i, ligand in enumerate(self.retrieve_ligands()):
+            if remove_disorder and ligand.is_disorder:  # remove disorder molecular structures first
+                self.remove_atoms(*ligand.atom_labels, remove_hydrogens=False)
+            elif remove_isolate_atoms and len(ligand.atoms) == 1:
+                self.remove_atoms(*ligand.atom_labels, remove_hydrogens=False)
+            elif _lib.get('Solvents').is_solvent(ligand):  # To judge if the ligand is solvents
+                self.remove_atoms(*ligand.atom_labels, remove_hydrogens=False)
+
+    def retrieve_ligands(self) -> List['Molecule']:
+        """ Retrieve all ligand molecule from this """
+        clone = self.copy()
+        clone.remove_metals()
+
+        return clone.components
+
+    def retrieve_metal_ligand_pairs(self) -> List['Molecule']:
+        """ Retrieve all clone of metal-ligand pairs in the molecule """
+        if not self.is_labels_unique:
+            self.normalize_labels()
+
+        ml_pairs = []
+        for metal, ligand in product(self.metals, self.retrieve_ligands()):
+            if set(metal.neighbours_label) & set(ligand.atom_labels):
+                pair = self.copy()
+
+                # Remove all the atoms is not the metal and not on the ligand
+                other_atoms = [a for a in pair.atoms if a.label != metal.label and a.label not in ligand.atom_labels]
+                pair.remove_atoms(*other_atoms, remove_hydrogens=False)
+
+                ml_pairs.append(pair)
+
+        return ml_pairs
+
+    @property
+    def rotatable_bonds_number(self):
+        return self.ob_mol.NumRotors()
+
+    def save_2d_img(self, file_path: Union[str, os.PathLike], **kwargs):
+        """
+        Export 2d image to file
+        Args:
+            file_path:
+            **kwargs: other keywords arguments for 2d image make and save
+
+        Keyword Args:
+
+        """
+        img = self.to_2d_img(**kwargs)
+        img.save(file_path)
+
+    def set(self, **kwargs):
+        """ Set the attributes directly """
+        self._set_attrs(**kwargs)
+
+    def set_label(self, ob_id: int, label: str):
+        self.atoms_dict[ob_id].label = label
+
+    def similarity(self, other: 'Molecule', fptype: Literal['FP2', 'FP3', 'FP4', 'MACCS'] = 'FP2') -> int:
+        """
+        Compare the similarity with other molecule, based on specified fingerprint
+        Args:
+            other(Molecule): the other Molecule
+            fptype(str): the fingerprint type to perform comparison of similarity
+
+        Return:
+            the similarity(int)
+        """
+        return self.fingerprint(fptype) | other.fingerprint(fptype)
+
+    def smarts(self):
+        """ Get the SMARTS string """
+        return Chem.MolToSmarts(self.to_rdmol())
+
+    @property
+    def smiles(self):
+        """ Get the canonical smiles """
+        return self.dump('can').split()[0]
+
+    @property
+    def spin(self):
+        return self.ob_mol.GetTotalSpinMultiplicity()
+
+    @spin.setter
+    def spin(self, spin: int):
+        self._set_spin_multiplicity(spin)
+
+    def thermo_init(self, **kwargs):
+        """
+        If certain substance don't retrieve information from current database, some required thermodynamical
+        parameters should pass into equation_of_state to initialization
+        Keyword Args:
+            T: the ambient temperature for thermodynamical system
+            P: the ambient pressure for thermodynamical system
+            V: the volume of thermodynamical system
+            Tc: the critical temperature of the molecule
+            Pc: the critical pressure of the molecule
+            omega: acentric factor of the molecule
+
+        Returns:
+            Thermo class
+        """
+        from tmo import Thermo
+        self._data['thermo'] = Thermo(self, **kwargs)
+        return self._data['thermo']
+
+    @property
+    def thermo(self):
+        return self._data.get('thermo')
+
+    def thermo_close(self):
+        _ = self._data.pop('thermo')
+        del _
+
+    @property
+    def torsions(self):
+        return [Torsion(self, *obi) for obi in ob.OBMolTorsionIter(self.ob_mol)]
+
+    def to_2d_img(self, **kwargs):
+        """
+        Get a 2D image objects for the molecule
+        Keyword Args:
+            kekulize: whether to applying Kekulize style to aromatical rings
+
+        Returns:
+
+        """
+        clone = self.copy()
+        clone.build_2d()
+        return Draw.MolToImage(clone.to_rdmol(), **kwargs)
+
+    def to_dpmd_sys(
+            self, system_dir: Union[str, os.PathLike],
+            mode: Literal['std', 'att'] = 'std',
+            validate_ratio: float = None,
+            validate_dir: Union[str, Path] = None
+    ):
+        """
+        convert to DeePMD-Kit System, there are two system mode, that `standard` (std) and `attention` (att)
+            1) standard: https://docs.deepmodeling.com/projects/deepmd/en/master/data/system.html
+            2) attention: https://docs.deepmodeling.com/projects/deepmd/en/master/model/train-se-atten.html#data-format
+
+        Args:
+            system_dir: the dir for all system data store, if the validate_dir has been given, this is the dir of
+             training system
+            mode: the system mode, choose from att or std
+            validate_ratio(float): the ratio of validate data set.
+            validate_dir(str|Path): if validate_ratio has been specified, this must be given
+        """
+        system: DeepSystem = self.dump('dpmd_sys')
+        system(system_dir, mode, validate_ratio, validate_dir)
+
+    def to_mix_mol(self):
+        """ Convert this Molecule object to MixSaveAtomMol """
+        return MixSameAtomMol(_data=self._data)
+
+    def to_rdmol(self):
+        """ convert hotpot Molecule object to RdKit mol object """
+        return Chem.MolFromMol2Block(self.dump('mol2'))
+
+    @property
+    def unique_all_atoms(self) -> List[Union['Atom', 'PseudoAtom']]:
+        return self.unique_atoms + self.unique_pseudo_atoms
+
+    @property
+    def unique_atoms(self):
+        uni = []
+        for a in self.atoms:
+            if a not in uni:
+                uni.append(a)
+        return uni
+
+    @property
+    def unique_bonds(self):
+        uni = []
+        for b in self.bonds:
+            if b not in uni:
+                uni.append(b)
+        return uni
+
+    @property
+    def unique_bond_pairs(self) -> List[Tuple[int, int, int]]:
+        """ Retrieve unique bond pair in the molecule, i.e. a bond with same atoms element combination and bond type """
+        return [b.pair_key for b in self.unique_bonds]
+
+    @property
+    def unique_pseudo_atoms(self) -> List['PseudoAtom']:
+        uni = []
+        for pa in self.pseudo_atoms:
+            if pa not in uni:
+                uni.append(pa)
+        return uni
+
+    @property
+    def weight(self):
+        return self.ob_mol.GetExactMass()
+
+    def writefile(self, fmt: str, path_file, retrieve_script=False, *args, **kwargs):
+        """Write the Molecule Info into a file with specific format(fmt)"""
+        script = self.dump(fmt=fmt, *args, **kwargs)
+        if isinstance(script, str):
+            mode = 'w'
+        elif isinstance(script, bytes):
+            mode = 'wb'
+        else:
+            raise IOError(f'the {type(script)} type for script is not supported to write into file')
+
+        with open(path_file, mode) as writer:
+            writer.write(script)
+
+        if retrieve_script:
+            return script
+
+    @property
+    def xyz_min(self) -> np.ndarray:
+        """ Return the minimum of x coordinates wreathing all atoms """
+        return self.coordinates.min(axis=0)
+
+    @property
+    def xyz_max(self) -> np.ndarray:
+        return self.coordinates.max(axis=0)
+
+    @property
+    def xyz_diff(self):
+        return self.xyz_max - self.xyz_min
+
+    @property
+    def z_matrix(self) -> 'ZMatrix':
+        return ZMatrix(self)
+
+
+class MixSameAtomMol(Molecule):
+    """ the only difference to the Molecule class is the method of their addition  """
+
+    def __repr__(self):
+        return f'MixMol({self.formula})'
+
+    def _merge_conformer_attr(self, other: 'Molecule'):
+        """"""
+        # merge the MixSameAtomMol-specific conformer attributes
+        left_atomic_numbers: Dict[Tuple[int], int] = self.atomic_numbers
+        right_atomic_numbers: Union[Dict[Tuple[int], int], Tuple[int]] = other.atomic_numbers
+
+        # If the right atomic_number is a tuple convert it to dict.
+        if isinstance(right_atomic_numbers, tuple):
+            right_atomic_numbers = {right_atomic_numbers: other.conformer_counts}
+
+        for atomic_numbers, conformer_counts in right_atomic_numbers.items():
+            left_atomic_numbers[atomic_numbers] = left_atomic_numbers.get(atomic_numbers, 0) + conformer_counts
+
+        self._set_atomic_numbers(left_atomic_numbers)
+
+        # ##### the super method ######
+        # Merge the basic conformer attributes
+        super(MixSameAtomMol, self)._merge_conformer_attr(other)
+
+        return self
+
+    def _set_atomic_numbers(self, atomic_numbers: Dict[Tuple[int], int]):
+        """ Set all atoms' atomic numbers and their corresponding number of conformers """
+        self.update_attr_data({'atomic_numbers': atomic_numbers})
+
+    @property
+    def atomic_numbers(self) -> Dict[Tuple[int], int]:
+        """ get each conformer atomic numbers """
+        atomic_numbers = self.data.get('atomic_numbers')
+        if not atomic_numbers:
+            atomic_numbers = {super(MixSameAtomMol, self).atomic_numbers: self.conformer_counts}
+            self._set_atomic_numbers(atomic_numbers)
+
+        return atomic_numbers
+
+    @property
+    def atomic_number_counts(self):
+        """ the counts of series of atomic_numbers """
+        return len(self.atomic_numbers)
+
+    @property
+    def atomic_numbers_array(self) -> np.ndarray:
+        """ the conformer corresponding attributes with array shape (counts_of_atoms, counts_of_conformers) """
+        atomic_numbers_array = []
+        for atomic_numbers, conformer_counts in self.atomic_numbers.items():
+            atomic_numbers_array.append(np.array(atomic_numbers).reshape(1, -1).repeat(conformer_counts, axis=0))
+
+        return np.concatenate(atomic_numbers_array)
+
+    def iadd_accessible(self, other):
+        if self.atom_counts == other.atom_counts:
+            return True
+        return False
+
+    def to_mol(self):
+        """ Convert this MixSameAtomMol object to Molecule """
+        if self.atomic_number_counts > 1:
+            raise AttributeError(
+                'Cannot convert the MixSameAtomMol with multipy atomic_number series to Molecule object\n'
+                f'atomic_number_counts = {self.atomic_number_counts}'
+            )
+
+        return Molecule(_data=self.data)
+
+
+class Atom(Wrapper, ABC):
+    """ The Atom wrapper for OBAtom class in openbabel """
+
+    def __init__(
+            self,
+            ob_atom: ob.OBAtom = None,
+            **kwargs
+    ):
+        # Contain all data to reappear this Atom
+        self._data: Dict[str, Any] = {
+            'ob_obj': ob_atom if ob_atom else ob.OBAtom(),
+        }
+
+        self._set_attrs(**kwargs)
+
+    def __eq__(self, other):
+        if isinstance(other, Atom):
+            return self.ob_atom == other.ob_atom
+
+    def __hash__(self):
+        return hash(f'Atom({self.atomic_number})')
+
+    @property
+    def ob_atom(self):
+        return self._data['ob_obj']
+
+    @ob_atom.setter
+    def ob_atom(self, oba):
+        self._data['ob_obj'] = oba
+
+    def ob_atom_pop(self):
+        return self._data.pop('ob_obj')
+
+    def ob_atom_rewrap(self, ob_atom):
+        self._data['ob_obj'] = ob_atom
+
+    def __repr__(self):
+        return f"Atom({self.label if self.label else self.symbol})"
+
+    def _assign_formal_charge(self):
+        """ assign formal charge for this atom, the formal charge equal its valence minus its covalent valence """
+        if self.is_polar_hydrogen:
+            self.formal_charge = 1
+        elif self.is_hydrogen or self.is_carbon:
+            self.formal_charge = 0
+        elif self.is_metal:
+            self.formal_charge = _stable_charges[self.symbol]
+        else:
+            self.formal_charge = -len([a for a in self.neighbours if a.is_polar_hydrogen])
+
+    @property
+    def _attr_setters(self) -> Dict[str, Callable]:
+        return {
+            '_mol': self._set_molecule,
+            'mol': self._set_molecule,
+            'molecule': self._set_molecule,
+            'atomic_number': self._set_atomic_number,
+            'symbol': self._set_atomic_symbol,
+            'coordinates': self._set_coordinate,
+            'formal_charge': self._set_formal_charge,
+            'partial_charge': self._set_partial_charge,
+            'label': self._set_label,
+            'ob_id': self._set_ob_id,
+            'spin_density': self._set_spin_density
+        }
+
+    def _set_atomic_number(self, atomic_number: int):
+        self.ob_atom.SetAtomicNum(int(atomic_number))
+
+    def _set_atomic_symbol(self, symbol):
+        self.ob_atom.SetAtomicNum(ob.GetAtomicNum(symbol))
+
+    def _set_coordinate(self, coordinates):
+        self.ob_atom.SetVector(*coordinates)
+
+    def _set_force_vector(self, force_vector: Union[Sequence, np.ndarray]):
+        if isinstance(force_vector, Sequence):
+            if all(isinstance(f, float) for f in force_vector):
+                force_vector = np.array(force_vector)
+            else:
+                ValueError('the give force_vector must float vector with dimension 3')
+        elif isinstance(force_vector, np.ndarray):
+            force_vector = force_vector.flatten()
+        else:
+            raise TypeError('the force vector should be Sequence or np.ndarray')
+
+        self._data['force_vector'] = force_vector
+
+    def _set_formal_charge(self, charge: float):
+        self.ob_atom.SetFormalCharge(charge)
+
+    def _set_ob_id(self, ob_id):
+        self.ob_atom.SetId(ob_id)
+
+    def _set_label(self, label):
+        label_data = ob.OBCommentData()
+
+        label_data.SetAttribute('label')
+        label_data.SetData(label)
+
+        self.ob_atom.CloneData(label_data)
+
+    def _set_molecule(self, molecule: Molecule):
+        self._data['mol'] = molecule
+
+    def _set_partial_charge(self, charge):
+        self.ob_atom.SetPartialCharge(charge)
+
+    def _set_spin_density(self, spin_density: float):
+        self._data['spin_density'] = spin_density
+
+    @property
+    def atom_type(self):
+        """ Some atom have specific type, such as Carbon with sp1, sp2 and sp3, marked as C1, C2 and C3 """
+        return self.ob_atom.GetType()
+
+    def add_atom(self, symbol: str, bond_type=1, **atom_attrs):
+        """ add atom to link with this atom """
+        new_atom = self.molecule.add_atom(symbol, **atom_attrs)
+        self.molecule.add_bond(self, new_atom, bond_type)
+
+    def add_hydrogen(self):
+        """ add hydrogen to the atom """
+        self.add_atom('H')
+
+    @property
+    def atomic_number(self):
+        return self.ob_atom.GetAtomicNum()
+
+    def balance_hydrogen(self):
+        """ Remove or add hydrogens link with this atom, if the bond valence is not equal to the atomic valence """
+        if self.is_heavy and not self.is_metal:  # Do not add or remove hydrogens to the metal, H or inert elements
+            while self.valence > self.stable_valence and self.neighbours_hydrogen:
+                self.molecule.remove_atoms(self.neighbours_hydrogen[0])
+
+            # add hydrogen, if the bond valence less than the atomic valence
+            while self.valence < self.stable_valence:
+                self.add_hydrogen()
+
+    @property
+    def bonds(self):
+        """ Get all bonds link with the atoms """
+        return [self.molecule.bonds_dict[obb.GetId()] for obb in ob.OBAtomBondIter(self.ob_atom)]
+
+    @property
+    def coordinates(self) -> (float, float, float):
+        return self.ob_atom.GetX(), self.ob_atom.GetY(), self.ob_atom.GetZ()
+
+    @coordinates.setter
+    def coordinates(self, value):
+        self._set_coordinate(value)
+
+    @property
+    def coordinates_array(self) -> np.ndarray:
+        """ the array of coordinates """
+        return np.array(self.coordinates)
+
+    def copy(self):
+        """ Make a copy of self """
+        # Extract old data
+        data = self.data
+        data.pop('ob_obj')  # Remove the old OBAtom
+        # Remove molecule if the parent atom in a molecule
+        if self.molecule:
+            data.pop('mol')
+
+        # Copy the information contained in OBAtom
+        new_attrs = {
+            "atomic_number": self.atomic_number,
+            "coordinates": self.coordinates,
+            'partial_charge': self.partial_charge,
+        }
+
+        new_attrs.update(**data)
+
+        return Atom(**new_attrs)
+
+    @property
+    def covalent_valence(self):
+        """ the number of covalent electrons for this atoms """
+        return sum(b.type if b.is_covalent else 0 for b in self.bonds)
+
+    def element_features(self, *feature_names) -> np.ndarray:
+        """ Retrieve the feature vector """
+        atom_feature = periodic_table[self.symbol]
+
+        features = []
+        for feature_name in feature_names:
+            if feature_name == 'atomic_orbital':
+                features.extend(self._atomic_orbital_feature().values())
+            elif feature_name == 'atomic_number':
+                features.append(self.atomic_number)
+            else:
+                features.append(atom_feature[feature_name])
+
+        return np.array(features)
+
+    def _atomic_orbital_feature(self, outermost_layer=True, nonexistent_orbit=0):
+        """    Calculating the feature about atomic orbital structures    """
+        _atomic_orbital_structure_max = {
+            "1s": 2,
+            "2s": 2, "2p": 6,
+            "3s": 2, "3p": 6,
+            "4s": 2, "3d": 10, "4p": 6,
+            "5s": 2, "4d": 10, "5p": 6,
+            "6s": 2, "4f": 14, "5d": 10, "6p": 6,
+            "7s": 2, "5f": 14, "6d": 10, "7p": 6
+        }
+        atomic_orbital_structure = {
+            "1s": 0,
+            "2s": 0, "2p": 0,
+            "3s": 0, "3p": 0,
+            "4s": 0, "3d": 0, "4p": 0,
+            "5s": 0, "4d": 0, "5p": 0,
+            "6s": 0, "4f": 0, "5d": 0, "6p": 0,
+            "7s": 0, "5f": 0, "6d": 0, "7p": 0
+        }
+
+        # Calculating atomic orbital structure
+        residual_electron = self.atomic_number
+        n_osl = 0  # Principal qm number (n) of open shell layers (osl)
+        for orbital_name, men in _atomic_orbital_structure_max.items():  # max electron number (men)
+
+            # Update Principal qm number (n)
+            if orbital_name[1] == "s":
+                n_osl = int(orbital_name[0])
+
+            # Filled atomic orbital
+            if residual_electron - men >= 0:
+                residual_electron = residual_electron - men
+                atomic_orbital_structure[orbital_name] = men
+            else:
+                atomic_orbital_structure[orbital_name] = residual_electron
+                break
+
+        # Readout and return outermost electron structure
+        atom_orbital_feature = {"atomic_number": self.atomic_number, "n_osl": n_osl}
+        if outermost_layer:
+            diff_max_n = {"s": 0, "p": 0, "d": -1, "f": -2}
+            for layer, diff in diff_max_n.items():  # Angular momentum qm number (l)
+                electron_number = atomic_orbital_structure.get(f"{n_osl + diff}{layer}", nonexistent_orbit)
+                atom_orbital_feature[layer] = electron_number
+        else:
+            atom_orbital_feature.update(atomic_orbital_structure)
+
+        # return whole electron structure directly
+        return atom_orbital_feature
+
+    @property
+    def force_vector(self):
+        return self._data.get('force_vector', np.zeros(3, dtype=float))
+
+    @force_vector.setter
+    def force_vector(self, force_vector: Union[Sequence, np.ndarray]):
+        self._set_force_vector(force_vector)
+
+    @property
+    def formal_charge(self) -> float:
+        return self.ob_atom.GetFormalCharge()
+
+    @formal_charge.setter
+    def formal_charge(self, value: float):
+        self.ob_atom.SetFormalCharge(value)
+
+    @property
+    def has_unknown_bond(self) -> bool:
+        return any(not b.type for b in self.bonds)
+
+    @property
+    def hybridization(self):
+        """ The hybridization of this atom:
+        1 for sp, 2 for sp2, 3 for sp3, 4 for sq. planar, 5 for trig. bipy, 6 for octahedral """
+        return self.ob_atom.GetHyb()
+
+    @property
+    def kwargs_attributes(self):
+        return tuple(self._attr_setters.keys())
+
+    @property
+    def ob_id(self):
+        return self.ob_atom.GetId()
+
+    @property
+    def ob_idx(self):
+        return self.ob_atom.GetIdx()
+
+    @property
+    def is_aromatic(self):
+        return self.ob_atom.IsAromatic()
+
+    @property
+    def is_carbon(self):
+        return self.atomic_number == 6
+
+    @property
+    def is_chiral(self):
+        return self.ob_atom.IsChiral()
+
+    @property
+    def is_hydrogen(self):
+        return self.ob_atom.GetAtomicNum() == 1
+
+    @property
+    def is_heavy(self):
+        """ Whether the atom is heavy atom """
+        return not self.is_hydrogen
+
+    @property
+    def is_polar_hydrogen(self) -> bool:
+        """ Is this atom a hydrogen connected to a polar atom """
+        return self.ob_atom.IsPolarHydrogen()
+
+    @property
+    def is_metal(self):
+        return self.ob_atom.IsMetal()
+
+    @property
+    def label(self):
+        label_data = self.ob_atom.GetData('label')
+
+        if label_data:
+            label_data = ob.toCommentData(label_data)
+            return label_data.GetValue()
+        else:
+            return self.symbol
+
+    @label.setter
+    def label(self, value):
+        self._set_label(value)
+
+    @property
+    def link_degree(self) -> int:
+        """ the degree of the atom in their parent molecule """
+        return self.ob_atom.GetTotalDegree()
+
+    @property
+    def mass(self):
+        return self.ob_atom.GetAtomicMass()
+
+    @property
+    def max_bonds(self):
+        """ the max allowed bond order"""
+        return ob.GetMaxBonds(self.atomic_number)
+
+    @property
+    def molecule(self) -> Molecule:
+        return self._data.get('mol')
+
+    @molecule.setter
+    def molecule(self, mol: 'Molecule'):
+        self._data['mol'] = mol
+
+    @property
+    def neighbours_hydrogen(self) -> List['Atom']:
+        """ return all neigh hydrogen atoms """
+        return [a for a in self.neighbours if a.is_hydrogen]
+
+    @property
+    def electronegativity(self):
+        return ob.GetElectroNeg(self.atomic_number)
+
+    @property
+    def neighbours(self) -> List['Atom']:
+        """ Get all atoms bond with this atom in same molecule """
+        if self.molecule:
+            _ = self.molecule.atoms  # update the atoms dict
+            return [self.molecule.atoms_dict[ob_atom.GetId()] for ob_atom in ob.OBAtomAtomIter(self.ob_atom)]
+        else:
+            return []
+
+    @property
+    def neighbours_label(self) -> List[str]:
+        """ return all neighbours labels """
+        return [a.label for a in self.neighbours]
+
+    @property
+    def neighbours_position(self) -> Generator[Tuple[Union['Atom', np.ndarray]], None, None]:
+        """ Retrieve the relative position of neigh atoms, assign this atom as the origin """
+        for neigh_atom in self.neighbours:
+            yield neigh_atom, neigh_atom.coordinates_array - self.coordinates_array
+
+    @property
+    def partial_charge(self):
+        return self.ob_atom.GetPartialCharge()
+
+    @partial_charge.setter
+    def partial_charge(self, value: float):
+        # This is necessary to take effect to the assignment.
+        # the reason is unknown
+        self.ob_atom.GetPartialCharge()
+        self._set_partial_charge(value)
+
+    def remove_hydrogen(self):
+        """ remove the first atom linking with the atoms """
+        hydrogens = self.neighbours_hydrogen
+        if hydrogens:
+            self.molecule.remove_atoms(hydrogens[0])
+
+    def remove_hydrogens(self):
+        """ Remove all hydrogens linking with the atom"""
+        hydrogens = self.neighbours_hydrogen
+        self.molecule.remove_atoms(*hydrogens)
+
+    def replace_attr_data(self, data: Dict):
+        """ Replace the core data dict directly """
+        self._data = data
+
+    def set(self, **kwargs):
+        """
+        Set atom attributes by kwargs
+        Kwargs:
+            atomic_number(int): set atomic number
+            symbol(str): set atomic symbol
+            coordinates(Sequence, numpy.ndarray): coordinates of the atom
+            partial_charge:
+            label:
+            spin_density:
+        """
+        self._set_attrs(**kwargs)  # set attributes
+
+    @property
+    def spin_density(self):
+        return self._data.get('spin_density', 0.0)
+
+    @spin_density.setter
+    def spin_density(self, spin_density: float):
+        self._set_spin_density(spin_density)
+
+    @property
+    def stable_valence(self) -> int:
+        if self.is_metal:
+            return 0
+        elif self.symbol == 'S':
+            if not [a for a in self.neighbours if a.symbol == 'O']:
+                return 2
+            elif self.covalent_valence <= 2:
+                return 2
+            elif self.covalent_valence <= 4:
+                return 4
+            else:
+                return 6
+        elif self.symbol == 'S':
+            if not [a for a in self.neighbours if a.symbol == 'O']:
+                return 3
+            elif self.covalent_valence == 0:
+                return 0
+            elif self.covalent_valence == 1:
+                return 1
+            elif self.covalent_valence <= 3:
+                return 3
+            else:
+                return 5
+        else:
+            return abs(_stable_charges[self.symbol])
+
+    @property
+    def symbol(self) -> str:
+        return ob.GetSymbol(self.atomic_number)
+
+    @property
+    def valence(self) -> int:
+        # if self.has_unknown_bond:
+        #     raise AttributeError('Cannot calculate the bond valence, because of the existence of unknown bonds')
+        return sum(b.type if b.type else 0 if b.is_covalent else 1 for b in self.bonds)
+
+
+class PseudoAtom(Wrapper, ABC):
+    """ A data wrapper for pseudo atom """
+
+    def __init__(self, symbol: str, mass: float, coordinates: Union[Sequence, np.ndarray], **kwargs):
+        if isinstance(coordinates, Sequence):
+            coordinates = np.array(coordinates)
+
+        assert isinstance(coordinates, np.ndarray) and coordinates.shape == (3,)
+
+        self._data = dict(symbol=symbol, mass=mass, coordinates=coordinates, **kwargs)
+
+    def __eq__(self, other):
+        if isinstance(other, PseudoAtom):
+            return self.symbol == other.symbol
+        return False
+
+    def __hash__(self):
+        return hash(f'PseudoAtom({self.symbol})')
+
+    def _attr_setters(self) -> Dict[str, Callable]:
+        return {}
+
+    def __repr__(self):
+        return f'PseudoAtom({self.symbol})'
+
+    def __dir__(self) -> Iterable[str]:
+        return list(self._data.keys())
+
+    def __getattr__(self, item):
+        return self._data.get(item, 0.)
+
+
+class Bond(Wrapper, ABC):
+    """"""
+
+    def __init__(self, ob_bond: ob.OBBond, _mol: Molecule):
+        self._data = {
+            'ob_obj': ob_bond,
+            'mol': _mol
+        }
+
+    def __repr__(self):
+        return f"Bond({self.atoms[0].label}, {self.atoms[1].label}, {self.type_name})"
+
+    def __eq__(self, other: 'Bond'):
+        if isinstance(other, Bond):
+            return self.pair_key == other.pair_key
+
+    def __hash__(self):
+        return hash(self.pair_key)
+
+    def __getitem__(self, item):
+        return self._data.get(item)
+
+    def __setitem__(self, key, value):
+        if key in super()._protected_data:
+            raise KeyError('the protected attr cannot be set be __setitem__ method')
+
+        self._data[key] = value
+
+    @property
+    def _protected_data(self):
+        return 'ob_obj', 'mol'
+
+    @property
+    def ob_bond(self):
+        return self._data['ob_obj']
+
+    def ob_bond_pop(self):
+        return self._data.pop('ob_obj')
+
+    def ob_bond_rewrap(self, ob_bond):
+        self._data['ob_obj'] = ob_bond
+
+    @property
+    def _attr_setters(self) -> Dict[str, Callable]:
+        return {
+        }
+
+    @property
+    def atom1(self) -> Atom:
+        return self.molecule.atoms_dict[self.ob_atom1_id]
+
+    @property
+    def atom2(self) -> Atom:
+        return self.molecule.atoms_dict[self.ob_atom2_id]
+
+    @property
+    def atomic_number1(self):
+        return self.ob_bond.GetBeginAtom().GetAtomicNum()
+
+    @property
+    def atomic_number2(self):
+        return self.ob_bond.GetEndAtom().GetAtomicNum()
+
+    @property
+    def atoms(self):
+        return self.atom1, self.atom2
+
+    @property
+    def begin_end_ob_id(self) -> (int, int):
+        return self.ob_bond.GetBeginAtom().GetId(), self.ob_bond.GetEndAtom().GetId()
+
+    @property
+    def begin_end_atomic_number(self):
+        return self.ob_bond.GetBeginAtom().GetAtomicNum(), self.ob_bond.GetEndAtom().GetAtomicNum()
+
+    @property
+    def is_covalent(self) -> bool:
+        return not self.ob_atom1.IsMetal() and not self.ob_atom2.IsMetal()
+
+    @property
+    def ideal_length(self):
+        return self.ob_bond.GetEquibLength()
+
+    @property
+    def ob_id(self):
+        return self.ob_bond.GetId()
+
+    @property
+    def ob_idx(self):
+        return self.ob_bond.GetIdx()
+
+    @property
+    def ob_atom1(self):
+        return self.ob_bond.GetBeginAtom()
+
+    @property
+    def ob_atom2(self):
+        return self.ob_bond.GetEndAtom()
+
+    @property
+    def ob_atom1_id(self):
+        return self.ob_atom1.GetId()
+
+    @property
+    def ob_atom2_id(self):
+        return self.ob_atom2.GetId()
+
+    @property
+    def pair_key(self):
+        """ Get the bond pair key, a string that show combination of element of end atoms and bond type,
+        where, the atomic symbol with lower atomic number is placed in the first, the higher in the last"""
+        if self.atomic_number1 <= self.atomic_number2:
+            return self.atomic_number1, self.type, self.atomic_number2
+        return self.atomic_number2, self.type, self.atomic_number1
+
+    @property
+    def length(self):
+        return self.ob_bond.GetLength()
+
+    @property
+    def molecule(self):
+        return self._data['mol']
+
+    @molecule.setter
+    def molecule(self, mol: Molecule):
+        self._data['mol'] = mol
+
+    @property
+    def type_name(self):
+        return _type_bond[self.type]
+
+    @property
+    def type(self):
+        return self.ob_bond.GetBondOrder()
+
+
+class Angle(MolLinker, ABC):
+    """ Data wrapper of angle in molecule """
+    def __init__(self, mol: Molecule, *ob_ids: int):
+        assert len(ob_ids) == 3
+        super().__init__(mol, ob_ids[1], ob_ids[0], ob_ids[2])
+
+    @property
+    def _degree(self) -> float:
+        return round(self.mol.ob_mol.GetAngle(*self.ob_atoms), 3)
+
+    @property
+    def degree(self) -> float:
+        return self._degree
+
+
+class Torsion(MolLinker):
+    """"""
+    @property
+    def _degree(self) -> float:
+        return self.mol.ob_mol.GetTorsion(*self.ob_atoms)
+
+    @property
+    def a(self) -> Atom:
+        """ The first atom """
+        return self.mol.atoms_dict[self.ob_atoms[0].GetId()]
+
+    @property
+    def b(self) -> Atom:
+        """ The second atom """
+        return self.mol.atoms_dict[self.ob_atoms[1].GetId()]
+
+    @property
+    def c(self) -> Atom:
+        """ The third atom """
+        return self.mol.atoms_dict[self.ob_atoms[2].GetId()]
+
+    @property
+    def d(self) -> Atom:
+        """ The fourth atom """
+        return self.mol.atoms_dict[self.ob_atoms[3].GetId()]
+
+    @property
+    def torsion(self) -> float:
+        return self._degree
+
+
+class Crystal(Wrapper, ABC):
+    """"""
+    _lattice_type = (
+        'Undefined', 'Triclinic', 'Monoclinic', 'Orthorhombic', 'Tetragonal', 'Rhombohedral', 'Hexagonal', 'Cubic'
+    )
+
+    def __init__(self, ob_unitcell: ob.OBUnitCell = None, **kwargs):
+
+        self._data: Dict[str, Any] = {
+            'OBUnitCell': ob_unitcell if ob_unitcell else ob.OBUnitCell(),
+        }
+
+        self._set_attrs(**kwargs)
+
+    def __repr__(self):
+        return f'Crystal({self.lattice_type}, {self.space_group}, {self.molecule})'
+
+    @property
+    def ob_unit_cell(self) -> ob.OBUnitCell:
+        return self._data.get('OBUnitCell')
+
+    @staticmethod
+    def _matrix_to_params(matrix: np.ndarray):
+        """ Covert the cell matrix to cell parameters: a, b, c, alpha, beta, gamma """
+        va, vb, vc = matrix
+        a = sum(va ** 2) ** 0.5
+        b = sum(vb ** 2) ** 0.5
+        c = sum(vc ** 2) ** 0.5
+
+        alpha = np.arccos(np.dot(va, vb) / (a * b)) / np.pi * 180
+        beta = np.arccos(np.dot(va, vc) / (a * c)) / np.pi * 180
+        gamma = np.arccos(np.dot(vb, vc) / (b * c)) / np.pi * 180
+
+        return a, b, c, alpha, beta, gamma
+
+    def _set_molecule(self, molecule: Molecule):
+        if molecule.crystal and isinstance(molecule.crystal, Crystal):
+            print(AttributeError("the Molecule have been stored in a Crystal, "
+                                 "can't save the same Molecule into two Crystals"))
+        else:
+            self._data['mol'] = molecule
+
+    def _set_space_group(self, space_group: str):
+        self.ob_unit_cell.SetSpaceGroup(space_group)
+
+    @property
+    def _attr_setters(self) -> Dict[str, Callable]:
+        return {
+            'mol': self._set_molecule,
+            'molecule': self._set_molecule,
+            'space_group': self._set_space_group
+        }
+
+    @property
+    def lattice_type(self) -> str:
+        return self._lattice_type[self.ob_unit_cell.GetLatticeType()]
+
+    @property
+    def lattice_params(self) -> np.ndarray[2, 3]:
+        a = self.ob_unit_cell.GetA()
+        b = self.ob_unit_cell.GetB()
+        c = self.ob_unit_cell.GetC()
+        alpha = self.ob_unit_cell.GetAlpha()
+        beta = self.ob_unit_cell.GetBeta()
+        gamma = self.ob_unit_cell.GetGamma()
+        return np.array([[a, b, c], [alpha, beta, gamma]])
+
+    @property
+    def molecule(self) -> Molecule:
+        return self._data.get('mol')
+
+    @molecule.setter
+    def molecule(self, mol: Molecule):
+        self._data['mol'] = mol
+
+    @property
+    def pack_molecule(self) -> Molecule:
+        mol = self.molecule  # Get the contained Molecule
+
+        if not mol:  # if you get None
+            print(RuntimeWarning("the crystal doesn't contain any Molecule!"))
+
+        pack_mol = mol.copy()
+        self.ob_unit_cell.FillUnitCell(pack_mol.ob_mol)  # Full the crystal
+        pack_mol._reorganize_atom_indices()  # Rearrange the atom indices.
+
+        return pack_mol
+
+    def set_lattice(
+            self,
+            a: float, b: float, c: float,
+            alpha: float, beta: float, gamma: float
+    ):
+        self.ob_unit_cell.SetData(a, b, c, alpha, beta, gamma)
+
+    def set_vectors(
+            self,
+            va: Union[np.ndarray, Sequence],
+            vb: Union[np.ndarray, Sequence],
+            vc: Union[np.ndarray, Sequence]
+    ):
+        """"""
+        vectors = [va, vb, vc]
+        matrix = np.array(vectors)
+        self.set_matrix(matrix)
+
+    def set_matrix(self, matrix: np.ndarray):
+        """ Set cell matrix for the crystal """
+        if matrix.shape != (3, 3):
+            raise AttributeError('the shape of cell_vectors should be [3, 3]')
+
+        cell_params = map(float, self._matrix_to_params(matrix))
+
+        self.ob_unit_cell.SetData(*cell_params)
+
+    @property
+    def space_group(self):
+        space_group = self.ob_unit_cell.GetSpaceGroup()
+        if space_group:
+            return space_group.GetHMName()
+        else:
+            return None
+
+    @space_group.setter
+    def space_group(self, value: str):
+        self._set_space_group(value)
+
+    @property
+    def volume(self):
+        return self.ob_unit_cell.GetCellVolume()
+
+    @property
+    def vector(self):
+        v1, v2, v3 = self.ob_unit_cell.GetCellVectors()
+        return np.array([
+            [v1.GetX(), v1.GetY(), v1.GetZ()],
+            [v2.GetX(), v2.GetY(), v2.GetZ()],
+            [v3.GetX(), v3.GetY(), v3.GetZ()]
+        ])
+
+    def zeo_plus_plus(self):
+        """ TODO: complete the method after define the Crystal and ZeoPlusPlus tank """
+
+
+class ZMatrix:
+    """
+    Represent the Z-Matrix(internal coordinates) in a Molecule.
+    The Z-Matrix of a Molecule objects could be accessed by its attribute `z_matrix`
+
+    Each element of Z-Matrix, like start atom, radium, angle, dihedral could be accessed by subscript.
+    Liking ZMatrix['r10'], it gets a radium start from 10th atoms. the subscripts are encode to be strings
+    with 's'(start atom), 'r'(radium), 'a'(angle), 'd'(dihedral) as the first header, and the number of atoms
+    as the follower. It should be noted that the number of atoms start from 1 instead of the 0, in general
+    it's the ob_id - 1
+
+    Examples:
+        mol = hp.Molecule.read_from(...)
+        zmat = mol.z_matrix
+        print(zmat['s10'], zmat['r10'], zmat['a10'], zmat['d10'])
+
+    """
+    class ZMatrixItem:
+        def __init__(self, key: str, item: Union[Atom, Bond, Angle, Torsion], value: float):
+            self.key = key
+            self.item = item
+            self.value = value
+
+        def __repr__(self):
+            return f"{self.item.__class__.__name__}({self.key}, " \
+                   f"{self.item_value if isinstance(self.item_value, int) else round(self.item_value, 3)})"
+
+        @property
+        def item_value(self) -> Union[float, int]:
+            if isinstance(self.item, Atom):
+                return self.item.ob_id
+            elif isinstance(self.item, Bond):
+                return self.item.length
+            elif isinstance(self.item, Angle):
+                return self.item.degree
+            elif isinstance(self.item, Torsion):
+                return self.item.torsion
+
+    def __init__(self, mol: Molecule):
+        self.mol = mol
+        self._coords = {}
+        self._coord_line = {}
+        self._update_coords()
+
+    def __repr__(self):
+        return f'InternalCoordinates({len(self)})'
+
+    def __str__(self):
+        return '\n'.join(' '.join(str(item) for item in line) for _, line in self)
+
+    def __len__(self):
+        return len(self._coord_line)
+
+    def __iter__(self):
+        return iter(self._coord_line.items())
+
+    def __getitem__(self, item):
+        self._update_coords()
+        return self._coords[item]
+
+    def __setitem__(self, key, value):
+        """ Set the Z-Matrix, TODO: this method do not work now """
+        ob_internal_coords = list(self.mol.ob_mol.GetInternalCoord())
+        head, line_count = key[0], int(key[1:])
+
+        # Check the given key
+        if head not in ('r', 'a', 'd') or line_count >= len(ob_internal_coords):
+            raise KeyError(f'cannot not set the attr {key}, it is non-existent or irregular')
+        elif line_count == 2 and head in ('a', 'd'):
+            raise KeyError(f'cannot not set the attr {key}, it is non-existent or irregular')
+        elif line_count == 3 and head == 'd':
+            raise KeyError(f'cannot not set the attr {key}, it is non-existent or irregular')
+
+        # Get the original OBInternalCoord
+        set_coord: ob.OBInternalCoord = ob_internal_coords[line_count]
+
+        # Replace the value of specified item
+        kwargs = {
+            'a': set_coord._a,
+            'b': set_coord._b,
+            'c': set_coord._c,
+            'dst': value if head == 'r' else set_coord._dst,
+            'ang': value if head == 'a' else set_coord._ang,
+            'tor': value if head == 'd' else set_coord._tor
+        }
+        ob_internal_coords[line_count] = ob.OBInternalCoord(**kwargs)
+
+        # Set the parent molecule
+        self.mol.ob_mol.SetInternalCoord(ob_internal_coords)
+
+    def _update_coords(self):
+        """ Update the internal coordinates data """
+        coord_lines, coords = {}, {}
+
+        atoms = self.mol.atoms
+        for i, line in enumerate(self.mol.ob_mol.GetInternalCoord()):
+
+            # ignore the first item, it's None
+            if not line:
+                continue
+
+            atom = atoms[i - 1]
+
+            coords[f's{i}'] = self.ZMatrixItem(f's{i}', atom, i - 1)
+
+            coord_line = coord_lines.setdefault(i, [])
+            coord_line.append(coords[f's{i}'])
+
+            # atom_radial, atom_angle, atom_dihedral, radial, angle, dihedral
+            ar, aa, ad, r, a, d = line._a, line._b, line._c, line._dst, line._ang, line._tor
+
+            if isinstance(ar, ob.OBAtom):
+                assert isinstance(r, float)
+                coords[f'r{i}'] = self.ZMatrixItem(
+                    f'r{i}', self.mol.bond(atom.ob_id, ar.GetId()), r
+                )
+                coord_line.append(coords[f'r{i}'])
+
+            if isinstance(aa, ob.OBAtom):
+                assert isinstance(a, float)
+                coords[f'a{i}'] = self.ZMatrixItem(
+                    f'a{i}', self.mol.angle(atom.ob_id, ar.GetId(), aa.GetId()), a
+                )
+                coord_line.append(coords[f'a{i}'])
+
+            if isinstance(ad, ob.OBAtom):
+                assert isinstance(d, float)
+                coords[f'd{i}'] = self.ZMatrixItem(
+                    f'd{i}', self.mol.torsion(atom.ob_id, ar.GetId(), aa.GetId(), ad.GetId()), d
+                )
+                coord_line.append(coords[f'd{i}'])
+
+        self._coord_line = coord_lines
+        self._coords = coords
+
+
+import hotpot.bundle as bd
+from hotpot._io import Dumper, Parser
+from hotpot.tanks.cc import PairBundle
+from hotpot.tanks.deepmd import DeepSystem
```

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/deepmd_script.json` & `hotpot-zzy-0.3.1.0/hotpot/data/deepmd_script.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.3.1.0/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.3.1.0/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/periodic_table.json` & `hotpot-zzy-0.3.1.0/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,1-trichloroethane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,1-trichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,1-trifluroethanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,1-trifluroethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,2-trichloroethene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1,2-trichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-dichloroethene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-diethoxypropane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-diethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-dimethoxymethane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,1-dimethoxymethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dichloroethane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dichloroethene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dimethoxyethane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,2-dimethoxyethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,4-dioxane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1,4-dioxane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-butanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-pentanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-pentanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-propanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2,2-dimethoxypropane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2,2-dimethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-butanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-ethoxyethanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-ethoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methoxyethanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methyl-1-propanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methyl-1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methyltetrahydrofuran.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/2-methyltetrahydrofuran.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/3-methyl-1-butanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/3-methyl-1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/DCM.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/DCM.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/DMF.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/DMF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/DMSO.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/DMSO.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/N,N-dimethylacetamide.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/N,N-dimethylacetamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/N-methylpyrrolidone.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/N-methylpyrrolidone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/THF.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/THF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetic_acid.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetone.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetonitrile.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/acetonitrile.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/benzene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/benzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/butylacetate.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/butylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/carbon_tetrachloride.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/carbon_tetrachloride.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/chlorobenzene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/chlorobenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/chloroform.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/chloroform.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/cumene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/cumene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/cyclohexane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/cyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/diethylether.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/diethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/diisopropylamine.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/diisopropylamine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethyl_formate.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethyl_formate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethylacetate.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethyleneglycol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ethyleneglycol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/formamide.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/formamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/formic_acid.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/formic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/heptane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/heptane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/hexane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/hexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isobutyl_acetate.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isobutyl_acetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isooctane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isooctane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropylacetate.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropylether.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/isopropylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/meta-xylene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/meta-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methanol.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methoxybenzene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methoxybenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylacetate.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylbutylketone.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylbutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylcyclohexane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylcyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylethylketone.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylethylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylisobutylketone.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylisobutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylisopropylketone.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/methylisopropylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/morpholine.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/morpholine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/nitromethane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/nitromethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ortho-xylene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/ortho-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/para-xylene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/para-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/pentane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/pentane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/propylacetate.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/propylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/pyridine.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/pyridine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/sulfolane.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/sulfolane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/t-butylmethylether.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/t-butylmethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/tetralin.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/tetralin.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/toluene.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/toluene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/trichloroacetic_acid.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/trichloroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/data/solvents/trifluoroacetic_acid.mol2` & `hotpot-zzy-0.3.1.0/hotpot/data/solvents/trifluoroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/tanks/deepmd.py` & `hotpot-zzy-0.3.1.0/hotpot/tanks/deepmd.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,225 +1,241 @@
-"""
-python v3.9.0
-@Project: hotpot
-@File   : deepmd.py
-@Author : Zhiyuan Zhang
-@Date   : 2023/6/26
-@Time   : 21:42
-"""
-import os
-import json
-from typing import *
-from pathlib import Path
-from copy import copy
-
-import numpy as np
-
-from hotpot import data_root
-from hotpot.cheminfo import Molecule, periodic_table
-
-# Manuscript training script
-_script = json.load(open(os.path.join(data_root, 'deepmd_script.json')))
-
-
-class DeepSystem:
-    """
-    a handle class to track DeepMD data
-    Args:
-        mol(Molecule):
-
-    """
-
-    required_items = ('coord', 'type')
-    check_atom_num = ('coord', 'force', 'charge')
-    share_same_conformers = ('type', 'coord', 'energy', 'force', 'charge', 'virial', 'box', 'identifiers')
-    need_reshape = ('coord', 'force')
-
-    def __init__(self, mol: Molecule = None, data: dict = None):
-        if mol:
-            self.data = self._organize_data(mol)
-            # check numpy.ndarray shape
-            self._check_shape()
-            # reshape array
-            self._reshape_array()
-        elif data:
-            self.data = data
-        else:
-            raise ValueError('the args mol or data should be given at least one!')
-
-    def __repr__(self):
-        return f'{self.__class__.__name__}({len(self.data["coord"])})'
-
-    def __call__(
-            self,
-            save_dir: Union[str, os.PathLike], mode: str = 'std',
-            validate_ratio: Optional[float] = None,
-            validate_dir: Union[str, os.PathLike] = None
-    ):
-        """
-        Save the DeepMData to files
-        Args:
-            save_dir(str|os.PathLike|Path): the root dir for all corresponding DeepMDate system files,
-             if the validate ratio is given, this the represent the training set save dir
-            validate_ratio(float): the ratio of validate set, if not given, not split the dataset
-            validate_dir: should be give when validate_ratio has been given, the root dir for validate data
-        """
-        if not isinstance(save_dir, Path):
-            save_dir = Path(save_dir)
-
-        if validate_ratio:
-            if not isinstance(validate_dir, (str, os.PathLike)):
-                raise ValueError('the arguments validate_dir has not been given!')
-            elif isinstance(validate_dir, str):
-                validate_dir = Path(validate_dir)
-
-            if not 0 < validate_ratio < 1:
-                raise ValueError('the validate ratio should from 0 to 1')
-
-            indices = np.arange(len(self))
-            validate_idx = np.random.choice(indices, size=int(len(self) * validate_ratio), replace=False)
-            training_idx = np.setdiff1d(indices, validate_idx)
-
-            validate_data = self[validate_idx]
-            training_data = self[training_idx]
-
-            self._save_deep_md(training_data, save_dir, mode)
-            self._save_deep_md(validate_data, validate_dir, mode)
-
-        else:
-            self._save_deep_md(self, save_dir, mode)
-
-    def __getitem__(self, item: Union[int, slice, np.ndarray]):
-        data = copy(self.data)
-        if not isinstance(item, (int, slice, np.ndarray)):
-            raise TypeError('the item should be int, slice or numpy.ndarray')
-
-        for name in self.share_same_conformers:
-            arrays = self.data.get(name)
-            if isinstance(arrays, np.ndarray):
-                data[name] = arrays[item]
-
-        return self.__class__(data=data)
-
-    def __getattr__(self, item: str):
-        if item not in self.__dir__():
-            raise AttributeError(f'the {self.__class__.__name__} not have attribute {item}')
-        return self.data.get(item, None)
-
-    def __dir__(self) -> Iterable[str]:
-        return [
-            'type', 'type_map', 'nopbc', 'coord', 'box', 'energy', 'force', 'charge',
-            'atom_counts','virial', 'atom_ener', 'atom_pref', 'dipole', 'atom_dipole',
-            'polarizability', 'atomic_polarizability'
-        ]
-
-    def __len__(self):
-        return len(self.data['coord'])
-
-    def _check_shape(self):
-        """ Check whether the shape ndarray is correct """
-        conf_counts = len(self.data['coord'])
-        atom_counts = self.data['atom_counts']
-
-        for name in self.required_items:
-            if self.data.get(name) is None:
-                raise ValueError('the required composition to make the dpmd system is incomplete!')
-
-        # Check whether the number of conformers are matching among data
-        if any(len(self.data[n]) != conf_counts for n in self.share_same_conformers if self.data[n] is not None):
-            raise ValueError('the number of conformers is not match')
-
-        # Check whether the number of atoms in data are matching to the molecular atoms
-        if any(self.data[n].shape[1] != atom_counts for n in self.check_atom_num if self.data[n] is not None):
-            raise ValueError('the number of atoms is not matching the number of atom is the molecule')
-
-    def _reshape_array(self):
-        for name in self.need_reshape:
-            item = self.data.get(name)
-            if isinstance(item, np.ndarray):
-                shape = item.shape
-
-                assert len(shape) == 3
-
-                self.data[name] = item.reshape((shape[0], shape[1] * shape[2]))
-
-    @staticmethod
-    def _organize_data(mol: Molecule) -> Dict[str, Any]:
-        """ Organize the conformer data to a dict """
-        conf_num = len(mol.all_coordinates)
-        crystal = mol.crystal()
-        if crystal:
-            box = mol.crystal().vector  # angstrom
-            is_periodic = True
-        else:
-            box = np.zeros((3, 3))
-            for i in range(3):
-                box[i, i] = 100.
-            is_periodic = False
-        box = box.reshape(-1, 9).repeat(conf_num, axis=0)
-
-        return {
-            'type': mol.atomic_numbers_array,  # matrix of (conformer_counts, atom_counts)
-            'type_map': ['-'] + list(periodic_table.symbols),
-            'nopbc': not is_periodic,
-            'coord': mol.all_coordinates,  # angstrom,
-            'box': box,
-            'energy': mol.all_energy,  # eV
-            'force': mol.all_forces,  # Hartree/Bohr,
-            'charge': mol.all_atom_charges,  # q
-            'atom_counts': mol.atom_counts,
-            'identifiers': mol.identifier_array,
-            'virial': None,
-            'atom_ener': None,
-            'atom_pref': None,
-            'dipole': None,
-            'atom_dipole': None,
-            'polarizability': None,
-            'atomic_polarizability': None
-        }
-
-    @staticmethod
-    def _save_deep_md(system: 'DeepSystem', save_dir: Path, mode: str):
-        """ Save DeepMData to dir """
-        if not save_dir.exists():
-            save_dir.mkdir()
-
-        # the dir of set data
-        set_root = save_dir.joinpath('set.000')
-        if not set_root.exists():
-            set_root.mkdir()
-
-        for name, value in system.data.items():
-
-            # if the value is None, go to next
-            if value is None:
-                continue
-
-            # Write the type raw
-            if name == 'type':
-                if mode == 'std':
-                    type_raw = value[0]
-                elif mode == 'att':
-                    type_raw = np.zeros(value[0].shape, dtype=int)
-                    np.save(set_root.joinpath("real_atom_types.npy"), value)
-                else:
-                    raise ValueError('the mode just allows to be "std" or "att"')
-
-                with open(save_dir.joinpath('type.raw'), 'w') as writer:
-                    writer.write('\n'.join([str(i) for i in type_raw]))
-
-            elif name == 'type_map':
-                with open(save_dir.joinpath('type_map.raw'), 'w') as writer:
-                    writer.write('\n'.join([str(i) for i in value]))
-
-            # Create an empty 'nopbc', when the system is not periodical
-            elif name == 'nopbc' and value is True:
-                with open(save_dir.joinpath('nopbc'), 'w') as writer:
-                    writer.write('')
-
-            # Save the numpy format data
-            elif isinstance(value, np.ndarray):
-                np.save(str(set_root.joinpath(f'{name}.npy')), value)
-
-
-def make_script():
-    """"""
+"""
+python v3.9.0
+@Project: hotpot
+@File   : deepmd.py
+@Author : Zhiyuan Zhang
+@Date   : 2023/6/26
+@Time   : 21:42
+"""
+import os
+import json
+from typing import *
+from pathlib import Path
+from copy import copy
+
+import numpy as np
+import pandas as pd
+
+from hotpot import data_root
+from hotpot.cheminfo import Molecule, periodic_table
+
+# Manuscript training script
+_script = json.load(open(os.path.join(data_root, 'deepmd_script.json')))
+
+
+class DeepSystem:
+    """
+    A handle to convert the Molecule object ot DeepModeling System data format
+    Args:
+        mol(Molecule):
+
+    """
+
+    required_items = ('coord', 'type')
+    check_atom_num = ('coord', 'force', 'charge')
+    share_same_conformers = ('type', 'coord', 'energy', 'force', 'charge', 'virial', 'box', 'identifiers')
+    need_reshape = ('coord', 'force')
+
+    def __init__(self, mol: Molecule = None, data: dict = None):
+        if mol:
+            self.data = self._organize_data(mol)
+            # check numpy.ndarray shape
+            self._check_shape()
+            # reshape array
+            self._reshape_array()
+        elif data:
+            self.data = data
+        else:
+            raise ValueError('the args mol or data should be given at least one!')
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}({len(self.data["coord"])})'
+
+    def __call__(
+            self,
+            save_dir: Union[str, os.PathLike], mode: str = 'std',
+            validate_ratio: Optional[float] = None,
+            validate_dir: Union[str, os.PathLike] = None
+    ):
+        """
+        Save the DeepMData to files
+        Args:
+            save_dir(str|os.PathLike|Path): the root dir for all corresponding DeepMDate system files,
+             if the validate ratio is given, this the represent the training set save dir
+            validate_ratio(float): the ratio of validate set, if not given, not split the dataset
+            validate_dir: should be give when validate_ratio has been given, the root dir for validate data
+        """
+        if not isinstance(save_dir, Path):
+            save_dir = Path(save_dir)
+
+        if validate_ratio:
+            if not isinstance(validate_dir, (str, os.PathLike)):
+                raise ValueError('the arguments validate_dir has not been given!')
+            elif isinstance(validate_dir, str):
+                validate_dir = Path(validate_dir)
+
+            if not 0 < validate_ratio < 1:
+                raise ValueError('the validate ratio should from 0 to 1')
+
+            indices = np.arange(len(self))
+            validate_idx = np.random.choice(indices, size=int(len(self) * validate_ratio), replace=False)
+            training_idx = np.setdiff1d(indices, validate_idx)
+
+            validate_data = self[validate_idx]
+            training_data = self[training_idx]
+
+            self._save_deep_md(training_data, save_dir, mode)
+            self._save_deep_md(validate_data, validate_dir, mode)
+
+        else:
+            self._save_deep_md(self, save_dir, mode)
+
+    def __getitem__(self, item: Union[int, slice, np.ndarray]):
+        data = copy(self.data)
+        if not isinstance(item, (int, slice, np.ndarray)):
+            raise TypeError('the item should be int, slice or numpy.ndarray')
+
+        for name in self.share_same_conformers:
+            arrays = self.data.get(name)
+            if isinstance(arrays, np.ndarray):
+                data[name] = arrays[item]
+
+        return self.__class__(data=data)
+
+    def __getattr__(self, item: str):
+        if item not in self.__dir__():
+            raise AttributeError(f'the {self.__class__.__name__} not have attribute {item}')
+        return self.data.get(item, None)
+
+    def __dir__(self) -> Iterable[str]:
+        return [
+            'type', 'type_map', 'nopbc', 'coord', 'box', 'energy', 'force', 'charge',
+            'atom_counts','virial', 'atom_ener', 'atom_pref', 'dipole', 'atom_dipole',
+            'polarizability', 'atomic_polarizability'
+        ]
+
+    def __len__(self):
+        return len(self.data['coord'])
+
+    def _check_shape(self):
+        """ Check whether the shape ndarray is correct """
+        conf_counts = len(self.data['coord'])
+        atom_counts = self.data['atom_counts']
+
+        for name in self.required_items:
+            if self.data.get(name) is None:
+                raise ValueError('the required composition to make the dpmd system is incomplete!')
+
+        # Check whether the number of conformers are matching among data
+        if any(len(self.data[n]) != conf_counts for n in self.share_same_conformers if self.data[n] is not None):
+            raise ValueError('the number of conformers is not match')
+
+        # Check whether the number of atoms in data are matching to the molecular atoms
+        if any(self.data[n].shape[1] != atom_counts for n in self.check_atom_num if self.data[n] is not None):
+            raise ValueError('the number of atoms is not matching the number of atom is the molecule')
+
+    def _reshape_array(self):
+        for name in self.need_reshape:
+            item = self.data.get(name)
+            if isinstance(item, np.ndarray):
+                shape = item.shape
+
+                assert len(shape) == 3
+
+                self.data[name] = item.reshape((shape[0], shape[1] * shape[2]))
+
+    @staticmethod
+    def _organize_data(mol: Molecule) -> Dict[str, Any]:
+        """ Organize the conformer data to a dict """
+        conf_num = len(mol.all_coordinates)
+        crystal = mol.crystal()
+        if crystal:
+            box = mol.crystal().vector  # angstrom
+            is_periodic = True
+        else:
+            box = np.zeros((3, 3))
+            for i in range(3):
+                box[i, i] = 100.
+            is_periodic = False
+        box = box.reshape(-1, 9).repeat(conf_num, axis=0)
+
+        return {
+            'type': mol.atomic_numbers_array,  # matrix of (conformer_counts, atom_counts)
+            'type_map': ['-'] + list(periodic_table.symbols),
+            'nopbc': not is_periodic,
+            'coord': mol.all_coordinates,  # angstrom,
+            'box': box,
+            'energy': mol.all_energy,  # eV
+            'force': mol.all_forces,  # Hartree/Bohr,
+            'charge': mol.all_atom_charges,  # q
+            'atom_counts': mol.atom_counts,
+            'identifiers': mol.identifier_array,
+            'virial': None,
+            'atom_ener': None,
+            'atom_pref': None,
+            'dipole': None,
+            'atom_dipole': None,
+            'polarizability': None,
+            'atomic_polarizability': None
+        }
+
+    @staticmethod
+    def _save_deep_md(system: 'DeepSystem', save_dir: Path, mode: str):
+        """ Save DeepMData to dir """
+        if not save_dir.exists():
+            save_dir.mkdir()
+
+        # the dir of set data
+        set_root = save_dir.joinpath('set.000')
+        if not set_root.exists():
+            set_root.mkdir()
+
+        for name, value in system.data.items():
+
+            # if the value is None, go to next
+            if value is None:
+                continue
+
+            # Write the type raw
+            if name == 'type':
+                if mode == 'std':
+                    type_raw = value[0]
+                elif mode == 'att':
+                    type_raw = np.zeros(value[0].shape, dtype=int)
+                    np.save(set_root.joinpath("real_atom_types.npy"), value)
+                else:
+                    raise ValueError('the mode just allows to be "std" or "att"')
+
+                with open(save_dir.joinpath('type.raw'), 'w') as writer:
+                    writer.write('\n'.join([str(i) for i in type_raw]))
+
+            elif name == 'type_map':
+                with open(save_dir.joinpath('type_map.raw'), 'w') as writer:
+                    writer.write('\n'.join([str(i) for i in value]))
+
+            # Create an empty 'nopbc', when the system is not periodical
+            elif name == 'nopbc' and value is True:
+                with open(save_dir.joinpath('nopbc'), 'w') as writer:
+                    writer.write('')
+
+            # Save the numpy format data
+            elif isinstance(value, np.ndarray):
+                np.save(str(set_root.joinpath(f'{name}.npy')), value)
+
+
+def make_script():
+    """"""
+
+
+def convert_lcurve_to_csv(path_lcurve: Union[str, Path], path_csv: Union[str, Path] = None) -> pd.DataFrame:
+    """ Convert the lcurve.out file to csv file """
+    path_lcurve = Path(path_lcurve)
+    if not path_csv:
+        path_csv = path_lcurve.parent.joinpath('lcurve.csv')
+    else:
+        path_csv = Path(path_csv)
+
+    df = pd.DataFrame(np.genfromtxt(path_lcurve, names=True))
+    df.set_index(df.columns[0], inplace=True)
+    df.to_csv(path_csv)
+
+    return df
```

### Comparing `hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.3.1.0/hotpot/tanks/lmp/materials.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,240 +1,249 @@
-"""
-python v3.7.9
-@Project: hotpot
-@File   : materials.py
-@Author : Zhiyuan Zhang
-@Date   : 2023/4/26
-@Time   : 1:50
-Notes:
-    This package is to perform some specific tasks base on the LAMMPS
-"""
-import os
-import os.path as osp
-from os.path import join as ptj
-from typing import *
-import math
-import random
-import numpy as np
-import openbabel.openbabel as ob
-import hotpot
-import hotpot.cheminfo as ci
-
-
-dir_force_field = osp.abspath(ptj(hotpot.data_root, 'force_field'))
-
-# Constants
-avogadro = 6.02214076e23  # Avogadro numbers
-angstrom = 1e-8  # cm
-
-
-class AmorphousMaker:
-    """ To make Amorphous Materials """
-    def __init__(
-            self,
-            element_composition: Dict[str, float],
-            force_field: Union[str, os.PathLike],
-            density: float = 1.0,  # g/cm^3
-            a: float = 25., b: float = 25., c: float = 25.,
-            alpha: float = 90., beta: float = 90., gamma: float = 90.,
-    ):
-        """"""
-        # Check the arguments
-        # Determine the path of force field.
-        if isinstance(force_field, os.PathLike):
-            pff = str(force_field)
-        elif osp.exists(force_field):
-            pff = force_field
-        else:
-            pff = ptj(dir_force_field, force_field)
-
-        # Make sure the existence of force field file
-        if not osp.exists(pff):
-            raise FileNotFoundError('the given force field file is not found!')
-
-        pff = osp.abspath(pff)
-
-        # assign attrs
-        sum_freq = sum(f for f in element_composition.values())
-        self.elements = {e: f/sum_freq for e, f in element_composition.items()}  # Normalize the elements' frequency
-        self.path_force_field = pff
-        self.density = density
-        self.cryst_params = (a, b, c, alpha, beta, gamma)
-
-    @staticmethod
-    def calc_cryst_density(cryst):
-        """ Calculation the density for Crystal object """
-        return (cryst.molecule.weight * avogadro) / (cryst.volume * angstrom ** 3)  # Density, g/cm^3
-
-    @staticmethod
-    def density2atom_numbers(ratio_elements: dict, density: float, cryst):
-        """
-        Calculate the round atom numbers in a crystal.
-        Args:
-            ratio_elements: Ratio of elements in the crystal
-            density: the demand density in the crystal
-            cryst: the crystal
-
-        Returns:
-            int, the number of atoms
-        """
-        # Convert the dict of elements and possibility to numpy array
-        elements = np.array(list(ratio_elements.keys()))
-        possibility = np.array(list(ratio_elements.values()))
-        possibility = possibility / possibility.sum()  # Normalize
-
-        average_mol_mass = sum(ob.GetMass(ob.GetAtomicNum(e)) * p for e, p in zip(elements, possibility))
-
-        # Terms:   [Mole in Crystal(Total Mass in Crystal (gram)/Average Mole Mass)]/Avogadro Number
-        # Units:      g/cm^3     angstrom^3  angstrom/cm             g/mol             _
-        num_atom = ((density * (cryst.volume * angstrom ** 3)) / average_mol_mass) * avogadro
-
-        v1, v2, v3 = cryst.vector  # crystal vectors
-        dv1, dv2, dv3 = np.sqrt(sum(v1 ** 2)), np.sqrt(sum(v2 ** 2)), np.sqrt(sum(v3 ** 2))  # length of crystal vectors
-        min_dv = min(dv1, dv2, dv3)  # the min length in these vectors
-        r_dv1, r_dv2, r_dv3 = dv1 / min_dv, dv2 / min_dv, dv3 / min_dv  # the ratios of length of vector to min vector
-
-        # If all vectors are replaced with the smallest one,
-        # how many times is the actual crystal volume after replacement
-        fold_min_dv_volume = r_dv1 * r_dv2 * r_dv3
-
-        # number of grid points in the direction of min vector
-        min_point = math.pow(num_atom / fold_min_dv_volume, 1 / 3)
-
-        # number of point for in the direction of v1, v2, v3
-        num_pv1, num_pv2, num_pv3 = int(r_dv1 * min_point), int(r_dv2 * min_point), int(r_dv3 * min_point)
-        # the coordinate of grad point in the bases of v1, v2, v3
-        pv1, pv2, pv3 = np.meshgrid(
-            np.linspace(0, 1, num_pv1, endpoint=False),
-            np.linspace(0, 1, num_pv2, endpoint=False),
-            np.linspace(0, 1, num_pv3, endpoint=False)
-        )
-
-        fraction_coordinates = np.stack((pv1.flatten(), pv2.flatten(), pv3.flatten()))
-
-        # the actual coordinates in the cartesian coordinates
-        cartesian_coordinates = np.matmul(cryst.vector, fraction_coordinates).T
-
-        num_atom = len(cartesian_coordinates)
-        atomic_symbols = np.random.choice(elements, num_atom, p=possibility)
-        atomic_numbers = np.array([ob.GetAtomicNum(symbol) for symbol in atomic_symbols])
-
-        return atomic_numbers, cartesian_coordinates
-
-    def load_atoms(self):
-        mol = ci.Molecule()
-        mol.make_crystal(*self.cryst_params)
-
-        cryst = mol.crystal()
-        atomic_number, coordinates = self.density2atom_numbers(
-            self.elements, self.density, cryst
-        )
-
-        mol.quick_build_atoms(atomic_number)
-        mol.set(all_coordinates=coordinates.reshape((-1, len(coordinates), 3)))
-
-        mol.conformer_select(0)
-
-        return mol
-
-    def melt_quench(
-            self, *ff_args, mol=None, path_writefile: Optional[str] = None,
-            origin_temp: float = 298.15, melt_temp: float = 4000., highest_temp: float = 10000,
-            time_step: float = 0.0001, path_dump_to: Optional[str] = None, dump_every: int = 100,
-    ):
-        """
-        Perform melt-quench process to manufacture a amorphous materials
-        Args:
-            *ff_args: the arguments the force file requried, refering the LAMMPS pair_coeff:
-             "pair_coeff I J args" url: https://docs.lammps.org/pair_coeff.html
-            mol: the molecule to be performed melt-quench. if not given, initialize according to elemental
-             compositions
-            path_writefile: the path to write the final material (screenshot) to file, if not specify, not save.
-            origin_temp: the initial temperature before melt
-            melt_temp: the round melting point to the materials
-            highest_temp: the highest temperature to liquefy the materials
-            time_step: time interval between path integrals when performing melt-quench
-            path_dump_to: the path to save the trajectory of the melt-quench process, if not specify not save
-            dump_every: the step interval between each dumps
-        Returns:
-            Molecule obj after melt-quench.
-        """
-        if not isinstance(mol, ci.Molecule):
-            mol = self.load_atoms()
-
-        mol.lmp_setup(units='metal')
-
-        # initialization
-        mol.lmp.commands_string(
-            """
-            units metal
-            dimension 3
-            atom_style full
-            """
-        )
-
-        # Read molecule into LAMMPS
-        mol.lmp.read_main_data()
-
-        # Configure the force field
-        mol.lmp("pair_style tersoff")
-        mol.lmp(f"pair_coeff * * {self.path_force_field} {' '.join(ff_args)}")
-
-        # Specify the thermodynamical output to screen
-        mol.lmp('thermo_style    custom step temp pe etotal press vol density')
-        mol.lmp('thermo          1000')
-
-        # the step interval of integral
-        mol.lmp(f'timestep {time_step}')
-
-        # Specify the dump configuration
-        if path_dump_to:
-            dump_fmt = path_dump_to.split('.')[-1]  # the dump fmt is the suffix of file name
-            mol.lmp(f'dump mq all {dump_fmt} {dump_every} {path_dump_to}')
-            mol.lmp(f'dump_modify mq element {" ".join(set(mol.atomic_symbols))}')
-
-        # Initialize the temperature for system
-        mol.lmp(f'velocity all create {origin_temp} {random.randint(100000, 999999)}')
-
-        # Melt
-        mol.lmp(f'fix 0 all nvt temp {origin_temp} {highest_temp} 0.7')
-        mol.lmp(f'run 10000')
-
-        mol.lmp(f'fix 0 all nvt temp {highest_temp} {highest_temp} 1000')
-        while mol.lmp.eval('temp') < highest_temp * 0.95:
-            mol.lmp(f'run 1000')
-
-        mol.lmp(f'run 10000')
-
-        # Relax
-        mol.lmp('thermo          250')
-        mol.lmp(f'fix 0 all nvt temp {melt_temp} {melt_temp} 1000.0')
-        while mol.lmp.eval('temp') > melt_temp * 1.05:
-            mol.lmp(f'velocity all scale {melt_temp}')
-            mol.lmp(f'run 2000')
-
-        mol.lmp('thermo          1000')
-        mol.lmp(f'run 20000')
-
-        # Quench
-        mol.lmp('thermo          250')
-        mol.lmp(f'fix 0 all nvt temp {origin_temp} {origin_temp} 1000.0')
-        while mol.lmp.eval('temp') > origin_temp*1.05:
-            mol.lmp(f'velocity all scale {(mol.lmp.eval("temp") - origin_temp) / 2 + origin_temp}')
-            mol.lmp(f'run 2000')
-
-        if not path_writefile:
-            pwf = ptj(os.getcwd(), 'write_dump.xyz')
-            write_fmt = 'xyz'
-        else:
-            pwf = path_writefile
-            write_fmt = path_writefile.split('.')[-1]
-
-        mol.lmp(f'write_dump all {write_fmt} {pwf} modify element {" ".join(set(mol.atomic_symbols))}')
-        made_mol = ci.Molecule.read_from(pwf)
-        if not path_writefile:
-            os.remove(pwf)
-
-        made_mol.create_crystal_by_matrix(mol.lmp.cryst_matrix)
-
-        return made_mol
-
+"""
+python v3.7.9
+@Project: hotpot
+@File   : materials.py
+@Author : Zhiyuan Zhang
+@Date   : 2023/4/26
+@Time   : 1:50
+Notes:
+    This package is to perform some specific tasks base on the LAMMPS
+"""
+import os
+import os.path as osp
+from os.path import join as ptj
+from typing import *
+import math
+import random
+import numpy as np
+from scipy import spatial
+import openbabel.openbabel as ob
+import hotpot
+import hotpot.cheminfo as ci
+
+
+dir_force_field = osp.abspath(ptj(hotpot.data_root, 'force_field'))
+
+# Constants
+avogadro = 6.02214076e23  # Avogadro numbers
+angstrom = 1e-8  # cm
+
+
+class AmorphousMaker:
+    """ To make Amorphous Materials """
+    def __init__(
+            self,
+            element_composition: Dict[str, float],
+            force_field: Union[str, os.PathLike],
+            density: float = 1.0,  # g/cm^3
+            a: float = 25., b: float = 25., c: float = 25.,
+            alpha: float = 90., beta: float = 90., gamma: float = 90.,
+    ):
+        """"""
+        # Check the arguments
+        # Determine the path of force field.
+        if isinstance(force_field, os.PathLike):
+            pff = str(force_field)
+        elif osp.exists(force_field):
+            pff = force_field
+        else:
+            pff = ptj(dir_force_field, force_field)
+
+        # Make sure the existence of force field file
+        if not osp.exists(pff):
+            raise FileNotFoundError('the given force field file is not found!')
+
+        pff = osp.abspath(pff)
+
+        # assign attrs
+        sum_freq = sum(f for f in element_composition.values())
+        self.elements = {e: f/sum_freq for e, f in element_composition.items()}  # Normalize the elements' frequency
+        self.path_force_field = pff
+        self.density = density * 1.123592147466166
+        self.cryst_params = (a, b, c, alpha, beta, gamma)
+
+    @staticmethod
+    def calc_cryst_density(cryst):
+        """ Calculation the density for Crystal object """
+        return (cryst.molecule.weight * avogadro) / (cryst.volume * angstrom ** 3)  # Density, g/cm^3
+
+    @staticmethod
+    def _density2atom_numbers(ratio_elements: dict, density: float, cryst):
+        """
+        Calculate the round atom numbers in a crystal.
+        Args:
+            ratio_elements: Ratio of elements in the crystal
+            density: the demand density in the crystal
+            cryst: the crystal
+
+        Returns:
+            int, the number of atoms
+        """
+        # Convert the dict of elements and possibility to numpy array
+        elements = np.array(list(ratio_elements.keys()))
+        possibility = np.array(list(ratio_elements.values()))
+        possibility = possibility / possibility.sum()  # Normalize
+
+        average_mol_mass = sum(ob.GetMass(ob.GetAtomicNum(e)) * p for e, p in zip(elements, possibility))
+
+        # Terms:       [Mole in Crystal(Total Mass in Crystal (gram)/Average Mole Mass)]/Avogadro Number
+        # Units:           g/cm^3     angstrom^3  angstrom/cm             g/mol             _
+        num_atom = round(((density * (cryst.volume * angstrom ** 3)) / average_mol_mass) * avogadro)
+
+        # calculate the fraction coordinates in the crystal cell
+        fraction_coordinates = np.array([np.random.uniform(size=3) for _ in range(num_atom)])
+
+        # the actual coordinates in the cartesian coordinates
+        cartesian_coordinates = np.matmul(cryst.vector, fraction_coordinates.T).T
+
+        distance_matrix = spatial.distance_matrix(cartesian_coordinates, cartesian_coordinates)
+        distance_matrix = np.tril(distance_matrix, k=-1)
+        distance_matrix[distance_matrix > 0.5] = 0
+
+        # loose the closing points
+        try_number = 0
+        while distance_matrix.any() and try_number < 100:
+            points1_idx, points2_idx = rows, cols = distance_matrix.nonzero()
+
+            points1_coords = cartesian_coordinates[points1_idx]
+            points2_coords = cartesian_coordinates[points2_idx]
+
+            vector12 = points2_coords - points1_coords
+
+            e12 = vector12/np.tile(np.linalg.norm(vector12, axis=1).reshape(-1, 1), 3)
+            scalar_displace = np.tile((0.51-np.linalg.norm(vector12, axis=1)).reshape(-1, 1)/2, 3)
+
+            displacement12 = e12 * scalar_displace
+            displacement21 = -displacement12
+
+            cartesian_coordinates[points1_idx] += displacement21
+            cartesian_coordinates[points2_idx] += displacement12
+
+            distance_matrix = spatial.distance_matrix(cartesian_coordinates, cartesian_coordinates)
+            distance_matrix = np.tril(distance_matrix, k=-1)
+            distance_matrix[distance_matrix > 0.5] = 0
+
+            try_number += 1
+
+        atomic_symbols = np.random.choice(elements, num_atom, p=possibility)
+        atomic_numbers = np.array([ob.GetAtomicNum(symbol) for symbol in atomic_symbols])
+
+        return atomic_numbers, cartesian_coordinates
+
+    def load_atoms(self):
+        mol = ci.Molecule()
+        mol.make_crystal(*self.cryst_params)
+
+        cryst = mol.crystal()
+        atomic_number, coordinates = self._density2atom_numbers(
+            self.elements, self.density, cryst
+        )
+
+        mol.quick_build_atoms(atomic_number)
+        mol.set(all_coordinates=coordinates.reshape((-1, len(coordinates), 3)))
+
+        mol.conformer_select(0)
+
+        return mol
+
+    def melt_quench(
+            self, *ff_args, mol=None, path_writefile: Optional[str] = None,
+            origin_temp: float = 298.15, melt_temp: float = 4000., highest_temp: float = 10000,
+            time_step: float = 0.0001, path_dump_to: Optional[str] = None, dump_every: int = 100,
+    ):
+        """
+        Perform melt-quench process to manufacture a amorphous materials
+        Args:
+            *ff_args: the arguments the force file requried, refering the LAMMPS pair_coeff:
+             "pair_coeff I J args" url: https://docs.lammps.org/pair_coeff.html
+            mol: the molecule to be performed melt-quench. if not given, initialize according to elemental
+             compositions
+            path_writefile: the path to write the final material (screenshot) to file, if not specify, not save.
+            origin_temp: the initial temperature before melt
+            melt_temp: the round melting point to the materials
+            highest_temp: the highest temperature to liquefy the materials
+            time_step: time interval between path integrals when performing melt-quench
+            path_dump_to: the path to save the trajectory of the melt-quench process, if not specify not save
+            dump_every: the step interval between each dumps
+        Returns:
+            Molecule obj after melt-quench.
+        """
+        if not isinstance(mol, ci.Molecule):
+            mol = self.load_atoms()
+
+        mol.lmp_setup(units='metal')
+
+        # initialization
+        mol.lmp.commands_string(
+            """
+            units metal
+            dimension 3
+            atom_style full
+            """
+        )
+
+        # Read molecule into LAMMPS
+        mol.lmp.read_main_data()
+
+        # Configure the force field
+        mol.lmp("pair_style tersoff")
+        mol.lmp(f"pair_coeff * * {self.path_force_field} {' '.join(ff_args)}")
+
+        # Specify the thermodynamical output to screen
+        mol.lmp('thermo_style    custom step temp pe etotal press vol density')
+        mol.lmp('thermo          1000')
+
+        # the step interval of integral
+        mol.lmp(f'timestep {time_step}')
+
+        # Specify the dump configuration
+        if path_dump_to:
+            dump_fmt = path_dump_to.split('.')[-1]  # the dump fmt is the suffix of file name
+            mol.lmp(f'dump mq all {dump_fmt} {dump_every} {path_dump_to}')
+            mol.lmp(f'dump_modify mq element {" ".join(set(mol.atomic_symbols))}')
+
+        # Initialize the temperature for system
+        mol.lmp(f'velocity all create {origin_temp} {random.randint(100000, 999999)}')
+
+        # Melt
+        mol.lmp(f'fix 0 all nvt temp {origin_temp} {highest_temp} 0.7')
+        mol.lmp(f'run 10000')
+
+        mol.lmp(f'fix 0 all nvt temp {highest_temp} {highest_temp} 1000')
+        while mol.lmp.eval('temp') < highest_temp * 0.95:
+            mol.lmp(f'run 1000')
+
+        mol.lmp(f'run 10000')
+
+        # Relax
+        mol.lmp('thermo          250')
+        mol.lmp(f'fix 0 all nvt temp {melt_temp} {melt_temp} 1000.0')
+        while mol.lmp.eval('temp') > melt_temp * 1.05:
+            mol.lmp(f'velocity all scale {melt_temp}')
+            mol.lmp(f'run 2000')
+
+        mol.lmp('thermo          1000')
+        mol.lmp(f'run 20000')
+
+        # Quench
+        mol.lmp('thermo          250')
+        mol.lmp(f'fix 0 all nvt temp {origin_temp} {origin_temp} 1000.0')
+        while mol.lmp.eval('temp') > origin_temp*1.05:
+            mol.lmp(f'velocity all scale {(mol.lmp.eval("temp") - origin_temp) / 2 + origin_temp}')
+            mol.lmp(f'run 2000')
+
+        if not path_writefile:
+            pwf = ptj(os.getcwd(), 'write_dump.xyz')
+            write_fmt = 'xyz'
+        else:
+            pwf = path_writefile
+            write_fmt = path_writefile.split('.')[-1]
+
+        mol.lmp(f'write_dump all {write_fmt} {pwf} modify element {" ".join(set(mol.atomic_symbols))}')
+        made_mol = ci.Molecule.read_from(pwf)
+        if not path_writefile:
+            os.remove(pwf)
+
+        made_mol.create_crystal_by_matrix(mol.lmp.cryst_matrix)
+
+        return made_mol
+
```

### Comparing `hotpot-zzy-0.3.0.9/hotpot/tmo.py` & `hotpot-zzy-0.3.1.0/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/tools.py` & `hotpot-zzy-0.3.1.0/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/utils/library.py` & `hotpot-zzy-0.3.1.0/hotpot/utils/library.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/hotpot/utils/units_convert.py` & `hotpot-zzy-0.3.1.0/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.9/pyproject.toml` & `hotpot-zzy-0.3.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "hotpot-zzy"
-version = "0.3.0.9"
-readme = "RAEDME.md"
-authors = [
-    { name = "Zhiyuan Zhang", email = "ZhiyuanZhang_scu@163.com" },
-    { name = "Yue Dong", email = "1320801310@qq.com" },
-    { name = "Yuqing Qiu", email = "2022223070045@stu.scu.edu.cn" },
-]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: Unix",
-]
-dependencies = [
-    "numpy",
-    "pandas",
-    "thermo",
-    "cclib",
-    "tqdm",
-    'rdkit',
-    'psutil'
-]
-
-[tool.setuptools]
-include-package-data = true
-
-[project.urls]
-"Homepage" = "https://github.com/Zhang-Zhiyuan-zzy/hotpot"
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "hotpot-zzy"
+version = "0.3.1.0"
+readme = "RAEDME.rst"
+authors = [
+    { name = "Zhiyuan Zhang", email = "ZhiyuanZhang_scu@163.com" },
+    { name = "Yue Dong", email = "1320801310@qq.com" },
+    { name = "Yuqing Qiu", email = "2022223070045@stu.scu.edu.cn" },
+]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: Unix",
+]
+dependencies = [
+    "numpy",
+    "pandas",
+    "thermo",
+    "cclib",
+    "tqdm",
+    'rdkit',
+    'psutil'
+]
+
+description = "A python package designed to communicate among various chemical and materials calculational tools"
+
+[tool.setuptools]
+include-package-data = true
+
+[project.urls]
+"Homepage" = "https://github.com/Zhang-Zhiyuan-zzy/hotpot"
+
```

