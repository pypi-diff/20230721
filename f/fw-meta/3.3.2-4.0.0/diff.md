# Comparing `tmp/fw_meta-3.3.2-py3-none-any.whl.zip` & `tmp/fw_meta-4.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14270 bytes, number of entries: 9
+Zip file size: 15483 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 fw_meta/__init__.py
--rw-r--r--  2.0 unx      631 b- defN 80-Jan-01 00:00 fw_meta/aliases.py
+-rw-r--r--  2.0 unx      665 b- defN 80-Jan-01 00:00 fw_meta/aliases.py
 -rw-r--r--  2.0 unx     7720 b- defN 80-Jan-01 00:00 fw_meta/exports.py
--rw-r--r--  2.0 unx    20553 b- defN 80-Jan-01 00:00 fw_meta/imports.py
+-rw-r--r--  2.0 unx    25025 b- defN 80-Jan-01 00:00 fw_meta/imports.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_meta/py.typed
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-3.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    10028 b- defN 80-Jan-01 00:00 fw_meta-3.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-3.3.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx      665 b- defN 16-Jan-01 00:00 fw_meta-3.3.2.dist-info/RECORD
-9 files, 41149 bytes uncompressed, 13142 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-4.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9983 b- defN 80-Jan-01 00:00 fw_meta-4.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-4.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      664 b- defN 16-Jan-01 00:00 fw_meta-4.0.0.dist-info/RECORD
+9 files, 45609 bytes uncompressed, 14355 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: fw_meta/imports.py
 Comment: 
 
 Filename: fw_meta/py.typed
 Comment: 
 
-Filename: fw_meta-3.3.2.dist-info/LICENSE
+Filename: fw_meta-4.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: fw_meta-3.3.2.dist-info/METADATA
+Filename: fw_meta-4.0.0.dist-info/METADATA
 Comment: 
 
-Filename: fw_meta-3.3.2.dist-info/WHEEL
+Filename: fw_meta-4.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: fw_meta-3.3.2.dist-info/RECORD
+Filename: fw_meta-4.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_meta/aliases.py

```diff
@@ -10,11 +10,12 @@
     r"^acq?(?=\.|$)": "acquisition",
     r"^group$": "group._id",
     r"^project$": "project.label",
     r"^subject$": "subject.label",
     r"^session$": "session.label",
     r"^acquisition$": "acquisition.label",
     r"^timestamp$": "acquisition.timestamp",
+    r".(time|ts)$": ".timestamp",
     r"^file$": "file.name",
     r"^info(?=\.|$)": "file.info",
     r"^classification(?=\.|$)": "file.classification",
 }
```

## fw_meta/imports.py

