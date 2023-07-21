# Comparing `tmp/deap-1.4.0.tar.gz` & `tmp/deap-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deap-1.4.0.tar", last modified: Thu Jul 20 00:45:33 2023, max compression
+gzip compressed data, was "deap-1.4.1.tar", last modified: Fri Jul 21 10:51:40 2023, max compression
```

## Comparing `deap-1.4.0.tar` & `deap-1.4.1.tar`

### file list

```diff
@@ -1,259 +1,271 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.063674 deap-1.4.0/
--rw-r--r--   0 runner     (501) staff       (20)      668 2023-07-20 00:45:10.000000 deap-1.4.0/INSTALL.txt
--rw-r--r--   0 runner     (501) staff       (20)     7637 2023-07-20 00:45:10.000000 deap-1.4.0/LICENSE.txt
--rw-r--r--   0 runner     (501) staff       (20)      224 2023-07-20 00:45:10.000000 deap-1.4.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    14446 2023-07-20 00:45:33.063218 deap-1.4.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    12385 2023-07-20 00:45:10.000000 deap-1.4.0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.947825 deap-1.4.0/deap/
--rw-r--r--   0 runner     (501) staff       (20)      761 2023-07-20 00:45:10.000000 deap-1.4.0/deap/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    23000 2023-07-20 00:45:10.000000 deap-1.4.0/deap/algorithms.py
--rw-r--r--   0 runner     (501) staff       (20)    14166 2023-07-20 00:45:10.000000 deap-1.4.0/deap/base.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.952930 deap-1.4.0/deap/benchmarks/
--rw-r--r--   0 runner     (501) staff       (20)    25783 2023-07-20 00:45:10.000000 deap-1.4.0/deap/benchmarks/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4862 2023-07-20 00:45:10.000000 deap-1.4.0/deap/benchmarks/binary.py
--rw-r--r--   0 runner     (501) staff       (20)     3818 2023-07-20 00:45:10.000000 deap-1.4.0/deap/benchmarks/gp.py
--rw-r--r--   0 runner     (501) staff       (20)    18385 2023-07-20 00:45:10.000000 deap-1.4.0/deap/benchmarks/movingpeaks.py
--rw-r--r--   0 runner     (501) staff       (20)    12164 2023-07-20 00:45:10.000000 deap-1.4.0/deap/benchmarks/tools.py
--rw-r--r--   0 runner     (501) staff       (20)    41817 2023-07-20 00:45:10.000000 deap-1.4.0/deap/cma.py
--rw-r--r--   0 runner     (501) staff       (20)     7186 2023-07-20 00:45:10.000000 deap-1.4.0/deap/creator.py
--rw-r--r--   0 runner     (501) staff       (20)    52405 2023-07-20 00:45:10.000000 deap-1.4.0/deap/gp.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.957799 deap-1.4.0/deap/tools/
--rw-r--r--   0 runner     (501) staff       (20)     1338 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.960349 deap-1.4.0/deap/tools/_hypervolume/
--rw-r--r--   0 runner     (501) staff       (20)      693 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/_hypervolume/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    46443 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/_hypervolume/_hv.c
--rw-r--r--   0 runner     (501) staff       (20)     2117 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/_hypervolume/_hv.h
--rw-r--r--   0 runner     (501) staff       (20)     4680 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/_hypervolume/hv.cpp
--rw-r--r--   0 runner     (501) staff       (20)    11648 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/_hypervolume/pyhv.py
--rw-r--r--   0 runner     (501) staff       (20)     7941 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/constraint.py
--rw-r--r--   0 runner     (501) staff       (20)    17311 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/crossover.py
--rw-r--r--   0 runner     (501) staff       (20)    33112 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/emo.py
--rw-r--r--   0 runner     (501) staff       (20)     1194 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/indicator.py
--rw-r--r--   0 runner     (501) staff       (20)     3283 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/init.py
--rw-r--r--   0 runner     (501) staff       (20)     2726 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/migration.py
--rw-r--r--   0 runner     (501) staff       (20)     9761 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/mutation.py
--rw-r--r--   0 runner     (501) staff       (20)    13325 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/selection.py
--rw-r--r--   0 runner     (501) staff       (20)    26498 2023-07-20 00:45:10.000000 deap-1.4.0/deap/tools/support.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.950354 deap-1.4.0/deap.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    14446 2023-07-20 00:45:32.000000 deap-1.4.0/deap.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6330 2023-07-20 00:45:32.000000 deap-1.4.0/deap.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-20 00:45:32.000000 deap-1.4.0/deap.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2023-07-20 00:45:32.000000 deap-1.4.0/deap.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        5 2023-07-20 00:45:32.000000 deap-1.4.0/deap.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.965352 deap-1.4.0/doc/
--rw-r--r--   0 runner     (501) staff       (20)     3143 2023-07-20 00:45:10.000000 deap-1.4.0/doc/Makefile
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.971079 deap-1.4.0/doc/_images/
--rw-r--r--   0 runner     (501) staff       (20)    42715 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_images/constraints.png
--rw-r--r--   0 runner     (501) staff       (20)   198299 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_images/genealogy.png
--rw-r--r--   0 runner     (501) staff       (20)    15591 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_images/gptree.png
--rw-r--r--   0 runner     (501) staff       (20)    11306 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_images/gptypederrtree.png
--rw-r--r--   0 runner     (501) staff       (20)    16637 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_images/gptypedtree.png
--rw-r--r--   0 runner     (501) staff       (20)    21744 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_images/gptypedtrees.png
--rw-r--r--   0 runner     (501) staff       (20)     1502 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_images/more.png
--rw-r--r--   0 runner     (501) staff       (20)   109712 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_images/nsga3.png
--rw-r--r--   0 runner     (501) staff       (20)    39433 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_images/twin_logbook.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.976517 deap-1.4.0/doc/_static/
--rw-r--r--   0 runner     (501) staff       (20)     2179 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/DEAP.pdf
--rw-r--r--   0 runner     (501) staff       (20)     2495 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/copybutton.js
--rw-r--r--   0 runner     (501) staff       (20)    11953 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/deap_icon-39x55.png
--rw-r--r--   0 runner     (501) staff       (20)     1150 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/deap_icon_16x16.ico
--rw-r--r--   0 runner     (501) staff       (20)    33554 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/deap_long.png
--rw-r--r--   0 runner     (501) staff       (20)     1150 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/deap_orange_icon_16x16.ico
--rw-r--r--   0 runner     (501) staff       (20)     4286 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/deap_orange_icon_32.ico
--rw-r--r--   0 runner     (501) staff       (20)   101766 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/lvsn.png
--rw-r--r--   0 runner     (501) staff       (20)     5168 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/sidebar.js
--rw-r--r--   0 runner     (501) staff       (20)     7827 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_static/ul.gif
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.977407 deap-1.4.0/doc/_templates/
--rw-r--r--   0 runner     (501) staff       (20)      526 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_templates/indexsidebar.html
--rw-r--r--   0 runner     (501) staff       (20)     1334 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_templates/layout.html
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.935650 deap-1.4.0/doc/_themes/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.977938 deap-1.4.0/doc/_themes/pydoctheme/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.978385 deap-1.4.0/doc/_themes/pydoctheme/static/
--rw-r--r--   0 runner     (501) staff       (20)     2831 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_themes/pydoctheme/static/pydoctheme.css
--rw-r--r--   0 runner     (501) staff       (20)      591 2023-07-20 00:45:10.000000 deap-1.4.0/doc/_themes/pydoctheme/theme.conf
--rw-r--r--   0 runner     (501) staff       (20)     2026 2023-07-20 00:45:10.000000 deap-1.4.0/doc/about.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.981836 deap-1.4.0/doc/api/
--rw-r--r--   0 runner     (501) staff       (20)     1632 2023-07-20 00:45:10.000000 deap-1.4.0/doc/api/algo.rst
--rw-r--r--   0 runner     (501) staff       (20)      375 2023-07-20 00:45:10.000000 deap-1.4.0/doc/api/base.rst
--rw-r--r--   0 runner     (501) staff       (20)     5302 2023-07-20 00:45:10.000000 deap-1.4.0/doc/api/benchmarks.rst
--rw-r--r--   0 runner     (501) staff       (20)      159 2023-07-20 00:45:10.000000 deap-1.4.0/doc/api/creator.rst
--rw-r--r--   0 runner     (501) staff       (20)      454 2023-07-20 00:45:10.000000 deap-1.4.0/doc/api/gp.rst
--rw-r--r--   0 runner     (501) staff       (20)      187 2023-07-20 00:45:10.000000 deap-1.4.0/doc/api/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     8665 2023-07-20 00:45:10.000000 deap-1.4.0/doc/api/tools.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.937296 deap-1.4.0/doc/code/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.990927 deap-1.4.0/doc/code/benchmarks/
--rw-r--r--   0 runner     (501) staff       (20)      686 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/ackley.py
--rw-r--r--   0 runner     (501) staff       (20)      702 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/bohachevsky.py
--rw-r--r--   0 runner     (501) staff       (20)      637 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/griewank.py
--rw-r--r--   0 runner     (501) staff       (20)      674 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/h1.py
--rw-r--r--   0 runner     (501) staff       (20)      674 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/himmelblau.py
--rw-r--r--   0 runner     (501) staff       (20)      855 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/kursawe.py
--rw-r--r--   0 runner     (501) staff       (20)      730 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/movingsc1.py
--rw-r--r--   0 runner     (501) staff       (20)      617 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/rastrigin.py
--rw-r--r--   0 runner     (501) staff       (20)      694 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/rosenbrock.py
--rw-r--r--   0 runner     (501) staff       (20)      639 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/schaffer.py
--rw-r--r--   0 runner     (501) staff       (20)      639 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/schwefel.py
--rw-r--r--   0 runner     (501) staff       (20)      879 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/benchmarks/shekel.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.992726 deap-1.4.0/doc/code/examples/
--rw-r--r--   0 runner     (501) staff       (20)      875 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/examples/nsga3_ref_points.py
--rw-r--r--   0 runner     (501) staff       (20)     1080 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/examples/nsga3_ref_points_combined.py
--rw-r--r--   0 runner     (501) staff       (20)     1086 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/examples/nsga3_ref_points_combined_plot.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.938193 deap-1.4.0/doc/code/tutorials/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.993454 deap-1.4.0/doc/code/tutorials/part_1/
--rw-r--r--   0 runner     (501) staff       (20)     2141 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_1/1_where_to_start.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.000842 deap-1.4.0/doc/code/tutorials/part_2/
--rw-r--r--   0 runner     (501) staff       (20)      220 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_1_fitness.py
--rw-r--r--   0 runner     (501) staff       (20)      617 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_2_1_list_of_floats.py
--rw-r--r--   0 runner     (501) staff       (20)      443 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_2_2_permutation.py
--rw-r--r--   0 runner     (501) staff       (20)      644 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_2_3_arithmetic_expression.py
--rw-r--r--   0 runner     (501) staff       (20)      832 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_2_4_evolution_strategy.py
--rw-r--r--   0 runner     (501) staff       (20)      679 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_2_5_particle.py
--rw-r--r--   0 runner     (501) staff       (20)      587 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_2_6_funky_one.py
--rw-r--r--   0 runner     (501) staff       (20)      535 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_3_1_bag.py
--rw-r--r--   0 runner     (501) staff       (20)      658 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_3_2_grid.py
--rw-r--r--   0 runner     (501) staff       (20)      827 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_3_3_swarm.py
--rw-r--r--   0 runner     (501) staff       (20)      585 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_3_4_demes.py
--rw-r--r--   0 runner     (501) staff       (20)      695 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/2_3_5_seeding_a_population.py
--rw-r--r--   0 runner     (501) staff       (20)       51 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_2/my_guess.json
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.005780 deap-1.4.0/doc/code/tutorials/part_3/
--rw-r--r--   0 runner     (501) staff       (20)      771 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_3/3_6_2_tool_decoration.py
--rw-r--r--   0 runner     (501) staff       (20)     1907 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_3/3_6_using_the_toolbox.py
--rw-r--r--   0 runner     (501) staff       (20)     1598 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_3/3_7_variations.py
--rw-r--r--   0 runner     (501) staff       (20)     1050 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_3/3_8_algorithms.py
--rw-r--r--   0 runner     (501) staff       (20)     1523 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_3/3_next_step.py
--rw-r--r--   0 runner     (501) staff       (20)     1407 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_3/logbook.py
--rw-r--r--   0 runner     (501) staff       (20)     1792 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_3/multistats.py
--rw-r--r--   0 runner     (501) staff       (20)     1426 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_3/stats.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.008295 deap-1.4.0/doc/code/tutorials/part_4/
--rw-r--r--   0 runner     (501) staff       (20)     4932 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_4/4_4_Using_Cpp_NSGA.py
--rw-r--r--   0 runner     (501) staff       (20)     5529 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_4/4_5_home_made_eval_func.py
--rw-r--r--   0 runner     (501) staff       (20)     6089 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_4/SNC.cpp
--rw-r--r--   0 runner     (501) staff       (20)      244 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_4/installSN.py
--rw-r--r--   0 runner     (501) staff       (20)     4640 2023-07-20 00:45:10.000000 deap-1.4.0/doc/code/tutorials/part_4/sortingnetwork.py
--rw-r--r--   0 runner     (501) staff       (20)     8151 2023-07-20 00:45:10.000000 deap-1.4.0/doc/conf.py
--rw-r--r--   0 runner     (501) staff       (20)     2477 2023-07-20 00:45:10.000000 deap-1.4.0/doc/contributing.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.019492 deap-1.4.0/doc/examples/
--rw-r--r--   0 runner     (501) staff       (20)     2127 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/bipop_cmaes.rst
--rw-r--r--   0 runner     (501) staff       (20)     1479 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/cmaes.rst
--rw-r--r--   0 runner     (501) staff       (20)     2579 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/cmaes_plotting.rst
--rw-r--r--   0 runner     (501) staff       (20)     2931 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/coev_coop.rst
--rw-r--r--   0 runner     (501) staff       (20)     2297 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/eda.rst
--rw-r--r--   0 runner     (501) staff       (20)     2425 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/es_fctmin.rst
--rw-r--r--   0 runner     (501) staff       (20)      138 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/es_onefifth.rst
--rw-r--r--   0 runner     (501) staff       (20)     3043 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/ga_knapsack.rst
--rw-r--r--   0 runner     (501) staff       (20)    10293 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/ga_onemax.rst
--rw-r--r--   0 runner     (501) staff       (20)     1036 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/ga_onemax_numpy.rst
--rw-r--r--   0 runner     (501) staff       (20)     1559 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/ga_onemax_short.rst
--rw-r--r--   0 runner     (501) staff       (20)     3127 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/gp_ant.rst
--rw-r--r--   0 runner     (501) staff       (20)     1829 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/gp_multiplexer.rst
--rw-r--r--   0 runner     (501) staff       (20)     2047 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/gp_parity.rst
--rw-r--r--   0 runner     (501) staff       (20)     3443 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/gp_spambase.rst
--rw-r--r--   0 runner     (501) staff       (20)     7033 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/gp_symbreg.rst
--rw-r--r--   0 runner     (501) staff       (20)     1046 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     4391 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/nsga3.rst
--rw-r--r--   0 runner     (501) staff       (20)     4847 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/pso_basic.rst
--rw-r--r--   0 runner     (501) staff       (20)     3093 2023-07-20 00:45:10.000000 deap-1.4.0/doc/examples/pso_multiswarm.rst
--rw-r--r--   0 runner     (501) staff       (20)     1986 2023-07-20 00:45:10.000000 deap-1.4.0/doc/index.rst
--rw-r--r--   0 runner     (501) staff       (20)      962 2023-07-20 00:45:10.000000 deap-1.4.0/doc/installation.rst
--rw-r--r--   0 runner     (501) staff       (20)     3581 2023-07-20 00:45:10.000000 deap-1.4.0/doc/overview.rst
--rw-r--r--   0 runner     (501) staff       (20)       32 2023-07-20 00:45:10.000000 deap-1.4.0/doc/pip_req.txt
--rw-r--r--   0 runner     (501) staff       (20)     3453 2023-07-20 00:45:10.000000 deap-1.4.0/doc/porting.rst
--rw-r--r--   0 runner     (501) staff       (20)     5534 2023-07-20 00:45:10.000000 deap-1.4.0/doc/releases.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:32.938982 deap-1.4.0/doc/tutorials/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.022083 deap-1.4.0/doc/tutorials/advanced/
--rw-r--r--   0 runner     (501) staff       (20)     2934 2023-07-20 00:45:10.000000 deap-1.4.0/doc/tutorials/advanced/benchmarking.rst
--rw-r--r--   0 runner     (501) staff       (20)     3389 2023-07-20 00:45:10.000000 deap-1.4.0/doc/tutorials/advanced/checkpoint.rst
--rw-r--r--   0 runner     (501) staff       (20)     3435 2023-07-20 00:45:10.000000 deap-1.4.0/doc/tutorials/advanced/constraints.rst
--rw-r--r--   0 runner     (501) staff       (20)    12053 2023-07-20 00:45:10.000000 deap-1.4.0/doc/tutorials/advanced/gp.rst
--rw-r--r--   0 runner     (501) staff       (20)     4153 2023-07-20 00:45:10.000000 deap-1.4.0/doc/tutorials/advanced/numpy.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.024242 deap-1.4.0/doc/tutorials/basic/
--rw-r--r--   0 runner     (501) staff       (20)    13177 2023-07-20 00:45:10.000000 deap-1.4.0/doc/tutorials/basic/part1.rst
--rw-r--r--   0 runner     (501) staff       (20)    10986 2023-07-20 00:45:10.000000 deap-1.4.0/doc/tutorials/basic/part2.rst
--rw-r--r--   0 runner     (501) staff       (20)     9635 2023-07-20 00:45:10.000000 deap-1.4.0/doc/tutorials/basic/part3.rst
--rw-r--r--   0 runner     (501) staff       (20)     5365 2023-07-20 00:45:10.000000 deap-1.4.0/doc/tutorials/basic/part4.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.025284 deap-1.4.0/examples/
--rw-r--r--   0 runner     (501) staff       (20)     5041 2023-07-20 00:45:10.000000 deap-1.4.0/examples/bbob.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.028691 deap-1.4.0/examples/coev/
--rw-r--r--   0 runner     (501) staff       (20)     4952 2023-07-20 00:45:10.000000 deap-1.4.0/examples/coev/coop_adapt.py
--rw-r--r--   0 runner     (501) staff       (20)     3822 2023-07-20 00:45:10.000000 deap-1.4.0/examples/coev/coop_base.py
--rw-r--r--   0 runner     (501) staff       (20)     6150 2023-07-20 00:45:10.000000 deap-1.4.0/examples/coev/coop_evol.py
--rw-r--r--   0 runner     (501) staff       (20)     4762 2023-07-20 00:45:10.000000 deap-1.4.0/examples/coev/coop_gen.py
--rw-r--r--   0 runner     (501) staff       (20)     3365 2023-07-20 00:45:10.000000 deap-1.4.0/examples/coev/coop_niche.py
--rw-r--r--   0 runner     (501) staff       (20)     5679 2023-07-20 00:45:10.000000 deap-1.4.0/examples/coev/hillis.py
--rw-r--r--   0 runner     (501) staff       (20)     4542 2023-07-20 00:45:10.000000 deap-1.4.0/examples/coev/symbreg.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.030150 deap-1.4.0/examples/de/
--rw-r--r--   0 runner     (501) staff       (20)     2816 2023-07-20 00:45:10.000000 deap-1.4.0/examples/de/basic.py
--rw-r--r--   0 runner     (501) staff       (20)     5807 2023-07-20 00:45:10.000000 deap-1.4.0/examples/de/dynamic.py
--rw-r--r--   0 runner     (501) staff       (20)     3767 2023-07-20 00:45:10.000000 deap-1.4.0/examples/de/sphere.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.031030 deap-1.4.0/examples/eda/
--rw-r--r--   0 runner     (501) staff       (20)     3411 2023-07-20 00:45:10.000000 deap-1.4.0/examples/eda/emna.py
--rw-r--r--   0 runner     (501) staff       (20)     2789 2023-07-20 00:45:10.000000 deap-1.4.0/examples/eda/pbil.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.034362 deap-1.4.0/examples/es/
--rw-r--r--   0 runner     (501) staff       (20)     1996 2023-07-20 00:45:10.000000 deap-1.4.0/examples/es/cma_1+l_minfct.py
--rw-r--r--   0 runner     (501) staff       (20)     8278 2023-07-20 00:45:10.000000 deap-1.4.0/examples/es/cma_bipop.py
--rw-r--r--   0 runner     (501) staff       (20)     2164 2023-07-20 00:45:10.000000 deap-1.4.0/examples/es/cma_minfct.py
--rw-r--r--   0 runner     (501) staff       (20)     5978 2023-07-20 00:45:10.000000 deap-1.4.0/examples/es/cma_mo.py
--rw-r--r--   0 runner     (501) staff       (20)     4286 2023-07-20 00:45:10.000000 deap-1.4.0/examples/es/cma_plotting.py
--rw-r--r--   0 runner     (501) staff       (20)     2928 2023-07-20 00:45:10.000000 deap-1.4.0/examples/es/fctmin.py
--rw-r--r--   0 runner     (501) staff       (20)     2770 2023-07-20 00:45:10.000000 deap-1.4.0/examples/es/onefifth.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.045566 deap-1.4.0/examples/ga/
--rwxr-xr-x   0 runner     (501) staff       (20)     2905 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/evoknn.py
--rw-r--r--   0 runner     (501) staff       (20)     1929 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/evoknn_jmlr.py
--rw-r--r--   0 runner     (501) staff       (20)     4982 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/evosn.py
--rw-r--r--   0 runner     (501) staff       (20)    24180 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/heart_scale.csv
--rw-r--r--   0 runner     (501) staff       (20)     3564 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/knapsack.py
--rw-r--r--   0 runner     (501) staff       (20)     3438 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/knn.py
--rw-r--r--   0 runner     (501) staff       (20)     2940 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/kursawefct.py
--rw-r--r--   0 runner     (501) staff       (20)     7038 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/mo_rhv.py
--rw-r--r--   0 runner     (501) staff       (20)     3343 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/nqueens.py
--rw-r--r--   0 runner     (501) staff       (20)     5160 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/nsga2.py
--rw-r--r--   0 runner     (501) staff       (20)     4200 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/nsga3.py
--rw-r--r--   0 runner     (501) staff       (20)     5307 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/onemax.py
--rw-r--r--   0 runner     (501) staff       (20)     5253 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/onemax_island.py
--rw-r--r--   0 runner     (501) staff       (20)     2336 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/onemax_island_scoop.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2353 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/onemax_mp.py
--rw-r--r--   0 runner     (501) staff       (20)     3148 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/onemax_multidemic.py
--rw-r--r--   0 runner     (501) staff       (20)     3166 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/onemax_numpy.py
--rw-r--r--   0 runner     (501) staff       (20)     2067 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/onemax_short.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.050270 deap-1.4.0/examples/ga/pareto_front/
--rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/pareto_front/dtlz1_front.json
--rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/pareto_front/dtlz2_front.json
--rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/pareto_front/dtlz3_front.json
--rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/pareto_front/dtlz4_front.json
--rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/pareto_front/zdt1_front.json
--rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/pareto_front/zdt2_front.json
--rw-r--r--   0 runner     (501) staff       (20)    29340 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/pareto_front/zdt3_front.json
--rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/pareto_front/zdt4_front.json
--rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/pareto_front/zdt6_front.json
--rw-r--r--   0 runner     (501) staff       (20)     4361 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/sortingnetwork.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.051882 deap-1.4.0/examples/ga/tsp/
--rw-r--r--   0 runner     (501) staff       (20)    72474 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/tsp/gr120.json
--rw-r--r--   0 runner     (501) staff       (20)     1603 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/tsp/gr17.json
--rw-r--r--   0 runner     (501) staff       (20)     2965 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/tsp/gr24.json
--rw-r--r--   0 runner     (501) staff       (20)     2494 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/tsp.py
--rw-r--r--   0 runner     (501) staff       (20)     4336 2023-07-20 00:45:10.000000 deap-1.4.0/examples/ga/xkcd.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.058670 deap-1.4.0/examples/gp/
--rw-r--r--   0 runner     (501) staff       (20)      692 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6220 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/adf_symbreg.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.060476 deap-1.4.0/examples/gp/ant/
--rw-r--r--   0 runner     (501) staff       (20)    11532 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/ant/AntSimulatorFast.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1736 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/ant/AntSimulatorFast.hpp
--rw-r--r--   0 runner     (501) staff       (20)      308 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/ant/buildAntSimFast.py
--rw-r--r--   0 runner     (501) staff       (20)     1057 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/ant/santafe_trail.txt
--rw-r--r--   0 runner     (501) staff       (20)     6864 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/ant.py
--rw-r--r--   0 runner     (501) staff       (20)     3295 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/multiplexer.py
--rw-r--r--   0 runner     (501) staff       (20)     2949 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/parity.py
--rw-r--r--   0 runner     (501) staff       (20)   702942 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/spambase.csv
--rw-r--r--   0 runner     (501) staff       (20)     4043 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/spambase.py
--rw-r--r--   0 runner     (501) staff       (20)     3374 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/symbreg.py
--rw-r--r--   0 runner     (501) staff       (20)     3343 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/symbreg_epsilon_lexicase.py
--rw-r--r--   0 runner     (501) staff       (20)     3371 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/symbreg_harm.py
--rw-r--r--   0 runner     (501) staff       (20)     3289 2023-07-20 00:45:10.000000 deap-1.4.0/examples/gp/symbreg_numpy.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 00:45:33.062363 deap-1.4.0/examples/pso/
--rw-r--r--   0 runner     (501) staff       (20)     3352 2023-07-20 00:45:10.000000 deap-1.4.0/examples/pso/basic.py
--rw-r--r--   0 runner     (501) staff       (20)     3160 2023-07-20 00:45:10.000000 deap-1.4.0/examples/pso/basic_numpy.py
--rw-r--r--   0 runner     (501) staff       (20)     9309 2023-07-20 00:45:10.000000 deap-1.4.0/examples/pso/multiswarm.py
--rw-r--r--   0 runner     (501) staff       (20)     6580 2023-07-20 00:45:10.000000 deap-1.4.0/examples/pso/speciation.py
--rw-r--r--   0 runner     (501) staff       (20)      508 2023-07-20 00:45:10.000000 deap-1.4.0/examples/speed.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-20 00:45:33.063794 deap-1.4.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3818 2023-07-20 00:45:10.000000 deap-1.4.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.740156 deap-1.4.1/
+-rw-r--r--   0 runner     (501) staff       (20)      668 2023-07-21 10:51:13.000000 deap-1.4.1/INSTALL.txt
+-rw-r--r--   0 runner     (501) staff       (20)     7637 2023-07-21 10:51:13.000000 deap-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner     (501) staff       (20)      250 2023-07-21 10:51:13.000000 deap-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    13235 2023-07-21 10:51:40.739695 deap-1.4.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    12385 2023-07-21 10:51:13.000000 deap-1.4.1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.624471 deap-1.4.1/deap/
+-rw-r--r--   0 runner     (501) staff       (20)      761 2023-07-21 10:51:13.000000 deap-1.4.1/deap/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    23000 2023-07-21 10:51:13.000000 deap-1.4.1/deap/algorithms.py
+-rw-r--r--   0 runner     (501) staff       (20)    14166 2023-07-21 10:51:13.000000 deap-1.4.1/deap/base.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.630304 deap-1.4.1/deap/benchmarks/
+-rw-r--r--   0 runner     (501) staff       (20)    25783 2023-07-21 10:51:13.000000 deap-1.4.1/deap/benchmarks/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4862 2023-07-21 10:51:13.000000 deap-1.4.1/deap/benchmarks/binary.py
+-rw-r--r--   0 runner     (501) staff       (20)     3818 2023-07-21 10:51:13.000000 deap-1.4.1/deap/benchmarks/gp.py
+-rw-r--r--   0 runner     (501) staff       (20)    18385 2023-07-21 10:51:13.000000 deap-1.4.1/deap/benchmarks/movingpeaks.py
+-rw-r--r--   0 runner     (501) staff       (20)    12164 2023-07-21 10:51:13.000000 deap-1.4.1/deap/benchmarks/tools.py
+-rw-r--r--   0 runner     (501) staff       (20)    41817 2023-07-21 10:51:13.000000 deap-1.4.1/deap/cma.py
+-rw-r--r--   0 runner     (501) staff       (20)     7186 2023-07-21 10:51:13.000000 deap-1.4.1/deap/creator.py
+-rw-r--r--   0 runner     (501) staff       (20)    52405 2023-07-21 10:51:13.000000 deap-1.4.1/deap/gp.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.636043 deap-1.4.1/deap/tools/
+-rw-r--r--   0 runner     (501) staff       (20)     1338 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.638874 deap-1.4.1/deap/tools/_hypervolume/
+-rw-r--r--   0 runner     (501) staff       (20)      693 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/_hypervolume/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    46443 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/_hypervolume/_hv.c
+-rw-r--r--   0 runner     (501) staff       (20)     2117 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/_hypervolume/_hv.h
+-rw-r--r--   0 runner     (501) staff       (20)     4680 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/_hypervolume/hv.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    11648 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/_hypervolume/pyhv.py
+-rw-r--r--   0 runner     (501) staff       (20)     7941 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/constraint.py
+-rw-r--r--   0 runner     (501) staff       (20)    17311 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/crossover.py
+-rw-r--r--   0 runner     (501) staff       (20)    33112 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/emo.py
+-rw-r--r--   0 runner     (501) staff       (20)     1194 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/indicator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3283 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/init.py
+-rw-r--r--   0 runner     (501) staff       (20)     2726 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/migration.py
+-rw-r--r--   0 runner     (501) staff       (20)     9761 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/mutation.py
+-rw-r--r--   0 runner     (501) staff       (20)    13325 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/selection.py
+-rw-r--r--   0 runner     (501) staff       (20)    26498 2023-07-21 10:51:13.000000 deap-1.4.1/deap/tools/support.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.627589 deap-1.4.1/deap.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    13235 2023-07-21 10:51:40.000000 deap-1.4.1/deap.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6586 2023-07-21 10:51:40.000000 deap-1.4.1/deap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-21 10:51:40.000000 deap-1.4.1/deap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2023-07-21 10:51:40.000000 deap-1.4.1/deap.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        5 2023-07-21 10:51:40.000000 deap-1.4.1/deap.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.644087 deap-1.4.1/doc/
+-rw-r--r--   0 runner     (501) staff       (20)     3143 2023-07-21 10:51:13.000000 deap-1.4.1/doc/Makefile
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.650048 deap-1.4.1/doc/_images/
+-rw-r--r--   0 runner     (501) staff       (20)    42715 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_images/constraints.png
+-rw-r--r--   0 runner     (501) staff       (20)   198299 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_images/genealogy.png
+-rw-r--r--   0 runner     (501) staff       (20)    15591 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_images/gptree.png
+-rw-r--r--   0 runner     (501) staff       (20)    11306 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_images/gptypederrtree.png
+-rw-r--r--   0 runner     (501) staff       (20)    16637 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_images/gptypedtree.png
+-rw-r--r--   0 runner     (501) staff       (20)    21744 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_images/gptypedtrees.png
+-rw-r--r--   0 runner     (501) staff       (20)     1502 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_images/more.png
+-rw-r--r--   0 runner     (501) staff       (20)   109712 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_images/nsga3.png
+-rw-r--r--   0 runner     (501) staff       (20)    39433 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_images/twin_logbook.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.655333 deap-1.4.1/doc/_static/
+-rw-r--r--   0 runner     (501) staff       (20)     2179 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/DEAP.pdf
+-rw-r--r--   0 runner     (501) staff       (20)     2495 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/copybutton.js
+-rw-r--r--   0 runner     (501) staff       (20)    11953 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/deap_icon-39x55.png
+-rw-r--r--   0 runner     (501) staff       (20)     1150 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/deap_icon_16x16.ico
+-rw-r--r--   0 runner     (501) staff       (20)    33554 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/deap_long.png
+-rw-r--r--   0 runner     (501) staff       (20)     1150 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/deap_orange_icon_16x16.ico
+-rw-r--r--   0 runner     (501) staff       (20)     4286 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/deap_orange_icon_32.ico
+-rw-r--r--   0 runner     (501) staff       (20)   101766 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/lvsn.png
+-rw-r--r--   0 runner     (501) staff       (20)     5168 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/sidebar.js
+-rw-r--r--   0 runner     (501) staff       (20)     7827 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_static/ul.gif
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.656399 deap-1.4.1/doc/_templates/
+-rw-r--r--   0 runner     (501) staff       (20)      526 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_templates/indexsidebar.html
+-rw-r--r--   0 runner     (501) staff       (20)     1334 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_templates/layout.html
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.612458 deap-1.4.1/doc/_themes/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.656891 deap-1.4.1/doc/_themes/pydoctheme/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.657385 deap-1.4.1/doc/_themes/pydoctheme/static/
+-rw-r--r--   0 runner     (501) staff       (20)     2831 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_themes/pydoctheme/static/pydoctheme.css
+-rw-r--r--   0 runner     (501) staff       (20)      591 2023-07-21 10:51:13.000000 deap-1.4.1/doc/_themes/pydoctheme/theme.conf
+-rw-r--r--   0 runner     (501) staff       (20)     2026 2023-07-21 10:51:13.000000 deap-1.4.1/doc/about.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.660870 deap-1.4.1/doc/api/
+-rw-r--r--   0 runner     (501) staff       (20)     1632 2023-07-21 10:51:13.000000 deap-1.4.1/doc/api/algo.rst
+-rw-r--r--   0 runner     (501) staff       (20)      375 2023-07-21 10:51:13.000000 deap-1.4.1/doc/api/base.rst
+-rw-r--r--   0 runner     (501) staff       (20)     5302 2023-07-21 10:51:13.000000 deap-1.4.1/doc/api/benchmarks.rst
+-rw-r--r--   0 runner     (501) staff       (20)      159 2023-07-21 10:51:13.000000 deap-1.4.1/doc/api/creator.rst
+-rw-r--r--   0 runner     (501) staff       (20)      454 2023-07-21 10:51:13.000000 deap-1.4.1/doc/api/gp.rst
+-rw-r--r--   0 runner     (501) staff       (20)      187 2023-07-21 10:51:13.000000 deap-1.4.1/doc/api/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)     8665 2023-07-21 10:51:13.000000 deap-1.4.1/doc/api/tools.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.613844 deap-1.4.1/doc/code/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.666996 deap-1.4.1/doc/code/benchmarks/
+-rw-r--r--   0 runner     (501) staff       (20)      686 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/ackley.py
+-rw-r--r--   0 runner     (501) staff       (20)      702 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/bohachevsky.py
+-rw-r--r--   0 runner     (501) staff       (20)      637 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/griewank.py
+-rw-r--r--   0 runner     (501) staff       (20)      674 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/h1.py
+-rw-r--r--   0 runner     (501) staff       (20)      674 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/himmelblau.py
+-rw-r--r--   0 runner     (501) staff       (20)      855 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/kursawe.py
+-rw-r--r--   0 runner     (501) staff       (20)      730 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/movingsc1.py
+-rw-r--r--   0 runner     (501) staff       (20)      617 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/rastrigin.py
+-rw-r--r--   0 runner     (501) staff       (20)      694 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/rosenbrock.py
+-rw-r--r--   0 runner     (501) staff       (20)      639 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/schaffer.py
+-rw-r--r--   0 runner     (501) staff       (20)      639 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/schwefel.py
+-rw-r--r--   0 runner     (501) staff       (20)      879 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/benchmarks/shekel.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.668326 deap-1.4.1/doc/code/examples/
+-rw-r--r--   0 runner     (501) staff       (20)      875 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/examples/nsga3_ref_points.py
+-rw-r--r--   0 runner     (501) staff       (20)     1080 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/examples/nsga3_ref_points_combined.py
+-rw-r--r--   0 runner     (501) staff       (20)     1086 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/examples/nsga3_ref_points_combined_plot.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.614685 deap-1.4.1/doc/code/tutorials/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.668840 deap-1.4.1/doc/code/tutorials/part_1/
+-rw-r--r--   0 runner     (501) staff       (20)     2141 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_1/1_where_to_start.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.675140 deap-1.4.1/doc/code/tutorials/part_2/
+-rw-r--r--   0 runner     (501) staff       (20)      220 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_1_fitness.py
+-rw-r--r--   0 runner     (501) staff       (20)      617 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_2_1_list_of_floats.py
+-rw-r--r--   0 runner     (501) staff       (20)      443 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_2_2_permutation.py
+-rw-r--r--   0 runner     (501) staff       (20)      644 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_2_3_arithmetic_expression.py
+-rw-r--r--   0 runner     (501) staff       (20)      832 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_2_4_evolution_strategy.py
+-rw-r--r--   0 runner     (501) staff       (20)      679 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_2_5_particle.py
+-rw-r--r--   0 runner     (501) staff       (20)      587 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_2_6_funky_one.py
+-rw-r--r--   0 runner     (501) staff       (20)      535 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_3_1_bag.py
+-rw-r--r--   0 runner     (501) staff       (20)      658 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_3_2_grid.py
+-rw-r--r--   0 runner     (501) staff       (20)      827 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_3_3_swarm.py
+-rw-r--r--   0 runner     (501) staff       (20)      585 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_3_4_demes.py
+-rw-r--r--   0 runner     (501) staff       (20)      695 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/2_3_5_seeding_a_population.py
+-rw-r--r--   0 runner     (501) staff       (20)       51 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_2/my_guess.json
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.679048 deap-1.4.1/doc/code/tutorials/part_3/
+-rw-r--r--   0 runner     (501) staff       (20)      771 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_3/3_6_2_tool_decoration.py
+-rw-r--r--   0 runner     (501) staff       (20)     1907 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_3/3_6_using_the_toolbox.py
+-rw-r--r--   0 runner     (501) staff       (20)     1598 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_3/3_7_variations.py
+-rw-r--r--   0 runner     (501) staff       (20)     1050 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_3/3_8_algorithms.py
+-rw-r--r--   0 runner     (501) staff       (20)     1523 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_3/3_next_step.py
+-rw-r--r--   0 runner     (501) staff       (20)     1407 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_3/logbook.py
+-rw-r--r--   0 runner     (501) staff       (20)     1792 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_3/multistats.py
+-rw-r--r--   0 runner     (501) staff       (20)     1426 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_3/stats.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.681612 deap-1.4.1/doc/code/tutorials/part_4/
+-rw-r--r--   0 runner     (501) staff       (20)     4932 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_4/4_4_Using_Cpp_NSGA.py
+-rw-r--r--   0 runner     (501) staff       (20)     5529 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_4/4_5_home_made_eval_func.py
+-rw-r--r--   0 runner     (501) staff       (20)     6089 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_4/SNC.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      244 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_4/installSN.py
+-rw-r--r--   0 runner     (501) staff       (20)     4640 2023-07-21 10:51:13.000000 deap-1.4.1/doc/code/tutorials/part_4/sortingnetwork.py
+-rw-r--r--   0 runner     (501) staff       (20)     8151 2023-07-21 10:51:13.000000 deap-1.4.1/doc/conf.py
+-rw-r--r--   0 runner     (501) staff       (20)     2477 2023-07-21 10:51:13.000000 deap-1.4.1/doc/contributing.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.691256 deap-1.4.1/doc/examples/
+-rw-r--r--   0 runner     (501) staff       (20)     2127 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/bipop_cmaes.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1479 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/cmaes.rst
+-rw-r--r--   0 runner     (501) staff       (20)     2579 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/cmaes_plotting.rst
+-rw-r--r--   0 runner     (501) staff       (20)     2931 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/coev_coop.rst
+-rw-r--r--   0 runner     (501) staff       (20)     2297 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/eda.rst
+-rw-r--r--   0 runner     (501) staff       (20)     2425 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/es_fctmin.rst
+-rw-r--r--   0 runner     (501) staff       (20)      138 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/es_onefifth.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3043 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/ga_knapsack.rst
+-rw-r--r--   0 runner     (501) staff       (20)    10293 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/ga_onemax.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1036 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/ga_onemax_numpy.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1559 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/ga_onemax_short.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3127 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/gp_ant.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1829 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/gp_multiplexer.rst
+-rw-r--r--   0 runner     (501) staff       (20)     2047 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/gp_parity.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3443 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/gp_spambase.rst
+-rw-r--r--   0 runner     (501) staff       (20)     7033 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/gp_symbreg.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1046 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4391 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/nsga3.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4847 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/pso_basic.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3093 2023-07-21 10:51:13.000000 deap-1.4.1/doc/examples/pso_multiswarm.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1986 2023-07-21 10:51:13.000000 deap-1.4.1/doc/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)      962 2023-07-21 10:51:13.000000 deap-1.4.1/doc/installation.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3581 2023-07-21 10:51:13.000000 deap-1.4.1/doc/overview.rst
+-rw-r--r--   0 runner     (501) staff       (20)       32 2023-07-21 10:51:13.000000 deap-1.4.1/doc/pip_req.txt
+-rw-r--r--   0 runner     (501) staff       (20)     3453 2023-07-21 10:51:13.000000 deap-1.4.1/doc/porting.rst
+-rw-r--r--   0 runner     (501) staff       (20)     5534 2023-07-21 10:51:13.000000 deap-1.4.1/doc/releases.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.615518 deap-1.4.1/doc/tutorials/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.693617 deap-1.4.1/doc/tutorials/advanced/
+-rw-r--r--   0 runner     (501) staff       (20)     2934 2023-07-21 10:51:13.000000 deap-1.4.1/doc/tutorials/advanced/benchmarking.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3389 2023-07-21 10:51:13.000000 deap-1.4.1/doc/tutorials/advanced/checkpoint.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3435 2023-07-21 10:51:13.000000 deap-1.4.1/doc/tutorials/advanced/constraints.rst
+-rw-r--r--   0 runner     (501) staff       (20)    12053 2023-07-21 10:51:13.000000 deap-1.4.1/doc/tutorials/advanced/gp.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4153 2023-07-21 10:51:13.000000 deap-1.4.1/doc/tutorials/advanced/numpy.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.695392 deap-1.4.1/doc/tutorials/basic/
+-rw-r--r--   0 runner     (501) staff       (20)    13170 2023-07-21 10:51:13.000000 deap-1.4.1/doc/tutorials/basic/part1.rst
+-rw-r--r--   0 runner     (501) staff       (20)    10986 2023-07-21 10:51:13.000000 deap-1.4.1/doc/tutorials/basic/part2.rst
+-rw-r--r--   0 runner     (501) staff       (20)     9635 2023-07-21 10:51:13.000000 deap-1.4.1/doc/tutorials/basic/part3.rst
+-rw-r--r--   0 runner     (501) staff       (20)     5365 2023-07-21 10:51:13.000000 deap-1.4.1/doc/tutorials/basic/part4.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.696318 deap-1.4.1/examples/
+-rw-r--r--   0 runner     (501) staff       (20)     5041 2023-07-21 10:51:13.000000 deap-1.4.1/examples/bbob.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.699743 deap-1.4.1/examples/coev/
+-rw-r--r--   0 runner     (501) staff       (20)     4952 2023-07-21 10:51:13.000000 deap-1.4.1/examples/coev/coop_adapt.py
+-rw-r--r--   0 runner     (501) staff       (20)     3822 2023-07-21 10:51:13.000000 deap-1.4.1/examples/coev/coop_base.py
+-rw-r--r--   0 runner     (501) staff       (20)     6150 2023-07-21 10:51:13.000000 deap-1.4.1/examples/coev/coop_evol.py
+-rw-r--r--   0 runner     (501) staff       (20)     4762 2023-07-21 10:51:13.000000 deap-1.4.1/examples/coev/coop_gen.py
+-rw-r--r--   0 runner     (501) staff       (20)     3365 2023-07-21 10:51:13.000000 deap-1.4.1/examples/coev/coop_niche.py
+-rw-r--r--   0 runner     (501) staff       (20)     5679 2023-07-21 10:51:13.000000 deap-1.4.1/examples/coev/hillis.py
+-rw-r--r--   0 runner     (501) staff       (20)     4542 2023-07-21 10:51:13.000000 deap-1.4.1/examples/coev/symbreg.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.701445 deap-1.4.1/examples/de/
+-rw-r--r--   0 runner     (501) staff       (20)     2816 2023-07-21 10:51:13.000000 deap-1.4.1/examples/de/basic.py
+-rw-r--r--   0 runner     (501) staff       (20)     5807 2023-07-21 10:51:13.000000 deap-1.4.1/examples/de/dynamic.py
+-rw-r--r--   0 runner     (501) staff       (20)     3767 2023-07-21 10:51:13.000000 deap-1.4.1/examples/de/sphere.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.702584 deap-1.4.1/examples/eda/
+-rw-r--r--   0 runner     (501) staff       (20)     3411 2023-07-21 10:51:13.000000 deap-1.4.1/examples/eda/emna.py
+-rw-r--r--   0 runner     (501) staff       (20)     2789 2023-07-21 10:51:13.000000 deap-1.4.1/examples/eda/pbil.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.705889 deap-1.4.1/examples/es/
+-rw-r--r--   0 runner     (501) staff       (20)     1996 2023-07-21 10:51:13.000000 deap-1.4.1/examples/es/cma_1+l_minfct.py
+-rw-r--r--   0 runner     (501) staff       (20)     8278 2023-07-21 10:51:13.000000 deap-1.4.1/examples/es/cma_bipop.py
+-rw-r--r--   0 runner     (501) staff       (20)     2164 2023-07-21 10:51:13.000000 deap-1.4.1/examples/es/cma_minfct.py
+-rw-r--r--   0 runner     (501) staff       (20)     5978 2023-07-21 10:51:13.000000 deap-1.4.1/examples/es/cma_mo.py
+-rw-r--r--   0 runner     (501) staff       (20)     4286 2023-07-21 10:51:13.000000 deap-1.4.1/examples/es/cma_plotting.py
+-rw-r--r--   0 runner     (501) staff       (20)     2928 2023-07-21 10:51:13.000000 deap-1.4.1/examples/es/fctmin.py
+-rw-r--r--   0 runner     (501) staff       (20)     2770 2023-07-21 10:51:13.000000 deap-1.4.1/examples/es/onefifth.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.716613 deap-1.4.1/examples/ga/
+-rwxr-xr-x   0 runner     (501) staff       (20)     2905 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/evoknn.py
+-rw-r--r--   0 runner     (501) staff       (20)     1929 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/evoknn_jmlr.py
+-rw-r--r--   0 runner     (501) staff       (20)     4982 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/evosn.py
+-rw-r--r--   0 runner     (501) staff       (20)    24180 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/heart_scale.csv
+-rw-r--r--   0 runner     (501) staff       (20)     3564 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/knapsack.py
+-rw-r--r--   0 runner     (501) staff       (20)     3438 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/knn.py
+-rw-r--r--   0 runner     (501) staff       (20)     2940 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/kursawefct.py
+-rw-r--r--   0 runner     (501) staff       (20)     7038 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/mo_rhv.py
+-rw-r--r--   0 runner     (501) staff       (20)     3343 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/nqueens.py
+-rw-r--r--   0 runner     (501) staff       (20)     5160 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/nsga2.py
+-rw-r--r--   0 runner     (501) staff       (20)     4200 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/nsga3.py
+-rw-r--r--   0 runner     (501) staff       (20)     5307 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/onemax.py
+-rw-r--r--   0 runner     (501) staff       (20)     5253 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/onemax_island.py
+-rw-r--r--   0 runner     (501) staff       (20)     2336 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/onemax_island_scoop.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2353 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/onemax_mp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3148 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/onemax_multidemic.py
+-rw-r--r--   0 runner     (501) staff       (20)     3166 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/onemax_numpy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2067 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/onemax_short.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.721704 deap-1.4.1/examples/ga/pareto_front/
+-rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/pareto_front/dtlz1_front.json
+-rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/pareto_front/dtlz2_front.json
+-rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/pareto_front/dtlz3_front.json
+-rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/pareto_front/dtlz4_front.json
+-rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/pareto_front/zdt1_front.json
+-rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/pareto_front/zdt2_front.json
+-rw-r--r--   0 runner     (501) staff       (20)    29340 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/pareto_front/zdt3_front.json
+-rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/pareto_front/zdt4_front.json
+-rw-r--r--   0 runner     (501) staff       (20)    29000 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/pareto_front/zdt6_front.json
+-rw-r--r--   0 runner     (501) staff       (20)     4361 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/sortingnetwork.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.723445 deap-1.4.1/examples/ga/tsp/
+-rw-r--r--   0 runner     (501) staff       (20)    72474 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/tsp/gr120.json
+-rw-r--r--   0 runner     (501) staff       (20)     1603 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/tsp/gr17.json
+-rw-r--r--   0 runner     (501) staff       (20)     2965 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/tsp/gr24.json
+-rw-r--r--   0 runner     (501) staff       (20)     2494 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/tsp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4336 2023-07-21 10:51:13.000000 deap-1.4.1/examples/ga/xkcd.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.730371 deap-1.4.1/examples/gp/
+-rw-r--r--   0 runner     (501) staff       (20)      692 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6220 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/adf_symbreg.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.732220 deap-1.4.1/examples/gp/ant/
+-rw-r--r--   0 runner     (501) staff       (20)    11532 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/ant/AntSimulatorFast.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1736 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/ant/AntSimulatorFast.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      308 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/ant/buildAntSimFast.py
+-rw-r--r--   0 runner     (501) staff       (20)     1057 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/ant/santafe_trail.txt
+-rw-r--r--   0 runner     (501) staff       (20)     6864 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/ant.py
+-rw-r--r--   0 runner     (501) staff       (20)     3295 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/multiplexer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2949 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/parity.py
+-rw-r--r--   0 runner     (501) staff       (20)   702942 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/spambase.csv
+-rw-r--r--   0 runner     (501) staff       (20)     4043 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/spambase.py
+-rw-r--r--   0 runner     (501) staff       (20)     3374 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/symbreg.py
+-rw-r--r--   0 runner     (501) staff       (20)     3343 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/symbreg_epsilon_lexicase.py
+-rw-r--r--   0 runner     (501) staff       (20)     3371 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/symbreg_harm.py
+-rw-r--r--   0 runner     (501) staff       (20)     3289 2023-07-21 10:51:13.000000 deap-1.4.1/examples/gp/symbreg_numpy.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.733950 deap-1.4.1/examples/pso/
+-rw-r--r--   0 runner     (501) staff       (20)     3352 2023-07-21 10:51:13.000000 deap-1.4.1/examples/pso/basic.py
+-rw-r--r--   0 runner     (501) staff       (20)     3160 2023-07-21 10:51:13.000000 deap-1.4.1/examples/pso/basic_numpy.py
+-rw-r--r--   0 runner     (501) staff       (20)     9309 2023-07-21 10:51:13.000000 deap-1.4.1/examples/pso/multiswarm.py
+-rw-r--r--   0 runner     (501) staff       (20)     6580 2023-07-21 10:51:13.000000 deap-1.4.1/examples/pso/speciation.py
+-rw-r--r--   0 runner     (501) staff       (20)      508 2023-07-21 10:51:13.000000 deap-1.4.1/examples/speed.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-21 10:51:40.740270 deap-1.4.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3818 2023-07-21 10:51:13.000000 deap-1.4.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-21 10:51:40.739087 deap-1.4.1/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     8739 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_algorithms.py
+-rw-r--r--   0 runner     (501) staff       (20)     2354 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_benchmarks.py
+-rw-r--r--   0 runner     (501) staff       (20)    16006 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_convergence.py
+-rw-r--r--   0 runner     (501) staff       (20)     2591 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)      334 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_init.py
+-rw-r--r--   0 runner     (501) staff       (20)     1732 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_logbook.py
+-rw-r--r--   0 runner     (501) staff       (20)      661 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_multiproc.py
+-rw-r--r--   0 runner     (501) staff       (20)     1937 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_mutation.py
+-rw-r--r--   0 runner     (501) staff       (20)     1069 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_operators.py
+-rw-r--r--   0 runner     (501) staff       (20)     7300 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_pickle.py
+-rw-r--r--   0 runner     (501) staff       (20)      957 2023-07-21 10:51:13.000000 deap-1.4.1/tests/test_statistics.py
```

### Comparing `deap-1.4.0/INSTALL.txt` & `deap-1.4.1/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/LICENSE.txt` & `deap-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/PKG-INFO` & `deap-1.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,174 +1,175 @@
 Metadata-Version: 2.1
 Name: deap
