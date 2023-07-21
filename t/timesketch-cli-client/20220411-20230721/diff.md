# Comparing `tmp/timesketch-cli-client-20220411.tar.gz` & `tmp/timesketch-cli-client-20230721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timesketch-cli-client-20220411.tar", last modified: Tue Apr 12 09:26:51 2022, max compression
+gzip compressed data, was "timesketch-cli-client-20230721.tar", last modified: Fri Jul 21 12:11:15 2023, max compression
```

## Comparing `timesketch-cli-client-20220411.tar` & `timesketch-cli-client-20230721.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxrwxr-x   0 jbn       (1000) jbn       (1000)        0 2022-04-12 09:26:51.409292 timesketch-cli-client-20220411/
--rw-rw-r--   0 jbn       (1000) jbn       (1000)      460 2022-04-12 09:26:51.408292 timesketch-cli-client-20220411/PKG-INFO
--rw-rw-r--   0 jbn       (1000) jbn       (1000)       38 2022-04-12 09:26:51.409292 timesketch-cli-client-20220411/setup.cfg
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     1649 2022-04-11 15:33:04.000000 timesketch-cli-client-20220411/setup.py
-drwxrwxr-x   0 jbn       (1000) jbn       (1000)        0 2022-04-12 09:26:51.405292 timesketch-cli-client-20220411/timesketch_cli_client/
--rw-r--r--   0 jbn       (1000) jbn       (1000)        0 2022-04-06 20:43:39.000000 timesketch-cli-client-20220411/timesketch_cli_client/__init__.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     4933 2022-04-11 18:31:41.000000 timesketch-cli-client-20220411/timesketch_cli_client/cli.py
-drwxrwxr-x   0 jbn       (1000) jbn       (1000)        0 2022-04-12 09:26:51.408292 timesketch-cli-client-20220411/timesketch_cli_client/commands/
--rw-r--r--   0 jbn       (1000) jbn       (1000)        0 2022-04-06 20:43:39.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/__init__.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     3086 2022-04-12 09:26:24.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/analyze.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     1871 2022-04-11 15:33:04.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/config.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     2871 2022-04-11 15:33:04.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/importer.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     7213 2022-04-12 09:26:24.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/search.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     1721 2022-04-11 18:04:16.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/search_test.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     1736 2022-04-12 09:26:24.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/sketch.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     1502 2022-04-11 15:33:04.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/sketch_test.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     1652 2022-04-11 15:33:04.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/timelines.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     1535 2022-04-11 15:33:04.000000 timesketch-cli-client-20220411/timesketch_cli_client/commands/timelines_test.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)      734 2022-04-11 15:33:04.000000 timesketch-cli-client-20220411/timesketch_cli_client/definitions.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)     1293 2022-04-11 15:33:04.000000 timesketch-cli-client-20220411/timesketch_cli_client/test_lib.py
--rw-rw-r--   0 jbn       (1000) jbn       (1000)      766 2022-04-12 09:26:24.000000 timesketch-cli-client-20220411/timesketch_cli_client/version.py
-drwxrwxr-x   0 jbn       (1000) jbn       (1000)        0 2022-04-12 09:26:51.407292 timesketch-cli-client-20220411/timesketch_cli_client.egg-info/
--rw-rw-r--   0 jbn       (1000) jbn       (1000)      460 2022-04-12 09:26:51.000000 timesketch-cli-client-20220411/timesketch_cli_client.egg-info/PKG-INFO
--rw-rw-r--   0 jbn       (1000) jbn       (1000)      927 2022-04-12 09:26:51.000000 timesketch-cli-client-20220411/timesketch_cli_client.egg-info/SOURCES.txt
--rw-rw-r--   0 jbn       (1000) jbn       (1000)        1 2022-04-12 09:26:51.000000 timesketch-cli-client-20220411/timesketch_cli_client.egg-info/dependency_links.txt
--rw-rw-r--   0 jbn       (1000) jbn       (1000)       62 2022-04-12 09:26:51.000000 timesketch-cli-client-20220411/timesketch_cli_client.egg-info/entry_points.txt
--rw-rw-r--   0 jbn       (1000) jbn       (1000)        1 2022-04-08 07:24:24.000000 timesketch-cli-client-20220411/timesketch_cli_client.egg-info/not-zip-safe
--rw-rw-r--   0 jbn       (1000) jbn       (1000)       69 2022-04-12 09:26:51.000000 timesketch-cli-client-20220411/timesketch_cli_client.egg-info/requires.txt
--rw-rw-r--   0 jbn       (1000) jbn       (1000)       22 2022-04-12 09:26:51.000000 timesketch-cli-client-20220411/timesketch_cli_client.egg-info/top_level.txt
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:11:15.185254 timesketch-cli-client-20230721/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)      432 2023-07-21 12:11:15.185254 timesketch-cli-client-20230721/PKG-INFO
+-rw-r-----   0 jbn      (190240) primarygroup (89939)       38 2023-07-21 12:11:15.185254 timesketch-cli-client-20230721/setup.cfg
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1649 2022-05-04 12:34:04.000000 timesketch-cli-client-20230721/setup.py
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:11:15.173253 timesketch-cli-client-20230721/timesketch_cli_client/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)        0 2021-03-02 08:38:31.000000 timesketch-cli-client-20230721/timesketch_cli_client/__init__.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     6088 2023-07-10 09:06:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/cli.py
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:11:15.185254 timesketch-cli-client-20230721/timesketch_cli_client/commands/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)        0 2021-03-02 08:38:31.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/__init__.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     7581 2023-07-21 09:23:39.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/analyze.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     3422 2023-07-21 11:33:16.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/attribute.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1871 2022-05-04 12:34:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/config.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     5487 2023-07-10 09:06:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/events.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     5509 2023-07-10 09:06:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/events_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     2871 2022-05-04 12:34:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/importer.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     7860 2023-07-10 09:06:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/search.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1721 2022-05-04 12:34:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/search_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     2736 2023-07-10 09:06:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/sigma.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1722 2023-05-16 06:52:32.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/sigma_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     2924 2023-07-21 11:33:16.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/sketch.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1502 2022-05-04 12:34:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/sketch_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     2758 2023-07-10 09:06:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/timelines.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1535 2023-03-16 15:33:50.000000 timesketch-cli-client-20230721/timesketch_cli_client/commands/timelines_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)      742 2023-07-10 09:06:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/definitions.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1863 2023-07-10 09:06:04.000000 timesketch-cli-client-20230721/timesketch_cli_client/test_lib.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)      766 2023-07-21 11:58:10.000000 timesketch-cli-client-20230721/timesketch_cli_client/version.py
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:11:15.177253 timesketch-cli-client-20230721/timesketch_cli_client.egg-info/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)      432 2023-07-21 12:11:15.000000 timesketch-cli-client-20230721/timesketch_cli_client.egg-info/PKG-INFO
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1143 2023-07-21 12:11:15.000000 timesketch-cli-client-20230721/timesketch_cli_client.egg-info/SOURCES.txt
+-rw-r-----   0 jbn      (190240) primarygroup (89939)        1 2023-07-21 12:11:15.000000 timesketch-cli-client-20230721/timesketch_cli_client.egg-info/dependency_links.txt
+-rw-r-----   0 jbn      (190240) primarygroup (89939)       61 2023-07-21 12:11:15.000000 timesketch-cli-client-20230721/timesketch_cli_client.egg-info/entry_points.txt
+-rw-r-----   0 jbn      (190240) primarygroup (89939)        1 2023-07-21 12:11:15.000000 timesketch-cli-client-20230721/timesketch_cli_client.egg-info/not-zip-safe
+-rw-r-----   0 jbn      (190240) primarygroup (89939)       69 2023-07-21 12:11:15.000000 timesketch-cli-client-20230721/timesketch_cli_client.egg-info/requires.txt
+-rw-r-----   0 jbn      (190240) primarygroup (89939)       22 2023-07-21 12:11:15.000000 timesketch-cli-client-20230721/timesketch_cli_client.egg-info/top_level.txt
```

### Comparing `timesketch-cli-client-20220411/setup.py` & `timesketch-cli-client-20230721/setup.py`

 * *Files identical despite different names*

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/cli.py` & `timesketch-cli-client-20230721/timesketch_cli_client/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,43 +14,58 @@
 """Timesketch CLI client."""
 
 import sys
 import click
 
 from requests.exceptions import ConnectionError as RequestConnectionError
 
+# pylint: disable=import-error
 from timesketch_api_client import config as timesketch_config
 
+# pylint: enable=import-error
+
 from timesketch_cli_client.commands import analyze
 from timesketch_cli_client.commands import config
 from timesketch_cli_client.commands import importer
 from timesketch_cli_client.commands import search
 from timesketch_cli_client.commands import sketch as sketch_command
 from timesketch_cli_client.commands import timelines
+from timesketch_cli_client.commands import events
+from timesketch_cli_client.commands import sigma
 
 from .definitions import DEFAULT_OUTPUT_FORMAT
 from .version import get_version
 
 
 class TimesketchCli(object):
     """Timesketch CLI state object.
 
     Attributes:
         sketch_from_flag: Sketch ID if provided by flag
         config_assistant: Instance of ConfigAssistant
+        output_format_from_flag: Output format to use
     """
 
-    def __init__(self, api_client=None, sketch_from_flag=None, conf_file=""):
+    def __init__(
+        self,
+        api_client=None,
+        sketch_from_flag=None,
+        conf_file="",
+        output_format_from_flag=None,
+    ):
         """Initialize the state object.
 
         Args:
             sketch_from_flag: Sketch ID if provided by flag.
+            conf_file: Path to the config file.
+            output_format_from_flag: Output format to use.
         """
         self.api = api_client
         self.sketch_from_flag = sketch_from_flag
+        self.output_format_from_flag = output_format_from_flag
 
         if not api_client:
             try:
                 # TODO: Consider other config sections here as well.
                 self.api = timesketch_config.get_client(load_cli_config=True)
                 if not self.api:
                     raise RequestConnectionError
@@ -90,54 +105,72 @@
             click.echo("ERROR: No such sketch or you don't have access.")
             sys.exit(1)
 
         return active_sketch
 
     @property
     def output_format(self):
-        """Get the configured output format, or the default format if missing.
+        """Get the output format
+        The priority is:
+            * output_format set via flag
+            * output_format set via config file
+            * or the default format if missing.
 
         Returns:
             Output format as a string.
         """
-        output_format = self.config_assistant.get_config("output_format")
-        if not output_format:
+        if self.output_format_from_flag:
+            output_format = self.output_format_from_flag
+            self.config_assistant.set_config("output", output_format)
+            self.config_assistant.save_config()
+            return output_format
+        try:
+            output_format = self.config_assistant.get_config("output")
+        except KeyError:  # in case value does not exist in the config file
             self.config_assistant.set_config("output", DEFAULT_OUTPUT_FORMAT)
             self.config_assistant.save_config()
             output_format = DEFAULT_OUTPUT_FORMAT
         return output_format
 
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.version_option(version=get_version(), prog_name="Timesketch CLI")
 @click.option("--sketch", type=int, default=None, help="Sketch to work in.")
+@click.option(
+    "--output-format",
+    "output",
+    required=False,
+    help="Set output format [json, text, tabular, csv] (overrides global setting).",
+)
 @click.pass_context
-def cli(ctx, sketch):
+def cli(ctx, sketch, output):
     """Timesketch CLI client.
 
     This tool provides similar features as the web client does.
     It operates within the context of a sketch so you either need to
     provide an existing sketch or create a new one.
 
-    Basic options for editing the sketch is provided, e.g re-naming and
+    Basic options for editing the sketch is provided, e.g. re-naming and
     changing the description as well as archiving and exporting. For
     other actions not available in this CLI client the web client should be
     used.
 
     For detailed help on each command, run  <command> --help
     """
-    ctx.obj = TimesketchCli(sketch_from_flag=sketch)
+    ctx.obj = TimesketchCli(sketch_from_flag=sketch, output_format_from_flag=output)
 
 
 # Register all commands.
 cli.add_command(config.config_group)
 cli.add_command(timelines.timelines_group)
 cli.add_command(search.search_group)
 cli.add_command(search.saved_searches_group)
 cli.add_command(analyze.analysis_group)
 cli.add_command(sketch_command.sketch_group)
 cli.add_command(importer.importer)
+cli.add_command(events.events_group)
+cli.add_command(sigma.sigma_group)
 
 
 # pylint: disable=no-value-for-parameter
 if __name__ == "__main__":
     cli()
```

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/commands/config.py` & `timesketch-cli-client-20230721/timesketch_cli_client/commands/config.py`

 * *Files identical despite different names*

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/commands/importer.py` & `timesketch-cli-client-20230721/timesketch_cli_client/commands/importer.py`

 * *Files identical despite different names*

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/commands/search.py` & `timesketch-cli-client-20230721/timesketch_cli_client/commands/search.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,68 +18,81 @@
 
 import click
 from tabulate import tabulate
 
 from timesketch_api_client import search
 
 
