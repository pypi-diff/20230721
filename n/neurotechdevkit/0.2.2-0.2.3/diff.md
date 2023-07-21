# Comparing `tmp/neurotechdevkit-0.2.2.tar.gz` & `tmp/neurotechdevkit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurotechdevkit-0.2.2.tar", max compression
+gzip compressed data, was "neurotechdevkit-0.2.3.tar", max compression
```

## Comparing `neurotechdevkit-0.2.2.tar` & `neurotechdevkit-0.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11339 2023-07-20 06:30:37.803152 neurotechdevkit-0.2.2/LICENSE
--rw-r--r--   0        0        0     4034 2023-07-20 06:30:37.927153 neurotechdevkit-0.2.2/docs/index.md
--rw-r--r--   0        0        0     2217 2023-07-20 06:30:53.699297 neurotechdevkit-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2432 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/__init__.py
--rw-r--r--   0        0        0     4777 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/materials.py
--rw-r--r--   0        0        0     1162 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/__init__.py
--rw-r--r--   0        0        0     4747 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/_animations.py
--rw-r--r--   0        0        0     2304 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/_formatting.py
--rw-r--r--   0        0        0     8996 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/_source.py
--rw-r--r--   0        0        0     3485 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/_target.py
--rw-r--r--   0        0        0    49858 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/colormaps.py
--rw-r--r--   0        0        0     2307 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=10°.png
--rw-r--r--   0        0        0    30101 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=120°.png
--rw-r--r--   0        0        0    50607 2023-07-20 06:30:37.931153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=150°.png
--rw-r--r--   0        0        0    61496 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=180°.png
--rw-r--r--   0        0        0     4467 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=20°.png
--rw-r--r--   0        0        0      715 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=2°.png
--rw-r--r--   0        0        0     8691 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=40°.png
--rw-r--r--   0        0        0     1147 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=5°.png
--rw-r--r--   0        0        0    12673 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=60°.png
--rw-r--r--   0        0        0    20015 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=90°.png
--rw-r--r--   0        0        0     2753 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=Flat.png
--rw-r--r--   0        0        0     3377 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/target-dark.png
--rw-r--r--   0        0        0     3598 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/target-light.png
--rw-r--r--   0        0        0      722 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/font.py
--rw-r--r--   0        0        0    96364 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
--rw-r--r--   0        0        0    97116 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
--rw-r--r--   0        0        0    96304 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
--rw-r--r--   0        0        0    96312 2023-07-20 06:30:37.935153 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
--rw-r--r--   0        0        0    96492 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
--rw-r--r--   0        0        0    96412 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
--rw-r--r--   0        0        0    96528 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
--rw-r--r--   0        0        0     4314 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/layers.py
--rw-r--r--   0        0        0     5561 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/layout.py
--rw-r--r--   0        0        0     6290 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/legends.py
--rw-r--r--   0        0        0     7575 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/napari.py
--rw-r--r--   0        0        0     8880 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/simulations.py
--rw-r--r--   0        0        0      593 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/results/__init__.py
--rw-r--r--   0        0        0    13017 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/results/_metrics.py
--rw-r--r--   0        0        0    53469 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/results/_results.py
--rw-r--r--   0        0        0      620 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/__init__.py
--rw-r--r--   0        0        0    43604 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_base.py
--rw-r--r--   0        0        0     9234 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_resources.py
--rw-r--r--   0        0        0     4800 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_scenario_0.py
--rw-r--r--   0        0        0     8297 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_scenario_1.py
--rw-r--r--   0        0        0    11365 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_scenario_2.py
--rw-r--r--   0        0        0     7378 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_shots.py
--rw-r--r--   0        0        0     4559 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_time.py
--rw-r--r--   0        0        0    11913 2023-07-20 06:30:37.939154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_utils.py
--rw-r--r--   0        0        0  2195183 2023-07-20 06:30:37.951154 neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
--rw-r--r--   0        0        0    55819 2023-07-20 06:30:37.955154 neurotechdevkit-0.2.2/src/neurotechdevkit/sources.py
--rw-r--r--   0        0        0     5507 1970-01-01 00:00:00.000000 neurotechdevkit-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-07-21 06:29:00.766273 neurotechdevkit-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4034 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/docs/index.md
+-rw-r--r--   0        0        0     2217 2023-07-21 06:29:12.214260 neurotechdevkit-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2432 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/__init__.py
+-rw-r--r--   0        0        0     4777 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/materials.py
+-rw-r--r--   0        0        0     1162 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/__init__.py
+-rw-r--r--   0        0        0     4747 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/_animations.py
+-rw-r--r--   0        0        0     2304 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/_formatting.py
+-rw-r--r--   0        0        0     8996 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/_source.py
+-rw-r--r--   0        0        0     3485 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/_target.py
+-rw-r--r--   0        0        0    49858 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/colormaps.py
+-rw-r--r--   0        0        0     2307 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=10°.png
+-rw-r--r--   0        0        0    30101 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=120°.png
+-rw-r--r--   0        0        0    50607 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=150°.png
+-rw-r--r--   0        0        0    61496 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=180°.png
+-rw-r--r--   0        0        0     4467 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=20°.png
+-rw-r--r--   0        0        0      715 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=2°.png
+-rw-r--r--   0        0        0     8691 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=40°.png
+-rw-r--r--   0        0        0     1147 2023-07-21 06:29:00.886272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=5°.png
+-rw-r--r--   0        0        0    12673 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=60°.png
+-rw-r--r--   0        0        0    20015 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=90°.png
+-rw-r--r--   0        0        0     2753 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=Flat.png
+-rw-r--r--   0        0        0     3377 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/target-dark.png
+-rw-r--r--   0        0        0     3598 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/target-light.png
+-rw-r--r--   0        0        0      722 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/font.py
+-rw-r--r--   0        0        0    96364 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
+-rw-r--r--   0        0        0    97116 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
+-rw-r--r--   0        0        0    96304 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
+-rw-r--r--   0        0        0    96312 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
+-rw-r--r--   0        0        0    96492 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
+-rw-r--r--   0        0        0    96412 2023-07-21 06:29:00.890272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
+-rw-r--r--   0        0        0    96528 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
+-rw-r--r--   0        0        0     4314 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/layers.py
+-rw-r--r--   0        0        0     5561 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/layout.py
+-rw-r--r--   0        0        0     6290 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/legends.py
+-rw-r--r--   0        0        0     7575 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/napari.py
+-rw-r--r--   0        0        0     8880 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/simulations.py
+-rw-r--r--   0        0        0      593 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/results/__init__.py
+-rw-r--r--   0        0        0    13017 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/results/_metrics.py
+-rw-r--r--   0        0        0    53469 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/results/_results.py
+-rw-r--r--   0        0        0      620 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/__init__.py
+-rw-r--r--   0        0        0    43604 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_base.py
+-rw-r--r--   0        0        0     9234 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_resources.py
+-rw-r--r--   0        0        0     4801 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_scenario_0.py
+-rw-r--r--   0        0        0     8297 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_scenario_1.py
+-rw-r--r--   0        0        0    11365 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_scenario_2.py
+-rw-r--r--   0        0        0     7378 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_shots.py
+-rw-r--r--   0        0        0     4559 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_time.py
+-rw-r--r--   0        0        0    11913 2023-07-21 06:29:00.894272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_utils.py
+-rw-r--r--   0        0        0  2195183 2023-07-21 06:29:00.906272 neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
+-rw-r--r--   0        0        0    55819 2023-07-21 06:29:00.906272 neurotechdevkit-0.2.3/src/neurotechdevkit/sources.py
+-rw-r--r--   0        0        0     5507 1970-01-01 00:00:00.000000 neurotechdevkit-0.2.3/PKG-INFO
```

### Comparing `neurotechdevkit-0.2.2/LICENSE` & `neurotechdevkit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/docs/index.md` & `neurotechdevkit-0.2.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/pyproject.toml` & `neurotechdevkit-0.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neurotechdevkit"
-version = "v0.2.2"
+version = "v0.2.3"
 description = "Neurotech Development Kit: an open-source software library designed to enhance accessibility to cutting-edge neurotechnology"
 authors = ["AE Studio <bci@ae.studio>"]
 maintainers = ["AE Studio <bci@ae.studio>"]
 packages = [{include = "neurotechdevkit", from = "src" }]
 
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/__init__.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/materials.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/materials.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/__init__.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/_animations.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/_animations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/_formatting.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/_formatting.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/_source.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/_source.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/_target.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/_target.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/colormaps.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/colormaps.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=10°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=10°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=120°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=120°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=150°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=150°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=180°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=180°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=20°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=20°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=2°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=2°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=40°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=40°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=5°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=5°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=60°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=60°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=90°.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=90°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/Angle=Flat.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/Angle=Flat.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/target-dark.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/target-dark.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/components/target-light.png` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/components/target-light.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/font.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/font.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/layers.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/layers.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/layout.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/layout.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/legends.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/legends.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/napari.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/napari.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/rendering/simulations.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/rendering/simulations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/results/__init__.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/results/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/results/_metrics.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/results/_metrics.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/results/_results.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/results/_results.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/__init__.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_base.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_base.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_resources.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_resources.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_scenario_0.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_scenario_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def _get_material_masks(self, problem):
         return {
             name: _create_scenario_0_mask(name, problem.grid, self._origin)
             for name in self.material_layers
         }
 
-    def _compile_problem(self, center_frequency=float) -> stride.Problem:
+    def _compile_problem(self, center_frequency: float) -> stride.Problem:
         extent = np.array([0.05, 0.04])  # m
         origin = self.origin  # m
 
         # scenario constants
         speed_water = 1500  # m/s
 
         # desired resolution for complexity=fast
```

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_scenario_1.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_scenario_1.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_scenario_2.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_scenario_2.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_shots.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_shots.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_time.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_time.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/_utils.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/_utils.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat` & `neurotechdevkit-0.2.3/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/src/neurotechdevkit/sources.py` & `neurotechdevkit-0.2.3/src/neurotechdevkit/sources.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.2.2/PKG-INFO` & `neurotechdevkit-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurotechdevkit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Neurotech Development Kit: an open-source software library designed to enhance accessibility to cutting-edge neurotechnology
 License: Apache-2.0
 Author: AE Studio
 Author-email: bci@ae.studio
 Maintainer: AE Studio
 Maintainer-email: bci@ae.studio
 Requires-Python: >=3.9,<3.12
```

