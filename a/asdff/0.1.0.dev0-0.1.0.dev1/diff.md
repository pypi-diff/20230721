# Comparing `tmp/asdff-0.1.0.dev0.tar.gz` & `tmp/asdff-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asdff-0.1.0.dev0.tar", last modified: Fri Jul 21 08:46:40 2023, max compression
+gzip compressed data, was "asdff-0.1.0.dev1.tar", last modified: Fri Jul 21 13:22:07 2023, max compression
```

## Comparing `asdff-0.1.0.dev0.tar` & `asdff-0.1.0.dev1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    35184 2023-07-21 04:16:34.042881 asdff-0.1.0.dev0/LICENSE
--rw-r--r--   0        0        0      421 2023-07-21 08:46:07.512012 asdff-0.1.0.dev0/README.md
--rw-r--r--   0        0        0      123 2023-07-21 08:46:00.102334 asdff-0.1.0.dev0/asdff/__init__.py
--rw-r--r--   0        0        0       28 2023-07-21 04:29:00.961179 asdff-0.1.0.dev0/asdff/__version__.py
--rw-r--r--   0        0        0     6155 2023-07-21 08:43:19.869013 asdff-0.1.0.dev0/asdff/sd.py
--rw-r--r--   0        0        0     1988 2023-07-21 07:15:29.320339 asdff-0.1.0.dev0/asdff/yolo.py
--rw-r--r--   0        0        0      922 2023-07-21 08:46:40.849669 asdff-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 asdff-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0    35184 2023-07-21 04:16:34.042881 asdff-0.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0     3426 2023-07-21 12:55:26.798856 asdff-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0      178 2023-07-21 10:43:29.239300 asdff-0.1.0.dev1/asdff/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-21 12:29:43.262234 asdff-0.1.0.dev1/asdff/__version__.py
+-rw-r--r--   0        0        0     4282 2023-07-21 12:50:03.383098 asdff-0.1.0.dev1/asdff/sd.py
+-rw-r--r--   0        0        0     1810 2023-07-21 12:51:58.465683 asdff-0.1.0.dev1/asdff/utils.py
+-rw-r--r--   0        0        0     1993 2023-07-21 10:42:31.234547 asdff-0.1.0.dev1/asdff/yolo.py
+-rw-r--r--   0        0        0      922 2023-07-21 13:22:07.570435 asdff-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 asdff-0.1.0.dev1/PKG-INFO
```

### Comparing `asdff-0.1.0.dev0/LICENSE` & `asdff-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `asdff-0.1.0.dev0/asdff/sd.py` & `asdff-0.1.0.dev1/asdff/sd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from __future__ import annotations
 
-from functools import cached_property, partial
-from typing import Any, Callable
+from functools import cached_property
+from typing import Any, Callable, Iterable, List, Optional
 
-import cv2
-import numpy as np
 from diffusers import StableDiffusionInpaintPipeline, StableDiffusionPipeline
-from diffusers.pipelines.stable_diffusion import StableDiffusionPipelineOutput
 from diffusers.utils import logging
-from PIL import Image, ImageChops
+from PIL import Image
 
+from asdff.utils import (
+    ADOutput,
+    bbox_padding,
+    composite,
+    mask_dilate,
+    mask_gaussian_blur,
+)
 from asdff.yolo import yolo_detector
 
 logger = logging.get_logger("diffusers")
 
 
+DetectorType = Callable[[Image.Image], Optional[List[Image.Image]]]
+
+
 def ordinal(n: int) -> str:
     d = {1: "st", 2: "nd", 3: "rd"}
     return str(n) + ("th" if 11 <= n % 100 <= 13 else d.get(n % 10, "th"))
 
 
 class AdPipeline(StableDiffusionPipeline):
     @cached_property
@@ -27,132 +34,89 @@
             vae=self.vae,
             text_encoder=self.text_encoder,
             tokenizer=self.tokenizer,
             unet=self.unet,
             scheduler=self.scheduler,
             safety_checker=self.safety_checker,
             feature_extractor=self.feature_extractor,
-            requires_safety_checker=self.requires_safety_checker,
+            requires_safety_checker=self.config.requires_safety_checker,
         )
 
-    def __call__(
+    def __call__(  # noqa: C901
         self,
         common: dict[str, Any] | None = None,
         txt2img_only: dict[str, Any] | None = None,
         inpaint_only: dict[str, Any] | None = None,
-        detector: Callable[[Image.Image], list[Image.Image] | None] | None = None,
-        detector_kwargs: dict[str, Any] | None = None,
+        detectors: DetectorType | Iterable[DetectorType] | None = None,
         mask_dilation: int = 4,
+        mask_blur: int = 4,
         mask_padding: int = 32,
     ):
-        """
-        Call method for the StableDiffusionPipeline class.
-
-        Parameters
-        ----------
-            common (dict[str, Any] | None, optional): Common parameters for the pipeline. Defaults to None.
-            txt2img_only (dict[str, Any] | None, optional): Parameters for the txt2img step. Defaults to None.
-            inpaint_only (dict[str, Any] | None, optional): Parameters for the inpaint step. Defaults to None.
-            detector (Callable[[Image.Image], list[Image.Image] | None] | None, optional): Object detection function. Defaults to None.
-            detector_kwargs (dict[str, Any] | None, optional): Parameters for the object detection function. Defaults to None.
-            mask_dilation (int, optional): Dilation factor for the object mask. Defaults to 4.
-            mask_padding (int, optional): Padding size for the object mask. Defaults to 32.
-        Returns
-        -------
-            StableDiffusionPipelineOutput: Output of the StableDiffusionPipeline class.
-        """
         if common is None:
             common = {}
         if txt2img_only is None:
             txt2img_only = {}
         if inpaint_only is None:
             inpaint_only = {}
         inpaint_only.setdefault("strength", 0.4)
-        if detector_kwargs is None:
-            detector_kwargs = {}
-        if detector is None:
-            detector = partial(self.default_detector, **detector_kwargs)
-        else:
-            detector = partial(detector, **detector_kwargs)
 
-        txt2img_output = StableDiffusionPipeline.__call__(
-            self, **common, **txt2img_only, output_type="pil"
-        )
+        if detectors is None:
+            detectors = [self.default_detector]
+        elif callable(detectors):
+            detectors = [detectors]
+
+        txt2img_output = super().__call__(**common, **txt2img_only, output_type="pil")
         txt2img_images: list[Image.Image] = txt2img_output[0]
 
-        result_images = []
+        init_images = []
+        final_images = []
 
-        for i, txt2img_image in enumerate(txt2img_images):
-            masks = detector(txt2img_image)
-            if masks is None:
-                logger.info(f"No object detected on {ordinal(i + 1)} image.")
-                continue
-
-            for _j, mask in enumerate(masks):
-                mask = mask.convert("L")
-                mask = self.mask_dilate(mask, mask_dilation)
-                bbox = mask.getbbox()
-                if bbox is None:
-                    # Never happens
+        for i, init_image in enumerate(txt2img_images):
+            init_images.append(init_image.copy())
+            final_image = None
+
+            for j, detector in enumerate(detectors):
+                masks = detector(init_image)
+                if masks is None:
+                    logger.info(
+                        f"No object detected on {ordinal(i + 1)} image with {ordinal(j + 1)} detector."
+                    )
                     continue
-                bbox_padded = self.bbox_padding(bbox, txt2img_image.size, mask_padding)
 
-                img_masked = Image.new("RGBa", txt2img_image.size)
-                img_masked.paste(
-                    txt2img_image.convert("RGBA").convert("RGBa"),
-                    mask=ImageChops.invert(mask),
-                )
-                img_masked = img_masked.convert("RGBA")
-
-                crop_image = txt2img_image.crop(bbox_padded)
-                crop_mask = mask.crop(bbox_padded)
-
-                inpaint_output = self.inpaine_pipeline(
-                    **common,
-                    **inpaint_only,
-                    image=crop_image,
-                    mask_image=crop_mask,
-                    num_images_per_prompt=1,
-                    output_type="pil",
-                )
-                inpaint_image: Image.Image = inpaint_output[0][0]
-                resize = (
-                    bbox_padded[2] - bbox_padded[0],
-                    bbox_padded[3] - bbox_padded[1],
-                )
-                resized = inpaint_image.resize(resize)
-
-                result_img = Image.new("RGBA", txt2img_image.size)
-                result_img.paste(resized, bbox_padded)
-                result_img.alpha_composite(img_masked)
-                result_images.append(result_img.convert("RGB"))
+                for k, mask in enumerate(masks):
+                    mask = mask.convert("L")
+                    mask = mask_dilate(mask, mask_dilation)
+                    bbox = mask.getbbox()
+                    if bbox is None:
+                        logger.info(f"No object in {ordinal(k + 1)} mask.")
+                        continue
+                    mask = mask_gaussian_blur(mask, mask_blur)
+                    bbox_padded = bbox_padding(bbox, init_image.size, mask_padding)
+
+                    crop_image = init_image.crop(bbox_padded)
+                    crop_mask = mask.crop(bbox_padded)
+
+                    inpaint_output = self.inpaine_pipeline(
+                        **common,
+                        **inpaint_only,
+                        image=crop_image,
+                        mask_image=crop_mask,
+                        num_images_per_prompt=1,
+                        output_type="pil",
+                    )
+                    inpaint_image: Image.Image = inpaint_output[0][0]
+                    final_image = composite(
+                        init=init_image,
+                        mask=mask,
+                        gen=inpaint_image,
+                        bbox_padded=bbox_padded,
+                    )
+                    init_image = final_image
 
-        return StableDiffusionPipelineOutput(
-            images=result_images, nsfw_content_detected=None
-        )
+            if final_image is not None:
+                final_images.append(final_image)
+
+        return ADOutput(images=final_images, init_images=init_images)
 
     @property
     def default_detector(self) -> Callable[..., list[Image.Image] | None]:
         return yolo_detector
-
-    @staticmethod
-    def mask_dilate(image: Image.Image, value: int = 4) -> Image.Image:
-        if value <= 0:
-            return image
-
-        arr = np.array(image)
-        kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (value, value))
-        dilated = cv2.dilate(arr, kernel, iterations=1)
-        return Image.fromarray(dilated)
-
-    @staticmethod
-    def bbox_padding(
-        bbox: tuple[int, int, int, int], image_size: tuple[int, int], value: int = 32
-    ) -> tuple[int, int, int, int]:
-        if value <= 0:
-            return bbox
-
-        arr = np.array(bbox).reshape(2, 2)
-        arr[0] -= value
-        arr[1] += value
-        arr = np.clip(arr, (0, 0), image_size)
-        return tuple(arr.flatten())
```

### Comparing `asdff-0.1.0.dev0/asdff/yolo.py` & `asdff-0.1.0.dev1/asdff/yolo.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,10 +64,10 @@
     bboxes = pred[0].boxes.xyxy.cpu().numpy()
     if bboxes.size == 0:
         return None
 
     if pred[0].masks is None:
         masks = create_mask_from_bbox(bboxes, image.size)
     else:
-        masks = mask_to_pil(pred[0].masks, image.size)
+        masks = mask_to_pil(pred[0].masks.data, image.size)
 
     return masks
```

### Comparing `asdff-0.1.0.dev0/pyproject.toml` & `asdff-0.1.0.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "diffusers[torch]>=0.18.2",
     "transformers>=4.25.1",
     "ultralytics",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
-version = "0.1.0.dev0"
+version = "0.1.0.dev1"
 
 [project.license]
 text = "AGPL-3.0"
 
 [project.urls]
 repository = "https://github.com/Bing-su/asdff"
```