-def format_output(search_obj, output_format, show_headers):
+def format_output(search_obj, output_format, show_headers, show_internal_columns):
     """Format search result output.
 
     Args:
         search_obj: API Search object.
-        output_format: The format to use.
+        output_format: The format to use (text, csv, json, jsonl, tabular).
         show_headers: Boolean indicating if header row should be displayed.
+        show_internal_columns: Boolean indicating if internal columns should
+        be displayed.
 
     Returns:
         Search results in the requested output format.
     """
     dataframe = search_obj.to_pandas()
 
     # Label is being set regardless of return_fields. Remove if it is not in
     # the list of requested fields.
     if "label" not in search_obj.return_fields:
         dataframe = dataframe.drop(columns=["label"], errors="ignore")
 
-    # Remove internal OpenSeearch columns
-    dataframe = dataframe.drop(
-        columns=["__ts_timeline_id", "_id", "_index", "_source", "_type"],
-        errors="ignore",
-    )
+    if not show_internal_columns:
+        # Remove internal OpenSearch columns
+        dataframe = dataframe.drop(
+            columns=["__ts_timeline_id", "_id", "_index", "_source", "_type"],
+            errors="ignore",
+        )
 
     result = None
     if output_format == "text":
         result = dataframe.to_string(index=False, header=show_headers)
     elif output_format == "csv":
         result = dataframe.to_csv(index=False, header=show_headers)
