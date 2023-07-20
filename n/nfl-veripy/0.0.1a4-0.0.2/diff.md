# Comparing `tmp/nfl_veripy-0.0.1a4.tar.gz` & `tmp/nfl_veripy-0.0.2.tar.gz`

## Comparing `nfl_veripy-0.0.1a4.tar` & `nfl_veripy-0.0.2.tar`

### file list

```diff
@@ -1,381 +1,385 @@
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.dockerignore
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.gitlab-ci.yml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.gitmodules
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/mypy.ini
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/__init__.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/example.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/README.md
--rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator/us.pkl
--rw-r--r--   0        0        0    38879 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator/xs.pkl
--rw-r--r--   0        0        0    19521 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator2/us.pkl
--rw-r--r--   0        0        0    38881 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator2/xs.pkl
--rw-r--r--   0        0        0   200000 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/duffing/us.csv
--rw-r--r--   0        0        0   406460 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/duffing/xs.csv
--rw-r--r--   0        0        0  3585776 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/iss.mat
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/us.csv
--rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/xs.csv
--rw-r--r--   0        0        0   119223 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/quadrotor/us.pkl
--rw-r--r--   0        0        0   238287 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/quadrotor/xs.pkl
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/acc23_/testing
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/backreach.yaml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/duffing.yaml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/greedy_sim_guided.yaml
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/iss.yaml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/sim_guided.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig3a.yaml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4a.yaml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4b.yaml
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4c.yaml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig5.yaml
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp.yaml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp_partition.yaml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp.yaml
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp_partition.yaml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig4b.yaml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig5a.yaml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig5b.yaml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator.yaml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator_jit.yaml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_quadrotor.yaml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp.yaml
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp_iterate.yaml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly1.yaml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly5.yaml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/ojcsys23/di_breach.yaml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/ojcsys23/di_hybreach.yaml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/README.md
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.json
--rw-r--r--   0        0        0    59120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.h5
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.json
--rw-r--r--   0        0        0    87584 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.h5
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.json
--rw-r--r--   0        0        0   155728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.h5
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.json
--rw-r--r--   0        0        0   290336 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.h5
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.json
--rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.json
--rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.json
--rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.json
--rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.json
--rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.h5
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.json
--rw-r--r--   0        0        0    32240 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.json
--rw-r--r--   0        0        0    28736 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.json
--rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.json
--rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.json
--rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.json
--rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.json
--rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.h5
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.json
--rw-r--r--   0        0        0    35120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.json
--rw-r--r--   0        0        0    44368 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.json
--rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.h5
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.json
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/history.p
--rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.json
--rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.h5
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.json
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.h5
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.json
--rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.json
--rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/default/model.h5
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/default/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.h5
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.h5
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.json
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.h5
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.json
--rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.json
--rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/default/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/default/model.json
--rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_10_5/model.h5
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_10_5/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5/model.json
--rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.h5
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.json
--rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.h5
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.json
--rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.h5
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.json
--rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.h5
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.json
--rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.h5
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.json
--rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.h5
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.json
--rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.h5
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.json
--rw-r--r--   0        0        0    21948 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/model.h5
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/model.json
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/single_pendulum_small_controller.torch
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.json
--rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/default/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/default/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.h5
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.json
--rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.h5
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.json
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.h5
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.json
--rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.json
--rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/test/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/test/model.json
--rw-r--r--   0        0        0    43079 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_8D/intermediate_policy_0.pt
--rw-r--r--   0        0        0   300928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_8D/sim_data.npy
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.json
--rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.h5
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.json
--rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.h5
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.json
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.h5
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.json
--rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.json
--rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.json
--rw-r--r--   0        0        0   843480 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/default/model.h5
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/default/note.txt
--rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/from_pb/TinyTaxiNet.onnx
--rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/from_pb/saved_model.pb
--rw-r--r--   0        0        0     8788 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/to_pb/saved_model.pb
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/to_pb/variables/variables.data-00000-of-00001
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/to_pb/variables/variables.index
--rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.json
--rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unity/default/model.h5
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unity/default/model.json
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy/model.json
--rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy2/model.h5
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy2/model.json
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy3/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy3/model.json
--rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy4/model.h5
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy4/model.json
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/Analyzer.py
--rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/ClosedLoopAnalyzer.py
--rw-r--r--   0        0        0    19097 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/ClosedLoopBackwardAnalyzer.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/__init__.py
--rw-r--r--   0        0        0    36595 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/constraints/ClosedLoopConstraints.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/constraints/__init__.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DiscreteQuadrotor.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegrator.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegratorOutputFeedback.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegratorx4.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Duffing.py
--rw-r--r--   0        0        0    21852 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Dynamics.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/GroundRobotDI.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/GroundRobotSI.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/ISS.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/ISS_discrete.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Pendulum.py
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/QuadrotorOutputFeedback.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/QuadrotorOutputFeedback_v0.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor_8D.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor_v0.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Taxinet.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Unicycle.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Unity.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/__init__.py
--rw-r--r--   0        0        0    12768 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/elements/Element.py
--rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/elements/GuidedElement.py
--rw-r--r--   0        0        0    12723 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/elements/OptGuidedElement.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/elements/__init__.py
--rw-r--r--   0        0        0    33527 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/ClosedLoopExperiments.py
--rw-r--r--   0        0        0    36029 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/backward_experiments.py
--rw-r--r--   0        0        0    22030 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/experiments.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/expts.py
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/AdaptiveGreedySimGuidedPartitioner.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/BoundarySimGuidedPartitioner.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopGreedySimGuidedPartitioner.py
--rw-r--r--   0        0        0    19044 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopNickPartitioner.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopNoPartitioner.py
--rw-r--r--   0        0        0    28347 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopPartitioner.py
--rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopSimGuidedPartitioner.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopUnGuidedPartitioner.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopUniformPartitioner.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/GreedySimGuidedPartitioner.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/NoPartitioner.py
--rw-r--r--   0        0        0    31837 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/Partitioner.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/SimGuidedPartitioner.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/UnGuidedPartitioner.py
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/UniformPartitioner.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/AutoLIRPA.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopAUTOLIRPAPropagator.py
--rw-r--r--   0        0        0    38393 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopCROWNIBPCodebasePropagator.py
--rw-r--r--   0        0        0    36482 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopJaxVerifyPropagator.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopOVERTPropagator.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopPropagator.py
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopSDPPropagator.py
--rw-r--r--   0        0        0    10315 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopSeparablePropagator.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/CrownIBP.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/Propagator.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/SDP.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/__init__.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/alpha-beta-crown_test.py
--rw-r--r--   0        0        0    25699 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/closed_loop_verification_jax.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/controller_generation.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/create_training_dataset.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/debug_polytope.py
--rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/debug_prop.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/duffing_data_generating.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/generate_rpm_data.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/iss_data_generating.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/mpc.py
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn.py
--rw-r--r--   0        0        0    23321 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_bounds.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_closed_loop.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_jax.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/optimization_utils.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/plot_rect_prism.py
--rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/reach_sdp.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/run_overt.jl
--rw-r--r--   0        0        0    11928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/utils.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/tests/test.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/LICENSE
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/README.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0     9057 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/.dockerignore
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/.gitmodules
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/__init__.py
+-rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/example.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/online_verification.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/README.md
+-rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/double_integrator/us.pkl
+-rw-r--r--   0        0        0    38879 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/double_integrator/xs.pkl
+-rw-r--r--   0        0        0    19521 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/double_integrator2/us.pkl
+-rw-r--r--   0        0        0    38881 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/double_integrator2/xs.pkl
+-rw-r--r--   0        0        0   200000 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/duffing/us.csv
+-rw-r--r--   0        0        0   406460 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/duffing/xs.csv
+-rw-r--r--   0        0        0  3585776 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/iss/iss.mat
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/iss/us.csv
+-rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/iss/xs.csv
+-rw-r--r--   0        0        0   119223 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/quadrotor/us.pkl
+-rw-r--r--   0        0        0   238287 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/quadrotor/xs.pkl
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/acc23_/testing
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/backreach.yaml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/duffing.yaml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/greedy_sim_guided.yaml
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/iss.yaml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/sim_guided.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/cdc22/fig3a.yaml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/cdc22/fig4a.yaml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/cdc22/fig4b.yaml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/cdc22/fig4c.yaml
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/cdc22/fig5.yaml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp.yaml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp_partition.yaml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp.yaml
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp_partition.yaml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig4b.yaml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig5a.yaml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig5b.yaml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator_jit.yaml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/jax/jax_fwd_quadrotor.yaml
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp.yaml
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp_iterate.yaml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly1.yaml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly5.yaml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/ojcsys23/di_breach.yaml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/ojcsys23/di_hybreach.yaml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/README.md
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.json
+-rw-r--r--   0        0        0    59120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.h5
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.json
+-rw-r--r--   0        0        0    87584 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.h5
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.json
+-rw-r--r--   0        0        0   155728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.h5
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.json
+-rw-r--r--   0        0        0   290336 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.h5
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.json
+-rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.json
+-rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.json
+-rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.json
+-rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.json
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.h5
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.json
+-rw-r--r--   0        0        0    32240 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.json
+-rw-r--r--   0        0        0    28736 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.json
+-rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.json
+-rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.json
+-rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.json
+-rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.json
+-rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.h5
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.json
+-rw-r--r--   0        0        0    35120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.json
+-rw-r--r--   0        0        0    44368 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.json
+-rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.h5
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.json
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/history.p
+-rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.json
+-rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.h5
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.json
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.h5
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.json
+-rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.json
+-rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/default/model.h5
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/default/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.h5
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.h5
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.json
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.h5
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.json
+-rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.json
+-rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/default/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/default/model.json
+-rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_10_5/model.h5
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_10_5/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_5_5/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_5_5/model.json
+-rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.h5
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.json
+-rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.h5
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.json
+-rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.h5
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.json
+-rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.h5
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.json
+-rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.h5
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.json
+-rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.h5
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.json
+-rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.h5
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.json
+-rw-r--r--   0        0        0    21948 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Pendulum/default/model.h5
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Pendulum/default/model.json
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Pendulum/default/single_pendulum_small_controller.torch
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.json
+-rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/default/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/default/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.h5
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.json
+-rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.h5
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.json
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.h5
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.json
+-rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.json
+-rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/test/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/test/model.json
+-rw-r--r--   0        0        0    43079 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_8D/intermediate_policy_0.pt
+-rw-r--r--   0        0        0   300928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_8D/sim_data.npy
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.json
+-rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.h5
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.json
+-rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.h5
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.json
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.h5
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.json
+-rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.json
+-rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.json
+-rw-r--r--   0        0        0   843480 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/default/model.h5
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/default/note.txt
+-rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/from_pb/TinyTaxiNet.onnx
+-rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/from_pb/saved_model.pb
+-rw-r--r--   0        0        0     8788 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/to_pb/saved_model.pb
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/to_pb/variables/variables.data-00000-of-00001
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/to_pb/variables/variables.index
+-rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.json
+-rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unity/default/model.h5
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unity/default/model.json
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy/model.json
+-rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy2/model.h5
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy2/model.json
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy3/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy3/model.json
+-rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy4/model.h5
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy4/model.json
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/analyzers/Analyzer.py
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/analyzers/ClosedLoopAnalyzer.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/analyzers/ClosedLoopBackwardAnalyzer.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/analyzers/__init__.py
+-rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/constraints/Constraints.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/constraints/__init__.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/constraints/constraint_utils.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/DiscreteQuadrotor.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/DoubleIntegrator.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/DoubleIntegratorOutputFeedback.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/DoubleIntegratorx4.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Duffing.py
+-rw-r--r--   0        0        0    21852 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Dynamics.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/GroundRobotDI.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/GroundRobotSI.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/ISS.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/ISS_discrete.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Pendulum.py
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Quadrotor.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/QuadrotorOutputFeedback.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/QuadrotorOutputFeedback_v0.py
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Quadrotor_8D.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Quadrotor_v0.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Taxinet.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Unicycle.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Unity.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/dynamics/__init__.py
+-rw-r--r--   0        0        0    12768 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/elements/Element.py
+-rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/elements/GuidedElement.py
+-rw-r--r--   0        0        0    12723 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/elements/OptGuidedElement.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/elements/__init__.py
+-rw-r--r--   0        0        0    33527 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/experiments/ClosedLoopExperiments.py
+-rw-r--r--   0        0        0    36029 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/experiments/backward_experiments.py
+-rw-r--r--   0        0        0    22030 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/experiments/experiments.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/experiments/expts.py
+-rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/AdaptiveGreedySimGuidedPartitioner.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/BoundarySimGuidedPartitioner.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopGreedySimGuidedPartitioner.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopNoPartitioner.py
+-rw-r--r--   0        0        0    18567 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopPartitioner.py
+-rw-r--r--   0        0        0    12671 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopSimGuidedPartitioner.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopUnGuidedPartitioner.py
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopUniformPartitioner.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/GreedySimGuidedPartitioner.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/NoPartitioner.py
+-rw-r--r--   0        0        0    31837 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/Partitioner.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/SimGuidedPartitioner.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/UnGuidedPartitioner.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/UniformPartitioner.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/partitioners/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/AutoLIRPA.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopAUTOLIRPAPropagator.py
+-rw-r--r--   0        0        0    35966 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopCROWNIBPCodebasePropagator.py
+-rw-r--r--   0        0        0    29847 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopJaxVerifyPropagator.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopOVERTPropagator.py
+-rw-r--r--   0        0        0    13327 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopPropagator.py
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopSDPPropagator.py
+-rw-r--r--   0        0        0    10315 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopSeparablePropagator.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/CrownIBP.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/Propagator.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/SDP.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/propagators/__init__.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/alpha-beta-crown_test.py
+-rw-r--r--   0        0        0    25699 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/closed_loop_verification_jax.py
+-rw-r--r--   0        0        0    39929 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/controller_generation.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/create_training_dataset.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/debug_polytope.py
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/debug_prop.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/duffing_data_generating.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/generate_rpm_data.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/iss_data_generating.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/mpc.py
+-rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/nn.py
+-rw-r--r--   0        0        0    23321 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/nn_bounds.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/nn_closed_loop.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/nn_jax.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/optimization_utils.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/plot_rect_prism.py
+-rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/reach_sdp.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/run_overt.jl
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/utils/utils.py
+-rw-r--r--   0        0        0    14121 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/visualizers/BackwardVisualizer.py
+-rw-r--r--   0        0        0    12911 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/visualizers/ForwardVisualizer.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/src/nfl_veripy/visualizers/__init__.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/tests/test.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/tests/test_constraints.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/README.md
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 nfl_veripy-0.0.2/PKG-INFO
```

### Comparing `nfl_veripy-0.0.1a4/.gitlab-ci.yml` & `nfl_veripy-0.0.2/.gitlab-ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -18,29 +18,28 @@
 
 build_container:
   stage: build_container
   only:
     changes:
       - docker/Dockerfile
       - pyproject.toml
+      - third_party
+      - .gitlab-ci.yml
+      - .gitmodules
   script:
     - docker login -u $CI_REGISTRY_USER -p $CI_REGISTRY_PASSWORD $CI_REGISTRY
     - docker build --pull -t $CONTAINER_TEST_IMAGE -f docker/Dockerfile .
     - docker push $CONTAINER_TEST_IMAGE
 
 test_closed_loop:
   stage: test
-  # only:
-  #   changes:
-  #     - docker/Dockerfile
-  #     - nfl_veripy
   script:
     - docker login -u $CI_REGISTRY_USER -p $CI_REGISTRY_PASSWORD $CI_REGISTRY
     - docker pull $CONTAINER_TEST_IMAGE
-    - docker run -v /builds/mit-acl/ford_ugvs/nn_robustness_analysis:/home/nn_robustness_analysis $CONTAINER_TEST_IMAGE python tests/test.py
+    - docker run -v /builds/neu-autonomy/certifiable-learning/nfl_veripy:/home/nfl_veripy $CONTAINER_TEST_IMAGE python tests/test.py
 
 # release-image:
 #   stage: release
 #   script:
 #     - docker pull $CONTAINER_TEST_IMAGE
 #     - docker tag $CONTAINER_TEST_IMAGE $CONTAINER_RELEASE_IMAGE
 #     - docker push $CONTAINER_RELEASE_IMAGE
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/example.py` & `nfl_veripy-0.0.2/src/nfl_veripy/example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 """Runs a closed-loop reachability experiment according to a param file."""
 
-import argparse
-import ast
-import os
-import time
-from typing import Dict, Tuple
-
-import numpy as np
-import yaml
-
-import nfl_veripy.analyzers as analyzers
-import nfl_veripy.constraints as constraints
-import nfl_veripy.dynamics as dynamics
-from nfl_veripy.utils.nn import load_controller
+from nfl_veripy.utils.utils import suppress_unecessary_logs
+
+suppress_unecessary_logs()  # needs to happen before other imports
+
+import argparse  # noqa: E402
+import ast  # noqa: E402
+import logging  # noqa: E402
+import os  # noqa: E402
+import time  # noqa: E402
+from typing import Dict, Tuple  # noqa: E402
+
+import numpy as np  # noqa: E402
+import yaml  # noqa: E402
+
+import nfl_veripy.analyzers as analyzers  # noqa: E402
+import nfl_veripy.constraints as constraints  # noqa: E402
+import nfl_veripy.dynamics as dynamics  # noqa: E402
+from nfl_veripy.utils.nn import load_controller  # noqa: E402
+from nfl_veripy.utils.utils import get_plot_filename  # noqa: E402
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 
+logger = logging.getLogger(__name__)
+logger.setLevel(level=logging.INFO)
+
 
 def main_forward(params: dict) -> Tuple[Dict, Dict]:
     """Runs a forward reachability analysis experiment according to params."""
     np.random.seed(seed=0)
     stats = {}
 
     dyn = dynamics.get_dynamics_instance(
@@ -27,26 +36,28 @@
     )
 
     controller = load_controller(
         system=dyn.__class__.__name__,
         model_name=params["system"]["controller"],
     )
 
-    # Set up analyzer (+ parititoner + propagator)
+    # Set up analyzer (+ parititoner + propagator + visualizer)
     analyzer = analyzers.ClosedLoopAnalyzer(controller, dyn)
     analyzer.partitioner = params["analysis"]["partitioner"]
     analyzer.propagator = params["analysis"]["propagator"]
+    analyzer.visualizer = params["visualization"]
 
     initial_state_range = np.array(
         ast.literal_eval(params["analysis"]["initial_state_range"])
     )
     initial_state_set = constraints.state_range_to_constraint(
         initial_state_range, params["analysis"]["propagator"]["boundary_type"]
     )
 
+    # Run the analyzer to get reachable set estimates
     if params["analysis"]["estimate_runtime"]:
         # Run the analyzer N times to compute an estimated runtime
         times = np.empty(params["analysis"]["num_calls"])
         final_errors = np.empty(
             params["analysis"]["num_calls"], dtype=np.ndarray
         )
         avg_errors = np.empty(
@@ -55,15 +66,15 @@
         all_errors = np.empty(
             params["analysis"]["num_calls"], dtype=np.ndarray
         )
         all_reachable_sets = np.empty(
             params["analysis"]["num_calls"], dtype=object
         )
         for num in range(params["analysis"]["num_calls"]):
-            print(f"call: {num}")
+            logger.info(f"call: {num}")
             t_start = time.time()
             reachable_sets, analyzer_info = analyzer.get_reachable_set(
                 initial_state_set, t_max=params["analysis"]["t_max"]
             )
             t_end = time.time()
             times[num] = t_end - t_start
 
@@ -80,105 +91,47 @@
 
         stats["runtimes"] = times
         stats["final_step_errors"] = final_errors
         stats["avg_errors"] = avg_errors
         stats["all_errors"] = all_errors
         stats["reachable_sets"] = all_reachable_sets
 
-        print(f"All times: {times}")
-        print(f"Avg time: {times.mean()} +/- {times.std()}")
+        logger.info(f"All times: {times}")
+        logger.info(f"Avg time: {times.mean()} +/- {times.std()}")
     else:
         # Run analysis once
         t_start = time.time()
         reachable_sets, analyzer_info = analyzer.get_reachable_set(
             initial_state_set, t_max=params["analysis"]["t_max"]
         )
         t_end = time.time()
-        print(t_end - t_start)
+        logger.info(f"Runtime: {t_end - t_start} sec.")
         stats["reachable_sets"] = reachable_sets
 
+    # Calculate error of estimated reachable sets vs. true ones
     if params["analysis"]["estimate_error"]:
         final_error, avg_error, errors = analyzer.get_error(
             initial_state_set,
             reachable_sets,
             t_max=params["analysis"]["t_max"],
         )
-        print(f"Final step approximation error: {final_error}")
-        print(f"Avg errors: {avg_error}")
-        print(f"All errors: {errors}")
-
-    if params["visualization"]["save_plot"]:
-        this_file_dir = os.path.dirname(os.path.abspath(__file__))
-        save_dir = f"{this_file_dir}/results/examples/"
-        os.makedirs(save_dir, exist_ok=True)
-
-        # Ugly logic to embed parameters in filename:
-        pars = "_".join(
-            [
-                str(key) + "_" + str(value)
-                for key, value in sorted(
-                    params["analysis"]["partitioner"].items(),
-                    key=lambda kv: kv[0],
-                )
-                if key
-                not in [
-                    "make_animation",
-                    "show_animation",
-                    "type",
-                    "num_partitions",
-                ]
-            ]
-        )
-        pars2 = "_".join(
-            [
-                str(key) + "_" + str(value)
-                for key, value in sorted(
-                    params["analysis"]["propagator"].items(),
-                    key=lambda kv: kv[0],
-                )
-                if key not in ["input_shape", "type"]
-            ]
-        )
-        analyzer_info["save_name"] = (
-            save_dir
-            + dyn.name
-            + pars
-            + "_"
-            + params["analysis"]["partitioner"]["type"]
-            + "_"
-            + params["analysis"]["propagator"]["type"]
-            + "_"
-            + "tmax"
-            + "_"
-            + str(round(params["analysis"]["t_max"], 1))
-            + "_"
-            + params["analysis"]["propagator"]["boundary_type"]
-        )
-        if len(pars2) > 0:
-            analyzer_info["save_name"] = (
-                analyzer_info["save_name"] + "_" + pars2
-            )
-        analyzer_info["save_name"] = analyzer_info["save_name"] + ".png"
+        logger.info(f"Final step approximation error: {final_error}")
+        logger.info(f"Avg errors: {avg_error}")
+        logger.info(f"All errors: {errors}")
 
+    # Visualize the reachable sets and MC samples
     if (
         params["visualization"]["show_plot"]
         or params["visualization"]["save_plot"]
     ):
+        analyzer.visualizer.plot_filename = get_plot_filename(params)
         analyzer.visualize(
             initial_state_set,
             reachable_sets,
-            show_samples=params["visualization"]["show_samples"],
-            show_trajectories=params["visualization"]["show_trajectories"],
-            show=params["visualization"]["show_plot"],
-            axis_dims=[[a] for a in params["visualization"]["plot_dims"]],
-            axis_labels=params["visualization"]["plot_axis_labels"],
-            aspect=params["visualization"]["plot_aspect"],
-            plot_lims=params["visualization"]["plot_lims"],
-            iteration=None,
-            controller_name=None,
+            analyzer.propagator.network,
             **analyzer_info,
         )
 
     return stats, analyzer_info
 
 
 def main_backward(params: dict) -> tuple[dict, dict]:
@@ -201,14 +154,15 @@
         model_name=params["system"]["controller"],
     )
 
     # Set up analyzer (+ parititoner + propagator)
     analyzer = analyzers.ClosedLoopBackwardAnalyzer(controller, dyn)
     analyzer.partitioner = params["analysis"]["partitioner"]
     analyzer.propagator = params["analysis"]["propagator"]
+    analyzer.visualizer = params["visualization"]
 
     final_state_range = np.array(
         ast.literal_eval(params["analysis"]["final_state_range"])
     )
     target_set = constraints.state_range_to_constraint(
         final_state_range, params["analysis"]["propagator"]["boundary_type"]
     )
@@ -225,15 +179,15 @@
             params["analysis"]["num_calls"], dtype=np.ndarray
         )
         all_backprojection_sets = np.empty(
             params["analysis"]["num_calls"], dtype=object
         )
         target_sets = np.empty(params["analysis"]["num_calls"], dtype=object)
         for num in range(params["analysis"]["num_calls"]):
