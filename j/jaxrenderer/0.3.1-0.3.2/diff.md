# Comparing `tmp/jaxrenderer-0.3.1.tar.gz` & `tmp/jaxrenderer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrenderer-0.3.1.tar", max compression
+gzip compressed data, was "jaxrenderer-0.3.2.tar", max compression
```

## Comparing `jaxrenderer-0.3.1.tar` & `jaxrenderer-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11367 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/LICENSE
--rw-r--r--   0        0        0     2312 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/README.md
--rw-r--r--   0        0        0     6059 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/changelog.md
--rw-r--r--   0        0        0     1683 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5637 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/README.md
--rw-r--r--   0        0        0      539 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/__init__.py
--rw-r--r--   0        0        0     1342 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/_backport.py
--rw-r--r--   0        0        0      764 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/_meta_utils.py
--rw-r--r--   0        0        0    35017 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/geometry.py
--rw-r--r--   0        0        0    17560 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/model.py
--rw-r--r--   0        0        0    17577 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/pipeline.py
--rw-r--r--   0        0        0    14697 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/renderer.py
--rw-r--r--   0        0        0     9561 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/scene.py
--rw-r--r--   0        0        0    14672 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/shader.py
--rw-r--r--   0        0        0     4600 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/README.md
--rw-r--r--   0        0        0     1453 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/depth.py
--rw-r--r--   0        0        0     3493 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/gouraud.py
--rw-r--r--   0        0        0     5089 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/gouraud_texture.py
--rw-r--r--   0        0        0     5364 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/phong.py
--rw-r--r--   0        0        0     9900 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/phong_darboux.py
--rw-r--r--   0        0        0     8115 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/phong_reflection.py
--rw-r--r--   0        0        0     9839 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/phong_reflection_shadow.py
--rw-r--r--   0        0        0     4517 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shadow.py
--rw-r--r--   0        0        0    71549 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shapes/capsule.py
--rw-r--r--   0        0        0     3574 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shapes/cube.py
--rw-r--r--   0        0        0     3588 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/types.py
--rw-r--r--   0        0        0     3364 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/utils.py
--rw-r--r--   0        0        0      833 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/value_checker.py
--rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 jaxrenderer-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11367 2023-07-21 19:18:02.141521 jaxrenderer-0.3.2/LICENSE
+-rw-r--r--   0        0        0     9748 2023-07-21 19:18:02.141521 jaxrenderer-0.3.2/README.md
+-rw-r--r--   0        0        0     6515 2023-07-21 19:18:02.141521 jaxrenderer-0.3.2/changelog.md
+-rw-r--r--   0        0        0     2957 2023-07-21 19:18:02.445522 jaxrenderer-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5637 2023-07-21 19:18:02.445522 jaxrenderer-0.3.2/renderer/README.md
+-rw-r--r--   0        0        0     1564 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/__init__.py
+-rw-r--r--   0        0        0     1628 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/_backport.py
+-rw-r--r--   0        0        0     1950 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/_meta_utils.py
+-rw-r--r--   0        0        0    37956 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/geometry.py
+-rw-r--r--   0        0        0    18971 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/model.py
+-rw-r--r--   0        0        0    18949 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/pipeline.py
+-rw-r--r--   0        0        0    17433 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/renderer.py
+-rw-r--r--   0        0        0    10452 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/scene.py
+-rw-r--r--   0        0        0    15484 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shader.py
+-rw-r--r--   0        0        0     4602 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shaders/README.md
+-rw-r--r--   0        0        0     1615 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shaders/depth.py
+-rw-r--r--   0        0        0     3943 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shaders/gouraud.py
+-rw-r--r--   0        0        0     5635 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shaders/gouraud_texture.py
+-rw-r--r--   0        0        0     6329 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shaders/phong.py
+-rw-r--r--   0        0        0    11204 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shaders/phong_darboux.py
+-rw-r--r--   0        0        0     9061 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shaders/phong_reflection.py
+-rw-r--r--   0        0        0    10872 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shaders/phong_reflection_shadow.py
+-rw-r--r--   0        0        0     4728 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shadow.py
+-rw-r--r--   0        0        0    79649 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shapes/capsule.py
+-rw-r--r--   0        0        0     4399 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/shapes/cube.py
+-rw-r--r--   0        0        0     4997 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/types.py
+-rw-r--r--   0        0        0     4028 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/utils.py
+-rw-r--r--   0        0        0     1037 2023-07-21 19:18:02.449522 jaxrenderer-0.3.2/renderer/value_checker.py
+-rw-r--r--   0        0        0    11452 1970-01-01 00:00:00.000000 jaxrenderer-0.3.2/PKG-INFO
```

### Comparing `jaxrenderer-0.3.1/LICENSE` & `jaxrenderer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.1/changelog.md` & `jaxrenderer-0.3.2/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -48,17 +48,25 @@
 ## 0.2.1
 
 1. Refactor `Scene.set_object_*` methods to be a simple wrapper of `self._replace` and `ModelObject.replace_with_*`, to expose APIs of `ModelObject`s and allows manipulation and rendering without `Scene`.
 2. Expose `create_capsule` and `create_cube` APIs.
 
 ## 0.3.0
 
-1. Fix `gl_FrontFacing` computation in pipeline so it is consistent to comment: `True` if not backfacing (i.e. frontfacing & side facing).
+1. Fix `gl_FrontFacing` computation in pipeline so it is consistent to comment: `True` if not back-facing (i.e. front-facing & side facing).
 2. Add an extra stage `Shader.primitive_chooser` to choose which primitive to be rendered for each fragment. The default implementation is provided, which assumes that the depth is just the interpolated `z` value in the eye space. It just picks the values of the single primitive that is closest to the camera and is not discarded in the previous pipeline.
-3. Expose `loop_unroll` static option to allow unrolling several operations (row rendering) within a single iteration of the outmost loop (iterating along first axis of the canvas). This may be useful in some cases for performance improvement, but careful benchmarking is needed to determine the optimal value. The default value is `1` (no unrolling) as it is the most general case in larger canvases (benchmarked on `960x540` using [GPU T4 in Colab](https://colab.research.google.com/drive/1xhkYNz5WjvUCjQWpp72CLf9SIy3i5PnN)).
+3. Expose `loop_unroll` static option to allow unrolling several operations (row rendering) within a single iteration of the out-most loop (iterating along first axis of the canvas). This may be useful in some cases for performance improvement, but careful benchmarking is needed to determine the optimal value. The default value is `1` (no unrolling) as it is the most general case in larger canvases (benchmarked on `960x540` using [GPU T4 in Colab](https://colab.research.google.com/drive/1xhkYNz5WjvUCjQWpp72CLf9SIy3i5PnN)).
 4. Bump the minimum Python version to Python 3.10
 5. Lower the minimum jax & jaxlib version to 0.3.25.
 
 ## 0.3.1
 
 1. Lower minimum Python version to 3.8
 2. Introducing `type_extensions` package and improved typing annotations.
+
+## 0.3.2
+
+1. Bump minimum `jax` and `jaxlib` version to 0.4.0 as `jaxtyping` does not support `jax` 0.3.25.
+2. Bug fix: add `static_argnames` for utility function `transpose_for_display`.
+3. Change to [isort](https://github.com/PyCQA/isort) + [black](https://github.com/psf/black) code style.
+4. Migrate full codebase to be type-checked with [pyright](https://github.com/microsoft/pyright).
+5. Add smoke tests, and use GitHub Action as CI to run them.
```

### Comparing `jaxrenderer-0.3.1/pyproject.toml` & `jaxrenderer-0.3.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaxrenderer"
-version = "0.3.1"
+version = "0.3.2"
 description = "Jax implementation of rasterizer renderer."
 authors = ["Joey Teng <joey.teng.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JoeyTeng/jaxrenderer"
 repository = "https://github.com/JoeyTeng/jaxrenderer"
 classifiers = [
@@ -29,37 +29,89 @@
     "changelog.md",
     "pyproject.toml",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-jax = ">=0.3.25,<5.0.0"
+jax = "^0.4.0"
 numpy = "^1.22.0"
-jaxlib = {version = ">=0.3.25,<5.0.0", source = "jax"}
+jaxlib = {version = "^0.4.0", source = "jax"}
 jaxtyping = [
     {version = ">=0.2.13,<0.2.20", python = ">=3.8,<3.9"},
     {version = "^0.2.19", python = "^3.9"}
 ]
 importlib-metadata = "^6.6.0"
 typing_extensions = "^4.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.6.2"
 pillow = "^9.4.0"
 importlib-resources = "^5.12.0"
 
 
+[tool.poetry.group.test.dependencies]
+pre-commit = "^3.3.3"
+pytest = "^7.0.0"
+tox = "^4.0.0"
+
+
 [[tool.poetry.source]]
 name = "jax"
 url = "https://storage.googleapis.com/jax-releases/jax_releases.html"
 priority = "explicit"
 
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/JoeyTeng/jaxrenderer/issues"
 
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+
+[tool.pytest.ini_options]
+addopts = [
+    "--import-mode=importlib",
+]
+
+[tool.isort]
+profile = "black"
+py_version= 311
+src_paths = ["renderer", "examples", "test_resources", "tests"]
+line_length = 88
+combine_star = true
+order_by_type = true
+case_sensitive = true
+force_sort_within_sections = true
+split_on_trailing_comma = true
+only_modified = true
+skip_gitignore = true
+
+[tool.black]
+target-versions = ["py38", "py39", "py310", "py311"]
+required-version = 23
+
+[tool.pyright]
+include = ["renderer", "examples", "test_resources", "tests"]
+exclude = ["typings/**", ".*/**", "**/node_modules", "**/__pycache__"]
+typeCheckingMode = "strict"
+
+pythonVersion = "3.11"
+pythonPlatform = "All"
+
+executionEnvironments = [
+  { root = ".", pythonVersion = "3.11", pythonPlatform = "All" },
+]
+
+reportCallInDefaultInitializer = "information"
+reportImplicitOverride = "information"
+reportImplicitStringConcatenation = "none"
+reportImportCycles = "error"
+reportMissingSuperCall = "information"
+reportPropertyTypeMismatch = "information"
+reportShadowedImports = "warning"
+reportUninitializedInstanceVariable = "warning"
+reportUnnecessaryTypeIgnoreComment = "warning"
+reportUnusedCallResult = "information"
```

### Comparing `jaxrenderer-0.3.1/renderer/README.md` & `jaxrenderer-0.3.2/renderer/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.1/renderer/_backport.py` & `jaxrenderer-0.3.2/renderer/_backport.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Export backward compatible bindings to replace new features used in later
     Python versions to support Python 3.8+.
 """
+
 import sys
 from typing import Any, TypeVar
 
 import jax.numpy as jnp
 
 if sys.version_info < (3, 11):
     from typing_extensions import NamedTuple
@@ -14,37 +15,54 @@
 if sys.version_info < (3, 10):
     from typing_extensions import ParamSpec, TypeAlias
 else:
     from typing import ParamSpec, TypeAlias
 
 if sys.version_info < (3, 9):
     """Type subscription requires python >= 3.9."""
-    from typing import Sequence, Tuple
+    from typing import List, Sequence, Tuple, Type
 else:
+    from builtins import list as List
     from builtins import tuple as Tuple
+    from builtins import type as Type
     from collections.abc import Sequence
 
 if sys.version_info < (3, 9):
     """Type subscription requires python >= 3.9."""
     JaxFloating: TypeAlias = jnp.floating
     JaxInteger: TypeAlias = jnp.integer
 else:
     JaxFloating: TypeAlias = jnp.floating[Any]
     JaxInteger: TypeAlias = jnp.integer[Any]
 
 K = TypeVar("K")
 V = TypeVar("V")
 if sys.version_info < (3, 9):
     from typing import Dict
+
     DictT: TypeAlias = Dict[K, V]
 else:
     DictT: TypeAlias = dict[K, V]
 
 
-def replace_dict(base: DictT, new: DictT) -> DictT:
+__all__ = [
+    "JaxFloating",
+    "JaxInteger",
+    "List",
+    "NamedTuple",
+    "ParamSpec",
+    "replace_dict",
+    "Sequence",
+    "Tuple",
+    "Type",
+    "TypeAlias",
+]
+
+
+def replace_dict(base: DictT[K, V], new: DictT[K, V]) -> DictT[K, V]:
     """Replace items in the old dictionary with new values in new dict."""
     if sys.version_info < (3, 9):
         old = base.copy()
         old.update(new)
 
         return old
```

### Comparing `jaxrenderer-0.3.1/renderer/geometry.py` & `jaxrenderer-0.3.2/renderer/geometry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,76 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 import enum
 from functools import partial
-from typing import NamedTuple, Optional, Union
+from typing import NamedTuple, Optional, Union, cast
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Float, Integer, Num, jaxtyped
+from jaxtyping import Array, Float, Integer, Num
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
+from ._backport import Tuple, TypeAlias
 from ._meta_utils import add_tracing_name
-from .types import JaxFloating, Triangle2Df, Vec2f, Vec3f, Vec4f
+from ._meta_utils import typed_jit as jit
+from .types import FloatV, JaxFloating, NumV, Triangle2Df, Vec2f, Vec2i, Vec3f, Vec4f
 
 # Transform matrix that takes a batch of homogeneous 3D vertices and transform
 # them into 2D cartesian vertices in screen space + Z value (making it 3D)
 #
 # The result of x-y values in screen space may be float, and thus further
 # conversion to integers are needed.
-World2Screen = Float[Array, "4 4"]
+World2Screen: TypeAlias = Float[Array, "4 4"]
 # Transform all coordinates from world space to view space, with camera at
 # origin. (Object Coordinates -> Eye Coordinates)
-View = Float[Array, "4 4"]
+View: TypeAlias = Float[Array, "4 4"]
 # Transform all coordinates from view space to viewing volume.
 # (Eye Coordinates -> Clip Coordinates)
-Projection = Float[Array, "4 4"]
+Projection: TypeAlias = Float[Array, "4 4"]
 # Transform all coordinates from clip space in a bi-unit cube ([-1...1]^3) to
 # a screen cube ([x, x+width] * [y, y+height] * [0, depth]) in view space.
 # (Normalised Device Coordinates -> Window Coordinates)
-Viewport = Float[Array, "4 4"]
+Viewport: TypeAlias = Float[Array, "4 4"]
 
 
 @jaxtyped
-@partial(jax.jit, donate_argnums=(0, ), inline=True)
+@partial(jit, donate_argnums=(0,), inline=True)
 @add_tracing_name
-def normalise(vector: Float[Array, "dim"]) -> Float[Array, "dim"]:
+def normalise(vector: Float[Array, "*a dim"]) -> Float[Array, "*a dim"]:
     """normalise vector in-place."""
-    return vector / jnp.linalg.norm(vector)
+    result: Float[Array, "*a dim"] = cast(
+        Float[Array, "*a dim"],
+        vector / jnp.linalg.norm(vector),
+    )
+    assert isinstance(result, Float[Array, "*a dim"])
+
+    return result
 
 
 class Interpolation(enum.Enum):
     """Interpolation methods for rasterisation.
 
     References:
       - [Interpolation qualifiers](https://www.khronos.org/opengl/wiki/Type_Qualifier_(GLSL)#Interpolation_qualifiers)
     """
+
     FLAT = 0
-    """Flat shading: use the value of the first vertex of the primitive""" ""
+    """Flat shading: use the value of the first vertex of the primitive"""
     NOPERSPECTIVE = 1
     """No perspective correction: linear interpolation in screen space"""
     SMOOTH = 2
     """Perspective correction: linear interpolation in clip space"""
 
     @jaxtyped
-    @partial(jax.jit, static_argnames=("self", ), inline=True)
+    @partial(
+        jit,
+        static_argnames=("self",),
+        inline=True,
+    )
     @add_tracing_name
     def __call__(
         self,
         values: Num[Array, "3 *valueDimensions"],
         barycentric_screen: Vec3f,
         barycentric_clip: Vec3f,
     ) -> Num[Array, "*valueDimensions"]:
@@ -66,42 +80,46 @@
           - values: values at the vertices of the triangle, with axis 0 being
             the batch axis.
           - barycentric_screen: barycentric coordinates in screen space of the
             point to interpolate
           - barycentric_clip: barycentric coordinates in clip space of the
             point to interpolate
         """
-        dtype = jax.dtypes.result_type(
+        dtype = jax.dtypes.result_type(  # pyright: ignore
             barycentric_screen,
             barycentric_clip,
             values,
         )
         coef: Vec3f
         # branches are ok because `self` is static: decided at compile time
         if self == Interpolation.FLAT:
             with jax.ensure_compile_time_eval():
-                coef = jnp.array([1, 0, 0], dtype=dtype)
+                coef = jnp.array([1, 0, 0], dtype=dtype)  # pyright: ignore
         elif self == Interpolation.NOPERSPECTIVE:
             coef = barycentric_screen
         elif self == Interpolation.SMOOTH:
             coef = barycentric_clip
         else:
             raise ValueError(f"Unknown interpolation method {self}")
 
-        interpolated = lax.dot_general(
-            coef.astype(dtype),
-            values.astype(dtype),
-            (((0, ), (0, )), ([], [])),
+        interpolated = lax.dot_general(  # pyright: ignore[reportUnknownMemberType]
+            coef.astype(dtype),  # pyright: ignore[reportUnknownMemberType]
+            values.astype(dtype),  # pyright: ignore[reportUnknownMemberType]
+            (((0,), (0,)), ([], [])),
         )
 
         return interpolated
 
 
 @jaxtyped
-@partial(jax.jit, static_argnames=("mode", ), inline=True)
+@partial(
+    jit,
+    static_argnames=("mode",),
+    inline=True,
+)
 @add_tracing_name
 def interpolate(
     values: Num[Array, "3 *valueDimensions"],
     barycentric_screen: Vec3f,
     barycentric_clip: Vec3f,
     mode: Interpolation = Interpolation.SMOOTH,
 ) -> Num[Array, "*valueDimensions"]:
@@ -117,95 +135,106 @@
     )
     assert isinstance(interpolated, Num[Array, "*valueDimensions"])
 
     return interpolated
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def to_homogeneous(
     coordinates: Float[Array, "*batch dim"],
-    value: Float[Array, "*batch"] = jnp.array(1.),
+    value: Union[float, Float[Array, "*batch"]] = 1.0,
 ) -> Float[Array, "*batch dim+1"]:
     """Transform the coordinates to homogeneous coordinates by append a batch
-        of `value`s (default 1.) in the last axis."""
+    of `value`s (default 1.) in the last axis."""
     if not isinstance(value, Float[Array, "*batch"]):
-        value = jnp.array(value)
+        value = jnp.array(value)  # pyright: ignore[reportUnknownMemberType]
 
-    paddings: Float[Array, "*batch 1"] = jnp.broadcast_to(
-        value.astype(jax.dtypes.result_type(coordinates)),
+    target_dtype = jax.dtypes.result_type(coordinates)  # pyright: ignore
+    paddings: Float[Array, "*batch 1"] = jnp.broadcast_to(  # pyright: ignore
+        value.astype(target_dtype),  # pyright: ignore
         (*coordinates.shape[:-1], 1),
     )
-    homo_coords: Float[Array, "*batch dim+1"] = lax.concatenate(
+    homo_coords: Float[Array, "*batch dim+1"] = lax.concatenate(  # pyright: ignore
         (coordinates, paddings),
         jnp.ndim(coordinates) - 1,
     )
 
     return homo_coords
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def normalise_homogeneous(
-    coordinates: Float[Array, "*batch dim"], ) -> Float[Array, "*batch dim"]:
+    coordinates: Float[Array, "*batch dim"],
+) -> Float[Array, "*batch dim"]:
     """Transform the homogenous coordinates to make the scale factor equals to
         either 1 or 0, by divide every element with the last element on the
         last axis.
 
     Noted that when a coordinate is 0 and divides by 0, it will produce a nan;
     for non-zero elements divides by 0, a inf will be produced.
     """
     return coordinates / coordinates[..., -1:]
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def to_cartesian(
-    coordinates: Float[Array, "*batch dim"], ) -> Float[Array, "*batch dim-1"]:
+    coordinates: Float[Array, "*batch dim"],
+) -> Float[Array, "*batch dim-1"]:
     """Transform the homogenous coordinates to cartesian coordinates by divide
         every element with the last element on the last axis, then drop them.
 
     When last component is 0, this function just discard the w-component
     without division.
     """
-    return jnp.where(
+    result: Float[Array, "*batch dim-1"]
+    result = jnp.where(  # pyright: ignore[reportUnknownMemberType]
         # if w component is 0, just discard it and return.
-        coordinates[..., -1:] == .0,
+        coordinates[..., -1:] == 0.0,
         coordinates[..., :-1],
         normalise_homogeneous(coordinates)[..., :-1],
     )
 
+    return result
+
 
 class Camera(NamedTuple):
     """Camera parameters.
 
     - view: transform from model space to view space
     - projection: transform from view space to clip space
     - viewport: transform from NDC (normalised device coordinate) space to
       screen space. Noticed that this is NDC space in OpenGL, which has range
       [-1, 1]^3.
     - world_to_clip: transform from model space to clip space
     - world_to_eye_norm: transform normals from model space to eye space, without projection.
     - world_to_screen: transform from model space to screen space
     """
+
     view: View
     projection: Projection
     viewport: Viewport
     world_to_clip: Projection
     world_to_eye_norm: Projection
     world_to_screen: World2Screen
     view_inv: View
     screen_to_world: World2Screen
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @partial(
+        jit,
+        static_argnames=("cls",),
+        inline=True,
+    )
     @add_tracing_name
     def create(
         cls,
         view: View,
         projection: Projection,
         viewport: Viewport,
         view_inv: Optional[View] = None,
@@ -215,19 +244,19 @@
         Parameters:
           - view: transform from model space to view space
           - projection: transform from view space to clip space
           - viewport: transform from NDC (normalised device coordinate) space to
           - view_inv: inverse of view. If not given, it will be computed.
         """
         if view_inv is None:
-            view_inv = jnp.linalg.inv(view)
+            view_inv = cast(View, jnp.linalg.inv(view))
         assert isinstance(view_inv, View)
 
-        projection_inv: Projection = lax.cond(
-            jnp.isclose(projection[3, 3], 0),
+        projection_inv: Projection = lax.cond(  # pyright: ignore
+            jnp.isclose(projection[3, 3], 0),  # pyright: ignore
             # is perspective projection matrix
             cls.perspective_projection_matrix_inv,
             # is orthographic projection matrix
             cls.orthographic_projection_matrix_inv,
             # arg
             projection,
         )
@@ -246,15 +275,15 @@
             world_to_screen=viewport @ projection @ view,
             view_inv=view_inv,
             screen_to_world=view_inv @ projection_inv @ viewport_inv,
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def apply(
         points: Num[Array, "*N 4"],
         matrix: Num[Array, "4 4"],
     ) -> Num[Array, "*N 4"]:
         """Transform homogeneous points using given matrix.
 
@@ -263,34 +292,35 @@
             being the batch axis. Batch axis can be omitted. Points must be
             in homogeneous coordinate.
           - matrix: shape (4, 4) transformation matrix
 
         Returns: coordinates transformed
         """
         assert jnp.ndim(points) < 3
-        assert (((jnp.ndim(points) == 2) and (points.shape[1] == 4))
-                or ((jnp.ndim(points) == 1) and (points.shape[0] == 4)))
+        assert ((jnp.ndim(points) == 2) and (points.shape[1] == 4)) or (
+            (jnp.ndim(points) == 1) and (points.shape[0] == 4)
+        )
 
         with jax.ensure_compile_time_eval():
             lhs_contract_axis = 1 if jnp.ndim(points) == 2 else 0
-            dtype = jax.dtypes.result_type(points, matrix)
+            dtype = jax.dtypes.result_type(points, matrix)  # pyright: ignore
 
         # put `points` at lhs to keep batch axis at axis 0 in the result.
-        transformed: Num[Array, "*N 4"] = lax.dot_general(
-            points.astype(dtype),
-            matrix.astype(dtype),
-            (((lhs_contract_axis, ), (1, )), ([], [])),
+        transformed: Num[Array, "*N 4"] = lax.dot_general(  # pyright: ignore
+            points.astype(dtype),  # pyright: ignore[reportUnknownMemberType]
+            matrix.astype(dtype),  # pyright: ignore[reportUnknownMemberType]
+            (((lhs_contract_axis,), (1,)), ([], [])),
         )
         assert isinstance(transformed, Num[Array, "*N 4"])
 
         return transformed
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @partial(jit, static_argnames=("cls",), inline=True)
     @add_tracing_name
     def apply_pos(
         cls,
         points: Num[Array, "*N 3"],
         matrix: Num[Array, "4 4"],
     ) -> Num[Array, "*N 3"]:
         """Transform points representing 3D positions using given matrix.
@@ -313,15 +343,15 @@
         transformed = to_cartesian(transformed_homo)
         assert isinstance(transformed, Num[Array, "*N 3"])
 
         return transformed
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @partial(jit, static_argnames=("cls",), inline=True)
     @add_tracing_name
     def apply_vec(
         cls,
         vectors: Num[Array, "*N 3"],
         matrix: Num[Array, "4 4"],
     ) -> Num[Array, "*N 3"]:
         """Transform vectors representing 3D positions using given matrix.
@@ -334,17 +364,20 @@
           - matrix: shape (4, 4) transformation matrix
 
         Returns: vectors transformed and normalised
         """
         normalised_vectors = normalise(vectors)
         assert isinstance(normalised_vectors, Num[Array, "*N 3"])
 
-        points_homo = to_homogeneous(
-            normalised_vectors,
-            jnp.zeros((), dtype=vectors.dtype),
+        points_homo = cast(
+            Num[Array, "*N 4"],
+            to_homogeneous(
+                normalised_vectors,
+                jnp.zeros((), dtype=vectors.dtype),  # pyright: ignore
+            ),
         )
         assert isinstance(points_homo, Num[Array, "*N 4"])
 
         transformed_homo = cls.apply(points_homo, matrix)
         assert isinstance(transformed_homo, Num[Array, "*N 4"])
 
         transformed = transformed_homo[..., :3]
@@ -352,15 +385,15 @@
 
         transformed_normalised = normalise(transformed)
         assert isinstance(transformed_normalised, Num[Array, "*N 3"])
 
         return transformed_normalised
 
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def to_screen(
         self,
         points: Num[Array, "*N 4"],
     ) -> Num[Array, "*N 4"]:
         """Transform points from model space to screen space.
 
@@ -378,15 +411,15 @@
 
         normalised = normalise_homogeneous(screen_space)
         assert isinstance(normalised, Num[Array, "*N 4"])
 
         return normalised
 
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def to_clip(
         self,
         points: Num[Array, "*N 4"],
     ) -> Num[Array, "*N 4"]:
         """Transform points from model space to screen space.
 
@@ -401,15 +434,15 @@
         """
         clip_space = self.apply(points, self.world_to_clip)
         assert isinstance(clip_space, Num[Array, "*N 4"])
 
         return clip_space
 
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def to_screen_inv(
         self,
         screen: Float[Array, "*N 4"],
     ) -> Float[Array, "*N 4"]:
         """Transform points from screen space to model space.
 
@@ -422,50 +455,46 @@
         `view_matrix_inv`, this should provide a much higher precision.
         """
         if screen.ndim == 1:
             _screen = screen[None, :]
         else:
             _screen = screen
 
-        clip = lax.linalg.triangular_solve(self.viewport, _screen)
+        clip: Float[Array, "*N 4"] = lax.linalg.triangular_solve(  # pyright: ignore
+            self.viewport,
+            _screen,
+        )
         assert isinstance(clip, Float[Array, "*N 4"])
-        shuffle = lax.cond(
+        shuffle = lax.cond(  # pyright: ignore
             self.projection[3, 3] == 0,
             # perspective projection
-            lambda: jnp.array([0, 1, 3, 2]),
+            lambda: jnp.array([0, 1, 3, 2]),  # pyright: ignore[reportUnknownMemberType]
             # orthographic projection
-            lambda: jnp.array([0, 1, 2, 3]),
+            lambda: jnp.array([0, 1, 2, 3]),  # pyright: ignore[reportUnknownMemberType]
         )
-        eye = lax.linalg.triangular_solve(
+        eye: Float[Array, "*N 4"] = lax.linalg.triangular_solve(  # pyright: ignore
             self.projection[..., shuffle],
             clip[..., shuffle],
         )[..., shuffle]
         assert isinstance(eye, Float[Array, "*N 4"])
         world = self.apply(eye, self.view_inv)
         assert isinstance(world, Float[Array, "*N 4"])
 
         if screen.ndim == 1:
             world = world[0]
 
-        jax.debug.print(
-            "s {} c {} e {} w {}",
-            normalise_homogeneous(screen),
-            normalise_homogeneous(clip),
-            normalise_homogeneous(eye),
-            normalise_homogeneous(world),
-        )
-
         return world
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def inv_scale_translation_matrix(
-            scale_translation_mat: Float[Array, "4 4"]) -> Float[Array, "4 4"]:
+        scale_translation_mat: Float[Array, "4 4"]
+    ) -> Float[Array, "4 4"]:
         """Compute the inverse matrix of a (4, 4) matrix representing a scale and translation, in a form of:
 
             [[s_x, 0,   0,   t_x],
              [0,   s_y, 0,   t_y],
              [0,   0,   s_z, t_z],
              [0,   0,   0,   1]]
 
@@ -476,35 +505,37 @@
         This utilise the fact that the inverse of a scale operation is just the
         reciprocal of the scale factor, and the inverse of a translation is
         just the negative of the translation. It separates the scale and
         translation operations first, inverse them separately, then combine
         them back (in reverse order).
         """
 
-        scale_inv = jnp.diag(1. / jnp.diag(scale_translation_mat))
+        scale_inv = jnp.diag(1.0 / jnp.diag(scale_translation_mat))  # pyright: ignore
         assert isinstance(scale_inv, Float[Array, "4 4"])
 
         # scale_translation = scale @ translation;
         # thus  translation = scale_inv @ scale @ translation
         #                   = scale_inv @ scale_translation
         translation: Float[Array, "4 4"] = scale_inv @ scale_translation_mat
         assert isinstance(translation, Float[Array, "4 4"])
 
         # inverse of translation: negative of translation
-        translation_inv = (jnp.identity(4).at[:3, 3].set(-translation[:3, 3]))
+        translation_inv = (
+            jnp.identity(4).at[:3, 3].set(-translation[:3, 3])  # pyright: ignore
+        )
         assert isinstance(translation_inv, Float[Array, "4 4"])
 
         scale_translation_inv = translation_inv @ scale_inv
         assert isinstance(scale_translation_inv, Float[Array, "4 4"])
 
         return scale_translation_inv
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def view_matrix(
         eye: Vec3f,
         centre: Vec3f,
         up: Vec3f,
     ) -> View:
         """Compute View matrix as defined by OpenGL / tinyrenderer.
@@ -521,32 +552,35 @@
         Reference:
           - [gluLookAt](https://registry.khronos.org/OpenGL-Refpages/gl2.1/xhtml/gluLookAt.xml)
           - [glTranslate](https://registry.khronos.org/OpenGL-Refpages/gl2.1/xhtml/glTranslate.xml)
           - [GluLookAt Code](https://www.khronos.org/opengl/wiki/GluLookAt_code)
         """
         forward: Vec3f = normalise(centre - eye)
         up = normalise(up)
-        side: Vec3f = normalise(jnp.cross(forward, up))
-        up = jnp.cross(side, forward)
+        side: Vec3f = normalise(jnp.cross(forward, up))  # pyright: ignore
+        up = cast(Vec3f, jnp.cross(side, forward))
 
         m: View = (
-            jnp.identity(4)  #
-            .at[0, :3].set(side)  #
-            .at[1, :3].set(up)  #
-            .at[2, :3].set(-forward)  #
+            jnp.identity(4)  # pyright: ignore[reportUnknownMemberType]
+            .at[0, :3]
+            .set(side)
+            .at[1, :3]
+            .set(up)
+            .at[2, :3]
+            .set(-forward)
         )
-        translation: View = jnp.identity(4).at[:3, 3].set(-eye)
+        translation: View = jnp.identity(4).at[:3, 3].set(-eye)  # pyright: ignore
 
         view: View = m @ translation
 
         return view
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def view_matrix_inv(
         eye: Vec3f,
         centre: Vec3f,
         up: Vec3f,
     ) -> View:
         """Compute the invert of View matrix as defined by OpenGL.
@@ -568,45 +602,48 @@
 
         Reference:
           - [gluLookAt](https://registry.khronos.org/OpenGL-Refpages/gl2.1/xhtml/gluLookAt.xml)
           - [4B](http://graphics.stanford.edu/courses/cs248-98-fall/Final/q4.html)
         """
         forward: Vec3f = normalise(centre - eye)
         up = normalise(up)
-        side: Vec3f = normalise(jnp.cross(forward, up))
-        up = jnp.cross(side, forward)
+        side: Vec3f = normalise(jnp.cross(forward, up))  # pyright: ignore
+        up = cast(Vec3f, jnp.cross(side, forward))
 
         # inverse of rotation is just the transpose
         m: View = (
-            jnp.identity(4)  #
-            .at[0, :3].set(side)  #
-            .at[1, :3].set(up)  #
-            .at[2, :3].set(-forward)  #
+            jnp.identity(4)  # pyright: ignore[reportUnknownMemberType]
+            .at[0, :3]
+            .set(side)
+            .at[1, :3]
+            .set(up)
+            .at[2, :3]
+            .set(-forward)
         )
         m_inv: View = m.T
         assert isinstance(m_inv, View)
 
         # inverse of translation is just the negative of translation
-        translation_inv: View = jnp.identity(4).at[:3, 3].set(eye)
+        translation_inv: View = jnp.identity(4).at[:3, 3].set(eye)  # pyright: ignore
         assert isinstance(translation_inv, View)
 
         view_matrix_inv: View = translation_inv @ m_inv
         assert isinstance(view_matrix_inv, View)
 
         return view_matrix_inv
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def perspective_projection_matrix(
-        fovy: JaxFloating,
-        aspect: JaxFloating,
-        z_near: JaxFloating,
-        z_far: JaxFloating,
+        fovy: Union[float, JaxFloating, FloatV],
+        aspect: Union[float, JaxFloating, FloatV],
+        z_near: Union[float, JaxFloating, FloatV],
+        z_far: Union[float, JaxFloating, FloatV],
     ) -> Projection:
         """Create a projection matrix to map the model in the camera frame (eye
             coordinates) onto the viewing volume (clip coordinates), using
             perspective transformation. This follows the implementation in
             OpenGL (gluPerspective)
 
         Parameters:
@@ -621,31 +658,38 @@
             plane (always positive).
 
         Return: Projection, (4, 4) matrix.
 
         Reference:
           - [gluPerspective](https://registry.khronos.org/OpenGL-Refpages/gl2.1/xhtml/gluPerspective.xml)
         """
-        f: jnp.single = 1. / lax.tan(
-            jnp.radians(jnp.asarray(fovy).astype(jnp.single)) / 2.)
+        deg: FloatV = jnp.asarray(fovy, dtype=jnp.single)  # pyright: ignore
+        f: FloatV = 1.0 / lax.tan(  # pyright: ignore[reportUnknownMemberType]
+            cast(FloatV, jnp.radians(deg) / 2.0)
+        )
         projection: Projection = (
-            jnp.zeros((4, 4), dtype=jnp.single)  #
-            .at[0, 0].set(f / aspect)  #
-            .at[1, 1].set(f)  #
-            .at[2, 2].set((z_far + z_near) / (z_near - z_far))  #
+            jnp.zeros((4, 4), dtype=jnp.single)  # pyright: ignore
+            .at[0, 0]
+            .set(f / aspect)
+            .at[1, 1]
+            .set(f)
+            .at[2, 2]
+            .set((z_far + z_near) / (z_near - z_far))
             # translate z
-            .at[2, 3].set((2. * z_far * z_near) / (z_near - z_far))  #
-            .at[3, 2].set(-1.)  # let \omega be -z
+            .at[2, 3]
+            .set((2.0 * z_far * z_near) / (z_near - z_far))
+            .at[3, 2]
+            .set(-1.0)  # let \omega be -z
         )
 
         return projection
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @partial(jit, static_argnames=("cls",), inline=True)
     @add_tracing_name
     def perspective_projection_matrix_inv(cls, mat: Projection) -> Projection:
         """Create the inverse of a perspective projection matrix as defined in
             `perspective_projection_matrix`.
 
         Since the perspective projection matrix is formed as:
 
@@ -657,33 +701,33 @@
         it can be simply transformed into a scale-translation matrix by
         swapping the last two columns. Thus, the inverse is computed by
         swapping the last columns, then inverting using
         `inv_scale_translation_matrix`, and finally swapping back (last two
         rows, instead).
         """
         with jax.ensure_compile_time_eval():
-            shuffle: Integer[Array, "4"] = jnp.array((0, 1, 3, 2))
+            shuffle: Integer[Array, "4"] = jnp.array((0, 1, 3, 2))  # pyright: ignore
             assert isinstance(shuffle, Integer[Array, "4"])
 
         inv = cls.inv_scale_translation_matrix(mat[:, shuffle])[shuffle, :]
         assert isinstance(inv, Projection)
 
         return inv
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def orthographic_projection_matrix(
-        left: JaxFloating,
-        right: JaxFloating,
-        bottom: JaxFloating,
-        top: JaxFloating,
-        z_near: JaxFloating,
-        z_far: JaxFloating,
+        left: Union[float, JaxFloating],
+        right: Union[float, JaxFloating],
+        bottom: Union[float, JaxFloating],
+        top: Union[float, JaxFloating],
+        z_near: Union[float, JaxFloating],
+        z_far: Union[float, JaxFloating],
     ) -> Projection:
         """Create a projection matrix to map the model in the camera frame (eye
             coordinates) onto the viewing volume (clip coordinates), using
             orthographic transformation. This follows the implementation in
             OpenGL (glOrtho).
 
         Parameters:
@@ -696,78 +740,84 @@
             if they are behind the viewer.
 
         Return: Projection, (4, 4) matrix.
 
         Reference:
           - [glOrtho](https://registry.khronos.org/OpenGL-Refpages/gl2.1/xhtml/glOrtho.xml)
         """
-        l_op: Float[Array, "3"] = jnp.array([right, top, z_far])
-        r_op: Float[Array, "3"] = jnp.array([left, bottom, z_near])
+        l_op: Float[Array, "3"] = jnp.array([right, top, z_far])  # pyright: ignore
+        r_op: Float[Array, "3"] = jnp.array([left, bottom, z_near])  # pyright: ignore
         projection: Projection = (
-            jnp.zeros((4, 4), dtype=jnp.single)  #
-            .at[0, 0].set(2 / (right - left))  #
-            .at[1, 1].set(2 / (top - bottom))  #
-            .at[2, 2].set(-2 / (z_far - z_near))  #
-            .at[3, 3].set(1)  #
-            .at[:3, 3].set(-(l_op + r_op) / (l_op - r_op))  #
+            jnp.zeros((4, 4), dtype=jnp.single)  # pyright: ignore
+            .at[0, 0]
+            .set(2 / (right - left))
+            .at[1, 1]
+            .set(2 / (top - bottom))
+            .at[2, 2]
+            .set(-2 / (z_far - z_near))
+            .at[3, 3]
+            .set(1)  #
+            .at[:3, 3]
+            .set(-(l_op + r_op) / (l_op - r_op))
         )
 
         return projection
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ))
+    @partial(jit, static_argnames=("cls",))
     @add_tracing_name
     def orthographic_projection_matrix_inv(cls, mat: Projection) -> Projection:
         """Create the inverse of a orthographic projection matrix as defined in
-            `orthographic_projection_matrix`. Since orthographic projection
-            matrix is a scale-translation matrix, the inverse is computed by
-            `inv_scale_translation_matrix` directly.
+        `orthographic_projection_matrix`. Since orthographic projection
+        matrix is a scale-translation matrix, the inverse is computed by
+        `inv_scale_translation_matrix` directly.
         """
         inv = cls.inv_scale_translation_matrix(mat)
         assert isinstance(inv, Projection)
 
         return inv
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def perspective_projection_matrix_tinyrenderer(
         eye: Vec3f,
         centre: Vec3f,
-        dtype: jnp.dtype = jnp.single,
+        dtype: type = jnp.single,
     ) -> Projection:
         """Create a projection matrix to map the model in the camera frame (eye
             coordinates) onto the viewing volume (clip coordinates), using
             perspective transformation.
 
         Parameters:
           - eye: the position of camera, in world space
           - centre: the centre of the frame, where the camera points to, in
             world space
           - dtype: the dtype for the projection matrix.
 
         Return: Projection, (4, 4) matrix.
         """
         projection: Projection = (
-            jnp.identity(4, dtype=dtype)  #
-            .at[3, 2].set(-1 / jnp.linalg.norm(eye - centre))  #
+            jnp.identity(4, dtype=dtype)  # pyright: ignore[reportUnknownMemberType]
+            .at[3, 2]
+            .set(-1 / jnp.linalg.norm(eye - centre))
         )
 
         return projection
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def viewport_matrix(
         lowerbound: Num[Array, "2"],
-        dimension: Integer[Array, "2"],
-        depth: Num[Array, ""],
+        dimension: Vec2i,
+        depth: Union[int, float, NumV],
     ) -> Viewport:
         """Create a viewport matrix to map the model in bi-unit cube
             ([-1...1]^3) onto the screen cube ([x, x+w]*[y, y+h]*[0, d]). The
             result matrix is the viewport matrix as defined in OpenGL /
             tinyrenderer.
 
         Parameters:
@@ -777,25 +827,30 @@
           - depth: the depth of the viewport in screen space, for zbuffer
           - dtype: the dtype for the viewport matrix.
 
         Return: Viewport, (4, 4) matrix.
         """
         width, height = dimension
         viewport: Viewport = (
-            jnp.identity(4)  #
-            .at[:2, 3].set(lowerbound + dimension / 2)  #
-            .at[0, 0].set(width / 2).at[1, 1].set(height / 2)  #
-            .at[2, 2:].set(depth / 2)  #
+            jnp.identity(4)  # pyright: ignore[reportUnknownMemberType]
+            .at[:2, 3]
+            .set(lowerbound + dimension / 2)
+            .at[0, 0]
+            .set(width / 2)
+            .at[1, 1]
+            .set(height / 2)
+            .at[2, 2:]
+            .set(depth / 2)
         )
 
         return viewport
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @partial(jit, static_argnames=("cls",), inline=True)
     @add_tracing_name
     def viewport_matrix_inv(cls, viewport: Viewport) -> Viewport:
         """Create the inverse of a viewport matrix as defined in `viewport_matrix`.
 
         Parameters:
           - viewport: Viewport matrix to invert.
 
@@ -804,194 +859,209 @@
         viewport_inv: Viewport = cls.inv_scale_translation_matrix(viewport)
         assert isinstance(viewport_inv, Viewport)
 
         return viewport_inv
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def world_to_screen_matrix(width: int, height: int) -> World2Screen:
         """Generate the projection matrix to convert model coordinates to
             screen/canvas coordinates.
 
         It assumes all model coordinates are in [-1...1] and will transform them
         into ([0...width], [0...height], [-1...1]).
 
         Return: World2Screen (Float[Array, "4 4"])
         """
         world2screen: World2Screen = (
             # 3. div by half to centering
-            jnp.identity(4).at[0, 0].set(.5).at[1, 1].set(.5)
+            jnp.identity(4).at[0, 0].set(0.5).at[1, 1].set(0.5)  # pyright: ignore
             # 2. mul by width, height
-            @ jnp.identity(4).at[0, 0].set(width).at[1, 1].set(height)
+            @ jnp.eye(4).at[0, 0].set(width).at[1, 1].set(height)  # pyright: ignore
             # 1. Add by 1 to make values positive
-            @ jnp.identity(4).at[:2, -1].set(1))
+            @ jnp.identity(4).at[:2, -1].set(1)  # pyright: ignore
+        )
 
         return world2screen
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def compute_normal(triangle_verts: Float[Array, "3 3"]) -> Float[Array, "3"]:
-    normal: Float[Array, "3"] = jnp.cross(
-        triangle_verts[2, :] - triangle_verts[0, :],
-        triangle_verts[1, :] - triangle_verts[0, :],
+    normal: Float[Array, "3"] = cast(
+        Float[Array, "3"],
+        jnp.cross(
+            triangle_verts[2, :] - triangle_verts[0, :],
+            triangle_verts[1, :] - triangle_verts[0, :],
+        ),
     )
-    normal = normal / jnp.linalg.norm(normal, keepdims=True)
+    normal = cast(Float[Array, "3"], normal / jnp.linalg.norm(normal, keepdims=True))
     assert isinstance(normal, Float[Array, "3"])
 
     return normal
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
-@add_tracing_name
-def compute_normals(batch_verts: Float[Array, "b 3 3"]) -> Float[Array, "b 3"]:
-    return jax.vmap(compute_normal)(batch_verts)
-
-
-@jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def quaternion(
-    rotation_axis: Union[Vec3f, tuple[float, float, float]],
-    rotation_angle: Union[Float[Array, ""], float],
+    rotation_axis: Union[Vec3f, Tuple[float, float, float]],
+    rotation_angle: Union[FloatV, float],
 ) -> Vec4f:
     """Generate a quaternion rotation from a rotation axis and angle.
 
     The rotation axis is normalised internally. The angle is specified in
     degrees (NOT radian). The rotation is clockwise.
 
     The resultant quaternion is in order of (w, x, y, z).
     """
-    axis = normalise(jnp.asarray(rotation_axis))
-    angle = jnp.radians(jnp.asarray(rotation_angle))
+    axis = normalise(jnp.asarray(rotation_axis))  # pyright: ignore
+    angle = jnp.radians(jnp.asarray(rotation_angle))  # pyright: ignore
     assert isinstance(axis, Vec3f), f"{rotation_axis}"
-    assert isinstance(angle, Float[Array, ""]), f"{rotation_angle}"
+    assert isinstance(angle, FloatV), f"{rotation_angle}"
 
     quaternion: Vec4f = (
-        jnp.zeros(4)  #
-        .at[0].set(jnp.cos(angle / 2))  #
-        .at[1:].set(axis * jnp.sin(angle / 2))  #
+        jnp.zeros(4)  # pyright: ignore[reportUnknownMemberType]
+        .at[0]
+        .set(jnp.cos(angle / 2))  # pyright: ignore[reportUnknownMemberType]
+        .at[1:]
+        .set(axis * jnp.sin(angle / 2))  # pyright: ignore[reportUnknownMemberType]
     )
 
     return quaternion
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def quaternion_mul(quatA: Vec4f, quatB: Vec4f) -> Vec4f:
     """Multiply two quaternion rotations, as to composite them.
 
     Noticed that all quaternions here are in order of (w, x, y, z).
 
     References:
       - [Quaternion multiplication](https://www.mathworks.com/help/nav/ref/quaternion.mtimes.html)
     """
     assert isinstance(quatA, Vec4f)
     assert isinstance(quatB, Vec4f)
 
     with jax.ensure_compile_time_eval():
-        idx103 = jnp.array((1, 0, 3))
-        idx230 = jnp.array((2, 3, 0))
-        idx013 = jnp.array((0, 1, 3))
-        idx320 = jnp.array((3, 2, 0))
-
-    return jnp.array((
-        quatA[0] * quatB[0] - quatA[1:] @ quatB[1:],
-        quatA[:3] @ quatB[idx103] - quatA[3] * quatB[2],
-        quatA[idx230] @ quatB[:3] - quatA[1] * quatB[3],
-        quatA[idx013] @ quatB[idx320] - quatA[2] * quatB[1],
-    ))
+        idx103 = jnp.array((1, 0, 3))  # pyright: ignore[reportUnknownMemberType]
+        idx230 = jnp.array((2, 3, 0))  # pyright: ignore[reportUnknownMemberType]
+        idx013 = jnp.array((0, 1, 3))  # pyright: ignore[reportUnknownMemberType]
+        idx320 = jnp.array((3, 2, 0))  # pyright: ignore[reportUnknownMemberType]
+
+    return jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (
+            quatA[0] * quatB[0] - quatA[1:] @ quatB[1:],
+            quatA[:3] @ quatB[idx103] - quatA[3] * quatB[2],
+            quatA[idx230] @ quatB[:3] - quatA[1] * quatB[3],
+            quatA[idx013] @ quatB[idx320] - quatA[2] * quatB[1],
+        )
+    )
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def rotation_matrix(
-    rotation_axis: Union[Vec3f, tuple[float, float, float]],
-    rotation_angle: Union[Float[Array, ""], float],
+    rotation_axis: Union[Vec3f, Tuple[float, float, float]],
+    rotation_angle: Union[FloatV, float],
 ) -> Float[Array, "3 3"]:
     """Generate a rotation matrix from a rotation axis and angle.
 
     The rotation axis is normalised internally. The angle is specified in
     degrees (NOT radian). The rotation is clockwise.
 
     References:
       - [glRotated](https://registry.khronos.org/OpenGL-Refpages/gl2.1/xhtml/glRotate.xml)
     """
-    axis = normalise(jnp.asarray(rotation_axis))
-    angle = jnp.radians(jnp.asarray(rotation_angle))
+    axis = normalise(jnp.asarray(rotation_axis))  # pyright: ignore
+    angle = jnp.radians(jnp.asarray(rotation_angle))  # pyright: ignore
     assert isinstance(axis, Vec3f), f"{rotation_axis}"
-    assert isinstance(angle, Float[Array, ""]), f"{rotation_angle}"
+    assert isinstance(angle, FloatV), f"{rotation_angle}"
 
-    s = jnp.sin(angle)
-    c = jnp.cos(angle)
+    c = jnp.cos(angle)  # pyright: ignore[reportUnknownMemberType]
 
-    rotation_matrix: Float[Array, "3 3"] = (
-        jnp.identity(3) * c  # +c at main diagonal
-        - jnp.sin(angle) * jnp.cross(axis, jnp.identity(3))  # second term
-        + (1 - c) * jnp.outer(axis, axis)  # first term
+    rotation_matrix: Float[Array, "3 3"] = cast(
+        Float[Array, "3 3"],
+        jnp.identity(3) * c  # +c at main diagonal # pyright: ignore
+        # second term
+        - jnp.sin(angle) * jnp.cross(axis, jnp.identity(3))  # pyright: ignore
+        + (1 - c) * jnp.outer(axis, axis),  # first term
     )
+    assert isinstance(rotation_matrix, Float[Array, "3 3"])
 
     return rotation_matrix
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def transform_matrix_from_rotation(rotation: Vec4f) -> Float[Array, "3 3"]:
     """Generate a transform matrix from a quaternion rotation.
 
     Quaternion is specified in (w, x, y, z) order. Supports non-unit rotation.
 
     References:
           - [Quaternions and spatial rotation#Quaternion-derived rotation matrix](https://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation#Quaternion-derived_rotation_matrix)
           - [TinySceneRenderer::set_object_orientation](https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/tinyrenderer.cpp#LL997C20-L997C20)
     """
     d = rotation @ rotation
     s = 2.0 / d  # here s is $2\times s$ in Wikipedia.
 
     rs: Vec3f = rotation[1:] * s  # x y z
-    ((wx, wy, wz), (xx, xy, xz), (_, yy, yz)) = jnp.outer(rotation[:3], rs)
+    ((wx, wy, wz), (xx, xy, xz), (_, yy, yz)) = jnp.outer(  # pyright: ignore
+        rotation[:3],
+        rs,
+    )
     zz = rotation[3] * rs[2]
 
-    mat: Float[Array, "3 3"] = jnp.array((
-        (1. - (yy + zz), xy - wz, xz + wy),
-        (xy + wz, 1. - (xx + zz), yz - wx),
-        (xz - wy, yz + wx, 1. - (xx + yy)),
-    ))
+    mat: Float[Array, "3 3"] = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (
+            (1.0 - (yy + zz), xy - wz, xz + wy),
+            (xy + wz, 1.0 - (xx + zz), yz - wx),
+            (xz - wy, yz + wx, 1.0 - (xx + yy)),
+        )
+    )
     assert isinstance(mat, Float[Array, "3 3"])
 
     return mat
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def barycentric(pts: Triangle2Df, p: Vec2f) -> Vec3f:
     """Compute the barycentric coordinate of `p`.
-        Returns u[-1] < 0 if `p` is outside of the triangle.
+    Returns u[-1] < 0 if `p` is outside of the triangle.
     """
-    mat: Float[Array, "3 2"] = jnp.vstack((
-        pts[2] - pts[0],
-        pts[1] - pts[0],
-        pts[0] - p,
-    ))
-    v: Vec3f = jnp.cross(mat[:, 0], mat[:, 1])
+    mat: Float[Array, "3 2"] = jnp.vstack(  # pyright: ignore[reportUnknownMemberType]
+        (
+            pts[2] - pts[0],
+            pts[1] - pts[0],
+            pts[0] - p,
+        )
+    )
+    v: Vec3f = cast(Vec3f, jnp.cross(mat[:, 0], mat[:, 1]))
     # `u[2]` is 0, that means triangle is degenerate, in this case
     # return something with negative coordinates
-    v = lax.cond(
-        jnp.abs(v[-1]) < 1e-10,
-        lambda: jnp.array((-1., 1., 1.)),
-        lambda: jnp.array((
-            1 - (v[0] + v[1]) / v[2],
-            v[1] / v[2],
-            v[0] / v[2],
-        )),
+    v = cast(
+        Vec3f,
+        lax.cond(  # pyright: ignore[reportUnknownMemberType]
+            jnp.abs(v[-1]) < 1e-10,  # pyright: ignore[reportUnknownArgumentType]
+            lambda: jnp.array((-1.0, 1.0, 1.0)),  # pyright: ignore
+            lambda: jnp.array(  # pyright: ignore[reportUnknownMemberType]
+                (
+                    1 - (v[0] + v[1]) / v[2],
+                    v[1] / v[2],
+                    v[0] / v[2],
+                )
+            ),
+        ),
     )
     assert isinstance(v, Vec3f)
 
     return v
```

### Comparing `jaxrenderer-0.3.1/renderer/model.py` & `jaxrenderer-0.3.2/renderer/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import Optional
+from typing import Optional, Union, cast
 
 import jax
 import jax.experimental.checkify as checkify
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import tree_map
-from jaxtyping import (Array, Bool, Float, Integer, Num, PyTree, Shaped,
-                       jaxtyped)
+from jaxtyping import Array, Bool, Float, Integer, Num, Shaped
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
-from ._backport import NamedTuple, Sequence, Tuple, TypeAlias
+from ._backport import List, NamedTuple, Sequence, Tuple, TypeAlias
 from ._meta_utils import add_tracing_name
+from ._meta_utils import typed_jit as jit
 from .geometry import Camera, transform_matrix_from_rotation
-from .types import (FALSE_ARRAY, FaceIndices, Normals, SpecularMap, Texture,
-                    UVCoordinates, Vec3f, Vec4f, Vertices)
+from .types import (
+    FALSE_ARRAY,
+    BoolV,
+    FaceIndices,
+    FloatV,
+    IntV,
+    Normals,
+    SpecularMap,
+    Texture,
+    UVCoordinates,
+    Vec3f,
+    Vec4f,
+    Vertices,
+)
 from .value_checker import index_in_bound
 
 ModelMatrix: TypeAlias = Float[Array, "4 4"]
 
 
 class Model(NamedTuple):
     """Model with vertices specification and attached maps.
 
     NormalMap is not included for now as it is not used in the reference
     implementation
     [erwincoumans/tinyrenderer](https://github.com/erwincoumans/tinyrenderer).
     """
+
     verts: Vertices
     norms: Normals
     uvs: UVCoordinates
     faces: FaceIndices
     faces_norm: FaceIndices
     faces_uv: FaceIndices
 
@@ -46,20 +60,20 @@
         norms: Normals,
         uvs: UVCoordinates,
         faces: FaceIndices,
         diffuse_map: Texture,
         specular_map: Optional[SpecularMap] = None,
     ) -> "Model":
         """A convenient method to create a Model assuming faces_norm and
-            faces_uv are the same as faces. A default specular_map is used if
-            not given, with a constant value of 2.0.
+        faces_uv are the same as faces. A default specular_map is used if
+        not given, with a constant value of 2.0.
         """
         if specular_map is None:
             # reference: https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/model.cpp#L215
-            specular_map = lax.full(diffuse_map.shape[:2], 2.0)
+            specular_map = lax.full(diffuse_map.shape[:2], 2.0)  # pyright: ignore
 
         assert isinstance(verts, Vertices), f"{verts}"
         assert isinstance(norms, Normals), f"{norms}"
         assert isinstance(uvs, UVCoordinates), f"{uvs}"
         assert isinstance(faces, FaceIndices), f"{faces}"
         assert isinstance(diffuse_map, Texture), f"{diffuse_map}"
         assert isinstance(specular_map, SpecularMap), f"{specular_map}"
@@ -72,81 +86,79 @@
             faces_norm=faces,
             faces_uv=faces,
             diffuse_map=diffuse_map,
             specular_map=specular_map,
         )
 
     @jaxtyped
-    @jax.jit
-    def asserts(self):
+    @jit
+    def asserts(self) -> None:
         """Asserts that all fields are of correct shape and type."""
         assert isinstance(self.verts, Vertices), f"{self.verts}"
         assert isinstance(self.norms, Normals), f"{self.norms}"
         assert isinstance(self.uvs, UVCoordinates), f"{self.uvs}"
         assert isinstance(self.faces, FaceIndices), f"{self.faces}"
         assert isinstance(self.faces_norm, FaceIndices), f"{self.faces_norm}"
         assert isinstance(self.faces_uv, FaceIndices), f"{self.faces_uv}"
         assert isinstance(self.diffuse_map, Texture), f"{self.diffuse_map}"
-        assert isinstance(self.specular_map,
-                          SpecularMap), f"{self.specular_map}"
+        assert isinstance(self.specular_map, SpecularMap), f"{self.specular_map}"
 
     @jaxtyped
     @checkify.checkify
-    @jax.jit
-    def value_checks(self):
+    @jit
+    def value_checks(self) -> None:
         """Check values are of correct value ranges.
 
         Checks implemented:
           - indices are in bound, for faces, faces_norm, faces_uv (against
             verts, norms, uv).
 
         UV coordinates are not checked as out-of-bound values are allowed and used as "repeat" mode.
 
         Usage:
           model = Model(...)
           err, _ = model.value_checks()
           err.throw()  # throw if any error is found.
         """
         # indices are in bound
-        checkify.check(
+        checkify.check(  # pyright: ignore[reportUnknownMemberType]
             index_in_bound(self.faces, self.verts.shape[0]),
             # f-string for shape as shape is compile-time constant and
             # is not supported as a format string parameter in checkify.
             f"faces out of bound, expected [0, {self.verts.shape[0]}),"
             # separately specify fmt_kwargs in a non-f-string.
             " got {max_idx}.",
-            max_idx=self.faces.max(),
+            max_idx=self.faces.max(),  # pyright: ignore[reportUnknownMemberType]
         )
-        checkify.check(
+        checkify.check(  # pyright: ignore[reportUnknownMemberType]
             index_in_bound(self.faces_norm, self.norms.shape[0]),
             f"faces_norm out of bound, expected [0, {self.norms.shape[0]}),"
             " got {max_idx}.",
-            max_idx=self.faces_norm.max(),
+            max_idx=self.faces_norm.max(),  # pyright: ignore[reportUnknownMemberType]
         )
-        checkify.check(
+        checkify.check(  # pyright: ignore[reportUnknownMemberType]
             index_in_bound(self.faces_uv, self.uvs.shape[0]),
             f"faces_uv out of bound, expected [0, {self.uvs.shape[0]}),"
             " got {max_idx}.",
-            max_idx=self.faces_uv.max(),
+            max_idx=self.faces_uv.max(),  # pyright: ignore[reportUnknownMemberType]
         )
 
 
 VertT: TypeAlias = Num[Array, "_dim ..."]
 VertsT: TypeAlias = Sequence[VertT]
 FaceIndicesT: TypeAlias = Num[Array, "_faces 3"]
 FaceIndicessT: TypeAlias = Sequence[FaceIndicesT]
 
 MapT: TypeAlias = Num[Array, "_width _height ..."]
 MapsT: TypeAlias = Sequence[MapT]
-Shape2DT: TypeAlias = Tuple[Integer[Array, ""], Integer[Array, ""]]
-"""Shape of first two components of a map, i.e., (width, height)."""
 
 
 class MergedModel(NamedTuple):
     """Merged model with vertices, normals, uv coordinates, and faces."""
+
     verts: Vertices
     norms: Normals
     uvs: UVCoordinates
     faces: FaceIndices
     faces_norm: FaceIndices
     faces_uv: FaceIndices
 
@@ -155,83 +167,90 @@
     """Texture map index for each vertex."""
     double_sided: Bool[Array, "vertices"]
     """Whether each face is double sided."""
 
     # Merged maps
     texture_shape: Integer[Array, "objects 2"]
     """Width, height of each texture map."""
-    offset: Integer[Array, ""]
+    offset: int
     """Width of biggest merged maps, as [0] returned by `merge_maps`."""
     diffuse_map: Texture
     specular_map: SpecularMap
 
     @staticmethod
     @jaxtyped
     @add_tracing_name
     def generate_object_vert_info(
         counts: Sequence[int],
-        values: Sequence[Shaped[Array, "..."]],
+        values: Sequence[Union[int, Shaped[Array, "..."]]],
     ) -> Shaped[Array, "vertices"]:
         """Generate object-wide info for each vertex in merged model as
             vertex-level info.
 
         Parameters:
           - counts: Number of vertices of each object.
           - values: value to be filled in for each object.
 
         Returns: Map indices for each face.
 
         Note: this function cannot be jitted by itself as it uses the value of
             `counts` to create matrices: the shape depends on the value of
             `counts`.
         """
-        values: Sequence[Shaped[Array, "_"]] = tree_map(
-            lambda count, value: jnp.full(
-                (count, *jnp.asarray(value).shape), value),
-            counts,
-            values,
+        _values: Sequence[Shaped[Array, "_"]] = cast(
+            Sequence[Shaped[Array, "_"]],
+            tree_map(
+                lambda count, value: jnp.full(  # pyright: ignore[reportUnknownMemberType]
+                    (count, *jnp.asarray(value).shape),  # pyright: ignore
+                    value,
+                ),
+                counts,
+                values,
+            ),
         )
-        map_indices = lax.concatenate(values, dimension=0)
+        map_indices = lax.concatenate(_values, dimension=0)  # pyright: ignore
 
         return map_indices
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def merge_verts(
         vs: VertsT,
         fs: FaceIndicessT,
-    ) -> tuple[VertT, FaceIndicesT]:
+    ) -> Tuple[VertT, FaceIndicesT]:
         """"""
         counts = [v.shape[0] for v in vs[:-1]]
         cumsum = [0]
         for count in counts:
             cumsum.append(cumsum[-1] + count)
 
-        dtype = jax.dtypes.result_type(*vs)
+        dtype = jax.dtypes.result_type(*vs)  # pyright: ignore
 
         # merge vertices
-        verts: VertT = lax.concatenate(
-            [v.astype(dtype) for v in vs],
+        verts: VertT = lax.concatenate(  # pyright: ignore[reportUnknownMemberType]
+            [v.astype(dtype) for v in vs],  # pyright: ignore[reportUnknownMemberType]
             dimension=0,
         )
         # merge faces
-        faces: FaceIndicesT = lax.concatenate(
-            [f + cumsum[i] for i, f in enumerate(fs)],
-            dimension=0,
+        faces: FaceIndicesT = (
+            lax.concatenate(  # pyright: ignore[reportUnknownMemberType]
+                [f + cumsum[i] for i, f in enumerate(fs)],
+                dimension=0,
+            )
         )
 
         return verts, faces
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
-    def merge_maps(maps: MapsT) -> tuple[MapT, Shape2DT]:
+    def merge_maps(maps: MapsT) -> Tuple[MapT, Tuple[int, int]]:
         """Merge maps by concatenating them along the first axis.
 
         All maps must have the same number of dimensions, i.e., `len(m.shape)`
         must be the same for all maps `m`.
 
         If the other axises is not the same, they are padded with undefined
         values, keeping [0:shape[i]] as given values, and [shape[i]:] being
@@ -242,51 +261,57 @@
           - maps: a list of maps to merge.
 
         Returns:
           - A merged map.
           - shape of first and second axis of each map.
         """
         # TODO: find a better way to merge maps
-        dims: int = len(maps[0].shape)
-        shapes: PyTree[tuple[Integer[Array, ""], ...], ...]
-        shapes = tree_map(lambda m: m.shape, maps)
-        # pick the largest shape for each dimension
-        single_shape: tuple[Integer[Array, ""], ...]
-        single_shape = tuple(
-            (max((shape[i] for shape in shapes)) for i in range(dims)))
+        with jax.ensure_compile_time_eval():
+            dims: int = len(maps[0].shape)
+            shapes: Sequence[Tuple[int, ...]]
+            shapes = tree_map(lambda m: m.shape, maps)
+            # pick the largest shape for each dimension
+            single_shape: Tuple[int, ...] = cast(
+                Tuple[int, ...],
+                tuple(
+                    (
+                        max((shape[i] for shape in shapes))  # pyright: ignore
+                        for i in range(dims)
+                    )
+                ),
+            )
 
-        dtype = jax.dtypes.result_type(*maps)
+            dtype = jax.dtypes.result_type(*maps)  # pyright: ignore
 
-        new_map = lax.concatenate(
+        new_map = lax.concatenate(  # pyright: ignore[reportUnknownMemberType]
             tree_map(
-                lambda m: lax.pad(
+                lambda m: lax.pad(  # pyright: ignore[reportUnknownMemberType]
                     m,
-                    jnp.array(0, dtype=m.dtype),
+                    jnp.array(0, dtype=m.dtype),  # pyright: ignore
                     tree_map(
                         lambda capacity, content: (0, capacity - content, 0),
                         single_shape,
                         m.shape,
                     ),
                 ).astype(dtype),
                 maps,
             ),
             dimension=0,
         )
 
-        return new_map, single_shape[:2]
+        return new_map, (single_shape[0], single_shape[1])
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
     @add_tracing_name
     def uv_repeat(
         uv: Float[Array, "2"],
         shape: Integer[Array, "2"],
-        map_index: Integer[Array, ""],
-        offset: Integer[Array, ""],
+        map_index: IntV,
+        offset: IntV,
     ) -> Float[Array, "2"]:
         """Compute final UV coordinates as if it is repeatedly tiled (in case
             of out-of-bound uv coordinate).
 
         Parameters:
           - uv: raw uv coordinates, in floating numbers. Only fractional part
             is used, as if the uv coordinates are in [0, 1].
@@ -294,52 +319,55 @@
           - offset: of each map in the merged maps, as [0] returned by
             `merge_maps`. Only first axis is required, thus here we just need a
             scalar.
           - map_index: index of the map to use.
         """
         assert isinstance(uv, Float[Array, "2"]), f"{uv}"
         assert isinstance(shape, Integer[Array, "2"]), f"{shape}"
-        assert isinstance(map_index, Integer[Array, ""]), f"{map_index}"
-        assert isinstance(offset, Integer[Array, ""]), f"{offset}"
+        assert isinstance(map_index, IntV), f"{map_index}"
+        assert isinstance(offset, IntV), f"{offset}"
         # since given uv are in [0, 1] (and may be scaled, if is cube),
         # we need to multiply it by (w, h) of the texture map first.
         # This is equivalent to just obtain the fractional part of uv.
-        fractional_uv, _ = jnp.modf(uv)
-        fractional_uv = jnp.where(
+        fractional_uv: FloatV = cast(FloatV, jnp.modf(uv)[0])
+        fractional_uv = jnp.where(  # pyright: ignore[reportUnknownMemberType]
             fractional_uv < 0,
             fractional_uv + 1,
             fractional_uv,
         )
         assert isinstance(fractional_uv, Float[Array, "2"])
 
         return (fractional_uv * shape).at[0].add(map_index * offset)
 
 
 class ModelObject(NamedTuple):
     """Model object with model and transform."""
+
     model: Model
     """Reference to the model, with mesh, attached maps, etc."""
-    local_scaling: Vec3f = jnp.ones(3)
+    local_scaling: Vec3f = jnp.ones(3)  # pyright: ignore[reportUnknownMemberType]
     """Local scaling factors of the object, in x, y, z."""
-    transform: ModelMatrix = jnp.identity(4)
+    transform: ModelMatrix = jnp.identity(4)  # pyright: ignore[reportUnknownMemberType]
     """Transform matrix (model matrix) of the model."""
     # TODO: Support double_sided
-    double_sided: Bool[Array, ""] = FALSE_ARRAY
+    double_sided: BoolV = FALSE_ARRAY
     """Whether the object is double-sided."""
 
     @jaxtyped
     def replace_with_position(self, position: Vec3f) -> "ModelObject":
         """Return a new ModelObject with given position.
 
         !!This does not change the original object.
 
         Parameters:
           - position: the new position of the object.
         """
-        return self._replace(transform=self.transform.at[:3, 3].set(position))
+        return self._replace(
+            transform=self.transform.at[:3, 3].set(position)  # pyright: ignore
+        )
 
     @jaxtyped
     def replace_with_orientation(
         self,
         orientation: Optional[Vec4f] = None,
         rotation_matrix: Optional[Float[Array, "3 3"]] = None,
     ) -> "ModelObject":
@@ -352,65 +380,68 @@
 
         Parameters:
           - orientation: the new orientation of the object, optional.
           - rotation_matrix: the new rotation matrix of the object, optional
         """
         if rotation_matrix is None:
             if orientation is None:
-                orientation = jnp.array((0., 0., 0., 1.))
+                orientation = jnp.array((0.0, 0.0, 0.0, 1.0))  # pyright: ignore
 
             assert isinstance(orientation, Vec4f), f"{orientation}"
             rotation_matrix = transform_matrix_from_rotation(orientation)
 
         assert isinstance(
             rotation_matrix,
             Float[Array, "3 3"],
         ), f"{rotation_matrix}"
 
         return self._replace(
-            transform=self.transform.at[:3, :3].set(rotation_matrix))
+            transform=self.transform.at[:3, :3].set(rotation_matrix)  # pyright: ignore
+        )
 
     @jaxtyped
-    def replace_with_local_scaling(
-        self,
-        local_scaling: Vec3f,
-    ) -> "ModelObject":
+    def replace_with_local_scaling(self, local_scaling: Vec3f) -> "ModelObject":
         """Return a new ModelObject with given local_scaling.
 
         !!This does not change the original object.
 
         Parameters:
           - local_scaling: the new local scaling of the object.
         """
         return self._replace(local_scaling=local_scaling)
 
     @jaxtyped
-    def replace_with_double_sided(
-        self,
-        double_sided: Bool[Array, ""],
-    ) -> "ModelObject":
+    def replace_with_double_sided(self, double_sided: BoolV) -> "ModelObject":
         """Return a new ModelObject with given double_sided.
 
         !!This does not change the original object.
 
         Parameters:
           - double_sided: whether the object is double-sided.
         """
         return self._replace(double_sided=double_sided)
 
 
 @add_tracing_name
 def batch_models(models: Sequence[MergedModel]) -> MergedModel:
     """Merge multiple MergedModel into one, with each field being a batch, with
-        batch axis at 0. This is intended to facilitate `jax.vmap`.
+    batch axis at 0. This is intended to facilitate `jax.vmap`.
     """
-    merged_model = MergedModel._make((lax.concatenate(
-        [jnp.asarray(model[i])[None, ...] for model in models],
-        dimension=0,
-    ) for i in range(len(models[0]))))
+    merged_model = MergedModel._make(
+        (
+            lax.concatenate(  # pyright: ignore[reportUnknownMemberType]
+                [
+                    jnp.asarray(model[i])[None, ...]  # pyright: ignore
+                    for model in models
+                ],
+                dimension=0,
+            )
+            for i in range(len(models[0]))
+        )
+    )
 
     return merged_model
 
 
 @jaxtyped
 @add_tracing_name
 def merge_objects(objects: Sequence[ModelObject]) -> MergedModel:
@@ -421,80 +452,83 @@
 
     Returns: A model containing the merged objects into one single mesh.
     """
     with jax.ensure_compile_time_eval():
         models = [obj.model for obj in objects]
 
         # broadcasted per vertex info
-        counts: list[int] = [len(m.verts) for m in models]
+        counts: List[int] = [len(m.verts) for m in models]
 
         map_indices: Integer[Array, "vertices"]
         map_indices = MergedModel.generate_object_vert_info(
             counts,
             list(range(len(models))),
         )
         assert isinstance(map_indices, Integer[Array, "vertices"])
 
-        map_wh_per_object = jnp.asarray(
-            [m.diffuse_map.shape[:2] for m in models])
+        map_wh_per_object = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+            [m.diffuse_map.shape[:2] for m in models]
+        )
         assert isinstance(map_wh_per_object, Integer[Array, "objects 2"])
 
         double_sided: Bool[Array, "vertices"]
         double_sided = MergedModel.generate_object_vert_info(
             counts,
             [obj.double_sided for obj in objects],
         )
         assert isinstance(double_sided, Bool[Array, "vertices"])
 
     # merge maps
     diffuse_map, single_map_shape = MergedModel.merge_maps(
-        [m.diffuse_map for m in models])
-    specular_map, _ = MergedModel.merge_maps([m.specular_map for m in models])
+        [m.diffuse_map for m in models]
+    )
+    specular_map = MergedModel.merge_maps([m.specular_map for m in models])[0]
 
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def transform_vert(
         verts: Float[Array, "N 3"],
         local_scaling: Vec3f,
         transform: ModelMatrix,
     ) -> Vertices:
         """Apply transforms defined in `ModelObject` to vertices."""
-        world: Float[Array, "N 3"] = Camera.apply_pos(
-            verts * local_scaling,
-            transform,
-        )
+        world: Float[Array, "N 3"] = Camera.apply_pos(verts * local_scaling, transform)
         assert isinstance(world, Float[Array, "N 3"])
 
         return world
 
     # merge verts
     verts, faces = MergedModel.merge_verts(
         [
             transform_vert(
                 verts=obj.model.verts,
                 local_scaling=obj.local_scaling,
                 transform=obj.transform,
-            ) for obj in objects
+            )
+            for obj in objects
         ],
         [m.faces for m in models],
     )
 
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def transform_normals(
         normals: Float[Array, "N 3"],
         transform: ModelMatrix,
     ) -> Vertices:
         """Apply transforms defined in `ModelObject` to vertex normals."""
-        world: Float[Array, "N 3"] = Camera.apply_vec(
-            normals,
-            # transform by inverse transpose
-            jnp.linalg.inv(transform).T,
+        world: Float[Array, "N 3"] = cast(
+            Float[Array, "N 3"],
+            Camera.apply_vec(
+                normals,
+                # transform by inverse transpose
+                jnp.linalg.inv(transform).T,  # pyright: ignore
+            ),
         )
         assert isinstance(world, Float[Array, "N 3"])
 
         return world
 
     norms, faces_norm = MergedModel.merge_verts(
         [transform_normals(obj.model.norms, obj.transform) for obj in objects],
```

### Comparing `jaxrenderer-0.3.1/renderer/pipeline.py` & `jaxrenderer-0.3.2/renderer/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,230 +1,266 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import Any, NamedTuple
+from typing import Any, NamedTuple, TypeVar, cast
 
 import jax
+from jax import lax
 import jax.lax as lax
 import jax.numpy as jnp
-from jax import lax
 from jax.tree_util import tree_map
-from jaxtyping import Array, Bool, Float, Integer, Num, jaxtyped
+from jaxtyping import Array, Bool, Float, Integer, Num
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
-from ._backport import Tuple, TypeAlias
+from ._backport import Tuple
 from ._meta_utils import add_tracing_name
+from ._meta_utils import typed_jit as jit
 from .geometry import Camera, Interpolation, Viewport, interpolate
-from .shader import (ID, MixedExtraT, MixerOutput, PerFragment, PerVertex,
-                     Shader, ShaderExtraInputT, VaryingT)
-from .types import (FALSE_ARRAY, Buffers, CanvasMask, FaceIndices, Triangle,
-                    Vec2f, Vec2i, Vec3f, Vec4f, ZBuffer)
+from .shader import (
+    ID,
+    MixedExtraT,
+    MixerOutput,
+    PerFragment,
+    PerVertex,
+    Shader,
+    ShaderExtraInputT,
+    VaryingT,
+)
+from .types import (
+    BoolV,
+    Buffers,
+    CanvasMask,
+    FaceIndices,
+    FloatV,
+    IntV,
+    Triangle,
+    Vec2f,
+    Vec2i,
+    Vec3f,
+    Vec4f,
+    ZBuffer,
+)
 
-jax.config.update('jax_array', True)
+jax.config.update("jax_array", True)  # pyright: ignore[reportUnknownMemberType]
 
 RowIndices = Integer[Array, "row_batches row_batch_size"]
 """Indices of the rows in the buffers to be processed in this batch."""
 
 
 class PerPrimitive(NamedTuple):
     """Input for each primitive, using outputs from Vertex Shader.
 
     gl_Position is in clip-space, not normalised.
     """
+
     gl_Position: Triangle
     # gl_PointSize is meaningful only when rendering point primitives.
     # not supported for now
     # gl_PointSize: Float[Array, "primitives"]
-    keep: Bool[Array, ""]
+    keep: BoolV
     """Whether to keep this primitive for rasterisation.
         !!Never keep a primitive with a zero determinant.
     """
-    determinant: Float[Array, ""]
+    determinant: FloatV
     """determinant of the matrix with [x, y, w] of the three vertices in clip
         space, in a shape of
 
         [[x0, y0, w0],
          [x1, y1, w1],
          [x2, y2, w2]].
 
         When determinant is 0, the triangle will not be rendered for now.
     """
     matrix_inv: Float[Array, "3 3"]
     """inverse of the matrix described above (of [x, y, w])."""
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @partial(jit, static_argnames=("cls",), inline=True)
     @add_tracing_name
     def create(cls, per_vertex: PerVertex) -> "PerPrimitive":
         """per_vertex is batched with size 3 (3 vertices per triangle)
-            in clip-space, not normalised.
+        in clip-space, not normalised.
         """
         clip: Triangle = per_vertex.gl_Position
         assert isinstance(clip, Triangle)
         # matrix with x, y, w
-        matrix: Float[Array, "3 3"] = clip[:, jnp.array((0, 1, 3))]
+        matrix: Float[Array, "3 3"] = clip[:, jnp.array((0, 1, 3))]  # pyright: ignore
         # If == 0, the matrix inverse does not exist, should use another
         # interpolation method. Early exit for now.
         # `jnp.linalg.det` has built-in 3x3 det optimisation
-        determinant: Float[Array, ""] = jnp.linalg.det(matrix)
-        assert isinstance(determinant, Float[Array, ""])
+        determinant = cast(
+            FloatV,
+            jnp.linalg.det(matrix),  # pyright: ignore[reportUnknownMemberType]
+        )
+        assert isinstance(determinant, FloatV)
 
         # an arbitrary number for numerical stability
-        keep: Bool[Array, ""] = lax.abs(determinant) > 1e-6
+        keep: BoolV = (
+            lax.abs(determinant) > 1e-6  # pyright: ignore[reportUnknownMemberType]
+        )
 
         # although this may result in NaN or Inf when keep is False,
         # it will be discarded later.
         # Perf: Remove lax.cond to reduce extra operations `select_n` in HLO.
-        mat_inv: Float[Array, "3 3"] = jnp.linalg.inv(matrix)
+        mat_inv = cast(Float[Array, "3 3"], jnp.linalg.inv(matrix))
         assert isinstance(mat_inv, Float[Array, "3 3"])
 
         return cls(
             gl_Position=clip,
             keep=keep,
             determinant=determinant,
             matrix_inv=mat_inv,
         )
 
 
+T = TypeVar("T", bound=Tuple[Any, ...])
+
+
 @jaxtyped
 @partial(
-    jax.jit,
+    jit,
     static_argnames=("shader", "loop_unroll"),
-    donate_argnums=(1, ),
+    donate_argnums=(1,),
     inline=True,
 )
 @add_tracing_name
 def _postprocessing(
     shader: type[Shader[ShaderExtraInputT, VaryingT, MixedExtraT]],
-    buffers: Buffers,
-    per_primitive: tuple[Any, ...],  # Batch PerPrimitive
+    buffers: Buffers[T],
+    per_primitive: Tuple[Any, ...],  # Batch PerPrimitive
     varyings: VaryingT,
     extra: ShaderExtraInputT,
     viewport: Viewport,
     loop_unroll: int,
-) -> Buffers:
+) -> Buffers[T]:
     with jax.ensure_compile_time_eval():
         # vmap batch along second axis
         batch_size: int = int(buffers[0].shape[1])
         row_indices: Integer[Array, "width"]
-        row_indices = lax.iota(int, int(buffers[0].shape[0]))
+        row_indices = lax.iota(  # pyright: ignore[reportUnknownMemberType]
+            int, int(buffers[0].shape[0])
+        )
 
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
-    def _per_pixel(coord: Vec2i) -> tuple[MixerOutput, MixedExtraT]:
-
+    def _per_pixel(coord: Vec2i) -> Tuple[MixerOutput, MixedExtraT]:
         assert isinstance(coord, Vec2i), f"expected Vec2i, got {coord}"
 
         ReturnT = Tuple[  #
             Float[Array, "kept_primitives 4"],  #
             Bool[Array, "kept_primitives"],  #
             Float[Array, "kept_primitives 2"],  #
             Bool[Array, "kept_primitives"],  #
             VaryingT,  #
             Float[Array, "kept_primitives 3"],  #
             Float[Array, "kept_primitives 3"],  #
         ]
 
         @jaxtyped
-        @partial(jax.jit, inline=True)
+        @partial(jit, inline=True)
         @add_tracing_name
         def _per_primitive_preprocess(
             primitive: PerPrimitive,
             varying_per_primitive: VaryingT,
         ) -> ReturnT:
             # PROCESS: Early Culling (`primitive_chooser`)
 
             # For early exit when not keep primitive / determinant is 0
-            @partial(jax.jit, inline=True)
+            @partial(jit, inline=True)
             @add_tracing_name
-            def _when_keep_primitive() -> tuple[Vec3f, Float[Array, ""]]:
+            def _when_keep_primitive() -> Tuple[Vec3f, FloatV]:
                 """Returns clip_coef, w_reciprocal."""
                 # x/w, y/w, with x, y, w in clip space.
-                xy: Float[Array, "2"] = (
-                    (coord - viewport[:2, 3]) /
-                    viewport[jnp.arange(2), jnp.arange(2)])
-                xy1_ndc: Float[Array, "3"] = jnp.array((xy[0], xy[1], 1))
+                _idx: Integer[Array, "2"]
+                _idx = jnp.arange(2)  # pyright: ignore[reportUnknownMemberType]
+                xy: Float[Array, "2"] = (coord - viewport[:2, 3]) / viewport[_idx, _idx]
+                xy1_ndc: Float[Array, "3"]
+                xy1_ndc = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+                    (xy[0], xy[1], 1)
+                )
 
                 # As the interpolation formula is `xy1_ndc @ (mat_inv @ values)`
                 # we can utilise associativity to generate a set of fixed Vec3f
                 # coefficient for interpolation.
                 # Noticed that this is also the "edge function" values, with
                 # a pseudo-parameter that is zero at the two vertices on the
                 # edge and one at the opposite vertex, as described
                 # in [Olano and Greer, 1997].
-                clip_coef: Vec3f = jnp.dot(xy1_ndc, primitive.matrix_inv)
+                clip_coef = cast(Vec3f, jnp.dot(xy1_ndc, primitive.matrix_inv))
                 assert isinstance(clip_coef, Vec3f)
                 # 1/w, w in clip space.
-                w_reciprocal: Float[Array, ""] = clip_coef.sum()
-                assert isinstance(w_reciprocal, Float[Array, ""])
+                w_reciprocal: FloatV = clip_coef.sum()  # pyright: ignore
+                assert isinstance(w_reciprocal, FloatV)
 
                 return clip_coef, w_reciprocal
 
             # END OF `_when_keep_primitive`
 
-            @partial(jax.jit, inline=True)
+            @partial(jit, inline=True)
             @add_tracing_name
             def _when_in_triangle(
                 clip_coef: Vec3f,
-                w_reciprocal: Float[Array, ""],
-            ) -> tuple[  #
-                    Float[Array, "kept_primitives 4"],  # gl_FragCoord
-                    Bool[Array, "kept_primitives"],  # gl_FrontFacing
-                    Float[Array, "kept_primitives 2"],  # gl_PointCoord
-                    Float[Array, "kept_primitives 3"],  # true_clip_coef
+                w_reciprocal: FloatV,
+            ) -> Tuple[  #
+                Float[Array, "kept_primitives 4"],  # gl_FragCoord
+                Bool[Array, "kept_primitives"],  # gl_FrontFacing
+                Float[Array, "kept_primitives 2"],  # gl_PointCoord
+                Float[Array, "kept_primitives 3"],  # true_clip_coef
             ]:
                 # Prepare inputs for fragment shader
-                z: Float[Array, ""] = interpolate(
+                z: FloatV = interpolate(
                     values=primitive.gl_Position[:, 2],
                     barycentric_screen=clip_coef,
                     barycentric_clip=clip_coef,
                     mode=Interpolation.SMOOTH,
                 )
                 # viewport transform for z, from clip space to window space
                 z = z * viewport[2, 2] + viewport[2, 3]
-                gl_FragCoord: Vec4f = jnp.array((
-                    coord[0],
-                    coord[1],
-                    z,
-                    w_reciprocal,
-                ))
+                gl_FragCoord: Vec4f = jnp.array(  # pyright: ignore
+                    (
+                        coord[0],
+                        coord[1],
+                        z,
+                        w_reciprocal,
+                    )
+                )
                 assert isinstance(gl_FragCoord, Vec4f)
 
                 # Ref: https://registry.khronos.org/OpenGL-Refpages/gl4/html/gl_FrontFacing.xhtml
                 # True if not back-facing.
-                gl_FrontFacing: Bool[Array, ""] = primitive.determinant >= 0
-                assert isinstance(gl_FrontFacing, Bool[Array, ""])
+                gl_FrontFacing: BoolV = primitive.determinant >= 0
+                assert isinstance(gl_FrontFacing, BoolV)
 
                 gl_PointCoord: Vec2f
                 with jax.ensure_compile_time_eval():
                     # TODO: implement Point primitive properly.
-                    gl_PointCoord = lax.full((2, ), 0.)
+                    gl_PointCoord = lax.full((2,), 0.0)  # pyright: ignore
 
                 # this interpolates to target value u, not u/w
                 true_clip_coef: Vec3f = clip_coef / w_reciprocal
                 assert isinstance(true_clip_coef, Vec3f)
 
-                return (gl_FragCoord, gl_FrontFacing, gl_PointCoord,
-                        true_clip_coef)
+                return (gl_FragCoord, gl_FrontFacing, gl_PointCoord, true_clip_coef)
 
             # END OF `_when_in_triangle`
 
             # Prepare for interpolation parameters
             # clip_coef here interpolates to 1/w * target value
             # Perf: although this may result in garbage values (NaN or Inf)
             # when keep is False, since it will be discarded later, we can
             # remove the lax.cond to reduce extra operations `select_n` in HLO
             # as the computation is quite cheap.
             # also see google/brax#8409 for why `_when_keep_primitive` is
             # always executed.
             clip_coef, w_reciprocal = _when_keep_primitive()
 
-            in_triangle: Bool[Array, ""] = (clip_coef >= 0).all()
-            assert isinstance(in_triangle, Bool[Array, ""])
+            in_triangle: BoolV = (clip_coef >= 0).all()  # pyright: ignore
+            assert isinstance(in_triangle, BoolV)
 
             # Perf: although this may result in garbage values (NaN or Inf)
             # when keep or in_triangle is False, since it will be discarded
             # later, we can remove the lax.cond to reduce extra operations
             # `select_n` in HLO.
             # See google/brax#8409 for why `_when_keep_primitive` is always
             # executed.
@@ -240,25 +276,25 @@
                 varying_per_primitive,
                 true_clip_coef,
                 true_clip_coef,
             )
 
         # END OF `_per_primitive_preprocess`
 
-        @partial(jax.jit, inline=True)
+        @partial(jit, inline=True)
         @add_tracing_name
         def _interpolate_and_fragment_shading(
             gl_FragCoord: Vec4f,
-            gl_FrontFacing: Bool[Array, ""],
+            gl_FrontFacing: BoolV,
             gl_PointCoord: Vec2f,
-            keeps: Bool[Array, ""],
+            keeps: BoolV,
             values: VaryingT,
             barycentric_screen: Vec3f,
             barycentric_clip: Vec3f,
-        ) -> tuple[PerFragment, VaryingT]:
+        ) -> Tuple[PerFragment, VaryingT]:
             # PROCESS: Interpolation
             varying: VaryingT = shader.interpolate(
                 values=values,
                 barycentric_screen=barycentric_screen,
                 barycentric_clip=barycentric_clip,
             )
             assert isinstance(varying, tuple)
@@ -273,29 +309,32 @@
                 varying=varying,
                 extra=extra,
             )
             assert isinstance(per_frag, PerFragment)
             assert isinstance(extra_fragment_output, tuple)
 
             # enforce default `gl_FragDepth` when `use_default_depth`
-            per_frag = lax.cond(
-                per_frag.use_default_depth,
-                lambda: per_frag._replace(gl_FragDepth=gl_FragCoord[2]),
-                lambda: per_frag,
+            per_frag = cast(
+                PerFragment,
+                lax.cond(  # pyright: ignore[reportUnknownMemberType]
+                    per_frag.use_default_depth,
+                    lambda: per_frag._replace(gl_FragDepth=gl_FragCoord[2]),
+                    lambda: per_frag,
+                ),
             )
             assert isinstance(per_frag, PerFragment)
 
             per_frag = per_frag._replace(keeps=keeps & per_frag.keeps)
 
             return per_frag, extra_fragment_output
 
         # END OF `_interpolate_fragment_shading`
 
         args = jax.vmap(_per_primitive_preprocess)(
-            per_primitive,
+            per_primitive,  # pyright: ignore # need to find a way to express un-batch
             varyings,
         )
         chosen_args = shader.primitive_chooser(*args)
 
         built_in: PerFragment
         extra_outputs: VaryingT
         _f = jax.vmap(_interpolate_and_fragment_shading)
@@ -306,83 +345,96 @@
         keeps = built_in.keeps
         assert isinstance(gl_Depths, Float[Array, "kept_primitives"])
         assert isinstance(keeps, Bool[Array, "kept_primitives"])
 
         # PROCESS: Per-Sample Operations (Mixing: depth test + colour blending)
         mixed_output: MixerOutput
         attachments: MixedExtraT
-        mixed_output, attachments = shader.mix(gl_Depths, keeps, extra_outputs)
+        mixed_output, attachments = cast(
+            Tuple[MixerOutput, MixedExtraT],
+            shader.mix(gl_Depths, keeps, extra_outputs),
+        )
         assert isinstance(mixed_output, MixerOutput)
         assert isinstance(attachments, tuple)
 
         return mixed_output, attachments
 
     # END OF `_per_pixel`
 
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
-    def _per_row(i: Integer[Array, ""], ) -> tuple[MixerOutput, MixedExtraT]:
+    def _per_row(
+        i: IntV,
+    ) -> Tuple[MixerOutput, MixedExtraT]:
         """Render one row.
 
         Parameters:
           - i: the index of the row to be rendered on the first axis of the
             resultant buffer.
 
         Returns: one row from `Shader.mixer`, `MixerOutput` and `MixerExtraT`.
         """
         keeps: Bool[Array, "height"]
         depths: Num[Array, "height"]
         extras: MixedExtraT
         # vmap over axis 1 (height) of the buffers. Axis 0 (width) is `i`.
-        (keeps, depths), extras = jax.vmap(_per_pixel)(lax.concatenate(
-            (
-                lax.full((batch_size, 1), i),
-                lax.broadcasted_iota(int, (batch_size, 1), 0),
-            ),
-            1,
-        ))
+        (keeps, depths), extras = jax.vmap(_per_pixel)(
+            lax.concatenate(  # pyright: ignore[reportUnknownMemberType]
+                (
+                    lax.full((batch_size, 1), i),  # pyright: ignore
+                    lax.broadcasted_iota(int, (batch_size, 1), 0),  # pyright: ignore
+                ),
+                1,
+            )
+        )
         assert isinstance(keeps, Bool[Array, "height"])
         assert isinstance(depths, Num[Array, "height"])
         assert isinstance(extras, tuple)
 
         return MixerOutput(keep=keeps, zbuffer=depths), extras
 
     # END OF `_per_row`
 
     @jaxtyped
-    @partial(jax.jit, donate_argnums=(1, ), inline=True)
+    @partial(jit, donate_argnums=(1,), inline=True)
     @add_tracing_name
     def merge_buffers(
-        mixer_outputs: tuple[MixerOutput, MixedExtraT],
-        old_buffers: Buffers,
-    ) -> Buffers:
+        mixer_outputs: Tuple[MixerOutput, MixedExtraT],
+        old_buffers: Buffers[T],
+    ) -> Buffers[T]:
         """Merge the rendered row into the buffers.
 
         Parameters:
           - mixer_outputs: the output from `Shader.mixer`, `MixerOutput` and
             `MixerExtraT`.
           - old_buffers: the buffers to be updated.
 
         Returns: the updated buffers.
         """
         keeps: CanvasMask = mixer_outputs[0].keep
         depths: ZBuffer = mixer_outputs[0].zbuffer
         extras: MixedExtraT = mixer_outputs[1]
 
-        @partial(jax.jit, donate_argnums=(2, ), inline=True)
-        def _merge_first_axis(_mask, _new, _old):
+        S = TypeVar("S")
 
-            @partial(jax.jit, donate_argnums=(2, ), inline=True)
-            def _merge_second_axis(__mask, __new, __old):
-                return lax.cond(__mask, lambda: __new, lambda: __old)
+        @partial(jit, donate_argnums=(2,), inline=True)
+        def _merge_first_axis(_mask: Bool[Array, "_"], _new: S, _old: S) -> S:
+            @partial(jit, donate_argnums=(2,), inline=True)
+            def _merge_second_axis(__mask: BoolV, __new: S, __old: S) -> S:
+                return cast(
+                    S,
+                    lax.cond(  # pyright: ignore[reportUnknownMemberType]
+                        __mask, lambda: __new, lambda: __old
+                    ),
+                )
 
             return jax.vmap(_merge_second_axis)(_mask, _new, _old)
 
-        new_buffers: Buffers = tree_map(
+        new_buffers: Buffers[T] = tree_map(
             lambda new, old: jax.vmap(_merge_first_axis)(keeps, new, old),
             Buffers(zbuffer=depths, targets=tuple(extras)),
             old_buffers,
         )
         assert isinstance(new_buffers, Buffers)
 
         return new_buffers
@@ -405,49 +457,51 @@
     assert isinstance(buffers, Buffers)
 
     return buffers
 
 
 @jaxtyped
 @partial(
-    jax.jit,
+    jit,
     static_argnames=("shader", "loop_unroll"),
-    donate_argnums=(2, ),
+    donate_argnums=(2,),
     inline=True,
 )
 @add_tracing_name
 def render(
     camera: Camera,
     shader: type[Shader[ShaderExtraInputT, VaryingT, MixedExtraT]],
-    buffers: Buffers,
+    buffers: Buffers[T],
     face_indices: FaceIndices,
     extra: ShaderExtraInputT,
     loop_unroll: int = 1,
-) -> Buffers:
+) -> Buffers[T]:
     """Render a scene with a shader.
 
     Parameters:
       - loop_unroll: the number of rows to be rendered in one loop. This may
         help improve the performance at the cost of increasing compilation time.
         Default: 1
     """
     vertices_count: int
     gl_InstanceID: ID
     with jax.ensure_compile_time_eval():
-        vertices_count = extra[0].shape[0]
-        gl_InstanceID = jnp.array(0, dtype=int)
+        assert len(extra) > 0
+        assert isinstance(extra[0], Num[Array, "*"])
+        vertices: Num[Array, "*"] = cast(Num[Array, "*"], extra[0])
+        vertices_count: int = vertices.shape[0]
+
+        gl_InstanceID = jnp.array(0, dtype=int)  # pyright: ignore
         assert isinstance(vertices_count, int)
         assert isinstance(gl_InstanceID, ID)
 
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
-    def vertex_processing(
-            gl_VertexID: Integer[Array, ""],  #
-    ) -> tuple[PerVertex, VaryingT]:
+    def vertex_processing(gl_VertexID: IntV) -> Tuple[PerVertex, VaryingT]:
         """Process one vertex into screen space, and keep varying values."""
         per_vertex: PerVertex
         varying: VaryingT
         per_vertex, varying = shader.vertex(
             gl_VertexID,
             gl_InstanceID,
             camera,
@@ -456,25 +510,27 @@
         assert isinstance(per_vertex, PerVertex)
         assert isinstance(varying, tuple)
 
         return per_vertex, varying
 
     # PROCESS: Vertex Processing
     per_vertices, varyings = jax.vmap(vertex_processing)(
-        lax.iota(int, vertices_count),  # gl_VertexID
+        lax.iota(int, vertices_count),  # gl_VertexID # pyright: ignore
     )
 
     # everything after vertex processing, will directly update buffers
     buffers = _postprocessing(
         shader=shader,
         buffers=buffers,
-        per_primitive=jax.vmap(PerPrimitive.create)(tree_map(
-            lambda field: field[face_indices],
-            per_vertices,
-        )),
+        per_primitive=jax.vmap(PerPrimitive.create)(
+            tree_map(
+                lambda field: field[face_indices],
+                per_vertices,
+            )
+        ),
         varyings=tree_map(lambda field: field[face_indices], varyings),
         extra=extra,
         viewport=camera.viewport,
         loop_unroll=loop_unroll,
     )
     assert isinstance(buffers, Buffers)
```

### Comparing `jaxrenderer-0.3.1/renderer/renderer.py` & `jaxrenderer-0.3.2/renderer/renderer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,191 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import NamedTuple, Optional, Sequence, Union
+from typing import Any, NamedTuple, Optional, Sequence, TypeVar, Union, cast
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import tree_map
-from jaxtyping import Array, Bool, Integer, Num, jaxtyped
+from jaxtyping import Array, Bool, Integer
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
+from ._backport import Tuple, TypeAlias
 from ._meta_utils import add_tracing_name
+from ._meta_utils import typed_jit as jit
 from .geometry import Camera, Projection, View, Viewport, normalise
 from .model import MergedModel, ModelObject, merge_objects
 from .pipeline import render
-from .shaders.phong_reflection import (PhongReflectionTextureExtraInput,
-                                       PhongReflectionTextureShader)
+from .shaders.phong_reflection import (
+    PhongReflectionTextureExtraInput,
+    PhongReflectionTextureShader,
+)
 from .shaders.phong_reflection_shadow import (
-    PhongReflectionShadowTextureExtraInput, PhongReflectionShadowTextureShader)
+    PhongReflectionShadowTextureExtraInput,
+    PhongReflectionShadowTextureShader,
+)
 from .shadow import Shadow
-from .types import (Buffers, Canvas, Colour, DtypeInfo, LightSource, Vec3f,
-                    ZBuffer)
+from .types import (
+    Buffers,
+    Canvas,
+    Colour,
+    DtypeInfo,
+    FloatV,
+    LightSource,
+    NumV,
+    Vec3f,
+    ZBuffer,
+)
 
-DoubleSidedFaces = Bool[Array, "faces"]
+DoubleSidedFaces: TypeAlias = Bool[Array, "faces"]
 """Whether to render both sides of each face (triangle primitive)."""
 
+TargetT = TypeVar("TargetT", bound=Tuple[Any])
+
 
 class CameraParameters(NamedTuple):
     """Parameters for rendering from camera.
 
     Default values come from [erwincoumans/tinyrenderer::TinyRendererCamera](https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/python/pytinyrenderer.cc#L56)
     """
+
     viewWidth: int = 640
     """width of the viewport."""
     viewHeight: int = 480
     """height of the viewport."""
-    viewDepth: float = 1.
+    viewDepth: float = 1.0
     """depth of the rendered view."""
     near: float = 0.01
     """near clipping plane."""
-    far: float = 1000.
+    far: float = 1000.0
     """far clipping plane."""
-    hfov: float = 58.
+    hfov: float = 58.0
     """horizontal field of view, in degrees."""
-    vfov: float = 45.
+    vfov: float = 45.0
     """vertical field of view, in degrees."""
-    position: Union[Vec3f, tuple[float, float, float]] = jnp.ones(3)
+    position: Union[Vec3f, Tuple[float, float, float]] = jnp.ones(3)  # pyright: ignore
     """position of the camera in world space."""
-    target: Union[Vec3f, tuple[float, float, float]] = jnp.zeros(3)
+    target: Union[Vec3f, Tuple[float, float, float]] = jnp.zeros(3)  # pyright: ignore
     """target of the camera."""
-    up: Union[Vec3f, tuple[float, float, float]] = jnp.array((0., 0., 1.))
+    up: Union[Vec3f, Tuple[float, float, float]] = jnp.array(  # pyright: ignore
+        (0.0, 0.0, 1.0)
+    )
     """up direction of the camera."""
 
 
 class LightParameters(NamedTuple):
     """Parameters for directional light in rendering.
 
     Default values come from [erwincoumans/tinyrenderer::TinyRenderLight](https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/python/pytinyrenderer.cc#L74).
     """
-    direction: Vec3f = normalise(jnp.array((0.57735, 0.57735, 0.57735)))
+
+    direction: Vec3f = normalise(
+        jnp.array(  # pyright: ignore[reportUnknownMemberType]
+            (0.57735, 0.57735, 0.57735)
+        )
+    )
     """in world space, as it goes from that position to origin (camera).
 
     For example, if direction = camera's eye, full specular will be applied to
     triangles with normal towards camera.
     """
-    colour: Colour = jnp.ones(3)
+    colour: Colour = jnp.ones(3)  # pyright: ignore[reportUnknownMemberType]
     """Light source to render."""
-    ambient: Colour = jnp.array((0.6, 0.6, 0.6))
+    ambient: Colour = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (0.6, 0.6, 0.6)
+    )
     """Ambient colour. This is added to the final colour of the object."""
-    diffuse: Colour = jnp.array((0.35, 0.35, 0.35))
+    diffuse: Colour = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (0.35, 0.35, 0.35)
+    )
     """Diffuse coefficient per colour channel. This is multiplied to the
         diffuse texture colour of the object.
     """
-    specular: Colour = jnp.array((0.05, 0.05, 0.05))
+    specular: Colour = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (0.05, 0.05, 0.05)
+    )
     """Specular coefficient per colour channel. This is multiplied to the
         computed specular light colour.
     """
 
 
 class ShadowParameters(NamedTuple):
     """Parameters for rendering shadow map.
 
     Default values come from:
       - [erwincoumans/tinyrenderer::TinyRenderLight](https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/python/pytinyrenderer.cc#L74).
       - for `up`, [erwincoumans/tinyrenderer::renderObject](https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/tinyrenderer.cpp#L372).
     """
-    centre: Vec3f = jnp.zeros(3)
+
+    centre: Vec3f = jnp.zeros(3)  # pyright: ignore[reportUnknownMemberType]
     """centre of the scene, same as object's camera's centre."""
-    up: Vec3f = jnp.array((0., 0., 1.))
+    up: Vec3f = jnp.array((0.0, 0.0, 1.0))  # pyright: ignore[reportUnknownMemberType]
     """up direction of the scene, same as object's camera's up."""
-    strength: Colour = 1 - jnp.array((0.4, 0.4, 0.4))
+    strength: Colour = 1 - jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (0.4, 0.4, 0.4)
+    )
     """Strength of shadow. Must be in [0, 1]. 0 means no shadow, 1 means fully
         black shadow.  See `Shadow.strength` for more details.
     """
     offset: float = 0.05
     """Offset to avoid self-shadowing / z-fighting. This will be subtracted to
         the shadow map, making the shadows further away from the light.
     """
 
 
 class Renderer:
-
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def create_camera_from_parameters(camera: CameraParameters) -> Camera:
         """Create a camera from camera parameters."""
-        eye: Vec3f = jnp.asarray(camera.position, dtype=float)
+        eye: Vec3f = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+            camera.position, dtype=float
+        )
         assert isinstance(eye, Vec3f), f"{eye}"
-        centre: Vec3f = jnp.asarray(camera.target, dtype=float)
+        centre: Vec3f = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+            camera.target, dtype=float
+        )
         assert isinstance(centre, Vec3f), f"{centre}"
-        up: Vec3f = jnp.asarray(camera.up, dtype=float)
+        up: Vec3f = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+            camera.up, dtype=float
+        )
         assert isinstance(up, Vec3f), f"{up}"
 
         view_mat: View = Camera.view_matrix(eye=eye, centre=centre, up=up)
         assert isinstance(view_mat, View), f"{view_mat}"
         view_inv: View = Camera.view_matrix_inv(eye=eye, centre=centre, up=up)
         assert isinstance(view_inv, View), f"{view_inv}"
         projection_mat: Projection = Camera.perspective_projection_matrix(
             fovy=camera.vfov,
-            aspect=(lax.tan(jnp.radians(camera.hfov) / 2.) /
-                    lax.tan(jnp.radians(camera.vfov) / 2.)),
+            aspect=(
+                lax.tan(  # pyright: ignore[reportUnknownMemberType]
+                    cast(FloatV, jnp.radians(camera.hfov) / 2.0)
+                )
+                / lax.tan(  # pyright: ignore[reportUnknownMemberType]
+                    cast(FloatV, jnp.radians(camera.vfov) / 2.0)
+                )
+            ),
             z_near=camera.near,
             z_far=camera.far,
         )
         assert isinstance(projection_mat, Projection), f"{projection_mat}"
         viewport_mat: Viewport = Camera.viewport_matrix(
-            lowerbound=jnp.zeros(2, dtype=int),
-            dimension=jnp.array((camera.viewWidth, camera.viewHeight)),
-            depth=jnp.array(camera.viewDepth),
+            lowerbound=jnp.zeros(  # pyright: ignore[reportUnknownMemberType]
+                2,
+                dtype=int,
+            ),
+            dimension=jnp.array(  # pyright: ignore[reportUnknownMemberType]
+                (camera.viewWidth, camera.viewHeight)
+            ),
+            depth=jnp.array(  # pyright: ignore[reportUnknownMemberType]
+                camera.viewDepth
+            ),
         )
         assert isinstance(viewport_mat, Viewport), f"{viewport_mat}"
 
         _camera: Camera = Camera.create(
             view=view_mat,
             projection=projection_mat,
             viewport=viewport_mat,
@@ -145,17 +198,23 @@
     @staticmethod
     @jaxtyped
     @add_tracing_name
     def create_buffers(
         width: int,
         height: int,
         batch: Optional[int] = None,
-        colour_default: Colour = jnp.array((1., 1., 1.), dtype=jnp.single),
-        zbuffer_default: Num[Array, ""] = jnp.array(1, dtype=jnp.single),
-    ) -> Buffers:
+        colour_default: Colour = jnp.array(  # pyright: ignore[reportUnknownMemberType, reportCallInDefaultInitializer]
+            (1.0, 1.0, 1.0),
+            dtype=jnp.single,
+        ),
+        zbuffer_default: NumV = jnp.array(  # pyright: ignore[reportUnknownMemberType, reportCallInDefaultInitializer]
+            1,
+            dtype=jnp.single,
+        ),
+    ) -> Buffers[Tuple[Canvas]]:
         """Render the scene with the given camera.
 
         The dtype of `colour_default` and `zbuffer_default` will be used as the
         dtype of canvas and zbuffer.
 
         Parameters:
           - width, height: the size of the image to render.
@@ -163,71 +222,81 @@
             axis at axis 0.
           - colour_default: default colours to fill the image with.
           - zbuffer_default: default zbuffer values to fill with.
           - shadow_param: the shadow parameters to render the scene with. Keep
 
         Returns: Buffers, with zbuffer and (coloured image, ).
         """
-        _batch = (batch, ) if batch is not None else ()
-        zbuffer: ZBuffer = lax.full(
+        _batch = (batch,) if batch is not None else ()
+        zbuffer: ZBuffer = lax.full(  # pyright: ignore[reportUnknownMemberType]
             (*_batch, width, height),
             zbuffer_default,
         )
-        canvas: Canvas = jnp.full(
+        canvas: Canvas = jnp.full(  # pyright: ignore[reportUnknownMemberType]
             (*_batch, width, height, colour_default.size),
             colour_default,
         )
-        buffers: Buffers = Buffers(
+        buffers: Buffers[Tuple[Canvas]] = Buffers(
             zbuffer=zbuffer,
-            targets=(canvas, ),
+            targets=(canvas,),
         )
 
         return buffers
 
     @classmethod
     @jaxtyped
     @partial(
-        jax.jit,
+        jit,
         static_argnames=("cls", "loop_unroll"),
-        donate_argnums=(4, ),
+        donate_argnums=(4,),
         inline=True,
     )
     @add_tracing_name
     def render(
         cls,
         model: MergedModel,
         light: LightParameters,
         camera: Camera,
-        buffers: Buffers,
+        buffers: Buffers[TargetT],
         shadow_param: Optional[ShadowParameters] = None,
         loop_unroll: int = 1,
-    ) -> Buffers:
+    ) -> Buffers[TargetT]:
         """Render the scene with the given camera.
 
         Parameters:
           - model: merged model of all the objects to render.
           - light: the light to render the scene with.
           - camera: the camera to render the scene with.
           - buffers: the buffers to render the scene with.
           - shadow_param: the shadow parameters to render the scene with. Keep
             it None to disable shadows.
           - loop_unroll: passed directly to `render`. See `pipeline:render`.
 
         Returns: Buffers, with zbuffer and (coloured image, ).
         """
         # flatten so each vertex has its own "extra"
-        position = model.verts[model.faces.reshape((-1, ))]
-        normal = model.norms[model.faces_norm.reshape((-1, ))]
-        uv = model.uvs[model.faces_uv.reshape((-1, ))]
-
-        texture_index = model.texture_index[model.faces_uv.reshape((-1, ))]
-        double_sided = model.texture_index[model.faces_uv.reshape((-1, ))]
+        position = model.verts[
+            model.faces.reshape((-1,))  # pyright: ignore[reportUnknownMemberType]
+        ]
+        normal = model.norms[
+            model.faces_norm.reshape((-1,))  # pyright: ignore[reportUnknownMemberType]
+        ]
+        uv = model.uvs[
+            model.faces_uv.reshape((-1,))  # pyright: ignore[reportUnknownMemberType]
+        ]
+
+        texture_index = model.texture_index[
+            model.faces_uv.reshape((-1,))  # pyright: ignore[reportUnknownMemberType]
+        ]
+        # double_sided = model.texture_index[model.faces_uv.reshape((-1,))]
 
         face_indices: Integer[Array, "_ 3"]
-        face_indices = jnp.arange(model.faces.size).reshape(model.faces.shape)
+        face_indices = jnp.arange(  # pyright: ignore[reportUnknownMemberType]
+            model.faces.size
+        ).reshape(model.faces.shape)
         assert isinstance(face_indices, Integer[Array, "_ 3"])
 
         light_dir: Vec3f = normalise(light.direction.copy())
         assert isinstance(light_dir, Vec3f), f"{light_dir}"
 
         light_dir_eye: Vec3f = Camera.apply_vec(
             light_dir.copy(),
@@ -242,15 +311,18 @@
             light=LightSource(
                 direction=light_dir,
                 colour=light.colour,
             ),
             light_dir_eye=light_dir_eye,
             texture_shape=model.texture_shape,
             texture_index=texture_index,
-            texture_offset=model.offset,
+            texture_offset=jnp.array(  # pyright: ignore[reportUnknownMemberType]
+                model.offset,
+                dtype=int,
+            ),
             texture=model.diffuse_map,
             specular_map=model.specular_map,
             ambient=light.ambient,
             diffuse=light.diffuse,
             specular=light.specular,
         )
 
@@ -265,32 +337,35 @@
                 loop_unroll=loop_unroll,
             )
             assert isinstance(buffers, Buffers), f"{buffers}"
 
             return buffers
         else:
             # with shadows
-            assert isinstance(shadow_param,
-                              ShadowParameters), f"{shadow_param}"
+            assert isinstance(shadow_param, ShadowParameters), f"{shadow_param}"
             # first pass: render shadow map
-            shadow: Shadow = Shadow.render_shadow_map(
-                shadow_map=lax.full_like(
-                    buffers.zbuffer,
-                    DtypeInfo.create(jax.dtypes.result_type(
-                        buffers.zbuffer)).max,
+            shadow = cast(
+                Shadow,
+                Shadow.render_shadow_map(
+                    shadow_map=lax.full_like(  # pyright: ignore[reportUnknownMemberType]
+                        buffers.zbuffer,
+                        DtypeInfo.create(
+                            jax.dtypes.result_type(buffers.zbuffer)  # pyright: ignore
+                        ).max,
+                    ),
+                    verts=model.verts,
+                    faces=model.faces,
+                    light_direction=light.direction,
+                    viewport_matrix=camera.viewport,
+                    centre=shadow_param.centre,
+                    up=shadow_param.up,
+                    strength=shadow_param.strength,
+                    offset=shadow_param.offset,
+                    loop_unroll=loop_unroll,
                 ),
-                verts=model.verts,
-                faces=model.faces,
-                light_direction=light.direction,
-                viewport_matrix=camera.viewport,
-                centre=shadow_param.centre,
-                up=shadow_param.up,
-                strength=shadow_param.strength,
-                offset=shadow_param.offset,
-                loop_unroll=loop_unroll,
             )
             assert isinstance(shadow, Shadow), f"{shadow}"
 
             _extra = PhongReflectionShadowTextureExtraInput(
                 **extra._asdict(),
                 shadow=shadow,
                 camera=camera,
@@ -308,28 +383,34 @@
             assert isinstance(buffers, Buffers), f"{buffers}"
 
             return buffers
 
     @classmethod
     @jaxtyped
     @partial(
-        jax.jit,
+        jit,
         static_argnames=("cls", "width", "height", "loop_unroll"),
         inline=True,
     )
     @add_tracing_name
     def get_camera_image(
         cls,
         objects: Sequence[ModelObject],
         light: LightParameters,
         camera: Union[Camera, CameraParameters],
         width: int,
         height: int,
-        colour_default: Colour = jnp.array((1., 1., 1.), dtype=jnp.single),
-        zbuffer_default: Num[Array, ""] = jnp.array(1, dtype=jnp.single),
+        colour_default: Colour = jnp.array(  # pyright: ignore[reportUnknownMemberType, reportCallInDefaultInitializer]
+            (1.0, 1.0, 1.0),
+            dtype=jnp.single,
+        ),
+        zbuffer_default: NumV = jnp.array(  # pyright: ignore[reportUnknownMemberType, reportCallInDefaultInitializer]
+            1,
+            dtype=jnp.single,
+        ),
         shadow_param: Optional[ShadowParameters] = None,
         loop_unroll: int = 1,
     ) -> Canvas:
         """Render the scene with the given camera.
 
         The dtype of `colour_default` and `zbuffer_default` will be used as the
         dtype of canvas and zbuffer.
@@ -352,41 +433,41 @@
             _camera = cls.create_camera_from_parameters(camera)
         else:
             _camera = camera
 
         assert isinstance(_camera, Camera), f"{_camera}"
 
         light = tree_map(
-            jnp.asarray,
+            jnp.asarray,  # pyright: ignore[reportUnknownMemberType, reportUnknownArgumentType]
             light,
             # only flatten one layer
             is_leaf=lambda x: not isinstance(x, LightParameters),
         )
         assert isinstance(light, LightParameters), f"{light}"
 
-        buffers: Buffers = cls.create_buffers(
+        buffers: Buffers[Tuple[Canvas]] = cls.create_buffers(
             width=width,
             height=height,
             colour_default=colour_default,
             zbuffer_default=zbuffer_default,
         )
 
         model: MergedModel = merge_objects(objects)
         assert isinstance(model, MergedModel), f"{model}"
 
         if shadow_param is not None:
             shadow_param = tree_map(
-                jnp.asarray,
+                jnp.asarray,  # pyright: ignore[reportUnknownMemberType, reportUnknownArgumentType]
                 shadow_param,
                 # only flatten one layer
                 is_leaf=lambda x: not isinstance(x, ShadowParameters),
             )
 
         canvas: Canvas
-        _, (canvas, ) = cls.render(
+        _, (canvas,) = cls.render(
             model=model,
             light=light,
             camera=_camera,
             buffers=buffers,
             shadow_param=shadow_param,
             loop_unroll=loop_unroll,
         )
```

### Comparing `jaxrenderer-0.3.1/renderer/scene.py` & `jaxrenderer-0.3.2/renderer/scene.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,97 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from typing import NamedTuple, NewType, Optional, Union
 
-import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Bool, Float, jaxtyped
+from jaxtyping import Array, Float
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
-from ._backport import replace_dict
+from ._backport import DictT, Tuple, replace_dict
 from .model import Model, ModelObject
 from .shapes.capsule import UpAxis, create_capsule
 from .shapes.cube import create_cube
-from .types import SpecularMap, Texture, Vec3f, Vec4f
+from .types import BoolV, SpecularMap, Texture, Vec3f, Vec4f
 
 GUID = NewType("GUID", int)
 
 
 class Scene(NamedTuple):
     """Scene with models and objects. Noticed that with each update to the
-        scene, the scene instance is replaced with a new one.
+    scene, the scene instance is replaced with a new one.
     """
+
     guid: GUID = GUID(0)
     """Max unique identifier among all objects in the scene. It equals to the
         numbers of models and objects ever created in the scene.
     """
-    models: dict[GUID, Model] = {}
+    models: DictT[GUID, Model] = {}
     """Models in the scene, indexed by their unique identifier."""
-    objects: dict[GUID, ModelObject] = {}
+    objects: DictT[GUID, ModelObject] = {}
     """Objects in the scene, indexed by their unique identifier."""
 
     @jaxtyped
-    def add_model(self, model: Model) -> tuple["Scene", GUID]:
+    def add_model(self, model: Model) -> Tuple["Scene", GUID]:
         """Add a model to the scene.
 
         Parameters:
           - model: a model to add to the scene.
 
         Returns:
           A tuple of the updated scene and the unique identifier of the model.
         """
         guid = self.guid
         new_scene = self._replace(
             guid=GUID(guid + 1),
-            models={
-                **self.models, guid: model
-            },
+            models={**self.models, guid: model},
         )
 
         return new_scene, guid
 
     @jaxtyped
     def add_cube(
         self,
-        half_extents: Union[Float[Array, "3"], tuple[float, float, float]],
+        half_extents: Union[Float[Array, "3"], Tuple[float, float, float]],
         diffuse_map: Texture,
-        texture_scaling: Union[Float[Array, "2"], tuple[float, float], float],
-    ) -> tuple["Scene", GUID]:
+        texture_scaling: Union[Float[Array, "2"], Tuple[float, float], float],
+    ) -> Tuple["Scene", GUID]:
         """Add a cube to the scene.
 
         Parameters:
           - half_extents: the half-size of the cube. The final cube would have
             x-y-z dimension of 2 * half_extents.
           - diffuse_map: the diffuse map of the cube.
           - texture_scaling: the scaling factor of the texture, in x and y. If
             only one number is given, it is used for both x and y.
         """
         # reference: https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/model.cpp#L215
-        specular_map: SpecularMap = lax.full(diffuse_map.shape[:2], 2.0)
+        specular_map: SpecularMap = (
+            lax.full(  # pyright: ignore[reportUnknownMemberType]
+                diffuse_map.shape[:2], 2.0
+            )
+        )
 
-        _half_extents = jnp.asarray(half_extents)
-        assert isinstance(_half_extents, Float[Array, "3"]), (
-            f"Expected 2 floats in half_extends, got {half_extents}")
+        _half_extents = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+            half_extents
+        )
+        assert isinstance(
+            _half_extents, Float[Array, "3"]
+        ), f"Expected 2 floats in half_extends, got {half_extents}"
 
-        _texture_scaling = jnp.asarray(texture_scaling)
+        _texture_scaling = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+            texture_scaling
+        )
         if _texture_scaling.size == 1:
-            _texture_scaling = lax.full((2, ), _texture_scaling)
-        assert isinstance(_texture_scaling, Float[Array, "2"]), (
-            f"Expected 2 floats in texture_scaling, got {texture_scaling}")
+            _texture_scaling = lax.full(  # pyright: ignore[reportUnknownMemberType]
+                (2,), _texture_scaling
+            )
+        assert isinstance(
+            _texture_scaling, Float[Array, "2"]
+        ), f"Expected 2 floats in texture_scaling, got {texture_scaling}"
 
         model: Model = create_cube(
             half_extents=_half_extents,
             texture_scaling=_texture_scaling,
             diffuse_map=diffuse_map,
             specular_map=specular_map,
         )
@@ -90,51 +101,56 @@
     @jaxtyped
     def add_capsule(
         self,
         radius: float,
         half_height: float,
         up_axis: UpAxis,
         diffuse_map: Texture,
-    ) -> tuple["Scene", GUID]:
+    ) -> Tuple["Scene", GUID]:
         """Add a capsule to the scene.
 
         Parameters:
           - radius: the radius of the capsule.
           - half_height: the half height of the capsule.
           - up_axis: the up axis of the capsule.
           - diffuse_map: the diffuse map of the capsule.
         """
         # reference: https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/model.cpp#L215
-        specular_map: SpecularMap = lax.full(diffuse_map.shape[:2], 2.0)
+        specular_map: SpecularMap = (
+            lax.full(  # pyright: ignore[reportUnknownMemberType]
+                diffuse_map.shape[:2],
+                2.0,
+            )
+        )
         model: Model = create_capsule(
-            radius=jnp.asarray(radius),
-            half_height=jnp.asarray(half_height),
+            radius=jnp.asarray(radius),  # pyright: ignore[reportUnknownMemberType]
+            half_height=jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+                half_height
+            ),
             up_axis=up_axis,
             diffuse_map=diffuse_map,
             specular_map=specular_map,
         )
 
         return self.add_model(model)
 
     @jaxtyped
-    def add_object_instance(self, model_id: GUID) -> tuple["Scene", GUID]:
+    def add_object_instance(self, model_id: GUID) -> Tuple["Scene", GUID]:
         """Add an object instance to the scene.
 
         Parameters:
           - model_id: the unique identifier of the model to add.
 
         Returns:
           A tuple of the updated scene and the unique identifier of the object.
         """
         guid = self.guid
         new_scene = self._replace(
             guid=GUID(guid + 1),
-            objects={
-                **self.objects, guid: ModelObject(model=self.models[model_id])
-            },
+            objects={**self.objects, guid: ModelObject(model=self.models[model_id])},
         )
 
         return new_scene, guid
 
     @jaxtyped
     def delete_model(self, model_id: GUID, check: bool) -> "Scene":
         """Delete a model from the scene.
@@ -150,16 +166,16 @@
             return self
 
         model = self.models[model_id]
         if check:
             for object_id, object in self.objects.items():
                 if object.model == model:
                     raise RuntimeError(
-                        f"model {model_id} is being used by object"
-                        f" {object_id}")
+                        f"model {model_id} is being used by object" f" {object_id}"
+                    )
 
         models = {k: v for k, v in self.models.items() if k != model_id}
         del model
 
         return self._replace(models=models)
 
     @jaxtyped
@@ -186,96 +202,108 @@
     def _replace_obj(self, object_id: GUID, new_obj: ModelObject) -> "Scene":
         """Replace an object in the scene.
 
         Parameters:
           - object_id: the unique identifier of the object to replace.
           - new_obj: the new object.
         """
-        return self._replace(objects=replace_dict(
-            self.objects,
-            {object_id: new_obj},
-        ))
+        return self._replace(
+            objects=replace_dict(
+                self.objects,
+                {object_id: new_obj},
+            )
+        )
 
     @jaxtyped
     def set_object_position(
         self,
         object_id: GUID,
-        position: Union[Vec3f, tuple[float, float, float]],
+        position: Union[Vec3f, Tuple[float, float, float]],
     ) -> "Scene":
         """Set the position of an object in the scene.
 
         Parameters:
           - object_id: the unique identifier of the object.
           - position: the new position of the object.
         """
-        position = jnp.asarray(position, dtype=float)
+        position = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+            position,
+            dtype=float,
+        )
         assert isinstance(position, Vec3f), f"{position}"
 
         new_obj = self.objects[object_id].replace_with_position(position)
 
         return self._replace_obj(object_id, new_obj)
 
     @jaxtyped
     def set_object_orientation(
         self,
         object_id: GUID,
-        orientation: Optional[Union[Vec4f, tuple[float, float, float,
-                                                 float]]] = None,
+        orientation: Optional[Union[Vec4f, Tuple[float, float, float, float]]] = None,
         rotation_matrix: Optional[Float[Array, "3 3"]] = None,
     ) -> "Scene":
         """Set the orientation of an object in the scene.
 
         If rotation_matrix is specified, it takes precedence over orientation.
         If none is specified, the object's orientation is set to identity.
 
         Parameters:
           - object_id: the unique identifier of the object.
           - orientation: the new orientation of the object, optional.
           - rotation_matrix: the new rotation matrix of the object, optional
         """
         if orientation is not None:
-            orientation = jnp.asarray(orientation)
+            orientation = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+                orientation
+            )
         if rotation_matrix is not None:
-            rotation_matrix = jnp.asarray(rotation_matrix)
+            rotation_matrix = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+                rotation_matrix
+            )
 
         new_obj = self.objects[object_id].replace_with_orientation(
             orientation=orientation,
             rotation_matrix=rotation_matrix,
         )
 
         return self._replace_obj(object_id, new_obj)
 
     @jaxtyped
     def set_object_local_scaling(
         self,
         object_id: GUID,
-        local_scaling: Union[Vec3f, tuple[float, float, float]],
+        local_scaling: Union[Vec3f, Tuple[float, float, float]],
     ) -> "Scene":
         """Set the local scaling of an object in the scene.
 
         Parameters:
           - object_id: the unique identifier of the object.
           - local_scaling: the new local scaling of the object.
         """
-        scaling = jnp.asarray(local_scaling, dtype=float)
+        scaling = jnp.asarray(  # pyright: ignore[reportUnknownMemberType]
+            local_scaling,
+            dtype=float,
+        )
         assert isinstance(scaling, Vec3f), f"{scaling}"
 
         new_obj = self.objects[object_id].replace_with_local_scaling(scaling)
 
         return self._replace_obj(object_id, new_obj)
 
     @jaxtyped
     def set_object_double_sided(
         self,
         object_id: GUID,
-        double_sided: Union[bool, Bool[Array, ""]],
+        double_sided: Union[bool, BoolV],
     ) -> "Scene":
         """Set whether an object in the scene is double-sided.
 
         Parameters:
           - object_id: the unique identifier of the object.
           - double_sided: whether the object is double-sided.
         """
         new_obj = self.objects[object_id].replace_with_double_sided(
-            jnp.asarray(double_sided))
+            jnp.asarray(double_sided)  # pyright: ignore[reportUnknownMemberType]
+        )
 
         return self._replace_obj(object_id, new_obj)
```

### Comparing `jaxrenderer-0.3.1/renderer/shader.py` & `jaxrenderer-0.3.2/renderer/shader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,71 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from abc import ABC, abstractmethod
 from functools import partial
-from typing import Generic, NamedTuple, TypeVar
+from typing import Generic, NamedTuple, TypeVar, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import Partial, tree_map
-from jaxtyping import Array, Bool, Float, Integer, PyTree, Shaped, jaxtyped
+from jaxtyping import Array, Bool, Float, Shaped
+from jaxtyping import PyTree  # pyright: ignore[reportUnknownVariableType]
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
-from ._backport import Tuple
+from ._backport import Tuple, TypeAlias
 from ._meta_utils import add_tracing_name
+from ._meta_utils import typed_jit as jit
 from .geometry import Camera, Interpolation, interpolate
-from .types import FALSE_ARRAY, INF_ARRAY, TRUE_ARRAY, Vec2f, Vec3f, Vec4f
+from .types import (
+    FALSE_ARRAY,
+    INF_ARRAY,
+    TRUE_ARRAY,
+    BoolV,
+    FloatV,
+    IntV,
+    Vec2f,
+    Vec3f,
+    Vec4f,
+)
 
-jax.config.update('jax_array', True)
+jax.config.update("jax_array", True)  # pyright: ignore[reportUnknownMemberType]
 
-ID = Integer[Array, ""]
+ID: TypeAlias = IntV
 
 ShaderExtraInputT = TypeVar(
-    'ShaderExtraInputT',
+    "ShaderExtraInputT",
     bound=PyTree[Shaped[Array, "..."]],
 )
 """Extra input for vertex shader & fragment shader, shared by all."""
 
 
 class PerVertex(NamedTuple):
     """Built-in output from Vertex Shader.
 
     gl_Position is in clip-space.
     """
+
     gl_Position: Vec4f
     # gl_PointSize is meaningful only when rendering point primitives.
     # not supported for now
-    # gl_PointSize: Float[Array, ""]
+    # gl_PointSize: FloatV
 
 
 class PerFragment(NamedTuple):
     """Built-in Output from Fragment Shader.
 
     If use_default_depth is True (default False), gl_FragCoord[2] will be used
     later by default.
     """
-    gl_FragDepth: Float[Array, ""] = INF_ARRAY
+
+    gl_FragDepth: FloatV = INF_ARRAY
     # not discard
-    keeps: Bool[Array, ""] = TRUE_ARRAY
-    use_default_depth: Bool[Array, ""] = FALSE_ARRAY
+    keeps: BoolV = TRUE_ARRAY
+    use_default_depth: BoolV = FALSE_ARRAY
 
 
 VaryingT = TypeVar(
     "VaryingT",
     bound=Tuple[Shaped[Array, "..."], ...],
 )
 """The user-defined input and second (extra) output of fragment shader."""
@@ -64,36 +79,37 @@
 
 class MixerOutput(NamedTuple):
     """Built-in output from `Shader.mix`.
 
     keep: bool, whether the output should be used to update buffers
     zbuffer: store depth value, and the result is used to set zbuffer.
     """
-    keep: Bool[Array, ""]
-    zbuffer: Float[Array, ""]
+
+    keep: BoolV
+    zbuffer: FloatV
 
 
 class Shader(ABC, Generic[ShaderExtraInputT, VaryingT, MixedExtraT]):
     """Base class for customised shader.
 
     Since JAX is pure functional (stateless), the state will be passed by
     returned values (the second return value in each function) in each process.
     """
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     @abstractmethod
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: ShaderExtraInputT,
-    ) -> tuple[PerVertex, VaryingT]:
+    ) -> Tuple[PerVertex, VaryingT]:
         """Override this to implement the vertex shader as defined by OpenGL.
 
         The meaning of the inputs follows the definitions in OpenGL. Additional
         named parameters can be defined and passed in if you need, as defined
         in `extra`.
 
         Noticed that no internal state will be tracked, thus if there is any
@@ -134,32 +150,32 @@
           - [Vertex Shader/Defined Inputs](https://www.khronos.org/opengl/wiki/Vertex_Shader/Defined_Inputs)
           - [Vertex Shader#Outputs](https://www.khronos.org/opengl/wiki/Vertex_Shader#Outputs)
         """
         raise NotImplementedError("vertex shader not implemented")
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def primitive_chooser(
         gl_FragCoord: Float[Array, "primitives 4"],
         gl_FrontFacing: Bool[Array, "primitives"],
         gl_PointCoord: Float[Array, "primitives 2"],
         keeps: Bool[Array, "primitives"],
         values: VaryingT,
         barycentric_screen: Float[Array, "primitives 3"],
         barycentric_clip: Float[Array, "primitives 3"],
-    ) -> tuple[  #
-            Float[Array, "kept_primitives 4"],  # gl_FragCoord
-            Bool[Array, "kept_primitives"],  # gl_FrontFacing
-            Float[Array, "kept_primitives 2"],  # gl_PointCoord
-            Bool[Array, "kept_primitives"],  # keeps
-            VaryingT,  # values
-            Float[Array, "kept_primitives 3"],  # barycentric_screen
-            Float[Array, "kept_primitives 3"],  # barycentric_clip
+    ) -> Tuple[  #
+        Float[Array, "kept_primitives 4"],  # gl_FragCoord
+        Bool[Array, "kept_primitives"],  # gl_FrontFacing
+        Float[Array, "kept_primitives 2"],  # gl_PointCoord
+        Bool[Array, "kept_primitives"],  # keeps
+        VaryingT,  # values
+        Float[Array, "kept_primitives 3"],  # barycentric_screen
+        Float[Array, "kept_primitives 3"],  # barycentric_clip
     ]:
         """Override this to customise the primitive choosing stage.
 
         The default implementation is to only keep the primitive with minimum
         `gl_FragCoord[2]` and `gl_FrontFacing` and `keeps` (interpolated `z`
         value in window space is minimum), i.e., the closest primitive that is
         kept and is not back-facing.
@@ -185,26 +201,30 @@
             point to interpolate
 
         Return:
           tuple of values from kept primitives, in same order and structure of
           the input parameters. The returned fields must be batched.
         """
         depths: Float[Array, "primitives"]
-        depths = jnp.where(keeps & gl_FrontFacing, gl_FragCoord[:, 2], jnp.inf)
+        depths = jnp.where(  # pyright: ignore[reportUnknownMemberType]
+            keeps & gl_FrontFacing,
+            gl_FragCoord[:, 2],
+            jnp.inf,
+        )
         assert isinstance(depths, Float[Array, "primitives"])
 
         # when all keeps are false, all depths will be inf, and there will
         # still be a valid idx generated, as promised by argmin.
-        idx: Integer[Array, ""] = jnp.argmin(depths)
-        assert isinstance(idx, Integer[Array, ""])
+        idx: IntV = jnp.argmin(depths)  # pyright: ignore[reportUnknownMemberType]
+        assert isinstance(idx, IntV)
 
         _get = partial(
             # use `dynamic_slice` instead of `slice` according to benchmark
             # https://colab.research.google.com/drive/1idBbgEDbxI6wi5kzlHF6kzWryoFSm8-p#scrollTo=-bHrz3kZ5A0p
-            lax.dynamic_slice_in_dim,
+            lax.dynamic_slice_in_dim,  # pyright: ignore[reportUnknownMemberType]
             start_index=idx,
             slice_size=1,
             axis=0,
         )
 
         _gl_FragCoord: Float[Array, "kept_primitives 4"] = _get(gl_FragCoord)
         assert isinstance(_gl_FragCoord, Float[Array, "kept_primitives 4"])
@@ -216,20 +236,27 @@
         assert isinstance(_keeps, Bool[Array, "kept_primitives"])
         _values: VaryingT = tree_map(_get, values)
         _screen: Float[Array, "kept_primitives 3"] = _get(barycentric_screen)
         assert isinstance(_screen, Float[Array, "kept_primitives 3"])
         _clip: Float[Array, "kept_primitives 3"] = _get(barycentric_clip)
         assert isinstance(_clip, Float[Array, "kept_primitives 3"])
 
-        return (_gl_FragCoord, _gl_FrontFacing, _gl_PointCoord, _keeps,
-                _values, _screen, _clip)
+        return (
+            _gl_FragCoord,
+            _gl_FrontFacing,
+            _gl_PointCoord,
+            _keeps,
+            _values,
+            _screen,
+            _clip,
+        )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def interpolate(
         values: VaryingT,
         barycentric_screen: Vec3f,
         barycentric_clip: Vec3f,
     ) -> VaryingT:
         """Override this to customise the interpolation of user-defined inputs.
@@ -260,23 +287,23 @@
             values,
         )
 
         return varying
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
-        gl_FrontFacing: Bool[Array, ""],
+        gl_FrontFacing: BoolV,
         gl_PointCoord: Vec2f,
         varying: VaryingT,
         extra: ShaderExtraInputT,
-    ) -> tuple[PerFragment, VaryingT]:
+    ) -> Tuple[PerFragment, VaryingT]:
         """Override this to implement the vertex shader as defined by OpenGL.
 
         This is optional. The default implementation writes nothing and thus
         `gl_FragDepth` further down the pipeline will use `gl_FragCoord[2]`.
         For the `varying` input, it will be returned directly untouched.
 
         If the output from this default implementation is re-used, noticed that
@@ -303,21 +330,21 @@
           - [Fragment Shader/Defined Inputs](https://www.khronos.org/opengl/wiki/Fragment_Shader/Defined_Inputs)
           - [Fragment Shader#Outputs](https://www.khronos.org/opengl/wiki/Fragment_Shader#Outputs)
         """
         return PerFragment(use_default_depth=TRUE_ARRAY), varying
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "kept_primitives"],
         keeps: Bool[Array, "kept_primitives"],
         extra: VaryingT,
-    ) -> tuple[MixerOutput, MixedExtraT]:
+    ) -> Tuple[MixerOutput, Union[VaryingT, MixedExtraT]]:
         """Override this to customise the mixing behaviour per fragment over
             different primitives (triangles).
 
         Use this to implement the `blending` behaviour if needed.
 
         For the default behaviour, the values from fragment with maximum
         `gl_FragDepth` value AND `keeps` being True will be used as the output.
@@ -331,30 +358,39 @@
               pixel in the buffers
             - zbuffer, the value used to update the zbuffer
           - User-defined outputs, must be a tuple (can be NamedTuple)
             Each field must be defined as same order as in the class `Buffers`.
             The values will be directly set to the `Buffers` **in the same
             order of the given definition** as if a usual `tuple`, but not
             based on field name.
+            This type must be `MixedExtraT` when override; `VaryingT` is used for the
+            default implementation here simply due to the limitation that we cannot
+            know how to create a MixedExtraT from a VaryingT at this time.
+            TODO: figure out a better way to define these generics.
 
         Reference:
           - [Blending](https://www.khronos.org/opengl/wiki/Blending)
         """
 
         depths: Float[Array, "primitives"]
-        depths = jnp.where(keeps, gl_FragDepth, jnp.inf)
+        depths = jnp.where(  # pyright: ignore[reportUnknownMemberType]
+            keeps,
+            gl_FragDepth,
+            jnp.inf,
+        )
         assert isinstance(depths, Float[Array, "primitives"])
 
         # when all keeps are false, all depths will be inf, and there will
         # still be a valid idx generated, as promised by argmin.
-        idx: Integer[Array, ""] = jnp.argmin(depths)
-        assert isinstance(idx, Integer[Array, ""])
-
-        keep: Bool[Array, ""] = keeps[idx]
-        assert isinstance(keep, Bool[Array, ""])
-        depth: Float[Array, ""] = depths[idx]
-        assert isinstance(depth, Float[Array, ""])
+        idx: IntV
+        idx = jnp.argmin(depths)  # pyright: ignore[reportUnknownMemberType]
+        assert isinstance(idx, IntV)
+
+        keep: BoolV = keeps[idx]
+        assert isinstance(keep, BoolV)
+        depth: FloatV = depths[idx]
+        assert isinstance(depth, FloatV)
 
         return (
             MixerOutput(keep=keep, zbuffer=depth),
             tree_map(lambda x: x[idx], extra),
         )
```

### Comparing `jaxrenderer-0.3.1/renderer/shaders/README.md` & `jaxrenderer-0.3.2/renderer/shaders/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
 
 Noticed that the light direction is not transformed and thus the light direction is used as if it is in the eye-space. This shows a "headlight" effect.
 
 ## Phong Shading with Phong Reflection Approximation `phong_reflection.py`
 
 This is a simple implementation of Phong shading with Phong reflection approximation, which interpolates the vertex normal and then computes the light direction in the Fragment Shader. Textures are sampled in clip space in the Fragment Shader.
 
-Phong's Approximation is used to support `specular`, `ambient` and `diffuse` lighting. The spcular lighting is computed with shininess factor given in a `SpecularMap`.
+Phong's Approximation is used to support `specular`, `ambient` and `diffuse` lighting. The specular lighting is computed with shininess factor given in a `SpecularMap`.
 
 The light direction needs to be given in the pre-projection view/eye space via `light_dir_eye`. The normals are transformed into eye space as well for light computation.
 
 ## Phong Shading with Shadow and Phong Reflection Approximation `phong_reflection_shadow.py`
 
 This is a simple implementation of Phong shading with Phong reflection approximation and shadow, which interpolates the vertex normal and then computes the light direction in the Fragment Shader. Textures are sampled in clip space in the Fragment Shader.
 
-Phong's Approximation is used to support `specular`, `ambient` and `diffuse` lighting. The spcular lighting is computed with shininess factor given in a `SpecularMap`.
+Phong's Approximation is used to support `specular`, `ambient` and `diffuse` lighting. The specular lighting is computed with shininess factor given in a `SpecularMap`.
 
 The light direction needs to be given in the pre-projection view/eye space via `light_dir_eye`. The normals are transformed into eye space as well for light computation.
 
-Shadows are simply tested in fragment shadow against a shadow map given by `Shadow`. Shadow coordinates is computed by first transform world coordinates of the vertices in the vertex shader into the clip space of the light, interpolated in clip space (`SMOOTH` by default) in the `Shader.interpolate`, then  projected into screen coordinates in the fragment shader, and finally compared against the shadow map. It is safe to interpolate in the light's clip space using barycentric coordinates obtained in the model/main camera's clip space, because there is a simple linear transformation (by a invertible matrix) between the two pre-projection clip spaces. CHECK: Thus after projection, the barycentric coordinates computed are the same. Reference of this method is here [Tutorial 16 : Shadow mapping/opengl-tutorial](http://www.opengl-tutorial.org/intermediate-tutorials/tutorial-16-shadow-mapping/#basic-shader).
+Shadows are simply tested in fragment shadow against a shadow map given by `Shadow`. Shadow coordinates is computed by first transform world coordinates of the vertices in the vertex shader into the clip space of the light, interpolated in clip space (`SMOOTH` by default) in the `Shader.interpolate`, then  projected into screen coordinates in the fragment shader, and finally compared against the shadow map. It is safe to interpolate in the light's clip space using barycentric coordinates obtained in the model/main camera's clip space, because there is a simple linear transformation (by a invertible matrix) between the two pre-projection clip spaces. CHECK: Thus after projection, the barycentric coordinates computed are the same. Reference of this method is here [Tutorial 16 : Shadow mapping/OpenGL-tutorial](http://www.opengl-tutorial.org/intermediate-tutorials/tutorial-16-shadow-mapping/#basic-shader).
 
 A common method of computing shadow to transform fragment coordinates first back to world space, then transform to light's screen space. This method does not work due to the precision lost. Even with handcrafted inverse matrices, the precision is still not enough. Using `jax.lax.linalg.triangular_solve` does not help either. This issue is not only about the depth (z-component), but also about the x- and y-components, leading to a failure of retrieving the shadow value in the shadow map.
```

### Comparing `jaxrenderer-0.3.1/renderer/shaders/gouraud.py` & `jaxrenderer-0.3.2/renderer/shaders/gouraud.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,124 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import NamedTuple
+from typing import NamedTuple, cast
 
 import jax
 import jax.numpy as jnp
-from jaxtyping import Array, Bool, Float, jaxtyped
+from jaxtyping import Array, Float
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
+from .._backport import Tuple
 from .._meta_utils import add_tracing_name
-from ..shader import ID, PerFragment, PerVertex, Shader
+from .._meta_utils import typed_jit as jit
 from ..geometry import Camera, normalise, to_homogeneous
-from ..types import Colour, LightSource, Vec2f, Vec3f, Vec4f
+from ..shader import ID, PerFragment, PerVertex, Shader
+from ..types import BoolV, Colour, FloatV, LightSource, Vec2f, Vec3f, Vec4f
 
-jax.config.update('jax_array', True)
+jax.config.update("jax_array", True)  # pyright: ignore[reportUnknownMemberType]
 
 
 class GouraudExtraInput(NamedTuple):
     """Extra input for Gouraud Shader.
 
     Attributes:
       - position: in world space, of each vertex.
       - colour: of each vertex
       - normal: in world space, of each vertex.
       - light: parallel light source, shared by all vertices.
     """
+
     position: Float[Array, "vertices 3"]  # in world space
     colour: Float[Array, "vertices 3"]
     normal: Float[Array, "vertices 3"]  # in world space
     light: LightSource
 
 
 class GouraudExtraFragmentData(NamedTuple):
-    colour: Colour = jnp.array([0.0, 0.0, 0.0])
+    colour: Colour = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        [0.0, 0.0, 0.0]
+    )
 
 
 class GouraudExtraMixerOutput(NamedTuple):
     """When render to only one target, for simplicity."""
+
     canvas: Colour
 
 
-class GouraudShader(Shader[GouraudExtraInput, GouraudExtraFragmentData,
-                           GouraudExtraMixerOutput]):
+class GouraudShader(
+    Shader[GouraudExtraInput, GouraudExtraFragmentData, GouraudExtraMixerOutput]
+):
     """Gouraud Shading with simple parallel lighting."""
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: GouraudExtraInput,
-    ) -> tuple[PerVertex, GouraudExtraFragmentData]:
+    ) -> Tuple[PerVertex, GouraudExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
         position: Vec4f = to_homogeneous(extra.position[gl_VertexID])
         gl_Position: Vec4f = camera.to_clip(position)
         assert isinstance(gl_Position, Vec4f)
 
         # assume normal here is in world space. If it is in model space, it
         # must be transformed by the inverse transpose of the model matrix.
         # Ref: https://github.com/ssloy/tinyrenderer/wiki/Lesson-5:-Moving-the-camera#transformation-of-normal-vectors
         normal: Vec3f = normalise(extra.normal[gl_VertexID])
-        intensity: Float[Array, ""] = jnp.dot(
-            normal,
-            normalise(extra.light.direction),
+        intensity = cast(
+            FloatV,
+            jnp.dot(
+                normal,
+                normalise(extra.light.direction),
+            ),
         )
-        assert isinstance(intensity, Float[Array, ""])
+        assert isinstance(intensity, FloatV)
 
         colour: Colour
         colour = extra.colour[gl_VertexID] * extra.light.colour * intensity
 
         return (
             PerVertex(gl_Position=gl_Position),
             GouraudExtraFragmentData(colour=colour),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
-        gl_FrontFacing: Bool[Array, ""],
+        gl_FrontFacing: BoolV,
         gl_PointCoord: Vec2f,
         varying: GouraudExtraFragmentData,
         extra: GouraudExtraInput,
-    ) -> tuple[PerFragment, GouraudExtraFragmentData]:
+    ) -> Tuple[PerFragment, GouraudExtraFragmentData]:
         built_in: PerFragment = Shader.fragment(
             gl_FragCoord,
             gl_FrontFacing,
             gl_PointCoord,
             varying,
             extra,
         )[0]
         assert isinstance(built_in, PerFragment)
 
         return (
             PerFragment(
-                keeps=jnp.array((
-                    built_in.keeps,
-                    gl_FrontFacing,
-                    (varying.colour >= 0).all(),
-                )).all(),
+                keeps=jnp.array(  # pyright: ignore[reportUnknownMemberType]
+                    (
+                        built_in.keeps,
+                        gl_FrontFacing,
+                        jnp.all(  # pyright: ignore[reportUnknownMemberType]
+                            varying.colour >= 0
+                        ),
+                    )
+                ).all(),
                 use_default_depth=built_in.use_default_depth,
             ),
             varying,
         )
```

### Comparing `jaxrenderer-0.3.1/renderer/shaders/gouraud_texture.py` & `jaxrenderer-0.3.2/renderer/shaders/gouraud_texture.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,167 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import NamedTuple
+from typing import NamedTuple, cast
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Bool, Float, jaxtyped
+from jaxtyping import Array, Bool, Float
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
+from .._backport import Tuple
 from .._meta_utils import add_tracing_name
+from .._meta_utils import typed_jit as jit
 from ..geometry import Camera, normalise, to_homogeneous
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
-from ..types import Colour, LightSource, Texture, Vec2f, Vec3f, Vec4f
+from ..types import BoolV, Colour, FloatV, LightSource, Texture, Vec2f, Vec3f, Vec4f
 
-jax.config.update('jax_array', True)
+jax.config.update("jax_array", True)  # pyright: ignore[reportUnknownMemberType]
 
 
 class GouraudTextureExtraInput(NamedTuple):
     """Extra input for Gouraud Shader.
 
     Attributes:
       - position: in world space, of each vertex.
       - normal: in world space, of each vertex.
       - uv: in texture space, of each vertex.
       - light: parallel light source, shared by all vertices.
       - texture: texture, shared by all vertices.
     """
+
     position: Float[Array, "vertices 3"]  # in world space
     normal: Float[Array, "vertices 3"]  # in world space
     uv: Float[Array, "vertices 2"]  # in texture space
     light: LightSource
     texture: Texture
 
 
 class GouraudTextureExtraFragmentData(NamedTuple):
-    colour: Colour = jnp.array([0.0, 0.0, 0.0])
+    colour: Colour = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        [0.0, 0.0, 0.0]
+    )
     """light colour when passing from vertex shader to fragment shader;
     canvas colour when passing from fragment shader to mixer."""
-    uv: Vec2f = jnp.zeros(2)
+    uv: Vec2f = jnp.zeros(2)  # pyright: ignore[reportUnknownMemberType]
 
 
 class GouraudTextureExtraMixerOutput(NamedTuple):
     """When render to only one target, for simplicity."""
+
     canvas: Colour
 
 
-class GouraudTextureShader(Shader[GouraudTextureExtraInput,
-                                  GouraudTextureExtraFragmentData,
-                                  GouraudTextureExtraMixerOutput]):
+class GouraudTextureShader(
+    Shader[
+        GouraudTextureExtraInput,
+        GouraudTextureExtraFragmentData,
+        GouraudTextureExtraMixerOutput,
+    ]
+):
     """Gouraud Shading with simple parallel lighting and texture."""
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: GouraudTextureExtraInput,
-    ) -> tuple[PerVertex, GouraudTextureExtraFragmentData]:
+    ) -> Tuple[PerVertex, GouraudTextureExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
         position: Vec4f = to_homogeneous(extra.position[gl_VertexID])
         gl_Position: Vec4f = camera.to_clip(position)
         assert isinstance(gl_Position, Vec4f)
 
         # assume normal here is in world space. If it is in model space, it
         # must be transformed by the inverse transpose of the model matrix.
         # Ref: https://github.com/ssloy/tinyrenderer/wiki/Lesson-5:-Moving-the-camera#transformation-of-normal-vectors
         normal: Vec3f = normalise(extra.normal[gl_VertexID])
-        intensity: Float[Array, ""] = jnp.dot(
-            normal,
-            normalise(extra.light.direction),
+        intensity: FloatV = cast(
+            FloatV,
+            jnp.dot(
+                normal,
+                normalise(extra.light.direction),
+            ),
         )
-        assert isinstance(intensity, Float[Array, ""])
+        assert isinstance(intensity, FloatV)
 
         light_colour: Colour
         light_colour = extra.light.colour * intensity
 
         return (
             PerVertex(gl_Position=gl_Position),
             GouraudTextureExtraFragmentData(
                 colour=light_colour,
                 uv=extra.uv[gl_VertexID],
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
-        gl_FrontFacing: Bool[Array, ""],
+        gl_FrontFacing: BoolV,
         gl_PointCoord: Vec2f,
         varying: GouraudTextureExtraFragmentData,
         extra: GouraudTextureExtraInput,
-    ) -> tuple[PerFragment, GouraudTextureExtraFragmentData]:
+    ) -> Tuple[PerFragment, GouraudTextureExtraFragmentData]:
         built_in: PerFragment = Shader.fragment(
             gl_FragCoord,
             gl_FrontFacing,
             gl_PointCoord,
             varying,
             extra,
         )[0]
         assert isinstance(built_in, PerFragment)
 
         # repeat texture
-        uv = (lax.floor(varying.uv).astype(int) %
-              jnp.asarray(extra.texture.shape[:2]))
+        uv = lax.floor(varying.uv).astype(int)  # pyright: ignore
+        uv = uv % jnp.asarray(extra.texture.shape[:2])  # pyright: ignore
         texture_colour: Colour = extra.texture[uv[0], uv[1]]
         light_colour: Colour = varying.colour
 
         return (
             PerFragment(
-                keeps=jnp.array((
-                    built_in.keeps,
-                    gl_FrontFacing,
-                    (light_colour >= 0).all(),
-                )).all(),
+                keeps=jnp.array(  # pyright: ignore[reportUnknownMemberType]
+                    (
+                        built_in.keeps,
+                        gl_FrontFacing,
+                        (light_colour >= 0).all(),  # pyright: ignore
+                    )
+                ).all(),
                 use_default_depth=built_in.use_default_depth,
             ),
             GouraudTextureExtraFragmentData(
                 colour=texture_colour * light_colour,
                 uv=varying.uv,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: GouraudTextureExtraFragmentData,
-    ) -> tuple[MixerOutput, GouraudTextureExtraMixerOutput]:
+    ) -> Tuple[MixerOutput, GouraudTextureExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: GouraudTextureExtraFragmentData
-        mixer_output, extra_output = Shader.mix(gl_FragDepth, keeps, extra)
+        mixer_output, extra_output = cast(
+            Tuple[MixerOutput, GouraudTextureExtraFragmentData],
+            Shader.mix(gl_FragDepth, keeps, extra),
+        )
         assert isinstance(mixer_output, MixerOutput)
         assert isinstance(extra_output, GouraudTextureExtraFragmentData)
 
         return (
             mixer_output,
             GouraudTextureExtraMixerOutput(canvas=extra_output.colour),
         )
```

### Comparing `jaxrenderer-0.3.1/renderer/shaders/phong.py` & `jaxrenderer-0.3.2/renderer/shaders/phong.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import NamedTuple
+from typing import NamedTuple, cast
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Bool, Float, jaxtyped
+from jaxtyping import Array, Bool, Float
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
+from .._backport import Tuple
 from .._meta_utils import add_tracing_name
+from .._meta_utils import typed_jit as jit
 from ..geometry import Camera, normalise, to_homogeneous
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
-from ..types import Colour, LightSource, Texture, Vec2f, Vec3f, Vec4f
+from ..types import BoolV, Colour, LightSource, Texture, Vec2f, Vec3f, Vec4f
 
-jax.config.update('jax_array', True)
+jax.config.update("jax_array", True)  # pyright: ignore[reportUnknownMemberType]
 
 
 class PhongTextureExtraInput(NamedTuple):
     """Extra input for Phong Shader.
 
     Attributes:
       - position: in world space, of each vertex.
       - normal: in world space, of each vertex.
       - uv: in texture space, of each vertex.
       - light: parallel `headlight` light source, shared by all vertices.
         It is in the eye/view space.
       - texture: texture, shared by all vertices.
     """
+
     position: Float[Array, "vertices 3"]  # in world space
     normal: Float[Array, "vertices 3"]  # in world space
     uv: Float[Array, "vertices 2"]  # in texture space
     light: LightSource
     texture: Texture
 
 
@@ -38,39 +42,49 @@
     """From vertex shader to fragment shader, and from fragment shader to mixer.
 
     Attributes:
       - normal: in clip space, of each fragment; From VS to FS.
       - uv: in texture space, of each fragment; From VS to FS.
       - colour: colour when passing from FS to mixer.
     """
-    normal: Vec3f = jnp.array([0.0, 0.0, 0.0])
-    uv: Vec2f = jnp.zeros(2)
-    colour: Colour = jnp.array([0.0, 0.0, 0.0])
+
+    normal: Vec3f = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        [0.0, 0.0, 0.0]
+    )
+    uv: Vec2f = jnp.zeros(2)  # pyright: ignore[reportUnknownMemberType]
+    colour: Colour = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        [0.0, 0.0, 0.0]
+    )
 
 
 class PhongTextureExtraMixerOutput(NamedTuple):
     """When render to only one target, for simplicity."""
+
     canvas: Colour
 
 
-class PhongTextureShader(Shader[PhongTextureExtraInput,
-                                PhongTextureExtraFragmentData,
-                                PhongTextureExtraMixerOutput]):
+class PhongTextureShader(
+    Shader[
+        PhongTextureExtraInput,
+        PhongTextureExtraFragmentData,
+        PhongTextureExtraMixerOutput,
+    ]
+):
     """Phong Shading with simple parallel lighting and texture."""
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: PhongTextureExtraInput,
-    ) -> tuple[PerVertex, PhongTextureExtraFragmentData]:
+    ) -> Tuple[PerVertex, PhongTextureExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
         position: Vec4f = to_homogeneous(extra.position[gl_VertexID])
         gl_Position: Vec4f = camera.to_clip(position)
         assert isinstance(gl_Position, Vec4f)
 
         # assume normal here is in world space. If it is in model space, it
         # must be transformed by the inverse transpose of the model matrix.
@@ -87,71 +101,87 @@
                 normal=normal,
                 uv=extra.uv[gl_VertexID],
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
-        gl_FrontFacing: Bool[Array, ""],
+        gl_FrontFacing: BoolV,
         gl_PointCoord: Vec2f,
         varying: PhongTextureExtraFragmentData,
         extra: PhongTextureExtraInput,
-    ) -> tuple[PerFragment, PhongTextureExtraFragmentData]:
+    ) -> Tuple[PerFragment, PhongTextureExtraFragmentData]:
         built_in: PerFragment = Shader.fragment(
             gl_FragCoord,
             gl_FrontFacing,
             gl_PointCoord,
             varying,
             extra,
         )[0]
         assert isinstance(built_in, PerFragment)
 
         # repeat texture
-        uv = (lax.floor(varying.uv).astype(int) %
-              jnp.asarray(extra.texture.shape[:2]))
+        uv = lax.floor(varying.uv).astype(int)  # pyright: ignore
+        uv = uv % jnp.asarray(extra.texture.shape[:2])  # pyright: ignore
         texture_colour: Colour = extra.texture[uv[0], uv[1]]
 
         # light colour * intensity
-        light_colour: Colour = extra.light.colour * lax.dot(
-            normalise(varying.normal),
-            normalise(extra.light.direction),
+        light_colour: Colour = (
+            extra.light.colour
+            * lax.dot(  # pyright: ignore[reportUnknownMemberType]
+                normalise(varying.normal),
+                normalise(extra.light.direction),
+            )
         )
 
         return (
             PerFragment(
-                keeps=jnp.logical_and(built_in.keeps, gl_FrontFacing),
+                keeps=jnp.logical_and(  # pyright: ignore[reportUnknownMemberType]
+                    built_in.keeps,
+                    gl_FrontFacing,
+                ),
                 use_default_depth=built_in.use_default_depth,
             ),
             PhongTextureExtraFragmentData(
-                colour=lax.cond(
-                    (light_colour >= 0).all(),
-                    lambda: texture_colour * light_colour,
-                    lambda: jnp.zeros(3),
+                colour=cast(
+                    Vec3f,
+                    lax.cond(  # pyright: ignore[reportUnknownMemberType]
+                        jnp.all(  # pyright: ignore[reportUnknownMemberType]
+                            light_colour >= 0
+                        ),
+                        lambda: texture_colour * light_colour,
+                        lambda: jnp.zeros(  # pyright: ignore[reportUnknownMemberType]
+                            3
+                        ),
+                    ),
                 ),
                 uv=varying.uv,
                 normal=varying.normal,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: PhongTextureExtraFragmentData,
-    ) -> tuple[MixerOutput, PhongTextureExtraMixerOutput]:
+    ) -> Tuple[MixerOutput, PhongTextureExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: PhongTextureExtraFragmentData
-        mixer_output, extra_output = Shader.mix(gl_FragDepth, keeps, extra)
+        mixer_output, extra_output = cast(
+            Tuple[MixerOutput, PhongTextureExtraFragmentData],
+            Shader.mix(gl_FragDepth, keeps, extra),
+        )
         assert isinstance(mixer_output, MixerOutput)
         assert isinstance(extra_output, PhongTextureExtraFragmentData)
 
         return (
             mixer_output,
             PhongTextureExtraMixerOutput(canvas=extra_output.colour),
         )
```

### Comparing `jaxrenderer-0.3.1/renderer/shaders/phong_darboux.py` & `jaxrenderer-0.3.2/renderer/shaders/phong_darboux.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,48 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import NamedTuple
+from typing import NamedTuple, cast
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import Partial
-from jaxtyping import Array, Bool, Float, Integer, jaxtyped
+from jaxtyping import Array, Bool, Float, Integer
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
+from .._backport import Tuple, TypeAlias
 from .._meta_utils import add_tracing_name
-from ..geometry import (Camera, Interpolation, interpolate, normalise,
-                        to_cartesian, to_homogeneous)
+from .._meta_utils import typed_jit as jit
+from ..geometry import (
+    Camera,
+    Interpolation,
+    interpolate,
+    normalise,
+    to_cartesian,
+    to_homogeneous,
+)
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
-from ..types import (Colour, FaceIndices, LightSource, NormalMap, Texture,
-                     Triangle, Vec2f, Vec2i, Vec3f, Vec4f)
+from ..types import (
+    BoolV,
+    Colour,
+    FaceIndices,
+    LightSource,
+    NormalMap,
+    Texture,
+    Triangle,
+    Vec2f,
+    Vec3f,
+    Vec4f,
+)
 
-jax.config.update('jax_array', True)
+jax.config.update("jax_array", True)  # pyright: ignore[reportUnknownMemberType]
 
-Triangle3f = Float[Array, "3 3"]
-Triangle2f = Float[Array, "3 2"]
+Triangle3f: TypeAlias = Float[Array, "3 3"]
+Triangle2f: TypeAlias = Float[Array, "3 2"]
 
 
 class PhongTextureDarbouxExtraInput(NamedTuple):
     """Extra input for Phong Shader.
 
     Attributes:
       - position: in world space, of each vertex.
@@ -33,14 +52,15 @@
         It is in the eye/view space.
       - texture: texture, shared by all vertices.
       - normal_map: normal map, shared by all vertices.
         This is in Darboux frame.
       - id_to_face: id of the face that each vertex belongs to.
       - faces_indices: id of the vertex that each face contains.
     """
+
     position: Float[Array, "vertices 3"]  # in world space
     normal: Float[Array, "vertices 3"]  # in world space
     uv: Float[Array, "vertices 2"]  # in texture space
     light: LightSource
     texture: Texture
     normal_map: NormalMap
     """In Darboux frame."""
@@ -58,58 +78,72 @@
       - uv: in texture space, of each fragment; From VS to FS.
       - triangle: in normalised device coordinates (NDC), of each fragment;
         From VS to FS. This should not be interpolated.
       - triangle: in texture space, of each fragment; From VS to FS.
         This should not be interpolated.
       - colour: colour when passing from FS to mixer.
     """
-    normal: Vec3f = jnp.array([0.0, 0.0, 0.0])
-    uv: Vec2f = jnp.zeros(2)
-    triangle: Triangle3f = jnp.zeros((3, 3))
-    triangle_uv: Triangle2f = jnp.zeros((3, 2))
+
+    normal: Vec3f = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        [0.0, 0.0, 0.0]
+    )
+    uv: Vec2f = jnp.zeros(2)  # pyright: ignore[reportUnknownMemberType]
+    triangle: Triangle3f = jnp.zeros((3, 3))  # pyright: ignore[reportUnknownMemberType]
+    triangle_uv: Triangle2f = jnp.zeros(  # pyright: ignore[reportUnknownMemberType]
+        (3, 2)
+    )
     """triangle in NDC, not interpolated."""
-    colour: Colour = jnp.array([0.0, 0.0, 0.0])
+    colour: Colour = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        [0.0, 0.0, 0.0]
+    )
 
 
 class PhongTextureDarbouxExtraMixerOutput(NamedTuple):
     """When render to only one target, for simplicity."""
+
     canvas: Colour
 
 
-class PhongTextureDarbouxShader(Shader[PhongTextureDarbouxExtraInput,
-                                       PhongTextureDarbouxExtraFragmentData,
-                                       PhongTextureDarbouxExtraMixerOutput]):
+class PhongTextureDarbouxShader(
+    Shader[
+        PhongTextureDarbouxExtraInput,
+        PhongTextureDarbouxExtraFragmentData,
+        PhongTextureDarbouxExtraMixerOutput,
+    ]
+):
     """Phong Shading with simple parallel lighting and texture, normals are
-        represented in tangent space (Darboux frame)."""
+    represented in tangent space (Darboux frame)."""
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: PhongTextureDarbouxExtraInput,
-    ) -> tuple[PerVertex, PhongTextureDarbouxExtraFragmentData]:
+    ) -> Tuple[PerVertex, PhongTextureDarbouxExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
         assert isinstance(gl_VertexID, ID), gl_VertexID
         assert isinstance(gl_InstanceID, ID), gl_InstanceID
         position: Vec4f = to_homogeneous(extra.position[gl_VertexID])
         gl_Position: Vec4f = camera.to_clip(position)
         assert isinstance(gl_Position, Vec4f)
 
         assert isinstance(extra.id_to_face, Integer[Array, "vertices"]), (
             f"Expected Integer array with shape {extra.position.shape[:1]}, "
             f"got {type(extra.id_to_face)} with shape "
-            f"{extra.id_to_face.shape}")
+            f"{extra.id_to_face.shape}"
+        )
         assert isinstance(extra.faces_indices, Integer[Array, "faces 3"]), (
             f"Expected Integer array with shape (faces, 3), "
             f"got {type(extra.faces_indices)} with shape "
-            f"{extra.faces_indices.shape}")
+            f"{extra.faces_indices.shape}"
+        )
 
         face_indices = extra.faces_indices[extra.id_to_face[gl_VertexID]]
         triangle_model: Triangle = to_homogeneous(extra.position[face_indices])
         triangle_clip: Triangle = camera.to_clip(triangle_model)
         triangle_ndc: Triangle3f = to_cartesian(triangle_clip)
         assert isinstance(triangle_ndc, Triangle3f)
 
@@ -133,32 +167,32 @@
                 triangle=triangle_ndc,
                 triangle_uv=triangle_uv,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def interpolate(
         values: PhongTextureDarbouxExtraFragmentData,
         barycentric_screen: Vec3f,
         barycentric_clip: Vec3f,
     ) -> PhongTextureDarbouxExtraFragmentData:
         smooth_interpolation = Partial(
             interpolate,
             barycentric_screen=barycentric_screen,
             barycentric_clip=barycentric_clip,
             mode=Interpolation.SMOOTH,
         )
 
-        normal: Vec3f = smooth_interpolation(values.normal)
+        normal = cast(Vec3f, smooth_interpolation(values.normal))
         assert isinstance(normal, Vec3f)
 
-        uv: Vec2f = smooth_interpolation(values.uv)
+        uv = cast(Vec2f, smooth_interpolation(values.uv))
         assert isinstance(uv, Vec2f)
 
         varying: PhongTextureDarbouxExtraFragmentData = PhongTextureDarbouxExtraFragmentData(
             normal=normal,
             uv=uv,
             # pick first of the 3, as they are the same
             # noticed that `values` are batches, so here values.triangle is
@@ -169,94 +203,114 @@
         assert isinstance(varying.triangle, Triangle3f)
         assert isinstance(varying.triangle_uv, Triangle2f)
 
         return varying
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
-        gl_FrontFacing: Bool[Array, ""],
+        gl_FrontFacing: BoolV,
         gl_PointCoord: Vec2f,
         varying: PhongTextureDarbouxExtraFragmentData,
         extra: PhongTextureDarbouxExtraInput,
-    ) -> tuple[PerFragment, PhongTextureDarbouxExtraFragmentData]:
+    ) -> Tuple[PerFragment, PhongTextureDarbouxExtraFragmentData]:
         built_in: PerFragment = Shader.fragment(
             gl_FragCoord,
             gl_FrontFacing,
             gl_PointCoord,
             varying,
             extra,
         )[0]
         assert isinstance(built_in, PerFragment)
-        assert isinstance(varying, PhongTextureDarbouxExtraFragmentData), (
-            f"Expected PhongTextureDarbouxExtraFragmentData, got {varying}")
+        assert isinstance(
+            varying, PhongTextureDarbouxExtraFragmentData
+        ), f"Expected PhongTextureDarbouxExtraFragmentData, got {varying}"
 
         # repeat texture
-        uv = (lax.floor(varying.uv).astype(int) %
-              jnp.asarray(extra.texture.shape[:2]))
+        uv = lax.floor(varying.uv).astype(int)  # pyright: ignore
+        uv = uv % jnp.asarray(extra.texture.shape[:2])  # pyright: ignore
 
         normal: Vec3f = normalise(varying.normal)
-        A: Float[Array, "3 3"] = jnp.vstack([
-            varying.triangle[1, :] - varying.triangle[0, :],
-            varying.triangle[2, :] - varying.triangle[0, :],
-            normal,
-        ])
-        AI: Float[Array, "3 3"] = jnp.linalg.inv(A)
+        A: Float[Array, "3 3"] = jnp.vstack(  # pyright: ignore[reportUnknownMemberType]
+            [
+                varying.triangle[1, :] - varying.triangle[0, :],
+                varying.triangle[2, :] - varying.triangle[0, :],
+                normal,
+            ]
+        )
+        AI = cast(Float[Array, "3 3"], jnp.linalg.inv(A))
         _uv: Triangle2f = varying.triangle_uv
-        i: Vec3f = AI @ jnp.array(
-            [_uv[1, 0] - _uv[0, 0], _uv[2, 0] - _uv[0, 0], 0])
-        j: Vec3f = AI @ jnp.array(
-            [_uv[1, 1] - _uv[0, 1], _uv[2, 1] - _uv[0, 1], 0])
+        i: Vec3f = AI @ jnp.array(  # pyright: ignore[reportUnknownMemberType]
+            [_uv[1, 0] - _uv[0, 0], _uv[2, 0] - _uv[0, 0], 0]
+        )
+        j: Vec3f = AI @ jnp.array(  # pyright: ignore[reportUnknownMemberType]
+            [_uv[1, 1] - _uv[0, 1], _uv[2, 1] - _uv[0, 1], 0]
+        )
 
-        B: Float[Array, "3 3"] = lax.concatenate(
+        B = lax.concatenate(  # pyright: ignore[reportUnknownMemberType]
             [
                 normalise(i)[:, None],
                 normalise(j)[:, None],
                 normal[:, None],
             ],
             dimension=1,
         )
+        assert isinstance(B, Float[Array, "3 3"])
+
         normal = normalise(B @ extra.normal_map[uv[0], uv[1]])
         assert isinstance(normal, Vec3f)
 
         texture_colour: Colour = extra.texture[uv[0], uv[1]]
 
         # light colour * intensity
-        light_colour: Colour = extra.light.colour * lax.dot(
-            normal,
-            normalise(extra.light.direction),
+        light_colour: Colour = (
+            extra.light.colour
+            * lax.dot(  # pyright: ignore[reportUnknownMemberType]
+                normal,
+                normalise(extra.light.direction),
+            )
         )
 
         return (
             PerFragment(
-                keeps=jnp.logical_and(built_in.keeps, gl_FrontFacing),
+                keeps=jnp.logical_and(  # pyright: ignore[reportUnknownMemberType]
+                    built_in.keeps,
+                    gl_FrontFacing,
+                ),
                 use_default_depth=built_in.use_default_depth,
             ),
-            varying._replace(colour=lax.cond(
-                (light_colour >= 0).all(),
-                lambda: texture_colour * light_colour,
-                lambda: jnp.zeros(3),
-            )),
+            varying._replace(
+                colour=lax.cond(  # pyright: ignore[reportUnknownMemberType]
+                    jnp.all(  # pyright: ignore[reportUnknownMemberType]
+                        light_colour >= 0
+                    ),
+                    lambda: texture_colour * light_colour,
+                    lambda: jnp.zeros(3),  # pyright: ignore[reportUnknownMemberType]
+                )
+            ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: PhongTextureDarbouxExtraFragmentData,
-    ) -> tuple[MixerOutput, PhongTextureDarbouxExtraMixerOutput]:
+    ) -> Tuple[MixerOutput, PhongTextureDarbouxExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: PhongTextureDarbouxExtraFragmentData
-        mixer_output, extra_output = Shader.mix(gl_FragDepth, keeps, extra)
+        mixer_output, extra_output = cast(
+            Tuple[MixerOutput, PhongTextureDarbouxExtraFragmentData],
+            Shader.mix(gl_FragDepth, keeps, extra),
+        )
         assert isinstance(mixer_output, MixerOutput)
         assert isinstance(extra_output, PhongTextureDarbouxExtraFragmentData)
 
         return (
             mixer_output,
             PhongTextureDarbouxExtraMixerOutput(canvas=extra_output.colour),
         )
```

### Comparing `jaxrenderer-0.3.1/renderer/shaders/phong_reflection.py` & `jaxrenderer-0.3.2/renderer/shaders/phong_reflection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import NamedTuple
+from typing import NamedTuple, cast
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Bool, Float, Integer, jaxtyped
+from jaxtyping import Array, Bool, Float, Integer
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
+from .._backport import Tuple
 from .._meta_utils import add_tracing_name
+from .._meta_utils import typed_jit as jit
 from ..geometry import Camera, normalise, to_homogeneous
 from ..model import MergedModel
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
-from ..types import (Colour, LightSource, SpecularMap, Texture, Vec2f, Vec2i,
-                     Vec3f, Vec4f)
+from ..types import (
+    BoolV,
+    Colour,
+    FloatV,
+    IntV,
+    LightSource,
+    SpecularMap,
+    Texture,
+    Vec2f,
+    Vec2i,
+    Vec3f,
+    Vec4f,
+)
 
-jax.config.update('jax_array', True)
+jax.config.update("jax_array", True)  # pyright: ignore[reportUnknownMemberType]
 
 
 class PhongReflectionTextureExtraInput(NamedTuple):
     """Extra input for PhongReflection Shader.
 
     Attributes:
       - position: in world space, of each vertex.
@@ -32,22 +46,23 @@
       - offset_shape: offset of each texture map in the merged model.
       - texture: texture, shared by all vertices.
       - specular_map: specular map, shared by all vertices.
       - ambient: ambient strength, shared by all vertices.
       - diffuse: diffuse strength, shared by all vertices.
       - specular: specular strength, shared by all vertices.
     """
+
     position: Float[Array, "vertices 3"]  # in world space
     normal: Float[Array, "vertices 3"]  # in world space
     uv: Float[Array, "vertices 2"]  # in texture space
     light: LightSource
     light_dir_eye: Vec3f  # in eye/view space
     texture_shape: Integer[Array, "objects 2"]
     texture_index: Integer[Array, "vertices"]
-    texture_offset: Integer[Array, ""]
+    texture_offset: IntV
     texture: Texture
     specular_map: SpecularMap
     ambient: Colour
     diffuse: Colour
     specular: Colour
 
 
@@ -56,41 +71,46 @@
 
     Attributes:
       - normal: in clip space, of each fragment; From VS to FS.
       - uv: in texture space, of each fragment; From VS to FS.
       - texture_index: index of texture map for each fragment; From VS to FS.
       - colour: colour when passing from FS to mixer.
     """
-    normal: Vec3f = jnp.zeros(3)
-    uv: Vec2f = jnp.zeros(2)
-    texture_index: Integer[Array, ""] = jnp.array(0)
-    colour: Colour = jnp.zeros(3)
+
+    normal: Vec3f = jnp.zeros(3)  # pyright: ignore[reportUnknownMemberType]
+    uv: Vec2f = jnp.zeros(2)  # pyright: ignore[reportUnknownMemberType]
+    texture_index: IntV = jnp.array(0)  # pyright: ignore[reportUnknownMemberType]
+    colour: Colour = jnp.zeros(3)  # pyright: ignore[reportUnknownMemberType]
 
 
 class PhongReflectionTextureExtraMixerOutput(NamedTuple):
     """When render to only one target, for simplicity."""
+
     canvas: Colour
 
 
 class PhongReflectionTextureShader(
-        Shader[PhongReflectionTextureExtraInput,
-               PhongReflectionTextureExtraFragmentData,
-               PhongReflectionTextureExtraMixerOutput]):
+    Shader[
+        PhongReflectionTextureExtraInput,
+        PhongReflectionTextureExtraFragmentData,
+        PhongReflectionTextureExtraMixerOutput,
+    ]
+):
     """PhongReflection Shading with simple parallel lighting and texture."""
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: PhongReflectionTextureExtraInput,
-    ) -> tuple[PerVertex, PhongReflectionTextureExtraFragmentData]:
+    ) -> Tuple[PerVertex, PhongReflectionTextureExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
         position: Vec4f = to_homogeneous(extra.position[gl_VertexID])
         gl_Position: Vec4f = camera.to_clip(position)
         assert isinstance(gl_Position, Vec4f)
 
         # assume normal here is in world space. If it is in model space, it
         # must be transformed by the inverse transpose of the model matrix.
@@ -109,15 +129,15 @@
                 uv=extra.uv[gl_VertexID],
                 texture_index=extra.texture_index[gl_VertexID],
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def interpolate(
         values: PhongReflectionTextureExtraFragmentData,
         barycentric_screen: Vec3f,
         barycentric_clip: Vec3f,
     ) -> PhongReflectionTextureExtraFragmentData:
         varying = Shader.interpolate(
@@ -129,93 +149,110 @@
         varying = varying._replace(texture_index=values.texture_index[0])
         assert isinstance(varying, PhongReflectionTextureExtraFragmentData)
 
         return varying
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
-        gl_FrontFacing: Bool[Array, ""],
+        gl_FrontFacing: BoolV,
         gl_PointCoord: Vec2f,
         varying: PhongReflectionTextureExtraFragmentData,
         extra: PhongReflectionTextureExtraInput,
-    ) -> tuple[PerFragment, PhongReflectionTextureExtraFragmentData]:
+    ) -> Tuple[PerFragment, PhongReflectionTextureExtraFragmentData]:
         built_in: PerFragment = Shader.fragment(
             gl_FragCoord,
             gl_FrontFacing,
             gl_PointCoord,
             varying,
             extra,
         )[0]
         assert isinstance(built_in, PerFragment)
 
         # texture
-        texture_index = varying.texture_index.astype(int)
+        texture_index = varying.texture_index.astype(int)  # pyright: ignore
         texture_shape = extra.texture_shape[texture_index]
         uv = MergedModel.uv_repeat(
             uv=varying.uv,
             shape=texture_shape,
             map_index=texture_index,
             offset=extra.texture_offset,
         )
-        uv = lax.floor(uv).astype(int)
+        uv = lax.floor(uv).astype(int)  # pyright: ignore[reportUnknownMemberType]
         assert isinstance(uv, Vec2i)
         texture_colour: Colour = extra.texture[uv[0], uv[1]]
 
         normal: Vec3f = normalise(varying.normal)
         light_dir: Vec3f = normalise(extra.light_dir_eye)
 
         # Phong Reflection Model
-        diffuse: float = jnp.maximum(lax.dot(normal, light_dir), 0)
+        diffuse: Float[
+            Array, ""
+        ] = jnp.maximum(  # pyright: ignore[reportUnknownMemberType]
+            lax.dot(normal, light_dir),  # pyright: ignore[reportUnknownMemberType]
+            0,
+        )
         # as `light_dir * -1` should be used here, if
         # using `light_dir - 2 * diffuse * normal`
-        reflected_light: Vec3f = normalise(2 * lax.dot(normal, light_dir) *
-                                           normal - light_dir)
+        reflected_light: Vec3f = normalise(
+            2
+            * lax.dot(normal, light_dir)  # pyright: ignore[reportUnknownMemberType]
+            * normal
+            - light_dir
+        )
         assert isinstance(reflected_light, Vec3f)
 
-        specular: float = lax.pow(
-            lax.max(reflected_light[2], 0.),
+        specular: FloatV = lax.pow(  # pyright: ignore[reportUnknownMemberType]
+            lax.max(  # pyright: ignore[reportUnknownMemberType]
+                reflected_light[2], 0.0
+            ),
             extra.specular_map[uv[0], uv[1]],
         )
 
         # compute colour
         colour: Colour = (
-            extra.ambient * texture_colour +
-            (extra.diffuse * diffuse + extra.specular * specular) *
+            extra.ambient * texture_colour
+            + (extra.diffuse * diffuse + extra.specular * specular) *
             # intensity * light colour * texture colour
-            extra.light.colour * texture_colour)
+            extra.light.colour * texture_colour
+        )
 
         return (
             PerFragment(
-                keeps=jnp.logical_and(built_in.keeps, gl_FrontFacing),
+                keeps=jnp.logical_and(  # pyright: ignore[reportUnknownMemberType]
+                    built_in.keeps,
+                    gl_FrontFacing,
+                ),
                 use_default_depth=built_in.use_default_depth,
             ),
             PhongReflectionTextureExtraFragmentData(
                 colour=colour,
                 uv=varying.uv,
                 normal=varying.normal,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: PhongReflectionTextureExtraFragmentData,
-    ) -> tuple[MixerOutput, PhongReflectionTextureExtraMixerOutput]:
+    ) -> Tuple[MixerOutput, PhongReflectionTextureExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: PhongReflectionTextureExtraFragmentData
-        mixer_output, extra_output = Shader.mix(gl_FragDepth, keeps, extra)
+        mixer_output, extra_output = cast(
+            Tuple[MixerOutput, PhongReflectionTextureExtraFragmentData],
+            Shader.mix(gl_FragDepth, keeps, extra),
+        )
         assert isinstance(mixer_output, MixerOutput)
-        assert isinstance(extra_output,
-                          PhongReflectionTextureExtraFragmentData)
+        assert isinstance(extra_output, PhongReflectionTextureExtraFragmentData)
 
         return (
             mixer_output,
             PhongReflectionTextureExtraMixerOutput(canvas=extra_output.colour),
         )
```

### Comparing `jaxrenderer-0.3.1/renderer/shaders/phong_reflection_shadow.py` & `jaxrenderer-0.3.2/renderer/shaders/phong_reflection_shadow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import NamedTuple
+from typing import NamedTuple, cast
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Bool, Float, Integer, jaxtyped
+from jaxtyping import Array, Bool, Float, Integer
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
+from typing_extensions import override
 
+from .._backport import Tuple
 from .._meta_utils import add_tracing_name
+from .._meta_utils import typed_jit as jit
 from ..geometry import Camera, normalise, normalise_homogeneous, to_homogeneous
 from ..model import MergedModel
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
 from ..shadow import Shadow
-from ..types import (Colour, LightSource, SpecularMap, Texture, Vec2f, Vec2i,
-                     Vec3f, Vec4f)
+from ..types import (
+    BoolV,
+    Colour,
+    IntV,
+    LightSource,
+    SpecularMap,
+    Texture,
+    Vec2f,
+    Vec2i,
+    Vec3f,
+    Vec4f,
+)
 
-jax.config.update('jax_array', True)
+jax.config.update("jax_array", True)  # pyright: ignore[reportUnknownMemberType]
 
 
 class PhongReflectionShadowTextureExtraInput(NamedTuple):
     """Extra input for Phong Reflection with Shadow Shader.
 
     Attributes:
       - position: in world space, of each vertex.
@@ -36,22 +50,23 @@
       - shadow: Shadow from first pass, shared by all vertices.
       - shadow_mat: shadow matrix from target screen space to shadow's screen
         space, shared by all vertices.
       - ambient: ambient strength, shared by all vertices.
       - diffuse: diffuse strength, shared by all vertices.
       - specular: specular strength, shared by all vertices.
     """
+
     position: Float[Array, "vertices 3"]  # in world space
     normal: Float[Array, "vertices 3"]  # in world space
     uv: Float[Array, "vertices 2"]  # in texture space
     light: LightSource
     light_dir_eye: Vec3f  # in eye/view space.
     texture_shape: Integer[Array, "objects 2"]
     texture_index: Integer[Array, "vertices"]
-    texture_offset: Integer[Array, ""]
+    texture_offset: IntV
     texture: Texture
     specular_map: SpecularMap
     shadow: Shadow
     camera: Camera  # so accessible in FS as well.
     ambient: Colour
     diffuse: Colour
     specular: Colour
@@ -63,44 +78,50 @@
     Attributes:
       - normal: in clip space, of each fragment; From VS to FS.
       - uv: in texture space, of each fragment; From VS to FS.
       - texture_index: index of texture map for each fragment; From VS to FS.
       - shadow_coord: in shadow's clip space, of each fragment; From VS to FS.
       - colour: colour when passing from FS to mixer.
     """
-    normal: Vec3f = jnp.zeros(3)
-    uv: Vec2f = jnp.zeros(2)
-    texture_index: Integer[Array, ""] = jnp.array(0)
-    shadow_coord: Vec4f = jnp.zeros(4)
-    colour: Colour = jnp.zeros(3)
+
+    normal: Vec3f = jnp.zeros(3)  # pyright: ignore[reportUnknownMemberType]
+    uv: Vec2f = jnp.zeros(2)  # pyright: ignore[reportUnknownMemberType]
+    texture_index: IntV = jnp.array(0)  # pyright: ignore
+    shadow_coord: Vec4f = jnp.zeros(4)  # pyright: ignore[reportUnknownMemberType]
+    colour: Colour = jnp.zeros(3)  # pyright: ignore[reportUnknownMemberType]
 
 
 class PhongReflectionShadowTextureExtraMixerOutput(NamedTuple):
     """When render to only one target, for simplicity."""
+
     canvas: Colour
 
 
 class PhongReflectionShadowTextureShader(
-        Shader[PhongReflectionShadowTextureExtraInput,
-               PhongReflectionShadowTextureExtraFragmentData,
-               PhongReflectionShadowTextureExtraMixerOutput]):
+    Shader[
+        PhongReflectionShadowTextureExtraInput,
+        PhongReflectionShadowTextureExtraFragmentData,
+        PhongReflectionShadowTextureExtraMixerOutput,
+    ]
+):
     """Phong Shading with simple parallel lighting, texture, Phong Reflection
-        approximation and ShadowMap.
+    approximation and ShadowMap.
     """
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
+    @override
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: PhongReflectionShadowTextureExtraInput,
-    ) -> tuple[PerVertex, PhongReflectionShadowTextureExtraFragmentData]:
+    ) -> Tuple[PerVertex, PhongReflectionShadowTextureExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
         position: Vec4f = to_homogeneous(extra.position[gl_VertexID])
         gl_Position: Vec4f = camera.to_clip(position)
         assert isinstance(gl_Position, Vec4f)
 
         # assume normal here is in world space. If it is in model space, it
         # must be transformed by the inverse transpose of the model matrix.
@@ -110,147 +131,165 @@
             camera.world_to_eye_norm,
         )
         assert isinstance(normal, Vec3f)
 
         # shadow. Normalise here as it is not done implicitly in the pipeline.
         # the result is in shadow's clip space, as NDC.
         shadow_coord: Vec4f = normalise_homogeneous(
-            extra.shadow.camera.to_clip(position))
+            extra.shadow.camera.to_clip(position)
+        )
         assert isinstance(shadow_coord, Vec4f)
 
         return (
             PerVertex(gl_Position=gl_Position),
             PhongReflectionShadowTextureExtraFragmentData(
                 normal=normal,
                 uv=extra.uv[gl_VertexID],
                 texture_index=extra.texture_index[gl_VertexID],
                 shadow_coord=shadow_coord,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
+    @override
     def interpolate(
         values: PhongReflectionShadowTextureExtraFragmentData,
         barycentric_screen: Vec3f,
         barycentric_clip: Vec3f,
     ) -> PhongReflectionShadowTextureExtraFragmentData:
         varying = Shader.interpolate(
             values=values,
             barycentric_screen=barycentric_screen,
             barycentric_clip=barycentric_clip,
         )
         # all three values should be the same, just pick the first.
         varying = varying._replace(texture_index=values.texture_index[0])
-        assert isinstance(varying,
-                          PhongReflectionShadowTextureExtraFragmentData)
+        assert isinstance(varying, PhongReflectionShadowTextureExtraFragmentData)
 
         return varying
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
+    @override
     def fragment(
         gl_FragCoord: Vec4f,
-        gl_FrontFacing: Bool[Array, ""],
+        gl_FrontFacing: BoolV,
         gl_PointCoord: Vec2f,
         varying: PhongReflectionShadowTextureExtraFragmentData,
         extra: PhongReflectionShadowTextureExtraInput,
-    ) -> tuple[PerFragment, PhongReflectionShadowTextureExtraFragmentData]:
+    ) -> Tuple[PerFragment, PhongReflectionShadowTextureExtraFragmentData]:
         built_in: PerFragment = Shader.fragment(
             gl_FragCoord,
             gl_FrontFacing,
             gl_PointCoord,
             varying,
             extra,
         )[0]
         assert isinstance(built_in, PerFragment)
 
         # shadow
         # from NDC to screen coordinates, in shadow's screen space.
         shadow_coord: Vec4f = normalise_homogeneous(
-            extra.shadow.camera.viewport @ varying.shadow_coord)
+            extra.shadow.camera.viewport @ varying.shadow_coord
+        )
         assert isinstance(shadow_coord, Vec4f)
         shadow_str: Colour = extra.shadow.strength
         assert isinstance(shadow_str, Colour)
-        shadow: Colour = jnp.where(
+        shadow: Colour = jnp.where(  # pyright: ignore[reportUnknownMemberType]
             # if before/at shadow
             shadow_coord[2] <= extra.shadow.get(shadow_coord[:2]),
             # when not in shadow, keeps all light.
-            jnp.ones_like(shadow_str),
+            jnp.ones_like(shadow_str),  # pyright: ignore[reportUnknownMemberType]
             # if in shadow, only keep "1 - shadow_str" amount of light.
-            1. - shadow_str,
+            1.0 - shadow_str,
         )
 
         # texture
-        texture_index = varying.texture_index.astype(int)
+        texture_index = varying.texture_index.astype(int)  # pyright: ignore
         texture_shape = extra.texture_shape[texture_index]
         uv = MergedModel.uv_repeat(
             uv=varying.uv,
             shape=texture_shape,
             map_index=texture_index,
             offset=extra.texture_offset,
         )
-        uv = lax.floor(uv).astype(int)
+        uv = lax.floor(uv).astype(int)  # pyright: ignore[reportUnknownMemberType]
         assert isinstance(uv, Vec2i)
         texture_colour: Colour = extra.texture[uv[0], uv[1]]
 
         normal: Vec3f = normalise(varying.normal)
         # in Phong shading, the light direction is towards the light source;
         light_dir: Vec3f = normalise(extra.light_dir_eye)
 
         # Phong Reflection Model
-        diffuse: float = jnp.maximum(lax.dot(normal, light_dir), 0)
+        diffuse: Float[
+            Array, ""
+        ] = jnp.maximum(  # pyright: ignore[reportUnknownMemberType]
+            lax.dot(normal, light_dir),  # pyright: ignore[reportUnknownMemberType]
+            0,
+        )
         # If using standard reflection formula
         # `light_dir - 2 * diffuse * normal`, need to use
         # `-1 * light_dir` as `light_dir` instead.
-        reflected_light: Vec3f = normalise(2 * lax.dot(normal, light_dir) *
-                                           normal - light_dir)
+        reflected_light: Vec3f = normalise(
+            2 * lax.dot(normal, light_dir) * normal - light_dir  # pyright: ignore
+        )
         assert isinstance(reflected_light, Vec3f)
 
-        specular: float = lax.pow(
-            lax.max(reflected_light[2], 0.),
+        specular: Float[
+            Array, ""
+        ] = lax.pow(  # pyright: ignore[reportUnknownMemberType]
+            lax.max(reflected_light[2], 0.0),  # pyright: ignore
             extra.specular_map[uv[0], uv[1]],
         )
 
         # compute colour
         colour: Colour = (
-            extra.ambient * texture_colour + shadow *
-            (extra.diffuse * diffuse + extra.specular * specular) *
-            texture_colour * extra.light.colour)
+            extra.ambient * texture_colour
+            + shadow
+            * (extra.diffuse * diffuse + extra.specular * specular)
+            * texture_colour
+            * extra.light.colour
+        )
 
         return (
             PerFragment(
-                keeps=jnp.logical_and(built_in.keeps, gl_FrontFacing),
+                keeps=jnp.logical_and(  # pyright: ignore[reportUnknownMemberType]
+                    built_in.keeps, gl_FrontFacing
+                ),
                 use_default_depth=built_in.use_default_depth,
             ),
             PhongReflectionShadowTextureExtraFragmentData(
                 colour=colour,
                 uv=varying.uv,
                 normal=varying.normal,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, inline=True)
+    @partial(jit, inline=True)
     @add_tracing_name
+    @override
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: PhongReflectionShadowTextureExtraFragmentData,
-    ) -> tuple[MixerOutput, PhongReflectionShadowTextureExtraMixerOutput]:
+    ) -> Tuple[MixerOutput, PhongReflectionShadowTextureExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: PhongReflectionShadowTextureExtraFragmentData
-        mixer_output, extra_output = Shader.mix(gl_FragDepth, keeps, extra)
+        mixer_output, extra_output = cast(
+            Tuple[MixerOutput, PhongReflectionShadowTextureExtraFragmentData],
+            Shader.mix(gl_FragDepth, keeps, extra),
+        )
         assert isinstance(mixer_output, MixerOutput)
-        assert isinstance(extra_output,
-                          PhongReflectionShadowTextureExtraFragmentData)
+        assert isinstance(extra_output, PhongReflectionShadowTextureExtraFragmentData)
 
         return (
             mixer_output,
-            PhongReflectionShadowTextureExtraMixerOutput(
-                canvas=extra_output.colour),
+            PhongReflectionShadowTextureExtraMixerOutput(canvas=extra_output.colour),
         )
```

### Comparing `jaxrenderer-0.3.1/renderer/shadow.py` & `jaxrenderer-0.3.2/renderer/shadow.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Float, jaxtyped
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
+from ._backport import Tuple
 from ._meta_utils import add_tracing_name
 from .geometry import Camera, View, Viewport
 from .pipeline import render
 from .shaders.depth import DepthExtraInput, DepthShader
-from .types import (Buffers, Colour, FaceIndices, Vec2f, Vec2i, Vec3f,
-                    Vertices, ZBuffer)
+from .types import (
+    Buffers,
+    Colour,
+    FaceIndices,
+    FloatV,
+    Vec2f,
+    Vec2i,
+    Vec3f,
+    Vertices,
+    ZBuffer,
+)
 
 
 class Shadow(NamedTuple):
     """Shadow map for one light source."""
+
     shadow_map: ZBuffer
     """Depth map of the scene from the light source's point of view."""
     strength: Colour
     """Strength of shadow. Must be in [0, 1]. 0 means no shadow, 1 means fully
     black shadow. (1 - strength) of the original colour will be added to the
     shadowed colour.
     """
     camera: Camera
     """Camera from world space to shadow map's screen space."""
 
     @staticmethod
     @jaxtyped
     @partial(
-        jax.jit,
-        static_argnames=("loop_unroll", ),
-        donate_argnums=(0, ),
+        jax.jit,  # pyright: ignore[reportUnknownMemberType]
+        static_argnames=("loop_unroll",),
+        donate_argnums=(0,),
         inline=True,
     )
     @add_tracing_name
     def render_shadow_map(
         shadow_map: ZBuffer,
         verts: Vertices,
         faces: FaceIndices,
         light_direction: Vec3f,
         viewport_matrix: Viewport,
         centre: Vec3f,
         up: Vec3f,
         strength: Colour,
         offset: float = 0.001,
-        distance: float = 10.,
+        distance: float = 10.0,
         loop_unroll: int = 1,
     ) -> "Shadow":
         """Render shadow map from light source's point of view.
 
         Parameters:
           - shadow_map: ZBuffer to store the depth map.
           - verts: vertices of the object.
@@ -77,26 +88,26 @@
             up=up,
         )
         assert isinstance(view, View)
 
         _camera: Camera = Camera.create(
             view=view,
             projection=Camera.orthographic_projection_matrix(
-                left=-1.,
-                right=1.,
-                bottom=-1.,
-                top=1.,
-                z_near=-1.,
-                z_far=1.,
+                left=-1.0,
+                right=1.0,
+                bottom=-1.0,
+                top=1.0,
+                z_near=-1.0,
+                z_far=1.0,
             ),
             viewport=viewport_matrix,
         )
         assert isinstance(_camera, Camera)
 
-        buffers = Buffers(zbuffer=shadow_map, targets=tuple())
+        buffers: Buffers[Tuple[()]] = Buffers(zbuffer=shadow_map, targets=tuple())
         extra = DepthExtraInput(position=verts)
         shadow_map, _ = render(
             _camera,
             DepthShader,
             buffers,
             faces,
             extra,
@@ -110,31 +121,33 @@
             strength=strength,
             camera=_camera,
         )
 
         return shadow
 
     @jaxtyped
-    @partial(jax.jit, inline=True)
     @add_tracing_name
-    def get(self, position: Vec2f) -> Float[Array, ""]:
+    def get(self, position: Vec2f) -> FloatV:
         """Get shadow depth at `position`.
 
         Parameters:
           - position: position in shadow buffer's screen space.
         """
         assert isinstance(position, Vec2f), f"{position} is not a Vec3f."
 
-        pos: Vec2i = lax.round(position[:2]).astype(int)
+        pos: Vec2i = lax.round(  # pyright: ignore[reportUnknownMemberType]
+            position[:2]
+        ).astype(int)
         assert isinstance(pos, Vec2i)
 
-        value: Float[Array, ""]
-        value = self.shadow_map.at[pos[0], pos[1]].get(
+        value: FloatV = self.shadow_map.at[
+            pos[0], pos[1]
+        ].get(  # pyright: ignore[reportUnknownMemberType]
             mode="fill",
             indices_are_sorted=True,
             unique_indices=True,
             # outside shadow map, no shadow
             fill_value=jnp.inf,
         )
-        assert isinstance(value, Float[Array, ""])
+        assert isinstance(value, FloatV)
 
         return value
```

### Comparing `jaxrenderer-0.3.1/renderer/shapes/capsule.py` & `jaxrenderer-0.3.2/renderer/shapes/capsule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,1959 +1,1974 @@
 import enum
 
 import jax
-import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Float, Integer, jaxtyped
+from jaxtyping import Array, Integer
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
 from ..model import Model
-from ..types import (FaceIndices, Normals, SpecularMap, Texture, UVCoordinates,
-                     Vertices)
+from ..types import (
+    FaceIndices,
+    FloatV,
+    Normals,
+    SpecularMap,
+    Texture,
+    UVCoordinates,
+    Vertices,
+)
 
 with jax.ensure_compile_time_eval():
-    _verts: Vertices = jnp.array((
-        (0.000000, 0.879385, 0.500000),
-        (0.000000, 0.652704, 0.766044),
-        (0.326352, 0.565258, 0.766044),
-        (0.000000, 0.879385, 0.500000),
-        (0.326352, 0.565258, 0.766044),
-        (0.439693, 0.761570, 0.500000),
-        (0.000000, 0.652704, -0.766044),
-        (0.000000, 0.879385, -0.500000),
-        (0.439693, 0.761570, -0.500000),
-        (0.000000, 0.652704, -0.766044),
-        (0.439693, 0.761570, -0.500000),
-        (0.326352, 0.565258, -0.766044),
-        (0.000000, 1.000000, 0.173648),
-        (0.000000, 0.879385, 0.500000),
-        (0.439693, 0.761570, 0.500000),
-        (0.000000, 1.000000, 0.173648),
-        (0.439693, 0.761570, 0.500000),
-        (0.500000, 0.866026, 0.173648),
-        (0.000000, 0.347296, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (0.173648, 0.300768, 0.939693),
-        (0.000000, 0.347296, -0.939693),
-        (0.000000, 0.652704, -0.766044),
-        (0.326352, 0.565258, -0.766044),
-        (0.000000, 0.347296, -0.939693),
-        (0.326352, 0.565258, -0.766044),
-        (0.173648, 0.300768, -0.939693),
-        (0.000000, 1.000000, -0.173648),
-        (0.000000, 1.000000, 0.173648),
-        (0.500000, 0.866026, 0.173648),
-        (0.000000, 1.000000, -0.173648),
-        (0.500000, 0.866026, 0.173648),
-        (0.500000, 0.866026, -0.173648),
-        (0.000000, 0.652704, 0.766044),
-        (0.000000, 0.347296, 0.939693),
-        (0.173648, 0.300768, 0.939693),
-        (0.000000, 0.652704, 0.766044),
-        (0.173648, 0.300768, 0.939693),
-        (0.326352, 0.565258, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (0.000000, 0.347296, -0.939693),
-        (0.173648, 0.300768, -0.939693),
-        (0.000000, 0.879385, -0.500000),
-        (0.000000, 1.000000, -0.173648),
-        (0.500000, 0.866026, -0.173648),
-        (0.000000, 0.879385, -0.500000),
-        (0.500000, 0.866026, -0.173648),
-        (0.439693, 0.761570, -0.500000),
-        (0.500000, 0.866026, 0.173648),
-        (0.439693, 0.761570, 0.500000),
-        (0.761570, 0.439693, 0.500000),
-        (0.500000, 0.866026, 0.173648),
-        (0.761570, 0.439693, 0.500000),
-        (0.866025, 0.500000, 0.173648),
-        (0.173648, 0.300768, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (0.300767, 0.173648, 0.939693),
-        (0.173648, 0.300768, -0.939693),
-        (0.326352, 0.565258, -0.766044),
-        (0.565258, 0.326352, -0.766044),
-        (0.173648, 0.300768, -0.939693),
-        (0.565258, 0.326352, -0.766044),
-        (0.300767, 0.173648, -0.939693),
-        (0.500000, 0.866026, -0.173648),
-        (0.500000, 0.866026, 0.173648),
-        (0.866025, 0.500000, 0.173648),
-        (0.500000, 0.866026, -0.173648),
-        (0.866025, 0.500000, 0.173648),
-        (0.866025, 0.500000, -0.173648),
-        (0.326352, 0.565258, 0.766044),
-        (0.173648, 0.300768, 0.939693),
-        (0.300767, 0.173648, 0.939693),
-        (0.326352, 0.565258, 0.766044),
-        (0.300767, 0.173648, 0.939693),
-        (0.565258, 0.326352, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (0.173648, 0.300768, -0.939693),
-        (0.300767, 0.173648, -0.939693),
-        (0.439693, 0.761570, -0.500000),
-        (0.500000, 0.866026, -0.173648),
-        (0.866025, 0.500000, -0.173648),
-        (0.439693, 0.761570, -0.500000),
-        (0.866025, 0.500000, -0.173648),
-        (0.761570, 0.439693, -0.500000),
-        (0.439693, 0.761570, 0.500000),
-        (0.326352, 0.565258, 0.766044),
-        (0.565258, 0.326352, 0.766044),
-        (0.439693, 0.761570, 0.500000),
-        (0.565258, 0.326352, 0.766044),
-        (0.761570, 0.439693, 0.500000),
-        (0.326352, 0.565258, -0.766044),
-        (0.439693, 0.761570, -0.500000),
-        (0.761570, 0.439693, -0.500000),
-        (0.326352, 0.565258, -0.766044),
-        (0.761570, 0.439693, -0.500000),
-        (0.565258, 0.326352, -0.766044),
-        (0.565258, 0.326352, 0.766044),
-        (0.300767, 0.173648, 0.939693),
-        (0.347296, 0.000000, 0.939693),
-        (0.565258, 0.326352, 0.766044),
-        (0.347296, 0.000000, 0.939693),
-        (0.652704, 0.000000, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (0.300767, 0.173648, -0.939693),
-        (0.347296, 0.000000, -0.939693),
-        (0.761570, 0.439693, -0.500000),
-        (0.866025, 0.500000, -0.173648),
-        (1.000000, 0.000000, -0.173648),
-        (0.761570, 0.439693, -0.500000),
-        (1.000000, 0.000000, -0.173648),
-        (0.879385, 0.000000, -0.500000),
-        (0.761570, 0.439693, 0.500000),
-        (0.565258, 0.326352, 0.766044),
-        (0.652704, 0.000000, 0.766044),
-        (0.761570, 0.439693, 0.500000),
-        (0.652704, 0.000000, 0.766044),
-        (0.879385, 0.000000, 0.500000),
-        (0.565258, 0.326352, -0.766044),
-        (0.761570, 0.439693, -0.500000),
-        (0.879385, 0.000000, -0.500000),
-        (0.565258, 0.326352, -0.766044),
-        (0.879385, 0.000000, -0.500000),
-        (0.652704, 0.000000, -0.766044),
-        (0.866025, 0.500000, 0.173648),
-        (0.761570, 0.439693, 0.500000),
-        (0.879385, 0.000000, 0.500000),
-        (0.866025, 0.500000, 0.173648),
-        (0.879385, 0.000000, 0.500000),
-        (1.000000, 0.000000, 0.173648),
-        (0.300767, 0.173648, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (0.347296, 0.000000, 0.939693),
-        (0.300767, 0.173648, -0.939693),
-        (0.565258, 0.326352, -0.766044),
-        (0.652704, 0.000000, -0.766044),
-        (0.300767, 0.173648, -0.939693),
-        (0.652704, 0.000000, -0.766044),
-        (0.347296, 0.000000, -0.939693),
-        (0.866025, 0.500000, -0.173648),
-        (0.866025, 0.500000, 0.173648),
-        (1.000000, 0.000000, 0.173648),
-        (0.866025, 0.500000, -0.173648),
-        (1.000000, 0.000000, 0.173648),
-        (1.000000, 0.000000, -0.173648),
-        (0.652704, 0.000000, -0.766044),
-        (0.879385, 0.000000, -0.500000),
-        (0.761570, -0.439692, -0.500000),
-        (0.652704, 0.000000, -0.766044),
-        (0.761570, -0.439692, -0.500000),
-        (0.565258, -0.326352, -0.766044),
-        (1.000000, 0.000000, 0.173648),
-        (0.879385, 0.000000, 0.500000),
-        (0.761570, -0.439692, 0.500000),
-        (1.000000, 0.000000, 0.173648),
-        (0.761570, -0.439692, 0.500000),
-        (0.866025, -0.500000, 0.173648),
-        (0.347296, 0.000000, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (0.300767, -0.173648, 0.939693),
-        (0.347296, 0.000000, -0.939693),
-        (0.652704, 0.000000, -0.766044),
-        (0.565258, -0.326352, -0.766044),
-        (0.347296, 0.000000, -0.939693),
-        (0.565258, -0.326352, -0.766044),
-        (0.300767, -0.173648, -0.939693),
-        (1.000000, 0.000000, -0.173648),
-        (1.000000, 0.000000, 0.173648),
-        (0.866025, -0.500000, 0.173648),
-        (1.000000, 0.000000, -0.173648),
-        (0.866025, -0.500000, 0.173648),
-        (0.866025, -0.500000, -0.173648),
-        (0.652704, 0.000000, 0.766044),
-        (0.347296, 0.000000, 0.939693),
-        (0.300767, -0.173648, 0.939693),
-        (0.652704, 0.000000, 0.766044),
-        (0.300767, -0.173648, 0.939693),
-        (0.565258, -0.326352, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (0.347296, 0.000000, -0.939693),
-        (0.300767, -0.173648, -0.939693),
-        (0.879385, 0.000000, -0.500000),
-        (1.000000, 0.000000, -0.173648),
-        (0.866025, -0.500000, -0.173648),
-        (0.879385, 0.000000, -0.500000),
-        (0.866025, -0.500000, -0.173648),
-        (0.761570, -0.439692, -0.500000),
-        (0.879385, 0.000000, 0.500000),
-        (0.652704, 0.000000, 0.766044),
-        (0.565258, -0.326352, 0.766044),
-        (0.879385, 0.000000, 0.500000),
-        (0.565258, -0.326352, 0.766044),
-        (0.761570, -0.439692, 0.500000),
-        (0.866025, -0.500000, -0.173648),
-        (0.866025, -0.500000, 0.173648),
-        (0.500000, -0.866025, 0.173648),
-        (0.866025, -0.500000, -0.173648),
-        (0.500000, -0.866025, 0.173648),
-        (0.500000, -0.866025, -0.173648),
-        (0.565258, -0.326352, 0.766044),
-        (0.300767, -0.173648, 0.939693),
-        (0.173648, -0.300767, 0.939693),
-        (0.565258, -0.326352, 0.766044),
-        (0.173648, -0.300767, 0.939693),
-        (0.326352, -0.565258, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (0.300767, -0.173648, -0.939693),
-        (0.173648, -0.300767, -0.939693),
-        (0.761570, -0.439692, -0.500000),
-        (0.866025, -0.500000, -0.173648),
-        (0.500000, -0.866025, -0.173648),
-        (0.761570, -0.439692, -0.500000),
-        (0.500000, -0.866025, -0.173648),
-        (0.439693, -0.761570, -0.500000),
-        (0.761570, -0.439692, 0.500000),
-        (0.565258, -0.326352, 0.766044),
-        (0.326352, -0.565258, 0.766044),
-        (0.761570, -0.439692, 0.500000),
-        (0.326352, -0.565258, 0.766044),
-        (0.439693, -0.761570, 0.500000),
-        (0.565258, -0.326352, -0.766044),
-        (0.761570, -0.439692, -0.500000),
-        (0.439693, -0.761570, -0.500000),
-        (0.565258, -0.326352, -0.766044),
-        (0.439693, -0.761570, -0.500000),
-        (0.326352, -0.565258, -0.766044),
-        (0.866025, -0.500000, 0.173648),
-        (0.761570, -0.439692, 0.500000),
-        (0.439693, -0.761570, 0.500000),
-        (0.866025, -0.500000, 0.173648),
-        (0.439693, -0.761570, 0.500000),
-        (0.500000, -0.866025, 0.173648),
-        (0.300767, -0.173648, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (0.173648, -0.300767, 0.939693),
-        (0.300767, -0.173648, -0.939693),
-        (0.565258, -0.326352, -0.766044),
-        (0.326352, -0.565258, -0.766044),
-        (0.300767, -0.173648, -0.939693),
-        (0.326352, -0.565258, -0.766044),
-        (0.173648, -0.300767, -0.939693),
-        (0.439693, -0.761570, 0.500000),
-        (0.326352, -0.565258, 0.766044),
-        (0.000000, -0.652703, 0.766044),
-        (0.439693, -0.761570, 0.500000),
-        (0.000000, -0.652703, 0.766044),
-        (0.000000, -0.879385, 0.500000),
-        (0.326352, -0.565258, -0.766044),
-        (0.439693, -0.761570, -0.500000),
-        (0.000000, -0.879385, -0.500000),
-        (0.326352, -0.565258, -0.766044),
-        (0.000000, -0.879385, -0.500000),
-        (0.000000, -0.652703, -0.766044),
-        (0.500000, -0.866025, 0.173648),
-        (0.439693, -0.761570, 0.500000),
-        (0.000000, -0.879385, 0.500000),
-        (0.500000, -0.866025, 0.173648),
-        (0.000000, -0.879385, 0.500000),
-        (0.000000, -1.000000, 0.173648),
-        (0.173648, -0.300767, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (0.000000, -0.347296, 0.939693),
-        (0.173648, -0.300767, -0.939693),
-        (0.326352, -0.565258, -0.766044),
-        (0.000000, -0.652703, -0.766044),
-        (0.173648, -0.300767, -0.939693),
-        (0.000000, -0.652703, -0.766044),
-        (0.000000, -0.347296, -0.939693),
-        (0.500000, -0.866025, -0.173648),
-        (0.500000, -0.866025, 0.173648),
-        (0.000000, -1.000000, 0.173648),
-        (0.500000, -0.866025, -0.173648),
-        (0.000000, -1.000000, 0.173648),
-        (0.000000, -1.000000, -0.173648),
-        (0.326352, -0.565258, 0.766044),
-        (0.173648, -0.300767, 0.939693),
-        (0.000000, -0.347296, 0.939693),
-        (0.326352, -0.565258, 0.766044),
-        (0.000000, -0.347296, 0.939693),
-        (0.000000, -0.652703, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (0.173648, -0.300767, -0.939693),
-        (0.000000, -0.347296, -0.939693),
-        (0.439693, -0.761570, -0.500000),
-        (0.500000, -0.866025, -0.173648),
-        (0.000000, -1.000000, -0.173648),
-        (0.439693, -0.761570, -0.500000),
-        (0.000000, -1.000000, -0.173648),
-        (0.000000, -0.879385, -0.500000),
-        (0.000000, -0.347296, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (-0.173648, -0.300767, 0.939693),
-        (0.000000, -0.347296, -0.939693),
-        (0.000000, -0.652703, -0.766044),
-        (-0.326352, -0.565258, -0.766044),
-        (0.000000, -0.347296, -0.939693),
-        (-0.326352, -0.565258, -0.766044),
-        (-0.173648, -0.300767, -0.939693),
-        (0.000000, -1.000000, -0.173648),
-        (0.000000, -1.000000, 0.173648),
-        (-0.500000, -0.866025, 0.173648),
-        (0.000000, -1.000000, -0.173648),
-        (-0.500000, -0.866025, 0.173648),
-        (-0.500000, -0.866025, -0.173648),
-        (0.000000, -0.652703, 0.766044),
-        (0.000000, -0.347296, 0.939693),
-        (-0.173648, -0.300767, 0.939693),
-        (0.000000, -0.652703, 0.766044),
-        (-0.173648, -0.300767, 0.939693),
-        (-0.326352, -0.565258, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (0.000000, -0.347296, -0.939693),
-        (-0.173648, -0.300767, -0.939693),
-        (0.000000, -0.879385, -0.500000),
-        (0.000000, -1.000000, -0.173648),
-        (-0.500000, -0.866025, -0.173648),
-        (0.000000, -0.879385, -0.500000),
-        (-0.500000, -0.866025, -0.173648),
-        (-0.439693, -0.761570, -0.500000),
-        (0.000000, -0.879385, 0.500000),
-        (0.000000, -0.652703, 0.766044),
-        (-0.326352, -0.565258, 0.766044),
-        (0.000000, -0.879385, 0.500000),
-        (-0.326352, -0.565258, 0.766044),
-        (-0.439693, -0.761570, 0.500000),
-        (0.000000, -0.652703, -0.766044),
-        (0.000000, -0.879385, -0.500000),
-        (-0.439693, -0.761570, -0.500000),
-        (0.000000, -0.652703, -0.766044),
-        (-0.439693, -0.761570, -0.500000),
-        (-0.326352, -0.565258, -0.766044),
-        (0.000000, -1.000000, 0.173648),
-        (0.000000, -0.879385, 0.500000),
-        (-0.439693, -0.761570, 0.500000),
-        (0.000000, -1.000000, 0.173648),
-        (-0.439693, -0.761570, 0.500000),
-        (-0.500000, -0.866025, 0.173648),
-        (0.000000, 0.000000, -1.000000),
-        (-0.173648, -0.300767, -0.939693),
-        (-0.300767, -0.173648, -0.939693),
-        (-0.439693, -0.761570, -0.500000),
-        (-0.500000, -0.866025, -0.173648),
-        (-0.866025, -0.500000, -0.173648),
-        (-0.439693, -0.761570, -0.500000),
-        (-0.866025, -0.500000, -0.173648),
-        (-0.761570, -0.439692, -0.500000),
-        (-0.439693, -0.761570, 0.500000),
-        (-0.326352, -0.565258, 0.766044),
-        (-0.565258, -0.326352, 0.766044),
-        (-0.439693, -0.761570, 0.500000),
-        (-0.565258, -0.326352, 0.766044),
-        (-0.761570, -0.439692, 0.500000),
-        (-0.326352, -0.565258, -0.766044),
-        (-0.439693, -0.761570, -0.500000),
-        (-0.761570, -0.439692, -0.500000),
-        (-0.326352, -0.565258, -0.766044),
-        (-0.761570, -0.439692, -0.500000),
-        (-0.565258, -0.326352, -0.766044),
-        (-0.500000, -0.866025, 0.173648),
-        (-0.439693, -0.761570, 0.500000),
-        (-0.761570, -0.439692, 0.500000),
-        (-0.500000, -0.866025, 0.173648),
-        (-0.761570, -0.439692, 0.500000),
-        (-0.866025, -0.500000, 0.173648),
-        (-0.173648, -0.300767, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (-0.300767, -0.173648, 0.939693),
-        (-0.173648, -0.300767, -0.939693),
-        (-0.326352, -0.565258, -0.766044),
-        (-0.565258, -0.326352, -0.766044),
-        (-0.173648, -0.300767, -0.939693),
-        (-0.565258, -0.326352, -0.766044),
-        (-0.300767, -0.173648, -0.939693),
-        (-0.500000, -0.866025, -0.173648),
-        (-0.500000, -0.866025, 0.173648),
-        (-0.866025, -0.500000, 0.173648),
-        (-0.500000, -0.866025, -0.173648),
-        (-0.866025, -0.500000, 0.173648),
-        (-0.866025, -0.500000, -0.173648),
-        (-0.326352, -0.565258, 0.766044),
-        (-0.173648, -0.300767, 0.939693),
-        (-0.300767, -0.173648, 0.939693),
-        (-0.326352, -0.565258, 0.766044),
-        (-0.300767, -0.173648, 0.939693),
-        (-0.565258, -0.326352, 0.766044),
-        (-0.565258, -0.326352, -0.766044),
-        (-0.761570, -0.439692, -0.500000),
-        (-0.879385, 0.000000, -0.500000),
-        (-0.565258, -0.326352, -0.766044),
-        (-0.879385, 0.000000, -0.500000),
-        (-0.652704, 0.000000, -0.766044),
-        (-0.866025, -0.500000, 0.173648),
-        (-0.761570, -0.439692, 0.500000),
-        (-0.879385, 0.000000, 0.500000),
-        (-0.866025, -0.500000, 0.173648),
-        (-0.879385, 0.000000, 0.500000),
-        (-1.000000, 0.000000, 0.173648),
-        (-0.300767, -0.173648, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (-0.347296, 0.000000, 0.939693),
-        (-0.300767, -0.173648, -0.939693),
-        (-0.565258, -0.326352, -0.766044),
-        (-0.652704, 0.000000, -0.766044),
-        (-0.300767, -0.173648, -0.939693),
-        (-0.652704, 0.000000, -0.766044),
-        (-0.347296, 0.000000, -0.939693),
-        (-0.866025, -0.500000, -0.173648),
-        (-0.866025, -0.500000, 0.173648),
-        (-1.000000, 0.000000, 0.173648),
-        (-0.866025, -0.500000, -0.173648),
-        (-1.000000, 0.000000, 0.173648),
-        (-1.000000, 0.000000, -0.173648),
-        (-0.565258, -0.326352, 0.766044),
-        (-0.300767, -0.173648, 0.939693),
-        (-0.347296, 0.000000, 0.939693),
-        (-0.565258, -0.326352, 0.766044),
-        (-0.347296, 0.000000, 0.939693),
-        (-0.652704, 0.000000, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (-0.300767, -0.173648, -0.939693),
-        (-0.347296, 0.000000, -0.939693),
-        (-0.761570, -0.439692, -0.500000),
-        (-0.866025, -0.500000, -0.173648),
-        (-1.000000, 0.000000, -0.173648),
-        (-0.761570, -0.439692, -0.500000),
-        (-1.000000, 0.000000, -0.173648),
-        (-0.879385, 0.000000, -0.500000),
-        (-0.761570, -0.439692, 0.500000),
-        (-0.565258, -0.326352, 0.766044),
-        (-0.652704, 0.000000, 0.766044),
-        (-0.761570, -0.439692, 0.500000),
-        (-0.652704, 0.000000, 0.766044),
-        (-0.879385, 0.000000, 0.500000),
-        (-1.000000, 0.000000, -0.173648),
-        (-1.000000, 0.000000, 0.173648),
-        (-0.866025, 0.500000, 0.173648),
-        (-1.000000, 0.000000, -0.173648),
-        (-0.866025, 0.500000, 0.173648),
-        (-0.866025, 0.500000, -0.173648),
-        (-0.652704, 0.000000, 0.766044),
-        (-0.347296, 0.000000, 0.939693),
-        (-0.300767, 0.173648, 0.939693),
-        (-0.652704, 0.000000, 0.766044),
-        (-0.300767, 0.173648, 0.939693),
-        (-0.565258, 0.326352, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (-0.347296, 0.000000, -0.939693),
-        (-0.300767, 0.173648, -0.939693),
-        (-0.879385, 0.000000, -0.500000),
-        (-1.000000, 0.000000, -0.173648),
-        (-0.866025, 0.500000, -0.173648),
-        (-0.879385, 0.000000, -0.500000),
-        (-0.866025, 0.500000, -0.173648),
-        (-0.761570, 0.439693, -0.500000),
-        (-0.879385, 0.000000, 0.500000),
-        (-0.652704, 0.000000, 0.766044),
-        (-0.565258, 0.326352, 0.766044),
-        (-0.879385, 0.000000, 0.500000),
-        (-0.565258, 0.326352, 0.766044),
-        (-0.761570, 0.439693, 0.500000),
-        (-0.652704, 0.000000, -0.766044),
-        (-0.879385, 0.000000, -0.500000),
-        (-0.761570, 0.439693, -0.500000),
-        (-0.652704, 0.000000, -0.766044),
-        (-0.761570, 0.439693, -0.500000),
-        (-0.565258, 0.326352, -0.766044),
-        (-1.000000, 0.000000, 0.173648),
-        (-0.879385, 0.000000, 0.500000),
-        (-0.761570, 0.439693, 0.500000),
-        (-1.000000, 0.000000, 0.173648),
-        (-0.761570, 0.439693, 0.500000),
-        (-0.866025, 0.500000, 0.173648),
-        (-0.347296, 0.000000, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (-0.300767, 0.173648, 0.939693),
-        (-0.347296, 0.000000, -0.939693),
-        (-0.652704, 0.000000, -0.766044),
-        (-0.565258, 0.326352, -0.766044),
-        (-0.347296, 0.000000, -0.939693),
-        (-0.565258, 0.326352, -0.766044),
-        (-0.300767, 0.173648, -0.939693),
-        (-0.761570, 0.439693, 0.500000),
-        (-0.565258, 0.326352, 0.766044),
-        (-0.326352, 0.565258, 0.766044),
-        (-0.761570, 0.439693, 0.500000),
-        (-0.326352, 0.565258, 0.766044),
-        (-0.439693, 0.761570, 0.500000),
-        (-0.565258, 0.326352, -0.766044),
-        (-0.761570, 0.439693, -0.500000),
-        (-0.439693, 0.761570, -0.500000),
-        (-0.565258, 0.326352, -0.766044),
-        (-0.439693, 0.761570, -0.500000),
-        (-0.326352, 0.565258, -0.766044),
-        (-0.866025, 0.500000, 0.173648),
-        (-0.761570, 0.439693, 0.500000),
-        (-0.439693, 0.761570, 0.500000),
-        (-0.866025, 0.500000, 0.173648),
-        (-0.439693, 0.761570, 0.500000),
-        (-0.500000, 0.866026, 0.173648),
-        (-0.300767, 0.173648, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (-0.173648, 0.300767, 0.939693),
-        (-0.300767, 0.173648, -0.939693),
-        (-0.565258, 0.326352, -0.766044),
-        (-0.326352, 0.565258, -0.766044),
-        (-0.300767, 0.173648, -0.939693),
-        (-0.326352, 0.565258, -0.766044),
-        (-0.173648, 0.300768, -0.939693),
-        (-0.866025, 0.500000, -0.173648),
-        (-0.866025, 0.500000, 0.173648),
-        (-0.500000, 0.866026, 0.173648),
-        (-0.866025, 0.500000, -0.173648),
-        (-0.500000, 0.866026, 0.173648),
-        (-0.500000, 0.866025, -0.173648),
-        (-0.565258, 0.326352, 0.766044),
-        (-0.300767, 0.173648, 0.939693),
-        (-0.173648, 0.300767, 0.939693),
-        (-0.565258, 0.326352, 0.766044),
-        (-0.173648, 0.300767, 0.939693),
-        (-0.326352, 0.565258, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (-0.300767, 0.173648, -0.939693),
-        (-0.173648, 0.300768, -0.939693),
-        (-0.761570, 0.439693, -0.500000),
-        (-0.866025, 0.500000, -0.173648),
-        (-0.500000, 0.866025, -0.173648),
-        (-0.761570, 0.439693, -0.500000),
-        (-0.500000, 0.866025, -0.173648),
-        (-0.439693, 0.761570, -0.500000),
-        (-0.173648, 0.300767, 0.939693),
-        (0.000000, 0.000000, 1.000000),
-        (0.000000, 0.347296, 0.939693),
-        (-0.173648, 0.300768, -0.939693),
-        (-0.326352, 0.565258, -0.766044),
-        (0.000000, 0.652704, -0.766044),
-        (-0.173648, 0.300768, -0.939693),
-        (0.000000, 0.652704, -0.766044),
-        (0.000000, 0.347296, -0.939693),
-        (-0.500000, 0.866025, -0.173648),
-        (-0.500000, 0.866026, 0.173648),
-        (0.000000, 1.000000, 0.173648),
-        (-0.500000, 0.866025, -0.173648),
-        (0.000000, 1.000000, 0.173648),
-        (0.000000, 1.000000, -0.173648),
-        (-0.326352, 0.565258, 0.766044),
-        (-0.173648, 0.300767, 0.939693),
-        (0.000000, 0.347296, 0.939693),
-        (-0.326352, 0.565258, 0.766044),
-        (0.000000, 0.347296, 0.939693),
-        (0.000000, 0.652704, 0.766044),
-        (0.000000, 0.000000, -1.000000),
-        (-0.173648, 0.300768, -0.939693),
-        (0.000000, 0.347296, -0.939693),
-        (-0.439693, 0.761570, -0.500000),
-        (-0.500000, 0.866025, -0.173648),
-        (0.000000, 1.000000, -0.173648),
-        (-0.439693, 0.761570, -0.500000),
-        (0.000000, 1.000000, -0.173648),
-        (0.000000, 0.879385, -0.500000),
-        (-0.439693, 0.761570, 0.500000),
-        (-0.326352, 0.565258, 0.766044),
-        (0.000000, 0.652704, 0.766044),
-        (-0.439693, 0.761570, 0.500000),
-        (0.000000, 0.652704, 0.766044),
-        (0.000000, 0.879385, 0.500000),
-        (-0.326352, 0.565258, -0.766044),
-        (-0.439693, 0.761570, -0.500000),
-        (0.000000, 0.879385, -0.500000),
-        (-0.326352, 0.565258, -0.766044),
-        (0.000000, 0.879385, -0.500000),
-        (0.000000, 0.652704, -0.766044),
-        (-0.500000, 0.866026, 0.173648),
-        (-0.439693, 0.761570, 0.500000),
-        (0.000000, 0.879385, 0.500000),
-        (-0.500000, 0.866026, 0.173648),
-        (0.000000, 0.879385, 0.500000),
-        (0.000000, 1.000000, 0.173648),
-    ))
-    _normals: Normals = jnp.array((
-        (0.000000, 0.869900, 0.493200),
-        (-0.000000, 0.653800, 0.756700),
-        (0.326900, 0.566200, 0.756700),
-        (0.000000, 0.869900, 0.493200),
-        (0.326900, 0.566200, 0.756700),
-        (0.435000, 0.753400, 0.493200),
-        (-0.000000, 0.653800, -0.756700),
-        (-0.000000, 0.869900, -0.493200),
-        (0.435000, 0.753400, -0.493200),
-        (-0.000000, 0.653800, -0.756700),
-        (0.435000, 0.753400, -0.493200),
-        (0.326900, 0.566200, -0.756700),
-        (-0.000000, 0.985200, 0.171300),
-        (0.000000, 0.869900, 0.493200),
-        (0.435000, 0.753400, 0.493200),
-        (-0.000000, 0.985200, 0.171300),
-        (0.435000, 0.753400, 0.493200),
-        (0.492600, 0.853200, 0.171300),
-        (-0.000000, 0.362500, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (0.181300, 0.313900, 0.932000),
-        (-0.000000, 0.362500, -0.932000),
-        (-0.000000, 0.653800, -0.756700),
-        (0.326900, 0.566200, -0.756700),
-        (-0.000000, 0.362500, -0.932000),
-        (0.326900, 0.566200, -0.756700),
-        (0.181300, 0.313900, -0.932000),
-        (-0.000000, 0.985200, -0.171300),
-        (-0.000000, 0.985200, 0.171300),
-        (0.492600, 0.853200, 0.171300),
-        (-0.000000, 0.985200, -0.171300),
-        (0.492600, 0.853200, 0.171300),
-        (0.492600, 0.853200, -0.171300),
-        (-0.000000, 0.653800, 0.756700),
-        (-0.000000, 0.362500, 0.932000),
-        (0.181300, 0.313900, 0.932000),
-        (-0.000000, 0.653800, 0.756700),
-        (0.181300, 0.313900, 0.932000),
-        (0.326900, 0.566200, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (-0.000000, 0.362500, -0.932000),
-        (0.181300, 0.313900, -0.932000),
-        (-0.000000, 0.869900, -0.493200),
-        (-0.000000, 0.985200, -0.171300),
-        (0.492600, 0.853200, -0.171300),
-        (-0.000000, 0.869900, -0.493200),
-        (0.492600, 0.853200, -0.171300),
-        (0.435000, 0.753400, -0.493200),
-        (0.492600, 0.853200, 0.171300),
-        (0.435000, 0.753400, 0.493200),
-        (0.753400, 0.435000, 0.493200),
-        (0.492600, 0.853200, 0.171300),
-        (0.753400, 0.435000, 0.493200),
-        (0.853200, 0.492600, 0.171300),
-        (0.181300, 0.313900, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (0.313900, 0.181300, 0.932000),
-        (0.181300, 0.313900, -0.932000),
-        (0.326900, 0.566200, -0.756700),
-        (0.566200, 0.326900, -0.756700),
-        (0.181300, 0.313900, -0.932000),
-        (0.566200, 0.326900, -0.756700),
-        (0.313900, 0.181300, -0.932000),
-        (0.492600, 0.853200, -0.171300),
-        (0.492600, 0.853200, 0.171300),
-        (0.853200, 0.492600, 0.171300),
-        (0.492600, 0.853200, -0.171300),
-        (0.853200, 0.492600, 0.171300),
-        (0.853200, 0.492600, -0.171300),
-        (0.326900, 0.566200, 0.756700),
-        (0.181300, 0.313900, 0.932000),
-        (0.313900, 0.181300, 0.932000),
-        (0.326900, 0.566200, 0.756700),
-        (0.313900, 0.181300, 0.932000),
-        (0.566200, 0.326900, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (0.181300, 0.313900, -0.932000),
-        (0.313900, 0.181300, -0.932000),
-        (0.435000, 0.753400, -0.493200),
-        (0.492600, 0.853200, -0.171300),
-        (0.853200, 0.492600, -0.171300),
-        (0.435000, 0.753400, -0.493200),
-        (0.853200, 0.492600, -0.171300),
-        (0.753400, 0.435000, -0.493200),
-        (0.435000, 0.753400, 0.493200),
-        (0.326900, 0.566200, 0.756700),
-        (0.566200, 0.326900, 0.756700),
-        (0.435000, 0.753400, 0.493200),
-        (0.566200, 0.326900, 0.756700),
-        (0.753400, 0.435000, 0.493200),
-        (0.326900, 0.566200, -0.756700),
-        (0.435000, 0.753400, -0.493200),
-        (0.753400, 0.435000, -0.493200),
-        (0.326900, 0.566200, -0.756700),
-        (0.753400, 0.435000, -0.493200),
-        (0.566200, 0.326900, -0.756700),
-        (0.566200, 0.326900, 0.756700),
-        (0.313900, 0.181300, 0.932000),
-        (0.362500, 0.000000, 0.932000),
-        (0.566200, 0.326900, 0.756700),
-        (0.362500, 0.000000, 0.932000),
-        (0.653800, -0.000000, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (0.313900, 0.181300, -0.932000),
-        (0.362500, 0.000000, -0.932000),
-        (0.753400, 0.435000, -0.493200),
-        (0.853200, 0.492600, -0.171300),
-        (0.985200, -0.000000, -0.171300),
-        (0.753400, 0.435000, -0.493200),
-        (0.985200, -0.000000, -0.171300),
-        (0.869900, -0.000000, -0.493200),
-        (0.753400, 0.435000, 0.493200),
-        (0.566200, 0.326900, 0.756700),
-        (0.653800, -0.000000, 0.756700),
-        (0.753400, 0.435000, 0.493200),
-        (0.653800, -0.000000, 0.756700),
-        (0.869900, -0.000000, 0.493200),
-        (0.566200, 0.326900, -0.756700),
-        (0.753400, 0.435000, -0.493200),
-        (0.869900, -0.000000, -0.493200),
-        (0.566200, 0.326900, -0.756700),
-        (0.869900, -0.000000, -0.493200),
-        (0.653800, -0.000000, -0.756700),
-        (0.853200, 0.492600, 0.171300),
-        (0.753400, 0.435000, 0.493200),
-        (0.869900, -0.000000, 0.493200),
-        (0.853200, 0.492600, 0.171300),
-        (0.869900, -0.000000, 0.493200),
-        (0.985200, -0.000000, 0.171300),
-        (0.313900, 0.181300, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (0.362500, 0.000000, 0.932000),
-        (0.313900, 0.181300, -0.932000),
-        (0.566200, 0.326900, -0.756700),
-        (0.653800, -0.000000, -0.756700),
-        (0.313900, 0.181300, -0.932000),
-        (0.653800, -0.000000, -0.756700),
-        (0.362500, 0.000000, -0.932000),
-        (0.853200, 0.492600, -0.171300),
-        (0.853200, 0.492600, 0.171300),
-        (0.985200, -0.000000, 0.171300),
-        (0.853200, 0.492600, -0.171300),
-        (0.985200, -0.000000, 0.171300),
-        (0.985200, -0.000000, -0.171300),
-        (0.653800, -0.000000, -0.756700),
-        (0.869900, -0.000000, -0.493200),
-        (0.753400, -0.435000, -0.493200),
-        (0.653800, -0.000000, -0.756700),
-        (0.753400, -0.435000, -0.493200),
-        (0.566200, -0.326900, -0.756700),
-        (0.985200, -0.000000, 0.171300),
-        (0.869900, -0.000000, 0.493200),
-        (0.753400, -0.435000, 0.493200),
-        (0.985200, -0.000000, 0.171300),
-        (0.753400, -0.435000, 0.493200),
-        (0.853200, -0.492600, 0.171300),
-        (0.362500, 0.000000, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (0.313900, -0.181300, 0.932000),
-        (0.362500, 0.000000, -0.932000),
-        (0.653800, -0.000000, -0.756700),
-        (0.566200, -0.326900, -0.756700),
-        (0.362500, 0.000000, -0.932000),
-        (0.566200, -0.326900, -0.756700),
-        (0.313900, -0.181300, -0.932000),
-        (0.985200, -0.000000, -0.171300),
-        (0.985200, -0.000000, 0.171300),
-        (0.853200, -0.492600, 0.171300),
-        (0.985200, -0.000000, -0.171300),
-        (0.853200, -0.492600, 0.171300),
-        (0.853200, -0.492600, -0.171300),
-        (0.653800, -0.000000, 0.756700),
-        (0.362500, 0.000000, 0.932000),
-        (0.313900, -0.181300, 0.932000),
-        (0.653800, -0.000000, 0.756700),
-        (0.313900, -0.181300, 0.932000),
-        (0.566200, -0.326900, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (0.362500, 0.000000, -0.932000),
-        (0.313900, -0.181300, -0.932000),
-        (0.869900, -0.000000, -0.493200),
-        (0.985200, -0.000000, -0.171300),
-        (0.853200, -0.492600, -0.171300),
-        (0.869900, -0.000000, -0.493200),
-        (0.853200, -0.492600, -0.171300),
-        (0.753400, -0.435000, -0.493200),
-        (0.869900, -0.000000, 0.493200),
-        (0.653800, -0.000000, 0.756700),
-        (0.566200, -0.326900, 0.756700),
-        (0.869900, -0.000000, 0.493200),
-        (0.566200, -0.326900, 0.756700),
-        (0.753400, -0.435000, 0.493200),
-        (0.853200, -0.492600, -0.171300),
-        (0.853200, -0.492600, 0.171300),
-        (0.492600, -0.853200, 0.171300),
-        (0.853200, -0.492600, -0.171300),
-        (0.492600, -0.853200, 0.171300),
-        (0.492600, -0.853200, -0.171300),
-        (0.566200, -0.326900, 0.756700),
-        (0.313900, -0.181300, 0.932000),
-        (0.181300, -0.313900, 0.932000),
-        (0.566200, -0.326900, 0.756700),
-        (0.181300, -0.313900, 0.932000),
-        (0.326900, -0.566200, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (0.313900, -0.181300, -0.932000),
-        (0.181300, -0.313900, -0.932000),
-        (0.753400, -0.435000, -0.493200),
-        (0.853200, -0.492600, -0.171300),
-        (0.492600, -0.853200, -0.171300),
-        (0.753400, -0.435000, -0.493200),
-        (0.492600, -0.853200, -0.171300),
-        (0.435000, -0.753400, -0.493200),
-        (0.753400, -0.435000, 0.493200),
-        (0.566200, -0.326900, 0.756700),
-        (0.326900, -0.566200, 0.756700),
-        (0.753400, -0.435000, 0.493200),
-        (0.326900, -0.566200, 0.756700),
-        (0.435000, -0.753400, 0.493200),
-        (0.566200, -0.326900, -0.756700),
-        (0.753400, -0.435000, -0.493200),
-        (0.435000, -0.753400, -0.493200),
-        (0.566200, -0.326900, -0.756700),
-        (0.435000, -0.753400, -0.493200),
-        (0.326900, -0.566200, -0.756700),
-        (0.853200, -0.492600, 0.171300),
-        (0.753400, -0.435000, 0.493200),
-        (0.435000, -0.753400, 0.493200),
-        (0.853200, -0.492600, 0.171300),
-        (0.435000, -0.753400, 0.493200),
-        (0.492600, -0.853200, 0.171300),
-        (0.313900, -0.181300, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (0.181300, -0.313900, 0.932000),
-        (0.313900, -0.181300, -0.932000),
-        (0.566200, -0.326900, -0.756700),
-        (0.326900, -0.566200, -0.756700),
-        (0.313900, -0.181300, -0.932000),
-        (0.326900, -0.566200, -0.756700),
-        (0.181300, -0.313900, -0.932000),
-        (0.435000, -0.753400, 0.493200),
-        (0.326900, -0.566200, 0.756700),
-        (-0.000000, -0.653800, 0.756700),
-        (0.435000, -0.753400, 0.493200),
-        (-0.000000, -0.653800, 0.756700),
-        (0.000000, -0.869900, 0.493200),
-        (0.326900, -0.566200, -0.756700),
-        (0.435000, -0.753400, -0.493200),
-        (-0.000000, -0.869900, -0.493200),
-        (0.326900, -0.566200, -0.756700),
-        (-0.000000, -0.869900, -0.493200),
-        (0.000000, -0.653800, -0.756700),
-        (0.492600, -0.853200, 0.171300),
-        (0.435000, -0.753400, 0.493200),
-        (0.000000, -0.869900, 0.493200),
-        (0.492600, -0.853200, 0.171300),
-        (0.000000, -0.869900, 0.493200),
-        (0.000000, -0.985200, 0.171300),
-        (0.181300, -0.313900, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (-0.000000, -0.362500, 0.932000),
-        (0.181300, -0.313900, -0.932000),
-        (0.326900, -0.566200, -0.756700),
-        (0.000000, -0.653800, -0.756700),
-        (0.181300, -0.313900, -0.932000),
-        (0.000000, -0.653800, -0.756700),
-        (0.000000, -0.362500, -0.932000),
-        (0.492600, -0.853200, -0.171300),
-        (0.492600, -0.853200, 0.171300),
-        (0.000000, -0.985200, 0.171300),
-        (0.492600, -0.853200, -0.171300),
-        (0.000000, -0.985200, 0.171300),
-        (-0.000000, -0.985200, -0.171300),
-        (0.326900, -0.566200, 0.756700),
-        (0.181300, -0.313900, 0.932000),
-        (-0.000000, -0.362500, 0.932000),
-        (0.326900, -0.566200, 0.756700),
-        (-0.000000, -0.362500, 0.932000),
-        (-0.000000, -0.653800, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (0.181300, -0.313900, -0.932000),
-        (0.000000, -0.362500, -0.932000),
-        (0.435000, -0.753400, -0.493200),
-        (0.492600, -0.853200, -0.171300),
-        (-0.000000, -0.985200, -0.171300),
-        (0.435000, -0.753400, -0.493200),
-        (-0.000000, -0.985200, -0.171300),
-        (-0.000000, -0.869900, -0.493200),
-        (-0.000000, -0.362500, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (-0.181300, -0.313900, 0.932000),
-        (0.000000, -0.362500, -0.932000),
-        (0.000000, -0.653800, -0.756700),
-        (-0.326900, -0.566200, -0.756700),
-        (0.000000, -0.362500, -0.932000),
-        (-0.326900, -0.566200, -0.756700),
-        (-0.181300, -0.313900, -0.932000),
-        (-0.000000, -0.985200, -0.171300),
-        (0.000000, -0.985200, 0.171300),
-        (-0.492600, -0.853200, 0.171300),
-        (-0.000000, -0.985200, -0.171300),
-        (-0.492600, -0.853200, 0.171300),
-        (-0.492600, -0.853200, -0.171300),
-        (-0.000000, -0.653800, 0.756700),
-        (-0.000000, -0.362500, 0.932000),
-        (-0.181300, -0.313900, 0.932000),
-        (-0.000000, -0.653800, 0.756700),
-        (-0.181300, -0.313900, 0.932000),
-        (-0.326900, -0.566200, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (0.000000, -0.362500, -0.932000),
-        (-0.181300, -0.313900, -0.932000),
-        (-0.000000, -0.869900, -0.493200),
-        (-0.000000, -0.985200, -0.171300),
-        (-0.492600, -0.853200, -0.171300),
-        (-0.000000, -0.869900, -0.493200),
-        (-0.492600, -0.853200, -0.171300),
-        (-0.435000, -0.753400, -0.493200),
-        (0.000000, -0.869900, 0.493200),
-        (-0.000000, -0.653800, 0.756700),
-        (-0.326900, -0.566200, 0.756700),
-        (0.000000, -0.869900, 0.493200),
-        (-0.326900, -0.566200, 0.756700),
-        (-0.435000, -0.753400, 0.493200),
-        (0.000000, -0.653800, -0.756700),
-        (-0.000000, -0.869900, -0.493200),
-        (-0.435000, -0.753400, -0.493200),
-        (0.000000, -0.653800, -0.756700),
-        (-0.435000, -0.753400, -0.493200),
-        (-0.326900, -0.566200, -0.756700),
-        (0.000000, -0.985200, 0.171300),
-        (0.000000, -0.869900, 0.493200),
-        (-0.435000, -0.753400, 0.493200),
-        (0.000000, -0.985200, 0.171300),
-        (-0.435000, -0.753400, 0.493200),
-        (-0.492600, -0.853200, 0.171300),
-        (0.000000, -0.000000, -1.000000),
-        (-0.181300, -0.313900, -0.932000),
-        (-0.313900, -0.181300, -0.932000),
-        (-0.435000, -0.753400, -0.493200),
-        (-0.492600, -0.853200, -0.171300),
-        (-0.853200, -0.492600, -0.171300),
-        (-0.435000, -0.753400, -0.493200),
-        (-0.853200, -0.492600, -0.171300),
-        (-0.753400, -0.435000, -0.493200),
-        (-0.435000, -0.753400, 0.493200),
-        (-0.326900, -0.566200, 0.756700),
-        (-0.566200, -0.326900, 0.756700),
-        (-0.435000, -0.753400, 0.493200),
-        (-0.566200, -0.326900, 0.756700),
-        (-0.753400, -0.435000, 0.493200),
-        (-0.326900, -0.566200, -0.756700),
-        (-0.435000, -0.753400, -0.493200),
-        (-0.753400, -0.435000, -0.493200),
-        (-0.326900, -0.566200, -0.756700),
-        (-0.753400, -0.435000, -0.493200),
-        (-0.566200, -0.326900, -0.756700),
-        (-0.492600, -0.853200, 0.171300),
-        (-0.435000, -0.753400, 0.493200),
-        (-0.753400, -0.435000, 0.493200),
-        (-0.492600, -0.853200, 0.171300),
-        (-0.753400, -0.435000, 0.493200),
-        (-0.853200, -0.492600, 0.171300),
-        (-0.181300, -0.313900, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (-0.313900, -0.181300, 0.932000),
-        (-0.181300, -0.313900, -0.932000),
-        (-0.326900, -0.566200, -0.756700),
-        (-0.566200, -0.326900, -0.756700),
-        (-0.181300, -0.313900, -0.932000),
-        (-0.566200, -0.326900, -0.756700),
-        (-0.313900, -0.181300, -0.932000),
-        (-0.492600, -0.853200, -0.171300),
-        (-0.492600, -0.853200, 0.171300),
-        (-0.853200, -0.492600, 0.171300),
-        (-0.492600, -0.853200, -0.171300),
-        (-0.853200, -0.492600, 0.171300),
-        (-0.853200, -0.492600, -0.171300),
-        (-0.326900, -0.566200, 0.756700),
-        (-0.181300, -0.313900, 0.932000),
-        (-0.313900, -0.181300, 0.932000),
-        (-0.326900, -0.566200, 0.756700),
-        (-0.313900, -0.181300, 0.932000),
-        (-0.566200, -0.326900, 0.756700),
-        (-0.566200, -0.326900, -0.756700),
-        (-0.753400, -0.435000, -0.493200),
-        (-0.869900, -0.000000, -0.493200),
-        (-0.566200, -0.326900, -0.756700),
-        (-0.869900, -0.000000, -0.493200),
-        (-0.653800, -0.000000, -0.756700),
-        (-0.853200, -0.492600, 0.171300),
-        (-0.753400, -0.435000, 0.493200),
-        (-0.869900, -0.000000, 0.493200),
-        (-0.853200, -0.492600, 0.171300),
-        (-0.869900, -0.000000, 0.493200),
-        (-0.985200, -0.000000, 0.171300),
-        (-0.313900, -0.181300, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (-0.362500, 0.000000, 0.932000),
-        (-0.313900, -0.181300, -0.932000),
-        (-0.566200, -0.326900, -0.756700),
-        (-0.653800, -0.000000, -0.756700),
-        (-0.313900, -0.181300, -0.932000),
-        (-0.653800, -0.000000, -0.756700),
-        (-0.362500, 0.000000, -0.932000),
-        (-0.853200, -0.492600, -0.171300),
-        (-0.853200, -0.492600, 0.171300),
-        (-0.985200, -0.000000, 0.171300),
-        (-0.853200, -0.492600, -0.171300),
-        (-0.985200, -0.000000, 0.171300),
-        (-0.985200, -0.000000, -0.171300),
-        (-0.566200, -0.326900, 0.756700),
-        (-0.313900, -0.181300, 0.932000),
-        (-0.362500, 0.000000, 0.932000),
-        (-0.566200, -0.326900, 0.756700),
-        (-0.362500, 0.000000, 0.932000),
-        (-0.653800, -0.000000, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (-0.313900, -0.181300, -0.932000),
-        (-0.362500, 0.000000, -0.932000),
-        (-0.753400, -0.435000, -0.493200),
-        (-0.853200, -0.492600, -0.171300),
-        (-0.985200, -0.000000, -0.171300),
-        (-0.753400, -0.435000, -0.493200),
-        (-0.985200, -0.000000, -0.171300),
-        (-0.869900, -0.000000, -0.493200),
-        (-0.753400, -0.435000, 0.493200),
-        (-0.566200, -0.326900, 0.756700),
-        (-0.653800, -0.000000, 0.756700),
-        (-0.753400, -0.435000, 0.493200),
-        (-0.653800, -0.000000, 0.756700),
-        (-0.869900, -0.000000, 0.493200),
-        (-0.985200, -0.000000, -0.171300),
-        (-0.985200, -0.000000, 0.171300),
-        (-0.853200, 0.492600, 0.171300),
-        (-0.985200, -0.000000, -0.171300),
-        (-0.853200, 0.492600, 0.171300),
-        (-0.853200, 0.492600, -0.171300),
-        (-0.653800, -0.000000, 0.756700),
-        (-0.362500, 0.000000, 0.932000),
-        (-0.313900, 0.181300, 0.932000),
-        (-0.653800, -0.000000, 0.756700),
-        (-0.313900, 0.181300, 0.932000),
-        (-0.566200, 0.326900, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (-0.362500, 0.000000, -0.932000),
-        (-0.313900, 0.181300, -0.932000),
-        (-0.869900, -0.000000, -0.493200),
-        (-0.985200, -0.000000, -0.171300),
-        (-0.853200, 0.492600, -0.171300),
-        (-0.869900, -0.000000, -0.493200),
-        (-0.853200, 0.492600, -0.171300),
-        (-0.753400, 0.435000, -0.493200),
-        (-0.869900, -0.000000, 0.493200),
-        (-0.653800, -0.000000, 0.756700),
-        (-0.566200, 0.326900, 0.756700),
-        (-0.869900, -0.000000, 0.493200),
-        (-0.566200, 0.326900, 0.756700),
-        (-0.753400, 0.435000, 0.493200),
-        (-0.653800, -0.000000, -0.756700),
-        (-0.869900, -0.000000, -0.493200),
-        (-0.753400, 0.435000, -0.493200),
-        (-0.653800, -0.000000, -0.756700),
-        (-0.753400, 0.435000, -0.493200),
-        (-0.566200, 0.326900, -0.756700),
-        (-0.985200, -0.000000, 0.171300),
-        (-0.869900, -0.000000, 0.493200),
-        (-0.753400, 0.435000, 0.493200),
-        (-0.985200, -0.000000, 0.171300),
-        (-0.753400, 0.435000, 0.493200),
-        (-0.853200, 0.492600, 0.171300),
-        (-0.362500, 0.000000, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (-0.313900, 0.181300, 0.932000),
-        (-0.362500, 0.000000, -0.932000),
-        (-0.653800, -0.000000, -0.756700),
-        (-0.566200, 0.326900, -0.756700),
-        (-0.362500, 0.000000, -0.932000),
-        (-0.566200, 0.326900, -0.756700),
-        (-0.313900, 0.181300, -0.932000),
-        (-0.753400, 0.435000, 0.493200),
-        (-0.566200, 0.326900, 0.756700),
-        (-0.326900, 0.566200, 0.756700),
-        (-0.753400, 0.435000, 0.493200),
-        (-0.326900, 0.566200, 0.756700),
-        (-0.435000, 0.753400, 0.493200),
-        (-0.566200, 0.326900, -0.756700),
-        (-0.753400, 0.435000, -0.493200),
-        (-0.435000, 0.753400, -0.493200),
-        (-0.566200, 0.326900, -0.756700),
-        (-0.435000, 0.753400, -0.493200),
-        (-0.326900, 0.566200, -0.756700),
-        (-0.853200, 0.492600, 0.171300),
-        (-0.753400, 0.435000, 0.493200),
-        (-0.435000, 0.753400, 0.493200),
-        (-0.853200, 0.492600, 0.171300),
-        (-0.435000, 0.753400, 0.493200),
-        (-0.492600, 0.853200, 0.171300),
-        (-0.313900, 0.181300, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (-0.181300, 0.313900, 0.932000),
-        (-0.313900, 0.181300, -0.932000),
-        (-0.566200, 0.326900, -0.756700),
-        (-0.326900, 0.566200, -0.756700),
-        (-0.313900, 0.181300, -0.932000),
-        (-0.326900, 0.566200, -0.756700),
-        (-0.181300, 0.313900, -0.932000),
-        (-0.853200, 0.492600, -0.171300),
-        (-0.853200, 0.492600, 0.171300),
-        (-0.492600, 0.853200, 0.171300),
-        (-0.853200, 0.492600, -0.171300),
-        (-0.492600, 0.853200, 0.171300),
-        (-0.492600, 0.853200, -0.171300),
-        (-0.566200, 0.326900, 0.756700),
-        (-0.313900, 0.181300, 0.932000),
-        (-0.181300, 0.313900, 0.932000),
-        (-0.566200, 0.326900, 0.756700),
-        (-0.181300, 0.313900, 0.932000),
-        (-0.326900, 0.566200, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (-0.313900, 0.181300, -0.932000),
-        (-0.181300, 0.313900, -0.932000),
-        (-0.753400, 0.435000, -0.493200),
-        (-0.853200, 0.492600, -0.171300),
-        (-0.492600, 0.853200, -0.171300),
-        (-0.753400, 0.435000, -0.493200),
-        (-0.492600, 0.853200, -0.171300),
-        (-0.435000, 0.753400, -0.493200),
-        (-0.181300, 0.313900, 0.932000),
-        (-0.000000, -0.000000, 1.000000),
-        (-0.000000, 0.362500, 0.932000),
-        (-0.181300, 0.313900, -0.932000),
-        (-0.326900, 0.566200, -0.756700),
-        (-0.000000, 0.653800, -0.756700),
-        (-0.181300, 0.313900, -0.932000),
-        (-0.000000, 0.653800, -0.756700),
-        (-0.000000, 0.362500, -0.932000),
-        (-0.492600, 0.853200, -0.171300),
-        (-0.492600, 0.853200, 0.171300),
-        (-0.000000, 0.985200, 0.171300),
-        (-0.492600, 0.853200, -0.171300),
-        (-0.000000, 0.985200, 0.171300),
-        (-0.000000, 0.985200, -0.171300),
-        (-0.326900, 0.566200, 0.756700),
-        (-0.181300, 0.313900, 0.932000),
-        (-0.000000, 0.362500, 0.932000),
-        (-0.326900, 0.566200, 0.756700),
-        (-0.000000, 0.362500, 0.932000),
-        (-0.000000, 0.653800, 0.756700),
-        (0.000000, -0.000000, -1.000000),
-        (-0.181300, 0.313900, -0.932000),
-        (-0.000000, 0.362500, -0.932000),
-        (-0.435000, 0.753400, -0.493200),
-        (-0.492600, 0.853200, -0.171300),
-        (-0.000000, 0.985200, -0.171300),
-        (-0.435000, 0.753400, -0.493200),
-        (-0.000000, 0.985200, -0.171300),
-        (-0.000000, 0.869900, -0.493200),
-        (-0.435000, 0.753400, 0.493200),
-        (-0.326900, 0.566200, 0.756700),
-        (-0.000000, 0.653800, 0.756700),
-        (-0.435000, 0.753400, 0.493200),
-        (-0.000000, 0.653800, 0.756700),
-        (0.000000, 0.869900, 0.493200),
-        (-0.326900, 0.566200, -0.756700),
-        (-0.435000, 0.753400, -0.493200),
-        (-0.000000, 0.869900, -0.493200),
-        (-0.326900, 0.566200, -0.756700),
-        (-0.000000, 0.869900, -0.493200),
-        (-0.000000, 0.653800, -0.756700),
-        (-0.492600, 0.853200, 0.171300),
-        (-0.435000, 0.753400, 0.493200),
-        (0.000000, 0.869900, 0.493200),
-        (-0.492600, 0.853200, 0.171300),
-        (0.000000, 0.869900, 0.493200),
-        (-0.000000, 0.985200, 0.171300),
-    ))
-    _uvs: UVCoordinates = jnp.array((
-        (0.500144, 0.744995),
-        (0.500144, 0.876330),
-        (0.661251, 0.876330),
-        (0.500144, 0.744995),
-        (0.661251, 0.876330),
-        (0.717203, 0.744995),
-        (0.500144, 0.119997),
-        (0.500144, 0.251333),
-        (0.717203, 0.251333),
-        (0.500144, 0.119997),
-        (0.717203, 0.251333),
-        (0.661251, 0.119997),
-        (0.500144, 0.583887),
-        (0.500144, 0.744995),
-        (0.717203, 0.744995),
-        (0.500144, 0.583887),
-        (0.717203, 0.744995),
-        (0.746974, 0.583887),
-        (0.500144, 0.962054),
-        (0.500144, 0.991825),
-        (0.585867, 0.962054),
-        (0.500144, 0.034273),
-        (0.500144, 0.119997),
-        (0.661251, 0.119997),
-        (0.500144, 0.034273),
-        (0.661251, 0.119997),
-        (0.585867, 0.034273),
-        (0.500144, 0.412440),
-        (0.500144, 0.583887),
-        (0.746974, 0.583887),
-        (0.500144, 0.412440),
-        (0.746974, 0.583887),
-        (0.746974, 0.412440),
-        (0.500144, 0.876330),
-        (0.500144, 0.962054),
-        (0.585867, 0.962054),
-        (0.500144, 0.876330),
-        (0.585867, 0.962054),
-        (0.661251, 0.876330),
-        (0.500144, 0.004502),
-        (0.500144, 0.034273),
-        (0.585867, 0.034273),
-        (0.500144, 0.251333),
-        (0.500144, 0.412440),
-        (0.746974, 0.412440),
-        (0.500144, 0.251333),
-        (0.746974, 0.412440),
-        (0.717203, 0.251333),
-        (0.746974, 0.583887),
-        (0.717203, 0.744995),
-        (0.876102, 0.744995),
-        (0.746974, 0.583887),
-        (0.876102, 0.744995),
-        (0.927667, 0.583887),
-        (0.585867, 0.962054),
-        (0.500144, 0.991825),
-        (0.648621, 0.962054),
-        (0.585867, 0.034273),
-        (0.661251, 0.119997),
-        (0.779190, 0.119997),
-        (0.585867, 0.034273),
-        (0.779190, 0.119997),
-        (0.648621, 0.034274),
-        (0.746974, 0.412440),
-        (0.746974, 0.583887),
-        (0.927667, 0.583887),
-        (0.746974, 0.412440),
-        (0.927667, 0.583887),
-        (0.927667, 0.412440),
-        (0.661251, 0.876330),
-        (0.585867, 0.962054),
-        (0.648621, 0.962054),
-        (0.661251, 0.876330),
-        (0.648621, 0.962054),
-        (0.779190, 0.876330),
-        (0.500144, 0.004502),
-        (0.585867, 0.034273),
-        (0.648621, 0.034274),
-        (0.717203, 0.251333),
-        (0.746974, 0.412440),
-        (0.927667, 0.412440),
-        (0.717203, 0.251333),
-        (0.927667, 0.412440),
-        (0.876102, 0.251333),
-        (0.717203, 0.744995),
-        (0.661251, 0.876330),
-        (0.779190, 0.876330),
-        (0.717203, 0.744995),
-        (0.779190, 0.876330),
-        (0.876102, 0.744995),
-        (0.661251, 0.119997),
-        (0.717203, 0.251333),
-        (0.876102, 0.251333),
-        (0.661251, 0.119997),
-        (0.876102, 0.251333),
-        (0.779190, 0.119997),
-        (0.779190, 0.876330),
-        (0.648621, 0.962054),
-        (0.671590, 0.962054),
-        (0.779190, 0.876330),
-        (0.671590, 0.962054),
-        (0.822359, 0.876330),
-        (0.500144, 0.004502),
-        (0.648621, 0.034274),
-        (0.671590, 0.034274),
-        (0.876102, 0.251333),
-        (0.927667, 0.412440),
-        (0.993805, 0.412440),
-        (0.876102, 0.251333),
-        (0.993805, 0.412440),
-        (0.934262, 0.251333),
-        (0.876102, 0.744995),
-        (0.779190, 0.876330),
-        (0.822359, 0.876330),
-        (0.876102, 0.744995),
-        (0.822359, 0.876330),
-        (0.934262, 0.744995),
-        (0.779190, 0.119997),
-        (0.876102, 0.251333),
-        (0.934262, 0.251333),
-        (0.779190, 0.119997),
-        (0.934262, 0.251333),
-        (0.822359, 0.119997),
-        (0.927667, 0.583887),
-        (0.876102, 0.744995),
-        (0.934262, 0.744995),
-        (0.927667, 0.583887),
-        (0.934262, 0.744995),
-        (0.993805, 0.583887),
-        (0.648621, 0.962054),
-        (0.500144, 0.991825),
-        (0.671590, 0.962054),
-        (0.648621, 0.034274),
-        (0.779190, 0.119997),
-        (0.822359, 0.119997),
-        (0.648621, 0.034274),
-        (0.822359, 0.119997),
-        (0.671590, 0.034274),
-        (0.927667, 0.412440),
-        (0.927667, 0.583887),
-        (0.993805, 0.583887),
-        (0.927667, 0.412440),
-        (0.993805, 0.583887),
-        (0.993805, 0.412440),
-        (0.822359, 0.119997),
-        (0.934262, 0.251333),
-        (0.876102, 0.251333),
-        (0.822359, 0.119997),
-        (0.876102, 0.251333),
-        (0.779190, 0.119997),
-        (0.993805, 0.583887),
-        (0.934262, 0.744995),
-        (0.876102, 0.744995),
-        (0.993805, 0.583887),
-        (0.876102, 0.744995),
-        (0.927667, 0.583887),
-        (0.671590, 0.962054),
-        (0.500144, 0.991825),
-        (0.648621, 0.962054),
-        (0.671590, 0.034274),
-        (0.822359, 0.119997),
-        (0.779190, 0.119997),
-        (0.671590, 0.034274),
-        (0.779190, 0.119997),
-        (0.648621, 0.034274),
-        (0.993805, 0.412440),
-        (0.993805, 0.583887),
-        (0.927667, 0.583887),
-        (0.993805, 0.412440),
-        (0.927667, 0.583887),
-        (0.927667, 0.412440),
-        (0.822359, 0.876330),
-        (0.671590, 0.962054),
-        (0.648621, 0.962054),
-        (0.822359, 0.876330),
-        (0.648621, 0.962054),
-        (0.779190, 0.876330),
-        (0.500144, 0.004502),
-        (0.671590, 0.034274),
-        (0.648621, 0.034274),
-        (0.934262, 0.251333),
-        (0.993805, 0.412440),
-        (0.927667, 0.412440),
-        (0.934262, 0.251333),
-        (0.927667, 0.412440),
-        (0.876102, 0.251333),
-        (0.934262, 0.744995),
-        (0.822359, 0.876330),
-        (0.779190, 0.876330),
-        (0.934262, 0.744995),
-        (0.779190, 0.876330),
-        (0.876102, 0.744995),
-        (0.927667, 0.412440),
-        (0.927667, 0.583887),
-        (0.746974, 0.583887),
-        (0.927667, 0.412440),
-        (0.746974, 0.583887),
-        (0.746974, 0.412441),
-        (0.779190, 0.876330),
-        (0.648621, 0.962054),
-        (0.585867, 0.962054),
-        (0.779190, 0.876330),
-        (0.585867, 0.962054),
-        (0.661251, 0.876330),
-        (0.500144, 0.004502),
-        (0.648621, 0.034274),
-        (0.585867, 0.034274),
-        (0.876102, 0.251333),
-        (0.927667, 0.412440),
-        (0.746974, 0.412441),
-        (0.876102, 0.251333),
-        (0.746974, 0.412441),
-        (0.717203, 0.251333),
-        (0.876102, 0.744995),
-        (0.779190, 0.876330),
-        (0.661251, 0.876330),
-        (0.876102, 0.744995),
-        (0.661251, 0.876330),
-        (0.717203, 0.744995),
-        (0.779190, 0.119997),
-        (0.876102, 0.251333),
-        (0.717203, 0.251333),
-        (0.779190, 0.119997),
-        (0.717203, 0.251333),
-        (0.661251, 0.119997),
-        (0.927667, 0.583887),
-        (0.876102, 0.744995),
-        (0.717203, 0.744995),
-        (0.927667, 0.583887),
-        (0.717203, 0.744995),
-        (0.746974, 0.583887),
-        (0.648621, 0.962054),
-        (0.500144, 0.991825),
-        (0.585867, 0.962054),
-        (0.648621, 0.034274),
-        (0.779190, 0.119997),
-        (0.661251, 0.119997),
-        (0.648621, 0.034274),
-        (0.661251, 0.119997),
-        (0.585867, 0.034274),
-        (0.717203, 0.744995),
-        (0.661251, 0.876330),
-        (0.500144, 0.876330),
-        (0.717203, 0.744995),
-        (0.500144, 0.876330),
-        (0.500144, 0.744995),
-        (0.661251, 0.119997),
-        (0.717203, 0.251333),
-        (0.500144, 0.251333),
-        (0.661251, 0.119997),
-        (0.500144, 0.251333),
-        (0.500144, 0.119997),
-        (0.746974, 0.583887),
-        (0.717203, 0.744995),
-        (0.500144, 0.744995),
-        (0.746974, 0.583887),
-        (0.500144, 0.744995),
-        (0.500144, 0.583887),
-        (0.585867, 0.962054),
-        (0.500144, 0.991825),
-        (0.500144, 0.962054),
-        (0.585867, 0.034274),
-        (0.661251, 0.119997),
-        (0.500144, 0.119997),
-        (0.585867, 0.034274),
-        (0.500144, 0.119997),
-        (0.500144, 0.034274),
-        (0.746974, 0.412441),
-        (0.746974, 0.583887),
-        (0.500144, 0.583887),
-        (0.746974, 0.412441),
-        (0.500144, 0.583887),
-        (0.500144, 0.412441),
-        (0.661251, 0.876330),
-        (0.585867, 0.962054),
-        (0.500144, 0.962054),
-        (0.661251, 0.876330),
-        (0.500144, 0.962054),
-        (0.500144, 0.876330),
-        (0.500144, 0.004502),
-        (0.585867, 0.034274),
-        (0.500144, 0.034274),
-        (0.717203, 0.251333),
-        (0.746974, 0.412441),
-        (0.500144, 0.412441),
-        (0.717203, 0.251333),
-        (0.500144, 0.412441),
-        (0.500144, 0.251333),
-        (0.500144, 0.962054),
-        (0.500144, 0.991825),
-        (0.414420, 0.962054),
-        (0.500144, 0.034274),
-        (0.500144, 0.119997),
-        (0.339036, 0.119997),
-        (0.500144, 0.034274),
-        (0.339036, 0.119997),
-        (0.414420, 0.034274),
-        (0.500144, 0.412441),
-        (0.500144, 0.583887),
-        (0.253313, 0.583887),
-        (0.500144, 0.412441),
-        (0.253313, 0.583887),
-        (0.253313, 0.412441),
-        (0.500144, 0.876330),
-        (0.500144, 0.962054),
-        (0.414420, 0.962054),
-        (0.500144, 0.876330),
-        (0.414420, 0.962054),
-        (0.339036, 0.876330),
-        (0.500144, 0.004502),
-        (0.500144, 0.034274),
-        (0.414420, 0.034274),
-        (0.500144, 0.251333),
-        (0.500144, 0.412441),
-        (0.253313, 0.412441),
-        (0.500144, 0.251333),
-        (0.253313, 0.412441),
-        (0.283084, 0.251333),
-        (0.500144, 0.744995),
-        (0.500144, 0.876330),
-        (0.339036, 0.876330),
-        (0.500144, 0.744995),
-        (0.339036, 0.876330),
-        (0.283084, 0.744995),
-        (0.500144, 0.119997),
-        (0.500144, 0.251333),
-        (0.283084, 0.251333),
-        (0.500144, 0.119997),
-        (0.283084, 0.251333),
-        (0.339036, 0.119997),
-        (0.500144, 0.583887),
-        (0.500144, 0.744995),
-        (0.283084, 0.744995),
-        (0.500144, 0.583887),
-        (0.283084, 0.744995),
-        (0.253313, 0.583887),
-        (0.500144, 0.004502),
-        (0.414420, 0.034274),
-        (0.351667, 0.034274),
-        (0.283084, 0.251333),
-        (0.253313, 0.412441),
-        (0.072621, 0.412440),
-        (0.283084, 0.251333),
-        (0.072621, 0.412440),
-        (0.124186, 0.251333),
-        (0.283084, 0.744995),
-        (0.339036, 0.876330),
-        (0.221098, 0.876330),
-        (0.283084, 0.744995),
-        (0.221098, 0.876330),
-        (0.124186, 0.744995),
-        (0.339036, 0.119997),
-        (0.283084, 0.251333),
-        (0.124186, 0.251333),
-        (0.339036, 0.119997),
-        (0.124186, 0.251333),
-        (0.221098, 0.119997),
-        (0.253313, 0.583887),
-        (0.283084, 0.744995),
-        (0.124186, 0.744995),
-        (0.253313, 0.583887),
-        (0.124186, 0.744995),
-        (0.072621, 0.583887),
-        (0.414420, 0.962054),
-        (0.500144, 0.991825),
-        (0.351667, 0.962054),
-        (0.414420, 0.034274),
-        (0.339036, 0.119997),
-        (0.221098, 0.119997),
-        (0.414420, 0.034274),
-        (0.221098, 0.119997),
-        (0.351667, 0.034274),
-        (0.253313, 0.412441),
-        (0.253313, 0.583887),
-        (0.072621, 0.583887),
-        (0.253313, 0.412441),
-        (0.072621, 0.583887),
-        (0.072621, 0.412440),
-        (0.339036, 0.876330),
-        (0.414420, 0.962054),
-        (0.351667, 0.962054),
-        (0.339036, 0.876330),
-        (0.351667, 0.962054),
-        (0.221098, 0.876330),
-        (0.221098, 0.119997),
-        (0.124186, 0.251333),
-        (0.066025, 0.251333),
-        (0.221098, 0.119997),
-        (0.066025, 0.251333),
-        (0.177929, 0.119997),
-        (0.072621, 0.583887),
-        (0.124186, 0.744995),
-        (0.066025, 0.744995),
-        (0.072621, 0.583887),
-        (0.066025, 0.744995),
-        (0.006482, 0.583887),
-        (0.351667, 0.962054),
-        (0.500144, 0.991825),
-        (0.328697, 0.962054),
-        (0.351667, 0.034274),
-        (0.221098, 0.119997),
-        (0.177929, 0.119997),
-        (0.351667, 0.034274),
-        (0.177929, 0.119997),
-        (0.328697, 0.034274),
-        (0.072621, 0.412440),
-        (0.072621, 0.583887),
-        (0.006482, 0.583887),
-        (0.072621, 0.412440),
-        (0.006482, 0.583887),
-        (0.006482, 0.412440),
-        (0.221098, 0.876330),
-        (0.351667, 0.962054),
-        (0.328697, 0.962054),
-        (0.221098, 0.876330),
-        (0.328697, 0.962054),
-        (0.177929, 0.876330),
-        (0.500144, 0.004502),
-        (0.351667, 0.034274),
-        (0.328697, 0.034274),
-        (0.124186, 0.251333),
-        (0.072621, 0.412440),
-        (0.006482, 0.412440),
-        (0.124186, 0.251333),
-        (0.006482, 0.412440),
-        (0.066025, 0.251333),
-        (0.124186, 0.744995),
-        (0.221098, 0.876330),
-        (0.177929, 0.876330),
-        (0.124186, 0.744995),
-        (0.177929, 0.876330),
-        (0.066025, 0.744995),
-        (0.006482, 0.412440),
-        (0.006482, 0.583887),
-        (0.072621, 0.583887),
-        (0.006482, 0.412440),
-        (0.072621, 0.583887),
-        (0.072621, 0.412440),
-        (0.177929, 0.876330),
-        (0.328697, 0.962054),
-        (0.351667, 0.962054),
-        (0.177929, 0.876330),
-        (0.351667, 0.962054),
-        (0.221098, 0.876330),
-        (0.500144, 0.004502),
-        (0.328697, 0.034274),
-        (0.351667, 0.034274),
-        (0.066025, 0.251333),
-        (0.006482, 0.412440),
-        (0.072621, 0.412440),
-        (0.066025, 0.251333),
-        (0.072621, 0.412440),
-        (0.124186, 0.251333),
-        (0.066025, 0.744995),
-        (0.177929, 0.876330),
-        (0.221098, 0.876330),
-        (0.066025, 0.744995),
-        (0.221098, 0.876330),
-        (0.124186, 0.744995),
-        (0.177929, 0.119997),
-        (0.066025, 0.251333),
-        (0.124186, 0.251333),
-        (0.177929, 0.119997),
-        (0.124186, 0.251333),
-        (0.221098, 0.119997),
-        (0.006482, 0.583887),
-        (0.066025, 0.744995),
-        (0.124186, 0.744995),
-        (0.006482, 0.583887),
-        (0.124186, 0.744995),
-        (0.072621, 0.583887),
-        (0.328697, 0.962054),
-        (0.500144, 0.991825),
-        (0.351667, 0.962054),
-        (0.328697, 0.034274),
-        (0.177929, 0.119997),
-        (0.221098, 0.119997),
-        (0.328697, 0.034274),
-        (0.221098, 0.119997),
-        (0.351667, 0.034274),
-        (0.124186, 0.744995),
-        (0.221098, 0.876330),
-        (0.339036, 0.876330),
-        (0.124186, 0.744995),
-        (0.339036, 0.876330),
-        (0.283084, 0.744995),
-        (0.221098, 0.119997),
-        (0.124186, 0.251333),
-        (0.283084, 0.251333),
-        (0.221098, 0.119997),
-        (0.283084, 0.251333),
-        (0.339036, 0.119997),
-        (0.072621, 0.583887),
-        (0.124186, 0.744995),
-        (0.283084, 0.744995),
-        (0.072621, 0.583887),
-        (0.283084, 0.744995),
-        (0.253313, 0.583887),
-        (0.351667, 0.962054),
-        (0.500144, 0.991825),
-        (0.414420, 0.962054),
-        (0.351667, 0.034274),
-        (0.221098, 0.119997),
-        (0.339036, 0.119997),
-        (0.351667, 0.034274),
-        (0.339036, 0.119997),
-        (0.414420, 0.034273),
-        (0.072621, 0.412440),
-        (0.072621, 0.583887),
-        (0.253313, 0.583887),
-        (0.072621, 0.412440),
-        (0.253313, 0.583887),
-        (0.253313, 0.412440),
-        (0.221098, 0.876330),
-        (0.351667, 0.962054),
-        (0.414420, 0.962054),
-        (0.221098, 0.876330),
-        (0.414420, 0.962054),
-        (0.339036, 0.876330),
-        (0.500144, 0.004502),
-        (0.351667, 0.034274),
-        (0.414420, 0.034273),
-        (0.124186, 0.251333),
-        (0.072621, 0.412440),
-        (0.253313, 0.412440),
-        (0.124186, 0.251333),
-        (0.253313, 0.412440),
-        (0.283084, 0.251333),
-        (0.414420, 0.962054),
-        (0.500144, 0.991825),
-        (0.500144, 0.962054),
-        (0.414420, 0.034273),
-        (0.339036, 0.119997),
-        (0.500144, 0.119997),
-        (0.414420, 0.034273),
-        (0.500144, 0.119997),
-        (0.500144, 0.034273),
-        (0.253313, 0.412440),
-        (0.253313, 0.583887),
-        (0.500144, 0.583887),
-        (0.253313, 0.412440),
-        (0.500144, 0.583887),
-        (0.500144, 0.412440),
-        (0.339036, 0.876330),
-        (0.414420, 0.962054),
-        (0.500144, 0.962054),
-        (0.339036, 0.876330),
-        (0.500144, 0.962054),
-        (0.500144, 0.876330),
-        (0.500144, 0.004502),
-        (0.414420, 0.034273),
-        (0.500144, 0.034273),
-        (0.283084, 0.251333),
-        (0.253313, 0.412440),
-        (0.500144, 0.412440),
-        (0.283084, 0.251333),
-        (0.500144, 0.412440),
-        (0.500144, 0.251333),
-        (0.283084, 0.744995),
-        (0.339036, 0.876330),
-        (0.500144, 0.876330),
-        (0.283084, 0.744995),
-        (0.500144, 0.876330),
-        (0.500144, 0.744995),
-        (0.339036, 0.119997),
-        (0.283084, 0.251333),
-        (0.500144, 0.251333),
-        (0.339036, 0.119997),
-        (0.500144, 0.251333),
-        (0.500144, 0.119997),
-        (0.253313, 0.583887),
-        (0.283084, 0.744995),
-        (0.500144, 0.744995),
-        (0.253313, 0.583887),
-        (0.500144, 0.744995),
-        (0.500144, 0.583887),
-    ))
-    _faces: FaceIndices = jnp.array((
-        (0, 1, 2),
-        (3, 4, 5),
-        (6, 7, 8),
-        (9, 10, 11),
-        (12, 13, 14),
-        (15, 16, 17),
-        (18, 19, 20),
-        (21, 22, 23),
-        (24, 25, 26),
-        (27, 28, 29),
-        (30, 31, 32),
-        (33, 34, 35),
-        (36, 37, 38),
-        (39, 40, 41),
-        (42, 43, 44),
-        (45, 46, 47),
-        (48, 49, 50),
-        (51, 52, 53),
-        (54, 55, 56),
-        (57, 58, 59),
-        (60, 61, 62),
-        (63, 64, 65),
-        (66, 67, 68),
-        (69, 70, 71),
-        (72, 73, 74),
-        (75, 76, 77),
-        (78, 79, 80),
-        (81, 82, 83),
-        (84, 85, 86),
-        (87, 88, 89),
-        (90, 91, 92),
-        (93, 94, 95),
-        (96, 97, 98),
-        (99, 100, 101),
-        (102, 103, 104),
-        (105, 106, 107),
-        (108, 109, 110),
-        (111, 112, 113),
-        (114, 115, 116),
-        (117, 118, 119),
-        (120, 121, 122),
-        (123, 124, 125),
-        (126, 127, 128),
-        (129, 130, 131),
-        (132, 133, 134),
-        (135, 136, 137),
-        (138, 139, 140),
-        (141, 142, 143),
-        (144, 145, 146),
-        (147, 148, 149),
-        (150, 151, 152),
-        (153, 154, 155),
-        (156, 157, 158),
-        (159, 160, 161),
-        (162, 163, 164),
-        (165, 166, 167),
-        (168, 169, 170),
-        (171, 172, 173),
-        (174, 175, 176),
-        (177, 178, 179),
-        (180, 181, 182),
-        (183, 184, 185),
-        (186, 187, 188),
-        (189, 190, 191),
-        (192, 193, 194),
-        (195, 196, 197),
-        (198, 199, 200),
-        (201, 202, 203),
-        (204, 205, 206),
-        (207, 208, 209),
-        (210, 211, 212),
-        (213, 214, 215),
-        (216, 217, 218),
-        (219, 220, 221),
-        (222, 223, 224),
-        (225, 226, 227),
-        (228, 229, 230),
-        (231, 232, 233),
-        (234, 235, 236),
-        (237, 238, 239),
-        (240, 241, 242),
-        (243, 244, 245),
-        (246, 247, 248),
-        (249, 250, 251),
-        (252, 253, 254),
-        (255, 256, 257),
-        (258, 259, 260),
-        (261, 262, 263),
-        (264, 265, 266),
-        (267, 268, 269),
-        (270, 271, 272),
-        (273, 274, 275),
-        (276, 277, 278),
-        (279, 280, 281),
-        (282, 283, 284),
-        (285, 286, 287),
-        (288, 289, 290),
-        (291, 292, 293),
-        (294, 295, 296),
-        (297, 298, 299),
-        (300, 301, 302),
-        (303, 304, 305),
-        (306, 307, 308),
-        (309, 310, 311),
-        (312, 313, 314),
-        (315, 316, 317),
-        (318, 319, 320),
-        (321, 322, 323),
-        (324, 325, 326),
-        (327, 328, 329),
-        (330, 331, 332),
-        (333, 334, 335),
-        (336, 337, 338),
-        (339, 340, 341),
-        (342, 343, 344),
-        (345, 346, 347),
-        (348, 349, 350),
-        (351, 352, 353),
-        (354, 355, 356),
-        (357, 358, 359),
-        (360, 361, 362),
-        (363, 364, 365),
-        (366, 367, 368),
-        (369, 370, 371),
-        (372, 373, 374),
-        (375, 376, 377),
-        (378, 379, 380),
-        (381, 382, 383),
-        (384, 385, 386),
-        (387, 388, 389),
-        (390, 391, 392),
-        (393, 394, 395),
-        (396, 397, 398),
-        (399, 400, 401),
-        (402, 403, 404),
-        (405, 406, 407),
-        (408, 409, 410),
-        (411, 412, 413),
-        (414, 415, 416),
-        (417, 418, 419),
-        (420, 421, 422),
-        (423, 424, 425),
-        (426, 427, 428),
-        (429, 430, 431),
-        (432, 433, 434),
-        (435, 436, 437),
-        (438, 439, 440),
-        (441, 442, 443),
-        (444, 445, 446),
-        (447, 448, 449),
-        (450, 451, 452),
-        (453, 454, 455),
-        (456, 457, 458),
-        (459, 460, 461),
-        (462, 463, 464),
-        (465, 466, 467),
-        (468, 469, 470),
-        (471, 472, 473),
-        (474, 475, 476),
-        (477, 478, 479),
-        (480, 481, 482),
-        (483, 484, 485),
-        (486, 487, 488),
-        (489, 490, 491),
-        (492, 493, 494),
-        (495, 496, 497),
-        (498, 499, 500),
-        (501, 502, 503),
-        (504, 505, 506),
-        (507, 508, 509),
-        (510, 511, 512),
-        (513, 514, 515),
-        (516, 517, 518),
-        (519, 520, 521),
-        (522, 523, 524),
-        (525, 526, 527),
-        (528, 529, 530),
-        (531, 532, 533),
-        (534, 535, 536),
-        (537, 538, 539),
-        (540, 541, 542),
-        (543, 544, 545),
-        (546, 547, 548),
-        (549, 550, 551),
-        (552, 553, 554),
-        (555, 556, 557),
-        (558, 559, 560),
-        (561, 562, 563),
-        (564, 565, 566),
-        (567, 568, 569),
-        (570, 571, 572),
-        (573, 574, 575),
-    ))
+    _verts: Vertices = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (
+            (0.000000, 0.879385, 0.500000),
+            (0.000000, 0.652704, 0.766044),
+            (0.326352, 0.565258, 0.766044),
+            (0.000000, 0.879385, 0.500000),
+            (0.326352, 0.565258, 0.766044),
+            (0.439693, 0.761570, 0.500000),
+            (0.000000, 0.652704, -0.766044),
+            (0.000000, 0.879385, -0.500000),
+            (0.439693, 0.761570, -0.500000),
+            (0.000000, 0.652704, -0.766044),
+            (0.439693, 0.761570, -0.500000),
+            (0.326352, 0.565258, -0.766044),
+            (0.000000, 1.000000, 0.173648),
+            (0.000000, 0.879385, 0.500000),
+            (0.439693, 0.761570, 0.500000),
+            (0.000000, 1.000000, 0.173648),
+            (0.439693, 0.761570, 0.500000),
+            (0.500000, 0.866026, 0.173648),
+            (0.000000, 0.347296, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (0.173648, 0.300768, 0.939693),
+            (0.000000, 0.347296, -0.939693),
+            (0.000000, 0.652704, -0.766044),
+            (0.326352, 0.565258, -0.766044),
+            (0.000000, 0.347296, -0.939693),
+            (0.326352, 0.565258, -0.766044),
+            (0.173648, 0.300768, -0.939693),
+            (0.000000, 1.000000, -0.173648),
+            (0.000000, 1.000000, 0.173648),
+            (0.500000, 0.866026, 0.173648),
+            (0.000000, 1.000000, -0.173648),
+            (0.500000, 0.866026, 0.173648),
+            (0.500000, 0.866026, -0.173648),
+            (0.000000, 0.652704, 0.766044),
+            (0.000000, 0.347296, 0.939693),
+            (0.173648, 0.300768, 0.939693),
+            (0.000000, 0.652704, 0.766044),
+            (0.173648, 0.300768, 0.939693),
+            (0.326352, 0.565258, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (0.000000, 0.347296, -0.939693),
+            (0.173648, 0.300768, -0.939693),
+            (0.000000, 0.879385, -0.500000),
+            (0.000000, 1.000000, -0.173648),
+            (0.500000, 0.866026, -0.173648),
+            (0.000000, 0.879385, -0.500000),
+            (0.500000, 0.866026, -0.173648),
+            (0.439693, 0.761570, -0.500000),
+            (0.500000, 0.866026, 0.173648),
+            (0.439693, 0.761570, 0.500000),
+            (0.761570, 0.439693, 0.500000),
+            (0.500000, 0.866026, 0.173648),
+            (0.761570, 0.439693, 0.500000),
+            (0.866025, 0.500000, 0.173648),
+            (0.173648, 0.300768, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (0.300767, 0.173648, 0.939693),
+            (0.173648, 0.300768, -0.939693),
+            (0.326352, 0.565258, -0.766044),
+            (0.565258, 0.326352, -0.766044),
+            (0.173648, 0.300768, -0.939693),
+            (0.565258, 0.326352, -0.766044),
+            (0.300767, 0.173648, -0.939693),
+            (0.500000, 0.866026, -0.173648),
+            (0.500000, 0.866026, 0.173648),
+            (0.866025, 0.500000, 0.173648),
+            (0.500000, 0.866026, -0.173648),
+            (0.866025, 0.500000, 0.173648),
+            (0.866025, 0.500000, -0.173648),
+            (0.326352, 0.565258, 0.766044),
+            (0.173648, 0.300768, 0.939693),
+            (0.300767, 0.173648, 0.939693),
+            (0.326352, 0.565258, 0.766044),
+            (0.300767, 0.173648, 0.939693),
+            (0.565258, 0.326352, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (0.173648, 0.300768, -0.939693),
+            (0.300767, 0.173648, -0.939693),
+            (0.439693, 0.761570, -0.500000),
+            (0.500000, 0.866026, -0.173648),
+            (0.866025, 0.500000, -0.173648),
+            (0.439693, 0.761570, -0.500000),
+            (0.866025, 0.500000, -0.173648),
+            (0.761570, 0.439693, -0.500000),
+            (0.439693, 0.761570, 0.500000),
+            (0.326352, 0.565258, 0.766044),
+            (0.565258, 0.326352, 0.766044),
+            (0.439693, 0.761570, 0.500000),
+            (0.565258, 0.326352, 0.766044),
+            (0.761570, 0.439693, 0.500000),
+            (0.326352, 0.565258, -0.766044),
+            (0.439693, 0.761570, -0.500000),
+            (0.761570, 0.439693, -0.500000),
+            (0.326352, 0.565258, -0.766044),
+            (0.761570, 0.439693, -0.500000),
+            (0.565258, 0.326352, -0.766044),
+            (0.565258, 0.326352, 0.766044),
+            (0.300767, 0.173648, 0.939693),
+            (0.347296, 0.000000, 0.939693),
+            (0.565258, 0.326352, 0.766044),
+            (0.347296, 0.000000, 0.939693),
+            (0.652704, 0.000000, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (0.300767, 0.173648, -0.939693),
+            (0.347296, 0.000000, -0.939693),
+            (0.761570, 0.439693, -0.500000),
+            (0.866025, 0.500000, -0.173648),
+            (1.000000, 0.000000, -0.173648),
+            (0.761570, 0.439693, -0.500000),
+            (1.000000, 0.000000, -0.173648),
+            (0.879385, 0.000000, -0.500000),
+            (0.761570, 0.439693, 0.500000),
+            (0.565258, 0.326352, 0.766044),
+            (0.652704, 0.000000, 0.766044),
+            (0.761570, 0.439693, 0.500000),
+            (0.652704, 0.000000, 0.766044),
+            (0.879385, 0.000000, 0.500000),
+            (0.565258, 0.326352, -0.766044),
+            (0.761570, 0.439693, -0.500000),
+            (0.879385, 0.000000, -0.500000),
+            (0.565258, 0.326352, -0.766044),
+            (0.879385, 0.000000, -0.500000),
+            (0.652704, 0.000000, -0.766044),
+            (0.866025, 0.500000, 0.173648),
+            (0.761570, 0.439693, 0.500000),
+            (0.879385, 0.000000, 0.500000),
+            (0.866025, 0.500000, 0.173648),
+            (0.879385, 0.000000, 0.500000),
+            (1.000000, 0.000000, 0.173648),
+            (0.300767, 0.173648, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (0.347296, 0.000000, 0.939693),
+            (0.300767, 0.173648, -0.939693),
+            (0.565258, 0.326352, -0.766044),
+            (0.652704, 0.000000, -0.766044),
+            (0.300767, 0.173648, -0.939693),
+            (0.652704, 0.000000, -0.766044),
+            (0.347296, 0.000000, -0.939693),
+            (0.866025, 0.500000, -0.173648),
+            (0.866025, 0.500000, 0.173648),
+            (1.000000, 0.000000, 0.173648),
+            (0.866025, 0.500000, -0.173648),
+            (1.000000, 0.000000, 0.173648),
+            (1.000000, 0.000000, -0.173648),
+            (0.652704, 0.000000, -0.766044),
+            (0.879385, 0.000000, -0.500000),
+            (0.761570, -0.439692, -0.500000),
+            (0.652704, 0.000000, -0.766044),
+            (0.761570, -0.439692, -0.500000),
+            (0.565258, -0.326352, -0.766044),
+            (1.000000, 0.000000, 0.173648),
+            (0.879385, 0.000000, 0.500000),
+            (0.761570, -0.439692, 0.500000),
+            (1.000000, 0.000000, 0.173648),
+            (0.761570, -0.439692, 0.500000),
+            (0.866025, -0.500000, 0.173648),
+            (0.347296, 0.000000, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (0.300767, -0.173648, 0.939693),
+            (0.347296, 0.000000, -0.939693),
+            (0.652704, 0.000000, -0.766044),
+            (0.565258, -0.326352, -0.766044),
+            (0.347296, 0.000000, -0.939693),
+            (0.565258, -0.326352, -0.766044),
+            (0.300767, -0.173648, -0.939693),
+            (1.000000, 0.000000, -0.173648),
+            (1.000000, 0.000000, 0.173648),
+            (0.866025, -0.500000, 0.173648),
+            (1.000000, 0.000000, -0.173648),
+            (0.866025, -0.500000, 0.173648),
+            (0.866025, -0.500000, -0.173648),
+            (0.652704, 0.000000, 0.766044),
+            (0.347296, 0.000000, 0.939693),
+            (0.300767, -0.173648, 0.939693),
+            (0.652704, 0.000000, 0.766044),
+            (0.300767, -0.173648, 0.939693),
+            (0.565258, -0.326352, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (0.347296, 0.000000, -0.939693),
+            (0.300767, -0.173648, -0.939693),
+            (0.879385, 0.000000, -0.500000),
+            (1.000000, 0.000000, -0.173648),
+            (0.866025, -0.500000, -0.173648),
+            (0.879385, 0.000000, -0.500000),
+            (0.866025, -0.500000, -0.173648),
+            (0.761570, -0.439692, -0.500000),
+            (0.879385, 0.000000, 0.500000),
+            (0.652704, 0.000000, 0.766044),
+            (0.565258, -0.326352, 0.766044),
+            (0.879385, 0.000000, 0.500000),
+            (0.565258, -0.326352, 0.766044),
+            (0.761570, -0.439692, 0.500000),
+            (0.866025, -0.500000, -0.173648),
+            (0.866025, -0.500000, 0.173648),
+            (0.500000, -0.866025, 0.173648),
+            (0.866025, -0.500000, -0.173648),
+            (0.500000, -0.866025, 0.173648),
+            (0.500000, -0.866025, -0.173648),
+            (0.565258, -0.326352, 0.766044),
+            (0.300767, -0.173648, 0.939693),
+            (0.173648, -0.300767, 0.939693),
+            (0.565258, -0.326352, 0.766044),
+            (0.173648, -0.300767, 0.939693),
+            (0.326352, -0.565258, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (0.300767, -0.173648, -0.939693),
+            (0.173648, -0.300767, -0.939693),
+            (0.761570, -0.439692, -0.500000),
+            (0.866025, -0.500000, -0.173648),
+            (0.500000, -0.866025, -0.173648),
+            (0.761570, -0.439692, -0.500000),
+            (0.500000, -0.866025, -0.173648),
+            (0.439693, -0.761570, -0.500000),
+            (0.761570, -0.439692, 0.500000),
+            (0.565258, -0.326352, 0.766044),
+            (0.326352, -0.565258, 0.766044),
+            (0.761570, -0.439692, 0.500000),
+            (0.326352, -0.565258, 0.766044),
+            (0.439693, -0.761570, 0.500000),
+            (0.565258, -0.326352, -0.766044),
+            (0.761570, -0.439692, -0.500000),
+            (0.439693, -0.761570, -0.500000),
+            (0.565258, -0.326352, -0.766044),
+            (0.439693, -0.761570, -0.500000),
+            (0.326352, -0.565258, -0.766044),
+            (0.866025, -0.500000, 0.173648),
+            (0.761570, -0.439692, 0.500000),
+            (0.439693, -0.761570, 0.500000),
+            (0.866025, -0.500000, 0.173648),
+            (0.439693, -0.761570, 0.500000),
+            (0.500000, -0.866025, 0.173648),
+            (0.300767, -0.173648, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (0.173648, -0.300767, 0.939693),
+            (0.300767, -0.173648, -0.939693),
+            (0.565258, -0.326352, -0.766044),
+            (0.326352, -0.565258, -0.766044),
+            (0.300767, -0.173648, -0.939693),
+            (0.326352, -0.565258, -0.766044),
+            (0.173648, -0.300767, -0.939693),
+            (0.439693, -0.761570, 0.500000),
+            (0.326352, -0.565258, 0.766044),
+            (0.000000, -0.652703, 0.766044),
+            (0.439693, -0.761570, 0.500000),
+            (0.000000, -0.652703, 0.766044),
+            (0.000000, -0.879385, 0.500000),
+            (0.326352, -0.565258, -0.766044),
+            (0.439693, -0.761570, -0.500000),
+            (0.000000, -0.879385, -0.500000),
+            (0.326352, -0.565258, -0.766044),
+            (0.000000, -0.879385, -0.500000),
+            (0.000000, -0.652703, -0.766044),
+            (0.500000, -0.866025, 0.173648),
+            (0.439693, -0.761570, 0.500000),
+            (0.000000, -0.879385, 0.500000),
+            (0.500000, -0.866025, 0.173648),
+            (0.000000, -0.879385, 0.500000),
+            (0.000000, -1.000000, 0.173648),
+            (0.173648, -0.300767, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (0.000000, -0.347296, 0.939693),
+            (0.173648, -0.300767, -0.939693),
+            (0.326352, -0.565258, -0.766044),
+            (0.000000, -0.652703, -0.766044),
+            (0.173648, -0.300767, -0.939693),
+            (0.000000, -0.652703, -0.766044),
+            (0.000000, -0.347296, -0.939693),
+            (0.500000, -0.866025, -0.173648),
+            (0.500000, -0.866025, 0.173648),
+            (0.000000, -1.000000, 0.173648),
+            (0.500000, -0.866025, -0.173648),
+            (0.000000, -1.000000, 0.173648),
+            (0.000000, -1.000000, -0.173648),
+            (0.326352, -0.565258, 0.766044),
+            (0.173648, -0.300767, 0.939693),
+            (0.000000, -0.347296, 0.939693),
+            (0.326352, -0.565258, 0.766044),
+            (0.000000, -0.347296, 0.939693),
+            (0.000000, -0.652703, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (0.173648, -0.300767, -0.939693),
+            (0.000000, -0.347296, -0.939693),
+            (0.439693, -0.761570, -0.500000),
+            (0.500000, -0.866025, -0.173648),
+            (0.000000, -1.000000, -0.173648),
+            (0.439693, -0.761570, -0.500000),
+            (0.000000, -1.000000, -0.173648),
+            (0.000000, -0.879385, -0.500000),
+            (0.000000, -0.347296, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (-0.173648, -0.300767, 0.939693),
+            (0.000000, -0.347296, -0.939693),
+            (0.000000, -0.652703, -0.766044),
+            (-0.326352, -0.565258, -0.766044),
+            (0.000000, -0.347296, -0.939693),
+            (-0.326352, -0.565258, -0.766044),
+            (-0.173648, -0.300767, -0.939693),
+            (0.000000, -1.000000, -0.173648),
+            (0.000000, -1.000000, 0.173648),
+            (-0.500000, -0.866025, 0.173648),
+            (0.000000, -1.000000, -0.173648),
+            (-0.500000, -0.866025, 0.173648),
+            (-0.500000, -0.866025, -0.173648),
+            (0.000000, -0.652703, 0.766044),
+            (0.000000, -0.347296, 0.939693),
+            (-0.173648, -0.300767, 0.939693),
+            (0.000000, -0.652703, 0.766044),
+            (-0.173648, -0.300767, 0.939693),
+            (-0.326352, -0.565258, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (0.000000, -0.347296, -0.939693),
+            (-0.173648, -0.300767, -0.939693),
+            (0.000000, -0.879385, -0.500000),
+            (0.000000, -1.000000, -0.173648),
+            (-0.500000, -0.866025, -0.173648),
+            (0.000000, -0.879385, -0.500000),
+            (-0.500000, -0.866025, -0.173648),
+            (-0.439693, -0.761570, -0.500000),
+            (0.000000, -0.879385, 0.500000),
+            (0.000000, -0.652703, 0.766044),
+            (-0.326352, -0.565258, 0.766044),
+            (0.000000, -0.879385, 0.500000),
+            (-0.326352, -0.565258, 0.766044),
+            (-0.439693, -0.761570, 0.500000),
+            (0.000000, -0.652703, -0.766044),
+            (0.000000, -0.879385, -0.500000),
+            (-0.439693, -0.761570, -0.500000),
+            (0.000000, -0.652703, -0.766044),
+            (-0.439693, -0.761570, -0.500000),
+            (-0.326352, -0.565258, -0.766044),
+            (0.000000, -1.000000, 0.173648),
+            (0.000000, -0.879385, 0.500000),
+            (-0.439693, -0.761570, 0.500000),
+            (0.000000, -1.000000, 0.173648),
+            (-0.439693, -0.761570, 0.500000),
+            (-0.500000, -0.866025, 0.173648),
+            (0.000000, 0.000000, -1.000000),
+            (-0.173648, -0.300767, -0.939693),
+            (-0.300767, -0.173648, -0.939693),
+            (-0.439693, -0.761570, -0.500000),
+            (-0.500000, -0.866025, -0.173648),
+            (-0.866025, -0.500000, -0.173648),
+            (-0.439693, -0.761570, -0.500000),
+            (-0.866025, -0.500000, -0.173648),
+            (-0.761570, -0.439692, -0.500000),
+            (-0.439693, -0.761570, 0.500000),
+            (-0.326352, -0.565258, 0.766044),
+            (-0.565258, -0.326352, 0.766044),
+            (-0.439693, -0.761570, 0.500000),
+            (-0.565258, -0.326352, 0.766044),
+            (-0.761570, -0.439692, 0.500000),
+            (-0.326352, -0.565258, -0.766044),
+            (-0.439693, -0.761570, -0.500000),
+            (-0.761570, -0.439692, -0.500000),
+            (-0.326352, -0.565258, -0.766044),
+            (-0.761570, -0.439692, -0.500000),
+            (-0.565258, -0.326352, -0.766044),
+            (-0.500000, -0.866025, 0.173648),
+            (-0.439693, -0.761570, 0.500000),
+            (-0.761570, -0.439692, 0.500000),
+            (-0.500000, -0.866025, 0.173648),
+            (-0.761570, -0.439692, 0.500000),
+            (-0.866025, -0.500000, 0.173648),
+            (-0.173648, -0.300767, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (-0.300767, -0.173648, 0.939693),
+            (-0.173648, -0.300767, -0.939693),
+            (-0.326352, -0.565258, -0.766044),
+            (-0.565258, -0.326352, -0.766044),
+            (-0.173648, -0.300767, -0.939693),
+            (-0.565258, -0.326352, -0.766044),
+            (-0.300767, -0.173648, -0.939693),
+            (-0.500000, -0.866025, -0.173648),
+            (-0.500000, -0.866025, 0.173648),
+            (-0.866025, -0.500000, 0.173648),
+            (-0.500000, -0.866025, -0.173648),
+            (-0.866025, -0.500000, 0.173648),
+            (-0.866025, -0.500000, -0.173648),
+            (-0.326352, -0.565258, 0.766044),
+            (-0.173648, -0.300767, 0.939693),
+            (-0.300767, -0.173648, 0.939693),
+            (-0.326352, -0.565258, 0.766044),
+            (-0.300767, -0.173648, 0.939693),
+            (-0.565258, -0.326352, 0.766044),
+            (-0.565258, -0.326352, -0.766044),
+            (-0.761570, -0.439692, -0.500000),
+            (-0.879385, 0.000000, -0.500000),
+            (-0.565258, -0.326352, -0.766044),
+            (-0.879385, 0.000000, -0.500000),
+            (-0.652704, 0.000000, -0.766044),
+            (-0.866025, -0.500000, 0.173648),
+            (-0.761570, -0.439692, 0.500000),
+            (-0.879385, 0.000000, 0.500000),
+            (-0.866025, -0.500000, 0.173648),
+            (-0.879385, 0.000000, 0.500000),
+            (-1.000000, 0.000000, 0.173648),
+            (-0.300767, -0.173648, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (-0.347296, 0.000000, 0.939693),
+            (-0.300767, -0.173648, -0.939693),
+            (-0.565258, -0.326352, -0.766044),
+            (-0.652704, 0.000000, -0.766044),
+            (-0.300767, -0.173648, -0.939693),
+            (-0.652704, 0.000000, -0.766044),
+            (-0.347296, 0.000000, -0.939693),
+            (-0.866025, -0.500000, -0.173648),
+            (-0.866025, -0.500000, 0.173648),
+            (-1.000000, 0.000000, 0.173648),
+            (-0.866025, -0.500000, -0.173648),
+            (-1.000000, 0.000000, 0.173648),
+            (-1.000000, 0.000000, -0.173648),
+            (-0.565258, -0.326352, 0.766044),
+            (-0.300767, -0.173648, 0.939693),
+            (-0.347296, 0.000000, 0.939693),
+            (-0.565258, -0.326352, 0.766044),
+            (-0.347296, 0.000000, 0.939693),
+            (-0.652704, 0.000000, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (-0.300767, -0.173648, -0.939693),
+            (-0.347296, 0.000000, -0.939693),
+            (-0.761570, -0.439692, -0.500000),
+            (-0.866025, -0.500000, -0.173648),
+            (-1.000000, 0.000000, -0.173648),
+            (-0.761570, -0.439692, -0.500000),
+            (-1.000000, 0.000000, -0.173648),
+            (-0.879385, 0.000000, -0.500000),
+            (-0.761570, -0.439692, 0.500000),
+            (-0.565258, -0.326352, 0.766044),
+            (-0.652704, 0.000000, 0.766044),
+            (-0.761570, -0.439692, 0.500000),
+            (-0.652704, 0.000000, 0.766044),
+            (-0.879385, 0.000000, 0.500000),
+            (-1.000000, 0.000000, -0.173648),
+            (-1.000000, 0.000000, 0.173648),
+            (-0.866025, 0.500000, 0.173648),
+            (-1.000000, 0.000000, -0.173648),
+            (-0.866025, 0.500000, 0.173648),
+            (-0.866025, 0.500000, -0.173648),
+            (-0.652704, 0.000000, 0.766044),
+            (-0.347296, 0.000000, 0.939693),
+            (-0.300767, 0.173648, 0.939693),
+            (-0.652704, 0.000000, 0.766044),
+            (-0.300767, 0.173648, 0.939693),
+            (-0.565258, 0.326352, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (-0.347296, 0.000000, -0.939693),
+            (-0.300767, 0.173648, -0.939693),
+            (-0.879385, 0.000000, -0.500000),
+            (-1.000000, 0.000000, -0.173648),
+            (-0.866025, 0.500000, -0.173648),
+            (-0.879385, 0.000000, -0.500000),
+            (-0.866025, 0.500000, -0.173648),
+            (-0.761570, 0.439693, -0.500000),
+            (-0.879385, 0.000000, 0.500000),
+            (-0.652704, 0.000000, 0.766044),
+            (-0.565258, 0.326352, 0.766044),
+            (-0.879385, 0.000000, 0.500000),
+            (-0.565258, 0.326352, 0.766044),
+            (-0.761570, 0.439693, 0.500000),
+            (-0.652704, 0.000000, -0.766044),
+            (-0.879385, 0.000000, -0.500000),
+            (-0.761570, 0.439693, -0.500000),
+            (-0.652704, 0.000000, -0.766044),
+            (-0.761570, 0.439693, -0.500000),
+            (-0.565258, 0.326352, -0.766044),
+            (-1.000000, 0.000000, 0.173648),
+            (-0.879385, 0.000000, 0.500000),
+            (-0.761570, 0.439693, 0.500000),
+            (-1.000000, 0.000000, 0.173648),
+            (-0.761570, 0.439693, 0.500000),
+            (-0.866025, 0.500000, 0.173648),
+            (-0.347296, 0.000000, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (-0.300767, 0.173648, 0.939693),
+            (-0.347296, 0.000000, -0.939693),
+            (-0.652704, 0.000000, -0.766044),
+            (-0.565258, 0.326352, -0.766044),
+            (-0.347296, 0.000000, -0.939693),
+            (-0.565258, 0.326352, -0.766044),
+            (-0.300767, 0.173648, -0.939693),
+            (-0.761570, 0.439693, 0.500000),
+            (-0.565258, 0.326352, 0.766044),
+            (-0.326352, 0.565258, 0.766044),
+            (-0.761570, 0.439693, 0.500000),
+            (-0.326352, 0.565258, 0.766044),
+            (-0.439693, 0.761570, 0.500000),
+            (-0.565258, 0.326352, -0.766044),
+            (-0.761570, 0.439693, -0.500000),
+            (-0.439693, 0.761570, -0.500000),
+            (-0.565258, 0.326352, -0.766044),
+            (-0.439693, 0.761570, -0.500000),
+            (-0.326352, 0.565258, -0.766044),
+            (-0.866025, 0.500000, 0.173648),
+            (-0.761570, 0.439693, 0.500000),
+            (-0.439693, 0.761570, 0.500000),
+            (-0.866025, 0.500000, 0.173648),
+            (-0.439693, 0.761570, 0.500000),
+            (-0.500000, 0.866026, 0.173648),
+            (-0.300767, 0.173648, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (-0.173648, 0.300767, 0.939693),
+            (-0.300767, 0.173648, -0.939693),
+            (-0.565258, 0.326352, -0.766044),
+            (-0.326352, 0.565258, -0.766044),
+            (-0.300767, 0.173648, -0.939693),
+            (-0.326352, 0.565258, -0.766044),
+            (-0.173648, 0.300768, -0.939693),
+            (-0.866025, 0.500000, -0.173648),
+            (-0.866025, 0.500000, 0.173648),
+            (-0.500000, 0.866026, 0.173648),
+            (-0.866025, 0.500000, -0.173648),
+            (-0.500000, 0.866026, 0.173648),
+            (-0.500000, 0.866025, -0.173648),
+            (-0.565258, 0.326352, 0.766044),
+            (-0.300767, 0.173648, 0.939693),
+            (-0.173648, 0.300767, 0.939693),
+            (-0.565258, 0.326352, 0.766044),
+            (-0.173648, 0.300767, 0.939693),
+            (-0.326352, 0.565258, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (-0.300767, 0.173648, -0.939693),
+            (-0.173648, 0.300768, -0.939693),
+            (-0.761570, 0.439693, -0.500000),
+            (-0.866025, 0.500000, -0.173648),
+            (-0.500000, 0.866025, -0.173648),
+            (-0.761570, 0.439693, -0.500000),
+            (-0.500000, 0.866025, -0.173648),
+            (-0.439693, 0.761570, -0.500000),
+            (-0.173648, 0.300767, 0.939693),
+            (0.000000, 0.000000, 1.000000),
+            (0.000000, 0.347296, 0.939693),
+            (-0.173648, 0.300768, -0.939693),
+            (-0.326352, 0.565258, -0.766044),
+            (0.000000, 0.652704, -0.766044),
+            (-0.173648, 0.300768, -0.939693),
+            (0.000000, 0.652704, -0.766044),
+            (0.000000, 0.347296, -0.939693),
+            (-0.500000, 0.866025, -0.173648),
+            (-0.500000, 0.866026, 0.173648),
+            (0.000000, 1.000000, 0.173648),
+            (-0.500000, 0.866025, -0.173648),
+            (0.000000, 1.000000, 0.173648),
+            (0.000000, 1.000000, -0.173648),
+            (-0.326352, 0.565258, 0.766044),
+            (-0.173648, 0.300767, 0.939693),
+            (0.000000, 0.347296, 0.939693),
+            (-0.326352, 0.565258, 0.766044),
+            (0.000000, 0.347296, 0.939693),
+            (0.000000, 0.652704, 0.766044),
+            (0.000000, 0.000000, -1.000000),
+            (-0.173648, 0.300768, -0.939693),
+            (0.000000, 0.347296, -0.939693),
+            (-0.439693, 0.761570, -0.500000),
+            (-0.500000, 0.866025, -0.173648),
+            (0.000000, 1.000000, -0.173648),
+            (-0.439693, 0.761570, -0.500000),
+            (0.000000, 1.000000, -0.173648),
+            (0.000000, 0.879385, -0.500000),
+            (-0.439693, 0.761570, 0.500000),
+            (-0.326352, 0.565258, 0.766044),
+            (0.000000, 0.652704, 0.766044),
+            (-0.439693, 0.761570, 0.500000),
+            (0.000000, 0.652704, 0.766044),
+            (0.000000, 0.879385, 0.500000),
+            (-0.326352, 0.565258, -0.766044),
+            (-0.439693, 0.761570, -0.500000),
+            (0.000000, 0.879385, -0.500000),
+            (-0.326352, 0.565258, -0.766044),
+            (0.000000, 0.879385, -0.500000),
+            (0.000000, 0.652704, -0.766044),
+            (-0.500000, 0.866026, 0.173648),
+            (-0.439693, 0.761570, 0.500000),
+            (0.000000, 0.879385, 0.500000),
+            (-0.500000, 0.866026, 0.173648),
+            (0.000000, 0.879385, 0.500000),
+            (0.000000, 1.000000, 0.173648),
+        )
+    )
+    _normals: Normals = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (
+            (0.000000, 0.869900, 0.493200),
+            (-0.000000, 0.653800, 0.756700),
+            (0.326900, 0.566200, 0.756700),
+            (0.000000, 0.869900, 0.493200),
+            (0.326900, 0.566200, 0.756700),
+            (0.435000, 0.753400, 0.493200),
+            (-0.000000, 0.653800, -0.756700),
+            (-0.000000, 0.869900, -0.493200),
+            (0.435000, 0.753400, -0.493200),
+            (-0.000000, 0.653800, -0.756700),
+            (0.435000, 0.753400, -0.493200),
+            (0.326900, 0.566200, -0.756700),
+            (-0.000000, 0.985200, 0.171300),
+            (0.000000, 0.869900, 0.493200),
+            (0.435000, 0.753400, 0.493200),
+            (-0.000000, 0.985200, 0.171300),
+            (0.435000, 0.753400, 0.493200),
+            (0.492600, 0.853200, 0.171300),
+            (-0.000000, 0.362500, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (0.181300, 0.313900, 0.932000),
+            (-0.000000, 0.362500, -0.932000),
+            (-0.000000, 0.653800, -0.756700),
+            (0.326900, 0.566200, -0.756700),
+            (-0.000000, 0.362500, -0.932000),
+            (0.326900, 0.566200, -0.756700),
+            (0.181300, 0.313900, -0.932000),
+            (-0.000000, 0.985200, -0.171300),
+            (-0.000000, 0.985200, 0.171300),
+            (0.492600, 0.853200, 0.171300),
+            (-0.000000, 0.985200, -0.171300),
+            (0.492600, 0.853200, 0.171300),
+            (0.492600, 0.853200, -0.171300),
+            (-0.000000, 0.653800, 0.756700),
+            (-0.000000, 0.362500, 0.932000),
+            (0.181300, 0.313900, 0.932000),
+            (-0.000000, 0.653800, 0.756700),
+            (0.181300, 0.313900, 0.932000),
+            (0.326900, 0.566200, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (-0.000000, 0.362500, -0.932000),
+            (0.181300, 0.313900, -0.932000),
+            (-0.000000, 0.869900, -0.493200),
+            (-0.000000, 0.985200, -0.171300),
+            (0.492600, 0.853200, -0.171300),
+            (-0.000000, 0.869900, -0.493200),
+            (0.492600, 0.853200, -0.171300),
+            (0.435000, 0.753400, -0.493200),
+            (0.492600, 0.853200, 0.171300),
+            (0.435000, 0.753400, 0.493200),
+            (0.753400, 0.435000, 0.493200),
+            (0.492600, 0.853200, 0.171300),
+            (0.753400, 0.435000, 0.493200),
+            (0.853200, 0.492600, 0.171300),
+            (0.181300, 0.313900, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (0.313900, 0.181300, 0.932000),
+            (0.181300, 0.313900, -0.932000),
+            (0.326900, 0.566200, -0.756700),
+            (0.566200, 0.326900, -0.756700),
+            (0.181300, 0.313900, -0.932000),
+            (0.566200, 0.326900, -0.756700),
+            (0.313900, 0.181300, -0.932000),
+            (0.492600, 0.853200, -0.171300),
+            (0.492600, 0.853200, 0.171300),
+            (0.853200, 0.492600, 0.171300),
+            (0.492600, 0.853200, -0.171300),
+            (0.853200, 0.492600, 0.171300),
+            (0.853200, 0.492600, -0.171300),
+            (0.326900, 0.566200, 0.756700),
+            (0.181300, 0.313900, 0.932000),
+            (0.313900, 0.181300, 0.932000),
+            (0.326900, 0.566200, 0.756700),
+            (0.313900, 0.181300, 0.932000),
+            (0.566200, 0.326900, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (0.181300, 0.313900, -0.932000),
+            (0.313900, 0.181300, -0.932000),
+            (0.435000, 0.753400, -0.493200),
+            (0.492600, 0.853200, -0.171300),
+            (0.853200, 0.492600, -0.171300),
+            (0.435000, 0.753400, -0.493200),
+            (0.853200, 0.492600, -0.171300),
+            (0.753400, 0.435000, -0.493200),
+            (0.435000, 0.753400, 0.493200),
+            (0.326900, 0.566200, 0.756700),
+            (0.566200, 0.326900, 0.756700),
+            (0.435000, 0.753400, 0.493200),
+            (0.566200, 0.326900, 0.756700),
+            (0.753400, 0.435000, 0.493200),
+            (0.326900, 0.566200, -0.756700),
+            (0.435000, 0.753400, -0.493200),
+            (0.753400, 0.435000, -0.493200),
+            (0.326900, 0.566200, -0.756700),
+            (0.753400, 0.435000, -0.493200),
+            (0.566200, 0.326900, -0.756700),
+            (0.566200, 0.326900, 0.756700),
+            (0.313900, 0.181300, 0.932000),
+            (0.362500, 0.000000, 0.932000),
+            (0.566200, 0.326900, 0.756700),
+            (0.362500, 0.000000, 0.932000),
+            (0.653800, -0.000000, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (0.313900, 0.181300, -0.932000),
+            (0.362500, 0.000000, -0.932000),
+            (0.753400, 0.435000, -0.493200),
+            (0.853200, 0.492600, -0.171300),
+            (0.985200, -0.000000, -0.171300),
+            (0.753400, 0.435000, -0.493200),
+            (0.985200, -0.000000, -0.171300),
+            (0.869900, -0.000000, -0.493200),
+            (0.753400, 0.435000, 0.493200),
+            (0.566200, 0.326900, 0.756700),
+            (0.653800, -0.000000, 0.756700),
+            (0.753400, 0.435000, 0.493200),
+            (0.653800, -0.000000, 0.756700),
+            (0.869900, -0.000000, 0.493200),
+            (0.566200, 0.326900, -0.756700),
+            (0.753400, 0.435000, -0.493200),
+            (0.869900, -0.000000, -0.493200),
+            (0.566200, 0.326900, -0.756700),
+            (0.869900, -0.000000, -0.493200),
+            (0.653800, -0.000000, -0.756700),
+            (0.853200, 0.492600, 0.171300),
+            (0.753400, 0.435000, 0.493200),
+            (0.869900, -0.000000, 0.493200),
+            (0.853200, 0.492600, 0.171300),
+            (0.869900, -0.000000, 0.493200),
+            (0.985200, -0.000000, 0.171300),
+            (0.313900, 0.181300, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (0.362500, 0.000000, 0.932000),
+            (0.313900, 0.181300, -0.932000),
+            (0.566200, 0.326900, -0.756700),
+            (0.653800, -0.000000, -0.756700),
+            (0.313900, 0.181300, -0.932000),
+            (0.653800, -0.000000, -0.756700),
+            (0.362500, 0.000000, -0.932000),
+            (0.853200, 0.492600, -0.171300),
+            (0.853200, 0.492600, 0.171300),
+            (0.985200, -0.000000, 0.171300),
+            (0.853200, 0.492600, -0.171300),
+            (0.985200, -0.000000, 0.171300),
+            (0.985200, -0.000000, -0.171300),
+            (0.653800, -0.000000, -0.756700),
+            (0.869900, -0.000000, -0.493200),
+            (0.753400, -0.435000, -0.493200),
+            (0.653800, -0.000000, -0.756700),
+            (0.753400, -0.435000, -0.493200),
+            (0.566200, -0.326900, -0.756700),
+            (0.985200, -0.000000, 0.171300),
+            (0.869900, -0.000000, 0.493200),
+            (0.753400, -0.435000, 0.493200),
+            (0.985200, -0.000000, 0.171300),
+            (0.753400, -0.435000, 0.493200),
+            (0.853200, -0.492600, 0.171300),
+            (0.362500, 0.000000, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (0.313900, -0.181300, 0.932000),
+            (0.362500, 0.000000, -0.932000),
+            (0.653800, -0.000000, -0.756700),
+            (0.566200, -0.326900, -0.756700),
+            (0.362500, 0.000000, -0.932000),
+            (0.566200, -0.326900, -0.756700),
+            (0.313900, -0.181300, -0.932000),
+            (0.985200, -0.000000, -0.171300),
+            (0.985200, -0.000000, 0.171300),
+            (0.853200, -0.492600, 0.171300),
+            (0.985200, -0.000000, -0.171300),
+            (0.853200, -0.492600, 0.171300),
+            (0.853200, -0.492600, -0.171300),
+            (0.653800, -0.000000, 0.756700),
+            (0.362500, 0.000000, 0.932000),
+            (0.313900, -0.181300, 0.932000),
+            (0.653800, -0.000000, 0.756700),
+            (0.313900, -0.181300, 0.932000),
+            (0.566200, -0.326900, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (0.362500, 0.000000, -0.932000),
+            (0.313900, -0.181300, -0.932000),
+            (0.869900, -0.000000, -0.493200),
+            (0.985200, -0.000000, -0.171300),
+            (0.853200, -0.492600, -0.171300),
+            (0.869900, -0.000000, -0.493200),
+            (0.853200, -0.492600, -0.171300),
+            (0.753400, -0.435000, -0.493200),
+            (0.869900, -0.000000, 0.493200),
+            (0.653800, -0.000000, 0.756700),
+            (0.566200, -0.326900, 0.756700),
+            (0.869900, -0.000000, 0.493200),
+            (0.566200, -0.326900, 0.756700),
+            (0.753400, -0.435000, 0.493200),
+            (0.853200, -0.492600, -0.171300),
+            (0.853200, -0.492600, 0.171300),
+            (0.492600, -0.853200, 0.171300),
+            (0.853200, -0.492600, -0.171300),
+            (0.492600, -0.853200, 0.171300),
+            (0.492600, -0.853200, -0.171300),
+            (0.566200, -0.326900, 0.756700),
+            (0.313900, -0.181300, 0.932000),
+            (0.181300, -0.313900, 0.932000),
+            (0.566200, -0.326900, 0.756700),
+            (0.181300, -0.313900, 0.932000),
+            (0.326900, -0.566200, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (0.313900, -0.181300, -0.932000),
+            (0.181300, -0.313900, -0.932000),
+            (0.753400, -0.435000, -0.493200),
+            (0.853200, -0.492600, -0.171300),
+            (0.492600, -0.853200, -0.171300),
+            (0.753400, -0.435000, -0.493200),
+            (0.492600, -0.853200, -0.171300),
+            (0.435000, -0.753400, -0.493200),
+            (0.753400, -0.435000, 0.493200),
+            (0.566200, -0.326900, 0.756700),
+            (0.326900, -0.566200, 0.756700),
+            (0.753400, -0.435000, 0.493200),
+            (0.326900, -0.566200, 0.756700),
+            (0.435000, -0.753400, 0.493200),
+            (0.566200, -0.326900, -0.756700),
+            (0.753400, -0.435000, -0.493200),
+            (0.435000, -0.753400, -0.493200),
+            (0.566200, -0.326900, -0.756700),
+            (0.435000, -0.753400, -0.493200),
+            (0.326900, -0.566200, -0.756700),
+            (0.853200, -0.492600, 0.171300),
+            (0.753400, -0.435000, 0.493200),
+            (0.435000, -0.753400, 0.493200),
+            (0.853200, -0.492600, 0.171300),
+            (0.435000, -0.753400, 0.493200),
+            (0.492600, -0.853200, 0.171300),
+            (0.313900, -0.181300, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (0.181300, -0.313900, 0.932000),
+            (0.313900, -0.181300, -0.932000),
+            (0.566200, -0.326900, -0.756700),
+            (0.326900, -0.566200, -0.756700),
+            (0.313900, -0.181300, -0.932000),
+            (0.326900, -0.566200, -0.756700),
+            (0.181300, -0.313900, -0.932000),
+            (0.435000, -0.753400, 0.493200),
+            (0.326900, -0.566200, 0.756700),
+            (-0.000000, -0.653800, 0.756700),
+            (0.435000, -0.753400, 0.493200),
+            (-0.000000, -0.653800, 0.756700),
+            (0.000000, -0.869900, 0.493200),
+            (0.326900, -0.566200, -0.756700),
+            (0.435000, -0.753400, -0.493200),
+            (-0.000000, -0.869900, -0.493200),
+            (0.326900, -0.566200, -0.756700),
+            (-0.000000, -0.869900, -0.493200),
+            (0.000000, -0.653800, -0.756700),
+            (0.492600, -0.853200, 0.171300),
+            (0.435000, -0.753400, 0.493200),
+            (0.000000, -0.869900, 0.493200),
+            (0.492600, -0.853200, 0.171300),
+            (0.000000, -0.869900, 0.493200),
+            (0.000000, -0.985200, 0.171300),
+            (0.181300, -0.313900, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (-0.000000, -0.362500, 0.932000),
+            (0.181300, -0.313900, -0.932000),
+            (0.326900, -0.566200, -0.756700),
+            (0.000000, -0.653800, -0.756700),
+            (0.181300, -0.313900, -0.932000),
+            (0.000000, -0.653800, -0.756700),
+            (0.000000, -0.362500, -0.932000),
+            (0.492600, -0.853200, -0.171300),
+            (0.492600, -0.853200, 0.171300),
+            (0.000000, -0.985200, 0.171300),
+            (0.492600, -0.853200, -0.171300),
+            (0.000000, -0.985200, 0.171300),
+            (-0.000000, -0.985200, -0.171300),
+            (0.326900, -0.566200, 0.756700),
+            (0.181300, -0.313900, 0.932000),
+            (-0.000000, -0.362500, 0.932000),
+            (0.326900, -0.566200, 0.756700),
+            (-0.000000, -0.362500, 0.932000),
+            (-0.000000, -0.653800, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (0.181300, -0.313900, -0.932000),
+            (0.000000, -0.362500, -0.932000),
+            (0.435000, -0.753400, -0.493200),
+            (0.492600, -0.853200, -0.171300),
+            (-0.000000, -0.985200, -0.171300),
+            (0.435000, -0.753400, -0.493200),
+            (-0.000000, -0.985200, -0.171300),
+            (-0.000000, -0.869900, -0.493200),
+            (-0.000000, -0.362500, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (-0.181300, -0.313900, 0.932000),
+            (0.000000, -0.362500, -0.932000),
+            (0.000000, -0.653800, -0.756700),
+            (-0.326900, -0.566200, -0.756700),
+            (0.000000, -0.362500, -0.932000),
+            (-0.326900, -0.566200, -0.756700),
+            (-0.181300, -0.313900, -0.932000),
+            (-0.000000, -0.985200, -0.171300),
+            (0.000000, -0.985200, 0.171300),
+            (-0.492600, -0.853200, 0.171300),
+            (-0.000000, -0.985200, -0.171300),
+            (-0.492600, -0.853200, 0.171300),
+            (-0.492600, -0.853200, -0.171300),
+            (-0.000000, -0.653800, 0.756700),
+            (-0.000000, -0.362500, 0.932000),
+            (-0.181300, -0.313900, 0.932000),
+            (-0.000000, -0.653800, 0.756700),
+            (-0.181300, -0.313900, 0.932000),
+            (-0.326900, -0.566200, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (0.000000, -0.362500, -0.932000),
+            (-0.181300, -0.313900, -0.932000),
+            (-0.000000, -0.869900, -0.493200),
+            (-0.000000, -0.985200, -0.171300),
+            (-0.492600, -0.853200, -0.171300),
+            (-0.000000, -0.869900, -0.493200),
+            (-0.492600, -0.853200, -0.171300),
+            (-0.435000, -0.753400, -0.493200),
+            (0.000000, -0.869900, 0.493200),
+            (-0.000000, -0.653800, 0.756700),
+            (-0.326900, -0.566200, 0.756700),
+            (0.000000, -0.869900, 0.493200),
+            (-0.326900, -0.566200, 0.756700),
+            (-0.435000, -0.753400, 0.493200),
+            (0.000000, -0.653800, -0.756700),
+            (-0.000000, -0.869900, -0.493200),
+            (-0.435000, -0.753400, -0.493200),
+            (0.000000, -0.653800, -0.756700),
+            (-0.435000, -0.753400, -0.493200),
+            (-0.326900, -0.566200, -0.756700),
+            (0.000000, -0.985200, 0.171300),
+            (0.000000, -0.869900, 0.493200),
+            (-0.435000, -0.753400, 0.493200),
+            (0.000000, -0.985200, 0.171300),
+            (-0.435000, -0.753400, 0.493200),
+            (-0.492600, -0.853200, 0.171300),
+            (0.000000, -0.000000, -1.000000),
+            (-0.181300, -0.313900, -0.932000),
+            (-0.313900, -0.181300, -0.932000),
+            (-0.435000, -0.753400, -0.493200),
+            (-0.492600, -0.853200, -0.171300),
+            (-0.853200, -0.492600, -0.171300),
+            (-0.435000, -0.753400, -0.493200),
+            (-0.853200, -0.492600, -0.171300),
+            (-0.753400, -0.435000, -0.493200),
+            (-0.435000, -0.753400, 0.493200),
+            (-0.326900, -0.566200, 0.756700),
+            (-0.566200, -0.326900, 0.756700),
+            (-0.435000, -0.753400, 0.493200),
+            (-0.566200, -0.326900, 0.756700),
+            (-0.753400, -0.435000, 0.493200),
+            (-0.326900, -0.566200, -0.756700),
+            (-0.435000, -0.753400, -0.493200),
+            (-0.753400, -0.435000, -0.493200),
+            (-0.326900, -0.566200, -0.756700),
+            (-0.753400, -0.435000, -0.493200),
+            (-0.566200, -0.326900, -0.756700),
+            (-0.492600, -0.853200, 0.171300),
+            (-0.435000, -0.753400, 0.493200),
+            (-0.753400, -0.435000, 0.493200),
+            (-0.492600, -0.853200, 0.171300),
+            (-0.753400, -0.435000, 0.493200),
+            (-0.853200, -0.492600, 0.171300),
+            (-0.181300, -0.313900, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (-0.313900, -0.181300, 0.932000),
+            (-0.181300, -0.313900, -0.932000),
+            (-0.326900, -0.566200, -0.756700),
+            (-0.566200, -0.326900, -0.756700),
+            (-0.181300, -0.313900, -0.932000),
+            (-0.566200, -0.326900, -0.756700),
+            (-0.313900, -0.181300, -0.932000),
+            (-0.492600, -0.853200, -0.171300),
+            (-0.492600, -0.853200, 0.171300),
+            (-0.853200, -0.492600, 0.171300),
+            (-0.492600, -0.853200, -0.171300),
+            (-0.853200, -0.492600, 0.171300),
+            (-0.853200, -0.492600, -0.171300),
+            (-0.326900, -0.566200, 0.756700),
+            (-0.181300, -0.313900, 0.932000),
+            (-0.313900, -0.181300, 0.932000),
+            (-0.326900, -0.566200, 0.756700),
+            (-0.313900, -0.181300, 0.932000),
+            (-0.566200, -0.326900, 0.756700),
+            (-0.566200, -0.326900, -0.756700),
+            (-0.753400, -0.435000, -0.493200),
+            (-0.869900, -0.000000, -0.493200),
+            (-0.566200, -0.326900, -0.756700),
+            (-0.869900, -0.000000, -0.493200),
+            (-0.653800, -0.000000, -0.756700),
+            (-0.853200, -0.492600, 0.171300),
+            (-0.753400, -0.435000, 0.493200),
+            (-0.869900, -0.000000, 0.493200),
+            (-0.853200, -0.492600, 0.171300),
+            (-0.869900, -0.000000, 0.493200),
+            (-0.985200, -0.000000, 0.171300),
+            (-0.313900, -0.181300, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (-0.362500, 0.000000, 0.932000),
+            (-0.313900, -0.181300, -0.932000),
+            (-0.566200, -0.326900, -0.756700),
+            (-0.653800, -0.000000, -0.756700),
+            (-0.313900, -0.181300, -0.932000),
+            (-0.653800, -0.000000, -0.756700),
+            (-0.362500, 0.000000, -0.932000),
+            (-0.853200, -0.492600, -0.171300),
+            (-0.853200, -0.492600, 0.171300),
+            (-0.985200, -0.000000, 0.171300),
+            (-0.853200, -0.492600, -0.171300),
+            (-0.985200, -0.000000, 0.171300),
+            (-0.985200, -0.000000, -0.171300),
+            (-0.566200, -0.326900, 0.756700),
+            (-0.313900, -0.181300, 0.932000),
+            (-0.362500, 0.000000, 0.932000),
+            (-0.566200, -0.326900, 0.756700),
+            (-0.362500, 0.000000, 0.932000),
+            (-0.653800, -0.000000, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (-0.313900, -0.181300, -0.932000),
+            (-0.362500, 0.000000, -0.932000),
+            (-0.753400, -0.435000, -0.493200),
+            (-0.853200, -0.492600, -0.171300),
+            (-0.985200, -0.000000, -0.171300),
+            (-0.753400, -0.435000, -0.493200),
+            (-0.985200, -0.000000, -0.171300),
+            (-0.869900, -0.000000, -0.493200),
+            (-0.753400, -0.435000, 0.493200),
+            (-0.566200, -0.326900, 0.756700),
+            (-0.653800, -0.000000, 0.756700),
+            (-0.753400, -0.435000, 0.493200),
+            (-0.653800, -0.000000, 0.756700),
+            (-0.869900, -0.000000, 0.493200),
+            (-0.985200, -0.000000, -0.171300),
+            (-0.985200, -0.000000, 0.171300),
+            (-0.853200, 0.492600, 0.171300),
+            (-0.985200, -0.000000, -0.171300),
+            (-0.853200, 0.492600, 0.171300),
+            (-0.853200, 0.492600, -0.171300),
+            (-0.653800, -0.000000, 0.756700),
+            (-0.362500, 0.000000, 0.932000),
+            (-0.313900, 0.181300, 0.932000),
+            (-0.653800, -0.000000, 0.756700),
+            (-0.313900, 0.181300, 0.932000),
+            (-0.566200, 0.326900, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (-0.362500, 0.000000, -0.932000),
+            (-0.313900, 0.181300, -0.932000),
+            (-0.869900, -0.000000, -0.493200),
+            (-0.985200, -0.000000, -0.171300),
+            (-0.853200, 0.492600, -0.171300),
+            (-0.869900, -0.000000, -0.493200),
+            (-0.853200, 0.492600, -0.171300),
+            (-0.753400, 0.435000, -0.493200),
+            (-0.869900, -0.000000, 0.493200),
+            (-0.653800, -0.000000, 0.756700),
+            (-0.566200, 0.326900, 0.756700),
+            (-0.869900, -0.000000, 0.493200),
+            (-0.566200, 0.326900, 0.756700),
+            (-0.753400, 0.435000, 0.493200),
+            (-0.653800, -0.000000, -0.756700),
+            (-0.869900, -0.000000, -0.493200),
+            (-0.753400, 0.435000, -0.493200),
+            (-0.653800, -0.000000, -0.756700),
+            (-0.753400, 0.435000, -0.493200),
+            (-0.566200, 0.326900, -0.756700),
+            (-0.985200, -0.000000, 0.171300),
+            (-0.869900, -0.000000, 0.493200),
+            (-0.753400, 0.435000, 0.493200),
+            (-0.985200, -0.000000, 0.171300),
+            (-0.753400, 0.435000, 0.493200),
+            (-0.853200, 0.492600, 0.171300),
+            (-0.362500, 0.000000, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (-0.313900, 0.181300, 0.932000),
+            (-0.362500, 0.000000, -0.932000),
+            (-0.653800, -0.000000, -0.756700),
+            (-0.566200, 0.326900, -0.756700),
+            (-0.362500, 0.000000, -0.932000),
+            (-0.566200, 0.326900, -0.756700),
+            (-0.313900, 0.181300, -0.932000),
+            (-0.753400, 0.435000, 0.493200),
+            (-0.566200, 0.326900, 0.756700),
+            (-0.326900, 0.566200, 0.756700),
+            (-0.753400, 0.435000, 0.493200),
+            (-0.326900, 0.566200, 0.756700),
+            (-0.435000, 0.753400, 0.493200),
+            (-0.566200, 0.326900, -0.756700),
+            (-0.753400, 0.435000, -0.493200),
+            (-0.435000, 0.753400, -0.493200),
+            (-0.566200, 0.326900, -0.756700),
+            (-0.435000, 0.753400, -0.493200),
+            (-0.326900, 0.566200, -0.756700),
+            (-0.853200, 0.492600, 0.171300),
+            (-0.753400, 0.435000, 0.493200),
+            (-0.435000, 0.753400, 0.493200),
+            (-0.853200, 0.492600, 0.171300),
+            (-0.435000, 0.753400, 0.493200),
+            (-0.492600, 0.853200, 0.171300),
+            (-0.313900, 0.181300, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (-0.181300, 0.313900, 0.932000),
+            (-0.313900, 0.181300, -0.932000),
+            (-0.566200, 0.326900, -0.756700),
+            (-0.326900, 0.566200, -0.756700),
+            (-0.313900, 0.181300, -0.932000),
+            (-0.326900, 0.566200, -0.756700),
+            (-0.181300, 0.313900, -0.932000),
+            (-0.853200, 0.492600, -0.171300),
+            (-0.853200, 0.492600, 0.171300),
+            (-0.492600, 0.853200, 0.171300),
+            (-0.853200, 0.492600, -0.171300),
+            (-0.492600, 0.853200, 0.171300),
+            (-0.492600, 0.853200, -0.171300),
+            (-0.566200, 0.326900, 0.756700),
+            (-0.313900, 0.181300, 0.932000),
+            (-0.181300, 0.313900, 0.932000),
+            (-0.566200, 0.326900, 0.756700),
+            (-0.181300, 0.313900, 0.932000),
+            (-0.326900, 0.566200, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (-0.313900, 0.181300, -0.932000),
+            (-0.181300, 0.313900, -0.932000),
+            (-0.753400, 0.435000, -0.493200),
+            (-0.853200, 0.492600, -0.171300),
+            (-0.492600, 0.853200, -0.171300),
+            (-0.753400, 0.435000, -0.493200),
+            (-0.492600, 0.853200, -0.171300),
+            (-0.435000, 0.753400, -0.493200),
+            (-0.181300, 0.313900, 0.932000),
+            (-0.000000, -0.000000, 1.000000),
+            (-0.000000, 0.362500, 0.932000),
+            (-0.181300, 0.313900, -0.932000),
+            (-0.326900, 0.566200, -0.756700),
+            (-0.000000, 0.653800, -0.756700),
+            (-0.181300, 0.313900, -0.932000),
+            (-0.000000, 0.653800, -0.756700),
+            (-0.000000, 0.362500, -0.932000),
+            (-0.492600, 0.853200, -0.171300),
+            (-0.492600, 0.853200, 0.171300),
+            (-0.000000, 0.985200, 0.171300),
+            (-0.492600, 0.853200, -0.171300),
+            (-0.000000, 0.985200, 0.171300),
+            (-0.000000, 0.985200, -0.171300),
+            (-0.326900, 0.566200, 0.756700),
+            (-0.181300, 0.313900, 0.932000),
+            (-0.000000, 0.362500, 0.932000),
+            (-0.326900, 0.566200, 0.756700),
+            (-0.000000, 0.362500, 0.932000),
+            (-0.000000, 0.653800, 0.756700),
+            (0.000000, -0.000000, -1.000000),
+            (-0.181300, 0.313900, -0.932000),
+            (-0.000000, 0.362500, -0.932000),
+            (-0.435000, 0.753400, -0.493200),
+            (-0.492600, 0.853200, -0.171300),
+            (-0.000000, 0.985200, -0.171300),
+            (-0.435000, 0.753400, -0.493200),
+            (-0.000000, 0.985200, -0.171300),
+            (-0.000000, 0.869900, -0.493200),
+            (-0.435000, 0.753400, 0.493200),
+            (-0.326900, 0.566200, 0.756700),
+            (-0.000000, 0.653800, 0.756700),
+            (-0.435000, 0.753400, 0.493200),
+            (-0.000000, 0.653800, 0.756700),
+            (0.000000, 0.869900, 0.493200),
+            (-0.326900, 0.566200, -0.756700),
+            (-0.435000, 0.753400, -0.493200),
+            (-0.000000, 0.869900, -0.493200),
+            (-0.326900, 0.566200, -0.756700),
+            (-0.000000, 0.869900, -0.493200),
+            (-0.000000, 0.653800, -0.756700),
+            (-0.492600, 0.853200, 0.171300),
+            (-0.435000, 0.753400, 0.493200),
+            (0.000000, 0.869900, 0.493200),
+            (-0.492600, 0.853200, 0.171300),
+            (0.000000, 0.869900, 0.493200),
+            (-0.000000, 0.985200, 0.171300),
+        )
+    )
+    _uvs: UVCoordinates = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (
+            (0.500144, 0.744995),
+            (0.500144, 0.876330),
+            (0.661251, 0.876330),
+            (0.500144, 0.744995),
+            (0.661251, 0.876330),
+            (0.717203, 0.744995),
+            (0.500144, 0.119997),
+            (0.500144, 0.251333),
+            (0.717203, 0.251333),
+            (0.500144, 0.119997),
+            (0.717203, 0.251333),
+            (0.661251, 0.119997),
+            (0.500144, 0.583887),
+            (0.500144, 0.744995),
+            (0.717203, 0.744995),
+            (0.500144, 0.583887),
+            (0.717203, 0.744995),
+            (0.746974, 0.583887),
+            (0.500144, 0.962054),
+            (0.500144, 0.991825),
+            (0.585867, 0.962054),
+            (0.500144, 0.034273),
+            (0.500144, 0.119997),
+            (0.661251, 0.119997),
+            (0.500144, 0.034273),
+            (0.661251, 0.119997),
+            (0.585867, 0.034273),
+            (0.500144, 0.412440),
+            (0.500144, 0.583887),
+            (0.746974, 0.583887),
+            (0.500144, 0.412440),
+            (0.746974, 0.583887),
+            (0.746974, 0.412440),
+            (0.500144, 0.876330),
+            (0.500144, 0.962054),
+            (0.585867, 0.962054),
+            (0.500144, 0.876330),
+            (0.585867, 0.962054),
+            (0.661251, 0.876330),
+            (0.500144, 0.004502),
+            (0.500144, 0.034273),
+            (0.585867, 0.034273),
+            (0.500144, 0.251333),
+            (0.500144, 0.412440),
+            (0.746974, 0.412440),
+            (0.500144, 0.251333),
+            (0.746974, 0.412440),
+            (0.717203, 0.251333),
+            (0.746974, 0.583887),
+            (0.717203, 0.744995),
+            (0.876102, 0.744995),
+            (0.746974, 0.583887),
+            (0.876102, 0.744995),
+            (0.927667, 0.583887),
+            (0.585867, 0.962054),
+            (0.500144, 0.991825),
+            (0.648621, 0.962054),
+            (0.585867, 0.034273),
+            (0.661251, 0.119997),
+            (0.779190, 0.119997),
+            (0.585867, 0.034273),
+            (0.779190, 0.119997),
+            (0.648621, 0.034274),
+            (0.746974, 0.412440),
+            (0.746974, 0.583887),
+            (0.927667, 0.583887),
+            (0.746974, 0.412440),
+            (0.927667, 0.583887),
+            (0.927667, 0.412440),
+            (0.661251, 0.876330),
+            (0.585867, 0.962054),
+            (0.648621, 0.962054),
+            (0.661251, 0.876330),
+            (0.648621, 0.962054),
+            (0.779190, 0.876330),
+            (0.500144, 0.004502),
+            (0.585867, 0.034273),
+            (0.648621, 0.034274),
+            (0.717203, 0.251333),
+            (0.746974, 0.412440),
+            (0.927667, 0.412440),
+            (0.717203, 0.251333),
+            (0.927667, 0.412440),
+            (0.876102, 0.251333),
+            (0.717203, 0.744995),
+            (0.661251, 0.876330),
+            (0.779190, 0.876330),
+            (0.717203, 0.744995),
+            (0.779190, 0.876330),
+            (0.876102, 0.744995),
+            (0.661251, 0.119997),
+            (0.717203, 0.251333),
+            (0.876102, 0.251333),
+            (0.661251, 0.119997),
+            (0.876102, 0.251333),
+            (0.779190, 0.119997),
+            (0.779190, 0.876330),
+            (0.648621, 0.962054),
+            (0.671590, 0.962054),
+            (0.779190, 0.876330),
+            (0.671590, 0.962054),
+            (0.822359, 0.876330),
+            (0.500144, 0.004502),
+            (0.648621, 0.034274),
+            (0.671590, 0.034274),
+            (0.876102, 0.251333),
+            (0.927667, 0.412440),
+            (0.993805, 0.412440),
+            (0.876102, 0.251333),
+            (0.993805, 0.412440),
+            (0.934262, 0.251333),
+            (0.876102, 0.744995),
+            (0.779190, 0.876330),
+            (0.822359, 0.876330),
+            (0.876102, 0.744995),
+            (0.822359, 0.876330),
+            (0.934262, 0.744995),
+            (0.779190, 0.119997),
+            (0.876102, 0.251333),
+            (0.934262, 0.251333),
+            (0.779190, 0.119997),
+            (0.934262, 0.251333),
+            (0.822359, 0.119997),
+            (0.927667, 0.583887),
+            (0.876102, 0.744995),
+            (0.934262, 0.744995),
+            (0.927667, 0.583887),
+            (0.934262, 0.744995),
+            (0.993805, 0.583887),
+            (0.648621, 0.962054),
+            (0.500144, 0.991825),
+            (0.671590, 0.962054),
+            (0.648621, 0.034274),
+            (0.779190, 0.119997),
+            (0.822359, 0.119997),
+            (0.648621, 0.034274),
+            (0.822359, 0.119997),
+            (0.671590, 0.034274),
+            (0.927667, 0.412440),
+            (0.927667, 0.583887),
+            (0.993805, 0.583887),
+            (0.927667, 0.412440),
+            (0.993805, 0.583887),
+            (0.993805, 0.412440),
+            (0.822359, 0.119997),
+            (0.934262, 0.251333),
+            (0.876102, 0.251333),
+            (0.822359, 0.119997),
+            (0.876102, 0.251333),
+            (0.779190, 0.119997),
+            (0.993805, 0.583887),
+            (0.934262, 0.744995),
+            (0.876102, 0.744995),
+            (0.993805, 0.583887),
+            (0.876102, 0.744995),
+            (0.927667, 0.583887),
+            (0.671590, 0.962054),
+            (0.500144, 0.991825),
+            (0.648621, 0.962054),
+            (0.671590, 0.034274),
+            (0.822359, 0.119997),
+            (0.779190, 0.119997),
+            (0.671590, 0.034274),
+            (0.779190, 0.119997),
+            (0.648621, 0.034274),
+            (0.993805, 0.412440),
+            (0.993805, 0.583887),
+            (0.927667, 0.583887),
+            (0.993805, 0.412440),
+            (0.927667, 0.583887),
+            (0.927667, 0.412440),
+            (0.822359, 0.876330),
+            (0.671590, 0.962054),
+            (0.648621, 0.962054),
+            (0.822359, 0.876330),
+            (0.648621, 0.962054),
+            (0.779190, 0.876330),
+            (0.500144, 0.004502),
+            (0.671590, 0.034274),
+            (0.648621, 0.034274),
+            (0.934262, 0.251333),
+            (0.993805, 0.412440),
+            (0.927667, 0.412440),
+            (0.934262, 0.251333),
+            (0.927667, 0.412440),
+            (0.876102, 0.251333),
+            (0.934262, 0.744995),
+            (0.822359, 0.876330),
+            (0.779190, 0.876330),
+            (0.934262, 0.744995),
+            (0.779190, 0.876330),
+            (0.876102, 0.744995),
+            (0.927667, 0.412440),
+            (0.927667, 0.583887),
+            (0.746974, 0.583887),
+            (0.927667, 0.412440),
+            (0.746974, 0.583887),
+            (0.746974, 0.412441),
+            (0.779190, 0.876330),
+            (0.648621, 0.962054),
+            (0.585867, 0.962054),
+            (0.779190, 0.876330),
+            (0.585867, 0.962054),
+            (0.661251, 0.876330),
+            (0.500144, 0.004502),
+            (0.648621, 0.034274),
+            (0.585867, 0.034274),
+            (0.876102, 0.251333),
+            (0.927667, 0.412440),
+            (0.746974, 0.412441),
+            (0.876102, 0.251333),
+            (0.746974, 0.412441),
+            (0.717203, 0.251333),
+            (0.876102, 0.744995),
+            (0.779190, 0.876330),
+            (0.661251, 0.876330),
+            (0.876102, 0.744995),
+            (0.661251, 0.876330),
+            (0.717203, 0.744995),
+            (0.779190, 0.119997),
+            (0.876102, 0.251333),
+            (0.717203, 0.251333),
+            (0.779190, 0.119997),
+            (0.717203, 0.251333),
+            (0.661251, 0.119997),
+            (0.927667, 0.583887),
+            (0.876102, 0.744995),
+            (0.717203, 0.744995),
+            (0.927667, 0.583887),
+            (0.717203, 0.744995),
+            (0.746974, 0.583887),
+            (0.648621, 0.962054),
+            (0.500144, 0.991825),
+            (0.585867, 0.962054),
+            (0.648621, 0.034274),
+            (0.779190, 0.119997),
+            (0.661251, 0.119997),
+            (0.648621, 0.034274),
+            (0.661251, 0.119997),
+            (0.585867, 0.034274),
+            (0.717203, 0.744995),
+            (0.661251, 0.876330),
+            (0.500144, 0.876330),
+            (0.717203, 0.744995),
+            (0.500144, 0.876330),
+            (0.500144, 0.744995),
+            (0.661251, 0.119997),
+            (0.717203, 0.251333),
+            (0.500144, 0.251333),
+            (0.661251, 0.119997),
+            (0.500144, 0.251333),
+            (0.500144, 0.119997),
+            (0.746974, 0.583887),
+            (0.717203, 0.744995),
+            (0.500144, 0.744995),
+            (0.746974, 0.583887),
+            (0.500144, 0.744995),
+            (0.500144, 0.583887),
+            (0.585867, 0.962054),
+            (0.500144, 0.991825),
+            (0.500144, 0.962054),
+            (0.585867, 0.034274),
+            (0.661251, 0.119997),
+            (0.500144, 0.119997),
+            (0.585867, 0.034274),
+            (0.500144, 0.119997),
+            (0.500144, 0.034274),
+            (0.746974, 0.412441),
+            (0.746974, 0.583887),
+            (0.500144, 0.583887),
+            (0.746974, 0.412441),
+            (0.500144, 0.583887),
+            (0.500144, 0.412441),
+            (0.661251, 0.876330),
+            (0.585867, 0.962054),
+            (0.500144, 0.962054),
+            (0.661251, 0.876330),
+            (0.500144, 0.962054),
+            (0.500144, 0.876330),
+            (0.500144, 0.004502),
+            (0.585867, 0.034274),
+            (0.500144, 0.034274),
+            (0.717203, 0.251333),
+            (0.746974, 0.412441),
+            (0.500144, 0.412441),
+            (0.717203, 0.251333),
+            (0.500144, 0.412441),
+            (0.500144, 0.251333),
+            (0.500144, 0.962054),
+            (0.500144, 0.991825),
+            (0.414420, 0.962054),
+            (0.500144, 0.034274),
+            (0.500144, 0.119997),
+            (0.339036, 0.119997),
+            (0.500144, 0.034274),
+            (0.339036, 0.119997),
+            (0.414420, 0.034274),
+            (0.500144, 0.412441),
+            (0.500144, 0.583887),
+            (0.253313, 0.583887),
+            (0.500144, 0.412441),
+            (0.253313, 0.583887),
+            (0.253313, 0.412441),
+            (0.500144, 0.876330),
+            (0.500144, 0.962054),
+            (0.414420, 0.962054),
+            (0.500144, 0.876330),
+            (0.414420, 0.962054),
+            (0.339036, 0.876330),
+            (0.500144, 0.004502),
+            (0.500144, 0.034274),
+            (0.414420, 0.034274),
+            (0.500144, 0.251333),
+            (0.500144, 0.412441),
+            (0.253313, 0.412441),
+            (0.500144, 0.251333),
+            (0.253313, 0.412441),
+            (0.283084, 0.251333),
+            (0.500144, 0.744995),
+            (0.500144, 0.876330),
+            (0.339036, 0.876330),
+            (0.500144, 0.744995),
+            (0.339036, 0.876330),
+            (0.283084, 0.744995),
+            (0.500144, 0.119997),
+            (0.500144, 0.251333),
+            (0.283084, 0.251333),
+            (0.500144, 0.119997),
+            (0.283084, 0.251333),
+            (0.339036, 0.119997),
+            (0.500144, 0.583887),
+            (0.500144, 0.744995),
+            (0.283084, 0.744995),
+            (0.500144, 0.583887),
+            (0.283084, 0.744995),
+            (0.253313, 0.583887),
+            (0.500144, 0.004502),
+            (0.414420, 0.034274),
+            (0.351667, 0.034274),
+            (0.283084, 0.251333),
+            (0.253313, 0.412441),
+            (0.072621, 0.412440),
+            (0.283084, 0.251333),
+            (0.072621, 0.412440),
+            (0.124186, 0.251333),
+            (0.283084, 0.744995),
+            (0.339036, 0.876330),
+            (0.221098, 0.876330),
+            (0.283084, 0.744995),
+            (0.221098, 0.876330),
+            (0.124186, 0.744995),
+            (0.339036, 0.119997),
+            (0.283084, 0.251333),
+            (0.124186, 0.251333),
+            (0.339036, 0.119997),
+            (0.124186, 0.251333),
+            (0.221098, 0.119997),
+            (0.253313, 0.583887),
+            (0.283084, 0.744995),
+            (0.124186, 0.744995),
+            (0.253313, 0.583887),
+            (0.124186, 0.744995),
+            (0.072621, 0.583887),
+            (0.414420, 0.962054),
+            (0.500144, 0.991825),
+            (0.351667, 0.962054),
+            (0.414420, 0.034274),
+            (0.339036, 0.119997),
+            (0.221098, 0.119997),
+            (0.414420, 0.034274),
+            (0.221098, 0.119997),
+            (0.351667, 0.034274),
+            (0.253313, 0.412441),
+            (0.253313, 0.583887),
+            (0.072621, 0.583887),
+            (0.253313, 0.412441),
+            (0.072621, 0.583887),
+            (0.072621, 0.412440),
+            (0.339036, 0.876330),
+            (0.414420, 0.962054),
+            (0.351667, 0.962054),
+            (0.339036, 0.876330),
+            (0.351667, 0.962054),
+            (0.221098, 0.876330),
+            (0.221098, 0.119997),
+            (0.124186, 0.251333),
+            (0.066025, 0.251333),
+            (0.221098, 0.119997),
+            (0.066025, 0.251333),
+            (0.177929, 0.119997),
+            (0.072621, 0.583887),
+            (0.124186, 0.744995),
+            (0.066025, 0.744995),
+            (0.072621, 0.583887),
+            (0.066025, 0.744995),
+            (0.006482, 0.583887),
+            (0.351667, 0.962054),
+            (0.500144, 0.991825),
+            (0.328697, 0.962054),
+            (0.351667, 0.034274),
+            (0.221098, 0.119997),
+            (0.177929, 0.119997),
+            (0.351667, 0.034274),
+            (0.177929, 0.119997),
+            (0.328697, 0.034274),
+            (0.072621, 0.412440),
+            (0.072621, 0.583887),
+            (0.006482, 0.583887),
+            (0.072621, 0.412440),
+            (0.006482, 0.583887),
+            (0.006482, 0.412440),
+            (0.221098, 0.876330),
+            (0.351667, 0.962054),
+            (0.328697, 0.962054),
+            (0.221098, 0.876330),
+            (0.328697, 0.962054),
+            (0.177929, 0.876330),
+            (0.500144, 0.004502),
+            (0.351667, 0.034274),
+            (0.328697, 0.034274),
+            (0.124186, 0.251333),
+            (0.072621, 0.412440),
+            (0.006482, 0.412440),
+            (0.124186, 0.251333),
+            (0.006482, 0.412440),
+            (0.066025, 0.251333),
+            (0.124186, 0.744995),
+            (0.221098, 0.876330),
+            (0.177929, 0.876330),
+            (0.124186, 0.744995),
+            (0.177929, 0.876330),
+            (0.066025, 0.744995),
+            (0.006482, 0.412440),
+            (0.006482, 0.583887),
+            (0.072621, 0.583887),
+            (0.006482, 0.412440),
+            (0.072621, 0.583887),
+            (0.072621, 0.412440),
+            (0.177929, 0.876330),
+            (0.328697, 0.962054),
+            (0.351667, 0.962054),
+            (0.177929, 0.876330),
+            (0.351667, 0.962054),
+            (0.221098, 0.876330),
+            (0.500144, 0.004502),
+            (0.328697, 0.034274),
+            (0.351667, 0.034274),
+            (0.066025, 0.251333),
+            (0.006482, 0.412440),
+            (0.072621, 0.412440),
+            (0.066025, 0.251333),
+            (0.072621, 0.412440),
+            (0.124186, 0.251333),
+            (0.066025, 0.744995),
+            (0.177929, 0.876330),
+            (0.221098, 0.876330),
+            (0.066025, 0.744995),
+            (0.221098, 0.876330),
+            (0.124186, 0.744995),
+            (0.177929, 0.119997),
+            (0.066025, 0.251333),
+            (0.124186, 0.251333),
+            (0.177929, 0.119997),
+            (0.124186, 0.251333),
+            (0.221098, 0.119997),
+            (0.006482, 0.583887),
+            (0.066025, 0.744995),
+            (0.124186, 0.744995),
+            (0.006482, 0.583887),
+            (0.124186, 0.744995),
+            (0.072621, 0.583887),
+            (0.328697, 0.962054),
+            (0.500144, 0.991825),
+            (0.351667, 0.962054),
+            (0.328697, 0.034274),
+            (0.177929, 0.119997),
+            (0.221098, 0.119997),
+            (0.328697, 0.034274),
+            (0.221098, 0.119997),
+            (0.351667, 0.034274),
+            (0.124186, 0.744995),
+            (0.221098, 0.876330),
+            (0.339036, 0.876330),
+            (0.124186, 0.744995),
+            (0.339036, 0.876330),
+            (0.283084, 0.744995),
+            (0.221098, 0.119997),
+            (0.124186, 0.251333),
+            (0.283084, 0.251333),
+            (0.221098, 0.119997),
+            (0.283084, 0.251333),
+            (0.339036, 0.119997),
+            (0.072621, 0.583887),
+            (0.124186, 0.744995),
+            (0.283084, 0.744995),
+            (0.072621, 0.583887),
+            (0.283084, 0.744995),
+            (0.253313, 0.583887),
+            (0.351667, 0.962054),
+            (0.500144, 0.991825),
+            (0.414420, 0.962054),
+            (0.351667, 0.034274),
+            (0.221098, 0.119997),
+            (0.339036, 0.119997),
+            (0.351667, 0.034274),
+            (0.339036, 0.119997),
+            (0.414420, 0.034273),
+            (0.072621, 0.412440),
+            (0.072621, 0.583887),
+            (0.253313, 0.583887),
+            (0.072621, 0.412440),
+            (0.253313, 0.583887),
+            (0.253313, 0.412440),
+            (0.221098, 0.876330),
+            (0.351667, 0.962054),
+            (0.414420, 0.962054),
+            (0.221098, 0.876330),
+            (0.414420, 0.962054),
+            (0.339036, 0.876330),
+            (0.500144, 0.004502),
+            (0.351667, 0.034274),
+            (0.414420, 0.034273),
+            (0.124186, 0.251333),
+            (0.072621, 0.412440),
+            (0.253313, 0.412440),
+            (0.124186, 0.251333),
+            (0.253313, 0.412440),
+            (0.283084, 0.251333),
+            (0.414420, 0.962054),
+            (0.500144, 0.991825),
+            (0.500144, 0.962054),
+            (0.414420, 0.034273),
+            (0.339036, 0.119997),
+            (0.500144, 0.119997),
+            (0.414420, 0.034273),
+            (0.500144, 0.119997),
+            (0.500144, 0.034273),
+            (0.253313, 0.412440),
+            (0.253313, 0.583887),
+            (0.500144, 0.583887),
+            (0.253313, 0.412440),
+            (0.500144, 0.583887),
+            (0.500144, 0.412440),
+            (0.339036, 0.876330),
+            (0.414420, 0.962054),
+            (0.500144, 0.962054),
+            (0.339036, 0.876330),
+            (0.500144, 0.962054),
+            (0.500144, 0.876330),
+            (0.500144, 0.004502),
+            (0.414420, 0.034273),
+            (0.500144, 0.034273),
+            (0.283084, 0.251333),
+            (0.253313, 0.412440),
+            (0.500144, 0.412440),
+            (0.283084, 0.251333),
+            (0.500144, 0.412440),
+            (0.500144, 0.251333),
+            (0.283084, 0.744995),
+            (0.339036, 0.876330),
+            (0.500144, 0.876330),
+            (0.283084, 0.744995),
+            (0.500144, 0.876330),
+            (0.500144, 0.744995),
+            (0.339036, 0.119997),
+            (0.283084, 0.251333),
+            (0.500144, 0.251333),
+            (0.339036, 0.119997),
+            (0.500144, 0.251333),
+            (0.500144, 0.119997),
+            (0.253313, 0.583887),
+            (0.283084, 0.744995),
+            (0.500144, 0.744995),
+            (0.253313, 0.583887),
+            (0.500144, 0.744995),
+            (0.500144, 0.583887),
+        )
+    )
+    _faces: FaceIndices = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (
+            (0, 1, 2),
+            (3, 4, 5),
+            (6, 7, 8),
+            (9, 10, 11),
+            (12, 13, 14),
+            (15, 16, 17),
+            (18, 19, 20),
+            (21, 22, 23),
+            (24, 25, 26),
+            (27, 28, 29),
+            (30, 31, 32),
+            (33, 34, 35),
+            (36, 37, 38),
+            (39, 40, 41),
+            (42, 43, 44),
+            (45, 46, 47),
+            (48, 49, 50),
+            (51, 52, 53),
+            (54, 55, 56),
+            (57, 58, 59),
+            (60, 61, 62),
+            (63, 64, 65),
+            (66, 67, 68),
+            (69, 70, 71),
+            (72, 73, 74),
+            (75, 76, 77),
+            (78, 79, 80),
+            (81, 82, 83),
+            (84, 85, 86),
+            (87, 88, 89),
+            (90, 91, 92),
+            (93, 94, 95),
+            (96, 97, 98),
+            (99, 100, 101),
+            (102, 103, 104),
+            (105, 106, 107),
+            (108, 109, 110),
+            (111, 112, 113),
+            (114, 115, 116),
+            (117, 118, 119),
+            (120, 121, 122),
+            (123, 124, 125),
+            (126, 127, 128),
+            (129, 130, 131),
+            (132, 133, 134),
+            (135, 136, 137),
+            (138, 139, 140),
+            (141, 142, 143),
+            (144, 145, 146),
+            (147, 148, 149),
+            (150, 151, 152),
+            (153, 154, 155),
+            (156, 157, 158),
+            (159, 160, 161),
+            (162, 163, 164),
+            (165, 166, 167),
+            (168, 169, 170),
+            (171, 172, 173),
+            (174, 175, 176),
+            (177, 178, 179),
+            (180, 181, 182),
+            (183, 184, 185),
+            (186, 187, 188),
+            (189, 190, 191),
+            (192, 193, 194),
+            (195, 196, 197),
+            (198, 199, 200),
+            (201, 202, 203),
+            (204, 205, 206),
+            (207, 208, 209),
+            (210, 211, 212),
+            (213, 214, 215),
+            (216, 217, 218),
+            (219, 220, 221),
+            (222, 223, 224),
+            (225, 226, 227),
+            (228, 229, 230),
+            (231, 232, 233),
+            (234, 235, 236),
+            (237, 238, 239),
+            (240, 241, 242),
+            (243, 244, 245),
+            (246, 247, 248),
+            (249, 250, 251),
+            (252, 253, 254),
+            (255, 256, 257),
+            (258, 259, 260),
+            (261, 262, 263),
+            (264, 265, 266),
+            (267, 268, 269),
+            (270, 271, 272),
+            (273, 274, 275),
+            (276, 277, 278),
+            (279, 280, 281),
+            (282, 283, 284),
+            (285, 286, 287),
+            (288, 289, 290),
+            (291, 292, 293),
+            (294, 295, 296),
+            (297, 298, 299),
+            (300, 301, 302),
+            (303, 304, 305),
+            (306, 307, 308),
+            (309, 310, 311),
+            (312, 313, 314),
+            (315, 316, 317),
+            (318, 319, 320),
+            (321, 322, 323),
+            (324, 325, 326),
+            (327, 328, 329),
+            (330, 331, 332),
+            (333, 334, 335),
+            (336, 337, 338),
+            (339, 340, 341),
+            (342, 343, 344),
+            (345, 346, 347),
+            (348, 349, 350),
+            (351, 352, 353),
+            (354, 355, 356),
+            (357, 358, 359),
+            (360, 361, 362),
+            (363, 364, 365),
+            (366, 367, 368),
+            (369, 370, 371),
+            (372, 373, 374),
+            (375, 376, 377),
+            (378, 379, 380),
+            (381, 382, 383),
+            (384, 385, 386),
+            (387, 388, 389),
+            (390, 391, 392),
+            (393, 394, 395),
+            (396, 397, 398),
+            (399, 400, 401),
+            (402, 403, 404),
+            (405, 406, 407),
+            (408, 409, 410),
+            (411, 412, 413),
+            (414, 415, 416),
+            (417, 418, 419),
+            (420, 421, 422),
+            (423, 424, 425),
+            (426, 427, 428),
+            (429, 430, 431),
+            (432, 433, 434),
+            (435, 436, 437),
+            (438, 439, 440),
+            (441, 442, 443),
+            (444, 445, 446),
+            (447, 448, 449),
+            (450, 451, 452),
+            (453, 454, 455),
+            (456, 457, 458),
+            (459, 460, 461),
+            (462, 463, 464),
+            (465, 466, 467),
+            (468, 469, 470),
+            (471, 472, 473),
+            (474, 475, 476),
+            (477, 478, 479),
+            (480, 481, 482),
+            (483, 484, 485),
+            (486, 487, 488),
+            (489, 490, 491),
+            (492, 493, 494),
+            (495, 496, 497),
+            (498, 499, 500),
+            (501, 502, 503),
+            (504, 505, 506),
+            (507, 508, 509),
+            (510, 511, 512),
+            (513, 514, 515),
+            (516, 517, 518),
+            (519, 520, 521),
+            (522, 523, 524),
+            (525, 526, 527),
+            (528, 529, 530),
+            (531, 532, 533),
+            (534, 535, 536),
+            (537, 538, 539),
+            (540, 541, 542),
+            (543, 544, 545),
+            (546, 547, 548),
+            (549, 550, 551),
+            (552, 553, 554),
+            (555, 556, 557),
+            (558, 559, 560),
+            (561, 562, 563),
+            (564, 565, 566),
+            (567, 568, 569),
+            (570, 571, 572),
+            (573, 574, 575),
+        )
+    )
 
 
 class UpAxis(enum.IntEnum):
     X = 0
     Y = 1
     Z = 2
 
 
 @jaxtyped
 def create_capsule(
-    radius: Float[Array, ""],
-    half_height: Float[Array, ""],
+    radius: FloatV,
+    half_height: FloatV,
     up_axis: UpAxis,
     diffuse_map: Texture,
     specular_map: SpecularMap,
 ) -> Model:
     """Create a capsule model.
 
     Parameters:
@@ -1962,27 +1977,31 @@
       - up_axis: The axis that points up
       - diffuse_map: The diffuse map.
       - specular_map: The specular map.
 
     Reference:
       - [create_capsule](https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/tinyrenderer.cpp#L914)
     """
-    shuffled: Integer[Array, "3"] = jnp.array((
-        (1, 2, 0),
-        (0, 1, 2),
-        (2, 0, 1),
-    ))[up_axis, :]
+    shuffled: Integer[Array, "3"]
+    shuffled = jnp.array(  # pyright: ignore[reportUnknownMemberType]
+        (
+            (1, 2, 0),
+            (0, 1, 2),
+            (2, 0, 1),
+        )
+    )[up_axis, :]
 
     verts: Vertices = _verts[:, shuffled] * radius
     verts = verts.at[:, up_axis].add(
-        jnp.where(
+        jnp.where(  # pyright: ignore[reportUnknownMemberType]
             verts[:, up_axis] > 0,
             half_height,
             -half_height,
-        ))
+        )
+    )
     assert isinstance(verts, Vertices)
 
     normals: Normals = _normals[:, shuffled]
     assert isinstance(normals, Normals)
 
     return Model(
         verts=verts,
```

### Comparing `jaxrenderer-0.3.1/renderer/types.py` & `jaxrenderer-0.3.2/renderer/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,64 @@
-from typing import Generic, TypeVar, Union
+from typing import Any, Generic, TypeVar, Union, cast
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Bool, Float, Integer, jaxtyped
+from jaxtyping import Array, Bool, Float, Integer, Num
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
-from ._backport import JaxFloating, JaxInteger, NamedTuple, TypeAlias
+from ._backport import JaxFloating, JaxInteger, NamedTuple, Tuple, Type, TypeAlias
 
-jax.config.update('jax_array', True)
-
-TRUE_ARRAY: Bool[Array, ""] = lax.full((), True, dtype=jnp.bool_)
-FALSE_ARRAY: Bool[Array, ""] = lax.full((), False, dtype=jnp.bool_)
-INF_ARRAY: Float[Array, ""] = lax.full((), jnp.inf)
+__all__ = [
+    "JaxFloating",
+    "JaxInteger",
+    "TRUE_ARRAY",
+    "FALSE_ARRAY",
+    "INF_ARRAY",
+    "Index",
+    "CanvasMask",
+    "BatchCanvasMask",
+    "Canvas",
+    "ZBuffer",
+    "Colour",
+    "Vec2i",
+    "Vec3i",
+    "Vec2f",
+    "Vec3f",
+    "Vec4f",
+    "Triangle2D",
+    "Triangle",
+    "TriangleBarycentric",
+    "FaceIndices",
+    "Vertices",
+    "Normals",
+    "UVCoordinates",
+    "Texture",
+    "SpecularMap",
+    "NormalMap",
+    "DtypeInfo",
+    "LightSource",
+    "Buffers",
+]
+
+jax.config.update("jax_array", True)  # pyright: ignore[reportUnknownMemberType]
+
+BoolV: TypeAlias = Bool[Array, ""]
+"""JAX Array with single bool value.""" ""
+FloatV: TypeAlias = Float[Array, ""]
+"""JAX Array with single float value."""
+IntV: TypeAlias = Integer[Array, ""]
+"""JAX Array with single int value.""" ""
+NumV: TypeAlias = Num[Array, ""]
+"""JAX Array with single num value.""" ""
+
+
+TRUE_ARRAY: BoolV = lax.full((), True, dtype=jnp.bool_)  # pyright: ignore
+FALSE_ARRAY: BoolV = lax.full((), False, dtype=jnp.bool_)  # pyright: ignore
+INF_ARRAY: FloatV = lax.full((), jnp.inf)  # pyright: ignore
 
 Index: TypeAlias = Integer[Array, ""]
 
 CanvasMask: TypeAlias = Bool[Array, "#width #height"]
 BatchCanvasMask: TypeAlias = Bool[Array, "#batch #width #height"]
 Canvas: TypeAlias = Float[Array, "width height channel"]
 ZBuffer: TypeAlias = Float[Array, "width height"]
@@ -42,64 +85,71 @@
 Vertices: TypeAlias = Float[Array, "vertices 3"]
 Normals: TypeAlias = Float[Array, "normals 3"]
 UVCoordinates: TypeAlias = Float[Array, "uv_counts 2"]
 Texture: TypeAlias = Float[Array, "textureWidth textureHeight channel"]
 SpecularMap: TypeAlias = Float[Array, "textureWidth textureHeight"]
 NormalMap: TypeAlias = Float[Array, "textureWidth textureHeight 3"]
 
-_DtypeT = TypeVar("_DtypeT", bound=Union[JaxFloating, JaxInteger])
+_DtypeT = TypeVar("_DtypeT", bound=Union[JaxFloating, JaxInteger, int])
 
 
 class DtypeInfo(NamedTuple, Generic[_DtypeT]):
     min: _DtypeT
     max: _DtypeT
     bits: int
-    dtype: type
+    dtype: Type
 
     @classmethod
     @jaxtyped
     # cannot be jitted as `dtype` will not be a valid JAX type
-    def create(cls, dtype: type) -> "DtypeInfo":
+    def create(cls, dtype: Type[_DtypeT]) -> "DtypeInfo[_DtypeT]":
         with jax.ensure_compile_time_eval():
-            if jnp.issubdtype(dtype, jnp.floating):
+            if jnp.issubdtype(dtype, jnp.floating):  # pyright: ignore
                 finfo = jnp.finfo(dtype)
 
                 return cls(
-                    min=finfo.min,
-                    max=finfo.max,
+                    min=cast(
+                        _DtypeT,
+                        finfo.min,  # pyright: ignore[reportUnknownMemberType]
+                    ),
+                    max=cast(
+                        _DtypeT,
+                        finfo.max,  # pyright: ignore[reportUnknownMemberType]
+                    ),
                     bits=finfo.bits,
                     dtype=dtype,
                 )
-            if jnp.issubdtype(dtype, jnp.integer):
+            if jnp.issubdtype(dtype, jnp.integer):  # pyright: ignore
                 iinfo = jnp.iinfo(dtype)
 
                 return cls(
-                    min=iinfo.min,
-                    max=iinfo.max,
+                    min=cast(_DtypeT, iinfo.min),
+                    max=cast(_DtypeT, iinfo.max),
                     bits=iinfo.bits,
                     dtype=dtype,
                 )
 
         raise ValueError(f"Unexpected dtype {dtype}")
 
 
 class LightSource(NamedTuple):
-    direction: Vec3f = jax.numpy.array((0., 0., -1.))
+    direction: Vec3f = jax.numpy.array((0.0, 0.0, -1.0))  # pyright: ignore
     """in world space, as it goes from that position to origin (camera).
 
     For example, if direction = camera's eye, full specular will be applied to
     triangles with normal towards camera.
     """
-    colour: Colour = jax.numpy.ones(3)
+    colour: Colour = jax.numpy.ones(3)  # pyright: ignore[reportUnknownMemberType]
 
 
-_TargetsT = TypeVar("_TargetsT", bound=tuple)
+_TargetsT = TypeVar("_TargetsT", bound=Tuple[Any, ...])
 """Extra target buffers, must be in shape of (width, height, ...)."""
 
 
 class Buffers(NamedTuple, Generic[_TargetsT]):
     """Use lax.full to create buffers and attach here.
 
     targets must be a tuple of arrays with shape of (width, height, ...).
     """
+
     zbuffer: ZBuffer
     targets: _TargetsT
```

### Comparing `jaxrenderer-0.3.1/renderer/utils.py` & `jaxrenderer-0.3.2/renderer/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,98 @@
 from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
 
 from functools import partial
-from typing import Sequence, Union
+from typing import Sequence, Union, cast
 
 import jax
-import jax.numpy as jnp
 from jax import lax
-from jaxtyping import Array, Integer, Num, Shaped, jaxtyped
+import jax.numpy as jnp
+from jaxtyping import Array, Integer, Num, Shaped
+from jaxtyping import jaxtyped  # pyright: ignore[reportUnknownVariableType]
 
+from ._backport import Tuple
 from ._meta_utils import add_tracing_name
-from .types import Canvas, Texture, ZBuffer
+from ._meta_utils import typed_jit as jit
+from .types import Canvas, IntV, Texture, ZBuffer
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def get_value_from_index(
     matrix: Shaped[Array, "width height batch *valueDimensions"],
     index: Integer[Array, "width height"],
 ) -> Shaped[Array, "width height *valueDimensions"]:
     """Retrieve value along 3rd axis using index value from index matrix."""
-    return jax.vmap(jax.vmap(lambda mt, ix: mt[ix]))(matrix, index)
+
+    def _get(
+        mt: Shaped[Array, "batch *valueDimensions"],
+        ix: IntV,
+    ) -> Shaped[Array, "*valueDimensions"]:
+        return mt[ix]
+
+    return jax.vmap(jax.vmap(_get))(matrix, index)
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(jit, inline=True)
 @add_tracing_name
 def merge_canvases(
     zbuffers: Num[Array, "batch width height"],
     canvases: Shaped[Array, "batch width height channel"],
-) -> tuple[ZBuffer, Canvas]:
+) -> Tuple[ZBuffer, Canvas]:
     """Merge canvases by selecting each pixel with max z value in zbuffer,
-        then merge zbuffer as well.
+    then merge zbuffer as well.
     """
-    pixel_idx: Integer[Array, "width height"] = jnp.argmax(zbuffers, axis=0)
+    pixel_idx: Integer[Array, "width height"]
+    pixel_idx = jnp.argmax(zbuffers, axis=0)  # pyright: ignore[reportUnknownMemberType]
     assert isinstance(pixel_idx, Integer[Array, "width height"])
 
     zbuffer: ZBuffer = get_value_from_index(
-        lax.transpose(zbuffers, (1, 2, 0)),
+        lax.transpose(  # pyright: ignore[reportUnknownMemberType]
+            zbuffers,
+            (1, 2, 0),
+        ),
         pixel_idx,
     )
     assert isinstance(zbuffer, ZBuffer)
 
     canvas: Canvas = get_value_from_index(
         # first vmap along width, then height, then choose among "faces"
-        lax.transpose(canvases, (1, 2, 0, 3)),
+        lax.transpose(  # pyright: ignore[reportUnknownMemberType]
+            canvases,
+            (1, 2, 0, 3),
+        ),
         pixel_idx,
     )
     assert isinstance(canvas, Canvas)
 
     return zbuffer, canvas
 
 
 @jaxtyped
-@partial(jax.jit, inline=True)
+@partial(
+    jit,
+    inline=True,
+    static_argnames=("flip_vertical",),
+)
 @add_tracing_name
 def transpose_for_display(
     matrix: Num[Array, "fst snd *channel"],
     flip_vertical: bool = True,
 ) -> Num[Array, "snd fst *channel"]:
     """Transpose matrix for display.
 
     When flip_vertical is disabled, the matrix's origin ([0, 0]) is assumed to
     be at bottom-left. Thus, the correct way to display the matrix is to using
     tools like matplotlib is to specify `origin="lower"`.
     To be compatible with PyTinyrenderer and most image processing programs,
-    the default behavior is to flip vertically.
+    the default behaviour is to flip vertically.
     """
-    mat = jnp.swapaxes(matrix, 0, 1)
+    mat = cast(Num[Array, "snd fst *channel"], jnp.swapaxes(matrix, 0, 1))
     assert isinstance(mat, Num[Array, "snd fst *channel"])
     if flip_vertical:
         mat = mat[::-1, ...]
 
     return mat
 
 
@@ -93,12 +114,12 @@
         the resulted texture still has 3 dimensions, with last dimension of
         side 1.
       - width: width of the texture.
       - height: height of the texture.
 
     Returns: A texture with shape `(width, height, channels)`.
     """
-    return jnp.reshape(
-        jnp.asarray(texture),
+    return jnp.reshape(  # pyright: ignore[reportUnknownMemberType]
+        jnp.asarray(texture),  # pyright: ignore[reportUnknownMemberType]
         (width, height, -1),
         order="C",
     ).swapaxes(0, 1)[:, ::-1, :]
```