+    elif output_format == "json":
+        result = dataframe.to_json(orient="records", lines=False)
+    elif output_format == "jsonl":
+        result = dataframe.to_json(orient="records", lines=True)
     elif output_format == "tabular":
         if show_headers:
             result = tabulate(
                 dataframe, headers="keys", tablefmt="psql", showindex=False
             )
         else:
             result = tabulate(dataframe, tablefmt="psql", showindex=False)
 
     return result
 
 
 def describe_query(search_obj):
-    """Print details of a search query nd filter."""
+    """Print details of a search query and filter."""
     filter_pretty = json.dumps(search_obj.query_filter, indent=2)
     click.echo(f"Query string: {search_obj.query_string}")
     click.echo(f"Return fields: {search_obj.return_fields}")
     click.echo(f"Filter: {filter_pretty}")
 
 
 @click.command("search")
 @click.option(
-    "--query", "-q", default="*", help="Search query in OpenSearch query string format"
+    "--query",
+    "-q",
+    default="*",
+    help="Search query in OpenSearch query string format",
 )
 @click.option(
-    "--time", "times", multiple=True, help="Datetime filter (e.g. 2020-01-01T12:00)"
+    "--time",
+    "times",
+    multiple=True,
+    help="Datetime filter (e.g. 2020-01-01T12:00)",
 )
 @click.option(
     "--time-range",
     "time_ranges",
     multiple=True,
     nargs=2,
     help="Datetime range filter (e.g: 2020-01-01 2020-02-01)",
@@ -87,67 +100,80 @@
 @click.option("--label", "labels", multiple=True, help="Filter events with label")
 @click.option(
     "--header/--no-header",
     default=True,
     help="Toggle header information (default is to show)",
 )
 @click.option(
-    "--output-format", "output", help="Set output format (overrides global setting)"
+    "--return-fields",
+    "return_fields",
+    default="",
+    help="What event fields to show",
 )
 @click.option(
-    "--return-fields", "return_fields", default="", help="What event fields to show"
+    "--order",
+    default="asc",
+    help="Order the output (asc/desc) based on the time field",
 )
 @click.option(
-    "--order", default="asc", help="Order the output (asc/desc) based on the time field"
-)
-@click.option(
-    "--limit", type=int, default=40, help="Limit amount of events to show (default: 40)"
+    "--limit",
+    type=int,
+    default=40,
+    help="Limit amount of events to show (default: 40)",
 )
 @click.option("--saved-search", type=int, help="Query and filter from saved search")
 @click.option(
     "--describe",
     is_flag=True,
     default=False,
     help="Show the query and filter then exit",
 )
+@click.option(
+    "--show-internal-columns",
+    is_flag=True,
+    default=False,
+    help="Show all columns including Timesketch internal ones",
+)
 @click.pass_context
 # pylint: disable=too-many-arguments
 def search_group(
     ctx,
     query,
     times,
     time_ranges,
     labels,
     header,
-    output,
     return_fields,
     order,
     limit,
     saved_search,
     describe,
+    show_internal_columns,
 ):
     """Search and explore."""
     sketch = ctx.obj.sketch
     output_format = ctx.obj.output_format
     search_obj = search.Search(sketch=sketch)
 
-    if output:
-        output_format = output
-
     new_line = True
     if output_format == "csv":
         new_line = False
 
     # Construct query from saved search and return early.
     if saved_search:
         search_obj.from_saved(saved_search)
+        if limit:
+            search_obj.max_entries = limit
         if describe:
             describe_query(search_obj)
             return
-        click.echo(format_output(search_obj, output_format, header), nl=new_line)
+        click.echo(
+            format_output(search_obj, output_format, header, show_internal_columns),
+            nl=new_line,
+        )
         return
 
     # Construct the query from flags.
     # TODO (berggren): Add support for query DSL.
     search_obj.query_string = query
 
     if return_fields:
@@ -162,29 +188,29 @@
         search_obj.order_descending()
 
     # TODO: Add term chips.
     if time_ranges:
         for time_range in time_ranges:
             try:
                 range_chip = search.DateRangeChip()
-                range_chip.add_start_time = time_range[0]
-                range_chip.add_end_time = time_range[1]
+                range_chip.add_start_time(time_range[0])
+                range_chip.add_end_time(time_range[1])
                 search_obj.add_chip(range_chip)
             except ValueError:
                 click.echo("Error parsing date (make sure it is ISO formatted)")
                 sys.exit(1)
 
     # TODO (berggren): This should support dates like 2021-02-12 and then
     # convert to ISO format.
     if times:
         for time in times:
             try:
                 range_chip = search.DateRangeChip()
-                range_chip.add_start_time = time
-                range_chip.add_end_time = time
+                range_chip.add_start_time(time)
+                range_chip.add_end_time(time)
                 search_obj.add_chip(range_chip)
             except ValueError:
                 click.echo("Error parsing date (make sure it is ISO formatted)")
                 sys.exit(1)
 
     if labels:
         for label in labels:
@@ -197,15 +223,18 @@
                 label_chip.label = label
             search_obj.add_chip(label_chip)
 
     if describe:
         describe_query(search_obj)
         return
 
-    click.echo(format_output(search_obj, output_format, header), nl=new_line)
+    click.echo(
+        format_output(search_obj, output_format, header, show_internal_columns),
+        nl=new_line,
+    )
 
 
 @click.group("saved-searches")
 def saved_searches_group():
     """Managed saved searches."""
```

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/commands/search_test.py` & `timesketch-cli-client-20230721/timesketch_cli_client/commands/search_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/commands/sketch.py` & `timesketch-cli-client-20230721/timesketch_cli_client/commands/sketch.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,47 +9,87 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Commands for sketches."""
 
+import json
 import click
+import pandas as pd
+
+from timesketch_cli_client.commands import attribute as attribute_command
 
 
 @click.group("sketch")
 def sketch_group():
     """Manage sketch."""
 
 
-@sketch_group.command("list")
+# Add the attribute command group to the sketch command group.
+sketch_group.add_command(attribute_command.attribute_group)
+
+
+@sketch_group.command("list", help="List all sketches.")
 @click.pass_context
 def list_sketches(ctx):
     """List all sketches."""
     api_client = ctx.obj.api
+    output = ctx.obj.output_format
+    sketches = []
+
     for sketch in api_client.list_sketches():
-        click.echo(f"{sketch.id} {sketch.name}")
+        sketches.append({"id": sketch.id, "name": sketch.name})
 
+    sketch_panda = pd.DataFrame(sketches, columns=["id", "name"])
+    if output == "json":
+        click.echo(sketch_panda.to_json(orient="records", indent=4))
+    elif output == "text":
+        click.echo(f"{sketch_panda.to_string(index=False)}")
+    else:
+        click.echo(f"Output format {output} not implemented.")
+        ctx.exit(1)
 
-@sketch_group.command("describe")
+
+@sketch_group.command(
+    "describe",
+    help="Describe the active sketch",
+)
 @click.pass_context
 def describe_sketch(ctx):
-    """Show info about the active sketch."""
+    """Describe the active sketch.
+    Attributes only in JSON output format."""
     sketch = ctx.obj.sketch
-    # TODO (berggren): Add more details to the output.
-    click.echo(f"Name: {sketch.name}")
-    click.echo(f"Description: {sketch.description}")
+    output = ctx.obj.output_format
 
+    if output == "json":
+        click.echo(json.dumps(sketch.__dict__, indent=4, sort_keys=True, default=str))
+        return
+    if output == "text":
+        click.echo(f"Name: {sketch.name}")
+        click.echo(f"Description: {sketch.description}")
+        click.echo(f"Status: {sketch.status}")
+    else:
+        click.echo(f"Output format {output} not implemented.")
+        ctx.exit(1)
 
-@sketch_group.command("create")
+
+@sketch_group.command("create", help="Create a new sketch [text].")
 @click.option("--name", required=True, help="Name of the sketch.")
 @click.option(
-    "--description", required=False, help="Description of the sketch (optional)"
+    "--description",
+    required=False,
+    help="Description of the sketch (optional).",
 )
 @click.pass_context
 def create_sketch(ctx, name, description):
-    """Create a new sketch."""
+    """Create a new sketch.
+
+    Args:
+        name: Name of the sketch.
+        description: Description of the sketch (optional).
+    """
     api_client = ctx.obj.api
     if not description:
         description = name
     sketch = api_client.create_sketch(name=name, description=description)
     click.echo(f"Sketch created: {sketch.name}")
```

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/commands/sketch_test.py` & `timesketch-cli-client-20230721/timesketch_cli_client/commands/sketch_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/commands/timelines.py` & `timesketch-cli-client-20230721/timesketch_cli_client/commands/timelines.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,24 +31,49 @@
     """
     sketch = ctx.obj.sketch
     for timeline in sketch.list_timelines():
         click.echo(f"{timeline.id} {timeline.name}")
 
 
 @timelines_group.command("describe")
-@click.argument("timeline_id", type=int, required=False)
+@click.argument("timeline-id", type=int, required=False)
 @click.pass_context
 def describe_timeline(ctx, timeline_id):
     """Show details for a timeline.
 
     Args:
         ctx: Click CLI context object.
-        timeline_id: Timeline ID from argument.
+        timeline-id: Timeline ID from argument.
     """
     sketch = ctx.obj.sketch
-    # TODO (berggren): Add more details to the output, e.g. the data_sources
+    output = ctx.obj.output_format
     timeline = sketch.get_timeline(timeline_id=timeline_id)
     if not timeline:
         click.echo("No such timeline")
         return
+    timeline.lazyload_data()
+    if output == "json":
+        click.echo(f"{timeline.resource_data}")
+        return
+    if output != "text":
+        click.echo(f'Unsupported output format: "{output}" - using "text" instead')
+
     click.echo(f"Name: {timeline.name}")
     click.echo(f"Index: {timeline.index_name}")
+    click.echo(f"Status: {timeline.status}")
+    lines_indexed = timeline.resource_data.get("meta").get("lines_indexed", 0)
+    click.echo(f"Event count: {lines_indexed or 0}")
+
+    for timeline_object in timeline.resource_data.get("objects", None):
+        name = timeline_object.get("name", "no name")
+        created = timeline_object.get("created_at", 0)
+        click.echo(f"Name: {name}")
+        click.echo(f"Created: {created}")
+        click.echo("Datasources:")
+        for datasource in timeline_object.get("datasources", []):
+            error_message = datasource.get("error_message", None)
+            original_filename = datasource.get("original_filename", None)
+            file_on_disk = datasource.get("file_on_disk", None)
+
+            click.echo(f"\tOriginal filename: {original_filename}")
+            click.echo(f"\tFile on disk: {file_on_disk}")
+            click.echo(f"\tError: {error_message}")
```

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/commands/timelines_test.py` & `timesketch-cli-client-20230721/timesketch_cli_client/commands/timelines_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/definitions.py` & `timesketch-cli-client-20230721/timesketch_cli_client/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Definitions for the Timesketch CLI client."""
 
-SUPPORTED_OUTPUT_FORMATS = ["text", "csv", "tabular"]
+SUPPORTED_OUTPUT_FORMATS = ["text", "csv", "tabular", "json"]
 DEFAULT_OUTPUT_FORMAT = "tabular"
```

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/test_lib.py` & `timesketch-cli-client-20230721/timesketch_cli_client/test_lib.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,7 +40,32 @@
     api_client = client.TimesketchApi("http://127.0.0.1", "test", "test")
     with tempfile.NamedTemporaryFile(mode="w") as fw:
         fw.write(TEST_CONFIG)
         fw.seek(0)
         return TimesketchCli(
             api_client=api_client, sketch_from_flag=1, conf_file=fw.name
         )
+
+
+TEST_CONFIG_NO_OUTPUT_FORMAT = """
+[timesketch]
+host_uri = http://127.0.0.1
+username = foobar
+auth_mode = oauth
+client_id = myidfoo
+client_secret = sdfa@$FAsASDF132
+verify = True
+
+[cli]
+sketch = 1
+#output_format = tabular
+"""
+
+
+def get_cli_context_no_output():
+    api_client = client.TimesketchApi("http://127.0.0.1", "test", "test")
+    with tempfile.NamedTemporaryFile(mode="w") as fw:
+        fw.write(TEST_CONFIG_NO_OUTPUT_FORMAT)
+        fw.seek(0)
+        return TimesketchCli(
+            api_client=api_client, sketch_from_flag=1, conf_file=fw.name
+        )
```

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client/version.py` & `timesketch-cli-client-20230721/timesketch_cli_client/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Version information for the Timesketch CLI client."""
 
-__version__ = "20220411"
+__version__ = "20230721"
 
 
 def get_version():
     """Returns the version information."""
     return __version__
```

### Comparing `timesketch-cli-client-20220411/timesketch_cli_client.egg-info/SOURCES.txt` & `timesketch-cli-client-20230721/timesketch_cli_client.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 timesketch_cli_client.egg-info/dependency_links.txt
 timesketch_cli_client.egg-info/entry_points.txt
 timesketch_cli_client.egg-info/not-zip-safe
 timesketch_cli_client.egg-info/requires.txt
 timesketch_cli_client.egg-info/top_level.txt
 timesketch_cli_client/commands/__init__.py
 timesketch_cli_client/commands/analyze.py
+timesketch_cli_client/commands/attribute.py
 timesketch_cli_client/commands/config.py
+timesketch_cli_client/commands/events.py
+timesketch_cli_client/commands/events_test.py
 timesketch_cli_client/commands/importer.py
 timesketch_cli_client/commands/search.py
 timesketch_cli_client/commands/search_test.py
+timesketch_cli_client/commands/sigma.py
+timesketch_cli_client/commands/sigma_test.py
 timesketch_cli_client/commands/sketch.py
 timesketch_cli_client/commands/sketch_test.py
 timesketch_cli_client/commands/timelines.py
 timesketch_cli_client/commands/timelines_test.py
```