-            print(f"call: {num}")
+            logger.info(f"call: {num}")
             t_start = time.time()
             (
                 backprojection_sets,
                 analyzer_info,
             ) = analyzer.get_backprojection_set(
                 target_set,
                 t_max=params["analysis"]["t_max"],
@@ -263,121 +217,39 @@
         stats["final_step_errors"] = final_errors
         stats["avg_errors"] = avg_errors
         stats["all_errors"] = all_errors
         stats["all_backprojection_sets"] = all_backprojection_sets
         stats["target_sets"] = target_sets
         stats["avg_runtime"] = times.mean()
 
-        print(f"All times: {times}")
-        print(f"Avg time: {times.mean()} +/- {times.std()}")
-        print(f"Final Error: {final_errors[-1]}")
-        print(f"Avg Error: {avg_errors[-1]}")
+        logger.info(f"All times: {times}")
+        logger.info(f"Avg time: {times.mean()} +/- {times.std()}")
+        logger.info(f"Final Error: {final_errors[-1]}")
+        logger.info(f"Avg Error: {avg_errors[-1]}")
     else:
         # Run analysis once
         # Run analysis & generate a plot
         backprojection_sets, analyzer_info = analyzer.get_backprojection_set(
             target_set,
             t_max=params["analysis"]["t_max"],
             overapprox=params["analysis"]["overapprox"],
         )
         stats["backprojection_sets"] = backprojection_sets
 
-    controller_name = None
-    if params["visualization"]["show_policy"]:
-        controller_name = params["system"]["controller"]
-
-    if params["visualization"]["save_plot"]:
-        this_file_dir = os.path.dirname(os.path.abspath(__file__))
-        save_dir = f"{this_file_dir}/results/examples_backward/"
-        os.makedirs(save_dir, exist_ok=True)
-
-        # Ugly logic to embed parameters in filename:
-        pars = "_".join(
-            [
-                str(key) + "_" + str(value)
-                for key, value in sorted(
-                    params["analysis"]["partitioner"].items(),
-                    key=lambda kv: kv[0],
-                )
-                if key
-                not in [
-                    "make_animation",
-                    "show_animation",
-                    "type",
-                    "num_partitions",
-                ]
-            ]
-        )
-        pars2 = "_".join(
-            [
-                str(key) + "_" + str(value)
-                for key, value in sorted(
-                    params["analysis"]["propagator"].items(),
-                    key=lambda kv: kv[0],
-                )
-                if key not in ["input_shape", "type"]
-            ]
-        )
-        analyzer_info["save_name"] = (
-            save_dir
-            + params["system"]["type"]
-            + pars
-            + "_"
-            + params["analysis"]["partitioner"]["type"]
-            + "_"
-            + params["analysis"]["propagator"]["type"]
-            + "_"
-            # + "tmax"
-            # + "_"
-            # + str(round(params["analysis"]["t_max"], 1))
-            # + "_"
-            + params["analysis"]["propagator"]["boundary_type"]
-            + "_"
-            # + str(params["analysis"]["propagator"]["num_polytope_facets"])
-            # + "_"
-            + "partitions"
-            + "_"
-            # + np.array2string(num_partitions, separator='_')[1:-1]
-        )
-        if len(pars2) > 0:
-            analyzer_info["save_name"] = (
-                analyzer_info["save_name"] + "_" + pars2
-            )
-        analyzer_info["save_name"] = analyzer_info["save_name"] + ".png"
-
-    if params["analysis"].get("initial_state_range", None) is None:
-        initial_state_set = None
-    else:
-        initial_state_range = np.array(
-            ast.literal_eval(params["analysis"]["initial_state_range"])
-        )
-        initial_state_set = constraints.LpConstraint(initial_state_range)
-
+    # Visualize the reachable sets and MC samples
     if (
         params["visualization"]["show_plot"]
         or params["visualization"]["save_plot"]
     ):
+        analyzer.visualizer.plot_filename = get_plot_filename(params)
         analyzer.visualize(
-            backprojection_sets,
             target_set,
-            analyzer_info,
-            show=params["visualization"]["show_plot"],
-            show_samples=params["visualization"]["show_samples"],
-            show_samples_from_cells=params["visualization"][
-                "show_samples_from_cells"
-            ],
-            show_trajectories=params["visualization"]["show_trajectories"],
-            show_convex_hulls=params["visualization"]["show_convex_hulls"],
-            axis_dims=params["visualization"]["plot_dims"],
-            axis_labels=params["visualization"]["plot_axis_labels"],
-            aspect=params["visualization"]["plot_aspect"],
-            plot_lims=params["visualization"]["plot_lims"],
-            initial_constraint=initial_state_set,
-            controller_name=controller_name,
-            show_BReach=params["visualization"]["show_BReach"],
+            backprojection_sets,
+            analyzer.propagator.network,
+            **analyzer_info,
         )
 
     return stats, analyzer_info
 
 
 def setup_parser() -> dict:
     """Load yaml config file with experiment params."""
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator/us.pkl` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/double_integrator/us.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator/xs.pkl` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/double_integrator/xs.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator2/us.pkl` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/double_integrator2/us.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator2/xs.pkl` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/double_integrator2/xs.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/duffing/us.csv` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/duffing/us.csv`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/duffing/xs.csv` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/duffing/xs.csv`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/iss.mat` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/iss/iss.mat`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/us.csv` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/iss/us.csv`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/xs.csv` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/iss/xs.csv`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/quadrotor/us.pkl` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/quadrotor/us.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/quadrotor/xs.pkl` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/datasets/quadrotor/xs.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/acc23_/testing` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/acc23_/testing`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/backreach.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/backreach.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -18,17 +18,21 @@
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
-  show_samples: false
-  show_trajectories: false
   plot_dims: [0, 1]
   plot_axis_labels: ["$x_0$", "$x_1$"]
   plot_aspect: auto
   plot_lims: "[[1.8,3.2],[-0.3,1.3]]"
   show_policy: false
   show_samples_from_cells: true
-  show_convex_hulls: true
-  show_BReach: false
+  show_trajectories: false
+  show_backreachable_sets: false
+  show_true_backprojection_sets: true
+  show_target_set: true
+  show_true_backprojection_set_samples: false
+  show_policy: false
+  show_backprojection_sets: true
+  show_backprojection_set_cells: true
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/duffing.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/duffing.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/greedy_sim_guided.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/greedy_sim_guided.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/iss.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/iss.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/sim_guided.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   type: DoubleIntegrator
   feedback: FullState
   controller: default
 
 analysis:
   reachability_direction: forward
   partitioner:
-    type: SimGuided
+    type: None
   propagator:
     type: CROWN
     boundary_type: rectangle
   initial_state_range: "[[2.5, 3.0], [-0.25, 0.25]]"
   t_max: 2
   estimate_runtime: false
   estimate_error: false
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig3a.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/cdc22/fig4b.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 system:
-  type: DoubleIntegrator
+  type: GroundRobot
   feedback: FullState
-  controller: default
+  controller: complex_potential_field
 
 analysis:
-  reachability_direction: backward
+  reachability_direction: forward
   partitioner:
     type: Uniform
     num_partitions: "[4, 4]"
   propagator:
-    type: CROWNNStep
+    type: CROWN
     boundary_type: rectangle
-  final_state_range: "[[2.5,3.0],[-0.25,0.25]]"
-  overapprox: true
-  t_max: 5
+  initial_state_range: "[[-5.5,-4.5],[-0.5,0.5]]"
+  t_max: 9
   estimate_runtime: false
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
   show_samples: false
-  show_trajectories: false
+  show_trajectories: true
   plot_dims: [0, 1]
-  plot_axis_labels: ["$x_0$", "$x_1$"]
+  plot_axis_labels: ["$p_x$", "$p_y$"]
   plot_aspect: auto
-  plot_lims: "[[-3.8,5.64],[-0.64,2.5]]"
-  show_policy: false
-  show_samples_from_cells: true
-  show_convex_hulls: true
-  show_BReach: true
+  plot_lims: "[[-7.2,3],[-7.2,7.2]]"
+  show_policy: true
+  final_state_range: "[[-1,1],[-1,1]]"
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4a.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/cdc22/fig4a.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4b.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/cdc22/fig3a.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 system:
-  type: GroundRobot
+  type: DoubleIntegrator
   feedback: FullState
-  controller: complex_potential_field
+  controller: default
 
 analysis:
-  reachability_direction: forward
+  reachability_direction: backward
   partitioner:
     type: Uniform
     num_partitions: "[4, 4]"
   propagator:
-    type: CROWN
+    type: CROWNNStep
     boundary_type: rectangle
-  initial_state_range: "[[-5.5,-4.5],[-0.5,0.5]]"
-  t_max: 9
+  final_state_range: "[[2.5,3.0],[-0.25,0.25]]"
+  overapprox: true
+  t_max: 5
   estimate_runtime: false
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
-  show_samples: false
-  show_trajectories: true
   plot_dims: [0, 1]
-  plot_axis_labels: ["$p_x$", "$p_y$"]
+  plot_axis_labels: ["$x_0$", "$x_1$"]
   plot_aspect: auto
-  plot_lims: "[[-7.2,3],[-7.2,7.2]]"
-  show_policy: true
-  final_state_range: "[[-1,1],[-1,1]]"
+  plot_lims: "[[-3.8,5.64],[-0.64,2.5]]"
+  show_policy: false
+  show_trajectories: false
+  show_samples_from_cells: false
+  show_backreachable_sets: false
+  show_true_backprojection_sets: true
+  show_target_set: true
+  show_true_backprojection_set_samples: true
+  show_backprojection_sets: true
+  show_backprojection_set_cells: true
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4c.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig5b.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 system:
-  type: GroundRobot
-  feedback: FullState
-  controller: complex_potential_field
+  type: Quadrotor_v0
+  feedback: OutputFeedback
+  controller: default
 
 analysis:
-  reachability_direction: backward
+  reachability_direction: forward
   partitioner:
-    type: Uniform
-    num_partitions: "[4, 4]"
+    type: None
   propagator:
     type: CROWN
     boundary_type: rectangle
-  final_state_range: "[[-1,1],[-1,1]]"
-  overapprox: true
-  t_max: 9
+  initial_state_range: "[[4.65, 4.75], [4.65, 4.75], [2.95, 3.05], [0.94, 0.96], [-0.01, 0.01], [-0.01, 0.01]]"
+  t_max: 0.2
   estimate_runtime: false
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
-  show_samples: false
-  show_trajectories: true
-  plot_dims: [0, 1]
-  plot_axis_labels: ["$p_x$", "$p_y$"]
-  plot_aspect: auto
-  plot_lims: "[[-7.2,3],[-7.2,7.2]]"
-  show_policy: false
-  show_samples_from_cells: false
-  show_convex_hulls: false
-  show_BReach: false
-  initial_state_range: "[[-5.5,-4.5],[.5,1.5]]"
-
+  show_samples: true
+  show_trajectories: false
+  plot_dims: [0, 1, 2]
+  plot_axis_labels: ["$x$", "$y$", "$z$"]
+  plot_aspect: equal
+  plot_lims: null
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig5.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/cdc22/fig4c.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 system:
   type: GroundRobot
   feedback: FullState
-  controller: buggy_complex_potential_field
+  controller: complex_potential_field
 
 analysis:
   reachability_direction: backward
   partitioner:
     type: Uniform
-    num_partitions: "[8, 8]"
+    num_partitions: "[4, 4]"
   propagator:
-    type: CROWNNStep
+    type: CROWN
     boundary_type: rectangle
   final_state_range: "[[-1,1],[-1,1]]"
   overapprox: true
-  t_max: 6
+  t_max: 9
   estimate_runtime: false
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
-  show_samples: false
-  show_trajectories: true
   plot_dims: [0, 1]
   plot_axis_labels: ["$p_x$", "$p_y$"]
   plot_aspect: auto
   plot_lims: "[[-7.2,3],[-7.2,7.2]]"
-  show_policy: true
-  show_samples_from_cells: false
-  show_convex_hulls: false
-  show_BReach: false
   initial_state_range: "[[-5.5,-4.5],[.5,1.5]]"
+  show_trajectories: true
+  show_samples_from_cells: false
+  show_backreachable_sets: false
+  show_true_backprojection_sets: false
+  show_target_set: true
+  show_true_backprojection_set_samples: false
+  show_policy: true
+  show_backprojection_sets: true
+  show_backprojection_set_cells: false
+
+
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   controller: default
 
 analysis:
   reachability_direction: forward
   partitioner:
     type: None
   propagator:
-    type: CROWN
+    type: SDP
     boundary_type: rectangle
   initial_state_range: "[[2.5, 3.0], [-0.25, 0.25]]"
   t_max: 2
   estimate_runtime: false
   estimate_error: false
 
 visualization:
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp_partition.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp_partition.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
   controller: default
 
 analysis:
   reachability_direction: forward
   partitioner:
     type: None
   propagator:
-    type: SDP
+    type: JaxCROWNUnrolled
     boundary_type: rectangle
   initial_state_range: "[[2.5, 3.0], [-0.25, 0.25]]"
-  t_max: 2
+  t_max: 5
   estimate_runtime: false
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp_partition.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp_partition.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig4b.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig4b.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig5a.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/icra21/fig5a.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig5b.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator_jit.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 system:
-  type: Quadrotor_v0
-  feedback: OutputFeedback
+  type: DoubleIntegrator
+  feedback: FullState
   controller: default
 
 analysis:
   reachability_direction: forward
   partitioner:
     type: None
   propagator:
-    type: CROWN
+    type: JaxUnrolledJitted
     boundary_type: rectangle
-  initial_state_range: "[[4.65, 4.75], [4.65, 4.75], [2.95, 3.05], [0.94, 0.96], [-0.01, 0.01], [-0.01, 0.01]]"
-  t_max: 0.2
-  estimate_runtime: false
+  initial_state_range: "[[2.5, 3.0], [-0.25, 0.25]]"
+  t_max: 5
+  estimate_runtime: true
+  num_calls: 20
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
   show_samples: true
   show_trajectories: false
-  plot_dims: [0, 1, 2]
-  plot_axis_labels: ["$x$", "$y$", "$z$"]
-  plot_aspect: equal
+  plot_dims: [0, 1]
+  plot_axis_labels: ["$x_0$", "$x_1$"]
+  plot_aspect: auto
   plot_lims: null
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/jax/jax_fwd_quadrotor.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 system:
-  type: DoubleIntegrator
+  type: Quadrotor_v0
   feedback: FullState
   controller: default
 
 analysis:
   reachability_direction: forward
   partitioner:
     type: None
   propagator:
     type: JaxCROWNUnrolled
     boundary_type: rectangle
-  initial_state_range: "[[2.5, 3.0], [-0.25, 0.25]]"
-  t_max: 5
+  initial_state_range: "[[4.65, 4.75], [4.65, 4.75], [2.95, 3.05], [0.94, 0.96], [-0.01, 0.01], [-0.01, 0.01]]"
+  t_max: 0.5
   estimate_runtime: false
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator_jit.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/access21/sim_guided.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,28 @@
   type: DoubleIntegrator
   feedback: FullState
   controller: default
 
 analysis:
   reachability_direction: forward
   partitioner:
-    type: None
+    type: SimGuided
   propagator:
-    type: JaxUnrolledJitted
+    type: CROWN
     boundary_type: rectangle
   initial_state_range: "[[2.5, 3.0], [-0.25, 0.25]]"
-  t_max: 5
-  estimate_runtime: true
-  num_calls: 20
+  t_max: 2
+  estimate_runtime: false
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
   show_samples: true
   show_trajectories: false
+  show_reachable_set_cells: false
   plot_dims: [0, 1]
   plot_axis_labels: ["$x_0$", "$x_1$"]
   plot_aspect: auto
   plot_lims: null
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp_iterate.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp_iterate.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -18,17 +18,20 @@
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
-  show_samples: false
-  show_trajectories: false
   plot_dims: [0, 1]
   plot_axis_labels: ["$x_0$", "$x_1$"]
   plot_aspect: auto
   plot_lims: "[[-3.8,5.64],[-0.64,2.5]]"
   show_policy: false
+  show_trajectories: false
   show_samples_from_cells: false
-  show_convex_hulls: true
-  show_BReach: false
+  show_backreachable_sets: false
+  show_true_backprojection_sets: true
+  show_target_set: true
+  show_true_backprojection_set_samples: false
+  show_backprojection_sets: true
+  show_backprojection_set_cells: false
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly1.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly1.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -18,17 +18,20 @@
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
-  show_samples: false
-  show_trajectories: false
   plot_dims: [0, 1]
   plot_axis_labels: ["$x_0$", "$x_1$"]
   plot_aspect: auto
   plot_lims: "[[-3.8,5.64],[-0.64,2.5]]"
   show_policy: false
+  show_trajectories: false
   show_samples_from_cells: false
-  show_convex_hulls: true
-  show_BReach: false
+  show_backreachable_sets: false
+  show_true_backprojection_sets: true
+  show_target_set: true
+  show_true_backprojection_set_samples: false
+  show_backprojection_sets: true
+  show_backprojection_set_cells: false
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly5.yaml` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly5.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -18,17 +18,20 @@
   estimate_error: false
 
 visualization:
   save_plot: true
   show_plot: false
   make_animation: false
   show_animation: false
-  show_samples: false
-  show_trajectories: false
   plot_dims: [0, 1]
   plot_axis_labels: ["$x_0$", "$x_1$"]
   plot_aspect: auto
   plot_lims: "[[-3.8,5.64],[-0.64,2.5]]"
   show_policy: false
+  show_trajectories: false
   show_samples_from_cells: false
-  show_convex_hulls: true
-  show_BReach: false
+  show_backreachable_sets: false
+  show_true_backprojection_sets: true
+  show_target_set: true
+  show_true_backprojection_set_samples: false
+  show_backprojection_sets: true
+  show_backprojection_set_cells: false
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/history.p` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/history.p`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/default/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/default/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/default/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/default/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_10_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_10_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Pendulum/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Pendulum/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/single_pendulum_small_controller.torch` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Pendulum/default/single_pendulum_small_controller.torch`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/default/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/default/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/test/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/test/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/test/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor/test/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_8D/intermediate_policy_0.pt` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_8D/intermediate_policy_0.pt`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_8D/sim_data.npy` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_8D/sim_data.npy`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/default/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/from_pb/TinyTaxiNet.onnx` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/from_pb/TinyTaxiNet.onnx`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/from_pb/saved_model.pb` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/from_pb/saved_model.pb`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/to_pb/saved_model.pb` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Taxinet/to_pb/saved_model.pb`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unity/default/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unity/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unity/default/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/Unity/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy2/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy2/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy3/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy3/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy4/model.h5` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy4/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy4/model.json` & `nfl_veripy-0.0.2/src/nfl_veripy/_static/models/debug/corner_policy4/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/Analyzer.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopUniformPartitioner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,188 +1,173 @@
-import inspect
+import ast
+from itertools import product
+from typing import Any, Optional
 
-import matplotlib.pyplot as plt
-from scipy.spatial import ConvexHull
+import numpy as np
 
-import nfl_veripy.partitioners as partitioners
+import nfl_veripy.constraints as constraints
+import nfl_veripy.dynamics as dynamics
 import nfl_veripy.propagators as propagators
-from nfl_veripy.utils.utils import get_sampled_outputs, samples_to_range
+from nfl_veripy.utils.utils import get_crown_matrices
 
-plt.rcParams["mathtext.fontset"] = "stix"
-plt.rcParams["font.family"] = "STIXGeneral"
-plt.rcParams["font.size"] = "20"
+from .ClosedLoopPartitioner import ClosedLoopPartitioner
 
 
-class Analyzer:
-    def __init__(self, torch_model):
-        self.torch_model = torch_model
-
-        self.partitioner = None
-        self.propagator = None
-
-    @property
-    def partitioner_dict(self):
-        return partitioners.partitioner_dict
+class ClosedLoopUniformPartitioner(ClosedLoopPartitioner):
+    def __init__(
+        self,
+        dynamics: dynamics.Dynamics,
+    ):
+        super().__init__(dynamics=dynamics)
+        self.num_partitions: np.ndarray = np.array([4, 4])
+        self.interior_condition: str = "linf"
 
     @property
-    def propagator_dict(self):
-        return propagators.propagator_dict
+    def num_partitions(self):
+        return self._num_partitions
 
-    @property
-    def partitioner(self):
-        return self._partitioner
+    @num_partitions.setter
+    def num_partitions(self, value):
+        if type(value) == np.ndarray:
+            self._num_partitions = value
+        elif type(value) == str:
+            self._num_partitions = np.array(ast.literal_eval(value))
 
-    @partitioner.setter
-    def partitioner(self, hyperparams):
-        if hyperparams is None:
-            return
-
-        hyperparams_ = hyperparams.copy()
-        partitioner = hyperparams_.pop("type", None)
-
-        # Make sure we don't send any args to a partitioner that can't handle
-        # them. e.g, don't give NoPartitioner a time budget
-        args = inspect.getfullargspec(self.partitioner_dict[partitioner]).args
-        for hyperparam in hyperparams:
-            if hyperparam not in args:
-                hyperparams_.pop(hyperparam, None)
+    def get_one_step_reachable_set(
+        self,
+        initial_set: constraints.SingleTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
+        num_partitions: Optional[np.ndarray] = None,
+    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
+        reachable_set, info = self.get_reachable_set(
+            initial_set,
+            propagator,
+            t_max=1,
+        )
+        return reachable_set.get_constraint_at_time_index(0), info
 
-        self._partitioner = self.instantiate_partitioner(
-            partitioner, hyperparams_
+    def get_reachable_set(
+        self,
+        initial_set: constraints.SingleTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
+        t_max: int,
+    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
+        reachable_sets = constraints.create_empty_multi_timestep_constraint(
+            propagator.boundary_type, num_facets=propagator.num_polytope_facets
         )
 
-    def instantiate_partitioner(self, partitioner, hyperparams):
-        return self.partitioner_dict[partitioner](**hyperparams)
+        input_range = initial_set.to_range()
 
-    @property
-    def propagator(self):
-        return self._propagator
+        info = {}  # type: dict[str, Any]
+        num_propagator_calls = 0
 
-    @propagator.setter
-    def propagator(self, hyperparams):
-        if hyperparams is None:
-            return
-        hyperparams_ = hyperparams.copy()
-        propagator = hyperparams_.pop("type", None)
-
-        # Make sure we don't send any args to a propagator that can't handle
-        # them.
-        args = inspect.getfullargspec(self.propagator_dict[propagator]).args
-        for hyperparam in hyperparams:
-            if hyperparam not in args:
-                hyperparams_.pop(hyperparam, None)
-
-        self._propagator = self.instantiate_propagator(
-            propagator, hyperparams_
-        )
-        if propagator is not None:
-            self._propagator.network = self.torch_model
-
-    def instantiate_propagator(self, propagator, hyperparams):
-        return self.propagator_dict[propagator](**hyperparams)
-
-    def get_output_range(self, input_range, verbose=False):
-        output_range, info = self.partitioner.get_output_range(
-            input_range, self.propagator
+        slope = np.divide(
+            (input_range[..., 1] - input_range[..., 0]), self.num_partitions
         )
-        return output_range, info
 
-    def visualize(
-        self,
-        input_range,
-        output_range_estimate,
-        show=True,
-        show_samples=True,
-        show_legend=True,
-        show_input=True,
-        show_output=True,
-        title=None,
-        labels={},
-        aspects={},
-        **kwargs
-    ):
-        # sampled_outputs = self.get_sampled_outputs(input_range)
-        # output_range_exact = self.samples_to_range(sampled_outputs)
+        ranges = []
 
-        self.partitioner.setup_visualization(
-            input_range,
-            output_range_estimate,
-            self.propagator,
-            show_samples=show_samples,
-            inputs_to_highlight=kwargs.get("inputs_to_highlight", None),
-            outputs_to_highlight=kwargs.get("outputs_to_highlight", None),
-            show_input=show_input,
-            show_output=show_output,
-            labels=labels,
-            aspects=aspects,
-        )
-        self.partitioner.visualize(
-            kwargs.get(
-                "exterior_partitions", kwargs.get("all_partitions", [])
-            ),
-            kwargs.get("interior_partitions", []),
-            output_range_estimate,
-            show_input=show_input,
-            show_output=show_output,
-        )
-
-        if show_legend:
-            if show_input:
-                self.partitioner.input_axis.legend(
-                    bbox_to_anchor=(0, 1.02, 1, 0.2),
-                    loc="lower left",
-                    mode="expand",
-                    borderaxespad=0,
-                    ncol=1,
-                )
-            if show_output:
-                self.partitioner.output_axis.legend(
-                    bbox_to_anchor=(0, 1.02, 1, 0.2),
-                    loc="lower left",
-                    mode="expand",
-                    borderaxespad=0,
-                    ncol=2,
-                )
+        for element in product(
+            *[range(num) for num in self.num_partitions.flatten()]
+        ):
+            element_this_cell = np.array(element)
+            input_range_this_cell = np.empty_like(input_range)
+            input_range_this_cell[..., 0] = input_range[..., 0] + np.multiply(
+                element_this_cell, slope
+            )
+            input_range_this_cell[..., 1] = input_range[..., 0] + np.multiply(
+                element_this_cell + 1, slope
+            )
 
-        if title is not None:
-            plt.title(title)
+            initial_set_this_cell = initial_set.get_cell(input_range_this_cell)
 
-        plt.tight_layout()
+            reachable_sets_this_cell, info_this_cell = (
+                propagator.get_reachable_set(initial_set_this_cell, t_max)
+            )
+            num_propagator_calls += t_max
+            info["nn_matrices"] = info_this_cell
 
-        if "save_name" in kwargs and kwargs["save_name"] is not None:
-            plt.savefig(kwargs["save_name"])
+            reachable_sets.add_cell(reachable_sets_this_cell)
+            ranges.append((input_range_this_cell, reachable_sets_this_cell))
 
-        if show:
-            plt.show()
-        else:
-            plt.close()
+        reachable_sets.update_main_constraint_with_cells(overapprox=True)
 
-    def get_sampled_outputs(self, input_range, N=1000):
-        return get_sampled_outputs(input_range, self.propagator, N=N)
+        info["all_partitions"] = ranges
+        info["num_propagator_calls"] = num_propagator_calls
+        info["num_partitions"] = np.product(self.num_partitions)
 
-    def samples_to_range(self, sampled_outputs):
-        return samples_to_range(sampled_outputs)
+        return reachable_sets, info
 
-    def get_exact_output_range(self, input_range, N=int(1e4)):
-        sampled_outputs = self.get_sampled_outputs(input_range, N=N)
-        output_range = self.samples_to_range(sampled_outputs)
-        return output_range
+    def get_one_step_backprojection_set(
+        self,
+        target_sets: constraints.MultiTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
+        overapprox: bool = False,
+    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
+        backreachable_set, info = self.get_one_step_backreachable_set(
+            target_sets.get_constraint_at_time_index(-1)
+        )
+        info["backreachable_set"] = backreachable_set
 
-    def get_exact_hull(self, input_range, N=int(1e4)):
-        sampled_outputs = self.get_sampled_outputs(input_range, N=N)
-        return ConvexHull(sampled_outputs)
+        backprojection_set = constraints.create_empty_constraint(
+            boundary_type=propagator.boundary_type,
+            num_facets=propagator.num_polytope_facets,
+        )
+
+        """
+        Partition the backreachable set (xt).
+        For each cell in the partition:
+        - relax the NN (use CROWN to compute matrices for affine bounds)
+        - use the relaxed NN to compute bounds on xt1
+        - use those bounds to define constraints on xt, and if valid, add
+            to backprojection_set
+        """
+
+        # Setup the partitions
+        assert backreachable_set.range is not None
+        input_range = backreachable_set.range
+        slope = np.divide(
+            (input_range[..., 1] - input_range[..., 0]), self.num_partitions
+        )
 
-    def get_error(self, input_range, output_range, **analyzer_info):
-        if self.partitioner.interior_condition == "convex_hull":
-            exact_hull = self.get_exact_hull(input_range)
+        # Iterate through each partition
+        for element in product(
+            *[range(int(num)) for num in self.num_partitions.flatten()]
+        ):
+            # Compute this partition's min/max xt values
+            element_this_cell = np.array(element)
+            ranges = np.empty_like(input_range)
+            ranges[:, 0] = input_range[:, 0] + np.multiply(
+                element_this_cell, slope
+            )
+            ranges[:, 1] = input_range[:, 0] + np.multiply(
+                element_this_cell + 1, slope
+            )
+            backreachable_set_this_cell = constraints.LpConstraint(
+                range=ranges, p=np.inf
+            )
 
-            error = self.partitioner.get_error(
-                exact_hull, analyzer_info["estimated_hull"]
+            backprojection_set_this_cell, this_info = (
+                propagator.get_one_step_backprojection_set(
+                    backreachable_set_this_cell,
+                    target_sets,
+                    overapprox=overapprox,
+                )
             )
-        elif self.partitioner.interior_condition in ["lower_bnds", "linf"]:
-            output_range_exact = self.get_exact_output_range(input_range)
+            backprojection_set.add_cell(
+                backprojection_set_this_cell  # type: ignore
+            )
+
+        backprojection_set.update_main_constraint_with_cells(
+            overapprox=overapprox
+        )
 
-            error = self.partitioner.get_error(
-                output_range_exact, output_range
+        if overapprox:
+            # These will be used to further backproject this set in time
+            backprojection_set.crown_matrices = get_crown_matrices(
+                propagator,
+                backprojection_set,
+                self.dynamics.num_inputs,
+                self.dynamics.sensor_noise,
             )
 
-        return error
+        return backprojection_set, info
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/ClosedLoopBackwardAnalyzer.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopPartitioner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,535 +1,487 @@
-import ast
 from copy import deepcopy
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
-import matplotlib
-import matplotlib.pyplot as plt
+import cvxpy as cp
 import numpy as np
-import torch
+import pypoman
 from scipy.spatial import ConvexHull
 
-import nfl_veripy.analyzers as analyzers
 import nfl_veripy.constraints as constraints
 import nfl_veripy.dynamics as dynamics
-import nfl_veripy.partitioners as partitioners
 import nfl_veripy.propagators as propagators
-from nfl_veripy.utils.utils import get_sampled_outputs, samples_to_range
+from nfl_veripy.utils.optimization_utils import optimize_over_all_states
+from nfl_veripy.utils.utils import range_to_polytope
 
-# plt.rcParams['mathtext.fontset'] = 'stix'
-# plt.rcParams['font.family'] = 'STIXGeneral'
 
-
-class ClosedLoopBackwardAnalyzer(analyzers.Analyzer):
-    def __init__(
-        self, torch_model: torch.nn.Sequential, dynamics: dynamics.Dynamics
-    ):
-        self.torch_model = torch_model
+class ClosedLoopPartitioner:
+    def __init__(self, dynamics: dynamics.Dynamics):
         self.dynamics = dynamics
-        analyzers.Analyzer.__init__(self, torch_model=torch_model)
-
-        self.true_backprojection_set_color = "k"
-        self.estimated_backprojection_set_color = "tab:blue"
-        self.estimated_one_step_backprojection_set_color = "tab:orange"
-        self.estimated_backprojection_partitioned_set_color = "tab:gray"
-        self.backreachable_set_color = "tab:cyan"
-        self.target_set_color = "tab:red"
-        self.initial_set_color = "k"
-
-        self.true_backprojection_set_zorder = 3
-        self.estimated_backprojection_set_zorder = 2
-        self.estimated_one_step_backprojection_set_zorder = -1
-        self.estimated_backprojection_partitioned_set_zorder = 5
-        self.backreachable_set_zorder = -1
-        self.target_set_zorder = 1
-        self.initial_set_zorder = 1
-
-        self.true_backprojection_set_linestyle = "-"
-        self.estimated_backprojection_set_linestyle = "-"
-        self.estimated_one_step_backprojection_set_linestyle = "-"
-        self.estimated_backprojection_partitioned_set_linestyle = "-"
-        self.backreachable_set_linestyle = "--"
-        self.target_set_linestyle = "-"
-
-        # self.reachable_set_color = 'tab:green'
-        # self.reachable_set_zorder = 4
-        # self.initial_set_color = 'tab:gray'
-        # self.initial_set_zorder = 1
-
-    @property
-    def partitioner_dict(self):
-        return partitioners.partitioner_dict
-
-    @property
-    def propagator_dict(self):
-        return propagators.propagator_dict
-
-    def instantiate_partitioner(
-        self, partitioner: str, hyperparams: dict[str, Any]
-    ) -> partitioners.ClosedLoopPartitioner:
-        return partitioners.partitioner_dict[partitioner](
-            **{**hyperparams, "dynamics": self.dynamics}
-        )
 
-    def instantiate_propagator(
-        self, propagator: str, hyperparams: dict[str, Any]
-    ) -> propagators.ClosedLoopPropagator:
-        return propagators.propagator_dict[propagator](
-            **{**hyperparams, "dynamics": self.dynamics}
-        )
-
-    def get_one_step_backprojection_set(
+    def get_one_step_reachable_set(
         self,
-        target_set: constraints.SingleTimestepConstraint,
-        overapprox: bool = False,
-    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
-        backprojection_set, info = (
-            self.partitioner.get_one_step_backprojection_set(
-                target_set, self.propagator, overapprox=overapprox
-            )
+        initial_set: constraints.SingleTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
+    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
+        reachable_set, info = propagator.get_one_step_reachable_set(
+            initial_set
         )
-        return backprojection_set, info
+        return reachable_set, info
 
-    def get_backprojection_set(
+    def get_reachable_set(
         self,
-        target_set: constraints.SingleTimestepConstraint,
+        initial_set: constraints.SingleTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
         t_max: int,
-        overapprox: bool = False,
     ) -> tuple[constraints.MultiTimestepConstraint, dict]:
-        backprojection_set, info = self.partitioner.get_backprojection_set(
-            target_set, self.propagator, t_max, overapprox=overapprox
-        )
-        return backprojection_set, info
+        reachable_set, info = propagator.get_reachable_set(initial_set, t_max)
+        return reachable_set, info
 
-    def get_N_step_backprojection_set(
-        self,
-        target_set: constraints.SingleTimestepConstraint,
-        t_max: int,
-        num_partitions=None,
-        overapprox: bool = False,
-    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
-        backprojection_set, info = (
-            self.partitioner.get_N_step_backprojection_set(
-                target_set,
-                self.propagator,
-                t_max,
-                num_partitions=num_partitions,
-                overapprox=overapprox,
-            )
-        )
-        return backprojection_set, info
+        # # TODO: this is repeated from UniformPartitioner...
+        # # might be more efficient to directly return from propagator?
+        # _ = reachable_set.add_cell(reachable_set_this_cell)
 
-    def get_backprojection_error(
+        # return reachable_set, info
+
+    def get_error(  # type: ignore
         self,
-        target_set: constraints.SingleTimestepConstraint,
-        backprojection_sets: constraints.MultiTimestepConstraint,
+        initial_set: constraints.SingleTimestepConstraint,
+        reachable_sets: constraints.MultiTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
         t_max: int,
     ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
-        return self.partitioner.get_backprojection_error(
-            target_set,
-            backprojection_sets,
-            self.propagator,
-            t_max,
-            backreachable_sets=None,
-        )
+        errors = []
 
-    def visualize(  # type: ignore
-        self,
-        backprojection_sets: constraints.MultiTimestepConstraint,
-        target_set: constraints.SingleTimestepConstraint,
-        info: dict,
-        initial_constraint: Optional[
-            constraints.SingleTimestepConstraint
-        ] = None,
-        show: bool = True,
-        show_samples: bool = False,
-        show_samples_from_cells: bool = False,
-        show_trajectories: bool = False,
-        show_convex_hulls: bool = False,
-        aspect: str = "auto",
-        axis_labels: list = [],
-        axis_dims: list = [],
-        plot_lims: Optional[str] = None,
-        controller_name: Optional[str] = None,
-        show_BReach: bool = False,
-    ) -> None:
-        # sampled_outputs = self.get_sampled_outputs(input_range)
-        # output_range_exact = self.samples_to_range(sampled_outputs)
+        if isinstance(initial_set, constraints.LpConstraint):
+            estimated_reachable_set_ranges = reachable_sets.range
+            true_reachable_set_ranges = self.get_sampled_out_range(
+                initial_set, propagator, t_max, num_samples=1000
+            )
+            num_steps = true_reachable_set_ranges.shape[0]
+            for t in range(num_steps):
+                true_area = np.product(
+                    true_reachable_set_ranges[t][..., 1]
+                    - true_reachable_set_ranges[t][..., 0]
+                )
+                estimated_area = np.product(
+                    estimated_reachable_set_ranges[t][..., 1]
+                    - estimated_reachable_set_ranges[t][..., 0]
+                )
+                errors.append((estimated_area - true_area) / true_area)
+        elif isinstance(initial_set, constraints.PolytopeConstraint):
+            # Note: This compares the estimated polytope
+            # with the "best" polytope with those facets.
+            # There could be a much better polytope with lots of facets.
+            true_verts = self.get_sampled_out_range(
+                initial_set,
+                propagator,
+                t_max,
+                num_samples=1000,
+                output_constraint=reachable_sets,
+            )
 
-        self.partitioner.setup_visualization(
-            backprojection_sets.get_constraint_at_time_index(-1),
-            backprojection_sets.get_t_max(),
-            self.propagator,
-            show_samples=show_samples,
-            show_samples_from_cells=show_samples_from_cells,
-            axis_dims=axis_dims,
-            axis_labels=axis_labels,
-            aspect=aspect,
-            initial_set_color=self.estimated_backprojection_set_color,
-            initial_set_zorder=self.estimated_backprojection_set_zorder,
-            extra_constraint=initial_constraint,
-            extra_set_color=self.initial_set_color,
-            extra_set_zorder=self.initial_set_zorder,
-            controller_name=controller_name,
-        )
+            num_steps = reachable_sets.get_t_max()
+            from scipy.spatial import ConvexHull
 
-        self.visualize_single_set(
-            backprojection_sets,
-            target_set,
-            initial_constraint=initial_constraint,
-            show_samples=show_samples,
-            show_trajectories=show_trajectories,
-            show_convex_hulls=show_convex_hulls,
-            show=show,
-            aspect=aspect,
-            plot_lims=plot_lims,
-            axis_dims=axis_dims,
-            show_BReach=show_BReach,
-            **info
-        )
-        self.partitioner.animate_fig.tight_layout()
+            for t in range(num_steps):
+                true_hull = ConvexHull(true_verts[:, t + 1, :])
+                true_area = true_hull.volume
+                A, b = reachable_sets.get_constraint_at_time_index(
+                    t
+                ).get_polytope()
+                estimated_verts = pypoman.polygon.compute_polygon_hull(A, b)
+                estimated_hull = ConvexHull(estimated_verts)
+                estimated_area = estimated_hull.volume
+                errors.append((estimated_area - true_area) / true_area)
+        else:
+            raise ValueError(
+                "initial_set and reachable_sets need to both be Lp or both be"
+                " Polytope."
+            )
+        final_error = errors[-1]
+        avg_error = np.mean(errors)
+        return final_error, avg_error, np.array(errors)
+
+    def get_sampled_out_range(
+        self,
+        initial_set: constraints.SingleTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
+        t_max: int = 5,
+        num_samples: int = 1000,
+        output_constraint: Optional[constraints.Constraint] = None,
+    ) -> np.ndarray:
+        # TODO: change output_constraint to better name
+        return self.dynamics.get_sampled_output_range(
+            initial_set,
+            t_max,
+            num_samples,
+            controller=propagator.network,
+            output_constraint=output_constraint,
+        )
+
+    def get_sampled_out_range_guidance(
+        self,
+        initial_set: constraints.SingleTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
+        t_max: int = 5,
+        num_samples: int = 1000,
+    ) -> np.ndarray:
+        # Duplicate of get_sampled_out_range, but called during partitioning
+        return self.get_sampled_out_range(
+            initial_set, propagator, t_max=t_max, num_samples=num_samples
+        )
+
+    def get_one_step_backreachable_set(
+        self,
+        target_sets: Union[
+            constraints.SingleTimestepConstraint,
+            constraints.MultiTimestepConstraint,
+        ],
+    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
+        # Given a target_set, compute the backreachable_set
+        # that ensures that starting from within the backreachable_set
+        # will lead to a state within the target_set
+        info = {}  # type: dict[str, Any]
+        # if collected_input_constraints is None:
+        #     collected_input_constraints = [input_constraint]
+
+        # Extract elementwise bounds on xt1 from the lp-ball or polytope
+        # constraint
+        A_target, b_target = target_sets.get_constraint_at_time_index(
+            -1
+        ).get_polytope()
+
+        """
+        Step 1:
+        Find backreachable set: all the xt for which there is
+        some u in U that leads to a state xt1 in output_constraint
+        """
+
+        if self.dynamics.u_limits is None:
+            print(
+                "self.dynamics.u_limits is None ==>                 The"
+                " backreachable set is probably the whole state space.        "
+                "         Giving up."
+            )
+            raise NotImplementedError
+        else:
+            u_min = self.dynamics.u_limits[:, 0]
+            u_max = self.dynamics.u_limits[:, 1]
 
-        if plot_lims is not None:
-            plot_lims_arr = np.array(ast.literal_eval(plot_lims))
-            plt.xlim(plot_lims_arr[0])
-            plt.ylim(plot_lims_arr[1])
+        num_states = self.dynamics.num_states
+        num_control_inputs = self.dynamics.num_inputs
 
-        if info.get("save_name", None) is not None:
-            plt.savefig(info["save_name"])
+        xt = cp.Variable(num_states)
+        ut = cp.Variable(num_control_inputs)
 
-        plt.gca().autoscale()
+        # For each dimension of the output constraint (facet/lp-dimension):
+        # compute a bound of the NN output using the pre-computed matrices
+        constrs = []
+        constrs += [u_min <= ut]
+        constrs += [ut <= u_max]
+
+        # Included state limits to reduce size of backreachable sets by
+        # eliminating states that are not physically possible
+        # (e.g., maximum velocities)
+        # if self.dynamics.x_limits is not None:
+        #     x_llim = self.dynamics.x_limits[:, 0]
+        #     x_ulim = self.dynamics.x_limits[:, 1]
+        #     constrs += [x_llim <= xt]
+        #     constrs += [xt <= x_ulim]
+        #     # Also constrain the future state to be within the state limits
+        #     constrs += [self.dynamics.dynamics_step(xt,ut) <= x_ulim]
+        #     constrs += [self.dynamics.dynamics_step(xt,ut) >= x_llim]
+
+        # if self.dynamics.x_limits is not None:
+        #     for state in self.dynamics.x_limits:
+        #         constrs += [self.dynamics.x_limits[state][0] <= xt[state]]
+        #         constrs += [xt[state] <= self.dynamics.x_limits[state][1]]
+
+        constrs += [A_target @ self.dynamics.dynamics_step(xt, ut) <= b_target]
+
+        b, status = optimize_over_all_states(xt, constrs)
+        ranges = np.vstack([-b[num_states:], b[:num_states]]).T
+
+        backreachable_set = constraints.LpConstraint(range=ranges)
+        info["backreachable_set"] = backreachable_set
+        info["target_sets"] = target_sets
 
-        if show:
-            plt.show()
-        else:
-            plt.close()
+        return backreachable_set, info
 
-    def visualize_single_set(
+    def get_one_step_backprojection_set(
         self,
-        backprojection_sets: constraints.MultiTimestepConstraint,
-        target_set: constraints.SingleTimestepConstraint,
-        initial_constraint: Optional[
-            constraints.SingleTimestepConstraint
-        ] = None,
-        show: bool = True,
-        show_samples: bool = False,
-        show_trajectories: bool = False,
-        show_convex_hulls: bool = False,
-        aspect: str = "auto",
-        axis_labels: list = [],
-        plot_lims: Optional[str] = None,
-        inputs_to_highlight: Optional[list[dict]] = None,
-        show_BReach: bool = False,
-        **kwargs
-    ) -> None:
-        rects = backprojection_sets.plot(
-            self.partitioner.animate_axes,
-            self.partitioner.axis_dims,
-            self.estimated_backprojection_set_color,
-            zorder=self.estimated_backprojection_set_zorder,
-            linewidth=self.partitioner.linewidth,
-            plot_2d=self.partitioner.plot_2d,
+        target_sets: constraints.MultiTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
+        overapprox: bool = False,
+    ) -> tuple[Optional[constraints.SingleTimestepConstraint], dict]:
+        backreachable_set, info = self.get_one_step_backreachable_set(
+            target_sets
         )
-        self.partitioner.default_patches += rects
-        for cell in backprojection_sets.cells:
-            rects = cell.plot(
-                self.partitioner.animate_axes,
-                self.partitioner.axis_dims,
-                self.estimated_backprojection_set_color,
-                zorder=self.estimated_backprojection_set_zorder,
-                linewidth=self.partitioner.linewidth,
-                plot_2d=self.partitioner.plot_2d,
-            )
-            self.partitioner.default_patches += rects
+        info["backreachable_set"] = backreachable_set
 
-        # Show the target set
-        self.plot_target_set(
-            target_set,
-            color=self.target_set_color,
-            zorder=self.target_set_zorder,
-            linestyle=self.target_set_linestyle,
+        backprojection_set, _ = propagator.get_one_step_backprojection_set(
+            backreachable_set,
+            target_sets,
+            overapprox=overapprox,
         )
 
-        # Show the "true" N-Step backprojection set as a convex hull
-        backreachable_set = kwargs["per_timestep"][-1]["backreachable_set"]
-        t_max = backprojection_sets.get_t_max()
-        if show_convex_hulls:
-            self.plot_true_backprojection_sets(
-                backreachable_set,
-                target_set,
-                t_max=t_max,
-                color=self.true_backprojection_set_color,
-                zorder=self.true_backprojection_set_zorder,
-                linestyle=self.true_backprojection_set_linestyle,
-                show_samples=False,
-            )
+        # if overapprox:
+        #     # These will be used to further backproject this set in time
+        #     backprojection_set.crown_matrices = get_crown_matrices(
+        #         propagator,
+        #         backprojection_set,
+        #         self.dynamics.num_inputs,
+        #         self.dynamics.sensor_noise
+        #     )
 
-        # Sketchy workaround to trajectories not showing up
-        if show_trajectories and initial_constraint is not None:
-            self.dynamics.show_trajectories(
-                t_max * self.dynamics.dt,
-                initial_constraint,
-                ax=self.partitioner.animate_axes,
-                controller=self.propagator.network,
-            )
+        return backprojection_set, info
 
-    def get_sampled_outputs(self, input_range, N=1000):
-        return get_sampled_outputs(input_range, self.propagator, N=N)
+    """
+    Inputs:
+    - target_set: describes goal/avoid set at t=t_max
+    - propagator:
+    - t_max: how many timesteps to backproject
+    - num_partitions: number of splits per dimension in each backreachable set
+    - overapprox: bool
+        True = compute outer bounds of BP sets (for collision avoidance)
+        False = computer inner bounds of BP sets (for goal arrival)
+
+    Returns:
+    - backprojection_sets: [BP_{-1}, ..., BP_{-t_max}]
+          i.e., [ set of states that will get to goal/avoid set in 1 step,
+                  ...,
+                  set of states that will get to goal/avoid set in t_max steps
+                ]
+    - info: TODO
+    """
 
-    def get_sampled_output_range(
-        self, input_constraint, t_max=5, num_samples=1000
-    ):
-        return self.partitioner.get_sampled_out_range(
-            input_constraint, self.propagator, t_max, num_samples
+    def get_backprojection_set(
+        self,
+        target_set: constraints.SingleTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
+        t_max: int,
+        overapprox: bool = False,
+    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
+        # Initialize data structures to hold results
+        backprojection_sets = (
+            constraints.create_empty_multi_timestep_constraint(
+                propagator.boundary_type
+            )
         )
-
-    def get_output_range(self, input_constraint, output_constraint):
-        return self.partitioner.get_output_range(
-            input_constraint, output_constraint
+        info = {"per_timestep": []}  # type: dict[str, Any]
+
+        # Run one step of backprojection analysis
+        backprojection_set_this_timestep, info_this_timestep = (
+            self.get_one_step_backprojection_set(
+                target_set.to_multistep_constraint(),
+                propagator,
+                overapprox=overapprox,
+            )
         )
 
-    def samples_to_range(self, sampled_outputs):
-        return samples_to_range(sampled_outputs)
-
-    def get_exact_output_range(self, input_range):
-        sampled_outputs = self.get_sampled_outputs(input_range)
-        output_range = self.samples_to_range(sampled_outputs)
-        return output_range
-
-    def get_error(self, input_constraint, output_constraint, t_max):
-        return self.partitioner.get_error(
-            input_constraint, output_constraint, self.propagator, t_max
-        )
+        # Store that step's results
+        assert backprojection_set_this_timestep is not None
+        backprojection_sets = backprojection_sets.add_timestep_constraint(
+            backprojection_set_this_timestep
+        )
+        info["per_timestep"].append(info_this_timestep)
+
+        if overapprox:
+            for i in np.arange(
+                0 + propagator.dynamics.dt + 1e-10,
+                t_max,
+                propagator.dynamics.dt,
+            ):
+                # Run one step of backprojection analysis
+                backprojection_set_this_timestep, info_this_timestep = (
+                    self.get_one_step_backprojection_set(
+                        target_set.add_timestep_constraint(
+                            backprojection_sets
+                        ),
+                        propagator,
+                        overapprox=overapprox,
+                    )
+                )
+                assert backprojection_set_this_timestep is not None
+                backprojection_sets = (
+                    backprojection_sets.add_timestep_constraint(
+                        backprojection_set_this_timestep
+                    )
+                )
+                info["per_timestep"].append(info_this_timestep)
+        else:
+            for i in np.arange(
+                0 + propagator.dynamics.dt + 1e-10,
+                t_max,
+                propagator.dynamics.dt,
+            ):
+                # TODO: Support N-step backprojection in the
+                # under-approximation case
+                raise NotImplementedError
 
-    def plot_backreachable_set(
-        self,
-        backreachable_set: constraints.SingleTimestepConstraint,
-        color: str = "cyan",
-        zorder: Optional[int] = None,
-        linestyle: str = "-",
-    ) -> None:
-        self.partitioner.plot_reachable_sets(
-            backreachable_set,
-            self.partitioner.axis_dims,
-            reachable_set_color=color,
-            reachable_set_zorder=zorder,
-            reachable_set_ls=linestyle,
-        )
+        return backprojection_sets, info
 
-    def plot_target_set(
+    def get_backprojection_error(
         self,
         target_set: constraints.SingleTimestepConstraint,
-        color: str = "cyan",
-        zorder: Optional[int] = None,
-        linestyle: str = "-",
-        linewidth: float = 2.5,
-    ) -> None:
-        self.partitioner.plot_reachable_sets(
-            target_set,
-            self.partitioner.axis_dims,
-            reachable_set_color=color,
-            reachable_set_zorder=zorder,
-            reachable_set_ls=linestyle,
-            reachable_set_lw=linewidth,
-        )
+        backprojection_sets: constraints.MultiTimestepConstraint,
+        propagator: propagators.ClosedLoopPropagator,
+        t_max: int,
+    ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+        # Note: This almost certainly got messed up in the merge (3/24/23)
 
-    def plot_tightened_backprojection_set(
-        self,
-        tightened_set: constraints.SingleTimestepConstraint,
-        color: str = "darkred",
-        zorder: Optional[int] = None,
-        linestyle: str = "-",
-    ) -> None:
-        self.partitioner.plot_reachable_sets(
-            tightened_set,
-            self.partitioner.axis_dims,
-            reachable_set_color=color,
-            reachable_set_zorder=zorder,
-            reachable_set_ls=linestyle,
-        )
+        errors = []
 
-    def plot_backprojection_set(
-        self,
-        backreachable_set: constraints.SingleTimestepConstraint,
-        target_set: constraints.SingleTimestepConstraint,
-        show_samples: bool = False,
-        color: str = "g",
-        zorder: Optional[int] = None,
-        linestyle: str = "-",
-    ) -> None:
-        # Sample a bunch of pts from our "true" backreachable set
-        # (it's actually the tightest axis-aligned rectangle around the
-        # set) and run them forward 1 step in time under the NN policy
-        xt_samples_from_backreachable_set, xt1_from_those_samples = (
-            self.partitioner.dynamics.get_state_and_next_state_samples(
-                backreachable_set,
-                num_samples=1e5,
-                controller=self.propagator.network,
-            )
+        true_verts_reversed = self.dynamics.get_true_backprojection_set(
+            backprojection_sets.get_constraint_at_time_index(-1),
+            target_set,
+            t_max,
+            controller=propagator.network,
         )
+        true_verts = np.flip(true_verts_reversed, axis=1)
+        num_steps = backprojection_sets.get_t_max()
 
-        # Find which of the xt+1 points actually end up in the target set
-        target_set_A, target_set_b = target_set.get_polytope()
-        within_constraint_inds = np.where(
-            np.all(
-                (
-                    np.dot(target_set_A, xt1_from_those_samples.T)
-                    - np.expand_dims(target_set_b, axis=-1)
-                )
-                <= 0,
-                axis=0,
+        for t in range(num_steps):
+            x_min = np.min(true_verts[:, t + 1, :], axis=0)
+            x_max = np.max(true_verts[:, t + 1, :], axis=0)
+
+        if isinstance(target_set, constraints.LpConstraint):
+            Ats, bts = range_to_polytope(target_set.range)
+            true_verts_reversed = self.dynamics.get_true_backprojection_set(
+                backprojection_sets.get_constraint_at_time_index(-1),
+                target_set,
+                t_max,
+                controller=propagator.network,
+                num_samples=1e8,
             )
-        )
-        xt_samples_inside_backprojection_set = (
-            xt_samples_from_backreachable_set[(within_constraint_inds)]
-        )
+            true_verts = np.flip(true_verts_reversed, axis=1)
+            num_steps = backprojection_sets.get_t_max()
+
+            x_range = x_max - x_min
+            true_area = np.prod(x_range)
 
-        if show_samples:
-            xt1_from_those_samples_ = xt1_from_those_samples[
-                (within_constraint_inds)
-            ]
-
-            # Show samples from inside the backprojection set and their
-            # futures under the NN (should end in target set)
-            self.partitioner.dynamics.show_samples(
-                None,
-                None,
-                ax=self.partitioner.animate_axes,
-                controller=None,
-                input_dims=self.partitioner.axis_dims,
-                zorder=1,
-                xs=np.dstack(
-                    [
-                        xt_samples_inside_backprojection_set,
-                        xt1_from_those_samples_,
-                    ]
-                ).transpose(0, 2, 1),
-                colors=None,
+            estimated_area = backprojection_sets.get_constraint_at_time_index(
+                t
+            ).get_area()
+
+            # true_hull = ConvexHull(true_verts[:, t+1, :])
+            # true_area = true_hull.volume
+
+            Abp, bbp = backprojection_sets.get_constraint_at_time_index(
+                t
+            ).get_polytope()
+            estimated_verts = pypoman.polygon.compute_polygon_hull(Abp, bbp)
+            estimated_hull = ConvexHull(estimated_verts)
+            estimated_area = estimated_hull.volume
+
+            # print(f"estimated: estimated_area --- true: {true_area}")
+            # print(
+            #     "estimated range: {} --- true range: {}".format(
+            #         backprojection_sets[t].range, x_range
+            #     )
+            # )
+
+            errors.append((estimated_area - true_area) / true_area)
+        elif isinstance(target_set, constraints.RotatedLpConstraint):
+            true_verts_reversed = self.dynamics.get_true_backprojection_set(
+                # backreachable_sets[-1],
+                target_set,
+                t_max,
+                controller=propagator.network,
+                num_samples=1e8,
             )
+            true_verts = np.flip(true_verts_reversed, axis=1)
+            num_steps = len(backprojection_sets)
 
-        # Compute and draw a convex hull around all the backprojection set
-        # samples. This is our "true" backprojection set -- but...
-        # it is sampling-based so that is an under-approximation,
-        # and it is a convex hull, so that is an over-approximation,
-        # and it is computed only for one step, so that's an over-approximation
-        _ = plot_convex_hull(
-            xt_samples_inside_backprojection_set,
-            dims=self.partitioner.axis_dims,
-            color=color,
-            linewidth=2,
-            linestyle=linestyle,
-            zorder=zorder,
-            label="Backprojection Set (True)",
-            axes=self.partitioner.animate_axes,
-        )
-        # self.default_lines[self.output_axis].append(conv_hull_line[0])
+            for t in range(num_steps):
+                # x_min = np.min(true_verts[:,t+1,:], axis=0)
+                # x_max = np.max(true_verts[:,t+1,:], axis=0)
+
+                # x_range = x_max-x_min
+                # true_area = np.prod(x_range)
+                true_hull = ConvexHull(true_verts[:, t + 1, :])
+                true_area = true_hull.volume
+
+                # true_hull = ConvexHull(true_verts[:, t+1, :])
+                # true_area = true_hull.volume
+
+                # Abp, bbp = range_to_polytope(backprojection_sets[t].range)
+                # estimated_verts = (
+                #   pypoman.polygon.compute_polygon_hull(Abp, bbp)
+                # )
+                estimated_hull = ConvexHull(backprojection_sets[t].vertices)
+                estimated_area = estimated_hull.volume
+
+                # print(
+                #     "estimated: {} --- true: {}".format(
+                #         estimated_area, true_area
+                #     )
+                # )
+                # print(
+                #     "estimated range: {} --- true range: {}".format(
+                #         backprojection_sets[t].range, x_range
+                #     )
+                # )
 
-    def plot_true_backprojection_sets(
-        self,
-        backreachable_set: constraints.SingleTimestepConstraint,
-        target_set: constraints.SingleTimestepConstraint,
-        t_max: int,
-        show_samples: bool = False,
-        color: str = "g",
-        zorder: Optional[int] = None,
-        linestyle: str = "-",
-    ) -> None:
-        # Sample a bunch of pts from our "true" backreachable set
-        # (it's actually the tightest axis-aligned rectangle around the
-        # backreachable set) and run them forward t_max steps in time under
-        # the NN policy
-        x_samples_inside_backprojection_set = (
-            self.dynamics.get_true_backprojection_set(
-                backreachable_set,
+                errors.append((estimated_area - true_area) / true_area)
+        else:
+            # This implementation should actually be moved to Lp constraint
+
+            # Note: This compares the estimated polytope
+            # with the "best" polytope with those facets.
+            # There could be a much better polytope with lots of facets.
+            true_verts_reversed = self.dynamics.get_true_backprojection_set(
+                backprojection_sets.get_constraint_at_time_index(-1),
                 target_set,
-                t_max=t_max,
-                controller=self.propagator.network,
+                t_max,
+                controller=propagator.network,
             )
-        )
+            true_verts = np.flip(true_verts_reversed, axis=1)
+            num_steps = backprojection_sets.get_t_max()
 
-        if show_samples:
-            # xt1_from_those_samples_ = xt1_from_those_samples[
-            #     (within_constraint_inds)
-            # ]
-
-            # Show samples from inside the backprojection set and their
-            # futures under the NN (should end in target set)
-            self.partitioner.dynamics.show_samples(
-                None,
-                None,
-                ax=self.partitioner.animate_axes,
-                controller=None,
-                input_dims=self.partitioner.axis_dims,
-                zorder=1,
-                xs=x_samples_inside_backprojection_set,
-                colors=None,
-            )
-            print(self.partitioner.animate_axes.get_ylabel())
+            for t in range(num_steps):
+                x_min = np.min(true_verts[:, t + 1, :], axis=0)
+                x_max = np.max(true_verts[:, t + 1, :], axis=0)
+
+                x_range = x_max - x_min
+                true_area = np.prod(x_range)
+
+                Abp, bbp = backprojection_sets.get_constraint_at_time_index(
+                    t
+                ).get_polytope()
+                estimated_verts = pypoman.polygon.compute_polygon_hull(
+                    Abp, bbp
+                )
+                estimated_hull = ConvexHull(estimated_verts)
+                estimated_area = estimated_hull.volume
 
-        # Compute and draw a convex hull around all the backprojection set
-        # samples. This is our "true" backprojection set -- but...
-        # it is sampling-based so that is an under-approximation,
-        # and it is a convex hull, so that is an over-approximation.
-        for t in range(t_max):
-            _ = plot_convex_hull(
-                x_samples_inside_backprojection_set[:, t, :],
-                dims=self.partitioner.axis_dims,
-                color=color,
-                linewidth=2,
-                linestyle=linestyle,
-                zorder=zorder,
-                label="Backprojection Set (True)",
-                axes=self.partitioner.animate_axes,
-            )
-        # self.default_lines[self.output_axis].append(conv_hull_line[0])
+                errors.append((estimated_area - true_area) / true_area)
+
+        final_error = errors[-1]
+        avg_error = np.mean(errors)
+        return final_error, avg_error, np.array(errors)
 
-    def plot_relaxed_sequence(
-        self, start_region, bp_sets, crown_bounds, target_set, marker="o"
+    def get_N_step_backprojection_set(
+        self,
+        output_constraint,
+        input_constraint,
+        propagator,
+        t_max,
+        num_partitions=None,
+        overapprox=False,
+        heuristic="guided",
+        all_lps=False,
+        slow_cvxpy=False,
     ):
-        bp_sets = deepcopy(bp_sets)
-        bp_sets.reverse()
-        bp_sets.append(target_set)
-        sequences = (
-            self.partitioner.dynamics.get_relaxed_backprojection_samples(
-                start_region, bp_sets, crown_bounds, target_set
-            )
+        input_constraint_, info = propagator.get_N_step_backprojection_set(
+            output_constraint,
+            deepcopy(input_constraint),
+            t_max,
+            num_partitions=num_partitions,
+            overapprox=overapprox,
+            heuristic=heuristic,
+            all_lps=all_lps,
+            slow_cvxpy=slow_cvxpy,
         )
+        input_constraint = input_constraint_.copy()
 
-        ax = (self.partitioner.animate_axes,)
-        x = []
-        y = []
-        for seq in [sequences[0]]:
-            for point in seq:
-                x.append(point[0])
-                y.append(point[1])
-
-        # import pdb; pdb.set_trace()
-        ax[0].scatter(x, y, s=40, zorder=15, c="k", marker=marker)
-
-
-def plot_convex_hull(
-    samples: np.ndarray,
-    dims: list,
-    color: str,
-    linewidth: float,
-    linestyle: str,
-    zorder: Optional[int],
-    label: str,
-    axes: matplotlib.axes,
-) -> matplotlib.lines.Line2D:
-    hull = ConvexHull(samples[..., dims].squeeze())
-    line = axes.plot(
-        np.append(
-            samples[hull.vertices][..., dims[0]],
-            samples[hull.vertices[0]][..., dims[0]],
-        ),
-        np.append(
-            samples[hull.vertices][..., dims[1]],
-            samples[hull.vertices[0]][..., dims[1]],
-        ),
-        color=color,
-        linewidth=linewidth,
-        linestyle=linestyle,
-        zorder=zorder,
-        label=label,
-    )
-    return line
+        return input_constraint, info
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/constraints/ClosedLoopConstraints.py` & `nfl_veripy-0.0.2/src/nfl_veripy/constraints/Constraints.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,365 +1,43 @@
 """Tools for representing sets during reachability analysis."""
 from __future__ import annotations
 
 import collections
-from abc import ABC
-from typing import Any, Optional, TypeGuard, Union
+from typing import Optional, Union
 
 import jax
+import jax_verify
 import numpy as np
 import pypoman
-from matplotlib.patches import Rectangle
-from nfl_veripy.utils.plot_rect_prism import rect_prism
-from nfl_veripy.utils.utils import (
-    CROWNMatrices,
-    get_polytope_A,
-    range_to_polytope,
-)
 from scipy.spatial import ConvexHull
 
-import jax_verify
-
-
-class Constraint(ABC):
-    """Abstract class describing a set of states."""
-
-    def to_reachable_input_objects(self):
-        """Get the objects needed for forward reachability."""
-
-    def to_fwd_reachable_output_objects(self, num_states):
-        """Get the objects needed for forward reachability."""
-
-    def get_t_max(self) -> int:
-        """Get the time duration this constraint represents"""
-
-    def add_cell(self, other: Optional[Constraint]) -> None:
-        """Expand this constraint's set to include a new set."""
-
-    def update_main_constraint_with_cells(self, overapprox: bool) -> None:
-        """Set bounds of full set based on combination of all cells."""
-
-    def add_cell_and_update_main_constraint(
-        self, other: Optional[LpConstraint]
-    ) -> None:
-        """Insert cell into set and also update bounds of full set."""
-
-    def to_linf(self) -> np.ndarray:
-        """Get hyperrectangle bounds around set."""
-
-    def get_area(self) -> float:
-        """Get area contained by set."""
-
-    def get_polytope(self) -> tuple[np.ndarray, np.ndarray]:
-        """Get polytope bounds around set."""
-
-    def get_constraint_at_time_index(self, i: int) -> PolytopeConstraint:
-        """Get set corresponding to a single timestep."""
-
-
-class PolytopeConstraint(Constraint):
-    """Represents single timestep's set of states with a H-rep polytope."""
-
-    def __init__(
-        self, A: Optional[np.ndarray] = None, b: Optional[np.ndarray] = None
-    ):
-        super().__init__()
-        self.A = A
-        self.b = b
-        self.cells: list[PolytopeConstraint] = []
-        self.crown_matrices: Optional[CROWNMatrices] = None
-        self.main_constraint_stale = False
-
-    def update_main_constraint_with_cells(self, overapprox: bool) -> None:
-        if len(self.cells) == 0:
-            raise ValueError("Can't update because self.cells is empty.")
-        elif len(self.cells) == 1:
-            self.A = self.cells[0].A
-            self.b = self.cells[0].b
-            self.main_constraint_stale = False
-        else:
-            if overapprox:
-                # TODO: compute all vertices, then get conv hull using pypoman
-                raise NotImplementedError
-            else:
-                # Simplest under-approximation of union of polytopes is one of
-                # those polytopes :/
-                # TODO: compute a better under-approximation :)
-                self.A = self.cells[0].A
-                self.b = self.cells[0].b
-                self.main_constraint_stale = False
-
-    def add_cell(self, other: Optional[PolytopeConstraint]) -> None:
-        if other is None:
-            return
-
-        self.cells.append(other)
-        self.main_constraint_stale = True
-
-    def get_cell(self, input_range: np.ndarray) -> PolytopeConstraint:
-        # This is a disaster hack to partition polytopes
-        A_rect, b_rect = range_to_polytope(input_range)
-        rectangle_verts = pypoman.polygon.compute_polygon_hull(A_rect, b_rect)
-        input_polytope_verts = pypoman.polygon.compute_polygon_hull(
-            self.A, self.b
-        )
-        partition_verts = pypoman.intersection.intersect_polygons(
-            input_polytope_verts, rectangle_verts
-        )
-        (
-            A_inputs_,
-            b_inputs_,
-        ) = pypoman.duality.compute_polytope_halfspaces(partition_verts)
-        constraint = self.__class__(A_inputs_, b_inputs_)
-        return constraint
-
-    def to_range(self) -> np.ndarray:
-        if self.A is None or self.b is None:
-            raise ValueError(
-                "Can't convert PolytopeConstraint to range, since self.A or"
-                " self.b are None."
-            )
-
-        # only used to compute slope in non-closedloop manner...
-        input_polytope_verts = pypoman.duality.compute_polytope_vertices(
-            self.A, self.b
-        )
-        input_range = np.empty((self.A.shape[1], 2))
-        input_range[:, 0] = np.min(np.stack(input_polytope_verts), axis=0)
-        input_range[:, 1] = np.max(np.stack(input_polytope_verts), axis=0)
-        return input_range
-
-    def set_bound(self, i: int, max_value: float, min_value: float) -> None:
-        if self.b is None:
-            raise ValueError(
-                "Can't set bound on PolytopeConstraint, since self.b is None."
-            )
-        self.b[i] = max_value
-
-    def to_reachable_input_objects(
-        self,
-    ) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, float]:
-        if self.A is None or self.b is None:
-            raise ValueError(
-                "Can't convert PolytopeConstraint to"
-                " to_reachable_input_objects, since self.A or self.b are None."
-            )
-
-        A_inputs = self.A
-        b_inputs = self.b
-
-        # Get bounds on each state from A_inputs, b_inputs
-        try:
-            vertices_list = pypoman.compute_polytope_vertices(
-                A_inputs, b_inputs
-            )  # type: list[np.ndarray]
-        except Exception:
-            # Sometimes get arithmetic error... this may fix it
-            vertices_list = pypoman.compute_polytope_vertices(
-                A_inputs, b_inputs + 1e-6
-            )
-        vertices = np.stack(vertices_list)
-        x_max = np.max(vertices, 0)  # type: np.ndarray
-        x_min = np.min(vertices, 0)  # type: np.ndarray
-        norm = np.inf
-        return A_inputs, b_inputs, x_max, x_min, norm
-
-    def to_fwd_reachable_output_objects(
-        self, num_states: int
-    ) -> tuple[np.ndarray, int]:
-        if self.A is None:
-            raise ValueError(
-                "Can't convert PolytopeConstraint to"
-                " to_fwd_reachable_output_objects, since self.A is None."
-            )
-        A_out = self.A
-        num_facets = A_out.shape[0]
-        self.b = np.zeros((num_facets))
-        return A_out, num_facets
-
-    def to_linf(self) -> np.ndarray:
-        if isinstance(self.A, list):
-            # Mainly for backreachability, return a list of ranges if
-            # the constraint contains a list of polytopes
-            ranges = []
-            for A, b in zip(self.A, self.b):
-                vertices = np.stack(
-                    pypoman.duality.compute_polytope_vertices(A, b)
-                )
-                ranges.append(
-                    np.dstack(
-                        [np.min(vertices, axis=0), np.max(vertices, axis=0)]
-                    )[0]
-                )
-        else:
-            vertices = np.stack(
-                pypoman.duality.compute_polytope_vertices(self.A, self.b)
-            )
-            ranges = np.dstack(
-                [np.min(vertices, axis=0), np.max(vertices, axis=0)]
-            )[0]
-        return ranges
-
-    def plot(
-        self,
-        ax,
-        dims,
-        color,
-        fc_color="None",
-        linewidth=1.5,
-        label=None,
-        zorder=2,
-        plot_2d=True,
-        ls="-",
-    ):
-        if not plot_2d:
-            raise NotImplementedError
-
-        # TODO: this doesn't use the computed input_dims...
-
-        if linewidth != 2.5:
-            linewidth = 1.5
-
-        lines = []
-
-        if isinstance(self.A, list):
-            # Backward reachability
-            # input_constraint.A will be a list
-            # of polytope facets, whose union is the estimated
-            # backprojection set
-
-            for A, b in zip(self.A, self.b):
-                line = make_polytope_from_arrs(
-                    ax,
-                    A,
-                    b,
-                    color,
-                    label,
-                    zorder,
-                    ls,
-                    linewidth,
-                )
-                lines += line
-
-        else:
-            # Forward reachability
-            if isinstance(self.b, np.ndarray) and self.b.ndim == 1:
-                line = make_polytope_from_arrs(
-                    ax, self.A, self.b, color, label, zorder, ls, linewidth
-                )
-                lines += line
-            else:
-                for A, b in zip(self.A, self.b):
-                    line = make_polytope_from_arrs(
-                        ax,
-                        A,
-                        b,
-                        color,
-                        label,
-                        zorder,
-                        ls,
-                        linewidth,
-                    )
-                    lines += line
-
-        return lines
-
-    # other should really be
-    # Union[PolytopeConstraint, MultiTimestepPolytopeConstraint]
-    def add_timestep_constraint(
-        self,
-        other: Union[
-            SingleTimestepConstraint, MultiTimestepPolytopeConstraint
-        ],
-    ) -> MultiTimestepPolytopeConstraint:
-        if not isinstance(
-            other, (PolytopeConstraint, MultiTimestepPolytopeConstraint)
-        ):
-            raise TypeError(
-                "in add_timestep_constraint, other should be"
-                " Union[PolytopeConstraint, MultiTimestepPolytopeConstraint]."
-            )
-        if self.A is None or self.b is None:
-            raise ValueError(
-                "Trying to add_timestep_constraint but self.A or self.b are"
-                " None."
-            )
-        if other.A is None or other.b is None:
-            raise ValueError(
-                "Trying to add_timestep_constraint but other.A or other.b are"
-                " None."
-            )
-        return MultiTimestepPolytopeConstraint(
-            A=[self.A] + other.A, b=[self.b] + other.b
-        )
-
-    def to_multistep_constraint(self) -> MultiTimestepPolytopeConstraint:
-        if self.A is None or self.b is None:
-            raise ValueError(
-                "Trying to convert to multistep constraint but self.A or"
-                " self.b are None."
-            )
-        constraint = MultiTimestepPolytopeConstraint(A=[self.A], b=[self.b])
-        constraint.cells = [
-            cell.to_multistep_constraint() for cell in self.cells
-        ]
-        return constraint
-
-    def get_area(self) -> float:
-        estimated_verts = pypoman.polygon.compute_polygon_hull(self.A, self.b)
-        estimated_hull = ConvexHull(estimated_verts)
-        estimated_area = estimated_hull.volume
-        return estimated_area
-
-    def get_polytope(self) -> tuple[np.ndarray, np.ndarray]:
-        assert self.A is not None
-        assert self.b is not None
-        return self.A, self.b
-
-    def get_constraint_at_time_index(self, i: int) -> PolytopeConstraint:
-        return self
-
-    def to_jittable(self):
-        return JittablePolytopeConstraint(
-            self.A, self.b, {jax_verify.IntervalBound: None}, {}
-        )
-
-    @classmethod
-    def from_jittable(cls, jittable_constraint):
-        return cls(
-            range=np.array(
-                [jittable_constraint.lower, jittable_constraint.upper]
-            )
-        )
-
-    def _tree_flatten(self):
-        children = (self.A, self.b)  # arrays / dynamic values
-        aux_data = {}  # static values
-        return (children, aux_data)
-
-    @classmethod
-    def _tree_unflatten(cls, aux_data, children):
-        return cls(*children, **aux_data)
+from nfl_veripy.constraints.constraint_utils import (
+    make_polytope_from_arrs,
+    make_rect_from_arr,
+)
+from nfl_veripy.utils.plot_rect_prism import rect_prism
+from nfl_veripy.utils.utils import CROWNMatrices, range_to_polytope
 
 
-class LpConstraint(Constraint):
+class LpConstraint:
     """Represents single timestep's set of states with an lp-ball."""
 
     def __init__(
         self,
         range: Optional[np.ndarray] = None,
         p: float = np.inf,
         crown_matrices: Optional[CROWNMatrices] = None,
     ):
         super().__init__()
         self.range = range
         self.p = p
         self.crown_matrices = crown_matrices
         self.cells = []  # type: list[LpConstraint]
-        self.main_constraint_stale = False
+        self.main_constraint_stale: bool = False
+        self.is_infeasible: bool = False
 
     def set_bound(self, i: int, max_value: float, min_value: float) -> None:
         if self.range is None:
             raise ValueError(
                 "Can't set bound on LpConstraint, since self.range is None."
             )
         self.range[i, 0] = min_value
@@ -382,38 +60,48 @@
         self.main_constraint_stale = True
 
     def add_cell_and_update_main_constraint(
         self, other: Optional[LpConstraint]
     ) -> None:
         """Insert cell into set and also update bounds of full set."""
         assert self.main_constraint_stale is False
+        if other is None:
+            return
         self.add_cell(other)
+        if other.range is None:
+            # No need to update main constraint
+            self.main_constraint_stale = False
+            return
 
-        if len(self.cells) == 1:
+        if len(self.cells) == 1 or self.range is None:
             self.range = other.range
         else:
             self.range[:, 0] = np.minimum(self.range[:, 0], other.range[:, 0])
             self.range[:, 1] = np.maximum(self.range[:, 1], other.range[:, 1])
         self.main_constraint_stale = False
 
     def update_main_constraint_with_cells(self, overapprox: bool) -> None:
         if overapprox:
             # get min of all mins, get max of all maxes
             tmp = np.stack(
-                [c.range for c in self.cells],
+                [c.range for c in self.cells if c.range is not None],
                 axis=-1,
             )
             self.range = np.empty_like(self.cells[0].range)
             self.range[..., 0] = np.min(tmp[..., 0, :], axis=-1)
             self.range[..., 1] = np.max(tmp[..., 1, :], axis=-1)
         else:
             raise NotImplementedError
 
         self.main_constraint_stale = False
 
+    def get_vertices(self) -> np.ndarray:
+        Abp, bbp = range_to_polytope(self.range)
+        return np.stack(pypoman.polygon.compute_polygon_hull(Abp, bbp))
+
     def to_reachable_input_objects(
         self,
     ) -> tuple[
         Optional[np.ndarray],
         Optional[np.ndarray],
         np.ndarray,
         np.ndarray,
@@ -476,42 +164,27 @@
         plot_2d=True,
     ):
         rect = rect_prism(
             *self.range[dims, :], ax, color, linewidth, fc_color, zorder=zorder
         )
         return rect
 
-    # other should really be Union[LpConstraint, MultiTimestepLpConstraint]
     def add_timestep_constraint(
         self, other: Union[SingleTimestepConstraint, MultiTimestepConstraint]
-    ) -> MultiTimestepLpConstraint:
-        if not isinstance(other, (LpConstraint, MultiTimestepLpConstraint)):
-            raise TypeError(
-                "in add_timestep_constraint, other should be"
-                " Union[LpConstraint, MultiTimestepLpConstraint]."
-            )
-        if self.range is None:
-            raise ValueError(
-                "Trying to add_timestep_constraint but self.range is None."
-            )
-        if other.range is None:
-            raise ValueError(
-                "Trying to add_timestep_constraint but other.range is None."
-            )
-        return MultiTimestepLpConstraint(
-            range=np.vstack([np.expand_dims(self.range, 0), other.range])
-        )
+    ) -> MultiTimestepConstraint:
+        constraints = [self] + other.to_multistep_constraint().constraints
+        return MultiTimestepConstraint(constraints=constraints)
 
-    def to_multistep_constraint(self) -> MultiTimestepLpConstraint:
+    def to_multistep_constraint(self) -> MultiTimestepConstraint:
         if self.range is None:
             raise ValueError(
                 "Trying to convert to multistep constraint but self.range is"
                 " None."
             )
-        return MultiTimestepLpConstraint(range=np.expand_dims(self.range, 0))
+        return MultiTimestepConstraint(constraints=[self])
 
     def get_area(self) -> float:
         Abp, bbp = range_to_polytope(self.range)
         estimated_verts = pypoman.polygon.compute_polygon_hull(Abp, bbp)
         estimated_hull = ConvexHull(estimated_verts)
         estimated_area = estimated_hull.volume
         return estimated_area
@@ -548,23 +221,53 @@
         return (children, aux_data)
 
     @classmethod
     def _tree_unflatten(cls, aux_data, children):
         return cls(*children, **aux_data)
 
 
-class MultiTimestepLpConstraint(LpConstraint):
+JittableLpConstraint = collections.namedtuple(
+    "JittableLpConstraint", ["lower", "upper", "bound_type", "kwargs"]
+)
+
+
+def unjit_lp_constraints(*inputs):
+    """Replace all the jittable bounds by standard bound objects."""
+
+    def is_jittable_constraint(b):
+        return isinstance(b, JittableLpConstraint)
+
+    def unjit_bound(b):
+        return next(iter(b.bound_type)).from_jittable(b)
+
+    return jax.tree_util.tree_map(
+        lambda b: unjit_bound(b) if is_jittable_constraint(b) else b,
+        inputs,
+        is_leaf=is_jittable_constraint,
+    )
+
+
+jax.tree_util.register_pytree_node(
+    LpConstraint, LpConstraint._tree_flatten, LpConstraint._tree_unflatten
+)
+
+
+class MultiTimestepConstraint:
     # range: (num_timesteps, num_states, 2)
     def __init__(
         self,
-        range: Optional[np.ndarray] = None,
-        p: float = np.inf,
-        crown_matrices: Optional[CROWNMatrices] = None,
+        constraints: list[SingleTimestepConstraint] = [],
+        # crown_matrices: Optional[CROWNMatrices] = None,
     ):
-        super().__init__(range=range, p=p, crown_matrices=crown_matrices)
+        self.constraints = constraints
+        self.cells: list[MultiTimestepConstraint] = []
+
+    @property
+    def range(self) -> np.ndarray:
+        return np.array([constraint.range for constraint in self.constraints])
 
     def plot(
         self,
         ax,
         dims,
         color,
         fc_color="None",
@@ -578,138 +281,123 @@
                 ax,
                 dims,
                 color,
                 fc_color=fc_color,
                 linewidth=linewidth,
                 zorder=zorder,
             )
-        for i in range(len(self.range)):
-            rect = make_rect_from_arr(
-                self.range[i],
-                dims,
-                color,
-                linewidth,
-                fc_color,
-                ls,
-                zorder=zorder,
+        for constraint in self.constraints:
+            rect = constraint.plot(
+                ax, dims, color, fc_color, linewidth, zorder=zorder
             )
-            ax.add_patch(rect)
         return [rect]
 
     def plot3d(
         self,
         ax,
         dims,
         color,
         fc_color="None",
         linewidth=1,
         zorder=2,
         plot_2d=True,
     ):
         for i in range(len(self.range)):
             rect = rect_prism(
-                *self.range[i][dims, :],
+                *self.constraints[i].range[dims, :],
                 ax,
                 color,
                 linewidth,
                 fc_color,
                 zorder=zorder,
             )
         return rect
 
     def get_t_max(self) -> int:
-        if self.range is None:
-            raise ValueError(
-                "Can't get t_max from MultiTimestepLpConstraint, since"
-                " self.range is None."
-            )
-        return self.range.shape[0]
+        return len(self.constraints)
 
     def to_reachable_input_objects(
         self,
     ) -> tuple[
         Optional[np.ndarray],
         Optional[np.ndarray],
         np.ndarray,
         np.ndarray,
         float,
     ]:
-        if self.range is None:
+        assert len(self.constraints) > 0
+        last_constraint = self.constraints[-1]
+        if last_constraint.range is None:
             raise ValueError(
                 "Can't convert LpConstraint to reachable_input_objects, since"
                 " self.range is None."
             )
-        x_min = self.range[-1, :, 0]
-        x_max = self.range[-1, :, 1]
-        norm = self.p
+        x_min = last_constraint.range[:, 0]
+        x_max = last_constraint.range[:, 1]
+        norm = last_constraint.p
         A_inputs = None
         b_inputs = None
         return A_inputs, b_inputs, x_max, x_min, norm
 
-    # other should really be Union[LpConstraint, MultiTimestepLpConstraint]
     def add_timestep_constraint(
         self, other: Union[SingleTimestepConstraint, MultiTimestepConstraint]
-    ) -> MultiTimestepLpConstraint:
-        if not isinstance(other, (LpConstraint, MultiTimestepLpConstraint)):
-            raise TypeError(
-                "in add_timestep_constraint, other should be"
-                " Union[LpConstraint, MultiTimestepLpConstraint]."
-            )
+    ) -> MultiTimestepConstraint:
         if other.range is None:
             raise ValueError(
                 "Trying to add_timestep_constraint but other.range is None."
             )
         if self.range is None:
             return other.to_multistep_constraint()
-        return MultiTimestepLpConstraint(
-            range=np.vstack(
-                [self.range, other.to_multistep_constraint().range]
-            )
+        return MultiTimestepConstraint(
+            constraints=self.constraints
+            + [
+                constraint
+                for constraint in other.to_multistep_constraint().constraints
+            ]
         )
 
-    def get_constraint_at_time_index(self, i: int) -> LpConstraint:
-        if self.range is None:
-            raise ValueError(
-                "Trying to get_constraint_at_time_index, but self.range is"
-                " None"
-            )
-        return LpConstraint(range=self.range[i, ...])
+    def get_constraint_at_time_index(self, i: int) -> SingleTimestepConstraint:
+        return self.constraints[i]
 
-    def add_cell(self, other: Optional[MultiTimestepLpConstraint]) -> None:
+    def add_cell(self, other: Optional[MultiTimestepConstraint]) -> None:
         if other is None:
             return
 
         self.cells.append(other)
         self.main_constraint_stale = True
 
     def update_main_constraint_with_cells(self, overapprox: bool) -> None:
         if overapprox:
             # get min of all mins, get max of all maxes
             tmp = np.stack(
-                [c.range for c in self.cells],
+                [c.range for c in self.cells if c.range is not None],
                 axis=-1,
             )
-            self.range = np.empty_like(self.cells[0].range)
-            self.range[..., 0] = np.min(tmp[..., 0, :], axis=-1)
-            self.range[..., 1] = np.max(tmp[..., 1, :], axis=-1)
+            ranges = np.empty_like(self.cells[0].range)
+            ranges[..., 0] = np.min(tmp[..., 0, :], axis=-1)
+            ranges[..., 1] = np.max(tmp[..., 1, :], axis=-1)
+            self.constraints = []
+            for t, range in enumerate(ranges):
+                self.constraints.append(LpConstraint(range=range))
+
         else:
             raise NotImplementedError
 
         self.main_constraint_stale = False
 
-    def to_multistep_constraint(self) -> MultiTimestepLpConstraint:
+    def to_multistep_constraint(self) -> MultiTimestepConstraint:
         if self.range is None:
             raise ValueError(
                 "Trying to convert to multistep constraint but self.range is"
                 " None."
             )
         return self
 
     def to_jittable(self):
-        return JittableMultiTimestepLpConstraint(
+        return JittableMultiTimestepConstraint(
             self.range[..., 0],
             self.range[..., 1],
             {jax_verify.IntervalBound: None},
             {},
         )
 
     @classmethod
@@ -726,71 +414,145 @@
         return (children, aux_data)
 
     @classmethod
     def _tree_unflatten(cls, aux_data, children):
         return cls(*children, **aux_data)
 
 
-class MultiTimestepPolytopeConstraint(PolytopeConstraint):
-    # A: [(num_facets_0, num_states), ..., (num_facets_t, num_states)] <- num_timesteps # noqa
-    # b: [(num_facets_0,), ..., (num_facets_t,)] <- num_timesteps
+JittableMultiTimestepConstraint = collections.namedtuple(
+    "JittableMultiTimestepConstraint",
+    ["lower", "upper", "bound_type", "kwargs"],
+)
+
+
+def unjit_multi_timestep_constraints(*inputs):
+    """Replace all the jittable bounds by standard bound objects."""
+
+    def is_jittable_constraint(b):
+        return isinstance(b, JittableMultiTimestepConstraint)
+
+    def unjit_bound(b):
+        return next(iter(b.bound_type)).from_jittable(b)
+
+    return jax.tree_util.tree_map(
+        lambda b: unjit_bound(b) if is_jittable_constraint(b) else b,
+        inputs,
+        is_leaf=is_jittable_constraint,
+    )
+
+
+jax.tree_util.register_pytree_node(
+    MultiTimestepConstraint,
+    MultiTimestepConstraint._tree_flatten,
+    MultiTimestepConstraint._tree_unflatten,
+)
+
+
+class PolytopeConstraint:
+    """Represents single timestep's set of states with a H-rep polytope."""
+
     def __init__(
         self, A: Optional[np.ndarray] = None, b: Optional[np.ndarray] = None
     ):
-        super().__init__(A=A, b=b)
+        super().__init__()
+        self.A = A
+        self.b = b
+        self.cells: list[PolytopeConstraint] = []
+        self.crown_matrices: Optional[CROWNMatrices] = None
+        self.main_constraint_stale: bool = False
+        self.is_infeasible: bool = False
 
-    def plot(
-        self,
-        ax,
-        dims,
-        color,
-        fc_color="None",
-        linewidth=1.5,
-        label=None,
-        zorder=2,
-        plot_2d=True,
-        ls="-",
-    ):
-        if not plot_2d:
-            raise NotImplementedError
+    def update_main_constraint_with_cells(self, overapprox: bool) -> None:
+        if len(self.cells) == 0:
+            raise ValueError("Can't update because self.cells is empty.")
+        elif len(self.cells) == 1:
+            self.A = self.cells[0].A
+            self.b = self.cells[0].b
+            self.main_constraint_stale = False
+        else:
+            if overapprox:
+                # TODO: compute all vertices, then get conv hull using pypoman
+                raise NotImplementedError
+            else:
+                # Simplest under-approximation of union of polytopes is one of
+                # those polytopes :/
+                # TODO: compute a better under-approximation :)
+                self.A = self.cells[0].A
+                self.b = self.cells[0].b
+                self.main_constraint_stale = False
 
-        lines = []
+    def add_cell(self, other: Optional[PolytopeConstraint]) -> None:
+        if other is None:
+            return
 
-        for i in range(len(self.A)):
-            line = make_polytope_from_arrs(
-                ax, self.A[i], self.b[i], color, label, zorder, ls, linewidth
+        self.cells.append(other)
+        self.main_constraint_stale = True
+
+    def get_cell(self, input_range: np.ndarray) -> PolytopeConstraint:
+        # This is a disaster hack to partition polytopes
+        A_rect, b_rect = range_to_polytope(input_range)
+        rectangle_verts = pypoman.polygon.compute_polygon_hull(A_rect, b_rect)
+        input_polytope_verts = pypoman.polygon.compute_polygon_hull(
+            self.A, self.b
+        )
+        partition_verts = pypoman.intersection.intersect_polygons(
+            input_polytope_verts, rectangle_verts
+        )
+        (
+            A_inputs_,
+            b_inputs_,
+        ) = pypoman.duality.compute_polytope_halfspaces(partition_verts)
+        constraint = self.__class__(A_inputs_, b_inputs_)
+        return constraint
+
+    @property
+    def range(self) -> np.ndarray:
+        return self.to_range()
+
+    @property
+    def p(self) -> float:
+        return np.inf
+
+    def get_vertices(self) -> np.ndarray:
+        return np.stack(
+            pypoman.duality.compute_polytope_vertices(self.A, self.b)
+        )
+
+    def to_range(self) -> np.ndarray:
+        if self.A is None or self.b is None:
+            raise ValueError(
+                "Can't convert PolytopeConstraint to range, since self.A or"
+                " self.b are None."
             )
-            lines += line
 
-        return lines
+        # only used to compute slope in non-closedloop manner...
+        input_polytope_verts = self.get_vertices()
+        input_range = np.empty((self.A.shape[1], 2))
+        input_range[:, 0] = np.min(input_polytope_verts, axis=0)
+        input_range[:, 1] = np.max(input_polytope_verts, axis=0)
+        return input_range
 
-    def get_t_max(self) -> int:
-        if self.A is None:
+    def set_bound(self, i: int, max_value: float, min_value: float) -> None:
+        if self.b is None:
             raise ValueError(
-                "Can't get t_max from MultiTimestepPolytopeConstraint, since"
-                " self.A is None."
+                "Can't set bound on PolytopeConstraint, since self.b is None."
             )
-        return len(self.A)
+        self.b[i] = max_value
 
     def to_reachable_input_objects(
         self,
     ) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, float]:
-        if self.A is None:
-            raise ValueError(
-                "Can't convert PolytopeConstraint to"
-                " to_reachable_input_objects, since self.A is None."
-            )
-        if self.b is None:
+        if self.A is None or self.b is None:
             raise ValueError(
                 "Can't convert PolytopeConstraint to"
-                " to_reachable_input_objects, since self.b is None."
+                " to_reachable_input_objects, since self.A or self.b are None."
             )
 
-        A_inputs = self.A[0]
-        b_inputs = self.b[0]
+        A_inputs = self.A
+        b_inputs = self.b
 
         # Get bounds on each state from A_inputs, b_inputs
         try:
             vertices_list = pypoman.compute_polytope_vertices(
                 A_inputs, b_inputs
             )  # type: list[np.ndarray]
         except Exception:
@@ -800,131 +562,170 @@
             )
         vertices = np.stack(vertices_list)
         x_max = np.max(vertices, 0)  # type: np.ndarray
         x_min = np.min(vertices, 0)  # type: np.ndarray
         norm = np.inf
         return A_inputs, b_inputs, x_max, x_min, norm
 
-    # other should really be
-    # Union[PolytopeConstraint, MultiTimestepPolytopeConstraint]
-    def add_timestep_constraint(
-        self, other: Union[SingleTimestepConstraint, MultiTimestepConstraint]
-    ) -> MultiTimestepPolytopeConstraint:
-        if not isinstance(
-            other, (PolytopeConstraint, MultiTimestepPolytopeConstraint)
-        ):
-            raise TypeError(
-                "in add_timestep_constraint, other should be"
-                " Union[PolytopeConstraint, MultiTimestepPolytopeConstraint]."
-            )
-        if other.A is None or other.b is None:
+    def to_fwd_reachable_output_objects(
+        self, num_states: int
+    ) -> tuple[np.ndarray, int]:
+        if self.A is None:
             raise ValueError(
-                "Trying to add_timestep_constraint but other.A or other.b are"
-                " None."
+                "Can't convert PolytopeConstraint to"
+                " to_fwd_reachable_output_objects, since self.A is None."
             )
-        if self.A is None or self.b is None:
-            return other.to_multistep_constraint()
-        constraint = MultiTimestepPolytopeConstraint(
-            A=self.A + [other.A], b=self.b + [other.b]
-        )
-        if len(self.cells) == 0:
-            # We're adding cells to a constraint with no cells, so all those
-            # new cells should use the constraint's existing value for its
-            # first N timesteps
-            for cell in other.cells:
-                constraint.add_cell(constraint.add_timestep_constraint(cell))
+        A_out = self.A
+        num_facets = A_out.shape[0]
+        self.b = np.zeros((num_facets))
+        return A_out, num_facets
+
+    def to_linf(self) -> np.ndarray:
+        if isinstance(self.A, list):
+            # Mainly for backreachability, return a list of ranges if
+            # the constraint contains a list of polytopes
+            ranges = []
+            for A, b in zip(self.A, self.b):
+                vertices = np.stack(
+                    pypoman.duality.compute_polytope_vertices(A, b)
+                )
+                ranges.append(
+                    np.dstack(
+                        [np.min(vertices, axis=0), np.max(vertices, axis=0)]
+                    )[0]
+                )
         else:
-            # TODO: Not clear how one should combine self.cells and other.cells
+            vertices = np.stack(
+                pypoman.duality.compute_polytope_vertices(self.A, self.b)
+            )
+            ranges = np.dstack(
+                [np.min(vertices, axis=0), np.max(vertices, axis=0)]
+            )[0]
+        return ranges
+
+    def plot(
+        self,
+        ax,
+        dims,
+        color,
+        fc_color="None",
+        linewidth=1.5,
+        label=None,
+        zorder=2,
+        plot_2d=True,
+        ls="-",
+    ):
+        if not plot_2d:
             raise NotImplementedError
-        return constraint
 
-    def get_constraint_at_time_index(self, i: int) -> PolytopeConstraint:
+        # TODO: this doesn't use the computed input_dims...
+
+        if linewidth != 2.5:
+            linewidth = 1.5
+
+        lines = []
+
+        if isinstance(self.A, list):
+            # Backward reachability
+            # input_constraint.A will be a list
+            # of polytope facets, whose union is the estimated
+            # backprojection set
+
+            for A, b in zip(self.A, self.b):
+                line = make_polytope_from_arrs(
+                    ax,
+                    A,
+                    b,
+                    color,
+                    label,
+                    zorder,
+                    ls,
+                    linewidth,
+                )
+                lines += line
+
+        else:
+            # Forward reachability
+            if isinstance(self.b, np.ndarray) and self.b.ndim == 1:
+                line = make_polytope_from_arrs(
+                    ax, self.A, self.b, color, label, zorder, ls, linewidth
+                )
+                lines += line
+            else:
+                for A, b in zip(self.A, self.b):
+                    line = make_polytope_from_arrs(
+                        ax,
+                        A,
+                        b,
+                        color,
+                        label,
+                        zorder,
+                        ls,
+                        linewidth,
+                    )
+                    lines += line
+
+        return lines
+
+    def add_timestep_constraint(
+        self,
+        other: Union[SingleTimestepConstraint, MultiTimestepConstraint],
+    ) -> MultiTimestepConstraint:
+        constraints = [self] + other.to_multistep_constraint().constraints
+        return MultiTimestepConstraint(constraints=constraints)
+
+    def to_multistep_constraint(self) -> MultiTimestepConstraint:
         if self.A is None or self.b is None:
             raise ValueError(
-                "Trying to get_constraint_at_time_index, but self.A or self.b"
-                " are None"
+                "Trying to convert to multistep constraint but self.A or"
+                " self.b are None."
             )
-        constraint = PolytopeConstraint(A=self.A[i], b=self.b[i])
-        for cell in self.cells:
-            constraint.add_cell(cell.get_constraint_at_time_index(i))
+        constraint = MultiTimestepConstraint(constraints=[self])
+        constraint.cells = [
+            cell.to_multistep_constraint() for cell in self.cells
+        ]
         return constraint
 
-    def add_cell(
-        self, other: Optional[MultiTimestepPolytopeConstraint]
-    ) -> None:
-        if other is None:
-            return
+    def get_area(self) -> float:
+        estimated_verts = pypoman.polygon.compute_polygon_hull(self.A, self.b)
+        estimated_hull = ConvexHull(estimated_verts)
+        estimated_area = estimated_hull.volume
+        return estimated_area
 
-        self.cells.append(other)
-        self.main_constraint_stale = True
+    def get_polytope(self) -> tuple[np.ndarray, np.ndarray]:
+        assert self.A is not None
+        assert self.b is not None
+        return self.A, self.b
 
-    def to_multistep_constraint(self) -> MultiTimestepPolytopeConstraint:
-        if self.range is None:
-            raise ValueError(
-                "Trying to convert to multistep constraint but self.range is"
-                " None."
-            )
+    def get_constraint_at_time_index(self, i: int) -> PolytopeConstraint:
         return self
 
     def to_jittable(self):
-        return JittableMultiTimestepPolytopeConstraint(
-            self.range[..., 0],
-            self.range[..., 1],
-            {jax_verify.IntervalBound: None},
-            {},
+        return JittablePolytopeConstraint(
+            self.A, self.b, {jax_verify.IntervalBound: None}, {}
         )
 
     @classmethod
     def from_jittable(cls, jittable_constraint):
         return cls(
             range=np.array(
                 [jittable_constraint.lower, jittable_constraint.upper]
             )
         )
 
     def _tree_flatten(self):
-        children = (self.range,)  # arrays / dynamic values
+        children = (self.A, self.b)  # arrays / dynamic values
         aux_data = {}  # static values
         return (children, aux_data)
 
     @classmethod
     def _tree_unflatten(cls, aux_data, children):
         return cls(*children, **aux_data)
 
 
-MultiTimestepConstraint = Union[
-    MultiTimestepLpConstraint, MultiTimestepPolytopeConstraint
-]
-SingleTimestepConstraint = Union[LpConstraint, PolytopeConstraint]
-
-JittableLpConstraint = collections.namedtuple(
-    "JittableLpConstraint", ["lower", "upper", "bound_type", "kwargs"]
-)
-
-
-def unjit_lp_constraints(*inputs):
-    """Replace all the jittable bounds by standard bound objects."""
-
-    def is_jittable_constraint(b):
-        return isinstance(b, JittableLpConstraint)
-
-    def unjit_bound(b):
-        return next(iter(b.bound_type)).from_jittable(b)
-
-    return jax.tree_util.tree_map(
-        lambda b: unjit_bound(b) if is_jittable_constraint(b) else b,
-        inputs,
-        is_leaf=is_jittable_constraint,
-    )
-
-
-jax.tree_util.register_pytree_node(
-    LpConstraint, LpConstraint._tree_flatten, LpConstraint._tree_unflatten
-)
-
 JittablePolytopeConstraint = collections.namedtuple(
     "JittablePolytopeConstraint", ["A", "b", "bound_type", "kwargs"]
 )
 
 
 def unjit_polytope_constraints(*inputs):
     """Replace all the jittable bounds by standard bound objects."""
@@ -944,224 +745,12 @@
 
 jax.tree_util.register_pytree_node(
     PolytopeConstraint,
     PolytopeConstraint._tree_flatten,
     PolytopeConstraint._tree_unflatten,
 )
 
-JittableMultiTimestepLpConstraint = collections.namedtuple(
-    "JittableMultiTimestepLpConstraint",
-    ["lower", "upper", "bound_type", "kwargs"],
-)
-
-
-def unjit_multi_timestep_lp_constraints(*inputs):
-    """Replace all the jittable bounds by standard bound objects."""
-
-    def is_jittable_constraint(b):
-        return isinstance(b, JittableMultiTimestepLpConstraint)
-
-    def unjit_bound(b):
-        return next(iter(b.bound_type)).from_jittable(b)
 
-    return jax.tree_util.tree_map(
-        lambda b: unjit_bound(b) if is_jittable_constraint(b) else b,
-        inputs,
-        is_leaf=is_jittable_constraint,
-    )
-
-
-jax.tree_util.register_pytree_node(
-    MultiTimestepLpConstraint,
-    MultiTimestepLpConstraint._tree_flatten,
-    MultiTimestepLpConstraint._tree_unflatten,
-)
-
-JittableMultiTimestepPolytopeConstraint = collections.namedtuple(
-    "JittableMultiTimestepPolytopeConstraint",
-    ["A", "b", "bound_type", "kwargs"],
-)
-
-
-def unjit_multi_timestep_polytope_constraints(*inputs):
-    """Replace all the jittable bounds by standard bound objects."""
-
-    def is_jittable_constraint(b):
-        return isinstance(b, JittableMultiTimestepPolytopeConstraint)
-
-    def unjit_bound(b):
-        return next(iter(b.bound_type)).from_jittable(b)
-
-    return jax.tree_util.tree_map(
-        lambda b: unjit_bound(b) if is_jittable_constraint(b) else b,
-        inputs,
-        is_leaf=is_jittable_constraint,
-    )
-
-
-jax.tree_util.register_pytree_node(
-    MultiTimestepPolytopeConstraint,
-    MultiTimestepPolytopeConstraint._tree_flatten,
-    MultiTimestepPolytopeConstraint._tree_unflatten,
-)
-
-
-def make_rect_from_arr(
-    arr: np.ndarray,
-    dims: np.ndarray,
-    color: str,
-    linewidth: float,
-    fc_color: str,
-    ls: int,
-    zorder: Optional[int] = None,
-    angle: float = 0.0,
-) -> Rectangle:
-    rect = Rectangle(
-        arr[dims, 0],
-        arr[dims[0], 1] - arr[dims[0], 0],
-        arr[dims[1], 1] - arr[dims[1], 0],
-        angle=angle,
-        fc=fc_color,
-        linewidth=linewidth,
-        edgecolor=color,
-        zorder=zorder,
-        linestyle=ls,
-    )
-    return rect
-
-
-class RotatedLpConstraint(Constraint):
-    def __init__(self, pose=None, W=None, theta=0, vertices=None):
-        Constraint.__init__(self)
-        self.width = W
-        self.theta = theta
-        self.pose = pose
-        self.bounding_box = np.vstack(
-            (np.min(vertices, axis=0), np.max(vertices, axis=0))
-        ).T
-        self.vertices = vertices
-
-    def plot(
-        self,
-        ax,
-        plot_2d=True,
-    ):
-        if not plot_2d:
-            raise NotImplementedError
-        from scipy.spatial import ConvexHull, convex_hull_plot_2d
-
-        hull = ConvexHull(self.vertices)
-        convex_hull_plot_2d(hull, ax)
-
-    def plot3d(
-        self,
-        ax,
-        dims,
-        color,
-        fc_color="None",
-        linewidth=1,
-        zorder=2,
-        plot_2d=True,
-    ):
-        raise NotImplementedError
-
-    def get_t_max(self):
-        return len(self.bounding_box)
-
-
-def make_polytope_from_arrs(
-    ax,
-    A: np.ndarray,
-    b: np.ndarray,
-    color: str,
-    label: str,
-    zorder: int,
-    ls: str,
-    linewidth: float = 1.5,
-) -> list:
-    vertices = np.stack(pypoman.polygon.compute_polygon_hull(A, b + 1e-10))
-    lines = ax.plot(
-        [v[0] for v in vertices] + [vertices[0][0]],
-        [v[1] for v in vertices] + [vertices[0][1]],
-        color=color,
-        label=label,
-        zorder=zorder,
-        ls=ls,
-        linewidth=linewidth,
-    )
-    return lines
-
-
-def create_empty_constraint(
-    boundary_type: str, num_facets: Optional[int] = None
-) -> SingleTimestepConstraint:
-    if boundary_type == "polytope":
-        if num_facets:
-            return PolytopeConstraint(A=get_polytope_A(num_facets))
-        return PolytopeConstraint()
-    elif boundary_type == "rectangle":
-        return LpConstraint()
-    else:
-        raise NotImplementedError
-
-
-def create_empty_multi_timestep_constraint(
-    boundary_type: str, num_facets: Optional[int] = None
-) -> MultiTimestepConstraint:
-    if boundary_type == "polytope":
-        if num_facets:
-            return MultiTimestepPolytopeConstraint(
-                A=get_polytope_A(num_facets)
-            )
-        return MultiTimestepPolytopeConstraint()
-    elif boundary_type == "rectangle":
-        return MultiTimestepLpConstraint()
-    else:
-        raise NotImplementedError
-
-
-def state_range_to_constraint(
-    state_range: np.ndarray, boundary_type: str
-) -> Constraint:
-    if boundary_type == "polytope":
-        A, b = range_to_polytope(state_range)
-        return PolytopeConstraint(A, b)
-    elif boundary_type == "rectangle":
-        return LpConstraint(range=state_range, p=np.inf)
-    else:
-        raise NotImplementedError
-
-
-def is_lp_constraint_list(xs: list[Any]) -> TypeGuard[list[LpConstraint]]:
-    return all(
-        isinstance(x, LpConstraint) and isinstance(x.range, np.ndarray)
-        for x in xs
-    )
-
-
-def is_polytope_constraint_list(
-    xs: list[Any],
-) -> TypeGuard[list[PolytopeConstraint]]:
-    return all(isinstance(x, PolytopeConstraint) for x in xs)
-
-
-def is_npndarray_list(xs: list[Any]) -> TypeGuard[list[np.ndarray]]:
-    return all(isinstance(x, np.ndarray) for x in xs)
-
-
-def list_to_constraint(
-    reachable_sets: Union[list[LpConstraint], list[PolytopeConstraint]]
-) -> MultiTimestepConstraint:
-    if is_lp_constraint_list(reachable_sets):
-        range = [r.range for r in reachable_sets]
-        assert is_npndarray_list(range)  # ensure all ranges are not None
-        return MultiTimestepLpConstraint(range=np.stack(range))
-    elif is_polytope_constraint_list(reachable_sets):
-        As = [r.A for r in reachable_sets]
-        bs = [r.b for r in reachable_sets]
-        assert is_npndarray_list(As)  # ensure all As are not None
-        assert is_npndarray_list(bs)  # ensure all bs are not None
-        return MultiTimestepPolytopeConstraint(A=np.stack(As), b=np.stack(bs))
-    else:
-        raise ValueError(
-            "reachable_sets list contains constraints with None range or A, b."
-        )
+SingleTimestepConstraint = Union[LpConstraint, PolytopeConstraint]
+JittableSingleTimestepConstraint = Union[
+    JittableLpConstraint, JittablePolytopeConstraint
+]
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DiscreteQuadrotor.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/DiscreteQuadrotor.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegrator.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/DoubleIntegrator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegratorOutputFeedback.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/DoubleIntegratorOutputFeedback.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegratorx4.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/DoubleIntegratorx4.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Duffing.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Duffing.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Dynamics.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Dynamics.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/GroundRobotDI.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/GroundRobotDI.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/GroundRobotSI.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/GroundRobotSI.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/ISS.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/ISS.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/ISS_discrete.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/ISS_discrete.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Pendulum.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Pendulum.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Quadrotor.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/QuadrotorOutputFeedback.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/QuadrotorOutputFeedback.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/QuadrotorOutputFeedback_v0.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/QuadrotorOutputFeedback_v0.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor_8D.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Quadrotor_8D.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor_v0.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Quadrotor_v0.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Taxinet.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Taxinet.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Unicycle.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Unicycle.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Unity.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/Unity.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/__init__.py` & `nfl_veripy-0.0.2/src/nfl_veripy/dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/elements/Element.py` & `nfl_veripy-0.0.2/src/nfl_veripy/elements/Element.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/elements/GuidedElement.py` & `nfl_veripy-0.0.2/src/nfl_veripy/elements/GuidedElement.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/elements/OptGuidedElement.py` & `nfl_veripy-0.0.2/src/nfl_veripy/elements/OptGuidedElement.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/ClosedLoopExperiments.py` & `nfl_veripy-0.0.2/src/nfl_veripy/experiments/ClosedLoopExperiments.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/backward_experiments.py` & `nfl_veripy-0.0.2/src/nfl_veripy/experiments/backward_experiments.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/experiments.py` & `nfl_veripy-0.0.2/src/nfl_veripy/experiments/experiments.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/expts.py` & `nfl_veripy-0.0.2/src/nfl_veripy/experiments/expts.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/AdaptiveGreedySimGuidedPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/AdaptiveGreedySimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/BoundarySimGuidedPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/BoundarySimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopGreedySimGuidedPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopGreedySimGuidedPartitioner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,77 @@
+from typing import Optional
+
 import numpy as np
 
+import nfl_veripy.constraints as constraints
+import nfl_veripy.dynamics as dynamics
+
 from .ClosedLoopSimGuidedPartitioner import ClosedLoopSimGuidedPartitioner
 
 
 class ClosedLoopGreedySimGuidedPartitioner(ClosedLoopSimGuidedPartitioner):
     def __init__(
         self,
-        dynamics,
-        num_partitions=16,
-        make_animation=False,
-        show_animation=False,
+        dynamics: dynamics.Dynamics,
     ):
-        ClosedLoopSimGuidedPartitioner.__init__(
-            self,
-            dynamics=dynamics,
-            make_animation=make_animation,
-            show_animation=show_animation,
-        )
+        super().__init__(dynamics=dynamics)
 
-    def grab_from_M(self, M, output_range_sim):
+    def grab_from_M(
+        self,
+        M: list[
+            tuple[
+                constraints.SingleTimestepConstraint,
+                constraints.MultiTimestepConstraint,
+            ]
+        ],
+        output_range_sim: Optional[np.ndarray],
+    ) -> tuple[
+        constraints.SingleTimestepConstraint,
+        constraints.MultiTimestepConstraint,
+    ]:
         if len(M) == 1:
-            input_range_, output_range_ = M.pop(0)
+            input_range, output_range = M.pop(0)
         else:
             if self.interior_condition == "linf":
                 # TEMP:
                 # choose solely based on first timestep!
                 # timestep_of_interest = 0
                 # choose solely based on last timestep!
                 timestep_of_interest = -1
 
-                M_last_timestep = [
-                    (inp, out.range[timestep_of_interest]) for (inp, out) in M
-                ]
+                output_range_last_timestep = np.array(
+                    [
+                        out.get_constraint_at_time_index(
+                            timestep_of_interest
+                        ).range
+                        for (_, out) in M
+                    ]
+                ).transpose(1, 2, 0)
+                assert output_range_sim is not None
                 output_range_sim_last_timestep = output_range_sim[
                     timestep_of_interest
                 ]
 
                 # look thru all output_range_s and see which are furthest from
                 # sim output range
-                M_numpy = np.dstack(
-                    [output_range_ for (_, output_range_) in M_last_timestep]
-                )
-                z = np.empty_like(M_numpy)
+                z = np.empty_like(output_range_last_timestep)
                 z[:, 0, :] = (
-                    output_range_sim_last_timestep[:, 0] - M_numpy[:, 0, :].T
+                    output_range_sim_last_timestep[:, 0]
+                    - output_range_last_timestep[:, 0, :].T
                 ).T
                 z[:, 1, :] = (
-                    M_numpy[:, 1, :].T - output_range_sim_last_timestep[:, 1]
+                    output_range_last_timestep[:, 1, :].T
+                    - output_range_sim_last_timestep[:, 1]
                 ).T
+
                 # This selects whatver output range is furthest from
                 # a boundary --> however, it can get too fixated on a single
                 # bndry, esp when there's a sharp corner, suggesting
                 # we might need to sample more, because our idea of where the
                 # sim bndry is might be too far inward
                 worst_index = np.unravel_index(z.argmax(), shape=z.shape)
                 worst_M_index = worst_index[-1]
-                input_range_, output_range_ = M.pop(worst_M_index)
+                input_range, output_range = M.pop(worst_M_index)
             else:
                 raise NotImplementedError
 
-        return input_range_, output_range_
+        return input_range, output_range
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopCROWNIBPCodebasePropagator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,765 +1,958 @@
-import os
 from copy import deepcopy
-from typing import Any, Optional, Union
+from typing import Optional
 
 import cvxpy as cp
-import matplotlib.pyplot as plt
 import numpy as np
 import pypoman
-from matplotlib.lines import Line2D
-from matplotlib.patches import Patch
-from scipy.spatial import ConvexHull
+import torch
 
 import nfl_veripy.constraints as constraints
 import nfl_veripy.dynamics as dynamics
-import nfl_veripy.propagators as propagators
-from nfl_veripy.utils.optimization_utils import optimize_over_all_states
-from nfl_veripy.utils.utils import range_to_polytope
+from nfl_veripy.utils.nn_bounds import BoundClosedLoopController
+from nfl_veripy.utils.optimization_utils import (
+    optimization_results_to_backprojection_set,
+    optimize_over_all_states,
+)
+from nfl_veripy.utils.utils import get_crown_matrices
+
+from .ClosedLoopPropagator import ClosedLoopPropagator
+
+
+class ClosedLoopCROWNIBPCodebasePropagator(ClosedLoopPropagator):
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.params: dict[str, bool] = {}
+        self.method_opt: str = "TODO"
+
+    def torch2network(
+        self, torch_model: torch.nn.Sequential
+    ) -> BoundClosedLoopController:
+        torch_model_cl = BoundClosedLoopController.convert(
+            torch_model, dynamics=self.dynamics, bound_opts=self.params
+        )
+        return torch_model_cl
+
+    def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
+        return self.network(
+            torch.Tensor(input_data), method_opt=None
+        ).data.numpy()
 
-from .Partitioner import Partitioner
+    def get_one_step_reachable_set(
+        self, initial_set: constraints.SingleTimestepConstraint
+    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
+        A_inputs, b_inputs, x_max, x_min, norm = (
+            initial_set.to_reachable_input_objects()
+        )
 
+        reachable_set = constraints.create_empty_constraint(
+            self.boundary_type, num_facets=self.num_polytope_facets
+        )
+        A_out, num_facets = reachable_set.to_fwd_reachable_output_objects(
+            self.dynamics.num_states
+        )
+
+        # Because there might sensor noise, the NN could see a different set of
+        # states than the system is actually in
+        prev_state_max = torch.Tensor(np.array([x_max]))
+        prev_state_min = torch.Tensor(np.array([x_min]))
+        nn_input_max = prev_state_max
+        nn_input_min = prev_state_min
+        if self.dynamics.sensor_noise is not None:
+            nn_input_max += torch.Tensor(
+                np.array([self.dynamics.sensor_noise[:, 1]])
+            )
+            nn_input_min += torch.Tensor(
+                np.array([self.dynamics.sensor_noise[:, 0]])
+            )
+
+        # Compute the NN output matrices (for the input constraints)
+        num_control_inputs = self.dynamics.bt.shape[1]
+        C = torch.eye(num_control_inputs).unsqueeze(0)
+        lower_A, upper_A, lower_sum_b, upper_sum_b = self.network(
+            method_opt=self.method_opt,
+            norm=norm,
+            x_U=nn_input_max,
+            x_L=nn_input_min,
+            upper=True,
+            lower=True,
+            C=C,
+            return_matrices=True,
+        )
+
+        for i in range(num_facets):
+            # For each dimension of the output constraint (facet/lp-dimension):
+            # compute a bound of the NN output using the pre-computed matrices
+            if A_out is None:
+                A_out_torch = None
+            else:
+                A_out_torch = torch.Tensor(np.array([A_out[i, :]]))
+
+            # CROWN was initialized knowing dynamics, no need to pass them here
+            # (unless they've changed, e.g., time-varying At matrix)
+            (
+                A_out_xt1_max,
+                A_out_xt1_min,
+            ) = self.network.compute_bound_from_matrices(
+                lower_A,
+                lower_sum_b,
+                upper_A,
+                upper_sum_b,
+                prev_state_max,
+                prev_state_min,
+                norm,
+                A_out_torch,
+                A_in=A_inputs,
+                b_in=b_inputs,
+            )
+
+            reachable_set.set_bound(i, A_out_xt1_max, A_out_xt1_min)
+
+        # Auxiliary info
+        nn_matrices = {
+            "lower_A": lower_A.data.numpy()[0],
+            "upper_A": upper_A.data.numpy()[0],
+            "lower_sum_b": lower_sum_b.data.numpy()[0],
+            "upper_sum_b": upper_sum_b.data.numpy()[0],
+        }
 
-class ClosedLoopPartitioner(Partitioner):
-    def __init__(
-        self,
-        dynamics: dynamics.Dynamics,
-        make_animation: bool = False,
-        show_animation: bool = False,
-    ):
-        super().__init__()
-        self.dynamics = dynamics
+        return reachable_set, {"nn_matrices": nn_matrices}
 
-        # Animation-related flags
-        self.make_animation = make_animation
-        self.show_animation = show_animation
-        self.tmp_animation_save_dir = "{}/../../results/tmp_animation/".format(
-            os.path.dirname(os.path.abspath(__file__))
-        )
-        self.animation_save_dir = "{}/../../results/animations/".format(
-            os.path.dirname(os.path.abspath(__file__))
-        )
+    """
+    Inputs:
+        target_set:
+            - constraints.LpConstraint: set of final states to backproject
+            from, OR
+            - [constraints.LpConstraint, ...]: [X_T, BP_{-1}, ...,]
+        input_constriant: empty constraint object
+        overapprox: flag to calculate over approximations of the BP set (set
+            to true gives algorithm 1 in CDC 2022)
+
+    Outputs:
+        input_constraint: one step BP set estimate
+        info: dict with extra info (e.g. backreachable set, etc.)
+    """
 
-    def get_one_step_reachable_set(
+    def get_one_step_backprojection_set(
         self,
-        initial_set: constraints.SingleTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
-        reachable_set, info = propagator.get_one_step_reachable_set(
-            initial_set
+        backreachable_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+        overapprox: bool = False,
+        info: dict = {},
+        facet_inds_to_optimize: Optional[np.ndarray] = None,
+    ) -> tuple[Optional[constraints.SingleTimestepConstraint], dict]:
+        backreachable_set.crown_matrices = get_crown_matrices(
+            self,
+            backreachable_set,
+            self.dynamics.num_inputs,
+            self.dynamics.sensor_noise,
         )
-        return reachable_set, info
 
-    def get_reachable_set(
+        if overapprox:
+            backprojection_set = (
+                self.get_one_step_backprojection_set_overapprox(
+                    backreachable_set,
+                    target_sets,
+                    facet_inds_to_optimize=facet_inds_to_optimize,
+                )
+            )
+        else:
+            backprojection_set = (
+                self.get_one_step_backprojection_set_underapprox(
+                    backreachable_set, target_sets
+                )
+            )
+
+        return backprojection_set, info
+
+    """
+    Inputs:
+        ranges: section of backreachable set
+        upper_A, lower_A, upper_sum_b, lower_sum_b: CROWN variables
+        xt1max, xt1min: target set max values
+        input_constraint: empty constraint object
+    Outputs:
+        input_constraint: one step BP set under-approximation
+    """
+
+    def get_one_step_backprojection_set_underapprox(
         self,
-        initial_set: constraints.SingleTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-        t_max: int,
-    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
-        reachable_set, info = propagator.get_reachable_set(initial_set, t_max)
-        return reachable_set, info
+        backreachable_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+    ) -> Optional[constraints.PolytopeConstraint]:
+        # For our under-approximation, refer to the Access21 paper.
 
-        # # TODO: this is repeated from UniformPartitioner...
-        # # might be more efficient to directly return from propagator?
-        # _ = reachable_set.add_cell(reachable_set_this_cell)
+        if not backreachable_set.crown_matrices:
+            raise ValueError("Need to set backreachable_set.crown_matrices.")
+        upper_A, lower_A, upper_sum_b, lower_sum_b = (
+            backreachable_set.crown_matrices.to_numpy()
+        )
+
+        target_set = target_sets.get_constraint_at_time_index(0)
+        target_set_range = target_set.to_range()
+        assert (
+            target_set_range is not None
+        ), "target_set.range is None -- make sure it's set to an array."
+
+        # The NN matrices define three types of constraints:
+        # - NN's resulting lower bnds on xt1 >= lower bnds on xt1
+        # - NN's resulting upper bnds on xt1 <= upper bnds on xt1
+        # - NN matrices are only valid within the partition
+        A_NN, b_NN = backreachable_set.get_polytope()
+        A = np.vstack(
+            [
+                (self.dynamics.At + self.dynamics.bt @ upper_A),
+                -(self.dynamics.At + self.dynamics.bt @ lower_A),
+                A_NN,
+            ]
+        )
+        b = np.hstack(
+            [
+                target_set_range[:, 1] - self.dynamics.bt @ upper_sum_b,
+                -target_set_range[:, 0] + self.dynamics.bt @ lower_sum_b,
+                b_NN,
+            ]
+        )
+
+        # If those constraints to a non-empty set, then add it to
+        # the list of input_constraints. Otherwise, skip it.
+        try:
+            pypoman.polygon.compute_polygon_hull(A, b + 1e-10)
+        except Exception:
+            return None
 
-        # return reachable_set, info
+        backprojection_set = constraints.PolytopeConstraint(A=A, b=b)
 
-    def get_error(  # type: ignore
+        return backprojection_set
+
+    def get_one_step_backprojection_set_overapprox(
         self,
-        initial_set: constraints.SingleTimestepConstraint,
-        reachable_sets: constraints.MultiTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-        t_max: int,
-    ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
-        errors = []
-
-        if isinstance(initial_set, constraints.LpConstraint) and isinstance(
-            reachable_sets, constraints.MultiTimestepLpConstraint
-        ):
-            estimated_reachable_set_ranges = reachable_sets.to_range()
-            true_reachable_set_ranges = self.get_sampled_out_range(
-                initial_set, propagator, t_max, num_samples=1000
-            )
-            num_steps = true_reachable_set_ranges.shape[0]
-            for t in range(num_steps):
-                true_area = np.product(
-                    true_reachable_set_ranges[t][..., 1]
-                    - true_reachable_set_ranges[t][..., 0]
-                )
-                estimated_area = np.product(
-                    estimated_reachable_set_ranges[t][..., 1]
-                    - estimated_reachable_set_ranges[t][..., 0]
+        backreachable_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+        facet_inds_to_optimize: Optional[np.ndarray] = None,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
+        backprojection_set: Optional[constraints.SingleTimestepConstraint] = (
+            deepcopy(backreachable_set)
+        )
+        for _ in range(self.num_iterations):
+            if backprojection_set is None:
+                continue
+            backprojection_set = (
+                self.improve_one_step_backprojection_set_overapprox(
+                    backprojection_set,
+                    target_sets,
+                    facet_inds_to_optimize=facet_inds_to_optimize,
                 )
-                errors.append((estimated_area - true_area) / true_area)
-        elif isinstance(
-            initial_set, constraints.PolytopeConstraint
-        ) and isinstance(
-            reachable_sets, constraints.MultiTimestepPolytopeConstraint
-        ):
-            # Note: This compares the estimated polytope
-            # with the "best" polytope with those facets.
-            # There could be a much better polytope with lots of facets.
-            true_verts = self.get_sampled_out_range(
-                initial_set,
-                propagator,
-                t_max,
-                num_samples=1000,
-                output_constraint=reachable_sets,
             )
+        return backprojection_set
 
-            num_steps = reachable_sets.get_t_max()
-            from scipy.spatial import ConvexHull
+    """
+    CDC 2022 Paper Alg 1
 
-            for t in range(num_steps):
-                true_hull = ConvexHull(true_verts[:, t + 1, :])
-                true_area = true_hull.volume
-                if reachable_sets.A is None or reachable_sets.b is None:
-                    raise ValueError(
-                        "Can't compute polygon hull because reachable_sets has"
-                        " Nones in it."
-                    )
-                estimated_verts = pypoman.polygon.compute_polygon_hull(
-                    reachable_sets.A[t], reachable_sets.b[t]
-                )
-                estimated_hull = ConvexHull(estimated_verts)
-                estimated_area = estimated_hull.volume
-                errors.append((estimated_area - true_area) / true_area)
-        else:
-            raise ValueError(
-                "initial_set and reachable_sets need to both be Lp or both be"
-                " Polytope."
-            )
-        final_error = errors[-1]
-        avg_error = np.mean(errors)
-        return final_error, avg_error, np.array(errors)
+    Inputs:
+        backreachable_set: our current best bounds on BP (this could be a BR
+            or a BP from a previous iteration)
+        target_sets: [target_set, BP_{-1}, ..., BP{-T}]
+            * Note: only target_set is used for this algorithm! (other BPs are
+                discarded)
+        facet_inds_to_optimize: Assuming facets are [I, -I], list/array of
+            indices to optimize over
+    Outputs:
+        backprojection_set: a tighter version of backreachable_set
+    """
 
-    def get_sampled_out_range(
+    def improve_one_step_backprojection_set_overapprox(
         self,
-        initial_set: constraints.SingleTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-        t_max: int = 5,
-        num_samples: int = 1000,
-        output_constraint: Optional[
-            constraints.SingleTimestepConstraint
-        ] = None,
-    ) -> np.ndarray:
-        # TODO: change output_constraint to better name
-        return self.dynamics.get_sampled_output_range(
-            initial_set,
-            t_max,
-            num_samples,
-            controller=propagator.network,
-            output_constraint=output_constraint,
+        backreachable_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+        facet_inds_to_optimize: Optional[np.ndarray] = None,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
+        num_states, num_control_inputs = self.dynamics.bt.shape
+
+        # An over-approximation of the backprojection set is the set of:
+        # all x_t s.t. there exists some u \in [pi^L(x_t), pi^U(x_t)]
+        #              that leads to the target set
+
+        xt = cp.Variable(num_states)
+        ut = cp.Variable(num_control_inputs)
+        constrs = []
+
+        # Constraints to ensure that xt stays within the backreachable set
+        A_backreach, b_backreach = backreachable_set.get_polytope()
+        constrs += [A_backreach @ xt <= b_backreach]
+
+        # Constraints to ensure that ut satisfies the affine bounds
+        if backreachable_set.crown_matrices is None:
+            backreachable_set.crown_matrices = get_crown_matrices(
+                self,
+                backreachable_set,
+                self.dynamics.num_inputs,
+                self.dynamics.sensor_noise,
+            )
+        assert (
+            backreachable_set.crown_matrices is not None
+        ), "Need to set backreachable_set.crown_matrices."
+        constrs += [
+            backreachable_set.crown_matrices.lower_A_numpy @ xt
+            + backreachable_set.crown_matrices.lower_sum_b_numpy
+            <= ut
+        ]
+        constrs += [
+            ut
+            <= backreachable_set.crown_matrices.upper_A_numpy @ xt
+            + backreachable_set.crown_matrices.upper_sum_b_numpy
+        ]
+
+        # Constraints to ensure xt reaches the "target set" given ut
+        # ... where target set = our best bounds on the next state set
+        # (i.e., either the true target set or a backprojection set)
+        A_target, b_target = target_sets.get_constraint_at_time_index(
+            -1
+        ).get_polytope()
+        constrs += [A_target @ self.dynamics.dynamics_step(xt, ut) <= b_target]
+
+        b, status = optimize_over_all_states(
+            xt, constrs, facet_inds_to_optimize=facet_inds_to_optimize
         )
 
-    def get_sampled_out_range_guidance(
-        self,
-        initial_set: constraints.SingleTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-        t_max: int = 5,
-        num_samples: int = 1000,
-    ) -> np.ndarray:
-        # Duplicate of get_sampled_out_range, but called during partitioning
-        return self.get_sampled_out_range(
-            initial_set, propagator, t_max=t_max, num_samples=num_samples
+        backprojection_set = optimization_results_to_backprojection_set(
+            status, b, backreachable_set
         )
 
-    def setup_visualization(
-        self,
-        initial_set: constraints.SingleTimestepConstraint,
-        t_max: int,
-        propagator: propagators.ClosedLoopPropagator,
-        show_samples: bool = True,
-        show_samples_from_cells: bool = True,
-        show_trajectories: bool = False,
-        axis_labels: Optional[list] = None,
-        axis_dims: Optional[list] = None,
-        aspect: str = "auto",
-        initial_set_color: Optional[str] = None,
-        initial_set_zorder: Optional[int] = None,
-        extra_set_color: Optional[str] = None,
-        extra_set_zorder: Optional[int] = None,
-        sample_zorder: Optional[int] = None,
-        sample_colors: Optional[str] = None,
-        extra_constraint: Optional[
-            constraints.SingleTimestepConstraint
-        ] = None,
-        plot_lims: Optional[list] = None,
-        controller_name: Optional[str] = None,
-    ) -> None:
-        self.default_patches = []
-        self.default_lines = []
-
-        self.axis_dims = axis_dims
-
-        if len(axis_dims) == 2:
-            projection = None
-            self.plot_2d = True
-            self.linewidth = 2
-        elif len(axis_dims) == 3:
-            projection = "3d"
-            self.plot_2d = False
-            self.linewidth = 1
-            aspect = "auto"
-
-        self.animate_fig, self.animate_axes = plt.subplots(
-            1, 1, subplot_kw=dict(projection=projection)
-        )
-        if controller_name is not None:
-            from nfl_veripy.utils.controller_generation import (
-                display_ground_robot_control_field,
-            )
-
-            display_ground_robot_control_field(
-                name=controller_name, ax=self.animate_axes
-            )
-
-        # if controller_name is not None:
-        #     from nfl_veripy.utils.controller_generation import (
-        #         display_ground_robot_DI_control_field,
-        #     )
+        return backprojection_set
 
-        #     display_ground_robot_DI_control_field(
-        #         name=controller_name, ax=self.animate_axes
+    def setup_LPs(self, nstep=False, bp_sets=None):
+        raise NotImplementedError
+        # if nstep:
+        #     return self.setup_LPs_nstep(
+        #         modifier=modifier, infos=infos, bp_sets=bp_sets
         #     )
+        # else:
+        #     return self.setup_LPs_1step()
 
-        self.animate_axes.set_aspect(aspect)
+    def setup_LPs_1step(self):
+        # TODO: accept this as arg
+        boundaries = "rectangle"
 
-        if show_samples:
-            self.dynamics.show_samples(
-                t_max * self.dynamics.dt,
-                initial_set,
-                ax=self.animate_axes,
-                controller=propagator.network,
-                input_dims=axis_dims,
-                zorder=sample_zorder,
-                colors=sample_colors,
-            )
-
-        if show_samples_from_cells:
-            for initial_set_cell in initial_set.cells:
-                self.dynamics.show_samples(
-                    t_max * self.dynamics.dt,
-                    initial_set_cell,
-                    ax=self.animate_axes,
-                    controller=propagator.network,
-                    input_dims=axis_dims,
-                    zorder=sample_zorder,
-                    colors=sample_colors,
-                )
+        num_states = self.dynamics.At.shape[0]
+        num_control_inputs = self.dynamics.bt.shape[1]
 
-        if show_trajectories:
-            self.dynamics.show_trajectories(
-                t_max * self.dynamics.dt,
-                initial_set,
-                ax=self.animate_axes,
-                controller=propagator.network,
-                input_dims=axis_dims,
-                zorder=sample_zorder,
-                colors=sample_colors,
-            )
-
-        self.animate_axes.set_xlabel(axis_labels[0])
-        self.animate_axes.set_ylabel(axis_labels[1])
-        if not self.plot_2d:
-            self.animate_axes.set_zlabel(axis_labels[2])
-
-        # Plot the initial state set's boundaries
-        if initial_set_color is None:
-            initial_set_color = "tab:grey"
-        rect = initial_set.plot(
-            self.animate_axes,
-            axis_dims,
-            initial_set_color,
-            zorder=initial_set_zorder,
-            linewidth=self.linewidth,
-            plot_2d=self.plot_2d,
-        )
-        self.default_patches += rect
-
-        if show_samples_from_cells:
-            for cell in initial_set.cells:
-                rect = initial_set_cell.plot(
-                    self.animate_axes,
-                    axis_dims,
-                    initial_set_color,
-                    zorder=initial_set_zorder,
-                    linewidth=self.linewidth,
-                    plot_2d=self.plot_2d,
-                )
-                self.default_patches += rect
+        xt = cp.Variable(num_states)
+        ut = cp.Variable(num_control_inputs)
 
-        if extra_set_color is None:
-            extra_set_color = "tab:red"
-        # if extra_constraint[0] is not None:
-        #     for i in range(len(extra_constraint)):
-        #         rect = extra_constraint[i].plot(
-        #             self.animate_axes,
-        #             input_dims,
-        #             extra_set_color,
-        #             zorder=extra_set_zorder,
-        #             linewidth=self.linewidth,
-        #             plot_2d=self.plot_2d,
-        #         )
-        #         self.default_patches += rect
+        lower_A = cp.Parameter((num_control_inputs, num_states))
+        upper_A = cp.Parameter((num_control_inputs, num_states))
+        lower_sum_b = cp.Parameter(num_control_inputs)
+        upper_sum_b = cp.Parameter(num_control_inputs)
+
+        if boundaries == "rectangle":
+            xt_min = cp.Parameter(num_states)
+            xt_max = cp.Parameter(num_states)
+
+            xt1_min = cp.Parameter(num_states)
+            xt1_max = cp.Parameter(num_states)
+
+            A_t = cp.Parameter(num_states)
+
+            params = {
+                "lower_A": lower_A,
+                "upper_A": upper_A,
+                "lower_sum_b": lower_sum_b,
+                "upper_sum_b": upper_sum_b,
+                "xt_min": xt_min,
+                "xt_max": xt_max,
+                "xt1_min": xt1_min,
+                "xt1_max": xt1_max,
+                "A_t": A_t,
+            }
+
+            constrs = []
+            constrs += [lower_A @ xt + lower_sum_b <= ut]
+            constrs += [ut <= upper_A @ xt + upper_sum_b]
+
+            # Included state limits to reduce size of backreachable sets by
+            # eliminating states that are not physically possible
+            # (e.g., maximum velocities)
+            constrs += [xt_min <= xt]
+            constrs += [xt <= xt_max]
+
+            # Dynamics must be satisfied
+            constrs += [self.dynamics.dynamics_step(xt, ut) <= xt1_max]
+            constrs += [self.dynamics.dynamics_step(xt, ut) >= xt1_min]
+
+        elif boundaries == "rotated":
+            xt_min = cp.Parameter(num_states)
+            xt_max = cp.Parameter(num_states)
+
+            R = cp.Parameter((num_states, num_states))
+            pose = cp.Parameter(num_states)
+            W = cp.Parameter(num_states)
+
+            A_t = cp.Parameter(num_states)
+
+            params = {
+                "lower_A": lower_A,
+                "upper_A": upper_A,
+                "lower_sum_b": lower_sum_b,
+                "upper_sum_b": upper_sum_b,
+                "xt_min": xt_min,
+                "xt_max": xt_max,
+                "R": R,
+                "W": W,
+                "pose": pose,
+                "A_t": A_t,
+            }
+
+            constrs = []
+            constrs += [lower_A @ xt + lower_sum_b <= ut]
+            constrs += [ut <= upper_A @ xt + upper_sum_b]
+
+            # Included state limits to reduce size of backreachable sets by
+            # eliminating states that are not physically possible
+            # (e.g., maximum velocities)
+            constrs += [xt_min <= xt]
+            constrs += [xt <= xt_max]
+
+            # Dynamics must be satisfied
+
+            constrs += [
+                R @ self.dynamics.dynamics_step(xt, ut) - R @ pose <= W
+            ]
+            constrs += [
+                R @ self.dynamics.dynamics_step(xt, ut) - R @ pose
+                >= np.array([0, 0])
+            ]
+
+        obj = A_t @ xt
+        min_prob = cp.Problem(cp.Minimize(obj), constrs)
+        max_prob = cp.Problem(cp.Maximize(obj), constrs)
 
-    def visualize(  # type: ignore
-        self,
-        M: list,
-        interior_M: list,
-        reachable_sets: constraints.MultiTimestepConstraint,
-        iteration: int = 0,
-        title: Optional[str] = None,
-        reachable_set_color: Optional[str] = None,
-        reachable_set_zorder: Optional[int] = None,
-        reachable_set_ls: Optional[str] = None,
-        dont_tighten_layout: bool = False,
-        plot_lims: Optional[str] = None,
-    ) -> None:
-        # Bring forward whatever default items should be in the plot
-        # (e.g., MC samples, initial state set boundaries)
-        for item in self.default_patches + self.default_lines:
-            if isinstance(item, Patch):
-                self.animate_axes.add_patch(item)
-            elif isinstance(item, Line2D):
-                self.animate_axes.add_line(item)
-
-        self.plot_reachable_sets(
-            reachable_sets,
-            self.axis_dims,
-            reachable_set_color=reachable_set_color,
-            reachable_set_zorder=reachable_set_zorder,
-            reachable_set_ls=reachable_set_ls,
-        )
-
-        if plot_lims is not None:
-            import ast
-
-            plot_lims_arr = np.array(ast.literal_eval(plot_lims))
-            plt.xlim(plot_lims_arr[0])
-            plt.ylim(plot_lims_arr[1])
-
-        # Do auxiliary stuff to make sure animations look nice
-        if title is not None:
-            plt.suptitle(title)
-
-        if (iteration == 0 or iteration == -1) and not dont_tighten_layout:
-            plt.tight_layout()
-
-        if self.show_animation:
-            plt.pause(0.01)
-
-        if self.make_animation and iteration is not None:
-            os.makedirs(self.tmp_animation_save_dir, exist_ok=True)
-            filename = self.get_tmp_animation_filename(iteration)
-            plt.savefig(filename)
-
-        if self.make_animation and not self.plot_2d:
-            # Make an animated 3d view
-            os.makedirs(self.tmp_animation_save_dir, exist_ok=True)
-            for i, angle in enumerate(range(-100, 0, 2)):
-                self.animate_axes.view_init(30, angle)
-                filename = self.get_tmp_animation_filename(i)
-                plt.savefig(filename)
-            self.compile_animation(i, delete_files=True, duration=0.2)
+        return max_prob, min_prob, params
 
-    def plot_reachable_sets(
-        self,
-        constraint: constraints.MultiTimestepConstraint,
-        dims: list,
-        reachable_set_color: Optional[str] = None,
-        reachable_set_zorder: Optional[int] = None,
-        reachable_set_ls: Optional[str] = None,
-        reachable_set_lw: Optional[int] = None,
+    def setup_LPs_nstep(
+        self, nstep=False, modifier=0, infos=None, bp_sets=None
     ):
-        if reachable_set_color is None:
-            reachable_set_color = "tab:blue"
-        if reachable_set_ls is None:
-            reachable_set_ls = "-"
-        if reachable_set_lw is None:
-            reachable_set_lw = self.linewidth
-        fc_color = "None"
-        constraint.plot(
-            self.animate_axes,
-            dims,
-            reachable_set_color,
-            fc_color=fc_color,
-            zorder=reachable_set_zorder,
-            plot_2d=self.plot_2d,
-            linewidth=reachable_set_lw,
-            ls=reachable_set_ls,
-        )
-
-    def plot_partition(self, constraint, dims, color):
-        # This if shouldn't really be necessary -- someone is calling
-        # self.plot_partitions with something other than a
-        # (constraint, ___) element in M?
-        if isinstance(constraint, np.ndarray):
-            constraint = constraints.LpConstraint(range=constraint)
+        num_states = self.dynamics.At.shape[0]
+        num_control_inputs = self.dynamics.bt.shape[1]
 
-        constraint.plot(
-            self.animate_axes, dims, color, linewidth=1, plot_2d=self.plot_2d
-        )
+        if isinstance(bp_sets[0], constraints.LpConstraint):
+            num_steps = len(bp_sets)
+            xt = cp.Variable((num_states, num_steps + 1))
+            ut = cp.Variable((num_control_inputs, num_steps))
+
+            lower_A_list = [
+                cp.Parameter((num_control_inputs, num_states))
+                for i in range(num_steps)
+            ]
+            upper_A_list = [
+                cp.Parameter((num_control_inputs, num_states))
+                for i in range(num_steps)
+            ]
+            lower_sum_b_list = [
+                cp.Parameter(num_control_inputs) for i in range(num_steps)
+            ]
+            upper_sum_b_list = [
+                cp.Parameter(num_control_inputs) for i in range(num_steps)
+            ]
+
+            xt_min = [cp.Parameter(num_states) for i in range(num_steps + 1)]
+            xt_max = [cp.Parameter(num_states) for i in range(num_steps + 1)]
+
+            A_t = cp.Parameter(num_states)
+
+            params = {
+                "lower_A": lower_A_list,
+                "upper_A": upper_A_list,
+                "lower_sum_b": lower_sum_b_list,
+                "upper_sum_b": upper_sum_b_list,
+                "xt_min": xt_min,
+                "xt_max": xt_max,
+                "A_t": A_t,
+            }
 
-    def plot_partitions(
-        self,
-        M: list[tuple[constraints.SingleTimestepConstraint, np.ndarray]],
-        dims: list,
-    ) -> None:
-        # first = True
-        for input_constraint, output_range in M:
-            # Next state constraint of that cell
-            output_constraint_ = constraints.LpConstraint(range=output_range)
-            self.plot_partition(output_constraint_, dims, "grey")
+            constrs = []
 
-            # Initial state constraint of that cell
-            self.plot_partition(input_constraint, dims, "tab:red")
+            for t in range(num_steps):
+                # Gather CROWN bounds and previous BP bounds
+                if t > 0:
+                    upper_A_list[t].value = infos[-t - modifier]["upper_A"]
+                    lower_A_list[t].value = infos[-t - modifier]["lower_A"]
+                    upper_sum_b_list[t].value = infos[-t - modifier][
+                        "upper_sum_b"
+                    ]
+                    lower_sum_b_list[t].value = infos[-t - modifier][
+                        "lower_sum_b"
+                    ]
+
+                    xt_min[t].value = bp_sets[-t - modifier].range[:, 0]
+                    xt_max[t].value = bp_sets[-t - modifier].range[:, 1]
+
+                # u_t bounded by CROWN bounds
+                constrs += [
+                    lower_A_list[t] @ xt[:, t] + lower_sum_b_list[t]
+                    <= ut[:, t]
+                ]
+                constrs += [
+                    ut[:, t]
+                    <= upper_A_list[t] @ xt[:, t] + upper_sum_b_list[t]
+                ]
 
-    def get_one_step_backreachable_set(
-        self,
-        target_sets: Union[
-            constraints.SingleTimestepConstraint,
-            constraints.MultiTimestepConstraint,
-        ],
-    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
-        # Given a target_set, compute the backreachable_set
-        # that ensures that starting from within the backreachable_set
-        # will lead to a state within the target_set
-        info = {}  # type: dict[str, Any]
-        # if collected_input_constraints is None:
-        #     collected_input_constraints = [input_constraint]
+                # Each xt must fall in the original backprojection
+                constrs += [xt_min[t] <= xt[:, t]]
+                constrs += [xt[:, t] <= xt_max[t]]
+
+                # x_t and x_{t+1} connected through system dynamics
+                constrs += [
+                    self.dynamics.dynamics_step(xt[:, t], ut[:, t])
+                    == xt[:, t + 1]
+                ]
 
-        # Extract elementwise bounds on xt1 from the lp-ball or polytope
-        # constraint
-        A_target, b_target = target_sets.get_constraint_at_time_index(
-            -1
-        ).get_polytope()
+        elif isinstance(bp_sets[0], constraints.RotatedLpConstraint):
+            num_steps = len(bp_sets)
+            xt = cp.Variable((num_states, num_steps + 1))
+            ut = cp.Variable((num_control_inputs, num_steps))
+
+            lower_A_list = [
+                cp.Parameter((num_control_inputs, num_states))
+                for i in range(num_steps)
+            ]
+            upper_A_list = [
+                cp.Parameter((num_control_inputs, num_states))
+                for i in range(num_steps)
+            ]
+            lower_sum_b_list = [
+                cp.Parameter(num_control_inputs) for i in range(num_steps)
+            ]
+            upper_sum_b_list = [
+                cp.Parameter(num_control_inputs) for i in range(num_steps)
+            ]
+
+            xt_min = [cp.Parameter(num_states)]
+            xt_max = [cp.Parameter(num_states)]
+
+            R = [
+                cp.Parameter((num_states, num_states))
+                for i in range(num_steps + 1)
+            ]
+            pose = [cp.Parameter(num_states) for i in range(num_steps + 1)]
+            W = [cp.Parameter(num_states) for i in range(num_steps + 1)]
+
+            A_t = cp.Parameter(num_states)
+
+            params = {
+                "lower_A": lower_A_list,
+                "upper_A": upper_A_list,
+                "lower_sum_b": lower_sum_b_list,
+                "upper_sum_b": upper_sum_b_list,
+                "xt_min": xt_min,
+                "xt_max": xt_max,
+                "A_t": A_t,
+            }
 
-        """
-        Step 1:
-        Find backreachable set: all the xt for which there is
-        some u in U that leads to a state xt1 in output_constraint
-        """
-
-        if self.dynamics.u_limits is None:
-            print(
-                "self.dynamics.u_limits is None ==>                 The"
-                " backreachable set is probably the whole state space.        "
-                "         Giving up."
-            )
-            raise NotImplementedError
-        else:
-            u_min = self.dynamics.u_limits[:, 0]
-            u_max = self.dynamics.u_limits[:, 1]
+            constrs = []
 
-        num_states = self.dynamics.num_states
-        num_control_inputs = self.dynamics.num_inputs
+            constrs += [xt_min[0] <= xt[:, 0]]
+            constrs += [xt[:, 0] <= xt_max[0]]
 
-        xt = cp.Variable(num_states)
-        ut = cp.Variable(num_control_inputs)
+            for t in range(num_steps):
+                # Gather CROWN bounds and previous BP bounds
+                if t > 0:
+                    upper_A_list[t].value = infos[-t - modifier]["upper_A"]
+                    lower_A_list[t].value = infos[-t - modifier]["lower_A"]
+                    upper_sum_b_list[t].value = infos[-t - modifier][
+                        "upper_sum_b"
+                    ]
+                    lower_sum_b_list[t].value = infos[-t - modifier][
+                        "lower_sum_b"
+                    ]
+
+                    theta = bp_sets[-t - modifier].theta
+
+                    R[t].value = np.array(
+                        [
+                            [np.cos(theta), np.sin(theta)],
+                            [-np.sin(theta), np.cos(theta)],
+                        ]
+                    )
+                    W[t].value = bp_sets[-t - modifier].width
+                    pose[t].value = bp_sets[-t - modifier].pose
 
-        # For each dimension of the output constraint (facet/lp-dimension):
-        # compute a bound of the NN output using the pre-computed matrices
-        constrs = []
-        constrs += [u_min <= ut]
-        constrs += [ut <= u_max]
+                    # Each xt must fall in the previously calculated (rotated)
+                    # backprojection
+                    constrs += [R[t] @ xt[:, t] <= W[t] + R[t] @ pose[t]]
+                    constrs += [R[t] @ xt[:, t] >= R[t] @ pose[t]]
+
+                # u_t bounded by CROWN bounds
+                constrs += [
+                    lower_A_list[t] @ xt[:, t] + lower_sum_b_list[t]
+                    <= ut[:, t]
+                ]
+                constrs += [
+                    ut[:, t]
+                    <= upper_A_list[t] @ xt[:, t] + upper_sum_b_list[t]
+                ]
 
-        # Included state limits to reduce size of backreachable sets by
-        # eliminating states that are not physically possible
-        # (e.g., maximum velocities)
-        # if self.dynamics.x_limits is not None:
-        #     x_llim = self.dynamics.x_limits[:, 0]
-        #     x_ulim = self.dynamics.x_limits[:, 1]
-        #     constrs += [x_llim <= xt]
-        #     constrs += [xt <= x_ulim]
-        #     # Also constrain the future state to be within the state limits
-        #     constrs += [self.dynamics.dynamics_step(xt,ut) <= x_ulim]
-        #     constrs += [self.dynamics.dynamics_step(xt,ut) >= x_llim]
-
-        # if self.dynamics.x_limits is not None:
-        #     for state in self.dynamics.x_limits:
-        #         constrs += [self.dynamics.x_limits[state][0] <= xt[state]]
-        #         constrs += [xt[state] <= self.dynamics.x_limits[state][1]]
+                # x_t and x_{t+1} connected through system dynamics
+                constrs += [
+                    self.dynamics.dynamics_step(xt[:, t], ut[:, t])
+                    == xt[:, t + 1]
+                ]
+        obj = A_t @ xt[:, 0]
+        min_prob = cp.Problem(cp.Minimize(obj), constrs)
+        max_prob = cp.Problem(cp.Maximize(obj), constrs)
 
-        constrs += [A_target @ self.dynamics.dynamics_step(xt, ut) <= b_target]
+        return max_prob, min_prob, params
 
-        b, status = optimize_over_all_states(xt, constrs)
-        ranges = np.vstack([-b[num_states:], b[:num_states]]).T
 
-        backreachable_set = constraints.LpConstraint(range=ranges)
-        info["backreachable_set"] = backreachable_set
-        info["target_sets"] = target_sets
+class ClosedLoopIBPPropagator(ClosedLoopCROWNIBPCodebasePropagator):
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        raise NotImplementedError
+        # TODO: Write nn_bounds.py:BoundClosedLoopController:interval_range
+        # (using bound_layers.py:BoundSequential:interval_range)
+        self.method_opt = "interval_range"
+        self.params = {}
 
-        return backreachable_set, info
 
-    def get_one_step_backprojection_set(
-        self,
-        target_sets: constraints.MultiTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-        overapprox: bool = False,
-    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
-        backreachable_set, info = self.get_one_step_backreachable_set(
-            target_sets
-        )
-        info["backreachable_set"] = backreachable_set
+class ClosedLoopCROWNPropagator(ClosedLoopCROWNIBPCodebasePropagator):
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.method_opt = "full_backward_range"
+        # self.params = {"same-slope": False, "zero-lb": True}
+        self.params = {"same-slope": False}
 
-        backprojection_set, _ = propagator.get_one_step_backprojection_set(
-            backreachable_set,
-            target_sets,
-            overapprox=overapprox,
-        )
 
-        # if overapprox:
-        #     # These will be used to further backproject this set in time
-        #     backprojection_set.crown_matrices = get_crown_matrices(
-        #         propagator,
-        #         backprojection_set,
-        #         self.dynamics.num_inputs,
-        #         self.dynamics.sensor_noise
-        #     )
+class ClosedLoopCROWNLPPropagator(ClosedLoopCROWNPropagator):
+    # Same as ClosedLoopCROWNPropagator but don't allow the
+    # use of closed-form soln to the optimization, even if it's possible
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.params["try_to_use_closed_form"] = False
 
-        return backprojection_set, info
 
-    """
-    Inputs:
-    - target_set: describes goal/avoid set at t=t_max
-    - propagator:
-    - t_max: how many timesteps to backproject
-    - num_partitions: number of splits per dimension in each backreachable set
-    - overapprox: bool
-        True = compute outer bounds of BP sets (for collision avoidance)
-        False = computer inner bounds of BP sets (for goal arrival)
-
-    Returns:
-    - backprojection_sets: [BP_{-1}, ..., BP_{-t_max}]
-          i.e., [ set of states that will get to goal/avoid set in 1 step,
-                  ...,
-                  set of states that will get to goal/avoid set in t_max steps
-                ]
-    - info: TODO
-    """
+class ClosedLoopFastLinPropagator(ClosedLoopCROWNIBPCodebasePropagator):
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.method_opt = "full_backward_range"
+        self.params = {"same-slope": True}
 
-    def get_backprojection_set(
-        self,
-        target_set: constraints.SingleTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-        t_max: int,
-        overapprox: bool = False,
+
+class ClosedLoopCROWNNStepPropagator(ClosedLoopCROWNPropagator):
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+
+    def get_reachable_set(
+        self, initial_set: constraints.SingleTimestepConstraint, t_max: int
     ) -> tuple[constraints.MultiTimestepConstraint, dict]:
-        # Initialize data structures to hold results
-        backprojection_sets = (
-            constraints.create_empty_multi_timestep_constraint(
-                propagator.boundary_type
+        # initial_set: constraint.LpConstraint(range=(num_states, 2))
+        # reachable_sets: constraint.LpConstraint(
+        #   range=(num_timesteps, num_states, 2))
+        reachable_sets, infos = super().get_reachable_set(initial_set, t_max)
+
+        # "undo" packaging of reachable_sets to simply get a list of the ranges
+        reachable_sets_list = [
+            constraints.LpConstraint(range=r) for r in reachable_sets.range
+        ]
+
+        # Symbolically refine all N steps
+        tightened_reachable_sets = (
+            []
+        )  # type: list[constraints.SingleTimestepConstraint]
+        tightened_infos = deepcopy(infos)
+        N = len(reachable_sets_list)
+        for t in range(2, N + 1):
+            # N-step analysis accepts as input:
+            # [1st output constraint, {2,...,t} tightened output constraints,
+            #  dummy output constraint]
+            reachable_set, info = self.get_N_step_reachable_set(
+                initial_set,
+                reachable_sets_list[:1]
+                + tightened_reachable_sets
+                + reachable_sets_list[:1],
+                infos["per_timestep"][:t],
             )
-        )
-        info = {"per_timestep": []}  # type: dict[str, Any]
+            tightened_reachable_sets.append(reachable_set)
+            tightened_infos["per_timestep"][t - 1] = info
 
-        # Run one step of backprojection analysis
-        backprojection_set_this_timestep, info_this_timestep = (
-            self.get_one_step_backprojection_set(
-                target_set.to_multistep_constraint(),
-                propagator,
-                overapprox=overapprox,
-            )
+        tightened_reachable_sets_list = (
+            reachable_sets_list[:1] + tightened_reachable_sets
         )
-
-        # Store that step's results
-        backprojection_sets = backprojection_sets.add_timestep_constraint(
-            backprojection_set_this_timestep
+        reachable_sets = constraints.list_to_constraint(
+            tightened_reachable_sets_list
         )
-        info["per_timestep"].append(info_this_timestep)
 
-        if overapprox:
-            for i in np.arange(
-                0 + propagator.dynamics.dt + 1e-10,
-                t_max,
-                propagator.dynamics.dt,
-            ):
-                # Run one step of backprojection analysis
-                backprojection_set_this_timestep, info_this_timestep = (
-                    self.get_one_step_backprojection_set(
-                        target_set.add_timestep_constraint(
-                            backprojection_sets
-                        ),
-                        propagator,
-                        overapprox=overapprox,
-                    )
-                )
-                backprojection_sets = (
-                    backprojection_sets.add_timestep_constraint(
-                        backprojection_set_this_timestep
-                    )
-                )
-                info["per_timestep"].append(info_this_timestep)
-        else:
-            for i in np.arange(
-                0 + propagator.dynamics.dt + 1e-10,
-                t_max,
-                propagator.dynamics.dt,
-            ):
-                # TODO: Support N-step backprojection in the
-                # under-approximation case
-                raise NotImplementedError
+        # Do N-step "symbolic" refinement
+        # reachable_set, new_infos = self.get_N_step_reachable_set(
+        #     input_constraint, reachable_sets, infos['per_timestep']
+        # )
+        # reachable_sets[-1] = reachable_set
+        # tightened_infos = infos  # TODO: fix this...
 
-        return backprojection_sets, info
+        return reachable_sets, tightened_infos
 
-    def get_backprojection_error(
+    def get_one_step_backprojection_set_underapprox(self):
+        raise NotImplementedError
+
+    def improve_one_step_backprojection_set_overapprox(
         self,
-        target_set: constraints.SingleTimestepConstraint,
-        backprojection_sets: constraints.MultiTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-        t_max: int,
-    ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
-        # Note: This almost certainly got messed up in the merge (3/24/23)
-
-        errors = []
-
-        true_verts_reversed = self.dynamics.get_true_backprojection_set(
-            backprojection_sets.get_constraint_at_time_index(-1),
-            target_set,
-            t_max,
-            controller=propagator.network,
-        )
-        true_verts = np.flip(true_verts_reversed, axis=1)
-        num_steps = backprojection_sets.get_t_max()
+        backreachable_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+        facet_inds_to_optimize: Optional[np.ndarray] = None,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
+        # The only difference between this and
+        # CROWNPropagator.improve_one_step_backprojection_set_overapprox
+        # should be that here, we enforce that xt needs to pass through *all*
+        # the target_sets, whereas in
+        # the latter, we only enforce that xt needs to pass through
+        # target_sets[-1] (the final target set).
+
+        # An over-approximation of the backprojection set is the set of:
+        # all x_t s.t. there exists some u \in [pi^L(x_t), pi^U(x_t)]
+        #              that leads to the target set
 
-        for t in range(num_steps):
-            x_min = np.min(true_verts[:, t + 1, :], axis=0)
-            x_max = np.max(true_verts[:, t + 1, :], axis=0)
+        num_states, num_control_inputs = self.dynamics.bt.shape
+        num_steps = target_sets.get_t_max()
 
-        if isinstance(target_set, constraints.LpConstraint):
-            Ats, bts = range_to_polytope(target_set.range)
-            true_verts_reversed = self.dynamics.get_true_backprojection_set(
-                backprojection_sets[-1],
-                target_set,
-                t_max,
-                controller=propagator.network,
-                num_samples=1e8,
-            )
-            true_verts = np.flip(true_verts_reversed, axis=1)
-            num_steps = len(backprojection_sets)
-
-            x_range = x_max - x_min
-            true_area = np.prod(x_range)
-
-            estimated_area = backprojection_sets.get_constraint_at_time_index(
-                t
-            ).get_area()
-
-            # true_hull = ConvexHull(true_verts[:, t+1, :])
-            # true_area = true_hull.volume
-
-            Abp, bbp = range_to_polytope(backprojection_sets[t].range)
-            estimated_verts = pypoman.polygon.compute_polygon_hull(Abp, bbp)
-            estimated_hull = ConvexHull(estimated_verts)
-            estimated_area = estimated_hull.volume
-
-            # print(f"estimated: estimated_area --- true: {true_area}")
-            # print(
-            #     "estimated range: {} --- true range: {}".format(
-            #         backprojection_sets[t].range, x_range
-            #     )
-            # )
-
-            errors.append((estimated_area - true_area) / true_area)
-        elif isinstance(target_set, constraints.RotatedLpConstraint):
-            true_verts_reversed = self.dynamics.get_true_backprojection_set(
-                # backreachable_sets[-1],
-                target_set,
-                t_max,
-                controller=propagator.network,
-                num_samples=1e8,
-            )
-            true_verts = np.flip(true_verts_reversed, axis=1)
-            num_steps = len(backprojection_sets)
-
-            for t in range(num_steps):
-                # x_min = np.min(true_verts[:,t+1,:], axis=0)
-                # x_max = np.max(true_verts[:,t+1,:], axis=0)
+        xt = cp.Variable((num_states, num_steps + 1))
+        ut = cp.Variable((num_control_inputs, num_steps))
+        constrs = []
 
-                # x_range = x_max-x_min
-                # true_area = np.prod(x_range)
-                true_hull = ConvexHull(true_verts[:, t + 1, :])
-                true_area = true_hull.volume
-
-                # true_hull = ConvexHull(true_verts[:, t+1, :])
-                # true_area = true_hull.volume
-
-                # Abp, bbp = range_to_polytope(backprojection_sets[t].range)
-                # estimated_verts = (
-                #   pypoman.polygon.compute_polygon_hull(Abp, bbp)
-                # )
-                estimated_hull = ConvexHull(backprojection_sets[t].vertices)
-                estimated_area = estimated_hull.volume
-
-                # print(
-                #     "estimated: {} --- true: {}".format(
-                #         estimated_area, true_area
-                #     )
-                # )
-                # print(
-                #     "estimated range: {} --- true range: {}".format(
-                #         backprojection_sets[t].range, x_range
-                #     )
-                # )
+        # Constraints to ensure that xt stays within the backreachable set
+        A_backreach, b_backreach = backreachable_set.get_polytope()
+        constrs += [A_backreach @ xt[:, 0] <= b_backreach]
 
-                errors.append((estimated_area - true_area) / true_area)
-        else:
-            # This implementation should actually be moved to Lp constraint
+        # Each ut must not exceed CROWN bounds
+        for t in range(num_steps):
+            if t == 0:
+                set_t = backreachable_set
+            else:
+                set_t = target_sets.get_constraint_at_time_index(-t)
+
+            # if set_t.crown_matrices is None:
+            # TODO: these matrices have probably been computed already
+            # elsewhere, grab those instead of re-calculating
+            set_t.crown_matrices = get_crown_matrices(
+                self,
+                set_t,
+                self.dynamics.num_inputs,
+                self.dynamics.sensor_noise,
+            )
+            assert (
+                set_t.crown_matrices is not None
+            ), "Need to set set_t.crown_matrices."
+            constrs += [
+                deepcopy(set_t.crown_matrices.lower_A_numpy) @ xt[:, t]
+                + deepcopy(set_t.crown_matrices.lower_sum_b_numpy)
+                <= ut[:, t]
+            ]
+            constrs += [
+                ut[:, t]
+                <= deepcopy(set_t.crown_matrices.upper_A_numpy) @ xt[:, t]
+                + deepcopy(set_t.crown_matrices.upper_sum_b_numpy)
+            ]
 
-            # Note: This compares the estimated polytope
-            # with the "best" polytope with those facets.
-            # There could be a much better polytope with lots of facets.
-            true_verts_reversed = self.dynamics.get_true_backprojection_set(
-                backprojection_sets[-1],
-                target_set,
-                t_max,
-                controller=propagator.network,
-            )
-            true_verts = np.flip(true_verts_reversed, axis=1)
-            num_steps = len(backprojection_sets)
+            constrs += [ut[:, t] >= self.dynamics.u_limits[:, 0]]
+            constrs += [ut[:, t] <= self.dynamics.u_limits[:, 1]]
 
-            for t in range(num_steps):
-                x_min = np.min(true_verts[:, t + 1, :], axis=0)
-                x_max = np.max(true_verts[:, t + 1, :], axis=0)
+        # x_t and x_{t+1} connected through system dynamics
+        for t in range(num_steps):
+            constrs += [
+                self.dynamics.dynamics_step(xt[:, t], ut[:, t]) == xt[:, t + 1]
+            ]
 
-                x_range = x_max - x_min
-                true_area = np.prod(x_range)
+        # ensure xt reaches the "target set" at each timestep
+        for t in range(num_steps):
+            A_set_t, b_target = target_sets.get_constraint_at_time_index(
+                -t - 1
+            ).get_polytope()
+            constrs += [A_set_t @ xt[:, t + 1] <= b_target]
 
-                estimated_verts = pypoman.polygon.compute_polygon_hull(
-                    backprojection_sets[t].A[0], backprojection_sets[t].b[0]
-                )
-                estimated_hull = ConvexHull(estimated_verts)
-                estimated_area = estimated_hull.volume
+        b, status = optimize_over_all_states(
+            xt[:, 0], constrs, facet_inds_to_optimize=facet_inds_to_optimize
+        )
 
-                errors.append((estimated_area - true_area) / true_area)
+        backprojection_set = optimization_results_to_backprojection_set(
+            status, b, backreachable_set
+        )
 
-        final_error = errors[-1]
-        avg_error = np.mean(errors)
-        return final_error, avg_error, np.array(errors)
+        return backprojection_set
 
-    def get_N_step_backprojection_set(
+    def get_N_step_reachable_set(
         self,
-        output_constraint,
-        input_constraint,
-        propagator,
-        t_max,
-        num_partitions=None,
-        overapprox=False,
-        heuristic="guided",
-        all_lps=False,
-        slow_cvxpy=False,
+        initial_set,
+        reachable_sets,
+        infos,
     ):
-        input_constraint_, info = propagator.get_N_step_backprojection_set(
-            output_constraint,
-            deepcopy(input_constraint),
-            t_max,
-            num_partitions=num_partitions,
-            overapprox=overapprox,
-            heuristic=heuristic,
-            all_lps=all_lps,
-            slow_cvxpy=slow_cvxpy,
-        )
-        input_constraint = input_constraint_.copy()
+        # TODO: Get this to work for Polytopes too
+        # TODO: Confirm this works with partitioners
+        # TODO: pull the cvxpy out of this function
+        # TODO: add back in noise, observation model
+
+        A_out = np.eye(self.dynamics.At.shape[0])
+        num_facets = A_out.shape[0]
+        ranges = np.zeros((num_facets, 2))
+        num_steps = len(reachable_sets)
+
+        # Because there might sensor noise, the NN could see a different set of
+        # states than the system is actually in
+        x_min = reachable_sets[-2].range[..., 0]
+        x_max = reachable_sets[-2].range[..., 1]
+        norm = reachable_sets[-2].p
+        prev_state_max = torch.Tensor(np.array([x_max]))
+        prev_state_min = torch.Tensor(np.array([x_min]))
+        nn_input_max = prev_state_max
+        nn_input_min = prev_state_min
+        if self.dynamics.sensor_noise is not None:
+            nn_input_max += torch.Tensor(
+                np.array([self.dynamics.sensor_noise[:, 1]])
+            )
+            nn_input_min += torch.Tensor(
+                np.array([self.dynamics.sensor_noise[:, 0]])
+            )
+
+        # Compute the NN output matrices (for the input constraints)
+        num_control_inputs = self.dynamics.bt.shape[1]
+        C = torch.eye(num_control_inputs).unsqueeze(0)
+        lower_A, upper_A, lower_sum_b, upper_sum_b = self.network(
+            method_opt=self.method_opt,
+            norm=norm,
+            x_U=nn_input_max,
+            x_L=nn_input_min,
+            upper=True,
+            lower=True,
+            C=C,
+            return_matrices=True,
+        )
+        infos[-1]["nn_matrices"] = {
+            "lower_A": lower_A.data.numpy()[0],
+            "upper_A": upper_A.data.numpy()[0],
+            "lower_sum_b": lower_sum_b.data.numpy()[0],
+            "upper_sum_b": upper_sum_b.data.numpy()[0],
+        }
+
+        num_states = self.dynamics.bt.shape[0]
+        xs = []
+        for t in range(num_steps + 1):
+            xs.append(cp.Variable(num_states))
+
+        constraints = []
+
+        # xt \in Xt
+        constraints += [
+            xs[0] <= initial_set.range[..., 1],
+            xs[0] >= initial_set.range[..., 0],
+        ]
+
+        # xt+1 \in our one-step overbound on Xt+1
+        for t in range(num_steps - 1):
+            constraints += [
+                xs[t + 1] <= reachable_sets[t].range[..., 1],
+                xs[t + 1] >= reachable_sets[t].range[..., 0],
+            ]
 
-        return input_constraint, info
+        # xt1 connected to xt via dynamics
+        for t in range(num_steps):
+            # Don't need to consider each state individually if we have Bt >= 0
+
+            # upper_A = infos[t]['nn_matrices']['upper_A']
+            # lower_A = infos[t]['nn_matrices']['lower_A']
+            # upper_sum_b = infos[t]['nn_matrices']['upper_sum_b']
+            # lower_sum_b = infos[t]['nn_matrices']['lower_sum_b']
+
+            # if self.dynamics.continuous_time:
+            #     constraints += [
+            #         xs[t+1] <= xs[t] + self.dynamics.dt *
+            #           (self.dynamics.At@xs[t]+self.dynamics.bt@(
+            #               upper_A@xs[t]+upper_sum_b)+self.dynamics.ct),
+            #         xs[t+1] >= xs[t] + self.dynamics.dt *
+            #           (self.dynamics.At@xs[t]+self.dynamics.bt@(
+            #               lower_A@xs[t]+lower_sum_b)+self.dynamics.ct),
+            #     ]
+            # else:
+            #     constraints += [
+            #         xs[t+1] <= self.dynamics.At@xs[t]+self.dynamics.bt@(
+            #           upper_A@xs[t]+upper_sum_b)+self.dynamics.ct,
+            #         xs[t+1] >= self.dynamics.At@xs[t]+self.dynamics.bt@(
+            #           lower_A@xs[t]+lower_sum_b)+self.dynamics.ct,
+            #     ]
+
+            # Handle case of Bt ! >= 0 by adding a constraint per state
+            for j in range(num_states):
+                upper_A = np.where(
+                    np.tile(self.dynamics.bt[j, :], (num_states, 1)).T >= 0,
+                    infos[t]["nn_matrices"]["upper_A"],
+                    infos[t]["nn_matrices"]["lower_A"],
+                )
+                lower_A = np.where(
+                    np.tile(self.dynamics.bt[j, :], (num_states, 1)).T >= 0,
+                    infos[t]["nn_matrices"]["lower_A"],
+                    infos[t]["nn_matrices"]["upper_A"],
+                )
+                upper_sum_b = np.where(
+                    self.dynamics.bt[j, :] >= 0,
+                    infos[t]["nn_matrices"]["upper_sum_b"],
+                    infos[t]["nn_matrices"]["lower_sum_b"],
+                )
+                lower_sum_b = np.where(
+                    self.dynamics.bt[j, :] >= 0,
+                    infos[t]["nn_matrices"]["lower_sum_b"],
+                    infos[t]["nn_matrices"]["upper_sum_b"],
+                )
+
+                if self.dynamics.continuous_time:
+                    constraints += [
+                        xs[t + 1][j]
+                        <= xs[t][j]
+                        + self.dynamics.dt
+                        * (
+                            self.dynamics.At[j, :] @ xs[t]
+                            + self.dynamics.bt[j, :]
+                            @ (upper_A @ xs[t] + upper_sum_b)
+                            + self.dynamics.ct[j]
+                        ),
+                        xs[t + 1][j]
+                        >= xs[t][j]
+                        + self.dynamics.dt
+                        * (
+                            self.dynamics.At[j, :] @ xs[t]
+                            + self.dynamics.bt[j, :]
+                            @ (lower_A @ xs[t] + lower_sum_b)
+                            + self.dynamics.ct[j]
+                        ),
+                    ]
+                else:
+                    constraints += [
+                        xs[t + 1][j]
+                        <= self.dynamics.At[j, :] @ xs[t]
+                        + self.dynamics.bt[j, :]
+                        @ (upper_A @ xs[t] + upper_sum_b)
+                        + self.dynamics.ct[j],
+                        xs[t + 1][j]
+                        >= self.dynamics.At[j, :] @ xs[t]
+                        + self.dynamics.bt[j, :]
+                        @ (lower_A @ xs[t] + lower_sum_b)
+                        + self.dynamics.ct[j],
+                    ]
+
+        A_out_facet = cp.Parameter(num_states)
+
+        obj = cp.Maximize(A_out_facet @ xs[-1])
+        prob_max = cp.Problem(obj, constraints)
+
+        obj = cp.Minimize(A_out_facet @ xs[-1])
+        prob_min = cp.Problem(obj, constraints)
+
+        for i in range(num_facets):
+            A_out_facet.value = A_out[i, :]
+
+            prob_max.solve()
+            A_out_xtN_max = prob_max.value
+
+            prob_min.solve()
+            A_out_xtN_min = prob_min.value
+
+            ranges[i, 0] = A_out_xtN_min
+            ranges[i, 1] = A_out_xtN_max
+
+        reachable_set = deepcopy(reachable_sets[-1])
+        reachable_set.range = ranges
+        return reachable_set, infos
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopSimGuidedPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopSimGuidedPartitioner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from itertools import product
-from typing import Union
+from typing import Any, Optional, Union
 
 import numpy as np
 
 import nfl_veripy.constraints as constraints
 import nfl_veripy.dynamics as dynamics
 import nfl_veripy.propagators as propagators
 from nfl_veripy.utils.utils import get_crown_matrices, sect
@@ -12,39 +12,24 @@
 from .ClosedLoopPartitioner import ClosedLoopPartitioner
 
 
 class ClosedLoopSimGuidedPartitioner(ClosedLoopPartitioner):
     def __init__(
         self,
         dynamics: dynamics.Dynamics,
-        num_partitions: Union[None, int, np.ndarray] = 16,
-        make_animation: bool = False,
-        show_animation: bool = False,
     ):
-        ClosedLoopPartitioner.__init__(
-            self,
-            dynamics=dynamics,
-            make_animation=make_animation,
-            show_animation=show_animation,
-        )
-        self.num_partitions = num_partitions
-        self.interior_condition = "linf"
-
-        self.termination_condition_type = "num_propagator_calls"
-        self.termination_condition_value = 200
+        super().__init__(dynamics=dynamics)
+        self.interior_condition: str = "linf"
 
-        self.reachable_set_color = "tab:blue"
-        self.reachable_set_zorder = 2
-        self.initial_set_color = "tab:red"
-        self.initial_set_zorder = 2
-        self.sample_zorder = 1
+        self.termination_condition_type: str = "num_propagator_calls"
+        self.termination_condition_value: int = 200
 
     def check_termination(  # type: ignore
         self,
-        num_propagator_calls: int,
+        num_propagator_calls: float,
     ) -> bool:
         if self.termination_condition_type == "num_propagator_calls":
             terminate = (
                 num_propagator_calls >= self.termination_condition_value
             )
         else:
             raise NotImplementedError
@@ -56,27 +41,26 @@
         propagator: propagators.ClosedLoopPropagator,
         num_partitions: Union[None, int, list, np.ndarray] = None,
     ) -> tuple[constraints.SingleTimestepConstraint, dict]:
         reachable_set, info = self.get_reachable_set(
             initial_set,
             propagator,
             t_max=1,
-            num_partitions=num_partitions,
         )
-        return reachable_set, info
+        return reachable_set.get_constraint_at_time_index(0), info
 
     def get_reachable_set(
         self,
         initial_set: constraints.SingleTimestepConstraint,
         propagator: propagators.ClosedLoopPropagator,
         t_max: int,
         num_partitions: Union[None, int, list, np.ndarray] = None,
     ) -> tuple[constraints.MultiTimestepConstraint, dict]:
         t_start_overall = time.time()
-        info = {}
+        info = {}  # type: dict[str, Any]
         propagator_computation_time = 0.0
 
         # Algorithm 1 of (Xiang, 2020): https://arxiv.org/pdf/2004.12273.pdf
         sect_method = "max"
 
         num_propagator_calls = 0
         interior_M = (
@@ -97,51 +81,41 @@
         reachable_sets, info = propagator.get_reachable_set(initial_set, t_max)
         t_end = time.time()
         propagator_computation_time += t_end - t_start
         num_propagator_calls += t_max
 
         M = [(initial_set, reachable_sets)]  # (Line 4)
 
-        if self.make_animation:
-            self.setup_visualization(
-                initial_set,
-                reachable_sets,
-                propagator,
-                show_samples=True,
-                inputs_to_highlight=[
-                    {"dim": [0], "name": "$x_0$"},
-                    {"dim": [1], "name": "$x_1$"},
-                ],
-                aspect="auto",
-                initial_set_color=self.initial_set_color,
-                initial_set_zorder=self.initial_set_zorder,
-                sample_zorder=self.sample_zorder,
-            )
-
         reachable_sets_range, info = self.partition_loop(
             M,
             interior_M,
             reachable_sets_range_sim,
             sect_method,
             num_propagator_calls,
             initial_set,
             reachable_sets.range,
             propagator,
             propagator_computation_time,
             t_start_overall,
             t_max,
+            info,
         )
 
         # info["all_partitions"] = ranges
         info["num_propagator_calls"] = num_propagator_calls
 
-        reachable_sets = constraints.MultiTimestepLpConstraint(
-            range=reachable_sets_range
+        reachable_sets = constraints.MultiTimestepConstraint(
+            constraints=[
+                constraints.LpConstraint(range=r) for r in reachable_sets_range
+            ]
         )
 
+        # store the cells in the constraints - only for plotting
+        reachable_sets.cells = [x[1] for x in M + interior_M]
+
         return reachable_sets, info
 
     def partition_loop(
         self,
         M: list[
             tuple[
                 constraints.SingleTimestepConstraint,
@@ -152,30 +126,30 @@
             tuple[
                 constraints.SingleTimestepConstraint,
                 constraints.MultiTimestepConstraint,
             ]
         ],
         reachable_set_range_sim,
         sect_method: str,
-        num_propagator_calls: int,
+        num_propagator_calls: float,
         initial_set: constraints.SingleTimestepConstraint,
         u_e,
         propagator: propagators.ClosedLoopPropagator,
         propagator_computation_time: float,
         t_start_overall: float,
-        t_max: float,
+        t_max: int,
+        info: dict,
     ) -> tuple[np.ndarray, dict]:
-        if self.make_animation:
-            self.call_visualizer(
-                reachable_set_range_sim,
-                M + interior_M,
-                num_propagator_calls,
-                interior_M,
-                iteration=-1,
-            )
+        # Store these items at each iteration for eventual visualization
+        info["iterations"] = {}
+        info["iterations"][-1] = {
+            "M": M,
+            "interior_M": interior_M,
+            "num_propagator_calls": num_propagator_calls,
+        }
 
         # Used by UnGuided, SimGuided, GreedySimGuided, etc.
         iteration = 0
         terminate = False
         while len(M) != 0 and not terminate:
             initial_set_this_cell, reachable_set_this_cell = self.grab_from_M(
                 M, reachable_set_range_sim
@@ -202,15 +176,15 @@
                         t_start = time.time()
 
                         initial_set_this_sected_cell = (
                             constraints.LpConstraint(
                                 range=sected_initial_set_range
                             )
                         )
-                        reachable_set_this_sected_cell, info = (
+                        reachable_set_this_sected_cell, this_info = (
                             propagator.get_reachable_set(
                                 initial_set_this_sected_cell, t_max
                             )
                         )
                         t_end = time.time()
                         propagator_computation_time += t_end - t_start
                         num_propagator_calls += t_max
@@ -221,96 +195,61 @@
                                 reachable_set_this_sected_cell,
                             )
                         )  # Line 18
 
                 else:  # Lines 19-20
                     M.append((initial_set_this_cell, reachable_set_this_cell))
 
-                if self.make_animation:
-                    self.call_visualizer(
-                        reachable_set_range_sim,
-                        M + interior_M,
-                        num_propagator_calls,
-                        interior_M,
-                        iteration=iteration,
-                        dont_tighten_layout=False,
-                    )
+                info["iterations"][iteration] = {
+                    "M": M,
+                    "interior_M": interior_M,
+                    "num_propagator_calls": num_propagator_calls,
+                }
             iteration += 1
 
         # Line 24
         u_e = self.squash_down_to_one_range(
             reachable_set_range_sim, M + interior_M
         )
         # u_e = self.squash_down_to_one_range(reachable_set_range_sim, M)
 
         ranges = []
         for m in M + interior_M:
             ranges.append((m[0].range, m[1].range))
         info["all_partitions"] = ranges
 
-        # Stats & Visualization
-        # info = self.compile_info(
-        #     reachable_set_range_sim,
-        #     M,
-        #     interior_M,
-        #     num_propagator_calls,
-        #     t_end_overall,
-        #     t_start_overall,
-        #     propagator_computation_time,
-        #     iteration,
-        # )
-        if self.make_animation:
-            self.compile_animation(
-                iteration, delete_files=False, start_iteration=-1
-            )
-
         return u_e, info
 
-    def call_visualizer(
-        self,
-        output_range_sim,
-        M,
-        num_propagator_calls,
-        interior_M,
-        iteration,
-        dont_tighten_layout=False,
-    ):
-        u_e = self.squash_down_to_one_range(output_range_sim, M)
-        # title = "# Partitions: {}, Error: {}".format(
-        #     str(len(M) + len(interior_M)), str(round(error, 3))
-        # )
-        title = "# Propagator Calls: {}".format(str(int(num_propagator_calls)))
-        # title = None
-
-        output_constraint = constraints.LpConstraint(range=u_e)
-        self.visualize(
-            M,
-            interior_M,
-            output_constraint,
-            iteration=iteration,
-            title=title,
-            reachable_set_color=self.reachable_set_color,
-            reachable_set_zorder=self.reachable_set_zorder,
-            dont_tighten_layout=dont_tighten_layout,
-        )
-
     def squash_down_to_one_range(self, output_range_sim, M):
         # (len(M)+1, t_max, n_states, 2)
         tmp = np.vstack(
             [
                 np.array([m[1].range for m in M]),
                 np.expand_dims(output_range_sim, axis=0),
             ]
         )
         mins = np.min(tmp[..., 0], axis=0)
         maxs = np.max(tmp[..., 1], axis=0)
         return np.stack([mins, maxs], axis=2)
 
-    def grab_from_M(self, M, output_range_sim=None):
-        return M.pop(0)
+    def grab_from_M(
+        self,
+        M: list[
+            tuple[
+                constraints.SingleTimestepConstraint,
+                constraints.MultiTimestepConstraint,
+            ]
+        ],
+        output_range_sim: Optional[np.ndarray],
+    ) -> tuple[
+        constraints.SingleTimestepConstraint,
+        constraints.MultiTimestepConstraint,
+    ]:
+        input_range, output_range = M.pop(0)
+        return input_range, output_range
 
     def check_if_partition_within_sim_bnds(
         self, reachable_set, reachable_set_range_sim
     ):
         reachable_set_range = reachable_set.range
 
         # Check if reachable_set_range's linf ball is within
@@ -323,14 +262,16 @@
             >= 0
         )
         return inside
 
     def get_one_step_backprojection_set(
         self, target_sets, propagator, num_partitions=None, overapprox=False
     ):
+        # Currently this seems to just copy-paste the uniform partitioning code
+        raise NotImplementedError
         backreachable_set, info = self.get_one_step_backreachable_set(
             target_sets[-1]
         )
         info["backreachable_set"] = backreachable_set
 
         if overapprox:
             # Set an empty Constraint that will get filled in
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopUnGuidedPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/ClosedLoopUnGuidedPartitioner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 import numpy as np
 
+import nfl_veripy.dynamics as dynamics
+
 from .ClosedLoopSimGuidedPartitioner import ClosedLoopSimGuidedPartitioner
 
 
 class ClosedLoopUnGuidedPartitioner(ClosedLoopSimGuidedPartitioner):
     def __init__(
         self,
-        dynamics,
-        num_partitions=16,
-        make_animation=False,
-        show_animation=False,
+        dynamics: dynamics.Dynamics,
     ):
-        ClosedLoopSimGuidedPartitioner.__init__(
-            self,
-            dynamics=dynamics,
-            make_animation=make_animation,
-            show_animation=show_animation,
-        )
+        super().__init__(dynamics=dynamics)
 
     def check_if_partition_within_sim_bnds(
         self, output_range, output_range_sim
-    ):
+    ) -> bool:
         return False
 
     def get_sampled_out_range_guidance(
         self, input_constraint, propagator, t_max=5, num_samples=1000
     ):
         return None
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopUniformPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/analyzers/ClosedLoopBackwardAnalyzer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,172 +1,156 @@
-import ast
-from itertools import product
-from typing import Optional, Union
+from typing import Any
 
+import numpy as np
+import torch
+
+import nfl_veripy.analyzers as analyzers
 import nfl_veripy.constraints as constraints
 import nfl_veripy.dynamics as dynamics
+import nfl_veripy.partitioners as partitioners
 import nfl_veripy.propagators as propagators
-import numpy as np
-from nfl_veripy.utils.utils import get_crown_matrices
+import nfl_veripy.visualizers as visualizers
+from nfl_veripy.utils.utils import get_sampled_outputs, samples_to_range
 
-from .ClosedLoopPartitioner import ClosedLoopPartitioner
+from .Analyzer import Analyzer
 
 
-class ClosedLoopUniformPartitioner(ClosedLoopPartitioner):
+class ClosedLoopBackwardAnalyzer(Analyzer):
     def __init__(
-        self,
-        dynamics: dynamics.Dynamics,
-        num_partitions: Union[None, int, np.ndarray] = 16,
-        make_animation: bool = False,
-        show_animation: bool = False,
+        self, torch_model: torch.nn.Sequential, dynamics: dynamics.Dynamics
     ):
-        ClosedLoopPartitioner.__init__(
-            self,
-            dynamics=dynamics,
-            make_animation=make_animation,
-            show_animation=show_animation,
-        )
-        self.num_partitions = np.array(ast.literal_eval(num_partitions))
-        self.interior_condition = "linf"
-        self.show_animation = False
-        self.make_animation = False
+        self.torch_model = torch_model
+        self.dynamics = dynamics
+        analyzers.Analyzer.__init__(self, torch_model=torch_model)
+
+    @property
+    def partitioner_dict(self):
+        return partitioners.partitioner_dict
+
+    @property
+    def propagator_dict(self):
+        return propagators.propagator_dict
+
+    def instantiate_partitioner(
+        self, partitioner_name: str, hyperparams: dict[str, Any]
+    ) -> partitioners.ClosedLoopPartitioner:
+        partitioner = partitioners.partitioner_dict[partitioner_name](
+            self.dynamics
+        )
+        for key, value in hyperparams.items():
+            if hasattr(partitioner, key):
+                setattr(partitioner, key, value)
+        return partitioner
+
+    def instantiate_propagator(
+        self, propagator_name: str, hyperparams: dict[str, Any]
+    ) -> propagators.ClosedLoopPropagator:
+        propagator = propagators.propagator_dict[propagator_name](
+            self.dynamics
+        )
+        for key, value in hyperparams.items():
+            if hasattr(propagator, key):
+                setattr(propagator, key, value)
+        return propagator
+
+    def instantiate_visualizer(
+        self, visualizer_name: str, hyperparams: dict[str, Any]
+    ) -> visualizers.BackwardVisualizer:
+        visualizer = visualizers.BackwardVisualizer(self.dynamics)
+        for key, value in hyperparams.items():
+            if hasattr(visualizer, key):
+                setattr(visualizer, key, value)
+        return visualizer
 
-    def get_one_step_reachable_set(
+    def get_one_step_backprojection_set(
         self,
-        initial_set: constraints.SingleTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-        num_partitions: Optional[np.ndarray] = None,
-    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
-        reachable_set, info = self.get_reachable_set(
-            initial_set,
-            propagator,
-            t_max=1,
-            num_partitions=num_partitions,
+        target_set: constraints.SingleTimestepConstraint,
+        overapprox: bool = False,
+    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
+        backprojection_set, info = (
+            self.partitioner.get_one_step_backprojection_set(
+                target_set, self.propagator, overapprox=overapprox
+            )
         )
-        return reachable_set, info
+        return backprojection_set, info
 
-    def get_reachable_set(
+    def get_backprojection_set(
         self,
-        initial_set: constraints.SingleTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
+        target_set: constraints.SingleTimestepConstraint,
         t_max: int,
+        overapprox: bool = False,
     ) -> tuple[constraints.MultiTimestepConstraint, dict]:
-        reachable_sets = constraints.create_empty_multi_timestep_constraint(
-            propagator.boundary_type, num_facets=propagator.num_polytope_facets
+        backprojection_set, info = self.partitioner.get_backprojection_set(
+            target_set, self.propagator, t_max, overapprox=overapprox
         )
+        return backprojection_set, info
 
-        input_range = initial_set.to_range()
-
-        info = {}
-        num_propagator_calls = 0
-
-        input_shape = input_range.shape[:-1]
-
-        slope = np.divide(
-            (input_range[..., 1] - input_range[..., 0]), self.num_partitions
+    def get_N_step_backprojection_set(
+        self,
+        target_set: constraints.SingleTimestepConstraint,
+        t_max: int,
+        num_partitions=None,
+        overapprox: bool = False,
+    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
+        backprojection_set, info = (
+            self.partitioner.get_N_step_backprojection_set(
+                target_set,
+                self.propagator,
+                t_max,
+                num_partitions=num_partitions,
+                overapprox=overapprox,
+            )
         )
+        return backprojection_set, info
 
-        ranges = []
-
-        for element in product(
-            *[range(num) for num in self.num_partitions.flatten()]
-        ):
-            element_ = np.array(element).reshape(input_shape)
-            input_range_this_cell = np.empty_like(input_range)
-            input_range_this_cell[..., 0] = input_range[..., 0] + np.multiply(
-                element_, slope
-            )
-            input_range_this_cell[..., 1] = input_range[..., 0] + np.multiply(
-                element_ + 1, slope
-            )
+    def get_backprojection_error(
+        self,
+        target_set: constraints.SingleTimestepConstraint,
+        backprojection_sets: constraints.MultiTimestepConstraint,
+        t_max: int,
+    ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+        return self.partitioner.get_backprojection_error(
+            target_set,
+            backprojection_sets,
+            self.propagator,
+            t_max,
+            backreachable_sets=None,
+        )
 
-            initial_set_this_cell = initial_set.get_cell(input_range_this_cell)
+    def get_sampled_outputs(self, input_range, N=1000):
+        return get_sampled_outputs(input_range, self.propagator, N=N)
 
-            reachable_sets_this_cell, info_this_cell = (
-                propagator.get_reachable_set(initial_set_this_cell, t_max)
-            )
-            num_propagator_calls += t_max
-            info["nn_matrices"] = info_this_cell
+    def get_sampled_output_range(
+        self, input_constraint, t_max=5, num_samples=1000
+    ):
+        return self.partitioner.get_sampled_out_range(
+            input_constraint, self.propagator, t_max, num_samples
+        )
 
-            reachable_sets.add_cell(reachable_sets_this_cell)
-            ranges.append((input_range_this_cell, reachable_sets_this_cell))
+    def get_output_range(self, input_constraint, output_constraint):
+        return self.partitioner.get_output_range(
+            input_constraint, output_constraint
+        )
 
-        reachable_sets.update_main_constraint_with_cells(overapprox=True)
+    def samples_to_range(self, sampled_outputs):
+        return samples_to_range(sampled_outputs)
 
-        info["all_partitions"] = ranges
-        info["num_propagator_calls"] = num_propagator_calls
-        info["num_partitions"] = np.product(self.num_partitions)
+    def get_exact_output_range(self, input_range):
+        sampled_outputs = self.get_sampled_outputs(input_range)
+        output_range = self.samples_to_range(sampled_outputs)
+        return output_range
 
-        return reachable_sets, info
+    def get_error(self, input_constraint, output_constraint, t_max):
+        return self.partitioner.get_error(
+            input_constraint, output_constraint, self.propagator, t_max
+        )
 
-    def get_one_step_backprojection_set(
+    def visualize(
         self,
-        target_sets: constraints.MultiTimestepConstraint,
-        propagator: propagators.ClosedLoopPropagator,
-        overapprox: bool = False,
-    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
-        backreachable_set, info = self.get_one_step_backreachable_set(
-            target_sets.get_constraint_at_time_index(-1)
-        )
-        info["backreachable_set"] = backreachable_set
-
-        backprojection_set = constraints.create_empty_constraint(
-            boundary_type=propagator.boundary_type,
-            num_facets=propagator.num_polytope_facets,
-        )
-
-        """
-        Partition the backreachable set (xt).
-        For each cell in the partition:
-        - relax the NN (use CROWN to compute matrices for affine bounds)
-        - use the relaxed NN to compute bounds on xt1
-        - use those bounds to define constraints on xt, and if valid, add
-            to backprojection_set
-        """
-
-        # Setup the partitions
-        input_range = backreachable_set.range
-        input_shape = input_range.shape[:-1]
-        slope = np.divide(
-            (input_range[..., 1] - input_range[..., 0]), self.num_partitions
-        )
-
-        # Iterate through each partition
-        for element in product(
-            *[range(int(num)) for num in self.num_partitions.flatten()]
-        ):
-            # Compute this partition's min/max xt values
-            element = np.array(element).reshape(input_shape)
-            backreachable_set_this_cell = constraints.LpConstraint(
-                range=np.empty_like(input_range), p=np.inf
-            )
-            backreachable_set_this_cell.range[:, 0] = input_range[
-                :, 0
-            ] + np.multiply(element, slope)
-            backreachable_set_this_cell.range[:, 1] = input_range[
-                :, 0
-            ] + np.multiply(element + 1, slope)
-
-            backprojection_set_this_cell, this_info = (
-                propagator.get_one_step_backprojection_set(
-                    backreachable_set_this_cell,
-                    target_sets,
-                    overapprox=overapprox,
-                )
-            )
-
-            backprojection_set.add_cell(backprojection_set_this_cell)
-
-        backprojection_set.update_main_constraint_with_cells(
-            overapprox=overapprox
+        initial_set: constraints.SingleTimestepConstraint,
+        reachable_sets: constraints.MultiTimestepConstraint,
+        network: torch.nn.Sequential,
+        **kwargs,
+    ) -> None:
+        self.visualizer.visualize(
+            initial_set, reachable_sets, network, **kwargs
         )
-
-        if overapprox:
-            # These will be used to further backproject this set in time
-            backprojection_set.crown_matrices = get_crown_matrices(
-                propagator,
-                backprojection_set,
-                self.dynamics.num_inputs,
-                self.dynamics.sensor_noise,
-            )
-
-        return backprojection_set, info
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/GreedySimGuidedPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/GreedySimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/NoPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/NoPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/Partitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/Partitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/SimGuidedPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/SimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/UnGuidedPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/UnGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/UniformPartitioner.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/UniformPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/__init__.py` & `nfl_veripy-0.0.2/src/nfl_veripy/partitioners/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,36 @@
+from typing import Type
+
+from .AdaptiveGreedySimGuidedPartitioner import (
+    AdaptiveGreedySimGuidedPartitioner,
+)
 from .ClosedLoopGreedySimGuidedPartitioner import (
     ClosedLoopGreedySimGuidedPartitioner,
 )
-from .ClosedLoopNickPartitioner import ClosedLoopNickPartitioner
 from .ClosedLoopNoPartitioner import ClosedLoopNoPartitioner
 from .ClosedLoopPartitioner import ClosedLoopPartitioner  # noqa
 from .ClosedLoopSimGuidedPartitioner import ClosedLoopSimGuidedPartitioner
 from .ClosedLoopUnGuidedPartitioner import ClosedLoopUnGuidedPartitioner
 from .ClosedLoopUniformPartitioner import ClosedLoopUniformPartitioner
+from .GreedySimGuidedPartitioner import GreedySimGuidedPartitioner
+from .NoPartitioner import NoPartitioner
+from .Partitioner import Partitioner  # noqa
+from .SimGuidedPartitioner import SimGuidedPartitioner
+from .UnGuidedPartitioner import UnGuidedPartitioner
+from .UniformPartitioner import UniformPartitioner
 
-partitioner_dict = {
+partitioner_dict: dict[str, Type[ClosedLoopPartitioner]] = {
     "None": ClosedLoopNoPartitioner,
     "Uniform": ClosedLoopUniformPartitioner,
     "SimGuided": ClosedLoopSimGuidedPartitioner,
     "GreedySimGuided": ClosedLoopGreedySimGuidedPartitioner,
     "UnGuided": ClosedLoopUnGuidedPartitioner,
-    "Nick": ClosedLoopNickPartitioner,
 }
 
 
-from .AdaptiveGreedySimGuidedPartitioner import (
-    AdaptiveGreedySimGuidedPartitioner,
-)
-from .GreedySimGuidedPartitioner import GreedySimGuidedPartitioner
-from .NoPartitioner import NoPartitioner
-from .Partitioner import Partitioner
-from .SimGuidedPartitioner import SimGuidedPartitioner
-from .UnGuidedPartitioner import UnGuidedPartitioner
-from .UniformPartitioner import UniformPartitioner
-
 open_loop_partitioner_dict = {
     "None": NoPartitioner,
     "Uniform": UniformPartitioner,
     "SimGuided": SimGuidedPartitioner,
     "GreedySimGuided": GreedySimGuidedPartitioner,
     "AdaptiveGreedySimGuided": AdaptiveGreedySimGuidedPartitioner,
     "UnGuided": UnGuidedPartitioner,
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/AutoLIRPA.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/AutoLIRPA.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopJaxVerifyPropagator.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopJaxVerifyPropagator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 """Compute reachable set of neural feedback loop in Jax."""
 import functools
-import itertools
+from typing import Callable, Optional
 
 import cvxpy as cp
 import jax
 import jax.numpy as jnp
+import jax_verify
 import numpy as np
-import pypoman
 import torch
+from tqdm import tqdm
+
+import nfl_veripy.dynamics as dynamics
 from nfl_veripy import constraints
 from nfl_veripy.utils.closed_loop_verification_jax import (
     backward_crown_bound_propagation_linfun,
     get_multi_step_reachable_sets_unrolled,
 )
 from nfl_veripy.utils.nn_jax import (
     predict_future_states,
     predict_mlp,
     predict_next_state,
 )
 from nfl_veripy.utils.utils import range_to_polytope
-from tqdm import tqdm
-
-import jax_verify
 
 from .ClosedLoopPropagator import ClosedLoopPropagator
 
 
 class ClosedLoopJaxPropagator(ClosedLoopPropagator):
     """Abstract class for fwd/bwd reachability using jax_verify library."""
 
-    def __init__(
-        self,
-        input_shape=None,
-        dynamics=None,
-        num_iterations=1,
-        pre_compile=False,
-    ):
-        super().__init__(input_shape=input_shape, dynamics=dynamics)
-        self.reach_fn = None
-        self.verif_fn = None
-        self.num_iterations = num_iterations
-        self.pre_compile = pre_compile
-
-    def torch2network(self, torch_model):
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.reach_fn: Callable = get_multi_step_reachable_sets_unrolled
+        self.verif_fn: Callable = jax_verify.backward_crown_bound_propagation
+        self.pre_compile: bool = False
+
+    def torch2network(
+        self, torch_model: torch.nn.Sequential
+    ) -> torch.nn.Sequential:
         params = []
         act = None
 
         # Extract params (weights, biases) from torch layers, to be used in
         # jax.
         # Note: This propagator assumes a feed-forward relu NN.
         for m in torch_model.modules():
@@ -66,362 +61,189 @@
             else:
                 raise ValueError("That layer isn't supported.")
         self.params = params
 
         # Internally, we'll just use the typical torch stuff
         return torch_model
 
-    def forward_pass(self, input_data):
+    def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
         return self.network(
             torch.Tensor(input_data), method_opt=None
         ).data.numpy()
 
     def get_one_step_backprojection_set(
-        self, output_constraint, input_constraint, num_partitions=None
-    ):
+        self,
+        backreachable_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+        overapprox: bool = False,
+        infos: dict = {},
+        facet_inds_to_optimize: Optional[np.ndarray] = None,
+    ) -> tuple[Optional[constraints.SingleTimestepConstraint], dict]:
         raise NotImplementedError
 
 
 class ClosedLoopJaxIterativePropagator(ClosedLoopJaxPropagator):
     """Fwd/Bwd reachability using jax_verify library."""
 
-    def __init__(
-        self,
-        input_shape=None,
-        dynamics=None,
-        num_iterations=1,
-        pre_compile=False,
-    ):
-        super().__init__(
-            input_shape=input_shape,
-            dynamics=dynamics,
-            num_iterations=num_iterations,
-            pre_compile=pre_compile,
-        )
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
         self.verif_fn = jax_verify.backward_crown_bound_propagation
 
-    def get_reachable_set(self, input_constraint, t_max):
+    def get_reachable_set(
+        self, initial_set: constraints.SingleTimestepConstraint, t_max: int
+    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
+        initial_set_range = initial_set.to_range()
         xt_bounds = jax_verify.IntervalBound(
-            jnp.array([input_constraint.range[..., 0]]),
-            jnp.array([input_constraint.range[..., 1]]),
+            jnp.array([initial_set_range[..., 0]]),
+            jnp.array([initial_set_range[..., 1]]),
         )
         num_timesteps = self.dynamics.tmax_to_num_timesteps(t_max)
 
         fun_to_prop = functools.partial(
             predict_next_state, self.params, self.dynamics
         )
         # fun_to_prop = functools.partial(predict_mlp_unclipped, self.params)
         all_bounds = [xt_bounds]
         for _ in range(num_timesteps):
             xt_bounds = self.verif_fn(fun_to_prop, xt_bounds)
             all_bounds.append(xt_bounds)
-        reachable_sets = jnp.array(
+        reachable_sets_jnp = jnp.array(
             [
                 jnp.array([all_bounds[i].lower, all_bounds[i].upper]).T
                 for i in range(1, len(all_bounds))
             ]
         )
 
-        reachable_sets = np.array(reachable_sets[:, :, 0, :])
+        reachable_sets_np = np.array(reachable_sets_jnp[:, :, 0, :])
 
-        output_constraints = constraints.MultiTimestepLpConstraint(
-            range=reachable_sets
+        reachable_sets = constraints.MultiTimestepConstraint(
+            constraints=[
+                constraints.LpConstraint(range=r) for r in reachable_sets_np
+            ]
         )
 
-        return output_constraints, {}
-
-    def get_backprojection_set(
-        self,
-        output_constraints,
-        input_constraint,
-        t_max,
-        num_partitions=None,
-        overapprox=False,
-        refined=False,
-    ):
-        bps = []
-        bp = output_constraints[0]
-        if isinstance(bp, constraints.LpConstraint):
-            A, b = range_to_polytope(bp.range)
-            bp = constraints.PolytopeConstraint(A=A, b=b)
-        infos = {"per_timestep": []}
-        num_timesteps = self.dynamics.tmax_to_num_timesteps(t_max)
-        for _ in range(num_timesteps):
-            bp, info = self.get_one_step_backprojection_set(
-                bp, num_partitions=num_partitions
-            )
-            bps.append(bp)
-            infos["per_timestep"].append(info)
-        return [bps], [infos]
+        return reachable_sets, {}
 
     def get_one_step_backprojection_set(
         self,
-        backreachable_set,
-        target_sets,
-        overapprox=False,
-    ):
-        info = {}
-        # backreachable_set = self.get_one_step_backreachable_set(target_set)
-        # info['backreachable_set'] = backreachable_set
-        # info['target_set'] = copy.deepcopy(target_set)
-
-        return self.get_one_step_backprojection_set_without_partitioning(
-            backreachable_set, target_sets, info
-        )
-        # else:
-        #   return self.get_one_step_backprojection_set_with_partitioning(
-        #       backreachable_set, target_sets, info, num_partitions)
-
-    def get_one_step_backprojection_set_without_partitioning(
-        self, backreachable_set, target_sets, info
-    ):
+        backreachable_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+        overapprox: bool = False,
+        info: dict = {},
+        facet_inds_to_optimize: Optional[np.ndarray] = None,
+    ) -> tuple[Optional[constraints.SingleTimestepConstraint], dict]:
         A, b = range_to_polytope(backreachable_set.range)
         backprojection_set = constraints.PolytopeConstraint(A=A, b=b)
-        for _ in range(self.num_iterations):
-            backprojection_set = self.improve_backprojection_set(
+        improved_backprojection_set = (
+            self.iteratively_improve_backprojection_set(
                 backprojection_set, target_sets
             )
-
-        return backprojection_set, info
-
-    def get_one_step_backprojection_set_with_partitioning(
-        self, backreachable_set, target_set, info, num_partitions
-    ):
-        slope = np.divide(
-            (backreachable_set.range[:, 1] - backreachable_set.range[:, 0]),
-            num_partitions,
-        )
-        vertices = []
-
-        # Iterate through each partition
-        for element in itertools.product(
-            *[range(num) for num in num_partitions.flatten()]
-        ):
-            element_ = np.array(element).reshape((self.dynamics.num_states,))
-            br_cell_range = np.empty_like(backreachable_set.range)
-            br_cell_range[:, 0] = backreachable_set.range[:, 0] + np.multiply(
-                element_, slope
-            )
-            br_cell_range[:, 1] = backreachable_set.range[:, 0] + np.multiply(
-                element_ + 1, slope
-            )
-            A, b = range_to_polytope(br_cell_range)
-            backprojection_set = constraints.PolytopeConstraint(A=A, b=b)
-
-            backprojection_set = self.iteratively_improve_backprojection_set(
-                backprojection_set, target_set
-            )
-            if backprojection_set == "infeasible":
-                continue
-
-            if isinstance(backprojection_set, constraints.LpConstraint):
-                v = np.array(
-                    list(itertools.product(*backprojection_set.range))
-                )
-            else:
-                v = pypoman.duality.compute_polytope_vertices(
-                    backprojection_set.A, backprojection_set.b
-                )
-            if len(v) == 0:
-                continue
-            vertices.append(v)
-
-        # Merge vertices of all partitions' BPOAs into a single polytope
-        A, b = pypoman.duality.compute_polytope_halfspaces(
-            pypoman.duality.convex_hull(np.vstack(vertices))
         )
-        backprojection_set = constraints.PolytopeConstraint(A=A, b=b)
 
-        return backprojection_set, info
+        return improved_backprojection_set, info
+
+    def improve_backprojection_set(
+        self,
+        backprojection_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
+        raise NotImplementedError
 
     def iteratively_improve_backprojection_set(
-        self, backprojection_set, target_set
-    ):
+        self,
+        backprojection_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
         for _ in range(self.num_iterations):
             backprojection_set = self.improve_backprojection_set(
-                backprojection_set, target_set
-            )
-            if backprojection_set == "infeasible":
-                return "infeasible"
+                backprojection_set, target_sets
+            )  # type: ignore
+            if backprojection_set.is_infeasible:
+                return backprojection_set
 
         return backprojection_set
 
-    def get_one_step_backreachable_set(self, target_set):
-        """Find (hyperrectangle) set of states that lead to target_set while
-        following dynamics, x_limits, u_limits."""
-
-        if self.dynamics.u_limits is None:
-            print("self.dynamics.u_limits is None")
-            print(
-                "==> The backreachable set is probably the whole state space."
-            )
-            print("Giving up.")
-            raise NotImplementedError
-        else:
-            u_min = self.dynamics.u_limits[:, 0]
-            u_max = self.dynamics.u_limits[:, 1]
-
-        xt = cp.Variable((self.dynamics.num_states, 2))
-        ut = cp.Variable(self.dynamics.num_inputs)
-
-        # For each dimension of the output constraint (facet/lp-dimension):
-        # compute a bound of the NN output using the pre-computed matrices
-        xt = cp.Variable(self.dynamics.num_states)
-        ut = cp.Variable(self.dynamics.num_inputs)
-        constrs = []
-        constrs += [u_min <= ut]
-        constrs += [ut <= u_max]
-
-        # Note: state limits are not included in CDC 2022 paper
-        # results/discussion. Included state limits to reduce size of
-        # backreachable sets by eliminating states that are not physically
-        # possible (e.g., maximum velocities)
-        if self.dynamics.x_limits is not None:
-            if isinstance(self.dynamics.x_limits, dict):
-                for state in self.dynamics.x_limits:
-                    constrs += [xt[state] >= self.dynamics.x_limits[state][0]]
-                    constrs += [xt[state] <= self.dynamics.x_limits[state][1]]
-            else:
-                constrs += [xt >= self.dynamics.x_limits[:, 0]]
-                constrs += [xt <= self.dynamics.x_limits[:, 1]]
-
-        if isinstance(target_set, constraints.PolytopeConstraint):
-            constrs += [
-                target_set.A @ self.dynamics.dynamics_step(xt, ut)
-                <= target_set.b
-            ]
-        elif isinstance(target_set, constraints.LpConstraint):
-            constrs += [
-                self.dynamics.dynamics_step(xt, ut) <= target_set.range[..., 1]
-            ]
-            constrs += [
-                self.dynamics.dynamics_step(xt, ut) >= target_set.range[..., 0]
-            ]
-
-        obj_facets = np.eye(self.dynamics.num_states)
-        num_facets = obj_facets.shape[0]
-        coords = np.empty(
-            (2 * self.dynamics.num_states, self.dynamics.num_states)
-        )
-
-        obj_facets_i = cp.Parameter(self.dynamics.num_states)
-        obj = obj_facets_i @ xt
-        min_prob = cp.Problem(cp.Minimize(obj), constrs)
-        max_prob = cp.Problem(cp.Maximize(obj), constrs)
-        for i in range(num_facets):
-            obj_facets_i.value = obj_facets[i, :]
-            min_prob.solve()
-            coords[2 * i, :] = xt.value
-            max_prob.solve()
-            coords[2 * i + 1, :] = xt.value
-
-        # min/max of each element of xt in the backreachable set
-        ranges = np.vstack([coords.min(axis=0), coords.max(axis=0)]).T
-
-        backreachable_set = constraints.LpConstraint(range=ranges)
-        return backreachable_set
-
 
 class ClosedLoopJaxPolytopePropagator(ClosedLoopJaxIterativePropagator):
     """Backward reachability using jax_verify, where BP sets are improved
     using closed-form solution based on polytope relaxation domains (DRIP)."""
 
-    def __init__(
-        self,
-        input_shape=None,
-        dynamics=None,
-        num_iterations=1,
-        pre_compile=False,
-    ):
-        super().__init__(
-            input_shape=input_shape,
-            dynamics=dynamics,
-            num_iterations=num_iterations,
-            pre_compile=pre_compile,
-        )
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
         self.boundary_type = "polytope"
 
     def improve_backprojection_set(
-        self, initial_backprojection_set, target_set
-    ):
-        fun_to_prop = functools.partial(
-            predict_next_state, self.params, self.dynamics
-        )
-
-        vertices = np.stack(
-            pypoman.compute_polytope_vertices(
-                initial_backprojection_set.A, initial_backprojection_set.b
-            )
-        )
-        # num_vertices = vertices.shape[0]
-
-        input_bounds = None  # simplex bound goes here
+        self,
+        backprojection_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
         raise NotImplementedError
-        input_interval_bounds = jax_verify.IntervalBound(
-            jnp.array(np.min(vertices, axis=0)),
-            jnp.array(np.max(vertices, axis=0)),
-        )
-
-        def predict_next_state_simplex(params, dynamics, xt_simplex):
-            xt = jnp.dot(xt_simplex, vertices)
-            ut = predict_mlp(params, dynamics.u_limits, xt)
-            xt1 = dynamics.dynamics_step_jnp(xt, ut)
-            return xt1
 
-        fun_to_prop = functools.partial(
-            predict_next_state_simplex, self.params, self.dynamics
-        )
-
-        obj = jnp.expand_dims(target_set.A, 1)
-        linfuns = backward_crown_bound_propagation_linfun(
-            fun_to_prop, input_bounds, obj=obj
-        )
-
-        B = jnp.vstack(
-            [
-                linfuns[0].lin_coeffs,
-                jnp.eye(self.dynamics.num_states),
-                -jnp.eye(self.dynamics.num_states),
-            ]
-        )
-        c = jnp.hstack(
-            [
-                target_set.b - linfuns[0].offset,
-                input_interval_bounds.upper,
-                -input_interval_bounds.lower,
-            ]
-        )
-        backprojection_set = constraints.PolytopeConstraint(
-            A=np.array(B, dtype=np.double), b=np.array(c, dtype=np.double)
-        )
+        # fun_to_prop = functools.partial(
+        #     predict_next_state, self.params, self.dynamics
+        # )
+
+        # vertices = backprojection_set.get_vertices()
+
+        # input_bounds = None  # simplex bound goes here
+
+        # input_interval_bounds = jax_verify.IntervalBound(
+        #     jnp.array(np.min(vertices, axis=0)),
+        #     jnp.array(np.max(vertices, axis=0)),
+        # )
+
+        # def predict_next_state_simplex(params, dynamics, xt_simplex):
+        #     xt = jnp.dot(xt_simplex, vertices)
+        #     ut = predict_mlp(params, dynamics.u_limits, xt)
+        #     xt1 = dynamics.dynamics_step_jnp(xt, ut)
+        #     return xt1
+
+        # fun_to_prop = functools.partial(
+        #     predict_next_state_simplex, self.params, self.dynamics
+        # )
+
+        # obj = jnp.expand_dims(target_set.A, 1)
+        # linfuns = backward_crown_bound_propagation_linfun(
+        #     fun_to_prop, input_bounds, obj=obj
+        # )
+
+        # B = jnp.vstack(
+        #     [
+        #         linfuns[0].lin_coeffs,
+        #         jnp.eye(self.dynamics.num_states),
+        #         -jnp.eye(self.dynamics.num_states),
+        #     ]
+        # )
+        # c = jnp.hstack(
+        #     [
+        #         target_set.b - linfuns[0].offset,
+        #         input_interval_bounds.upper,
+        #         -input_interval_bounds.lower,
+        #     ]
+        # )
+        # backprojection_set = constraints.PolytopeConstraint(
+        #     A=np.array(B, dtype=np.double), b=np.array(c, dtype=np.double)
+        # )
 
-        return backprojection_set
+        # return backprojection_set
 
 
 class ClosedLoopJaxPolytopeJittedPropagator(ClosedLoopJaxIterativePropagator):
     """JIT-enabled backward reachability using jax_verify, where BP sets are
     improved using closed-form solution based on polytope relaxation domains
     (DRIP).
     """
 
-    def __init__(
-        self,
-        input_shape=None,
-        dynamics=None,
-        num_iterations=1,
-        pre_compile=False,
-    ):
-        super().__init__(
-            input_shape=input_shape,
-            dynamics=dynamics,
-            num_iterations=num_iterations,
-            pre_compile=pre_compile,
-        )
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.boundary_type = "polytope"
 
-    def torch2network(self, torch_model):
+    def torch2network(
+        self, torch_model: torch.nn.Sequential
+    ) -> torch.nn.Sequential:
         return_args = super().torch2network(torch_model)
 
         self.fun_to_prop = functools.partial(
             predict_next_state, self.params, self.dynamics
         )
         if self.pre_compile:
             vertices_shapes = [(4, 2), (8, 2), (16, 2), (32, 2), (64, 2)]
@@ -438,147 +260,130 @@
             if pre_compile:
                 with tqdm(total=num_elements) as pbar:
                     for obj_shape in obj_shapes:
                         for vertices_shape in vertices_shapes:
                             vertices = np.zeros(vertices_shape)
                             obj = np.zeros(obj_shape)
                             input_bounds = None  # simplex bounds go here
+                            raise NotImplementedError
                             jittable_input_bounds = input_bounds.to_jittable()
                             _, _ = bound_prop_fun(
                                 jittable_input_bounds,
                                 vertices,
                                 obj,
                                 self.fun_to_prop,
                             )
                             pbar.update(1)
 
         return return_args
 
     def improve_backprojection_set(
-        self, initial_backprojection_set, target_set
-    ):
-        vertices = pypoman.compute_polytope_vertices(
-            initial_backprojection_set.A, initial_backprojection_set.b
-        )
-        vertices = np.stack(vertices)
-        num_vertices_to_pad = (
-            2 ** int(jnp.ceil(jnp.log2(vertices.shape[0]))) - vertices.shape[0]
-        )
-        vertices = np.vstack(
-            [vertices, np.tile(vertices[-1, :], (num_vertices_to_pad, 1))]
-        )
-        input_bounds = None  # simplex_bounds go here.
+        self,
+        backprojection_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
         raise NotImplementedError
-        input_interval_bounds = jax_verify.IntervalBound(
-            jnp.array(np.min(vertices, axis=0)),
-            jnp.array(np.max(vertices, axis=0)),
-        )
-
-        obj = target_set.A
-        num_facets_to_pad = (
-            2 ** int(jnp.ceil(jnp.log2(obj.shape[0]))) - obj.shape[0]
-        )
-        obj = np.vstack([obj, np.zeros((num_facets_to_pad, 2))])
-        obj = jnp.expand_dims(obj, 1)
-
-        jittable_input_bounds = input_bounds.to_jittable()
-
-        lin_coeffs, offset = simplex_bound_prop_fun(
-            jittable_input_bounds, vertices, obj, self.fun_to_prop
-        )
-
-        if num_facets_to_pad > 0:
-            lin_coeffs = lin_coeffs[:-num_facets_to_pad]
-            offset = offset[:-num_facets_to_pad]
 
-        # This could be tighter if we used initial_backprojection_set instead
-        # of input_interval_bounds, but the former adds a lot of redundant
-        # constraints that would need to be dealt with.
-        B = jnp.vstack(
-            [
-                lin_coeffs,
-                jnp.eye(self.dynamics.num_states),
-                -jnp.eye(self.dynamics.num_states),
-            ]
-        )
-        c = jnp.hstack(
-            [
-                target_set.b - offset,
-                input_interval_bounds.upper,
-                -input_interval_bounds.lower,
-            ]
-        )
-        backprojection_set = constraints.PolytopeConstraint(
-            A=np.array(B, dtype=np.double), b=np.array(c, dtype=np.double)
-        )
+        # vertices = backprojection_set.get_vertices()
+        # num_vertices_to_pad = (
+        #     2 ** int(jnp.ceil(jnp.log2(vertices.shape[0])))
+        #     - vertices.shape[0]
+        # )
+        # vertices = np.vstack(
+        #     [vertices, np.tile(vertices[-1, :], (num_vertices_to_pad, 1))]
+        # )
+        # input_bounds = None  # simplex_bounds go here.
+        # input_interval_bounds = jax_verify.IntervalBound(
+        #     jnp.array(np.min(vertices, axis=0)),
+        #     jnp.array(np.max(vertices, axis=0)),
+        # )
+
+        # obj = target_set.A
+        # num_facets_to_pad = (
+        #     2 ** int(jnp.ceil(jnp.log2(obj.shape[0]))) - obj.shape[0]
+        # )
+        # obj = np.vstack([obj, np.zeros((num_facets_to_pad, 2))])
+        # obj = jnp.expand_dims(obj, 1)
+
+        # jittable_input_bounds = input_bounds.to_jittable()
+
+        # lin_coeffs, offset = simplex_bound_prop_fun(
+        #     jittable_input_bounds, vertices, obj, self.fun_to_prop
+        # )
+
+        # if num_facets_to_pad > 0:
+        #     lin_coeffs = lin_coeffs[:-num_facets_to_pad]
+        #     offset = offset[:-num_facets_to_pad]
+
+        # # This could be tighter if we used initial_backprojection_set instead
+        # # of input_interval_bounds, but the former adds a lot of redundant
+        # # constraints that would need to be dealt with.
+        # B = jnp.vstack(
+        #     [
+        #         lin_coeffs,
+        #         jnp.eye(self.dynamics.num_states),
+        #         -jnp.eye(self.dynamics.num_states),
+        #     ]
+        # )
+        # c = jnp.hstack(
+        #     [
+        #         target_set.b - offset,
+        #         input_interval_bounds.upper,
+        #         -input_interval_bounds.lower,
+        #     ]
+        # )
+        # backprojection_set = constraints.PolytopeConstraint(
+        #     A=np.array(B, dtype=np.double), b=np.array(c, dtype=np.double)
+        # )
 
-        return backprojection_set
+        # return backprojection_set
 
 
 class ClosedLoopJaxRectanglePropagator(ClosedLoopJaxIterativePropagator):
     """Backward reachability using jax_verify, where BP sets are improved
     using a closed-form solution based on hyperrectangle relaxation domains
     (DRIP-HPoly)."""
 
-    def __init__(
-        self,
-        input_shape=None,
-        dynamics=None,
-        num_iterations=1,
-        pre_compile=False,
-    ):
-        super().__init__(
-            input_shape=input_shape,
-            dynamics=dynamics,
-            num_iterations=num_iterations,
-            pre_compile=pre_compile,
-        )
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
         self.boundary_type = "polytope"
 
     def improve_backprojection_set(
-        self, initial_backprojection_set, target_sets
-    ):
-        if isinstance(
-            initial_backprojection_set, constraints.PolytopeConstraint
-        ):
-            input_bounds_np = initial_backprojection_set.to_linf()
-            input_bounds = jax_verify.IntervalBound(
-                jnp.array([input_bounds_np[:, 0]]),
-                jnp.array([input_bounds_np[:, 1]]),
-            )
-        elif isinstance(initial_backprojection_set, constraints.LpConstraint):
-            input_bounds = jax_verify.IntervalBound(
-                jnp.array([initial_backprojection_set.range[:, 0]]),
-                jnp.array([initial_backprojection_set.range[:, 1]]),
-            )
+        self,
+        backprojection_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
+        input_bounds_np = backprojection_set.to_range()
+        input_bounds = jax_verify.IntervalBound(
+            jnp.array([input_bounds_np[:, 0]]),
+            jnp.array([input_bounds_np[:, 1]]),
+        )
 
         fun_to_prop = functools.partial(
             predict_next_state, self.params, self.dynamics
         )
 
         target_set = target_sets.get_constraint_at_time_index(-1)
-        if isinstance(target_sets, constraints.LpConstraint):
-            A, b = target_set.get_polytope()
-            target_set = constraints.PolytopeConstraint(A, b)
+        target_set_A, target_set_b = target_set.get_polytope()
 
-        obj = jnp.expand_dims(target_set.A, 1)
+        obj = jnp.expand_dims(target_set_A, 1)
         linfuns = backward_crown_bound_propagation_linfun(
             fun_to_prop, input_bounds, obj=obj
         )
 
         B = jnp.vstack(
             [
                 linfuns[0].lin_coeffs[:, 0, :],
                 jnp.eye(self.dynamics.num_states),
                 -jnp.eye(self.dynamics.num_states),
             ]
         )
         c = jnp.hstack(
             [
-                target_set.b - linfuns[0].offset,
+                target_set_b - linfuns[0].offset,
                 input_bounds.upper[0, :],
                 -input_bounds.lower[0, :],
             ]
         )
 
         backprojection_set = constraints.PolytopeConstraint(
             A=np.array(B, dtype=np.double), b=np.array(c, dtype=np.double)
@@ -588,29 +393,21 @@
 
 
 class ClosedLoopJaxRectangleJittedPropagator(ClosedLoopJaxIterativePropagator):
     """JIT-enabled backward reachability using jax_verify, where BP sets are
     improved using a closed-form solution based on hyperrectangle relaxation
     domains (DRIP-HPoly)."""
 
-    def __init__(
-        self,
-        input_shape=None,
-        dynamics=None,
-        num_iterations=1,
-        pre_compile=False,
-    ):
-        super().__init__(
-            input_shape=input_shape,
-            dynamics=dynamics,
-            num_iterations=num_iterations,
-            pre_compile=pre_compile,
-        )
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.boundary_type = "rectangle"
 
-    def torch2network(self, torch_model):
+    def torch2network(
+        self, torch_model: torch.nn.Sequential
+    ) -> torch.nn.Sequential:
         return_args = super().torch2network(torch_model)
 
         self.fun_to_prop = functools.partial(
             predict_next_state, self.params, self.dynamics
         )
 
         if self.pre_compile:
@@ -628,48 +425,46 @@
             num_elements = len(vertices_shapes) * len(obj_shapes)
             with tqdm(total=num_elements) as pbar:
                 for obj_shape in obj_shapes:
                     for vertices_shape in vertices_shapes:
                         vertices = np.zeros(vertices_shape)
                         obj = np.zeros(obj_shape)
                         input_bounds = None  # simplex bound goes here
+                        raise NotImplementedError
                         jittable_input_bounds = input_bounds.to_jittable()
                         _, _ = bound_prop_fun(
                             jittable_input_bounds,
                             vertices,
                             obj,
                             self.fun_to_prop,
                         )
                         pbar.update(1)
 
         return return_args
 
     def improve_backprojection_set(
-        self, initial_backprojection_set, target_set
-    ):
-        if isinstance(
-            initial_backprojection_set, constraints.PolytopeConstraint
-        ):
-            input_bounds_np = initial_backprojection_set.to_linf()
-            input_bounds = jax_verify.IntervalBound(
-                jnp.array(input_bounds_np[:, 0]),
-                jnp.array(input_bounds_np[:, 1]),
-            )
-        elif isinstance(initial_backprojection_set, constraints.LpConstraint):
-            input_bounds = jax_verify.IntervalBound(
-                jnp.array(initial_backprojection_set.range[:, 0]),
-                jnp.array(initial_backprojection_set.range[:, 1]),
-            )
+        self,
+        backprojection_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
+        input_bounds_np = backprojection_set.to_range()
+        input_bounds = jax_verify.IntervalBound(
+            jnp.array([input_bounds_np[:, 0]]),
+            jnp.array([input_bounds_np[:, 1]]),
+        )
 
-        obj = target_set.A
+        target_set = target_sets.get_constraint_at_time_index(-1)
+        target_set_A, target_set_b = target_set.get_polytope()
         num_facets_to_pad = (
-            2 ** int(jnp.ceil(jnp.log2(obj.shape[0]))) - obj.shape[0]
+            2 ** int(jnp.ceil(jnp.log2(target_set_A.shape[0])))
+            - target_set_A.shape[0]
+        )
+        obj = jnp.expand_dims(
+            np.vstack([target_set_A, np.zeros((num_facets_to_pad, 2))]), 1
         )
-        obj = np.vstack([obj, np.zeros((num_facets_to_pad, 2))])
-        obj = jnp.expand_dims(obj, 1)
 
         jittable_input_bounds = input_bounds.to_jittable()
 
         lin_coeffs, offset = bound_prop_fun(
             jittable_input_bounds, obj, self.fun_to_prop
         )
         if num_facets_to_pad > 0:
@@ -680,67 +475,55 @@
             [
                 lin_coeffs,
                 jnp.eye(self.dynamics.num_states),
                 -jnp.eye(self.dynamics.num_states),
             ]
         )
         c = jnp.hstack(
-            [target_set.b - offset, input_bounds.upper, -input_bounds.lower]
+            [target_set_b - offset, input_bounds.upper, -input_bounds.lower]
         )
 
         backprojection_set = constraints.PolytopeConstraint(
             A=np.array(B, dtype=np.double), b=np.array(c, dtype=np.double)
         )
 
         return backprojection_set
 
 
 class ClosedLoopJaxLPJittedPropagator(ClosedLoopJaxIterativePropagator):
     """JIT-enabled backward reachability using jax_verify, where BP sets are
     improved using a LP formulation."""
 
-    def __init__(
-        self,
-        input_shape=None,
-        dynamics=None,
-        num_iterations=1,
-        pre_compile=False,
-    ):
-        super().__init__(
-            input_shape=input_shape,
-            dynamics=dynamics,
-            num_iterations=num_iterations,
-            pre_compile=pre_compile,
-        )
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.boundary_type = "rectangle"
 
-    def torch2network(self, torch_model):
+    def torch2network(
+        self, torch_model: torch.nn.Sequential
+    ) -> torch.nn.Sequential:
         return_args = super().torch2network(torch_model)
 
         self.fun_to_prop = functools.partial(
             predict_mlp, self.params, self.dynamics.u_limits
         )
 
         if self.pre_compile:
             raise NotImplementedError
 
         return return_args
 
     def improve_backprojection_set(
-        self, initial_backprojection_set, target_set
-    ):
-        if isinstance(
-            initial_backprojection_set, constraints.PolytopeConstraint
-        ):
-            initial_backprojection_set = constraints.LpConstraint(
-                range=initial_backprojection_set.to_linf()
-            )
-
+        self,
+        backprojection_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
+        input_bounds_np = backprojection_set.to_range()
         input_bounds = jax_verify.IntervalBound(
-            jnp.array(initial_backprojection_set.range[:, 0]),
-            jnp.array(initial_backprojection_set.range[:, 1]),
+            jnp.array([input_bounds_np[:, 0]]),
+            jnp.array([input_bounds_np[:, 1]]),
         )
         jittable_input_bounds = input_bounds.to_jittable()
 
         obj = jnp.expand_dims(
             jnp.vstack(
                 [
                     jnp.eye(self.dynamics.num_inputs),
@@ -763,26 +546,19 @@
         constrs = []
 
         # Constraints to ensure that xt stays within the backreachable set
         constrs += [input_bounds.lower <= xt]
         constrs += [xt <= input_bounds.upper]
 
         # Constraints to ensure xt reaches the target set given ut
-        if isinstance(target_set, constraints.PolytopeConstraint):
-            constrs += [
-                target_set.A @ self.dynamics.dynamics_step(xt, ut)
-                <= target_set.b
-            ]
-        elif isinstance(target_set, constraints.LpConstraint):
-            constrs += [
-                self.dynamics.dynamics_step(xt, ut) <= target_set.range[:, 1]
-            ]
-            constrs += [
-                self.dynamics.dynamics_step(xt, ut) >= target_set.range[:, 0]
-            ]
+        target_set = target_sets.get_constraint_at_time_index(-1)
+        target_set_A, target_set_b = target_set.get_polytope()
+        constrs += [
+            target_set_A @ self.dynamics.dynamics_step(xt, ut) <= target_set_b
+        ]
 
         half_index = self.dynamics.num_states // 2
         lower_slope = lin_coeffs[:half_index]
         lower_intercept = offset[:half_index]
         upper_slope = -lin_coeffs[half_index:]
         upper_intercept = -offset[half_index:]
 
@@ -813,54 +589,41 @@
         return backprojection_set
 
 
 class ClosedLoopJaxLPPropagator(ClosedLoopJaxIterativePropagator):
     """Backward reachability using jax_verify, where BP sets are improved
     using a LP formulation."""
 
-    def __init__(
-        self,
-        input_shape=None,
-        dynamics=None,
-        num_iterations=1,
-        pre_compile=False,
-    ):
-        super().__init__(
-            input_shape=input_shape,
-            dynamics=dynamics,
-            num_iterations=num_iterations,
-            pre_compile=pre_compile,
-        )
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
         self.boundary_type = "rectangle"
 
-    def torch2network(self, torch_model):
+    def torch2network(
+        self, torch_model: torch.nn.Sequential
+    ) -> torch.nn.Sequential:
         return_args = super().torch2network(torch_model)
 
         self.fun_to_prop = functools.partial(
             predict_mlp, self.params, self.dynamics.u_limits
         )
 
         if self.pre_compile:
             raise NotImplementedError
 
         return return_args
 
     def improve_backprojection_set(
-        self, initial_backprojection_set, target_sets
-    ):
-        if isinstance(
-            initial_backprojection_set, constraints.PolytopeConstraint
-        ):
-            initial_backprojection_set = constraints.LpConstraint(
-                range=initial_backprojection_set.to_linf()
-            )
-
+        self,
+        backprojection_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+    ) -> Optional[constraints.SingleTimestepConstraint]:
+        input_bounds_np = backprojection_set.to_range()
         input_bounds = jax_verify.IntervalBound(
-            jnp.array([initial_backprojection_set.range[:, 0]]),
-            jnp.array([initial_backprojection_set.range[:, 1]]),
+            jnp.array([input_bounds_np[:, 0]]),
+            jnp.array([input_bounds_np[:, 1]]),
         )
 
         obj = jnp.expand_dims(
             jnp.vstack(
                 [
                     jnp.eye(self.dynamics.num_inputs),
                     -jnp.eye(self.dynamics.num_inputs),
@@ -880,29 +643,20 @@
         ut = cp.Variable((self.dynamics.num_inputs,))
         constrs = []
 
         # Constraints to ensure that xt stays within the backreachable set
         constrs += [input_bounds.lower[0, :] <= xt]
         constrs += [xt <= input_bounds.upper[0, :]]
 
-        target_set = target_sets.get_constraint_at_time_index(-1)
-
         # Constraints to ensure xt reaches the target set given ut
-        if isinstance(target_set, constraints.PolytopeConstraint):
-            constrs += [
-                target_set.A @ self.dynamics.dynamics_step(xt, ut)
-                <= target_set.b
-            ]
-        elif isinstance(target_set, constraints.LpConstraint):
-            constrs += [
-                self.dynamics.dynamics_step(xt, ut) <= target_set.range[:, 1]
-            ]
-            constrs += [
-                self.dynamics.dynamics_step(xt, ut) >= target_set.range[:, 0]
-            ]
+        target_set = target_sets.get_constraint_at_time_index(-1)
+        target_set_A, target_set_b = target_set.get_polytope()
+        constrs += [
+            target_set_A @ self.dynamics.dynamics_step(xt, ut) <= target_set_b
+        ]
 
         half_index = linfuns[0].shape[0] // 2
         lower_slope = linfuns[0].lin_coeffs[:half_index][0]
         lower_intercept = linfuns[0].offset[:half_index][0]
         upper_slope = -linfuns[0].lin_coeffs[half_index:][0]
         upper_intercept = -linfuns[0].offset[half_index:][0]
 
@@ -923,118 +677,143 @@
         b_ = np.empty(2 * self.dynamics.num_states)
         for i in range(2 * self.dynamics.num_states):
             obj_facets_i.value = obj_facets[i, :]
             prob.solve()
             b_[i] = prob.value
 
         if prob.status == "infeasible":
-            return "infeasible"
+            backprojection_set = constraints.LpConstraint()
+            backprojection_set.is_infeasible = True
+            return backprojection_set
         ranges = np.vstack(
             [-b_[self.dynamics.num_states :], b_[: self.dynamics.num_states]]
         ).T
         backprojection_set = constraints.LpConstraint(range=ranges)
 
         return backprojection_set
 
 
 class ClosedLoopJaxUnrolledPropagator(ClosedLoopJaxPropagator):
     """Run CROWN on unrolled closed-loop dynamics, dyn(con(...dyn(con(x))))."""
 
-    def __init__(self, input_shape=None, dynamics=None):
-        super().__init__(input_shape=input_shape, dynamics=dynamics)
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.boundary_type = "rectangle"
         self.reach_fn = get_multi_step_reachable_sets_unrolled
         self.verif_fn = jax_verify.backward_crown_bound_propagation
 
-    def get_reachable_set(self, input_constraint, t_max):
+    def get_reachable_set(
+        self, initial_set: constraints.SingleTimestepConstraint, t_max: int
+    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
+        initial_set_range = initial_set.to_range()
         xt_bounds = jax_verify.IntervalBound(
             jnp.array(
-                input_constraint.range[..., 0].reshape(
-                    -1, self.dynamics.num_states
-                )
+                initial_set_range[..., 0].reshape(-1, self.dynamics.num_states)
             ),
             jnp.array(
-                input_constraint.range[..., 1].reshape(
-                    -1, self.dynamics.num_states
-                )
+                initial_set_range[..., 1].reshape(-1, self.dynamics.num_states)
             ),
         )
 
         num_timesteps = self.dynamics.tmax_to_num_timesteps(t_max)
 
         fun_to_prop = functools.partial(
             predict_future_states, self.params, self.dynamics, num_timesteps
         )
         bounds = self.verif_fn(fun_to_prop, xt_bounds)
 
         lbs = jnp.array([bounds[i].lower for i in range(1, num_timesteps + 1)])
         ubs = jnp.array([bounds[i].upper for i in range(1, num_timesteps + 1)])
-        reachable_sets = jnp.stack([lbs, ubs]).transpose(2, 1, 3, 0).squeeze()
+        reachable_sets_jnp = (
+            jnp.stack([lbs, ubs]).transpose(2, 1, 3, 0).squeeze()
+        )
 
-        reachable_sets = np.array(reachable_sets)
+        reachable_sets_np = np.array(reachable_sets_jnp)
 
-        output_constraints = constraints.MultiTimestepLpConstraint(
-            range=reachable_sets
+        reachable_sets = constraints.MultiTimestepConstraint(
+            constraints=[
+                constraints.LpConstraint(range=r) for r in reachable_sets_np
+            ]
         )
 
-        return output_constraints, {}
+        return reachable_sets, {}
 
 
 class ClosedLoopJaxUnrolledJittedPropagator(ClosedLoopJaxPropagator):
     """(JIT-enabled) Run CROWN on unrolled closed-loop dynamics,
     dyn(con(...dyn(con(x))))."""
 
-    def __init__(self, input_shape=None, dynamics=None):
-        super().__init__(input_shape=input_shape, dynamics=dynamics)
+    def __init__(self, dynamics: dynamics.Dynamics):
+        super().__init__(dynamics=dynamics)
+        self.boundary_type = "rectangle"
         self.reach_fn = get_multi_step_reachable_sets_unrolled
         self.verif_fn = jax_verify.backward_crown_bound_propagation
 
-    def get_reachable_set(self, initial_state_set, t_max):
-        initial_state_set_jit = initial_state_set.to_jittable()
+    def get_reachable_set(
+        self, initial_set: constraints.SingleTimestepConstraint, t_max: int
+    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
+        initial_set_jit = initial_set.to_jittable()
         reachable_sets_jnp, info = self.get_reachable_set_jitted(
-            initial_state_set_jit, t_max
+            initial_set_jit, t_max
         )
-        reachable_sets = constraints.MultiTimestepLpConstraint(
-            range=np.array(reachable_sets_jnp)
+        reachable_sets = constraints.MultiTimestepConstraint(
+            constraints=[
+                constraints.LpConstraint(range=r) for r in reachable_sets_jnp
+            ]
         )
         return reachable_sets, info
 
     @functools.partial(jax.jit, static_argnames=["self", "t_max"])
-    def get_reachable_set_jitted(self, initial_state_set_jit, t_max):
+    def get_reachable_set_jitted(
+        self,
+        initial_set_jitted: constraints.JittableSingleTimestepConstraint,
+        t_max: int,
+    ) -> tuple[jnp.ndarray, dict]:
         num_timesteps = self.dynamics.tmax_to_num_timesteps(t_max)
 
-        def bound_prop_fun_(inp_bound, fun_to_prop):
+        def bound_prop_fun_(
+            inp_bound: constraints.JittableSingleTimestepConstraint,
+            fun_to_prop: Callable,
+        ) -> jnp.ndarray:
             (inp_bound_unjit,) = constraints.unjit_lp_constraints(inp_bound)
             bounds = self.verif_fn(fun_to_prop, inp_bound_unjit)
             lbs = jnp.array(
                 [bounds[i].lower for i in range(1, num_timesteps + 1)]
             )
             ubs = jnp.array(
                 [bounds[i].upper for i in range(1, num_timesteps + 1)]
             )
             return jnp.stack([lbs, ubs]).transpose(1, 2, 0)
 
         fun_to_prop = functools.partial(
             predict_future_states, self.params, self.dynamics, num_timesteps
         )
-        reachable_sets_jnp = bound_prop_fun_(
-            initial_state_set_jit, fun_to_prop
-        )
+        reachable_sets_jnp = bound_prop_fun_(initial_set_jitted, fun_to_prop)
 
         return reachable_sets_jnp, {}
 
 
 @functools.partial(jax.jit, static_argnames=["fun_to_prop"])
-def simplex_bound_prop_fun(inp_bound, vertices, obj, fun_to_prop):
+def simplex_bound_prop_fun(
+    inp_bound: constraints.JittableConstraint,
+    vertices: jnp.ndarray,
+    obj: jnp.ndarray,
+    fun_to_prop: Callable,
+) -> tuple[jnp.ndarray, jnp.ndarray]:
     (inp_bound,) = jax_verify.src.bound_propagation.unjit_inputs(inp_bound)
     linfuns = backward_crown_bound_propagation_linfun(
         lambda x: fun_to_prop(jnp.dot(x, vertices)), inp_bound, obj=obj
     )
     return linfuns[0].lin_coeffs, linfuns[0].offset
 
 
 @functools.partial(jax.jit, static_argnames=["fun_to_prop"])
-def bound_prop_fun(inp_bound, obj, fun_to_prop):
+def bound_prop_fun(
+    inp_bound: constraints.JittableConstraint,
+    obj: jnp.ndarray,
+    fun_to_prop: Callable,
+) -> tuple[jnp.ndarray, jnp.ndarray]:
     (inp_bound,) = jax_verify.src.bound_propagation.unjit_inputs(inp_bound)
     linfuns = backward_crown_bound_propagation_linfun(
         fun_to_prop, inp_bound, obj=obj
     )
     return linfuns[0].lin_coeffs, linfuns[0].offset
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopOVERTPropagator.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopOVERTPropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopPropagator.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopPropagator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,75 @@
 from copy import deepcopy
 from itertools import product
+from typing import Any, Optional
 
 import numpy as np
 from torch.multiprocessing import Pool
 
 import nfl_veripy.constraints as constraints
+import nfl_veripy.dynamics as dynamics
 
-from .Propagator import Propagator
 
-
-class ClosedLoopPropagator(Propagator):
+class ClosedLoopPropagator:
     def __init__(
         self,
-        input_shape=None,
-        dynamics=None,
-        boundary_type="rectangle",
-        num_polytope_facets=None,
+        dynamics: dynamics.Dynamics,
     ):
-        super().__init__(input_shape=input_shape)
         self.dynamics = dynamics
-        self.boundary_type = boundary_type
-        self.num_polytope_facets = num_polytope_facets
 
-    def get_one_step_reachable_set(self, input_constraint):
+        self.boundary_type: str = "rectangle"
+        self.num_polytope_facets: Optional[int] = None
+        self.num_iterations: int = 1
+
+    @property
+    def network(self):
+        return self._network
+
+    @network.setter
+    def network(self, network):
+        self._network = self.torch2network(network)
+
+    def get_one_step_reachable_set(
+        self, initial_set: constraints.SingleTimestepConstraint
+    ) -> tuple[constraints.SingleTimestepConstraint, dict]:
         raise NotImplementedError
 
-    def get_reachable_set(self, initial_set, t_max):
-        reachable_sets = []
-        info = {"per_timestep": []}
+    def get_reachable_set(
+        self,
+        initial_set: constraints.SingleTimestepConstraint,
+        t_max: int,
+    ) -> tuple[constraints.MultiTimestepConstraint, dict]:
+        reachable_sets_list = []
+        info = {"per_timestep": []}  # type: dict[str, Any]
         reachable_set, this_info = self.get_one_step_reachable_set(initial_set)
-        reachable_sets.append(deepcopy(reachable_set))
+        reachable_sets_list.append(deepcopy(reachable_set))
         info["per_timestep"].append(this_info)
         for i in np.arange(
             0 + self.dynamics.dt + 1e-10, t_max, self.dynamics.dt
         ):
             next_initial_set = deepcopy(reachable_set)
             reachable_set, this_info = self.get_one_step_reachable_set(
                 next_initial_set
             )
-            reachable_sets.append(deepcopy(reachable_set))
+            reachable_sets_list.append(deepcopy(reachable_set))
             info["per_timestep"].append(this_info)
 
-        reachable_sets = constraints.list_to_constraint(reachable_sets)
+        reachable_sets = constraints.list_to_constraint(reachable_sets_list)
 
         return reachable_sets, info
 
     def get_one_step_backprojection_set(
-        self, backreachable_set, target_sets, overapprox=False
-    ):
-        raise NotImplementedError
-
-    def get_backprojection_set(
-        self,
-        target_sets,
-        t_max,
-        num_partitions=None,
-        overapprox=False,
-        refined=False,
-        heuristic="guided",
-        all_lps=False,
-        slow_cvxpy=False,
-    ):
-        backprojection_set_list = []
-        tightened_infos_list = []
-        if not isinstance(target_sets, list):
-            target_set_list = [deepcopy(target_sets)]
-        else:
-            target_set_list = deepcopy(target_sets)
-
-        for target_set in target_set_list:
-            backprojection_sets, tightened_infos = (
-                self.get_single_target_backprojection_set(
-                    target_set,
-                    t_max=t_max,
-                    num_partitions=num_partitions,
-                    overapprox=overapprox,
-                    refined=refined,
-                )
-            )
-
-            backprojection_set_list.append(deepcopy(backprojection_sets))
-            tightened_infos_list.append(deepcopy(tightened_infos))
-
-        return backprojection_set_list, tightened_infos_list
-
-    def get_single_target_backprojection_set(
         self,
-        target_set,
-        t_max,
-        num_partitions=None,
-        overapprox=False,
-        refined=False,
-    ):
-        backprojection_set, info = self.get_one_step_backprojection_set(
-            target_set,
-            num_partitions=num_partitions,
-            overapprox=overapprox,
-            refined=refined,
-        )
-
-        return backprojection_set, info
+        backreachable_set: constraints.SingleTimestepConstraint,
+        target_sets: constraints.MultiTimestepConstraint,
+        overapprox: bool = False,
+        info: dict = {},
+        facet_inds_to_optimize: Optional[np.ndarray] = None,
+    ) -> tuple[Optional[constraints.SingleTimestepConstraint], dict]:
+        raise NotImplementedError
 
     def get_single_element_backprojection_set(
         self,
         oc,
         input_constraint,
         t_max,
         num_partitions=None,
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopSDPPropagator.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopSDPPropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopSeparablePropagator.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/ClosedLoopSeparablePropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/CrownIBP.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/CrownIBP.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/SDP.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/SDP.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/__init__.py` & `nfl_veripy-0.0.2/src/nfl_veripy/propagators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+from .AutoLIRPA import (
+    CROWNAutoLIRPAPropagator,
+    CROWNIBPAutoLIRPAPropagator,
+    ExhaustiveAutoLIRPAPropagator,
+    FastLinAutoLIRPAPropagator,
+    IBPAutoLIRPAPropagator,
+)
 from .ClosedLoopAUTOLIRPAPropagator import ClosedLoopAUTOLIRPAPropagator
 from .ClosedLoopCROWNIBPCodebasePropagator import (  # noqa
     ClosedLoopCROWNIBPCodebasePropagator,
     ClosedLoopCROWNLPPropagator,
     ClosedLoopCROWNNStepPropagator,
     ClosedLoopCROWNPropagator,
     ClosedLoopFastLinPropagator,
@@ -23,14 +30,17 @@
 from .ClosedLoopPropagator import ClosedLoopPropagator  # noqa
 from .ClosedLoopSDPPropagator import ClosedLoopSDPPropagator
 from .ClosedLoopSeparablePropagator import (
     ClosedLoopSeparableCROWNPropagator,
     ClosedLoopSeparableIBPPropagator,
     ClosedLoopSeparableSGIBPPropagator,
 )
+from .CrownIBP import CROWNPropagator, IBPPropagator
+from .Propagator import Propagator  # noqa
+from .SDP import SDPPropagator
 
 propagator_dict = {
     "CROWN": ClosedLoopCROWNPropagator,
     "CROWNNStep": ClosedLoopCROWNNStepPropagator,
     "CROWNLP": ClosedLoopCROWNLPPropagator,
     "IBP": ClosedLoopIBPPropagator,
     "FastLin": ClosedLoopFastLinPropagator,
@@ -52,24 +62,14 @@
     "JaxLP": ClosedLoopJaxLPPropagator,
     "JaxPolytopeJitted": ClosedLoopJaxPolytopeJittedPropagator,
     "JaxRectangleJitted": ClosedLoopJaxRectangleJittedPropagator,
     "JaxLPJitted": ClosedLoopJaxLPJittedPropagator,
     "AutoLiRPA": ClosedLoopAUTOLIRPAPropagator,
 }
 
-from .AutoLIRPA import (
-    CROWNAutoLIRPAPropagator,
-    CROWNIBPAutoLIRPAPropagator,
-    ExhaustiveAutoLIRPAPropagator,
-    FastLinAutoLIRPAPropagator,
-    IBPAutoLIRPAPropagator,
-)
-from .CrownIBP import CROWNPropagator, IBPPropagator
-from .Propagator import Propagator
-from .SDP import SDPPropagator
 
 open_loop_propagator_dict = {
     "IBP": IBPPropagator,
     "CROWN": CROWNPropagator,
     "CROWN_LIRPA": CROWNAutoLIRPAPropagator,
     "IBP_LIRPA": IBPAutoLIRPAPropagator,
     "CROWN-IBP_LIRPA": CROWNIBPAutoLIRPAPropagator,
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/alpha-beta-crown_test.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/alpha-beta-crown_test.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/closed_loop_verification_jax.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/closed_loop_verification_jax.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/controller_generation.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/controller_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import pickle
 
 import matplotlib.pyplot as plt
-import nfl_veripy.constraints as constraints
-import nfl_veripy.dynamics as dynamics
 import numpy as np
 import scipy.io
+import torch
+
+import nfl_veripy.constraints as constraints
+import nfl_veripy.dynamics as dynamics
 from nfl_veripy.utils.nn import (
     create_and_train_model,
     create_model,
     load_controller,
     save_model,
 )
 
@@ -323,25 +325,22 @@
         model,
         system="GroundRobotSI",
         model_name="buggy_complex_potential_field4",
     )
 
 
 def display_ground_robot_control_field(
-    name="avoid_origin_controller_simple", ax=None
-):
-    controller = load_controller(
-        system="GroundRobotSI", model_name=name, model_type="keras"
-    )
+    controller: torch.nn.Sequential, ax=None
+) -> None:
     x, y = np.meshgrid(np.linspace(-7.5, 4, 20), np.linspace(-7.2, 7.2, 20))
     # import pdb; pdb.set_trace()
     inputs = np.hstack(
         (x.reshape(len(x) * len(x[0]), 1), y.reshape(len(y) * len(y[0]), 1))
     )
-    us = controller.predict(inputs)
+    us = controller.forward(torch.Tensor(inputs)).detach().numpy()
 
     if ax is None:
         # import pdb; pdb.set_trace()
         plt.quiver(
             x,
             y,
             us[:, 0].reshape(len(x), len(y)),
```

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/create_training_dataset.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/create_training_dataset.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/debug_polytope.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/debug_polytope.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/debug_prop.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/debug_prop.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/duffing_data_generating.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/duffing_data_generating.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/generate_rpm_data.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/generate_rpm_data.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/iss_data_generating.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/iss_data_generating.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/mpc.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/mpc.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/nn.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_bounds.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/nn_bounds.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_closed_loop.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/nn_closed_loop.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_jax.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/nn_jax.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/optimization_utils.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/plot_rect_prism.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/plot_rect_prism.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/reach_sdp.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/reach_sdp.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/run_overt.jl` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/run_overt.jl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/utils.py` & `nfl_veripy-0.0.2/src/nfl_veripy/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,91 @@
+import logging
 import os
 import pickle
-import time
 
 import numpy as np
 import torch
 import torch.nn as nn
 from matplotlib import cm
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 
 
+def suppress_unecessary_logs():
+    logging.captureWarnings(True)
+
+    # https://github.com/google/jax/issues/6805
+    logging.getLogger("jax._src.xla_bridge").addFilter(
+        logging.Filter("No GPU/TPU found, falling back to CPU.")
+    )
+
+    # caused by matplotlib? should be fixed in v3.8.0 (not yet released)
+    logging.getLogger("py.warnings").addFilter(
+        logging.Filter("DeprecationWarning: pkg_resources is deprecated")
+    )
+    logging.getLogger("py.warnings").addFilter(
+        logging.Filter("DeprecationWarning: Deprecated call")
+    )
+
+    # caused by numpy??
+    logging.getLogger("numexpr.utils").addFilter(
+        logging.Filter("NumExpr defaulting to")
+    )
+
+
+def get_plot_filename(params):
+    this_file_dir = os.path.dirname(os.path.abspath(__file__))
+
+    if params["analysis"]["reachability_direction"] == "forward":
+        examples_dir = "examples"
+    else:
+        examples_dir = "examples_backward"
+    save_dir = f"{this_file_dir}/../../../results/{examples_dir}/"
+    os.makedirs(save_dir, exist_ok=True)
+
+    # Ugly logic to embed parameters in filename:
+    # pars = "_".join(
+    #     [
+    #         str(key) + "_" + str(value)
+    #         for key, value in sorted(
+    #             params["analysis"]["partitioner"].items(),
+    #             key=lambda kv: kv[0],
+    #         )
+    #         if key
+    #         not in [
+    #             "make_animation",
+    #             "show_animation",
+    #             "type",
+    #             "num_partitions",
+    #         ]
+    #     ]
+    # )
+    # pars2 = "_".join(
+    #     [
+    #         str(key) + "_" + str(value)
+    #         for key, value in sorted(
+    #             params["analysis"]["propagator"].items(),
+    #             key=lambda kv: kv[0],
+    #         )
+    #         if key not in ["input_shape", "type"]
+    #     ]
+    # )
+    plot_filename = f'{save_dir}/{params["system"]["type"]}_{params["system"]["feedback"]}_{params["analysis"]["partitioner"]["type"]}_{params["analysis"]["propagator"]["type"]}_tmax_{str(round(params["analysis"]["t_max"], 1))}_{params["analysis"]["propagator"]["boundary_type"]}'  # noqa: E501
+    plot_filename += ".png"
+    return plot_filename
+
+
 def bisect(input_range):
     return sect(input_range, num_sects=2)
 
 
 def sect(input_range, num_sects=3, select="random"):
     input_shape = input_range.shape[:-1]
     if select == "random":
-        # doesnt work
-        input_dim_to_sect = np.random.randint(0, num_inputs)
+        raise NotImplementedError
     else:
         lengths = input_range[..., 1] - input_range[..., 0]
         input_dim_to_sect = np.unravel_index(lengths.argmax(), lengths.shape)
     input_ranges = np.tile(
         input_range,
         (num_sects,) + tuple([1 for _ in range(len(input_shape) + 1)]),
     )
@@ -33,18 +96,20 @@
     for i in range(num_sects - 1):
         new_endpt = input_range[input_dim_to_sect + (0,)] + (i + 1) * diff
         input_ranges[(i,) + input_dim_to_sect + (1,)] = new_endpt
         input_ranges[(i + 1,) + input_dim_to_sect + (0,)] = new_endpt
     return input_ranges
 
 
-def get_sampled_outputs(input_range, propagator, N=1000):
+def get_sampled_outputs(
+    input_range: np.ndarray, propagator, num_samples: int = 1000
+) -> np.ndarray:
     input_shape = input_range.shape[:-1]
     sampled_inputs = np.random.uniform(
-        input_range[..., 0], input_range[..., 1], (N,) + input_shape
+        input_range[..., 0], input_range[..., 1], (num_samples,) + input_shape
     )
 
     sampled_outputs = propagator.forward_pass(sampled_inputs)
 
     return sampled_outputs
 
 
@@ -65,15 +130,15 @@
     # with tf.compat.v1.Session() as sess:
     # init = tf.global_variables_initializer()
     # sess.run(init)
     for i in range(len(w_tsr)):
         w = good_sess.run(w_tsr[i]).T
         b = good_sess.run(b_tsr[i])
         linear = torch.nn.Linear(w.shape[1], w.shape[0])
-        # print("Layer {}: Input: {}, Output: {}".format(i, w.shape[1], w.shape[0]))
+        # print(f"Layer {i}: Input: {w.shape[1]}, Output: {w.shape[0]}")
         # print("Bias {}: shape: {}".format(b, b.shape))
         # print(w)
         # import pdb; pdb.set_trace()
         linear.weight.data.copy_(torch.Tensor(w))
         linear.bias.data.copy_(torch.Tensor(b))
         modules.append(linear)
         if i < len(w_tsr) - 1:
```

### Comparing `nfl_veripy-0.0.1a4/tests/test.py` & `nfl_veripy-0.0.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/.gitignore` & `nfl_veripy-0.0.2/.gitignore`

 * *Files 21% similar despite different names*

```diff
@@ -35,8 +35,9 @@
 models/nnet/
 models/unity/
 datasets/DoubleIntegrator/
 datasets/Unity/
 
 nn_partition/models/nnet/
 
-venv*
+venv*
+.vscode
```

### Comparing `nfl_veripy-0.0.1a4/LICENSE` & `nfl_veripy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1a4/README.md` & `nfl_veripy-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,51 @@
+# nfl_veripy: Formal Verification of Neural Feedback Loops (NFLs)
+
 ## Updates
 
-- **2023-04-19:** Major cleanup and re-branding of repo, released PyPi package for easier usability!
+- **2023-07-20:** Added typing hints and re-factored visualization code as separate from other components.
+- **2023-04-21:** Major cleanup and re-branding of repo, released PyPi package for easier usability!
 - **2023-04-13:** Add new jax-based propagators, including some from [`DRIP` paper](https://arxiv.org/abs/2212.04646). Cleaned up implementation of BReach-LP and HyBReach-LP from OJCSYS paper.
 - **2022-06-20:** Add new backprojection code from [`BReach-LP` paper](https://arxiv.org/abs/2204.08319). More info [here](/docs/_static/cdc22/cdc22.md)
 - **2022-05-09:** Add new N-Step `ClosedLoopPropagator`. Rather than recursively computing reachable sets (suffers from the wrapping effect), we see improved performance by solving an LP directly for the reachable set N steps in the future. You can experiment with this using the `CROWNNStep` flag in `nfl_veripy/example.py`.
 - **2022-05-09:** Add new MILP-based `ClosedLoopPropagator`, using [`OVERT`](https://github.com/sisl/OVERTVerify.jl). Note that this component requires a Julia installation, and we pass data between Python and Julia using a lightweight local HTTP server. More info [here](/docs/_static/other.md).
 
 ## About
 
-### `nfl_veripy`: Closed-Loop Analysis (NNs in feedback loops) -- includes Reach-LP and BReach-LP
+`nfl_veripy` is a Python codebase for formal safety verification of neural feedback loops (NFLs).
+An example of an NFL is a dynamical system controlled by a neural network policy.
 
-**Handles problems such as:**
+Currently, **`nfl_veripy` handles problems such as:**
 - Given a set of possible initial states, a trained NN controller, and a known dynamics model, compute outer bounds on the set of possible future states (**forward reachable sets**).
 - Given a set of terminal states, a trained NN controller, and a known dynamics model, compute inner/outer bounds on the set of possible initial states that will/won't lead to the terminal state set (**backprojection sets**).
 
 For more info, please see [this README](/docs/_static/access21/access21.md) and [this README](/docs/_static/cdc22/cdc22.md).
 
 ## Setup
 
 If you just want to run the code, you can simply install our package via pip:
 ```bash
-pip install "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" \
-    "crown_ibp @ git+https://gitlab.com/mit-acl/ford_ugvs/crown_ibp.git" \
+pip install \
+    "jax_verify @ git+https://gitlab.com/neu-autonomy/certifiable-learning/jax_verify.git" \
+    "crown_ibp @ git+https://gitlab.com/neu-autonomy/certifiable-learning/crown_ibp.git" \
     nfl_veripy
 ```
 
-Aside: We acknowledge that the above method for installing `jax_verify` and `crown_ibp` (dependencies of `nfl_veripy`) in the above way is a little unconventional.
-It would be better to simply include these as dependencies of `nfl_veripy` and let pip find those packages, but (a) those packages are not available (or are too outdated) on PyPI, and (b) it is not allowed to include dependencies with direct URLs when releasing a package on PyPI.
-If there's a better way of doing this we would love to hear about it!
-
 ### Simple Examples
 
 Compute forward reachable sets for a closed-loop system with a pre-trained NN control policy:
 ```bash
 python -m nfl_veripy.example --config example_configs/icra21/fig3_reach_lp.yaml
 ```
 
 Compute backward reachable sets for a closed-loop system with a pre-trained NN control policy:
 ```bash
 python -m nfl_veripy.example --config example_configs/ojcsys23/di_breach.yaml
 ```
 
-### Jupyter Notebooks
-
-Please see the `jupyter_notebooks` folder for an interactive version of the above examples.
-
 ### Replicate plots from the papers:
 
 * LCSS/ACC '21: [README](/docs/_static/lcss21/lcss21.md)
 * ICRA '21: [README](/docs/_static/icra21/icra21.md)
 * IEEE Access '21: [README](/docs/_static/access21/access21.md)
 * CDC '22: [README](/docs/_static/cdc22/cdc22.md)
 * ACC '23 (to appear): Coming soon!
@@ -65,30 +62,23 @@
 * Rober, N., Everett, M., Zhang, S., & How, J. P. (2022). A Hybrid Partitioning Strategy for Backward Reachability of Neural Feedback Loops. arXiv preprint arXiv:2210.07918.
 * Rober, N., Katz, S. M., Sidrane, C., Yel, E., Everett, M., Kochenderfer, M. J., & How, J. P. (2023). Backward reachability analysis of neural feedback loops: Techniques for linear and nonlinear systems. IEEE Open Journal of Control Systems.
 * Everett, M., Bunel, R., & Omidshafiei, S. (2023). Drip: Domain refinement iteration with polytopes for backward reachability analysis of neural feedback loops. IEEE Control Systems Letters.
 
 
 ## Acknowledgements
 
-This research is supported in part by Ford Motor Company.
+This research was supported in part by Ford Motor Company.
 
 We build on excellent open-source repositories from the neural network analysis community. These repositories are imported as Git submodules or re-implemented in Python here, with some changes to reflect the slightly different problem statements:
 * [`auto_LIRPA`](https://github.com/KaidiXu/auto_LiRPA)
 * [`crown_ibp`](https://github.com/huanzhang12/CROWN-IBP)
 * [`robust_nn`](https://github.com/arobey1/RobustNN)
 * [`nnv`](https://github.com/verivital/nnv)
 * [`jax_verify`](https://github.com/deepmind/jax_verify)
 
-
-## TODOS:
-
-- [ ] add rtdocs (auto-fill code snippets from test files)
-- [ ] add installation instructions & tests for julia code
-
-
 ## Developer Setup
 
 If you want to work directly with the source code, here is how we set up our development environments.
 
 ### Get the code
 
 ```bash
@@ -106,23 +96,14 @@
 ```bash
 python -m virtualenv venv
 source venv/bin/activate
 ```
 
 Install the various python packages in this repo in editable mode (`-e`):
 ```bash
-python -m pip install -e third_party/crown_ibp third_party/jax_verify third_party/auto_LiRPA .
+python -m pip install -e third_party/crown_ibp
+python -m pip install -e third_party/jax_verify
+python -m pip install -e third_party/auto_LiRPA
+python -m pip install -e .
 ```
 
-You're good to go!
-
-## packaging info
-
-```bash
-cd nfl_veripy
-python -m build
-python -m twine upload --repository testpypi dist/nfl_veripy-0.0.1a0*
-
-python -m pip install "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" "crown_ibp @ git+https://gitlab.com/mit-acl/ford_ugvs/crown_ibp.git"
-python -m pip install --extra-index-url https://test.pypi.org/simple/ nfl-veripy==0.0.1.a3
-
-```
+You're good to go!
```

### Comparing `nfl_veripy-0.0.1a4/PKG-INFO` & `nfl_veripy-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nfl_veripy
-Version: 0.0.1a4
-Summary: A small example package
-Project-URL: repository, https://github.com/mit-acl/nn_robustness_analysis.git
+Version: 0.0.2
+Summary: Formal verification of neural feedback loops (NFLs)
+Project-URL: repository, https://github.com/neu-autonomy/nfl_veripy.git
 Author-email: Michael Everett <m.everett@northeastern.edu>, Nicholas Rober <nrober@mit.edu>
 License: MIT License
         
         Copyright (c) 2021 MIT Aerospace Controls Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -34,73 +34,72 @@
 Requires-Dist: auto-lirpa
 Requires-Dist: colour
 Requires-Dist: crown-ibp
 Requires-Dist: imageio
 Requires-Dist: jax
 Requires-Dist: jax-verify
 Requires-Dist: matplotlib
+Requires-Dist: mypy
 Requires-Dist: pandas
 Requires-Dist: parameterized
 Requires-Dist: pyclipper
 Requires-Dist: pygifsicle
+Requires-Dist: pylint
 Requires-Dist: pypoman
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tabulate
 Requires-Dist: torch
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
+# nfl_veripy: Formal Verification of Neural Feedback Loops (NFLs)
+
 ## Updates
 
-- **2023-04-19:** Major cleanup and re-branding of repo, released PyPi package for easier usability!
+- **2023-07-20:** Added typing hints and re-factored visualization code as separate from other components.
+- **2023-04-21:** Major cleanup and re-branding of repo, released PyPi package for easier usability!
 - **2023-04-13:** Add new jax-based propagators, including some from [`DRIP` paper](https://arxiv.org/abs/2212.04646). Cleaned up implementation of BReach-LP and HyBReach-LP from OJCSYS paper.
 - **2022-06-20:** Add new backprojection code from [`BReach-LP` paper](https://arxiv.org/abs/2204.08319). More info [here](/docs/_static/cdc22/cdc22.md)
 - **2022-05-09:** Add new N-Step `ClosedLoopPropagator`. Rather than recursively computing reachable sets (suffers from the wrapping effect), we see improved performance by solving an LP directly for the reachable set N steps in the future. You can experiment with this using the `CROWNNStep` flag in `nfl_veripy/example.py`.
 - **2022-05-09:** Add new MILP-based `ClosedLoopPropagator`, using [`OVERT`](https://github.com/sisl/OVERTVerify.jl). Note that this component requires a Julia installation, and we pass data between Python and Julia using a lightweight local HTTP server. More info [here](/docs/_static/other.md).
 
 ## About
 
-### `nfl_veripy`: Closed-Loop Analysis (NNs in feedback loops) -- includes Reach-LP and BReach-LP
+`nfl_veripy` is a Python codebase for formal safety verification of neural feedback loops (NFLs).
+An example of an NFL is a dynamical system controlled by a neural network policy.
 
-**Handles problems such as:**
+Currently, **`nfl_veripy` handles problems such as:**
 - Given a set of possible initial states, a trained NN controller, and a known dynamics model, compute outer bounds on the set of possible future states (**forward reachable sets**).
 - Given a set of terminal states, a trained NN controller, and a known dynamics model, compute inner/outer bounds on the set of possible initial states that will/won't lead to the terminal state set (**backprojection sets**).
 
 For more info, please see [this README](/docs/_static/access21/access21.md) and [this README](/docs/_static/cdc22/cdc22.md).
 
 ## Setup
 
 If you just want to run the code, you can simply install our package via pip:
 ```bash
-pip install "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" \
-    "crown_ibp @ git+https://gitlab.com/mit-acl/ford_ugvs/crown_ibp.git" \
+pip install \
+    "jax_verify @ git+https://gitlab.com/neu-autonomy/certifiable-learning/jax_verify.git" \
+    "crown_ibp @ git+https://gitlab.com/neu-autonomy/certifiable-learning/crown_ibp.git" \
     nfl_veripy
 ```
 
-Aside: We acknowledge that the above method for installing `jax_verify` and `crown_ibp` (dependencies of `nfl_veripy`) in the above way is a little unconventional.
-It would be better to simply include these as dependencies of `nfl_veripy` and let pip find those packages, but (a) those packages are not available (or are too outdated) on PyPI, and (b) it is not allowed to include dependencies with direct URLs when releasing a package on PyPI.
-If there's a better way of doing this we would love to hear about it!
-
 ### Simple Examples
 
 Compute forward reachable sets for a closed-loop system with a pre-trained NN control policy:
 ```bash
 python -m nfl_veripy.example --config example_configs/icra21/fig3_reach_lp.yaml
 ```
 
 Compute backward reachable sets for a closed-loop system with a pre-trained NN control policy:
 ```bash
 python -m nfl_veripy.example --config example_configs/ojcsys23/di_breach.yaml
 ```
 
-### Jupyter Notebooks
-
-Please see the `jupyter_notebooks` folder for an interactive version of the above examples.
-
 ### Replicate plots from the papers:
 
 * LCSS/ACC '21: [README](/docs/_static/lcss21/lcss21.md)
 * ICRA '21: [README](/docs/_static/icra21/icra21.md)
 * IEEE Access '21: [README](/docs/_static/access21/access21.md)
 * CDC '22: [README](/docs/_static/cdc22/cdc22.md)
 * ACC '23 (to appear): Coming soon!
@@ -117,30 +116,23 @@
 * Rober, N., Everett, M., Zhang, S., & How, J. P. (2022). A Hybrid Partitioning Strategy for Backward Reachability of Neural Feedback Loops. arXiv preprint arXiv:2210.07918.
 * Rober, N., Katz, S. M., Sidrane, C., Yel, E., Everett, M., Kochenderfer, M. J., & How, J. P. (2023). Backward reachability analysis of neural feedback loops: Techniques for linear and nonlinear systems. IEEE Open Journal of Control Systems.
 * Everett, M., Bunel, R., & Omidshafiei, S. (2023). Drip: Domain refinement iteration with polytopes for backward reachability analysis of neural feedback loops. IEEE Control Systems Letters.
 
 
 ## Acknowledgements
 
-This research is supported in part by Ford Motor Company.
+This research was supported in part by Ford Motor Company.
 
 We build on excellent open-source repositories from the neural network analysis community. These repositories are imported as Git submodules or re-implemented in Python here, with some changes to reflect the slightly different problem statements:
 * [`auto_LIRPA`](https://github.com/KaidiXu/auto_LiRPA)
 * [`crown_ibp`](https://github.com/huanzhang12/CROWN-IBP)
 * [`robust_nn`](https://github.com/arobey1/RobustNN)
 * [`nnv`](https://github.com/verivital/nnv)
 * [`jax_verify`](https://github.com/deepmind/jax_verify)
 
-
-## TODOS:
-
-- [ ] add rtdocs (auto-fill code snippets from test files)
-- [ ] add installation instructions & tests for julia code
-
-
 ## Developer Setup
 
 If you want to work directly with the source code, here is how we set up our development environments.
 
 ### Get the code
 
 ```bash
@@ -158,23 +150,14 @@
 ```bash
 python -m virtualenv venv
 source venv/bin/activate
 ```
 
 Install the various python packages in this repo in editable mode (`-e`):
 ```bash
-python -m pip install -e third_party/crown_ibp third_party/jax_verify third_party/auto_LiRPA .
+python -m pip install -e third_party/crown_ibp
+python -m pip install -e third_party/jax_verify
+python -m pip install -e third_party/auto_LiRPA
+python -m pip install -e .
 ```
 
-You're good to go!
-
-## packaging info
-
-```bash
-cd nfl_veripy
-python -m build
-python -m twine upload --repository testpypi dist/nfl_veripy-0.0.1a0*
-
-python -m pip install "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" "crown_ibp @ git+https://gitlab.com/mit-acl/ford_ugvs/crown_ibp.git"
-python -m pip install --extra-index-url https://test.pypi.org/simple/ nfl-veripy==0.0.1.a3
-
-```
+You're good to go!
```