-Version: 1.4.0
+Version: 1.4.1
 Summary: Distributed Evolutionary Algorithms in Python
 Home-page: https://www.github.com/deap
 Author: deap Development Team
 Author-email: deap-users@googlegroups.com
 License: LGPL
-Description: # DEAP
-        
-        [![Build status](https://travis-ci.org/DEAP/deap.svg?branch=master)](https://travis-ci.org/DEAP/deap) [![Download](https://img.shields.io/pypi/dm/deap.svg)](https://pypi.python.org/pypi/deap) [![Join the chat at https://gitter.im/DEAP/deap](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/DEAP/deap?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Build Status](https://dev.azure.com/fderainville/DEAP/_apis/build/status/DEAP.deap?branchName=master)](https://dev.azure.com/fderainville/DEAP/_build/latest?definitionId=1&branchName=master) [![Documentation Status](https://readthedocs.org/projects/deap/badge/?version=master)](https://deap.readthedocs.io/en/master/?badge=master)
-        
-        DEAP is a novel evolutionary computation framework for rapid prototyping and testing of 
-        ideas. It seeks to make algorithms explicit and data structures transparent. It works in perfect harmony with parallelisation mechanisms such as multiprocessing and [SCOOP](https://github.com/soravux/scoop).
-        
-        DEAP includes the following features:
-        
-          * Genetic algorithm using any imaginable representation
-            * List, Array, Set, Dictionary, Tree, Numpy Array, etc.
-          * Genetic programming using prefix trees
-            * Loosely typed, Strongly typed
-            * Automatically defined functions
-          * Evolution strategies (including CMA-ES)
-          * Multi-objective optimisation (NSGA-II, NSGA-III, SPEA2, MO-CMA-ES)
-          * Co-evolution (cooperative and competitive) of multiple populations
-          * Parallelization of the evaluations (and more)
-          * Hall of Fame of the best individuals that lived in the population
-          * Checkpoints that take snapshots of a system regularly
-          * Benchmarks module containing most common test functions
-          * Genealogy of an evolution (that is compatible with [NetworkX](https://github.com/networkx/networkx))
-          * Examples of alternative algorithms : Particle Swarm Optimization, Differential Evolution, Estimation of Distribution Algorithm
-        
-        ## Downloads
-        
-        Following acceptance of [PEP 438](http://www.python.org/dev/peps/pep-0438/) by the Python community, we have moved DEAP's source releases on [PyPI](https://pypi.python.org).
-        
-        You can find the most recent releases at: https://pypi.python.org/pypi/deap/.
-        
-        ## Documentation
-        See the [DEAP User's Guide](http://deap.readthedocs.org/) for DEAP documentation.
-        
-        In order to get the tip documentation, change directory to the `doc` subfolder and type in `make html`, the documentation will be under `_build/html`. You will need [Sphinx](http://sphinx.pocoo.org) to build the documentation.
-        
-        ### Notebooks
-        Also checkout our new [notebook examples](https://github.com/DEAP/notebooks). Using [Jupyter notebooks](http://jupyter.org)  you'll be able to navigate and execute each block of code individually and tell what every line is doing. Either, look at the notebooks online using the notebook viewer links at the botom of the page or download the notebooks, navigate to the you download directory and run
-        
-        ```bash
-        jupyter notebook
-        ```
-        
-        ## Installation
-        We encourage you to use easy_install or pip to install DEAP on your system. Other installation procedure like apt-get, yum, etc. usually provide an outdated version.
-        ```bash
-        pip install deap
-        ```
-        
-        The latest version can be installed with 
-        ```bash
-        pip install git+https://github.com/DEAP/deap@master
-        ```
-        
-        If you wish to build from sources, download or clone the repository and type
-        
-        ```bash
-        python setup.py install
-        ```
-        
-        ## Build Status
-        DEAP build status is available on Travis-CI https://travis-ci.org/DEAP/deap.
-        
-        ## Requirements
-        The most basic features of DEAP requires Python2.6. In order to combine the toolbox and the multiprocessing module Python2.7 is needed for its support to pickle partial functions. CMA-ES requires Numpy, and we recommend matplotlib for visualization of results as it is fully compatible with DEAP's API.
-        
-        Since version 0.8, DEAP is compatible out of the box with Python 3. The installation procedure automatically translates the source to Python 3 with 2to3, however this requires having `setuptools<=58`. It is recommended to use `pip install setuptools==57.5.0` to address this issue.
-        
-        ## Example
-        
-        The following code gives a quick overview how simple it is to implement the Onemax problem optimization with genetic algorithm using DEAP.  More examples are provided [here](http://deap.readthedocs.org/en/master/examples/index.html).
-        
-        ```python
-        import random
-        from deap import creator, base, tools, algorithms
-        
-        creator.create("FitnessMax", base.Fitness, weights=(1.0,))
-        creator.create("Individual", list, fitness=creator.FitnessMax)
-        
-        toolbox = base.Toolbox()
-        
-        toolbox.register("attr_bool", random.randint, 0, 1)
-        toolbox.register("individual", tools.initRepeat, creator.Individual, toolbox.attr_bool, n=100)
-        toolbox.register("population", tools.initRepeat, list, toolbox.individual)
-        
-        def evalOneMax(individual):
-            return sum(individual),
-        
-        toolbox.register("evaluate", evalOneMax)
-        toolbox.register("mate", tools.cxTwoPoint)
-        toolbox.register("mutate", tools.mutFlipBit, indpb=0.05)
-        toolbox.register("select", tools.selTournament, tournsize=3)
-        
-        population = toolbox.population(n=300)
-        
-        NGEN=40
-        for gen in range(NGEN):
-            offspring = algorithms.varAnd(population, toolbox, cxpb=0.5, mutpb=0.1)
-            fits = toolbox.map(toolbox.evaluate, offspring)
-            for fit, ind in zip(fits, offspring):
-                ind.fitness.values = fit
-            population = toolbox.select(offspring, k=len(population))
-        top10 = tools.selBest(population, k=10)
-        ```
-        
-        ## How to cite DEAP
-        Authors of scientific papers including results generated using DEAP are encouraged to cite the following paper.
-        
-        ```xml
-        @article{DEAP_JMLR2012, 
-            author    = " F\'elix-Antoine Fortin and Fran\c{c}ois-Michel {De Rainville} and Marc-Andr\'e Gardner and Marc Parizeau and Christian Gagn\'e ",
-            title     = { {DEAP}: Evolutionary Algorithms Made Easy },
-            pages    = { 2171--2175 },
-            volume    = { 13 },
-            month     = { jul },
-            year      = { 2012 },
-            journal   = { Journal of Machine Learning Research }
-        }
-        ```
-        
-        ## Publications on DEAP
-        
-          * François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP -- Enabling Nimbler Evolutions", SIGEVOlution, vol. 6, no 2, pp. 17-26, February 2014. [Paper](http://goo.gl/tOrXTp)
-          * Félix-Antoine Fortin, François-Michel De Rainville, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP: Evolutionary Algorithms Made Easy", Journal of Machine Learning Research, vol. 13, pp. 2171-2175, jul 2012. [Paper](http://goo.gl/amJ3x)
-          * François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP: A Python Framework for Evolutionary Algorithms", in !EvoSoft Workshop, Companion proc. of the Genetic and Evolutionary Computation Conference (GECCO 2012), July 07-11 2012. [Paper](http://goo.gl/pXXug)
-        
-        ## Projects using DEAP
-          * Ribaric, T., & Houghten, S. (2017, June). Genetic programming for improved cryptanalysis of elliptic curve cryptosystems. In 2017 IEEE Congress on Evolutionary Computation (CEC) (pp. 419-426). IEEE.
-          * Ellefsen, Kai Olav, Herman Augusto Lepikson, and Jan C. Albiez. "Multiobjective coverage path planning: Enabling automated inspection of complex, real-world structures." Applied Soft Computing 61 (2017): 264-282.
-          * S. Chardon, B. Brangeon, E. Bozonnet, C. Inard (2016), Construction cost and energy performance of single family houses : From integrated design to automated optimization, Automation in Construction, Volume 70, p.1-13.
-          * B. Brangeon, E. Bozonnet, C. Inard (2016), Integrated refurbishment of collective housing and optimization process with real products databases, Building Simulation Optimization, pp. 531–538 Newcastle, England.
-          * Randal S. Olson, Ryan J. Urbanowicz, Peter C. Andrews, Nicole A. Lavender, La Creis Kidd, and Jason H. Moore (2016). Automating biomedical data science through tree-based pipeline optimization. Applications of Evolutionary Computation, pages 123-137.
-          * Randal S. Olson, Nathan Bartley, Ryan J. Urbanowicz, and Jason H. Moore (2016). Evaluation of a Tree-based Pipeline Optimization Tool for Automating Data Science. Proceedings of GECCO 2016, pages 485-492.
-          * Van Geit W, Gevaert M, Chindemi G, Rössert C, Courcol J, Muller EB, Schürmann F, Segev I and Markram H (2016). BluePyOpt: Leveraging open source software and cloud infrastructure to optimise model parameters in neuroscience. Front. Neuroinform. 10:17. doi: 10.3389/fninf.2016.00017 https://github.com/BlueBrain/BluePyOpt
-          * Lara-Cabrera, R., Cotta, C. and Fernández-Leiva, A.J. (2014). Geometrical vs topological measures for the evolution of aesthetic maps in a rts game, Entertainment Computing,
-          * Macret, M. and Pasquier, P. (2013). Automatic Tuning of the OP-1 Synthesizer Using a Multi-objective Genetic Algorithm. In Proceedings of the 10th Sound and Music Computing Conference (SMC). (pp 614-621).
-          * Fortin, F. A., Grenier, S., & Parizeau, M. (2013, July). Generalizing the improved run-time complexity algorithm for non-dominated sorting. In Proceeding of the fifteenth annual conference on Genetic and evolutionary computation conference (pp. 615-622). ACM.
-          * Fortin, F. A., & Parizeau, M. (2013, July). Revisiting the NSGA-II crowding-distance computation. In Proceeding of the fifteenth annual conference on Genetic and evolutionary computation conference (pp. 623-630). ACM.
-          * Marc-André Gardner, Christian Gagné, and Marc Parizeau. Estimation of Distribution Algorithm based on Hidden Markov Models for Combinatorial Optimization. in Comp. Proc. Genetic and Evolutionary Computation Conference (GECCO 2013), July 2013.
-          * J. T. Zhai, M. A. Bamakhrama, and T. Stefanov. "Exploiting Just-enough Parallelism when Mapping Streaming Applications in Hard Real-time Systems". Design Automation Conference (DAC 2013), 2013.
-          * V. Akbarzadeh, C. Gagné, M. Parizeau, M. Argany, M. A Mostafavi, "Probabilistic Sensing Model for Sensor Placement Optimization Based on Line-of-Sight Coverage", Accepted in IEEE Transactions on Instrumentation and Measurement, 2012.
-          * M. Reif, F. Shafait, and A. Dengel. "Dataset Generation for Meta-Learning". Proceedings of the German Conference on Artificial Intelligence (KI'12). 2012. 
-          * M. T. Ribeiro, A. Lacerda, A. Veloso, and N. Ziviani. "Pareto-Efficient Hybridization for Multi-Objective Recommender Systems". Proceedings of the Conference on Recommanders Systems (!RecSys'12). 2012.
-          * M. Pérez-Ortiz, A. Arauzo-Azofra, C. Hervás-Martínez, L. García-Hernández and L. Salas-Morera. "A system learning user preferences for multiobjective optimization of facility layouts". Pr,oceedings on the Int. Conference on Soft Computing Models in Industrial and Environmental Applications (SOCO'12). 2012.
-          * Lévesque, J.C., Durand, A., Gagné, C., and Sabourin, R., Multi-Objective Evolutionary Optimization for Generating Ensembles of Classifiers in the ROC Space, Genetic and Evolutionary Computation Conference (GECCO 2012), 2012.
-          * Marc-André Gardner, Christian Gagné, and Marc Parizeau, "Bloat Control in Genetic Programming with Histogram-based Accept-Reject Method", in Proc. Genetic and Evolutionary Computation Conference (GECCO 2011), 2011.
-          * Vahab Akbarzadeh, Albert Ko, Christian Gagné, and Marc Parizeau, "Topography-Aware Sensor Deployment Optimization with CMA-ES", in Proc. of Parallel Problem Solving from Nature (PPSN 2010), Springer, 2010.
-          * DEAP is used in [TPOT](https://github.com/rhiever/tpot), an open source tool that uses genetic programming to optimize machine learning pipelines.
-          * DEAP is also used in ROS as an optimization package http://www.ros.org/wiki/deap.
-          * DEAP is an optional dependency for [PyXRD](https://github.com/mathijs-dumon/PyXRD), a Python implementation of the matrix algorithm developed for the X-ray diffraction analysis of disordered lamellar structures.
-          * DEAP is used in [glyph](https://github.com/Ambrosys/glyph), a library for symbolic regression with applications to [MLC](https://en.wikipedia.org/wiki/Machine_learning_control).
-          * DEAP is used in [Sklearn-genetic-opt](https://github.com/rodrigo-arenas/Sklearn-genetic-opt), an open source tool that uses evolutionary programming to fine tune machine learning hyperparameters.
-        
-        If you want your project listed here, send us a link and a brief description and we'll be glad to add it.
-        
 Keywords: evolutionary algorithms,genetic algorithms,genetic programming,cma-es,ga,gp,es,pso
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# DEAP
+
+[![Build status](https://travis-ci.org/DEAP/deap.svg?branch=master)](https://travis-ci.org/DEAP/deap) [![Download](https://img.shields.io/pypi/dm/deap.svg)](https://pypi.python.org/pypi/deap) [![Join the chat at https://gitter.im/DEAP/deap](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/DEAP/deap?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Build Status](https://dev.azure.com/fderainville/DEAP/_apis/build/status/DEAP.deap?branchName=master)](https://dev.azure.com/fderainville/DEAP/_build/latest?definitionId=1&branchName=master) [![Documentation Status](https://readthedocs.org/projects/deap/badge/?version=master)](https://deap.readthedocs.io/en/master/?badge=master)
+
+DEAP is a novel evolutionary computation framework for rapid prototyping and testing of 
+ideas. It seeks to make algorithms explicit and data structures transparent. It works in perfect harmony with parallelisation mechanisms such as multiprocessing and [SCOOP](https://github.com/soravux/scoop).
+
+DEAP includes the following features:
+
+  * Genetic algorithm using any imaginable representation
+    * List, Array, Set, Dictionary, Tree, Numpy Array, etc.
+  * Genetic programming using prefix trees
+    * Loosely typed, Strongly typed
+    * Automatically defined functions
+  * Evolution strategies (including CMA-ES)
+  * Multi-objective optimisation (NSGA-II, NSGA-III, SPEA2, MO-CMA-ES)
+  * Co-evolution (cooperative and competitive) of multiple populations
+  * Parallelization of the evaluations (and more)
+  * Hall of Fame of the best individuals that lived in the population
+  * Checkpoints that take snapshots of a system regularly
+  * Benchmarks module containing most common test functions
+  * Genealogy of an evolution (that is compatible with [NetworkX](https://github.com/networkx/networkx))
+  * Examples of alternative algorithms : Particle Swarm Optimization, Differential Evolution, Estimation of Distribution Algorithm
+
+## Downloads
+
+Following acceptance of [PEP 438](http://www.python.org/dev/peps/pep-0438/) by the Python community, we have moved DEAP's source releases on [PyPI](https://pypi.python.org).
+
+You can find the most recent releases at: https://pypi.python.org/pypi/deap/.
+
+## Documentation
+See the [DEAP User's Guide](http://deap.readthedocs.org/) for DEAP documentation.
+
+In order to get the tip documentation, change directory to the `doc` subfolder and type in `make html`, the documentation will be under `_build/html`. You will need [Sphinx](http://sphinx.pocoo.org) to build the documentation.
+
+### Notebooks
+Also checkout our new [notebook examples](https://github.com/DEAP/notebooks). Using [Jupyter notebooks](http://jupyter.org)  you'll be able to navigate and execute each block of code individually and tell what every line is doing. Either, look at the notebooks online using the notebook viewer links at the botom of the page or download the notebooks, navigate to the you download directory and run
+
+```bash
+jupyter notebook
+```
+
+## Installation
+We encourage you to use easy_install or pip to install DEAP on your system. Other installation procedure like apt-get, yum, etc. usually provide an outdated version.
+```bash
+pip install deap
+```
+
+The latest version can be installed with 
+```bash
+pip install git+https://github.com/DEAP/deap@master
+```
+
+If you wish to build from sources, download or clone the repository and type
+
+```bash
+python setup.py install
+```
+
+## Build Status
+DEAP build status is available on Travis-CI https://travis-ci.org/DEAP/deap.
+
+## Requirements
+The most basic features of DEAP requires Python2.6. In order to combine the toolbox and the multiprocessing module Python2.7 is needed for its support to pickle partial functions. CMA-ES requires Numpy, and we recommend matplotlib for visualization of results as it is fully compatible with DEAP's API.
+
+Since version 0.8, DEAP is compatible out of the box with Python 3. The installation procedure automatically translates the source to Python 3 with 2to3, however this requires having `setuptools<=58`. It is recommended to use `pip install setuptools==57.5.0` to address this issue.
+
+## Example
+
+The following code gives a quick overview how simple it is to implement the Onemax problem optimization with genetic algorithm using DEAP.  More examples are provided [here](http://deap.readthedocs.org/en/master/examples/index.html).
+
+```python
+import random
+from deap import creator, base, tools, algorithms
+
+creator.create("FitnessMax", base.Fitness, weights=(1.0,))
+creator.create("Individual", list, fitness=creator.FitnessMax)
+
+toolbox = base.Toolbox()
+
+toolbox.register("attr_bool", random.randint, 0, 1)
+toolbox.register("individual", tools.initRepeat, creator.Individual, toolbox.attr_bool, n=100)
+toolbox.register("population", tools.initRepeat, list, toolbox.individual)
+
+def evalOneMax(individual):
+    return sum(individual),
+
+toolbox.register("evaluate", evalOneMax)
+toolbox.register("mate", tools.cxTwoPoint)
+toolbox.register("mutate", tools.mutFlipBit, indpb=0.05)
+toolbox.register("select", tools.selTournament, tournsize=3)
+
+population = toolbox.population(n=300)
+
+NGEN=40
+for gen in range(NGEN):
+    offspring = algorithms.varAnd(population, toolbox, cxpb=0.5, mutpb=0.1)
+    fits = toolbox.map(toolbox.evaluate, offspring)
+    for fit, ind in zip(fits, offspring):
+        ind.fitness.values = fit
+    population = toolbox.select(offspring, k=len(population))
+top10 = tools.selBest(population, k=10)
+```
+
+## How to cite DEAP
+Authors of scientific papers including results generated using DEAP are encouraged to cite the following paper.
+
+```xml
+@article{DEAP_JMLR2012, 
+    author    = " F\'elix-Antoine Fortin and Fran\c{c}ois-Michel {De Rainville} and Marc-Andr\'e Gardner and Marc Parizeau and Christian Gagn\'e ",
+    title     = { {DEAP}: Evolutionary Algorithms Made Easy },
+    pages    = { 2171--2175 },
+    volume    = { 13 },
+    month     = { jul },
+    year      = { 2012 },
+    journal   = { Journal of Machine Learning Research }
+}
+```
+
+## Publications on DEAP
+
+  * François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP -- Enabling Nimbler Evolutions", SIGEVOlution, vol. 6, no 2, pp. 17-26, February 2014. [Paper](http://goo.gl/tOrXTp)
+  * Félix-Antoine Fortin, François-Michel De Rainville, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP: Evolutionary Algorithms Made Easy", Journal of Machine Learning Research, vol. 13, pp. 2171-2175, jul 2012. [Paper](http://goo.gl/amJ3x)
+  * François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP: A Python Framework for Evolutionary Algorithms", in !EvoSoft Workshop, Companion proc. of the Genetic and Evolutionary Computation Conference (GECCO 2012), July 07-11 2012. [Paper](http://goo.gl/pXXug)
+
+## Projects using DEAP
+  * Ribaric, T., & Houghten, S. (2017, June). Genetic programming for improved cryptanalysis of elliptic curve cryptosystems. In 2017 IEEE Congress on Evolutionary Computation (CEC) (pp. 419-426). IEEE.
+  * Ellefsen, Kai Olav, Herman Augusto Lepikson, and Jan C. Albiez. "Multiobjective coverage path planning: Enabling automated inspection of complex, real-world structures." Applied Soft Computing 61 (2017): 264-282.
+  * S. Chardon, B. Brangeon, E. Bozonnet, C. Inard (2016), Construction cost and energy performance of single family houses : From integrated design to automated optimization, Automation in Construction, Volume 70, p.1-13.
+  * B. Brangeon, E. Bozonnet, C. Inard (2016), Integrated refurbishment of collective housing and optimization process with real products databases, Building Simulation Optimization, pp. 531–538 Newcastle, England.
+  * Randal S. Olson, Ryan J. Urbanowicz, Peter C. Andrews, Nicole A. Lavender, La Creis Kidd, and Jason H. Moore (2016). Automating biomedical data science through tree-based pipeline optimization. Applications of Evolutionary Computation, pages 123-137.
+  * Randal S. Olson, Nathan Bartley, Ryan J. Urbanowicz, and Jason H. Moore (2016). Evaluation of a Tree-based Pipeline Optimization Tool for Automating Data Science. Proceedings of GECCO 2016, pages 485-492.
+  * Van Geit W, Gevaert M, Chindemi G, Rössert C, Courcol J, Muller EB, Schürmann F, Segev I and Markram H (2016). BluePyOpt: Leveraging open source software and cloud infrastructure to optimise model parameters in neuroscience. Front. Neuroinform. 10:17. doi: 10.3389/fninf.2016.00017 https://github.com/BlueBrain/BluePyOpt
+  * Lara-Cabrera, R., Cotta, C. and Fernández-Leiva, A.J. (2014). Geometrical vs topological measures for the evolution of aesthetic maps in a rts game, Entertainment Computing,
+  * Macret, M. and Pasquier, P. (2013). Automatic Tuning of the OP-1 Synthesizer Using a Multi-objective Genetic Algorithm. In Proceedings of the 10th Sound and Music Computing Conference (SMC). (pp 614-621).
+  * Fortin, F. A., Grenier, S., & Parizeau, M. (2013, July). Generalizing the improved run-time complexity algorithm for non-dominated sorting. In Proceeding of the fifteenth annual conference on Genetic and evolutionary computation conference (pp. 615-622). ACM.
+  * Fortin, F. A., & Parizeau, M. (2013, July). Revisiting the NSGA-II crowding-distance computation. In Proceeding of the fifteenth annual conference on Genetic and evolutionary computation conference (pp. 623-630). ACM.
+  * Marc-André Gardner, Christian Gagné, and Marc Parizeau. Estimation of Distribution Algorithm based on Hidden Markov Models for Combinatorial Optimization. in Comp. Proc. Genetic and Evolutionary Computation Conference (GECCO 2013), July 2013.
+  * J. T. Zhai, M. A. Bamakhrama, and T. Stefanov. "Exploiting Just-enough Parallelism when Mapping Streaming Applications in Hard Real-time Systems". Design Automation Conference (DAC 2013), 2013.
+  * V. Akbarzadeh, C. Gagné, M. Parizeau, M. Argany, M. A Mostafavi, "Probabilistic Sensing Model for Sensor Placement Optimization Based on Line-of-Sight Coverage", Accepted in IEEE Transactions on Instrumentation and Measurement, 2012.
+  * M. Reif, F. Shafait, and A. Dengel. "Dataset Generation for Meta-Learning". Proceedings of the German Conference on Artificial Intelligence (KI'12). 2012. 
+  * M. T. Ribeiro, A. Lacerda, A. Veloso, and N. Ziviani. "Pareto-Efficient Hybridization for Multi-Objective Recommender Systems". Proceedings of the Conference on Recommanders Systems (!RecSys'12). 2012.
+  * M. Pérez-Ortiz, A. Arauzo-Azofra, C. Hervás-Martínez, L. García-Hernández and L. Salas-Morera. "A system learning user preferences for multiobjective optimization of facility layouts". Pr,oceedings on the Int. Conference on Soft Computing Models in Industrial and Environmental Applications (SOCO'12). 2012.
+  * Lévesque, J.C., Durand, A., Gagné, C., and Sabourin, R., Multi-Objective Evolutionary Optimization for Generating Ensembles of Classifiers in the ROC Space, Genetic and Evolutionary Computation Conference (GECCO 2012), 2012.
+  * Marc-André Gardner, Christian Gagné, and Marc Parizeau, "Bloat Control in Genetic Programming with Histogram-based Accept-Reject Method", in Proc. Genetic and Evolutionary Computation Conference (GECCO 2011), 2011.
+  * Vahab Akbarzadeh, Albert Ko, Christian Gagné, and Marc Parizeau, "Topography-Aware Sensor Deployment Optimization with CMA-ES", in Proc. of Parallel Problem Solving from Nature (PPSN 2010), Springer, 2010.
+  * DEAP is used in [TPOT](https://github.com/rhiever/tpot), an open source tool that uses genetic programming to optimize machine learning pipelines.
+  * DEAP is also used in ROS as an optimization package http://www.ros.org/wiki/deap.
+  * DEAP is an optional dependency for [PyXRD](https://github.com/mathijs-dumon/PyXRD), a Python implementation of the matrix algorithm developed for the X-ray diffraction analysis of disordered lamellar structures.
+  * DEAP is used in [glyph](https://github.com/Ambrosys/glyph), a library for symbolic regression with applications to [MLC](https://en.wikipedia.org/wiki/Machine_learning_control).
+  * DEAP is used in [Sklearn-genetic-opt](https://github.com/rodrigo-arenas/Sklearn-genetic-opt), an open source tool that uses evolutionary programming to fine tune machine learning hyperparameters.
+
+If you want your project listed here, send us a link and a brief description and we'll be glad to add it.
```

### Comparing `deap-1.4.0/README.md` & `deap-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/__init__.py` & `deap-1.4.1/deap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #    GNU Lesser General Public License for more details.
 #
 #    You should have received a copy of the GNU Lesser General Public
 #    License along with DEAP. If not, see <http://www.gnu.org/licenses/>.
 __author__ = "DEAP Team"
 __version__ = "1.4"
-__revision__ = "1.4.0"
+__revision__ = "1.4.1"
```

### Comparing `deap-1.4.0/deap/algorithms.py` & `deap-1.4.1/deap/algorithms.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/base.py` & `deap-1.4.1/deap/base.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/benchmarks/__init__.py` & `deap-1.4.1/deap/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/benchmarks/binary.py` & `deap-1.4.1/deap/benchmarks/binary.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/benchmarks/gp.py` & `deap-1.4.1/deap/benchmarks/gp.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/benchmarks/movingpeaks.py` & `deap-1.4.1/deap/benchmarks/movingpeaks.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/benchmarks/tools.py` & `deap-1.4.1/deap/benchmarks/tools.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/cma.py` & `deap-1.4.1/deap/cma.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/creator.py` & `deap-1.4.1/deap/creator.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/gp.py` & `deap-1.4.1/deap/gp.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/__init__.py` & `deap-1.4.1/deap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/_hypervolume/__init__.py` & `deap-1.4.1/deap/tools/_hypervolume/__init__.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/_hypervolume/_hv.c` & `deap-1.4.1/deap/tools/_hypervolume/_hv.c`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/_hypervolume/_hv.h` & `deap-1.4.1/deap/tools/_hypervolume/_hv.h`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/_hypervolume/hv.cpp` & `deap-1.4.1/deap/tools/_hypervolume/hv.cpp`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/_hypervolume/pyhv.py` & `deap-1.4.1/deap/tools/_hypervolume/pyhv.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/constraint.py` & `deap-1.4.1/deap/tools/constraint.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/crossover.py` & `deap-1.4.1/deap/tools/crossover.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/emo.py` & `deap-1.4.1/deap/tools/emo.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/indicator.py` & `deap-1.4.1/deap/tools/indicator.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/init.py` & `deap-1.4.1/deap/tools/init.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/migration.py` & `deap-1.4.1/deap/tools/migration.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/mutation.py` & `deap-1.4.1/deap/tools/mutation.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/selection.py` & `deap-1.4.1/deap/tools/selection.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/deap/tools/support.py` & `deap-1.4.1/deap/tools/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         colors = [toolbox.evaluate(history.genealogy_history[i])[0] for i in graph]
         networkx.draw(graph, node_color=colors)
         plt.show()
 
     Using NetworkX in combination with `pygraphviz
     <http://networkx.lanl.gov/pygraphviz/>`_ (dot layout) this amazing
     genealogy tree can be obtained from the OneMax example with a population
-    size of 20 and 5 generations, where the color of the nodes indicate there
+    size of 20 and 5 generations, where the color of the nodes indicate their
     fitness, blue is low and red is high.
 
     .. image:: /_images/genealogy.png
        :width: 67%
 
     .. note::
        The genealogy tree might get very big if your population and/or the
```

### Comparing `deap-1.4.0/deap.egg-info/PKG-INFO` & `deap-1.4.1/deap.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,174 +1,175 @@
 Metadata-Version: 2.1
 Name: deap
-Version: 1.4.0
+Version: 1.4.1
 Summary: Distributed Evolutionary Algorithms in Python
 Home-page: https://www.github.com/deap
 Author: deap Development Team
 Author-email: deap-users@googlegroups.com
 License: LGPL
-Description: # DEAP
-        
-        [![Build status](https://travis-ci.org/DEAP/deap.svg?branch=master)](https://travis-ci.org/DEAP/deap) [![Download](https://img.shields.io/pypi/dm/deap.svg)](https://pypi.python.org/pypi/deap) [![Join the chat at https://gitter.im/DEAP/deap](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/DEAP/deap?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Build Status](https://dev.azure.com/fderainville/DEAP/_apis/build/status/DEAP.deap?branchName=master)](https://dev.azure.com/fderainville/DEAP/_build/latest?definitionId=1&branchName=master) [![Documentation Status](https://readthedocs.org/projects/deap/badge/?version=master)](https://deap.readthedocs.io/en/master/?badge=master)
-        
-        DEAP is a novel evolutionary computation framework for rapid prototyping and testing of 
-        ideas. It seeks to make algorithms explicit and data structures transparent. It works in perfect harmony with parallelisation mechanisms such as multiprocessing and [SCOOP](https://github.com/soravux/scoop).
-        
-        DEAP includes the following features:
-        
-          * Genetic algorithm using any imaginable representation
-            * List, Array, Set, Dictionary, Tree, Numpy Array, etc.
-          * Genetic programming using prefix trees
-            * Loosely typed, Strongly typed
-            * Automatically defined functions
-          * Evolution strategies (including CMA-ES)
-          * Multi-objective optimisation (NSGA-II, NSGA-III, SPEA2, MO-CMA-ES)
-          * Co-evolution (cooperative and competitive) of multiple populations
-          * Parallelization of the evaluations (and more)
-          * Hall of Fame of the best individuals that lived in the population
-          * Checkpoints that take snapshots of a system regularly
-          * Benchmarks module containing most common test functions
-          * Genealogy of an evolution (that is compatible with [NetworkX](https://github.com/networkx/networkx))
-          * Examples of alternative algorithms : Particle Swarm Optimization, Differential Evolution, Estimation of Distribution Algorithm
-        
-        ## Downloads
-        
-        Following acceptance of [PEP 438](http://www.python.org/dev/peps/pep-0438/) by the Python community, we have moved DEAP's source releases on [PyPI](https://pypi.python.org).
-        
-        You can find the most recent releases at: https://pypi.python.org/pypi/deap/.
-        
-        ## Documentation
-        See the [DEAP User's Guide](http://deap.readthedocs.org/) for DEAP documentation.
-        
-        In order to get the tip documentation, change directory to the `doc` subfolder and type in `make html`, the documentation will be under `_build/html`. You will need [Sphinx](http://sphinx.pocoo.org) to build the documentation.
-        
-        ### Notebooks
-        Also checkout our new [notebook examples](https://github.com/DEAP/notebooks). Using [Jupyter notebooks](http://jupyter.org)  you'll be able to navigate and execute each block of code individually and tell what every line is doing. Either, look at the notebooks online using the notebook viewer links at the botom of the page or download the notebooks, navigate to the you download directory and run
-        
-        ```bash
-        jupyter notebook
-        ```
-        
-        ## Installation
-        We encourage you to use easy_install or pip to install DEAP on your system. Other installation procedure like apt-get, yum, etc. usually provide an outdated version.
-        ```bash
-        pip install deap
-        ```
-        
-        The latest version can be installed with 
-        ```bash
-        pip install git+https://github.com/DEAP/deap@master
-        ```
-        
-        If you wish to build from sources, download or clone the repository and type
-        
-        ```bash
-        python setup.py install
-        ```
-        
-        ## Build Status
-        DEAP build status is available on Travis-CI https://travis-ci.org/DEAP/deap.
-        
-        ## Requirements
-        The most basic features of DEAP requires Python2.6. In order to combine the toolbox and the multiprocessing module Python2.7 is needed for its support to pickle partial functions. CMA-ES requires Numpy, and we recommend matplotlib for visualization of results as it is fully compatible with DEAP's API.
-        
-        Since version 0.8, DEAP is compatible out of the box with Python 3. The installation procedure automatically translates the source to Python 3 with 2to3, however this requires having `setuptools<=58`. It is recommended to use `pip install setuptools==57.5.0` to address this issue.
-        
-        ## Example
-        
-        The following code gives a quick overview how simple it is to implement the Onemax problem optimization with genetic algorithm using DEAP.  More examples are provided [here](http://deap.readthedocs.org/en/master/examples/index.html).
-        
-        ```python
-        import random
-        from deap import creator, base, tools, algorithms
-        
-        creator.create("FitnessMax", base.Fitness, weights=(1.0,))
-        creator.create("Individual", list, fitness=creator.FitnessMax)
-        
-        toolbox = base.Toolbox()
-        
-        toolbox.register("attr_bool", random.randint, 0, 1)
-        toolbox.register("individual", tools.initRepeat, creator.Individual, toolbox.attr_bool, n=100)
-        toolbox.register("population", tools.initRepeat, list, toolbox.individual)
-        
-        def evalOneMax(individual):
-            return sum(individual),
-        
-        toolbox.register("evaluate", evalOneMax)
-        toolbox.register("mate", tools.cxTwoPoint)
-        toolbox.register("mutate", tools.mutFlipBit, indpb=0.05)
-        toolbox.register("select", tools.selTournament, tournsize=3)
-        
-        population = toolbox.population(n=300)
-        
-        NGEN=40
-        for gen in range(NGEN):
-            offspring = algorithms.varAnd(population, toolbox, cxpb=0.5, mutpb=0.1)
-            fits = toolbox.map(toolbox.evaluate, offspring)
-            for fit, ind in zip(fits, offspring):
-                ind.fitness.values = fit
-            population = toolbox.select(offspring, k=len(population))
-        top10 = tools.selBest(population, k=10)
-        ```
-        
-        ## How to cite DEAP
-        Authors of scientific papers including results generated using DEAP are encouraged to cite the following paper.
-        
-        ```xml
-        @article{DEAP_JMLR2012, 
-            author    = " F\'elix-Antoine Fortin and Fran\c{c}ois-Michel {De Rainville} and Marc-Andr\'e Gardner and Marc Parizeau and Christian Gagn\'e ",
-            title     = { {DEAP}: Evolutionary Algorithms Made Easy },
-            pages    = { 2171--2175 },
-            volume    = { 13 },
-            month     = { jul },
-            year      = { 2012 },
-            journal   = { Journal of Machine Learning Research }
-        }
-        ```
-        
-        ## Publications on DEAP
-        
-          * François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP -- Enabling Nimbler Evolutions", SIGEVOlution, vol. 6, no 2, pp. 17-26, February 2014. [Paper](http://goo.gl/tOrXTp)
-          * Félix-Antoine Fortin, François-Michel De Rainville, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP: Evolutionary Algorithms Made Easy", Journal of Machine Learning Research, vol. 13, pp. 2171-2175, jul 2012. [Paper](http://goo.gl/amJ3x)
-          * François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP: A Python Framework for Evolutionary Algorithms", in !EvoSoft Workshop, Companion proc. of the Genetic and Evolutionary Computation Conference (GECCO 2012), July 07-11 2012. [Paper](http://goo.gl/pXXug)
-        
-        ## Projects using DEAP
-          * Ribaric, T., & Houghten, S. (2017, June). Genetic programming for improved cryptanalysis of elliptic curve cryptosystems. In 2017 IEEE Congress on Evolutionary Computation (CEC) (pp. 419-426). IEEE.
-          * Ellefsen, Kai Olav, Herman Augusto Lepikson, and Jan C. Albiez. "Multiobjective coverage path planning: Enabling automated inspection of complex, real-world structures." Applied Soft Computing 61 (2017): 264-282.
-          * S. Chardon, B. Brangeon, E. Bozonnet, C. Inard (2016), Construction cost and energy performance of single family houses : From integrated design to automated optimization, Automation in Construction, Volume 70, p.1-13.
-          * B. Brangeon, E. Bozonnet, C. Inard (2016), Integrated refurbishment of collective housing and optimization process with real products databases, Building Simulation Optimization, pp. 531–538 Newcastle, England.
-          * Randal S. Olson, Ryan J. Urbanowicz, Peter C. Andrews, Nicole A. Lavender, La Creis Kidd, and Jason H. Moore (2016). Automating biomedical data science through tree-based pipeline optimization. Applications of Evolutionary Computation, pages 123-137.
-          * Randal S. Olson, Nathan Bartley, Ryan J. Urbanowicz, and Jason H. Moore (2016). Evaluation of a Tree-based Pipeline Optimization Tool for Automating Data Science. Proceedings of GECCO 2016, pages 485-492.
-          * Van Geit W, Gevaert M, Chindemi G, Rössert C, Courcol J, Muller EB, Schürmann F, Segev I and Markram H (2016). BluePyOpt: Leveraging open source software and cloud infrastructure to optimise model parameters in neuroscience. Front. Neuroinform. 10:17. doi: 10.3389/fninf.2016.00017 https://github.com/BlueBrain/BluePyOpt
-          * Lara-Cabrera, R., Cotta, C. and Fernández-Leiva, A.J. (2014). Geometrical vs topological measures for the evolution of aesthetic maps in a rts game, Entertainment Computing,
-          * Macret, M. and Pasquier, P. (2013). Automatic Tuning of the OP-1 Synthesizer Using a Multi-objective Genetic Algorithm. In Proceedings of the 10th Sound and Music Computing Conference (SMC). (pp 614-621).
-          * Fortin, F. A., Grenier, S., & Parizeau, M. (2013, July). Generalizing the improved run-time complexity algorithm for non-dominated sorting. In Proceeding of the fifteenth annual conference on Genetic and evolutionary computation conference (pp. 615-622). ACM.
-          * Fortin, F. A., & Parizeau, M. (2013, July). Revisiting the NSGA-II crowding-distance computation. In Proceeding of the fifteenth annual conference on Genetic and evolutionary computation conference (pp. 623-630). ACM.
-          * Marc-André Gardner, Christian Gagné, and Marc Parizeau. Estimation of Distribution Algorithm based on Hidden Markov Models for Combinatorial Optimization. in Comp. Proc. Genetic and Evolutionary Computation Conference (GECCO 2013), July 2013.
-          * J. T. Zhai, M. A. Bamakhrama, and T. Stefanov. "Exploiting Just-enough Parallelism when Mapping Streaming Applications in Hard Real-time Systems". Design Automation Conference (DAC 2013), 2013.
-          * V. Akbarzadeh, C. Gagné, M. Parizeau, M. Argany, M. A Mostafavi, "Probabilistic Sensing Model for Sensor Placement Optimization Based on Line-of-Sight Coverage", Accepted in IEEE Transactions on Instrumentation and Measurement, 2012.
-          * M. Reif, F. Shafait, and A. Dengel. "Dataset Generation for Meta-Learning". Proceedings of the German Conference on Artificial Intelligence (KI'12). 2012. 
-          * M. T. Ribeiro, A. Lacerda, A. Veloso, and N. Ziviani. "Pareto-Efficient Hybridization for Multi-Objective Recommender Systems". Proceedings of the Conference on Recommanders Systems (!RecSys'12). 2012.
-          * M. Pérez-Ortiz, A. Arauzo-Azofra, C. Hervás-Martínez, L. García-Hernández and L. Salas-Morera. "A system learning user preferences for multiobjective optimization of facility layouts". Pr,oceedings on the Int. Conference on Soft Computing Models in Industrial and Environmental Applications (SOCO'12). 2012.
-          * Lévesque, J.C., Durand, A., Gagné, C., and Sabourin, R., Multi-Objective Evolutionary Optimization for Generating Ensembles of Classifiers in the ROC Space, Genetic and Evolutionary Computation Conference (GECCO 2012), 2012.
-          * Marc-André Gardner, Christian Gagné, and Marc Parizeau, "Bloat Control in Genetic Programming with Histogram-based Accept-Reject Method", in Proc. Genetic and Evolutionary Computation Conference (GECCO 2011), 2011.
-          * Vahab Akbarzadeh, Albert Ko, Christian Gagné, and Marc Parizeau, "Topography-Aware Sensor Deployment Optimization with CMA-ES", in Proc. of Parallel Problem Solving from Nature (PPSN 2010), Springer, 2010.
-          * DEAP is used in [TPOT](https://github.com/rhiever/tpot), an open source tool that uses genetic programming to optimize machine learning pipelines.
-          * DEAP is also used in ROS as an optimization package http://www.ros.org/wiki/deap.
-          * DEAP is an optional dependency for [PyXRD](https://github.com/mathijs-dumon/PyXRD), a Python implementation of the matrix algorithm developed for the X-ray diffraction analysis of disordered lamellar structures.
-          * DEAP is used in [glyph](https://github.com/Ambrosys/glyph), a library for symbolic regression with applications to [MLC](https://en.wikipedia.org/wiki/Machine_learning_control).
-          * DEAP is used in [Sklearn-genetic-opt](https://github.com/rodrigo-arenas/Sklearn-genetic-opt), an open source tool that uses evolutionary programming to fine tune machine learning hyperparameters.
-        
-        If you want your project listed here, send us a link and a brief description and we'll be glad to add it.
-        
 Keywords: evolutionary algorithms,genetic algorithms,genetic programming,cma-es,ga,gp,es,pso
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# DEAP
+
+[![Build status](https://travis-ci.org/DEAP/deap.svg?branch=master)](https://travis-ci.org/DEAP/deap) [![Download](https://img.shields.io/pypi/dm/deap.svg)](https://pypi.python.org/pypi/deap) [![Join the chat at https://gitter.im/DEAP/deap](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/DEAP/deap?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Build Status](https://dev.azure.com/fderainville/DEAP/_apis/build/status/DEAP.deap?branchName=master)](https://dev.azure.com/fderainville/DEAP/_build/latest?definitionId=1&branchName=master) [![Documentation Status](https://readthedocs.org/projects/deap/badge/?version=master)](https://deap.readthedocs.io/en/master/?badge=master)
+
+DEAP is a novel evolutionary computation framework for rapid prototyping and testing of 
+ideas. It seeks to make algorithms explicit and data structures transparent. It works in perfect harmony with parallelisation mechanisms such as multiprocessing and [SCOOP](https://github.com/soravux/scoop).
+
+DEAP includes the following features:
+
+  * Genetic algorithm using any imaginable representation
+    * List, Array, Set, Dictionary, Tree, Numpy Array, etc.
+  * Genetic programming using prefix trees
+    * Loosely typed, Strongly typed
+    * Automatically defined functions
+  * Evolution strategies (including CMA-ES)
+  * Multi-objective optimisation (NSGA-II, NSGA-III, SPEA2, MO-CMA-ES)
+  * Co-evolution (cooperative and competitive) of multiple populations
+  * Parallelization of the evaluations (and more)
+  * Hall of Fame of the best individuals that lived in the population
+  * Checkpoints that take snapshots of a system regularly
+  * Benchmarks module containing most common test functions
+  * Genealogy of an evolution (that is compatible with [NetworkX](https://github.com/networkx/networkx))
+  * Examples of alternative algorithms : Particle Swarm Optimization, Differential Evolution, Estimation of Distribution Algorithm
+
+## Downloads
+
+Following acceptance of [PEP 438](http://www.python.org/dev/peps/pep-0438/) by the Python community, we have moved DEAP's source releases on [PyPI](https://pypi.python.org).
+
+You can find the most recent releases at: https://pypi.python.org/pypi/deap/.
+
+## Documentation
+See the [DEAP User's Guide](http://deap.readthedocs.org/) for DEAP documentation.
+
+In order to get the tip documentation, change directory to the `doc` subfolder and type in `make html`, the documentation will be under `_build/html`. You will need [Sphinx](http://sphinx.pocoo.org) to build the documentation.
+
+### Notebooks
+Also checkout our new [notebook examples](https://github.com/DEAP/notebooks). Using [Jupyter notebooks](http://jupyter.org)  you'll be able to navigate and execute each block of code individually and tell what every line is doing. Either, look at the notebooks online using the notebook viewer links at the botom of the page or download the notebooks, navigate to the you download directory and run
+
+```bash
+jupyter notebook
+```
+
+## Installation
+We encourage you to use easy_install or pip to install DEAP on your system. Other installation procedure like apt-get, yum, etc. usually provide an outdated version.
+```bash
+pip install deap
+```
+
+The latest version can be installed with 
+```bash
+pip install git+https://github.com/DEAP/deap@master
+```
+
+If you wish to build from sources, download or clone the repository and type
+
+```bash
+python setup.py install
+```
+
+## Build Status
+DEAP build status is available on Travis-CI https://travis-ci.org/DEAP/deap.
+
+## Requirements
+The most basic features of DEAP requires Python2.6. In order to combine the toolbox and the multiprocessing module Python2.7 is needed for its support to pickle partial functions. CMA-ES requires Numpy, and we recommend matplotlib for visualization of results as it is fully compatible with DEAP's API.
+
+Since version 0.8, DEAP is compatible out of the box with Python 3. The installation procedure automatically translates the source to Python 3 with 2to3, however this requires having `setuptools<=58`. It is recommended to use `pip install setuptools==57.5.0` to address this issue.
+
+## Example
+
+The following code gives a quick overview how simple it is to implement the Onemax problem optimization with genetic algorithm using DEAP.  More examples are provided [here](http://deap.readthedocs.org/en/master/examples/index.html).
+
+```python
+import random
+from deap import creator, base, tools, algorithms
+
+creator.create("FitnessMax", base.Fitness, weights=(1.0,))
+creator.create("Individual", list, fitness=creator.FitnessMax)
+
+toolbox = base.Toolbox()
+
+toolbox.register("attr_bool", random.randint, 0, 1)
+toolbox.register("individual", tools.initRepeat, creator.Individual, toolbox.attr_bool, n=100)
+toolbox.register("population", tools.initRepeat, list, toolbox.individual)
+
+def evalOneMax(individual):
+    return sum(individual),
+
+toolbox.register("evaluate", evalOneMax)
+toolbox.register("mate", tools.cxTwoPoint)
+toolbox.register("mutate", tools.mutFlipBit, indpb=0.05)
+toolbox.register("select", tools.selTournament, tournsize=3)
+
+population = toolbox.population(n=300)
+
+NGEN=40
+for gen in range(NGEN):
+    offspring = algorithms.varAnd(population, toolbox, cxpb=0.5, mutpb=0.1)
+    fits = toolbox.map(toolbox.evaluate, offspring)
+    for fit, ind in zip(fits, offspring):
+        ind.fitness.values = fit
+    population = toolbox.select(offspring, k=len(population))
+top10 = tools.selBest(population, k=10)
+```
+
+## How to cite DEAP
+Authors of scientific papers including results generated using DEAP are encouraged to cite the following paper.
+
+```xml
+@article{DEAP_JMLR2012, 
+    author    = " F\'elix-Antoine Fortin and Fran\c{c}ois-Michel {De Rainville} and Marc-Andr\'e Gardner and Marc Parizeau and Christian Gagn\'e ",
+    title     = { {DEAP}: Evolutionary Algorithms Made Easy },
+    pages    = { 2171--2175 },
+    volume    = { 13 },
+    month     = { jul },
+    year      = { 2012 },
+    journal   = { Journal of Machine Learning Research }
+}
+```
+
+## Publications on DEAP
+
+  * François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP -- Enabling Nimbler Evolutions", SIGEVOlution, vol. 6, no 2, pp. 17-26, February 2014. [Paper](http://goo.gl/tOrXTp)
+  * Félix-Antoine Fortin, François-Michel De Rainville, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP: Evolutionary Algorithms Made Easy", Journal of Machine Learning Research, vol. 13, pp. 2171-2175, jul 2012. [Paper](http://goo.gl/amJ3x)
+  * François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau and Christian Gagné, "DEAP: A Python Framework for Evolutionary Algorithms", in !EvoSoft Workshop, Companion proc. of the Genetic and Evolutionary Computation Conference (GECCO 2012), July 07-11 2012. [Paper](http://goo.gl/pXXug)
+
+## Projects using DEAP
+  * Ribaric, T., & Houghten, S. (2017, June). Genetic programming for improved cryptanalysis of elliptic curve cryptosystems. In 2017 IEEE Congress on Evolutionary Computation (CEC) (pp. 419-426). IEEE.
+  * Ellefsen, Kai Olav, Herman Augusto Lepikson, and Jan C. Albiez. "Multiobjective coverage path planning: Enabling automated inspection of complex, real-world structures." Applied Soft Computing 61 (2017): 264-282.
+  * S. Chardon, B. Brangeon, E. Bozonnet, C. Inard (2016), Construction cost and energy performance of single family houses : From integrated design to automated optimization, Automation in Construction, Volume 70, p.1-13.
+  * B. Brangeon, E. Bozonnet, C. Inard (2016), Integrated refurbishment of collective housing and optimization process with real products databases, Building Simulation Optimization, pp. 531–538 Newcastle, England.
+  * Randal S. Olson, Ryan J. Urbanowicz, Peter C. Andrews, Nicole A. Lavender, La Creis Kidd, and Jason H. Moore (2016). Automating biomedical data science through tree-based pipeline optimization. Applications of Evolutionary Computation, pages 123-137.
+  * Randal S. Olson, Nathan Bartley, Ryan J. Urbanowicz, and Jason H. Moore (2016). Evaluation of a Tree-based Pipeline Optimization Tool for Automating Data Science. Proceedings of GECCO 2016, pages 485-492.
+  * Van Geit W, Gevaert M, Chindemi G, Rössert C, Courcol J, Muller EB, Schürmann F, Segev I and Markram H (2016). BluePyOpt: Leveraging open source software and cloud infrastructure to optimise model parameters in neuroscience. Front. Neuroinform. 10:17. doi: 10.3389/fninf.2016.00017 https://github.com/BlueBrain/BluePyOpt
+  * Lara-Cabrera, R., Cotta, C. and Fernández-Leiva, A.J. (2014). Geometrical vs topological measures for the evolution of aesthetic maps in a rts game, Entertainment Computing,
+  * Macret, M. and Pasquier, P. (2013). Automatic Tuning of the OP-1 Synthesizer Using a Multi-objective Genetic Algorithm. In Proceedings of the 10th Sound and Music Computing Conference (SMC). (pp 614-621).
+  * Fortin, F. A., Grenier, S., & Parizeau, M. (2013, July). Generalizing the improved run-time complexity algorithm for non-dominated sorting. In Proceeding of the fifteenth annual conference on Genetic and evolutionary computation conference (pp. 615-622). ACM.
+  * Fortin, F. A., & Parizeau, M. (2013, July). Revisiting the NSGA-II crowding-distance computation. In Proceeding of the fifteenth annual conference on Genetic and evolutionary computation conference (pp. 623-630). ACM.
+  * Marc-André Gardner, Christian Gagné, and Marc Parizeau. Estimation of Distribution Algorithm based on Hidden Markov Models for Combinatorial Optimization. in Comp. Proc. Genetic and Evolutionary Computation Conference (GECCO 2013), July 2013.
+  * J. T. Zhai, M. A. Bamakhrama, and T. Stefanov. "Exploiting Just-enough Parallelism when Mapping Streaming Applications in Hard Real-time Systems". Design Automation Conference (DAC 2013), 2013.
+  * V. Akbarzadeh, C. Gagné, M. Parizeau, M. Argany, M. A Mostafavi, "Probabilistic Sensing Model for Sensor Placement Optimization Based on Line-of-Sight Coverage", Accepted in IEEE Transactions on Instrumentation and Measurement, 2012.
+  * M. Reif, F. Shafait, and A. Dengel. "Dataset Generation for Meta-Learning". Proceedings of the German Conference on Artificial Intelligence (KI'12). 2012. 
+  * M. T. Ribeiro, A. Lacerda, A. Veloso, and N. Ziviani. "Pareto-Efficient Hybridization for Multi-Objective Recommender Systems". Proceedings of the Conference on Recommanders Systems (!RecSys'12). 2012.
+  * M. Pérez-Ortiz, A. Arauzo-Azofra, C. Hervás-Martínez, L. García-Hernández and L. Salas-Morera. "A system learning user preferences for multiobjective optimization of facility layouts". Pr,oceedings on the Int. Conference on Soft Computing Models in Industrial and Environmental Applications (SOCO'12). 2012.
+  * Lévesque, J.C., Durand, A., Gagné, C., and Sabourin, R., Multi-Objective Evolutionary Optimization for Generating Ensembles of Classifiers in the ROC Space, Genetic and Evolutionary Computation Conference (GECCO 2012), 2012.
+  * Marc-André Gardner, Christian Gagné, and Marc Parizeau, "Bloat Control in Genetic Programming with Histogram-based Accept-Reject Method", in Proc. Genetic and Evolutionary Computation Conference (GECCO 2011), 2011.
+  * Vahab Akbarzadeh, Albert Ko, Christian Gagné, and Marc Parizeau, "Topography-Aware Sensor Deployment Optimization with CMA-ES", in Proc. of Parallel Problem Solving from Nature (PPSN 2010), Springer, 2010.
+  * DEAP is used in [TPOT](https://github.com/rhiever/tpot), an open source tool that uses genetic programming to optimize machine learning pipelines.
+  * DEAP is also used in ROS as an optimization package http://www.ros.org/wiki/deap.
+  * DEAP is an optional dependency for [PyXRD](https://github.com/mathijs-dumon/PyXRD), a Python implementation of the matrix algorithm developed for the X-ray diffraction analysis of disordered lamellar structures.
+  * DEAP is used in [glyph](https://github.com/Ambrosys/glyph), a library for symbolic regression with applications to [MLC](https://en.wikipedia.org/wiki/Machine_learning_control).
+  * DEAP is used in [Sklearn-genetic-opt](https://github.com/rodrigo-arenas/Sklearn-genetic-opt), an open source tool that uses evolutionary programming to fine tune machine learning hyperparameters.
+
+If you want your project listed here, send us a link and a brief description and we'll be glad to add it.
```

### Comparing `deap-1.4.0/deap.egg-info/SOURCES.txt` & `deap-1.4.1/deap.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -213,8 +213,19 @@
 examples/gp/ant/AntSimulatorFast.cpp
 examples/gp/ant/AntSimulatorFast.hpp
 examples/gp/ant/buildAntSimFast.py
 examples/gp/ant/santafe_trail.txt
 examples/pso/basic.py
 examples/pso/basic_numpy.py
 examples/pso/multiswarm.py
-examples/pso/speciation.py
+examples/pso/speciation.py
+tests/test_algorithms.py
+tests/test_benchmarks.py
+tests/test_convergence.py
+tests/test_creator.py
+tests/test_init.py
+tests/test_logbook.py
+tests/test_multiproc.py
+tests/test_mutation.py
+tests/test_operators.py
+tests/test_pickle.py
+tests/test_statistics.py
```

### Comparing `deap-1.4.0/doc/Makefile` & `deap-1.4.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_images/constraints.png` & `deap-1.4.1/doc/_images/constraints.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_images/genealogy.png` & `deap-1.4.1/doc/_images/genealogy.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_images/gptree.png` & `deap-1.4.1/doc/_images/gptree.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_images/gptypederrtree.png` & `deap-1.4.1/doc/_images/gptypederrtree.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_images/gptypedtree.png` & `deap-1.4.1/doc/_images/gptypedtree.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_images/gptypedtrees.png` & `deap-1.4.1/doc/_images/gptypedtrees.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_images/more.png` & `deap-1.4.1/doc/_images/more.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_images/nsga3.png` & `deap-1.4.1/doc/_images/nsga3.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_images/twin_logbook.png` & `deap-1.4.1/doc/_images/twin_logbook.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/DEAP.pdf` & `deap-1.4.1/doc/_static/DEAP.pdf`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/copybutton.js` & `deap-1.4.1/doc/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/deap_icon-39x55.png` & `deap-1.4.1/doc/_static/deap_icon-39x55.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/deap_icon_16x16.ico` & `deap-1.4.1/doc/_static/deap_icon_16x16.ico`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/deap_long.png` & `deap-1.4.1/doc/_static/deap_long.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/deap_orange_icon_16x16.ico` & `deap-1.4.1/doc/_static/deap_orange_icon_16x16.ico`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/deap_orange_icon_32.ico` & `deap-1.4.1/doc/_static/deap_orange_icon_32.ico`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/lvsn.png` & `deap-1.4.1/doc/_static/lvsn.png`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/sidebar.js` & `deap-1.4.1/doc/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_static/ul.gif` & `deap-1.4.1/doc/_static/ul.gif`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_templates/indexsidebar.html` & `deap-1.4.1/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_templates/layout.html` & `deap-1.4.1/doc/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_themes/pydoctheme/static/pydoctheme.css` & `deap-1.4.1/doc/_themes/pydoctheme/static/pydoctheme.css`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/_themes/pydoctheme/theme.conf` & `deap-1.4.1/doc/_themes/pydoctheme/theme.conf`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/about.rst` & `deap-1.4.1/doc/about.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/api/algo.rst` & `deap-1.4.1/doc/api/algo.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/api/benchmarks.rst` & `deap-1.4.1/doc/api/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/api/tools.rst` & `deap-1.4.1/doc/api/tools.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/ackley.py` & `deap-1.4.1/doc/code/benchmarks/ackley.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/bohachevsky.py` & `deap-1.4.1/doc/code/benchmarks/bohachevsky.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/griewank.py` & `deap-1.4.1/doc/code/benchmarks/griewank.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/h1.py` & `deap-1.4.1/doc/code/benchmarks/h1.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/himmelblau.py` & `deap-1.4.1/doc/code/benchmarks/himmelblau.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/kursawe.py` & `deap-1.4.1/doc/code/benchmarks/kursawe.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/movingsc1.py` & `deap-1.4.1/doc/code/benchmarks/movingsc1.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/rastrigin.py` & `deap-1.4.1/doc/code/benchmarks/rastrigin.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/rosenbrock.py` & `deap-1.4.1/doc/code/benchmarks/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/schaffer.py` & `deap-1.4.1/doc/code/benchmarks/schaffer.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/schwefel.py` & `deap-1.4.1/doc/code/benchmarks/schwefel.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/benchmarks/shekel.py` & `deap-1.4.1/doc/code/benchmarks/shekel.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/examples/nsga3_ref_points.py` & `deap-1.4.1/doc/code/examples/nsga3_ref_points.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/examples/nsga3_ref_points_combined.py` & `deap-1.4.1/doc/code/examples/nsga3_ref_points_combined.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/examples/nsga3_ref_points_combined_plot.py` & `deap-1.4.1/doc/code/examples/nsga3_ref_points_combined_plot.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_1/1_where_to_start.py` & `deap-1.4.1/doc/code/tutorials/part_1/1_where_to_start.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_2_1_list_of_floats.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_2_1_list_of_floats.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_2_3_arithmetic_expression.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_2_3_arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_2_4_evolution_strategy.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_2_4_evolution_strategy.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_2_5_particle.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_2_5_particle.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_2_6_funky_one.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_2_6_funky_one.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_3_1_bag.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_3_1_bag.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_3_2_grid.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_3_2_grid.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_3_3_swarm.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_3_3_swarm.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_3_4_demes.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_3_4_demes.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_2/2_3_5_seeding_a_population.py` & `deap-1.4.1/doc/code/tutorials/part_2/2_3_5_seeding_a_population.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_3/3_6_2_tool_decoration.py` & `deap-1.4.1/doc/code/tutorials/part_3/3_6_2_tool_decoration.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_3/3_6_using_the_toolbox.py` & `deap-1.4.1/doc/code/tutorials/part_3/3_6_using_the_toolbox.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_3/3_7_variations.py` & `deap-1.4.1/doc/code/tutorials/part_3/3_7_variations.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_3/3_8_algorithms.py` & `deap-1.4.1/doc/code/tutorials/part_3/3_8_algorithms.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_3/3_next_step.py` & `deap-1.4.1/doc/code/tutorials/part_3/3_next_step.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_3/logbook.py` & `deap-1.4.1/doc/code/tutorials/part_3/logbook.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_3/multistats.py` & `deap-1.4.1/doc/code/tutorials/part_3/multistats.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_3/stats.py` & `deap-1.4.1/doc/code/tutorials/part_3/stats.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_4/4_4_Using_Cpp_NSGA.py` & `deap-1.4.1/doc/code/tutorials/part_4/4_4_Using_Cpp_NSGA.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_4/4_5_home_made_eval_func.py` & `deap-1.4.1/doc/code/tutorials/part_4/4_5_home_made_eval_func.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_4/SNC.cpp` & `deap-1.4.1/doc/code/tutorials/part_4/SNC.cpp`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/code/tutorials/part_4/sortingnetwork.py` & `deap-1.4.1/doc/code/tutorials/part_4/sortingnetwork.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/conf.py` & `deap-1.4.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/contributing.rst` & `deap-1.4.1/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/bipop_cmaes.rst` & `deap-1.4.1/doc/examples/bipop_cmaes.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/cmaes.rst` & `deap-1.4.1/doc/examples/cmaes.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/cmaes_plotting.rst` & `deap-1.4.1/doc/examples/cmaes_plotting.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/coev_coop.rst` & `deap-1.4.1/doc/examples/coev_coop.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/eda.rst` & `deap-1.4.1/doc/examples/eda.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/es_fctmin.rst` & `deap-1.4.1/doc/examples/es_fctmin.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/ga_knapsack.rst` & `deap-1.4.1/doc/examples/ga_knapsack.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/ga_onemax.rst` & `deap-1.4.1/doc/examples/ga_onemax.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/ga_onemax_numpy.rst` & `deap-1.4.1/doc/examples/ga_onemax_numpy.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/ga_onemax_short.rst` & `deap-1.4.1/doc/examples/ga_onemax_short.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/gp_ant.rst` & `deap-1.4.1/doc/examples/gp_ant.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/gp_multiplexer.rst` & `deap-1.4.1/doc/examples/gp_multiplexer.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/gp_parity.rst` & `deap-1.4.1/doc/examples/gp_parity.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/gp_spambase.rst` & `deap-1.4.1/doc/examples/gp_spambase.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/gp_symbreg.rst` & `deap-1.4.1/doc/examples/gp_symbreg.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/index.rst` & `deap-1.4.1/doc/examples/index.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/nsga3.rst` & `deap-1.4.1/doc/examples/nsga3.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/pso_basic.rst` & `deap-1.4.1/doc/examples/pso_basic.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/examples/pso_multiswarm.rst` & `deap-1.4.1/doc/examples/pso_multiswarm.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/index.rst` & `deap-1.4.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/installation.rst` & `deap-1.4.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/overview.rst` & `deap-1.4.1/doc/overview.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/porting.rst` & `deap-1.4.1/doc/porting.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/releases.rst` & `deap-1.4.1/doc/releases.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/tutorials/advanced/benchmarking.rst` & `deap-1.4.1/doc/tutorials/advanced/benchmarking.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/tutorials/advanced/checkpoint.rst` & `deap-1.4.1/doc/tutorials/advanced/checkpoint.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/tutorials/advanced/constraints.rst` & `deap-1.4.1/doc/tutorials/advanced/constraints.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/tutorials/advanced/gp.rst` & `deap-1.4.1/doc/tutorials/advanced/gp.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/tutorials/advanced/numpy.rst` & `deap-1.4.1/doc/tutorials/advanced/numpy.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/tutorials/basic/part1.rst` & `deap-1.4.1/doc/tutorials/basic/part1.rst`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 initialization function :func:`initParticle` is also registered to produce the
 individual receiving the particle class, size, domain, and speed limits as
 arguments.
 
 .. literalinclude:: /code/tutorials/part_2/2_2_5_particle.py
    :lines: 2-
 
-Calling :func:`toolbox.individual` will readily return a complete particle with
+Calling :func:`toolbox.particle` will readily return a complete particle with
 a speed vector and a fitness attribute for maximizing two objectives.
 
 .. _funky:
 
 A Funky One
 +++++++++++
 Supposing your problem has very specific needs, it is also possible to build
@@ -235,15 +235,15 @@
 visited by any particle. This is generally implemented by copying that global
 best position to a :attr:`gbest` attribute and the global best fitness to a
 :attr:`gbestfit` attribute.
 
 .. literalinclude:: /code/tutorials/part_2/2_3_3_swarm.py
    :lines: 11,23
 
-Calling :func:`toolbox.population` will readily return a complete swarm. After
+Calling :func:`toolbox.swarm` will readily return a complete swarm. After
 each evaluation the :attr:`gbest` and :attr:`gbestfit` should be set by the
 algorithm to reflect the best found position and fitness.
 
 Demes
 +++++
 A deme is a sub-population that is contained in a population. It is similar to
 an island in the island model. Demes, being only sub-populations, are in fact not
```

### Comparing `deap-1.4.0/doc/tutorials/basic/part2.rst` & `deap-1.4.1/doc/tutorials/basic/part2.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/tutorials/basic/part3.rst` & `deap-1.4.1/doc/tutorials/basic/part3.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/doc/tutorials/basic/part4.rst` & `deap-1.4.1/doc/tutorials/basic/part4.rst`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/bbob.py` & `deap-1.4.1/examples/bbob.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/coev/coop_adapt.py` & `deap-1.4.1/examples/coev/coop_adapt.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/coev/coop_base.py` & `deap-1.4.1/examples/coev/coop_base.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/coev/coop_evol.py` & `deap-1.4.1/examples/coev/coop_evol.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/coev/coop_gen.py` & `deap-1.4.1/examples/coev/coop_gen.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/coev/coop_niche.py` & `deap-1.4.1/examples/coev/coop_niche.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/coev/hillis.py` & `deap-1.4.1/examples/coev/hillis.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/coev/symbreg.py` & `deap-1.4.1/examples/coev/symbreg.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/de/basic.py` & `deap-1.4.1/examples/de/basic.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/de/dynamic.py` & `deap-1.4.1/examples/de/dynamic.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/de/sphere.py` & `deap-1.4.1/examples/de/sphere.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/eda/emna.py` & `deap-1.4.1/examples/eda/emna.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/eda/pbil.py` & `deap-1.4.1/examples/eda/pbil.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/es/cma_1+l_minfct.py` & `deap-1.4.1/examples/es/cma_1+l_minfct.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/es/cma_bipop.py` & `deap-1.4.1/examples/es/cma_bipop.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/es/cma_minfct.py` & `deap-1.4.1/examples/es/cma_minfct.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/es/cma_mo.py` & `deap-1.4.1/examples/es/cma_mo.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/es/cma_plotting.py` & `deap-1.4.1/examples/es/cma_plotting.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/es/fctmin.py` & `deap-1.4.1/examples/es/fctmin.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/es/onefifth.py` & `deap-1.4.1/examples/es/onefifth.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/evoknn.py` & `deap-1.4.1/examples/ga/evoknn.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/evoknn_jmlr.py` & `deap-1.4.1/examples/ga/evoknn_jmlr.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/evosn.py` & `deap-1.4.1/examples/ga/evosn.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/heart_scale.csv` & `deap-1.4.1/examples/ga/heart_scale.csv`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/knapsack.py` & `deap-1.4.1/examples/ga/knapsack.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/knn.py` & `deap-1.4.1/examples/ga/knn.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/kursawefct.py` & `deap-1.4.1/examples/ga/kursawefct.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/mo_rhv.py` & `deap-1.4.1/examples/ga/mo_rhv.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/nqueens.py` & `deap-1.4.1/examples/ga/nqueens.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/nsga2.py` & `deap-1.4.1/examples/ga/nsga2.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/nsga3.py` & `deap-1.4.1/examples/ga/nsga3.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/onemax.py` & `deap-1.4.1/examples/ga/onemax.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/onemax_island.py` & `deap-1.4.1/examples/ga/onemax_island.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/onemax_island_scoop.py` & `deap-1.4.1/examples/ga/onemax_island_scoop.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/onemax_mp.py` & `deap-1.4.1/examples/ga/onemax_mp.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/onemax_multidemic.py` & `deap-1.4.1/examples/ga/onemax_multidemic.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/onemax_numpy.py` & `deap-1.4.1/examples/ga/onemax_numpy.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/onemax_short.py` & `deap-1.4.1/examples/ga/onemax_short.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/pareto_front/dtlz1_front.json` & `deap-1.4.1/examples/ga/pareto_front/dtlz1_front.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/pareto_front/dtlz2_front.json` & `deap-1.4.1/examples/ga/pareto_front/dtlz2_front.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/pareto_front/dtlz3_front.json` & `deap-1.4.1/examples/ga/pareto_front/dtlz3_front.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/pareto_front/dtlz4_front.json` & `deap-1.4.1/examples/ga/pareto_front/dtlz4_front.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/pareto_front/zdt1_front.json` & `deap-1.4.1/examples/ga/pareto_front/zdt1_front.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/pareto_front/zdt2_front.json` & `deap-1.4.1/examples/ga/pareto_front/zdt2_front.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/pareto_front/zdt3_front.json` & `deap-1.4.1/examples/ga/pareto_front/zdt3_front.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/pareto_front/zdt4_front.json` & `deap-1.4.1/examples/ga/pareto_front/zdt4_front.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/pareto_front/zdt6_front.json` & `deap-1.4.1/examples/ga/pareto_front/zdt6_front.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/sortingnetwork.py` & `deap-1.4.1/examples/ga/sortingnetwork.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/tsp/gr120.json` & `deap-1.4.1/examples/ga/tsp/gr120.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/tsp/gr17.json` & `deap-1.4.1/examples/ga/tsp/gr17.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/tsp/gr24.json` & `deap-1.4.1/examples/ga/tsp/gr24.json`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/tsp.py` & `deap-1.4.1/examples/ga/tsp.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/ga/xkcd.py` & `deap-1.4.1/examples/ga/xkcd.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/__init__.py` & `deap-1.4.1/examples/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/adf_symbreg.py` & `deap-1.4.1/examples/gp/adf_symbreg.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/ant/AntSimulatorFast.cpp` & `deap-1.4.1/examples/gp/ant/AntSimulatorFast.cpp`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/ant/AntSimulatorFast.hpp` & `deap-1.4.1/examples/gp/ant/AntSimulatorFast.hpp`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/ant.py` & `deap-1.4.1/examples/gp/ant.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/multiplexer.py` & `deap-1.4.1/examples/gp/multiplexer.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/parity.py` & `deap-1.4.1/examples/gp/parity.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/spambase.csv` & `deap-1.4.1/examples/gp/spambase.csv`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/spambase.py` & `deap-1.4.1/examples/gp/spambase.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/symbreg.py` & `deap-1.4.1/examples/gp/symbreg.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/symbreg_epsilon_lexicase.py` & `deap-1.4.1/examples/gp/symbreg_epsilon_lexicase.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/symbreg_harm.py` & `deap-1.4.1/examples/gp/symbreg_harm.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/gp/symbreg_numpy.py` & `deap-1.4.1/examples/gp/symbreg_numpy.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/pso/basic.py` & `deap-1.4.1/examples/pso/basic.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/pso/basic_numpy.py` & `deap-1.4.1/examples/pso/basic_numpy.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/pso/multiswarm.py` & `deap-1.4.1/examples/pso/multiswarm.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/examples/pso/speciation.py` & `deap-1.4.1/examples/pso/speciation.py`

 * *Files identical despite different names*

### Comparing `deap-1.4.0/setup.py` & `deap-1.4.1/setup.py`

 * *Files identical despite different names*