```diff
@@ -1,34 +1,61 @@
 """Flywheel import metadata extraction fields and utilities."""
 # check out the core-api input validation regexes for field loading context:
 # https://gitlab.com/flywheel-io/product/backend/core-api/-/blob/master/core/models/regex.py
 import enum
 import json
 import re
+import string
 import typing as t
 from collections import defaultdict
-from functools import cached_property
 from pathlib import Path
 
 import fw_utils
-import pathvalidate
+from dateutil.tz import gettz
 from fw_utils import AttrDict, Pattern, Template, get_field, parse_field_name
 from pydantic import BaseModel, Field, PrivateAttr, root_validator
 
 from .aliases import ALIASES
 
 __all__ = ["MetaData", "MetaExtractor", "extract_meta"]
 
 
 class MetaData(dict):
     """Flywheel metadata dict with sorted/validated keys and attr access."""
 
-    def __setitem__(self, name: str, value) -> None:
-        """Validate/canonize field names before setting keys."""
-        super().__setitem__(validate_import_field(name)[0], value)
+    def __init__(self, *args, **kw) -> None:
+        """Initialize a new MetaData dict."""
+        super().__init__()
+        self.update(*args, **kw)
+
+    def update(self, *args, **kw) -> None:
+        """Update MetaData dict from another dict or kwargs."""
+        for field, value in dict(*args, **kw).items():
+            self[field] = value
+
+    def setdefault(self, field, value):
+        """Set metadata field value if not set yet."""
+        if value in ("", None):
+            return
+        field, value = load_field_tuple(field, value)
+        if not self.get(field):
+            self[field] = value
+        return value
+
+    def __setitem__(self, field, value) -> None:
+        """Validate/canonize field names and validate/normalize values."""
+        if value in ("", None):
+            return  # pragma: no cover
+        field, value = load_field_tuple(field, value)
+        if field in ("session.timestamp", "acquisition.timestamp"):
+            tz_key = field.replace("timestamp", "timezone")
+            tz_val = getattr(value.tzinfo, "key", value.tzname())
+            super().__setitem__(tz_key, tz_val)
+            value = value.isoformat(timespec="milliseconds")
+        super().__setitem__(field, value)
 
     def __getattr__(self, name: str):
         """Return dictionary keys as attributes."""
         return getattr(self.dict, name)
 
     def __iter__(self):
         """Return dict key iterator respecting the hierarchy/field order."""
@@ -54,15 +81,15 @@
     @property
     def dict(self) -> AttrDict:
         """Return inflated metadata dict ready for Flywheel uploads."""
         return AttrDict.from_flat(self)
 
     @property
     def json(self) -> bytes:
-        """Return JSON dump of the inflated meta."""
+        """Return JSON dump of the inflated/nested metadata."""
         return json.dumps(self.dict, separators=(",", ":")).encode()
 
 
 Mappings = t.Union[str, t.List[t.Union[t.Tuple[str, str], str]], t.Dict[str, str]]
 
 
 class MetaExtractor:
@@ -70,108 +97,110 @@
 
     def __init__(
         self,
         *,
         mappings: Mappings = None,
         defaults: Mappings = None,
         overrides: Mappings = None,
-        customize: t.Callable[[dict, dict], None] = None,
     ) -> None:
-        """Validate, compile and (functools)cache metadata extraction mapping patterns."""
-        # load/validate mapping patterns
-        # TODO allow mapping expressions in reverse order
-        # be aware of file.path and (fileinfo.)path conflict
-        self.mappings = [
-            (ImportTemplate(t), ImportPattern(p))
-            for t, p in parse_metadata_mappings(mappings or [])
-        ]
-        # validate default fields and values
+        """Validate, compile and cache metadata extraction templates & patterns."""
+        self.src_fields: t.Set[str] = set()
+        self.dst_fields: t.Set[str] = set()
+        self.mappings = []
+        for mapping in parse_metadata_mappings(mappings or []):
+            src_tpl, dst_pat = validate_metadata_mapping(mapping)
+            for field in sorted(src_tpl.fields):
+                if not field.startswith("!"):
+                    self.src_fields.add(field)
+                elif field[1:] not in self.dst_fields:  # pragma: no cover
+                    msg = f"cannot reference {field} before assignment"
+                    raise ValueError(msg)
+            self.dst_fields.update(dst_pat.fields)
+            self.mappings.append((src_tpl, dst_pat))
+
+        # NOTE use case for defaults and overrides came from reapers
+        # imports are tied to a project, so CLI doesn't expose them
+        # TODO gather current use cases and reimplement defaults/overrides:
+        # - D mapping-based extractions and literals *after* type/path-defaults
+        # - D !metaref capability *after* type/path-defaults
+        # - O for incrementally / minimally changing previous behavior
+        # early proposal:
+        # - support templates/patterns in defaults (literals vs validation?)
+        # - drop overrides for simplicity (use-case not strong enough)
         self.defaults = dict(
             load_field_tuple(field, default)
             for field, default in parse_metadata_mappings(defaults or [])
         )
-        # validate override fields and values
+        # validate override fields and literal values
         self.overrides = dict(
             load_field_tuple(field, override)
             for field, override in parse_metadata_mappings(overrides or [])
         )
-        self.customize = customize
 
-    @cached_property
-    def fields(self) -> t.Set[str]:
-        """Return set of fields appear in the mappings/defaults/overrides."""
-        return set().union(
-            self.defaults.keys(),
-            self.overrides.keys(),
-            *[p.fields for _, p in self.mappings],
-        )
-
-    def extract(self, data: t.Any) -> MetaData:
-        """Extract metadata from given dict like object."""
-        meta: t.Dict[str, t.Any] = {}
+    def extract(self, obj) -> MetaData:
+        """Extract metadata from given object's attrs or keys."""
+        meta = MetaData()
 
         def get(field):
             if field.startswith("!"):
                 return get_field(meta, field[1:])
-            return get_field(data, field)
-
-        def setdefault(field, value):
-            if value not in ("", None):
-                field, value = load_field_tuple(field, value)
-                meta.setdefault(field, value)
+            return get_field(obj, field)
 
+        # apply user-defined metadata mappings
         for template, pattern in self.mappings:
             ctx = {field: get(field) for field in template.fields}
-            # skip if data doesn't have a value for one or more fields
+            # skip if data doesn't have a value for any of the template fields
             if any(value in ("", None) for value in ctx.values()):
                 continue
             # format the template, then parse with the pattern
             for field, value in pattern.match(template.format(ctx)).to_flat().items():
                 # setdefault allows using multiple patterns as fallback
-                setdefault(field, value)
+                meta.setdefault(field, value)
+        # apply type-defaults (eg. {'acquisition.label': <SeriesDescription>})
+        get_meta = get("get_meta")  # fw-file integration
+        type_meta = get_meta() if get_meta else {}
+        for field, type_default in type_meta.items():
+            if field == "file.name":
+                continue  # pragma: no cover
+            meta.setdefault(field, type_default)
+        # apply path-defaults (eg. {'acquisition.label': <parent dir name>})
+        path = get("path") or ""
+        path_fields = ["file.name", "acquisition", "session", "subject"]
+        for field, path_default in zip(path_fields, reversed(path.split("/"))):
+            if field == "file.name":
+                continue
+            meta.setdefault(field, path_default)
+        # NOTE defaults and overrides are not officially exposed
         # apply user-defaults (eg. {'project.label': 'Default Project'})
         for field, user_default in self.defaults.items():
-            setdefault(field, user_default)
-        # apply file-defaults (eg. {'session.label': 'StudyDescription'})
-        default_meta: dict = getattr(data, "get_default_meta", lambda: {})()
-        for field, file_default in default_meta.items():
-            setdefault(field, file_default)
+            meta.setdefault(field, user_default)
         # apply user-overrides (eg. {'project.label': 'Override Project'})
         for field, user_override in self.overrides.items():
             meta[field] = user_override
-        # set timezone if timestamp present
-        for prefix in ("session", "acquisition"):
-            ts_field, tz_field = f"{prefix}.timestamp", f"{prefix}.timezone"
-            dt = meta.get(ts_field)
-            if dt:
-                meta[ts_field] = dt.isoformat(timespec="milliseconds")
-                meta[tz_field] = getattr(dt.tzinfo, "key", dt.tzname())
-        # trigger user-callback if given for further meta customization
-        if self.customize is not None:
-            self.customize(data, meta)
-        return MetaData(meta)
+        # consider adding single/zipped/member name candidates
+        # pop file.name -> == singe name candidate
+        # finally return the meta
+        return meta
 
 
 def extract_meta(
-    data: t.Any,
+    obj,
     *,
     mappings: Mappings = None,
     defaults: Mappings = None,
     overrides: Mappings = None,
-    customize: t.Callable[[dict, dict], None] = None,
 ) -> MetaData:
     """Extract Flywheel metadata from a dict like object."""
     # NOTE using the class enables validation and caching
     meta_extractor = MetaExtractor(
         mappings=mappings,
         defaults=defaults,
         overrides=overrides,
-        customize=customize,
     )
-    return meta_extractor.extract(data)
+    return meta_extractor.extract(obj)
 
 
 def load_group_id(value: str) -> t.Optional[str]:
     """Normalize to lowercase and return validated value (or None)."""
     group_id = value.lower()
     if re.match(r"^[0-9a-z][0-9a-z.@_-]{0,62}[0-9a-z]$", group_id):
         return group_id
@@ -182,58 +211,70 @@
     """Normalize to lowercase and return validated value (or None)."""
     cont_id = value.lower()
     if re.match(r"^[0-9a-f]{24}$", cont_id):
         return cont_id
     return None
 
 
-def load_cont_label(value: str, trunc: int = 64) -> str:
-    """Normalize for path compatibility as core would and truncate if needed."""
-    label = value.replace("*", "star")  # retain T2* MR context
-    label = str(pathvalidate.sanitize_filename(label, replacement_text="_"))
-    return label[:trunc] if trunc else label
+def load_cont_label(value: str) -> str:
+    """Sanitize for path compatibility and truncate to 64 chars for CoreAPI."""
+    return sanitize_label(value)[:64]
 
 
 def load_acq_label(value: str) -> str:
-    """Normalize for path compatibility but truncate at 128 instead of 64."""
-    return load_cont_label(value, trunc=128)
+    """Sanitize for path compatibility and truncate to 128 chars for CoreAPI."""
+    return sanitize_label(value)[:128]
 
 
 def load_file_name(value: t.Union[str, Path]) -> str:
-    """Normalize for path compatibility without truncating."""
-    name = value.as_posix() if isinstance(value, Path) else value
-    return load_cont_label(name, trunc=0)
+    """Sanitize for path compatibility."""
+    return sanitize_label(str(value))
+
+
+def sanitize_label(value: str) -> str:
+    """Sanitize and truncate labels for filesystem dir/filename compatibility."""
+    # replace '*' with 'star' (to retain eg. DICOM MR T2* domain context)
+    value = re.sub(r"\*", r"star", value)
+    # replace any occurrences of (one or more) invalid chars w/ an underscore
+    unprintable = [chr(c) for c in range(128) if chr(c) not in string.printable]
+    invalid_chars = "*/:<>?\\|\t\n\r\x0b\x0c" + "".join(unprintable)
+    value = re.sub(rf"[{re.escape(invalid_chars):s}]+", "_", value)
+    # finally, truncate to 255 chars and return
+    return value[:255]
 
 
 def load_subj_sex(value: str) -> t.Optional[str]:
     """Normalize to lowercase and return validated value (or None)."""
     subj_sex = value.lower()
     subj_sex_map = {"m": "male", "f": "female", "o": "other"}  # dicom
     subj_sex = subj_sex_map.get(subj_sex, subj_sex)
     if re.match(r"^male|female|other|unknown$", subj_sex):
         return subj_sex
     return None
 
 
-# TODO
-# def load_subj_type(value: str) -> t.Optional[str]:
-#     """Return validated subject type (or None)."""
-#     human|animal|phantom
+def load_subj_type(value: str) -> t.Optional[str]:  # pragma: no cover
+    """Return validated subject type (or None)."""
+    subj_type = value.lower()
+    if re.match(r"^human|animal|phantom$", subj_type):
+        return subj_type
+    return None
 
 
+# TODO
 # def load_subj_race(value: str) -> t.Optional[str]:
 #     """Return validated subject race (or None)."""
 #     r"American Indian or Alaska Native|Asian"
 #     r"|Native Hawaiian or Other Pacific Islander|Black or African American|White"
 #     r"|More Than One Race|Unknown or Not Reported"
 
 
 # def load_subj_ethnicity(value: str) -> t.Optional[str]:
 #     """Return validated subject ethnicity."""
-#     Not Hispanic or Latino|Hispanic or Latino|Unknown or Not Reported
+#     r"Not Hispanic or Latino|Hispanic or Latino|Unknown or Not Reported"
 
 
 def load_sess_age(value: t.Union[str, int, float]) -> t.Optional[int]:
     """Return as a validated integer (or None)."""
     # NOTE add unit conversion here if/when needed later [target: seconds]
     try:
         return int(value)
@@ -251,14 +292,21 @@
 
 
 def load_tags(value: str) -> list:
     """Return list of strings split by comma."""
     return value.split(",") if value else []
 
 
+def load_timezone(value: str) -> t.Optional[str]:  # pragma: no cover
+    """Return timezone string if it's a valid IANA timezone name."""
+    if gettz(value):
+        return value
+    return None
+
+
 def load_any(value):
     """Return value as-is."""
     return value  # pragma: no cover
 
 
 def load_field_tuple(field: str, value) -> t.Tuple[str, t.Any]:
     """Return validated field name and value as a tuple."""
@@ -279,38 +327,38 @@
     "project.info.*": load_any,
     "subject._id": load_cont_id,
     "subject.routing_field": load_any,
     "subject.label": load_cont_label,
     "subject.firstname": load_any,
     "subject.lastname": load_any,
     "subject.sex": load_subj_sex,
-    # "subject.type": load_subj_type,
+    "subject.type": load_subj_type,
     # "subject.race": load_subj_race,
     # "subject.ethnicity": load_subj_ethnicity,
     "subject.species": load_any,
     "subject.strain": load_any,
     "subject.tags": load_tags,
     "subject.info.*": load_any,
     "session._id": load_cont_id,
     "session.uid": load_any,
     "session.routing_field": load_any,
     "session.label": load_cont_label,
     "session.age": load_sess_age,
     "session.weight": load_sess_weight,
     "session.operator": load_any,
     "session.timestamp": Pattern.load_timestamp,
-    # session.timezone is auto-populated
+    "session.timezone": load_timezone,  # auto-populated from timestamp
     "session.tags": load_tags,
     "session.info.*": load_any,
     "acquisition._id": load_cont_id,
     "acquisition.uid": load_any,
     "acquisition.routing_field": load_any,
     "acquisition.label": load_acq_label,
     "acquisition.timestamp": Pattern.load_timestamp,
-    # acquisition.timezone is auto-populated
+    "acquisition.timezone": load_timezone,  # auto-populated from timestamp
     "acquisition.tags": load_tags,
     "acquisition.info.*": load_any,
     "file.name": load_file_name,
     "file.type": load_any,
     "file.tags": load_tags,
     "file.info.*": load_any,
     "file.path": str,
@@ -390,29 +438,37 @@
     # project = "project"
     # subject = "subject"
     # session = "session"
     acquisition = "acquisition"
 
 
 LEVELS = list(ImportLevel)
-
 IMPORT_FILTERS = {
-    # fields that are available when scanning filesystem
     "path": fw_utils.StringFilter,
+    "name": fw_utils.StringFilter,
+    "dir": fw_utils.StringFilter,
+    "depth": fw_utils.NumberFilter,
     "size": fw_utils.SizeFilter,
-    "created": fw_utils.TimeFilter,
-    "modified": fw_utils.TimeFilter,
-    # everything else available once we parsed the file
-    "*": fw_utils.StringFilter,
+    "ctime": fw_utils.TimeFilter,
+    "mtime": fw_utils.TimeFilter,
+}
+IMPORT_FILTER_ALIASES = {
+    r"^filepath$": "path",
+    r"^filename$": "name",
+    r"^dirname$": "dir",
+    r"^created$": "ctime",
+    r"^modified$": "mtime",
 }
 
 
 def validate_import_filter_field(field: str) -> str:
     """Return validated/canonic import filter field name for the field shorthand."""
-    return fw_utils.parse_field_name(field, allowed=list(IMPORT_FILTERS))
+    return fw_utils.parse_field_name(
+        field, aliases=IMPORT_FILTER_ALIASES, allowed=list(IMPORT_FILTERS)
+    )
 
 
 class ImportFilter(fw_utils.IncludeExcludeFilter):
     """Import include/exclude filter with field validation and filter types."""
 
     def __init__(
         self,
@@ -427,19 +483,17 @@
             validate=validate_import_filter_field,
         )
 
 
 class ImportRule(BaseModel):
     """Import rule defining what to import and how."""
 
-    # TODO rename here and in export to container
-    # TODO add depth, dirname and filename to filters (fs-like only)
     level: ImportLevel = Field(
         ImportLevel.acquisition,
-        title="Flywheel hierarchy level to import files to",
+        title="Flywheel container hierarchy level to import files to",
     )
     include: t.Optional[t.List[str]] = Field(
         title=(
             "Include filters - if given, "
             "only include files matching at least one include filter"
         ),
         example=["path=~.dcm"],
@@ -454,126 +508,130 @@
     type: t.Optional[str] = Field(
         title=(
             "Data type to import matching files with - if given, "
             "allows extracting additional metadata for known types"
         ),
         example="dicom",
     )
+    zip: t.Optional[t.Literal[True]] = Field(
+        title="Import multiple grouped files zipped together",
+    )
     group_by: t.Optional[str] = Field(
-        title="Group and process files together based on shared property",
-        readOnly=True,  # hide in inpus schemas for now
+        title="Group and process files together based on a shared prefix",
+        readOnly=True,  # hide in input schemas for now
         example="dir",
     )
-    zip: t.Optional[bool] = Field(title="Import multiple grouped files zipped together")
     mappings: Mappings = Field(
         title="Metadata mapping patterns",
         example=[
             ("path", "{sub}/{ses}/{acq}/{file}"),
             ("path", "{file.info.original_path}"),
         ],
     )
     defaults: t.Optional[Mappings] = Field(
         title="Metadata fallback defaults",
+        readOnly=True,  # hide in input schemas for now
         example={"session.label": "control"},
     )
     overrides: t.Optional[Mappings] = Field(
         title="Metadata manual overrides",
+        readOnly=True,  # hide in input schemas for now
         example={"subject.label": "ex1000"},
     )
 
-    @property
-    def meta_fields(self) -> t.Set[str]:
-        """Return metadata fields that are present in the rule."""
-        return self.extractor.fields
+    _filter: ImportFilter = PrivateAttr(None)
+    _group_by: ImportTemplate = PrivateAttr(None)
+    _extractor: MetaExtractor = PrivateAttr(None)
 
     @root_validator(pre=True, skip_on_failure=True)
     @classmethod
     def validate_rule(cls, values: dict) -> dict:
         """Validate the filters and the mappings given the level constraint."""
         level = ImportLevel(values.setdefault("level", "acquisition"))
-        # sanity check that level is acquisition for know
+        # sanity check that level is acquisition for now
         assert level == ImportLevel.acquisition, f"Unsupported import level {level}"
         # validate filters
         filt = ImportFilter(
-            include=values.get("include"),
-            exclude=values.get("exclude"),
+            include=values.get("includes") or values.get("include"),
+            exclude=values.get("excludes") or values.get("exclude"),
         )
         values["include"] = [str(i) for i in filt.include]
         values["exclude"] = [str(e) for e in filt.exclude]
-        # autofill type/group_by/zip
-        if values.get("type") == "dicom" and values.get("zip") is None:
-            # auto-fill zip=true for type=dicom
-            values["zip"] = True
-        if values.get("zip") and values.get("group_by") is None:
-            # auto-fill group_by=dir for zip=true
-            values["group_by"] = "dir"
-        # validate group_by template
+        # TODO use path globs in group_by for more flexibility, eg.:
+        # - ** = group by parent dir = current functionality
+        # - */* = group by the top 2 levels
+        # - **/foo = group by the closest parent dir named foo (also filters)
+        # when available, then it may be exposed as a feature
+        # default to group_by=dir if type=dicom and/or zip=true
+        if values.get("group_by") is None:
+            if values.get("type") == "dicom" or values.get("zip"):
+                values["group_by"] = "dir"
+        # if group_by is set, ensure it's a valid template
         if values.get("group_by"):
-            ImportTemplate(values["group_by"])
-            # shouldn't get direct input from hidden field, but still auto-fill
-            if values.get("zip") is None:
-                values["zip"] = True  # pragma: no cover
+            assert ImportTemplate(values["group_by"])
         # validate patterns
         extractor = MetaExtractor(
-            mappings=values.get("mappings"),
-            defaults=values.get("defaults"),
-            overrides=values.get("overrides"),
+            mappings=values.get("mappings") or values.get("mapping"),
+            defaults=values.get("defaults") or values.get("default"),
+            overrides=values.get("overrides") or values.get("override"),
         )
+        # check that untyped rules only reference known stat fields
+        if not values.get("type"):
+            allowed = set(IMPORT_FILTERS)
+            if invalid := extractor.src_fields - allowed:  # pragma: no cover
+                invalid_str = ",".join(invalid)
+                allowed_str = "|".join(allowed)
+                msg = f"invalid mapping field: {invalid_str} (allowed: {allowed_str})"
+                raise ValueError(msg)
         values["mappings"] = [(str(t), str(p)) for t, p in extractor.mappings]
         values["defaults"] = extractor.defaults
         values["overrides"] = extractor.overrides
-        assert values["mappings"], "At least one pattern is required"
         return values
 
-    _filter: ImportFilter = PrivateAttr(None)
-    _group_tpl: ImportTemplate = PrivateAttr(None)
-    _extractor: MetaExtractor = PrivateAttr(None)
+    def group(self, stat) -> t.Optional[str]:
+        """Return the file's prefix group based on the group_by template."""
+        if not self.group_by:
+            return None  # pragma: no cover
+        if not self._group_by:
+            self._group_by = ImportTemplate(self.group_by)
+        return self._group_by.format(stat)
 
-    @property
-    def filter(self) -> ImportFilter:
-        """Return initialized import filter instance."""
+    def match(self, stat) -> bool:
+        """Return True if the file matches the rule's include/exclude filters."""
         if not self._filter:
             self._filter = ImportFilter(include=self.include, exclude=self.exclude)
-        return self._filter
+        return self._filter.match(stat)
 
-    @property
-    def group_tpl(self) -> t.Optional[ImportTemplate]:
-        """Return initialized group_by template instance."""
-        if not self._group_tpl and self.group_by:
-            self._group_tpl = ImportTemplate(self.group_by)
-        return self._group_tpl
+    def extract(self, *stat_and_meta) -> t.Optional[MetaData]:
+        """Return extracted metadata if the object matches the filters."""
+        file = FieldGetter(*stat_and_meta)
+        if not self.match(file):
+            return None  # pragma: no cover
+        meta = self.extractor.extract(file)
+        if self.type:
+            meta.setdefault("file.type", self.type)
+        # TODO consider saving the import and the storage/path on info
+        # TODO consider suffixing [.type].zip to file.name here
+        return meta
 
     @property
     def extractor(self) -> MetaExtractor:
         """Return initialized meta extractor instance."""
         if not self._extractor:
             self._extractor = MetaExtractor(
                 mappings=self.mappings,
                 defaults=self.defaults,
                 overrides=self.overrides,
             )
         return self._extractor
 
-    def match(self, value) -> bool:
-        """Return True if the value passes the include/exclude filters."""
-        return self.filter.match(value)
-
-    def group(self, value) -> t.Optional[str]:
-        """Return the value's group based on the group_by template."""
-        return self.group_tpl.format(value) if self.group_tpl else None
-
-    def extract(self, value: dict) -> t.Optional[MetaData]:
-        """Return extracted metadata if the value matches the filters."""
-        if not self.match(value):
-            return None  # pragma: no cover
-        meta = self.extractor.extract(value)
-        if self.type:
-            meta.setdefault("file.type", self.type)
-        # TODO consider suffixing [.type].zip to file.name here
-        return meta
+    @property
+    def dst_fields(self) -> t.Set[str]:
+        """Return metadata fields that are present in the rule."""
+        return self.extractor.dst_fields
 
 
 # HELPERS
 
 
 def parse_metadata_mappings(mappings: Mappings) -> t.Iterable[t.Tuple[str, str]]:
     """Parse and yield metadata mappings as a tuple."""
@@ -582,7 +640,54 @@
     elif isinstance(mappings, dict):
         mappings = list(mappings.items())
     for mapping in mappings:
         if isinstance(mapping, str):
             yield mapping.split("=", maxsplit=1)  # type: ignore
         else:
             yield mapping
+
+
+def validate_metadata_mapping(
+    mapping: t.Tuple[str, str]
+) -> t.Tuple["ImportTemplate", "ImportPattern"]:  # pragma: no cover
+    """Return validated (ImportTemplate, ImportPattern) tuple from 2 strings."""
+    # attempt left-to-right first, then reversed for input flexibility
+    error: t.Optional[ValueError] = None
+    for template, pattern in [mapping, reversed(mapping)]:
+        try:
+            return ImportTemplate(template), ImportPattern(pattern)
+        except ValueError as exc:
+            error = error or exc
+    # always raise the left-to-right error for consistency
+    assert error
+    raise error
+
+
+class FieldGetter:
+    """Wrapper class dispatching attr/key access to multiple objects in order."""
+
+    def __init__(self, *objects) -> None:
+        """Init FieldGetter instance with one or more objects."""
+        assert objects, "at least one object required"
+        self._objects = objects
+
+    def __getattr__(self, field):
+        """Return the first object's attr that has it or raise AttributeError."""
+        error: t.Optional[AttributeError] = None
+        for obj in self._objects:
+            try:
+                return getattr(obj, field)
+            except AttributeError as exc:
+                error = exc
+        assert error
+        raise error
+
+    def __getitem__(self, field):
+        """Return the first object's key that has it or raise KeyError."""
+        error: t.Optional[KeyError] = None
+        for obj in self._objects:
+            try:
+                return obj[field]
+            except KeyError as exc:
+                error = exc
+        assert error
+        raise error
```

## Comparing `fw_meta-3.3.2.dist-info/LICENSE` & `fw_meta-4.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_meta-3.3.2.dist-info/METADATA` & `fw_meta-4.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-meta
-Version: 3.3.2
+Version: 4.0.0
 Summary: Flywheel metadata extraction.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-meta
 License: MIT
 Keywords: Flywheel,DICOM,metadata,extract
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: fw-utils (>=4.2.5,<5.0.0)
-Requires-Dist: pathvalidate (>=2.3.2,<3.0.0)
 Requires-Dist: pydantic (>=1.7.3,<2.0.0)
 Project-URL: Documentation, https://gitlab.com/flywheel-io/tools/lib/fw-meta
 Project-URL: Repository, https://gitlab.com/flywheel-io/tools/lib/fw-meta
 Description-Content-Type: text/markdown
 
 # fw-meta
```

