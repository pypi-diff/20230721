# Comparing `tmp/strangeworks_hybrid_optimize-0.1.2.tar.gz` & `tmp/strangeworks_hybrid_optimize-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_hybrid_optimize-0.1.2.tar", max compression
+gzip compressed data, was "strangeworks_hybrid_optimize-0.1.3.tar", max compression
```

## Comparing `strangeworks_hybrid_optimize-0.1.2.tar` & `strangeworks_hybrid_optimize-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       61 2023-07-18 12:53:25.808066 strangeworks_hybrid_optimize-0.1.2/README.md
--rw-r--r--   0        0        0      831 2023-07-18 12:53:43.847948 strangeworks_hybrid_optimize-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      346 2023-07-18 12:53:25.808066 strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/__init__.py
--rw-r--r--   0        0        0    23979 2023-07-18 12:53:25.808066 strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/sdk.py
--rw-r--r--   0        0        0    12428 2023-07-18 12:53:25.808066 strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/utils.py
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 strangeworks_hybrid_optimize-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-07-21 14:44:26.278407 strangeworks_hybrid_optimize-0.1.3/README.md
+-rw-r--r--   0        0        0      831 2023-07-21 14:44:46.251937 strangeworks_hybrid_optimize-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      346 2023-07-21 14:44:26.278407 strangeworks_hybrid_optimize-0.1.3/strangeworks_hybrid_optimize/__init__.py
+-rw-r--r--   0        0        0    24225 2023-07-21 14:44:26.278407 strangeworks_hybrid_optimize-0.1.3/strangeworks_hybrid_optimize/sdk.py
+-rw-r--r--   0        0        0    12428 2023-07-21 14:44:26.278407 strangeworks_hybrid_optimize-0.1.3/strangeworks_hybrid_optimize/utils.py
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 strangeworks_hybrid_optimize-0.1.3/PKG-INFO
```

### Comparing `strangeworks_hybrid_optimize-0.1.2/pyproject.toml` & `strangeworks_hybrid_optimize-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-hybrid-optimize"
-version = "0.1.2"
+version = "0.1.3"
 description = "Extension to strangeworks sdk to allow user to run the hybrid optimization service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_hybrid_optimize"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/sdk.py` & `strangeworks_hybrid_optimize-0.1.3/strangeworks_hybrid_optimize/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 class OptimizationParams:
     def __init__(
         self,
         solver: dict,
         bqm: Optional[BinaryQuadraticModel] | None = None,
         var_type: Optional[str] = "BINARY",
         lagrange_multiplier: Optional[float] = 0.0,
+        resource_slug: Optional[str] = "",
     ) -> None:
         self.bqm = json.dumps(bqm.to_serializable()) if bqm else None
         self.var_type = var_type
         self.lagrange_multiplier = lagrange_multiplier
         self.solver = solver
+        self.resource_slug = resource_slug
 
 
 class QAOAParams:
     def __init__(
         self,
         maxiter: int,
         shotsin: int,
@@ -467,36 +469,43 @@
                 "product_slug": self.sub_rsc.product.slug,
             }
 
         sw_job = strangeworks.execute(self.rsc, input_params, "run_hybrid_job")
 
         return sw_job
 
-    def get_job(self, sw_job):
+    def update_status(self, sw_job):
         if type(sw_job) is dict:
             job_slug = sw_job.get("slug")
         elif type(sw_job) is str:
             job_slug = sw_job
         else:
             job_slug = sw_job.slug
 
-        status = strangeworks.execute(self.rsc, {"job_slug": job_slug}, "status")
+        sw_job = strangeworks.execute(self.rsc, {"job_slug": job_slug}, "status")
+
+        if sw_job.get("status") == "QUEUED":
+            sw_job = strangeworks.execute(
+                self.rsc, {"job_slug": job_slug}, "status_subjobs"
+            )
+            strangeworks.execute(self.rsc, {"job_slug": job_slug}, "run_final_job")
+
+        return sw_job
+
+    def get_job(self, sw_job):
+        if type(sw_job) is dict:
+            job_slug = sw_job.get("slug")
+        elif type(sw_job) is str:
+            job_slug = sw_job
+        else:
+            job_slug = sw_job.slug
 
-        # from strangeworks.core.client.jobs import Job
+        sw_job = strangeworks.jobs(slug=job_slug)[0]
 
-        # status["resource"] = {"slug": self.rsc.slug, }
-        # Resource(
-        #     slug=d.get("slug"),
-        #     status=d.get("status"),
-        #     name=d.get("name"),
-        #     product=Product.from_dict(d.get("product")),
-        #     is_deleted=d.get("isDeleted"),
-        # )
-        # sw_job = Job.from_dict(status)
-        return status
+        return sw_job
 
     def get_results(self, sw_job, calculate_exact_sol=False, display_results=False):
         if type(sw_job) is dict:
             job_slug = sw_job.get("slug")
             sw_job = sw_job = strangeworks.jobs(slug=job_slug)[0]
         elif type(sw_job) is str:
             job_slug = sw_job
```

### Comparing `strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/utils.py` & `strangeworks_hybrid_optimize-0.1.3/strangeworks_hybrid_optimize/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_hybrid_optimize-0.1.2/PKG-INFO` & `strangeworks_hybrid_optimize-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-hybrid-optimize
-Version: 0.1.2
+Version: 0.1.3
 Summary: Extension to strangeworks sdk to allow user to run the hybrid optimization service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

