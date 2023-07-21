# Comparing `tmp/ptulsconv-1.0.7.tar.gz` & `tmp/ptulsconv-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptulsconv-1.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ptulsconv-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ptulsconv-1.0.7.tar` & `ptulsconv-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-06-03 02:45:27.925497 ptulsconv-1.0.7/LICENSE
--rw-r--r--   0        0        0     1241 2023-06-03 02:45:27.925497 ptulsconv-1.0.7/README.md
--rw-r--r--   0        0        0      216 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/__init__.py
--rw-r--r--   0        0        0     3930 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/__main__.py
--rw-r--r--   0        0        0     4130 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/broadcast_timecode.py
--rw-r--r--   0        0        0     8579 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/commands.py
--rw-r--r--   0        0        0       67 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/__init__.py
--rw-r--r--   0        0        0     4539 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/adr_entity.py
--rw-r--r--   0        0        0     5622 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/doc_entity.py
--rw-r--r--   0        0        0       34 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/generic_entity.py
--rw-r--r--   0        0        0     9996 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/pt_doc_parser.py
--rw-r--r--   0        0        0     8007 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/tag_compiler.py
--rw-r--r--   0        0        0     2922 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/tag_mapping.py
--rw-r--r--   0        0        0     2842 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/tagged_string_parser_visitor.py
--rw-r--r--   0        0        0      756 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/footage.py
--rw-r--r--   0        0        0      462 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/movie_export.py
--rw-r--r--   0        0        0    11941 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/__init__.py
--rw-r--r--   0        0        0     2075 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/continuity.py
--rw-r--r--   0        0        0    10181 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/line_count.py
--rw-r--r--   0        0        0       90 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/recordist_log.py
--rw-r--r--   0        0        0     5668 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/summary_log.py
--rw-r--r--   0        0        0    10063 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/supervisor_1pg.py
--rw-r--r--   0        0        0     2954 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/pdf/talent_sides.py
--rw-r--r--   0        0        0     2186 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/reporting.py
--rw-r--r--   0        0        0     2616 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/validations.py
--rw-r--r--   0        0        0     5494 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/xml/common.py
--rw-r--r--   0        0        0     3275 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/xslt/AvidMarkers.xsl
--rw-r--r--   0        0        0     1529 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/xslt/SRT.xsl
--rw-r--r--   0        0        0     1347 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 ptulsconv-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-21 21:29:59.710680 ptulsconv-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1241 2023-07-21 21:29:59.710680 ptulsconv-2.0.0/README.md
+-rw-r--r--   0        0        0      225 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/__init__.py
+-rw-r--r--   0        0        0     4074 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/__main__.py
+-rw-r--r--   0        0        0     4297 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/broadcast_timecode.py
+-rw-r--r--   0        0        0     9317 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/commands.py
+-rw-r--r--   0        0        0       68 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/docparser/__init__.py
+-rw-r--r--   0        0        0     4641 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/docparser/adr_entity.py
+-rw-r--r--   0        0        0     5835 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/docparser/doc_entity.py
+-rw-r--r--   0        0        0       36 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/generic_entity.py
+-rw-r--r--   0        0        0    10371 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/pt_doc_parser.py
+-rw-r--r--   0        0        0     7997 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/tag_compiler.py
+-rw-r--r--   0        0        0     2948 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/tag_mapping.py
+-rw-r--r--   0        0        0     2872 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/tagged_string_parser_visitor.py
+-rw-r--r--   0        0        0      754 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/footage.py
+-rw-r--r--   0        0        0      477 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/movie_export.py
+-rw-r--r--   0        0        0    12703 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/__init__.py
+-rw-r--r--   0        0        0     2102 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/continuity.py
+-rw-r--r--   0        0        0    11362 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/line_count.py
+-rw-r--r--   0        0        0       91 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/recordist_log.py
+-rw-r--r--   0        0        0     5826 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/summary_log.py
+-rw-r--r--   0        0        0    10929 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/supervisor_1pg.py
+-rw-r--r--   0        0        0     3188 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/talent_sides.py
+-rw-r--r--   0        0        0     2244 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/reporting.py
+-rw-r--r--   0        0        0     2869 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/validations.py
+-rw-r--r--   0        0        0     5909 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/xml/common.py
+-rw-r--r--   0        0        0     3275 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/xslt/AvidMarkers.xsl
+-rw-r--r--   0        0        0     1529 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/xslt/SRT.xsl
+-rw-r--r--   0        0        0     1336 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 ptulsconv-2.0.0/PKG-INFO
```

### Comparing `ptulsconv-1.0.7/LICENSE` & `ptulsconv-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.7/README.md` & `ptulsconv-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.7/ptulsconv/__main__.py` & `ptulsconv-2.0.0/ptulsconv/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,103 +1,114 @@
 from optparse import OptionParser, OptionGroup
 import datetime
 import sys
 
-from ptulsconv import __name__, __version__, __author__, __copyright__
+from ptulsconv import __name__, __copyright__
 from ptulsconv.commands import convert
-from ptulsconv.reporting import print_status_style, print_banner_style, print_section_header_style, print_fatal_error
+from ptulsconv.reporting import print_status_style, \
+    print_banner_style, print_section_header_style, \
+    print_fatal_error
 
 
 def dump_field_map(output=sys.stdout):
     from ptulsconv.docparser.tag_mapping import TagMapping
     from ptulsconv.docparser.adr_entity import ADRLine, GenericEvent
-    
+
     TagMapping.print_rules(GenericEvent, output=output)
     TagMapping.print_rules(ADRLine, output=output)
 
 
 def dump_formats():
     print_section_header_style("`raw` format:")
     sys.stderr.write("A JSON document of the parsed Pro Tools export.\n")
     print_section_header_style("`tagged` Format:")
-    sys.stderr.write("A JSON document containing one record for each clip, with\n"
-            "all tags parsed and all tagging rules applied. \n")
+    sys.stderr.write(
+        "A JSON document containing one record for each clip, with\n"
+        "all tags parsed and all tagging rules applied. \n")
     print_section_header_style("`doc` format:")
     sys.stderr.write("Creates a directory with folders for different types\n"
-            "of ADR reports.\n\n")
-
+                     "of ADR reports.\n\n")
 
 
 def main():
     """Entry point for the command-line invocation"""
     parser = OptionParser()
-    parser.usage = "ptulsconv [options] TEXT_EXPORT.txt"
+    parser.usage = "ptulsconv [options] [TEXT_EXPORT.txt]"
 
     parser.add_option('-f', '--format',
                       dest='output_format',
                       metavar='FMT',
                       choices=['raw', 'tagged', 'doc'],
                       default='doc',
                       help='Set output format, `raw`, `tagged`, `doc`.')
 
     warn_options = OptionGroup(title="Warning and Validation Options",
                                parser=parser)
 
     warn_options.add_option('-W', action='store_false',
                             dest='warnings',
                             default=True,
-                            help='Suppress warnings for common errors (missing code numbers etc.)')
+                            help='Suppress warnings for common '
+                            'errors (missing code numbers etc.)')
 
     parser.add_option_group(warn_options)
 
     informational_options = OptionGroup(title="Informational Options",
                                         parser=parser,
-                                        description='Print useful information and exit without processing '
-                                                    'input files.')
-
-    informational_options.add_option('--show-formats',
-            dest='show_formats',
-            action='store_true',
-            default=False,
-            help='Display helpful information about the '
-            'available output formats.')
-
-    informational_options.add_option('--show-available-tags',
-                                     dest='show_tags',
-                                     action='store_true',
-                                     default=False,
-                                     help='Display tag mappings for the FMP XML '
-                                          'output style and exit.')
+                                        description='Print useful '
+                                        'information '
+                                        'and exit without processing '
+                                        'input files.')
+
+    informational_options.add_option(
+        '--show-formats',
+        dest='show_formats',
+        action='store_true',
+        default=False,
+        help='Display helpful information about the available '
+        'output formats.')
+
+    informational_options.add_option(
+        '--show-available-tags',
+        dest='show_tags',
+        action='store_true',
+        default=False,
+        help='Display tag mappings for the FMP XML output style '
+        'and exit.')
 
     parser.add_option_group(informational_options)
 
     print_banner_style(__copyright__)
-    
-    (options, args) = parser.parse_args(sys.argv)
 
+    (options, args) = parser.parse_args(sys.argv)
 
     print_section_header_style("Startup")
-    print_status_style("This run started %s" % (datetime.datetime.now().isoformat()))
+    print_status_style("This run started %s" %
+                       (datetime.datetime.now().isoformat()))
 
     if options.show_tags:
         dump_field_map()
         sys.exit(0)
 
     elif options.show_formats:
         dump_formats()
         sys.exit(0)
-
-    if len(args) < 2:
-        print_fatal_error("Error: No input file")
-        parser.print_help(sys.stderr)
-        sys.exit(22)
-
     try:
         major_mode = options.output_format
-        convert(input_file=args[1], major_mode=major_mode, warnings=options.warnings)
+
+        if len(args) < 2:
+            print_status_style(
+                "No input file provided, will connect to Pro Tools "
+                "with PTSL...")
+            convert(major_mode=major_mode,
+                    warnings=options.warnings)
+        else:
+            convert(input_file=args[1],
+                    major_mode=major_mode,
+                    warnings=options.warnings)
 
     except FileNotFoundError as e:
         print_fatal_error("Error trying to read input file")
         raise e
 
     except Exception as e:
         import traceback
```

### Comparing `ptulsconv-1.0.7/ptulsconv/broadcast_timecode.py` & `ptulsconv-2.0.0/ptulsconv/broadcast_timecode.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,74 +5,82 @@
 import math
 import re
 from collections import namedtuple
 from fractions import Fraction
 from typing import Optional, SupportsFloat
 
 
-class TimecodeFormat(namedtuple("_TimecodeFormat", "frame_duration logical_fps drop_frame")):
+class TimecodeFormat(namedtuple("_TimecodeFormat",
+                                "frame_duration logical_fps drop_frame")):
     """
     A struct reperesenting a timecode datum.
     """
-    
+
     def smpte_to_seconds(self, smpte: str) -> Optional[Fraction]:
-        frame_count = smpte_to_frame_count(smpte, self.logical_fps, drop_frame_hint=self.drop_frame)
+        frame_count = smpte_to_frame_count(
+            smpte, self.logical_fps, drop_frame_hint=self.drop_frame)
         if frame_count is None:
             return None
         else:
             return frame_count * self.frame_duration
 
     def seconds_to_smpte(self, seconds: SupportsFloat) -> str:
         frame_count = int(seconds / self.frame_duration)
-        return frame_count_to_smpte(frame_count, self.logical_fps, self.drop_frame)
+        return frame_count_to_smpte(frame_count, self.logical_fps,
+                                    self.drop_frame)
 
 
-def smpte_to_frame_count(smpte_rep_string: str, frames_per_logical_second: int, drop_frame_hint=False) -> Optional[int]:
+def smpte_to_frame_count(smpte_rep_string: str, frames_per_logical_second: int,
+                         drop_frame_hint=False) -> Optional[int]:
     """
     Convert a string with a SMPTE timecode representation into a frame count.
 
     :param smpte_rep_string: The timecode string
-    :param frames_per_logical_second: Num of frames in a logical second. This is asserted to be
-            in one of `[24,25,30,48,50,60]`
-    :param drop_frame_hint: `True` if the timecode rep is drop frame. This is ignored (and implied `True`) if
-            the last separator in the timecode string is a semicolon. This is ignored (and implied `False`) if
-            `frames_per_logical_second` is not 30 or 60.
+    :param frames_per_logical_second: Num of frames in a logical second. This
+        is asserted to be in one of `[24,25,30,48,50,60]`
+    :param drop_frame_hint: `True` if the timecode rep is drop frame. This is
+        ignored (and implied `True`) if the last separator in the timecode
+        string is a semicolon. This is ignored (and implied `False`) if
+        `frames_per_logical_second` is not 30 or 60.
     """
     assert frames_per_logical_second in [24, 25, 30, 48, 50, 60]
 
-    m = re.search(r'(\d?\d)[:;](\d\d)[:;](\d\d)([:;])(\d\d)(\.\d+)?', smpte_rep_string)
-    
+    m = re.search(
+        r'(\d?\d)[:;](\d\d)[:;](\d\d)([:;])(\d\d)(\.\d+)?', smpte_rep_string)
+
     if m is None:
         return None
-    
+
     hh, mm, ss, sep, ff, frac = m.groups()
-    hh, mm, ss, ff, frac = int(hh), int(mm), int(ss), int(ff), float(frac or 0.0)
+    hh, mm, ss, ff, frac = int(hh), int(
+        mm), int(ss), int(ff), float(frac or 0.0)
 
     drop_frame = drop_frame_hint
     if sep == ";":
         drop_frame = True
 
     if frames_per_logical_second not in [30, 60]:
         drop_frame = False
 
-    raw_frames = hh * 3600 * frames_per_logical_second + mm * 60 * frames_per_logical_second + \
-                 ss * frames_per_logical_second + ff
+    raw_frames = hh * 3600 * frames_per_logical_second + mm * 60 * \
+        frames_per_logical_second + ss * frames_per_logical_second + ff
 
     frames = raw_frames
     if drop_frame is True:
         frames_dropped_per_inst = (frames_per_logical_second / 15)
         mins = hh * 60 + mm
         inst_count = mins - math.floor(mins / 10)
         dropped_frames = int(frames_dropped_per_inst) * inst_count
         frames = raw_frames - dropped_frames
 
     return frames
 
 
-def frame_count_to_smpte(frame_count: int, frames_per_logical_second: int, drop_frame: bool = False,
+def frame_count_to_smpte(frame_count: int, frames_per_logical_second: int,
+                         drop_frame: bool = False,
                          fractional_frame: Optional[float] = None) -> str:
     assert frames_per_logical_second in [24, 25, 30, 48, 50, 60]
     assert fractional_frame is None or fractional_frame < 1.0
 
     nominal_frames = frame_count
     separator = ":"
     if drop_frame:
@@ -86,15 +94,16 @@
 
     hh, rem = divmod(nominal_frames, frames_per_logical_second * 3600)
     mm, rem = divmod(rem, frames_per_logical_second * 60)
     ss, ff = divmod(rem, frames_per_logical_second)
 
     hh = hh % 24
     if fractional_frame is not None and fractional_frame > 0:
-        return "%02i:%02i:%02i%s%02i%s" % (hh, mm, ss, separator, ff, ("%.3f" % fractional_frame)[1:])
+        return "%02i:%02i:%02i%s%02i%s" % (hh, mm, ss, separator, ff,
+                                           ("%.3f" % fractional_frame)[1:])
     else:
         return "%02i:%02i:%02i%s%02i" % (hh, mm, ss, separator, ff)
 
 
 def footage_to_frame_count(footage_string) -> Optional[int]:
     m = re.search(r'(\d+)\+(\d+)(\.\d+)?', footage_string)
     if m is None:
```

### Comparing `ptulsconv-1.0.7/ptulsconv/commands.py` & `ptulsconv-2.0.0/ptulsconv/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 """
 import datetime
 import os
 
 import sys
 from itertools import chain
 import csv
-from typing import List
+from typing import List, Optional, Iterator
 from fractions import Fraction
 
-from .docparser.adr_entity import make_entities
-from .reporting import print_section_header_style, print_status_style, print_warning
-from .validations import *
+import ptsl
+
+from .docparser.adr_entity import make_entities, ADRLine
+from .reporting import print_section_header_style, print_status_style,\
+    print_warning
+from .validations import validate_unique_field, validate_non_empty_field,\
+    validate_dependent_value
 
 from ptulsconv.docparser import parse_document
 from ptulsconv.docparser.tag_compiler import TagCompiler
 from ptulsconv.broadcast_timecode import TimecodeFormat
-from fractions import Fraction
 
 from ptulsconv.pdf.supervisor_1pg import output_report as output_supervisor_1pg
 from ptulsconv.pdf.line_count import output_report as output_line_count
 from ptulsconv.pdf.talent_sides import output_report as output_talent_sides
 from ptulsconv.pdf.summary_log import output_report as output_summary
 from ptulsconv.pdf.continuity import output_report as output_continuity
 
@@ -34,100 +37,106 @@
     A subclass of :class:`JSONEncoder` which encodes :class:`Fraction` objects
     as a dict.
     """
     force_denominator: Optional[int]
 
     def default(self, o):
         """
-        
+
         """
         if isinstance(o, Fraction):
             return dict(numerator=o.numerator, denominator=o.denominator)
         else:
             return o.__dict__
 
 
 def output_adr_csv(lines: List[ADRLine], time_format: TimecodeFormat):
     """
-    Writes ADR lines as CSV to the current working directory. Creates directories
-    for each character number and name pair, and within that directory, creates
-    a CSV file for each reel.
+    Writes ADR lines as CSV to the current working directory. Creates
+    directories for each character number and name pair, and within that
+    directory, creates a CSV file for each reel.
     """
     reels = set([ln.reel for ln in lines])
 
     for n, name in [(n.character_id, n.character_name) for n in lines]:
         dir_name = "%s_%s" % (n, name)
         os.makedirs(dir_name, exist_ok=True)
         os.chdir(dir_name)
         for reel in reels:
-            these_lines = [ln for ln in lines if ln.character_id == n and ln.reel == reel]
+            these_lines = [ln for ln in lines
+                           if ln.character_id == n and ln.reel == reel]
 
             if len(these_lines) == 0:
                 continue
 
-            outfile_name = "%s_%s_%s_%s.csv" % (these_lines[0].title, n, these_lines[0].character_name, reel,)
+            outfile_name = "%s_%s_%s_%s.csv" % (these_lines[0].title, n,
+                                                these_lines[0].character_name,
+                                                reel,)
 
             with open(outfile_name, mode='w', newline='') as outfile:
                 writer = csv.writer(outfile, dialect='excel')
                 writer.writerow(['Title', 'Character Name', 'Cue Number',
                                  'Reel', 'Version',
                                  'Start', 'Finish',
                                  'Start Seconds', 'Finish Seconds',
                                  'Prompt',
                                  'Reason', 'Note', 'TV'])
 
                 for event in these_lines:
                     this_start = event.start or 0
                     this_finish = event.finish or 0
-                    this_row = [event.title, event.character_name, event.cue_number,
-                                event.reel, event.version,
-                                time_format.seconds_to_smpte(this_start), time_format.seconds_to_smpte(this_finish),
+                    this_row = [event.title, event.character_name,
+                                event.cue_number, event.reel, event.version,
+                                time_format.seconds_to_smpte(this_start),
+                                time_format.seconds_to_smpte(this_finish),
                                 float(this_start), float(this_finish),
                                 event.prompt,
-                                event.reason, event.note, "TV" if event.tv else ""]
+                                event.reason, event.note, "TV"
+                                if event.tv else ""]
 
                     writer.writerow(this_row)
         os.chdir("..")
 
 
-def generate_documents(session_tc_format, scenes, adr_lines: Iterator[ADRLine], title):
+def generate_documents(session_tc_format, scenes, adr_lines: Iterator[ADRLine],
+                       title):
     """
     Create PDF output.
     """
     print_section_header_style("Creating PDF Reports")
     report_date = datetime.datetime.now()
     reports_dir = "%s_%s" % (title, report_date.strftime("%Y-%m-%d_%H%M%S"))
     os.makedirs(reports_dir, exist_ok=False)
     os.chdir(reports_dir)
 
     client = next((x.client for x in adr_lines), "")
     supervisor = next((x.supervisor for x in adr_lines), "")
 
     output_continuity(scenes=scenes, tc_display_format=session_tc_format,
-                                  title=title, client=client, supervisor=supervisor)
+                      title=title, client=client,
+                      supervisor=supervisor)
 
-    # reels = sorted([r for r in compiler.compile_all_time_spans() if r[0] == 'Reel'],
-    #                key=lambda x: x[2])
     reels = ['R1', 'R2', 'R3', 'R4', 'R5', 'R6']
 
     if len(adr_lines) == 0:
-        print_status_style("No ADR lines were found in the "
-            "input document. ADR reports will not be generated.")
+        print_status_style("No ADR lines were found in the input document. "
+                           "ADR reports will not be generated.")
 
     else:
-        create_adr_reports(adr_lines, tc_display_format=session_tc_format, 
-            reel_list=sorted(reels))
+        create_adr_reports(adr_lines, tc_display_format=session_tc_format,
+                           reel_list=sorted(reels))
 
 
-def create_adr_reports(lines: List[ADRLine], tc_display_format: TimecodeFormat, reel_list: List[str]):
+def create_adr_reports(lines: List[ADRLine], tc_display_format: TimecodeFormat,
+                       reel_list: List[str]):
     """
-    Creates a directory heirarchy and a respective set of ADR reports, 
+    Creates a directory heirarchy and a respective set of ADR reports,
     given a list of lines.
     """
-    
+
     print_status_style("Creating ADR Report")
     output_summary(lines, tc_display_format=tc_display_format)
 
     print_status_style("Creating Line Count")
     output_line_count(lines, reel_list=reel_list)
 
     print_status_style("Creating Supervisor Logs directory and reports")
@@ -135,38 +144,56 @@
     os.chdir("Supervisor Logs")
     output_supervisor_1pg(lines, tc_display_format=tc_display_format)
     os.chdir("..")
 
     print_status_style("Creating Director's Logs director and reports")
     os.makedirs("Director Logs", exist_ok=True)
     os.chdir("Director Logs")
-    output_summary(lines, tc_display_format=tc_display_format, by_character=True)
+    output_summary(lines, tc_display_format=tc_display_format,
+                   by_character=True)
     os.chdir("..")
 
     print_status_style("Creating CSV outputs")
     os.makedirs("CSV", exist_ok=True)
     os.chdir("CSV")
     output_adr_csv(lines, time_format=tc_display_format)
     os.chdir("..")
 
     print_status_style("Creating Scripts directory and reports")
     os.makedirs("Talent Scripts", exist_ok=True)
     os.chdir("Talent Scripts")
     output_talent_sides(lines, tc_display_format=tc_display_format)
 
 
-def convert(input_file, major_mode, output=sys.stdout, warnings=True):
+def convert(major_mode, input_file=None, output=sys.stdout, warnings=True):
     """
     Primary worker function, accepts the input file and decides
     what to do with it based on the `major_mode`.
 
     :param input_file: a path to the input file.
     :param major_mode: the selected output mode, 'raw', 'tagged' or 'doc'.
     """
-    session = parse_document(input_file)
+    session_text = ""
+    if input_file is not None:
+        with open(input_file, "r") as file:
+            session_text = file.read()
+    else:
+        with ptsl.open_engine(
+                company_name="The ptulsconv developers",
+                application_name="ptulsconv") as engine:
+            req = engine.export_session_as_text()
+            req.utf8_encoding()
+            req.include_track_edls()
+            req.include_markers()
+            req.time_type("tc")
+            req.dont_show_crossfades()
+            req.selected_tracks_only()
+            session_text = req.export_string
+
+    session = parse_document(session_text)
     session_tc_format = session.header.timecode_format
 
     if major_mode == 'raw':
         output.write(MyEncoder().encode(session))
 
     else:
         compiler = TagCompiler()
@@ -175,48 +202,53 @@
 
         if major_mode == 'tagged':
             output.write(MyEncoder().encode(compiled_events))
 
         elif major_mode == 'doc':
             generic_events, adr_lines = make_entities(compiled_events)
 
-            scenes = sorted([s for s in compiler.compile_all_time_spans() if s[0] == 'Sc'],
+            scenes = sorted([s for s in compiler.compile_all_time_spans()
+                             if s[0] == 'Sc'],
                             key=lambda x: x[2])
 
             # TODO: Breakdown by titles
             titles = set([x.title for x in (generic_events + adr_lines)])
             if len(titles) != 1:
                 print_warning("Multiple titles per export is not supported, "
-                "found multiple titles: %s Exiting." % titles)
+                              "found multiple titles: %s Exiting." % titles)
                 exit(-1)
 
             title = list(titles)[0]
 
-            print_status_style("%i generic events found." % len(generic_events))
+            print_status_style(
+                "%i generic events found." % len(generic_events)
+            )
             print_status_style("%i ADR events found." % len(adr_lines))
 
             if warnings:
                 perform_adr_validations(adr_lines)
 
             generate_documents(session_tc_format, scenes, adr_lines, title)
-                
 
-def perform_adr_validations(lines : Iterator[ADRLine]):
+
+def perform_adr_validations(lines: Iterator[ADRLine]):
     """
     Performs validations on the input.
     """
-    for warning in chain(validate_unique_field(lines,
-                                               field='cue_number',
-                                               scope='title'),
-                         validate_non_empty_field(lines,
-                                                  field='cue_number'),
-                         validate_non_empty_field(lines,
-                                                  field='character_id'),
-                         validate_non_empty_field(lines,
-                                                  field='title'),
-                         validate_dependent_value(lines,
-                                                  key_field='character_id',
-                                                  dependent_field='character_name'),
-                         validate_dependent_value(lines,
-                                                  key_field='character_id',
-                                                  dependent_field='actor_name')):
+    for warning in chain(
+            validate_unique_field(lines,
+                                  field='cue_number',
+                                  scope='title'),
+            validate_non_empty_field(lines,
+                                     field='cue_number'),
+            validate_non_empty_field(lines,
+                                     field='character_id'),
+            validate_non_empty_field(lines,
+                                     field='title'),
+            validate_dependent_value(lines,
+                                     key_field='character_id',
+                                     dependent_field='character_name'),
+            validate_dependent_value(lines,
+                                     key_field='character_id',
+                                     dependent_field='actor_name')):
+
         print_warning(warning.report_message())
```

### Comparing `ptulsconv-1.0.7/ptulsconv/docparser/adr_entity.py` & `ptulsconv-2.0.0/ptulsconv/docparser/adr_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """
-This module defines classes and methods for converting :class:`Event` objects into 
-:class:`ADRLine` objects.
+This module defines classes and methods for converting :class:`Event` objects
+into :class:`ADRLine` objects.
 """
 
 from ptulsconv.docparser.tag_compiler import Event
-from typing import Optional, List, Tuple 
+from typing import Optional, List, Tuple
 from dataclasses import dataclass
 from fractions import Fraction
 
 from ptulsconv.docparser.tag_mapping import TagMapping
 
 
-def make_entities(from_events: List[Event]) -> Tuple[List['GenericEvent'], List['ADRLine']]:
+def make_entities(from_events: List[Event]) -> Tuple[List['GenericEvent'],
+                                                     List['ADRLine']]:
     """
     Accepts a list of Events and converts them into either ADRLine events or
     GenricEvents by calling :func:`make_entity` on each member.
 
     :param from_events: A list of `Event` objects.
 
-    :returns: A tuple of two lists, the first containing :class:`GenericEvent` and the 
-        second containing :class:`ADRLine`.
+    :returns: A tuple of two lists, the first containing :class:`GenericEvent`
+        and the second containing :class:`ADRLine`.
     """
     generic_events = list()
     adr_lines = list()
 
     for event in from_events:
         result = make_entity(event)
         if type(result) is ADRLine:
@@ -32,15 +33,15 @@
             generic_events.append(result)
 
     return generic_events, adr_lines
 
 
 def make_entity(from_event: Event) -> Optional[object]:
     """
-    Accepts an event and creates either an :class:`ADRLine` or a 
+    Accepts an event and creates either an :class:`ADRLine` or a
     :class:`GenericEvent`. An event is an "ADRLine" if it has a cue number/"QN"
     tag field.
 
     :param from_event:  An :class:`Event`.
 
     """
     instance = GenericEvent
@@ -63,37 +64,38 @@
 class GenericEvent:
     title: str = ""
     supervisor: Optional[str] = None
     client: Optional[str] = None
     scene: Optional[str] = None
     version: Optional[str] = None
     reel: Optional[str] = None
-    start: Fraction = Fraction(0,1)
-    finish: Fraction = Fraction(0,1)
+    start: Fraction = Fraction(0, 1)
+    finish: Fraction = Fraction(0, 1)
     omitted: bool = False
     note: Optional[str] = None
     requested_by: Optional[str] = None
 
     tag_mapping = [
-        TagMapping(source='Title', target="title", alt=TagMapping.ContentSource.Session),
+        TagMapping(source='Title', target="title",
+                   alt=TagMapping.ContentSource.Session),
         TagMapping(source="Supv", target="supervisor"),
         TagMapping(source="Client", target="client"),
         TagMapping(source="Sc", target="scene"),
         TagMapping(source="Ver", target="version"),
         TagMapping(source="Reel", target="reel"),
         TagMapping(source="Note", target="note"),
         TagMapping(source="Rq", target="requested_by"),
         TagMapping(source="OMIT", target="omitted",
                    formatter=(lambda x: len(x) > 0)),
     ]
 
 
 @dataclass
 class ADRLine(GenericEvent):
-    
+
     priority: Optional[int] = None
     cue_number: Optional[str] = None
     character_id: Optional[str] = None
     character_name: Optional[str] = None
     actor_name: Optional[str] = None
     prompt: Optional[str] = None
     reason: Optional[str] = None
@@ -107,17 +109,19 @@
     optional: bool = False
 
     tag_mapping = [
 
         TagMapping(source="P", target="priority"),
         TagMapping(source="QN", target="cue_number"),
         TagMapping(source="CN", target="character_id"),
-        TagMapping(source="Char", target="character_name", alt=TagMapping.ContentSource.Track),
+        TagMapping(source="Char", target="character_name",
+                   alt=TagMapping.ContentSource.Track),
         TagMapping(source="Actor", target="actor_name"),
-        TagMapping(source="Line", target="prompt", alt=TagMapping.ContentSource.Clip),
+        TagMapping(source="Line", target="prompt",
+                   alt=TagMapping.ContentSource.Clip),
         TagMapping(source="R", target="reason"),
         TagMapping(source="Mins", target="time_budget_mins",
                    formatter=(lambda n: float(n))),
         TagMapping(source="Spot", target="spot"),
         TagMapping(source="Shot", target="shot"),
         TagMapping(source="EFF", target="effort",
                    formatter=(lambda x: len(x) > 0)),
@@ -127,9 +131,7 @@
                    formatter=(lambda x: len(x) > 0)),
 
         TagMapping(source="ADLIB", target="adlib",
                    formatter=(lambda x: len(x) > 0)),
         TagMapping(source="OPT", target="optional",
                    formatter=(lambda x: len(x) > 0))
     ]
-
-
```

### Comparing `ptulsconv-1.0.7/ptulsconv/docparser/doc_entity.py` & `ptulsconv-2.0.0/ptulsconv/docparser/doc_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,32 @@
         self.clips = kwargs['clips']
         self.plugins = kwargs['plugins']
         self.tracks = kwargs['tracks']
         self.markers = kwargs['markers']
 
     def markers_timed(self) -> Iterator[Tuple['MarkerDescriptor', Fraction]]:
         for marker in self.markers:
-            marker_time = Fraction(marker.time_reference, int(self.header.sample_rate))
-            #marker_time = self.header.convert_timecode(marker.location)
+            marker_time = Fraction(marker.time_reference,
+                                   int(self.header.sample_rate))
+            # marker_time = self.header.convert_timecode(marker.location)
             yield marker, marker_time
 
-    def tracks_clips(self) -> Iterator[Tuple['TrackDescriptor', 'TrackClipDescriptor']]:
+    def tracks_clips(self) -> Iterator[Tuple['TrackDescriptor',
+                                             'TrackClipDescriptor']]:
         for track in self.tracks:
             for clip in track.clips:
                 yield track, clip
 
-    def track_clips_timed(self) -> Iterator[Tuple["TrackDescriptor", "TrackClipDescriptor",
-                                                  Fraction, Fraction, Fraction]]:
+    def track_clips_timed(self) -> Iterator[Tuple["TrackDescriptor",
+                                                  "TrackClipDescriptor",
+                                                  Fraction, Fraction, Fraction]
+                                            ]:
         """
-        :return: A Generator that yields track, clip, start time, finish time, and timestamp
+        :return: A Generator that yields track, clip, start time, finish time,
+        and timestamp
         """
         for track, clip in self.tracks_clips():
             start_time = self.header.convert_timecode(clip.start_timecode)
             finish_time = self.header.convert_timecode(clip.finish_timecode)
             timestamp_time = self.header.convert_timecode(clip.timestamp) \
                 if clip.timestamp is not None else None
 
@@ -101,15 +106,16 @@
                        "59.94": (60, Fraction(1001, 60_000)),
                        "60": (60, Fraction(1, 60))
                        }
 
         if self.timecode_fps in frame_rates.keys():
             return frame_rates[self.timecode_fps]
         else:
-            raise ValueError("Unrecognized TC rate (%s)" % self.timecode_format)
+            raise ValueError("Unrecognized TC rate (%s)" %
+                             self.timecode_format)
 
 
 class TrackDescriptor:
     name: str
     comments: str
     user_delay_samples: int
     state: List[str]
```

### Comparing `ptulsconv-1.0.7/ptulsconv/docparser/pt_doc_parser.py` & `ptulsconv-2.0.0/ptulsconv/docparser/pt_doc_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,97 +1,113 @@
 from parsimonious.nodes import NodeVisitor
 from parsimonious.grammar import Grammar
 
-from .doc_entity import SessionDescriptor, HeaderDescriptor, TrackDescriptor, FileDescriptor, \
-    TrackClipDescriptor, ClipDescriptor, PluginDescriptor, MarkerDescriptor
+from .doc_entity import SessionDescriptor, HeaderDescriptor, TrackDescriptor,\
+    FileDescriptor, TrackClipDescriptor, ClipDescriptor, PluginDescriptor,\
+    MarkerDescriptor
 
 
 protools_text_export_grammar = Grammar(
     r"""
-    document = header files_section? clips_section? plugin_listing? track_listing? markers_listing?
-    header   = "SESSION NAME:" fs string_value rs 
-               "SAMPLE RATE:" fs float_value rs 
-               "BIT DEPTH:" fs integer_value "-bit" rs 
-               "SESSION START TIMECODE:" fs string_value rs 
-               "TIMECODE FORMAT:" fs frame_rate " Drop"? " Frame" rs 
-               "# OF AUDIO TRACKS:" fs integer_value rs 
-               "# OF AUDIO CLIPS:" fs integer_value rs 
+    document = header files_section? clips_section? plugin_listing?
+               track_listing? markers_listing?
+    header   = "SESSION NAME:" fs string_value rs
+               "SAMPLE RATE:" fs float_value rs
+               "BIT DEPTH:" fs integer_value "-bit" rs
+               "SESSION START TIMECODE:" fs string_value rs
+               "TIMECODE FORMAT:" fs frame_rate " Drop"? " Frame" rs
+               "# OF AUDIO TRACKS:" fs integer_value rs
+               "# OF AUDIO CLIPS:" fs integer_value rs
                "# OF AUDIO FILES:" fs integer_value rs block_ending
-    
-    frame_rate           = ("60" / "59.94" / "30" / "29.97" / "25" / "24" / "23.976")
-    files_section        = files_header files_column_header file_record* block_ending
+
+    frame_rate           = ("60" / "59.94" / "30" / "29.97" / "25" / "24" /
+                           "23.976")
+    files_section        = files_header files_column_header file_record*
+                           block_ending
     files_header         = "F I L E S  I N  S E S S I O N" rs
     files_column_header  = "Filename" isp fs "Location" rs
     file_record          = string_value fs string_value rs
 
-    clips_section        = clips_header clips_column_header clip_record* block_ending
+    clips_section        = clips_header clips_column_header clip_record*
+                           block_ending
     clips_header         = "O N L I N E  C L I P S  I N  S E S S I O N" rs
     clips_column_header  = string_value fs string_value rs
-    clip_record          = string_value fs string_value (fs "[" integer_value "]")? rs
+    clip_record          = string_value fs string_value
+                           (fs "[" integer_value "]")? rs
 
-    plugin_listing       = plugin_header plugin_column_header plugin_record* block_ending
+    plugin_listing       = plugin_header plugin_column_header plugin_record*
+                           block_ending
     plugin_header        = "P L U G - I N S  L I S T I N G" rs
-    plugin_column_header = "MANUFACTURER            " fs "PLUG-IN NAME            " fs 
-                           "VERSION         " fs "FORMAT          " fs "STEMS                   " fs 
+    plugin_column_header = "MANUFACTURER            " fs
+                           "PLUG-IN NAME            " fs
+                           "VERSION         " fs
+                           "FORMAT          " fs
+                           "STEMS                   " fs
                            "NUMBER OF INSTANCES" rs
-    plugin_record        = string_value fs string_value fs string_value fs 
+    plugin_record        = string_value fs string_value fs string_value fs
                            string_value fs string_value fs string_value rs
 
     track_listing        = track_listing_header track_block*
     track_block          = track_list_top ( track_clip_entry / block_ending )*
-    
+
     track_listing_header = "T R A C K  L I S T I N G" rs
     track_list_top       = "TRACK NAME:" fs string_value rs
                            "COMMENTS:" fs string_value rs
                            "USER DELAY:" fs integer_value " Samples" rs
                            "STATE: " track_state_list rs
                            ("PLUG-INS: " ( fs string_value )* rs)?
-                           "CHANNEL " fs "EVENT   " fs "CLIP NAME                     " fs 
-                           "START TIME    " fs "END TIME      " fs "DURATION      " fs 
+                           "CHANNEL " fs "EVENT   " fs
+                           "CLIP NAME                     " fs
+                           "START TIME    " fs "END TIME      " fs
+                           "DURATION      " fs
                            ("TIMESTAMP         " fs)? "STATE" rs
-    
+
     track_state_list     = (track_state " ")*
-    
+
     track_state          = "Solo" / "Muted" / "Inactive" / "Hidden"
-    
-    track_clip_entry     = integer_value isp fs 
-                           integer_value isp fs 
-                           string_value fs 
-                           string_value fs string_value fs string_value fs (string_value fs)? 
+
+    track_clip_entry     = integer_value isp fs
+                           integer_value isp fs
+                           string_value fs
+                           string_value fs string_value fs string_value fs
+                           (string_value fs)?
                            track_clip_state rs
-                           
+
     track_clip_state     = ("Muted" / "Unmuted")
 
-    markers_listing        = markers_listing_header markers_column_header marker_record*
+    markers_listing        = markers_listing_header markers_column_header
+                             marker_record*
     markers_listing_header = "M A R K E R S  L I S T I N G" rs
-    markers_column_header  = "#   " fs "LOCATION     " fs "TIME REFERENCE    " fs 
-                             "UNITS    " fs "NAME                             " fs "COMMENTS" rs
+    markers_column_header  = "#   " fs "LOCATION     " fs
+                             "TIME REFERENCE    " fs
+                             "UNITS    " fs
+                             "NAME                             " fs
+                             "COMMENTS" rs
 
-    marker_record = integer_value isp fs string_value fs integer_value isp fs 
-                    string_value fs string_value fs string_value rs             
+    marker_record = integer_value isp fs string_value fs integer_value isp fs
+                    string_value fs string_value fs string_value rs
 
     fs = "\t"
     rs = "\n"
     block_ending = rs rs
     string_value   = ~r"[^\t\n]*"
     integer_value  = ~r"\d+"
     float_value    = ~r"\d+(\.\d+)?"
-    isp            = ~r"[^\d\t\n]*"    
+    isp            = ~r"[^\d\t\n]*"
     """)
 
 
-def parse_document(path: str) -> SessionDescriptor:
+def parse_document(session_text: str) -> SessionDescriptor:
     """
     Parse a Pro Tools text export.
-    :param path: path to a file
+    :param session_text: Pro Tools session text export
     :return: the session descriptor
     """
-    with open(path, 'r') as f:
-        ast = protools_text_export_grammar.parse(f.read())
-        return DocParserVisitor().visit(ast)
+    ast = protools_text_export_grammar.parse(session_text)
+    return DocParserVisitor().visit(ast)
 
 
 class DocParserVisitor(NodeVisitor):
 
     @staticmethod
     def visit_document(_, visited_children) -> SessionDescriptor:
         files = next(iter(visited_children[1]), None)
@@ -122,31 +138,36 @@
                                 timecode_drop_frame=tc_drop,
                                 count_audio_tracks=visited_children[25],
                                 count_clips=visited_children[29],
                                 count_files=visited_children[33])
 
     @staticmethod
     def visit_files_section(_, visited_children):
-        return list(map(lambda child: FileDescriptor(filename=child[0], path=child[2]), visited_children[2]))
+        return list(map(
+            lambda child: FileDescriptor(filename=child[0], path=child[2]),
+                    visited_children[2]))
 
     @staticmethod
     def visit_clips_section(_, visited_children):
         channel = next(iter(visited_children[2][3]), 1)
 
-        return list(map(lambda child: ClipDescriptor(clip_name=child[0], file=child[2], channel=channel),
-                        visited_children[2]))
+        return list(map(
+            lambda child: ClipDescriptor(clip_name=child[0], file=child[2],
+                                         channel=channel),
+            visited_children[2]))
 
     @staticmethod
     def visit_plugin_listing(_, visited_children):
-        return list(map(lambda child: PluginDescriptor(manufacturer=child[0],
-                                                       plugin_name=child[2],
-                                                       version=child[4],
-                                                       format=child[6],
-                                                       stems=child[8],
-                                                       count_instances=child[10]),
+        return list(map(lambda child:
+                        PluginDescriptor(manufacturer=child[0],
+                                         plugin_name=child[2],
+                                         version=child[4],
+                                         format=child[6],
+                                         stems=child[8],
+                                         count_instances=child[10]),
                         visited_children[2]))
 
     @staticmethod
     def visit_track_block(_, visited_children):
         track_header, track_clip_list = visited_children
         clips = []
         for clip in track_clip_list:
```

### Comparing `ptulsconv-1.0.7/ptulsconv/docparser/tag_compiler.py` & `ptulsconv-2.0.0/ptulsconv/docparser/tag_compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,32 +16,37 @@
     tags: Dict[str, str]
     start: Fraction
     finish: Fraction
 
 
 class TagCompiler:
     """
-    Uses a `SessionDescriptor` as a data source to produce `Intermediate` 
+    Uses a `SessionDescriptor` as a data source to produce `Intermediate`
     items.
     """
 
-    Intermediate = namedtuple('Intermediate', 'track_content track_tags track_comment_tags '
-                                              'clip_content clip_tags clip_tag_mode start finish')
+    Intermediate = namedtuple('Intermediate',
+                              'track_content track_tags track_comment_tags '
+                              'clip_content clip_tags clip_tag_mode start '
+                              'finish')
 
     session: doc_entity.SessionDescriptor
 
-    def compile_all_time_spans(self) -> List[Tuple[str, str, Fraction, Fraction]]:
+    def compile_all_time_spans(self) -> List[Tuple[str, str, Fraction,
+                                                   Fraction]]:
         """
-        :returns: A `List` of (key: str, value: str, start: Fraction, finish: Fraction)
+        :returns: A `List` of (key: str, value: str, start: Fraction,
+            finish: Fraction)
         """
         ret_list = list()
         for element in self.parse_data():
             if element.clip_tag_mode == TagPreModes.TIMESPAN:
                 for k in element.clip_tags.keys():
-                    ret_list.append((k, element.clip_tags[k], element.start, element.finish))
+                    ret_list.append((k, element.clip_tags[k], element.start,
+                                     element.finish))
 
         return ret_list
 
     def compile_tag_list(self) -> Dict[str, List[str]]:
         tags_dict = dict()
 
         def update_tags_dict(other_dict: dict):
@@ -69,34 +74,39 @@
     def compile_events(self) -> Iterator[Event]:
         step0 = self.parse_data()
         step1 = self.filter_out_directives(step0)
         step2 = self.apply_appends(step1)
         step3 = self.collect_time_spans(step2)
         step4 = self.apply_tags(step3)
         for datum in step4:
-            yield Event(clip_name=datum[0], track_name=datum[1], session_name=datum[2],
-                        tags=datum[3], start=datum[4], finish=datum[5])
+            yield Event(clip_name=datum[0], track_name=datum[1],
+                        session_name=datum[2], tags=datum[3], start=datum[4],
+                        finish=datum[5])
 
     def _marker_tags(self, at):
         retval = dict()
-        applicable = [(m, t) for (m, t) in self.session.markers_timed() if t <= at]
+
+        applicable = [(m, t) for (m, t) in
+                      self.session.markers_timed() if t <= at]
+
         for marker, _ in sorted(applicable, key=lambda x: x[1]):
             retval.update(parse_tags(marker.comments or "").tag_dict)
             retval.update(parse_tags(marker.name or "").tag_dict)
 
         return retval
 
-    def filter_out_directives(self, clips : Iterator[Intermediate]) -> Iterator[Intermediate]:
+    def filter_out_directives(self,
+                              clips: Iterator[Intermediate]) \
+            -> Iterator[Intermediate]:
         for clip in clips:
             if clip.clip_tag_mode == 'Directive':
                 continue
             else:
                 yield clip
 
-
     @staticmethod
     def _coalesce_tags(clip_tags: dict, track_tags: dict,
                        track_comment_tags: dict,
                        timespan_tags: dict,
                        marker_tags: dict, session_tags: dict):
         effective_tags = dict()
         effective_tags.update(session_tags)
@@ -113,37 +123,41 @@
             if clip.state == 'Muted':
                 continue
 
             track_parsed = parse_tags(track.name)
             track_comments_parsed = parse_tags(track.comments)
             clip_parsed = parse_tags(clip.clip_name)
 
-            yield TagCompiler.Intermediate(track_content=track_parsed.content,
-                                           track_tags=track_parsed.tag_dict,
-                                           track_comment_tags=track_comments_parsed.tag_dict,
-                                           clip_content=clip_parsed.content,
-                                           clip_tags=clip_parsed.tag_dict,
-                                           clip_tag_mode=clip_parsed.mode,
-                                           start=start, finish=finish)
+            yield TagCompiler.Intermediate(
+                track_content=track_parsed.content,
+                track_tags=track_parsed.tag_dict,
+                track_comment_tags=track_comments_parsed.tag_dict,
+                clip_content=clip_parsed.content,
+                clip_tags=clip_parsed.tag_dict,
+                clip_tag_mode=clip_parsed.mode,
+                start=start, finish=finish)
 
     @staticmethod
-    def apply_appends(parsed: Iterator[Intermediate]) -> Iterator[Intermediate]:
+    def apply_appends(parsed: Iterator[Intermediate]) -> \
+            Iterator[Intermediate]:
 
         def should_append(a, b):
-            return b.clip_tag_mode == TagPreModes.APPEND and b.start >= a.finish
+            return b.clip_tag_mode == TagPreModes.APPEND and \
+                b.start >= a.finish
 
         def do_append(a, b):
             merged_tags = dict(a.clip_tags)
             merged_tags.update(b.clip_tags)
-            return TagCompiler.Intermediate(track_content=a.track_content,
-                                            track_tags=a.track_tags,
-                                            track_comment_tags=a.track_comment_tags,
-                                            clip_content=a.clip_content + ' ' + b.clip_content,
-                                            clip_tags=merged_tags, clip_tag_mode=a.clip_tag_mode,
-                                            start=a.start, finish=b.finish)
+            return TagCompiler.Intermediate(
+                track_content=a.track_content,
+                track_tags=a.track_tags,
+                track_comment_tags=a.track_comment_tags,
+                clip_content=a.clip_content + ' ' + b.clip_content,
+                clip_tags=merged_tags, clip_tag_mode=a.clip_tag_mode,
+                start=a.start, finish=b.finish)
 
         yield from apply_appends(parsed, should_append, do_append)
 
     @staticmethod
     def collect_time_spans(parsed: Iterator[Intermediate]) -> \
             Iterator[Tuple[Intermediate, Tuple[dict, Fraction, Fraction]]]:
 
@@ -154,35 +168,39 @@
                 time_spans.append((item.clip_tags, item.start, item.finish))
             else:
                 yield item, list(time_spans)
 
     @staticmethod
     def _time_span_tags(at_time: Fraction, applicable_spans) -> dict:
         retval = dict()
-        for tags in reversed([a[0] for a in applicable_spans if a[1] <= at_time <= a[2]]):
+        for tags in reversed([a[0] for a in applicable_spans
+                              if a[1] <= at_time <= a[2]]):
             retval.update(tags)
 
         return retval
 
-    def apply_tags(self, parsed_with_time_spans) -> Iterator[Tuple[str, str, str, dict, Fraction, Fraction]]:
+    def apply_tags(self, parsed_with_time_spans) ->\
+            Iterator[Tuple[str, str, str, dict, Fraction, Fraction]]:
 
         session_parsed = parse_tags(self.session.header.session_name)
 
         for event, time_spans in parsed_with_time_spans:
             event: 'TagCompiler.Intermediate'
             marker_tags = self._marker_tags(event.start)
             time_span_tags = self._time_span_tags(event.start, time_spans)
-            tags = self._coalesce_tags(clip_tags=event.clip_tags,
-                                       track_tags=event.track_tags,
-                                       track_comment_tags=event.track_comment_tags,
-                                       timespan_tags=time_span_tags,
-                                       marker_tags=marker_tags,
-                                       session_tags=session_parsed.tag_dict)
+            tags = self._coalesce_tags(
+                    clip_tags=event.clip_tags,
+                    track_tags=event.track_tags,
+                    track_comment_tags=event.track_comment_tags,
+                    timespan_tags=time_span_tags,
+                    marker_tags=marker_tags,
+                    session_tags=session_parsed.tag_dict)
 
-            yield event.clip_content, event.track_content, session_parsed.content, tags, event.start, event.finish
+            yield (event.clip_content, event.track_content,
+                   session_parsed.content, tags, event.start, event.finish)
 
 
 def apply_appends(source: Iterator,
                   should_append: Callable,
                   do_append: Callable) -> Generator:
     """
     :param source:
```

### Comparing `ptulsconv-1.0.7/ptulsconv/docparser/tag_mapping.py` & `ptulsconv-2.0.0/ptulsconv/docparser/tag_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,16 @@
                     session_content: str,
                     to: object):
 
         done = set()
         for rule in rules:
             if rule.target in done:
                 continue
-            if rule.apply(tags, clip_content, track_content, session_content, to):
+            if rule.apply(tags, clip_content, track_content, session_content,
+                          to):
                 done.update(rule.target)
 
     def __init__(self, source: str,
                  target: str,
                  alt: Optional[ContentSource] = None,
                  formatter=None):
         self.source = source
```

### Comparing `ptulsconv-1.0.7/ptulsconv/docparser/tagged_string_parser_visitor.py` & `ptulsconv-2.0.0/ptulsconv/docparser/tagged_string_parser_visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from parsimonious import NodeVisitor, Grammar
-from typing import Dict, Union
+from typing import Dict
 from enum import Enum
 
 
 class TagPreModes(Enum):
     NORMAL = 'Normal'
     APPEND = 'Append'
     TIMESPAN = 'Timespan'
@@ -48,16 +48,17 @@
 class TagListVisitor(NodeVisitor):
 
     @staticmethod
     def visit_document(_, visited_children) -> TaggedStringResult:
         modifier_opt, line_opt, _, tag_list_opt = visited_children
 
         return TaggedStringResult(content=next(iter(line_opt), None),
-                                    tag_dict=next(iter(tag_list_opt), dict()),
-                                  mode=TagPreModes(next(iter(modifier_opt), 'Normal'))
+                                  tag_dict=next(iter(tag_list_opt), dict()),
+                                  mode=TagPreModes(
+                                      next(iter(modifier_opt), 'Normal'))
                                   )
 
     @staticmethod
     def visit_line(node, _):
         return str.strip(node.text, " ")
 
     @staticmethod
```

### Comparing `ptulsconv-1.0.7/ptulsconv/footage.py` & `ptulsconv-2.0.0/ptulsconv/footage.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from fractions import Fraction
 import re
 from typing import Optional
 
 
 def footage_to_seconds(footage: str) -> Optional[Fraction]:
     """
-    Converts a string representation of a footage (35mm, 24fps) 
-    into a :class:`Fraction`, this fraction being a some number of 
+    Converts a string representation of a footage (35mm, 24fps)
+    into a :class:`Fraction`, this fraction being a some number of
     seconds.
 
     :param footage: A string reprenentation of a footage of the form
         resembling "90+01".
     """
     m = re.match(r'(\d+)\+(\d+)(\.\d+)?', footage)
     if m is None:
```

### Comparing `ptulsconv-1.0.7/ptulsconv/pdf/__init__.py` & `ptulsconv-2.0.0/ptulsconv/pdf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 # TODO: A Generic report useful for spotting
 # TODO: A report useful for M&E mixer's notes
 # TODO: Use a default font that doesn't need to be installed
 
 # This is from https://code.activestate.com/recipes/576832/ for
 # generating page count messages
+
+
 class ReportCanvas(canvas.Canvas):
     def __init__(self, *args, **kwargs):
         canvas.Canvas.__init__(self, *args, **kwargs)
         self._saved_page_states = []
         self._report_date = datetime.datetime.now()
 
     def showPage(self):
@@ -34,18 +36,20 @@
             self.__dict__.update(state)
             self.draw_page_number(num_pages)
             canvas.Canvas.showPage(self)
         canvas.Canvas.save(self)
 
     def draw_page_number(self, page_count):
         self.saveState()
-        self.setFont('Helvetica', 10) #FIXME make this customizable
-        self.drawString(0.5 * inch, 0.5 * inch, "Page %d of %d" % (self._pageNumber, page_count))
+        self.setFont('Helvetica', 10)  # FIXME make this customizable
+        self.drawString(0.5 * inch, 0.5 * inch,
+                        "Page %d of %d" % (self._pageNumber, page_count))
         right_edge = self._pagesize[0] - 0.5 * inch
-        self.drawRightString(right_edge, 0.5 * inch, self._report_date.strftime("%m/%d/%Y %H:%M"))
+        self.drawRightString(right_edge, 0.5 * inch,
+                             self._report_date.strftime("%m/%d/%Y %H:%M"))
 
         top_line = self.beginPath()
         top_line.moveTo(0.5 * inch, 0.75 * inch)
         top_line.lineTo(right_edge, 0.75 * inch)
         self.setLineWidth(0.5)
         self.drawPath(top_line)
         self.restoreState()
@@ -70,24 +74,26 @@
     _, page_box = page_box.split_x(right_margin, direction='r')
     _, page_box = page_box.split_y(bottom_margin, direction='u')
     _, page_box = page_box.split_y(top_margin, direction='d')
 
     footer_box, page_box = page_box.split_y(0.25 * inch, direction='u')
     header_box, page_box = page_box.split_y(0.75 * inch, direction='d')
     title_box, report_box = header_box.split_x(3.5 * inch, direction='r')
-    
-    on_page_lambda = (lambda c, _: 
-        draw_header_footer(c, report_box, title_box, 
-        footer_box,title=title, 
-        supervisor=supervisor,     
-        document_subheader=document_subheader, 
-        client=client, doc_title=document_header))
-    
-    frames = [Frame(page_box.min_x, page_box.min_y, page_box.width, page_box.height)]
-    
+
+    on_page_lambda = (lambda c, _:
+                      draw_header_footer(c, report_box, title_box,
+                                         footer_box, title=title,
+                                         supervisor=supervisor,
+                                         document_subheader=document_subheader,
+                                         client=client,
+                                         doc_title=document_header))
+
+    frames = [Frame(page_box.min_x, page_box.min_y,
+                    page_box.width, page_box.height)]
+
     page_template = PageTemplate(id="Main",
                                  frames=frames,
                                  onPage=on_page_lambda)
 
     for font in fonts:
         pdfmetrics.registerFont(font)
 
@@ -115,44 +121,53 @@
         return "%im" % round(mins)
     else:
         m = round(mins)
         hh, mm = divmod(m, 60)
         return "%i:%02i" % (hh, mm)
 
 
-def draw_header_footer(a_canvas: ReportCanvas, left_box, right_box, footer_box, title: str, supervisor: str,
-                       document_subheader: str, client: str, doc_title="", font_name='Helvetica'):
-
-    (_supervisor_box, client_box,), title_box = right_box.divide_y([16., 16., ])
-    title_box.draw_text_cell(a_canvas, title, font_name, 18, inset_y=2., inset_x=5.)
-    client_box.draw_text_cell(a_canvas, client, font_name, 11, inset_y=2., inset_x=5.)
+def draw_header_footer(a_canvas: ReportCanvas, left_box, right_box,
+                       footer_box, title: str, supervisor: str,
+                       document_subheader: str, client: str, doc_title="",
+                       font_name='Helvetica'):
+
+    (_supervisor_box, client_box,), title_box = \
+        right_box.divide_y([16., 16., ])
+    title_box.draw_text_cell(a_canvas, title, font_name, 18,
+                             inset_y=2., inset_x=5.)
+    client_box.draw_text_cell(a_canvas, client, font_name, 11,
+                              inset_y=2., inset_x=5.)
 
     a_canvas.saveState()
     a_canvas.setLineWidth(0.5)
     tline = a_canvas.beginPath()
     tline.moveTo(left_box.min_x, right_box.min_y)
     tline.lineTo(right_box.max_x, right_box.min_y)
     a_canvas.drawPath(tline)
 
     tline2 = a_canvas.beginPath()
     tline2.moveTo(right_box.min_x, left_box.min_y)
     tline2.lineTo(right_box.min_x, left_box.max_y)
     a_canvas.drawPath(tline2)
     a_canvas.restoreState()
 
-    (doc_title_cell, spotting_version_cell,), _ = left_box.divide_y([18., 14], direction='d')
+    (doc_title_cell, spotting_version_cell,), _ = \
+        left_box.divide_y([18., 14], direction='d')
 
-    doc_title_cell.draw_text_cell(a_canvas, doc_title, font_name, 14., inset_y=2.)
+    doc_title_cell.draw_text_cell(a_canvas, doc_title, font_name, 14.,
+                                  inset_y=2.)
 
     if document_subheader is not None:
-        spotting_version_cell.draw_text_cell(a_canvas, document_subheader, font_name, 12., inset_y=2.)
+        spotting_version_cell.draw_text_cell(a_canvas, document_subheader,
+                                             font_name, 12., inset_y=2.)
 
     if supervisor is not None:
         a_canvas.setFont(font_name, 11.)
-        a_canvas.drawCentredString(footer_box.min_x + footer_box.width / 2., footer_box.min_y, supervisor)
+        a_canvas.drawCentredString(footer_box.min_x + footer_box.width / 2.,
+                                   footer_box.min_y, supervisor)
 
 
 class GRect:
     def __init__(self, x, y, width, height, debug_name=None):
         self.x = x
         self.y = y
         self.width = width
@@ -197,40 +212,46 @@
         if at >= self.width:
             return None, self
         elif at <= 0:
             return self, None
         else:
             if direction == 'l':
                 return (GRect(self.min_x, self.min_y, at, self.height),
-                        GRect(self.min_x + at, self.y, self.width - at, self.height))
+                        GRect(self.min_x + at, self.y,
+                              self.width - at, self.height))
             else:
                 return (GRect(self.max_x - at, self.y, at, self.height),
-                        GRect(self.min_x, self.y, self.width - at, self.height))
+                        GRect(self.min_x, self.y,
+                              self.width - at, self.height))
 
     def split_y(self, at, direction='u'):
         if at >= self.height:
             return None, self
         elif at <= 0:
             return self, None
         else:
             if direction == 'u':
                 return (GRect(self.x, self.y, self.width, at),
-                        GRect(self.x, self.y + at, self.width, self.height - at))
+                        GRect(self.x, self.y + at,
+                              self.width, self.height - at))
             else:
                 return (GRect(self.x, self.max_y - at, self.width, at),
-                        GRect(self.x, self.y, self.width, self.height - at))
+                        GRect(self.x, self.y,
+                              self.width, self.height - at))
 
     def inset_xy(self, dx, dy):
-        return GRect(self.x + dx, self.y + dy, self.width - dx * 2, self.height - dy * 2)
+        return GRect(self.x + dx, self.y + dy,
+                     self.width - dx * 2, self.height - dy * 2)
 
     def inset(self, d):
         return self.inset_xy(d, d)
 
     def __repr__(self):
-        return "<GRect x=%f y=%f width=%f height=%f>" % (self.x, self.y, self.width, self.height)
+        return "<GRect x=%f y=%f width=%f height=%f>" % \
+            (self.x, self.y, self.width, self.height)
 
     def divide_x(self, x_list, direction='l'):
         ret_list = list()
 
         rem = self
         for item in x_list:
             s, rem = rem.split_x(item, direction)
@@ -255,21 +276,25 @@
         a_canvas.drawString(self.x, self.y, self.debug_name or self.__repr__())
         a_canvas.restoreState()
 
     def draw_border(self, a_canvas, edge):
 
         def draw_border_impl(en):
             if en == 'min_x':
-                coordinates = ((self.min_x, self.min_y), (self.min_x, self.max_y))
+                coordinates = ((self.min_x, self.min_y),
+                               (self.min_x, self.max_y))
             elif en == 'max_x':
-                coordinates = ((self.max_x, self.min_y), (self.max_x, self.max_y))
+                coordinates = ((self.max_x, self.min_y),
+                               (self.max_x, self.max_y))
             elif en == 'min_y':
-                coordinates = ((self.min_x, self.min_y), (self.max_x, self.min_y))
+                coordinates = ((self.min_x, self.min_y),
+                               (self.max_x, self.min_y))
             elif en == 'max_y':
-                coordinates = ((self.min_x, self.max_y), (self.max_x, self.max_y))
+                coordinates = ((self.min_x, self.max_y),
+                               (self.max_x, self.max_y))
             else:
                 return
 
             s = a_canvas.beginPath()
             s.moveTo(*coordinates[0])
             s.lineTo(*coordinates[1])
             a_canvas.drawPath(s)
```

### Comparing `ptulsconv-1.0.7/ptulsconv/pdf/continuity.py` & `ptulsconv-2.0.0/ptulsconv/pdf/continuity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from fractions import Fraction
 from typing import Tuple, List
 
 from reportlab.lib.pagesizes import portrait, letter
 from reportlab.lib.styles import getSampleStyleSheet
 from reportlab.lib.units import inch
-from reportlab.platypus import Paragraph, Table, Spacer
+from reportlab.platypus import Paragraph, Table
 
 from ptulsconv.broadcast_timecode import TimecodeFormat
 from ptulsconv.pdf import make_doc_template
 
 
 # TODO: A Continuity
 
-def table_for_scene(scene, tc_format, font_name = 'Helvetica'):
+def table_for_scene(scene, tc_format, font_name='Helvetica'):
     scene_style = getSampleStyleSheet()['Normal']
     scene_style.fontName = font_name
     scene_style.leftIndent = 0.
     scene_style.leftPadding = 0.
     scene_style.spaceAfter = 18.
 
-    tc_data = "<em>%s</em><br />%s" % (tc_format.seconds_to_smpte(scene[2]), tc_format.seconds_to_smpte(scene[3]))
+    tc_data = "<em>%s</em><br />%s" % (tc_format.seconds_to_smpte(scene[2]),
+                                       tc_format.seconds_to_smpte(scene[3]))
 
     row = [
         Paragraph(tc_data, scene_style),
         Paragraph(scene[1], scene_style),
     ]
 
     style = [('VALIGN', (0, 0), (-1, -1), 'TOP'),
@@ -32,15 +33,15 @@
              ('FONTNAME', (0, 0), (-1, -1), font_name)]
 
     return Table(data=[row], style=style, colWidths=[1.0 * inch, 6.5 * inch])
 
 
 def output_report(scenes: List[Tuple[str, str, Fraction, Fraction]],
                   tc_display_format: TimecodeFormat,
-                  title: str, client: str, supervisor, paper_size = letter):
+                  title: str, client: str, supervisor, paper_size=letter):
     filename = "%s Continuity.pdf" % title
     document_header = "Continuity"
 
     doc = make_doc_template(page_size=portrait(paper_size),
                             filename=filename,
                             document_title="Continuity",
                             title=title,
```

### Comparing `ptulsconv-1.0.7/ptulsconv/pdf/line_count.py` & `ptulsconv-2.0.0/ptulsconv/pdf/line_count.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from typing import List, Optional
 
-from reportlab.pdfbase import pdfmetrics
-from reportlab.pdfbase.ttfonts import TTFont
+# from reportlab.pdfbase import pdfmetrics
+# from reportlab.pdfbase.ttfonts import TTFont
 
 from reportlab.lib.units import inch
 from reportlab.lib.pagesizes import letter, portrait
 from reportlab.lib import colors
 
 from reportlab.platypus import Table, Paragraph, Spacer
 from reportlab.lib.styles import getSampleStyleSheet
 
 from .__init__ import time_format, make_doc_template
 from ..docparser.adr_entity import ADRLine
 
 
-def build_columns(lines: List[ADRLine], reel_list: Optional[List[str]], show_priorities=False, include_omitted=False):
+def build_columns(lines: List[ADRLine], reel_list: Optional[List[str]],
+                  show_priorities=False, include_omitted=False):
     columns = list()
-    reel_numbers = reel_list or sorted(set([x.reel for x in lines if x.reel is not None]))
+    reel_numbers = reel_list or sorted(
+        set([x.reel for x in lines if x.reel is not None])
+    )
 
     num_column_width = 15. / 32. * inch
 
     columns.append({
         'heading': '#',
         'value_getter': lambda recs: recs[0].character_id,
         'value_getter2': lambda recs: "",
@@ -29,46 +32,67 @@
         'summarize': False
     })
 
     columns.append({
         'heading': 'Role',
         'value_getter': lambda recs: recs[0].character_name,
         'value_getter2': lambda recs: recs[0].actor_name or "",
-        'style_getter': lambda col_index: [('LINEAFTER', (col_index, 0), (col_index, -1), 1.0, colors.black)],
+        'style_getter': lambda col_index: [('LINEAFTER',
+                                            (col_index, 0),
+                                            (col_index, -1),
+                                            1.0, colors.black)],
         'width': 1.75 * inch,
         'summarize': False
     })
 
     columns.append({
         'heading': 'TV',
         'value_getter': lambda recs: len([r for r in recs if r.tv]),
-        'value_getter2': lambda recs: time_format(sum([r.time_budget_mins or 0.
-                                                       for r in recs if r.tv])),
-        'style_getter': lambda col_index: [('ALIGN', (col_index, 0), (col_index, -1), 'CENTER'),
-                                           ('LINEBEFORE', (col_index, 0), (col_index, -1), 1., colors.black),
-                                           ('LINEAFTER', (col_index, 0), (col_index, -1), .5, colors.gray)],
+        'value_getter2': (lambda recs:
+                          time_format(sum([r.time_budget_mins or 0.
+                                           for r in recs if r.tv]))
+                          ),
+        'style_getter': (lambda col_index:
+                         [('ALIGN', (col_index, 0), (col_index, -1),
+                           'CENTER'),
+                          ('LINEBEFORE', (col_index, 0), (col_index, -1),
+                           1., colors.black),
+                          ('LINEAFTER', (col_index, 0), (col_index, -1),
+                           .5, colors.gray)]
+                         ),
         'width': num_column_width
     })
 
     columns.append({
         'heading': 'Opt',
         'value_getter': lambda recs: len([r for r in recs if r.optional]),
-        'value_getter2': lambda recs: time_format(sum([r.time_budget_mins or 0.
-                                                       for r in recs if r.optional])),
-        'style_getter': lambda col_index: [('ALIGN', (col_index, 0), (col_index, -1), 'CENTER'),
-                                           ('LINEAFTER', (col_index, 0), (col_index, -1), .5, colors.gray)],
+        'value_getter2': (lambda recs:
+                          time_format(sum([r.time_budget_mins or 0.
+                                           for r in recs if r.optional]))
+                          ),
+        'style_getter': (lambda col_index:
+                         [('ALIGN', (col_index, 0), (col_index, -1),
+                           'CENTER'),
+                          ('LINEAFTER', (col_index, 0), (col_index, -1),
+                           .5, colors.gray)]
+                         ),
         'width': num_column_width
     })
 
     columns.append({
         'heading': 'Eff',
         'value_getter': lambda recs: len([r for r in recs if r.effort]),
-        'value_getter2': lambda recs: time_format(sum([r.time_budget_mins or 0.
-                                                       for r in recs if r.effort])),
-        'style_getter': lambda col_index: [('ALIGN', (col_index, 0), (col_index, -1), 'CENTER')],
+        'value_getter2': (lambda recs:
+                          time_format(sum([r.time_budget_mins or 0.
+                                           for r in recs if r.effort]))
+                          ),
+        'style_getter': (lambda col_index:
+                         [('ALIGN', (col_index, 0), (col_index, -1),
+                           'CENTER')]
+                         ),
         'width': num_column_width
     })
 
     columns.append({
         'heading': '',
         'value_getter': lambda _: '',
         'value_getter2': lambda _: '',
@@ -76,84 +100,110 @@
             ('LINEBEFORE', (col_index, 0), (col_index, -1), 1., colors.black),
             ('LINEAFTER', (col_index, 0), (col_index, -1), 1., colors.black),
         ],
         'width': 2.
     })
 
     if len(reel_numbers) > 0:
-        # columns.append({
-        #     'heading': 'RX',
-        #     'value_getter': lambda recs: blank_len([r for r in recs if 'Reel' not in r.keys()]),
-        #     'value_getter2': lambda recs: time_format(sum([r.get('Time Budget Mins', 0.) for r in recs
-        #                                                    if 'Reel' not in r.keys()])),
-        #     'style_getter': lambda col_index: [('ALIGN', (col_index, 0), (col_index, -1), 'CENTER')],
-        #     'width': num_column_width
-        # })
 
         for n in reel_numbers:
             columns.append({
                 'heading': n,
-                'value_getter': lambda recs, n1=n: len([r for r in recs if r.reel == n1]),
-                'value_getter2': lambda recs, n1=n: time_format(sum([r.time_budget_mins or 0. for r
-                                                                     in recs if r.reel == n1])),
-                'style_getter': lambda col_index: [('ALIGN', (col_index, 0), (col_index, -1), 'CENTER'),
-                                                   ('LINEAFTER', (col_index, 0), (col_index, -1), .5, colors.gray)],
+                'value_getter': (lambda recs, n1=n:
+                                 len([r for r in recs if r.reel == n1])
+                                 ),
+                'value_getter2': (lambda recs, n1=n:
+                                  time_format(sum([r.time_budget_mins or 0.
+                                                   for r in recs
+                                                   if r.reel == n1]))
+                                  ),
+                'style_getter': (lambda col_index:
+                                 [('ALIGN', (col_index, 0), (col_index, -1),
+                                   'CENTER'),
+                                  ('LINEAFTER', (col_index, 0),
+                                   (col_index, -1),
+                                   .5, colors.gray)]
+                                 ),
+
                 'width': num_column_width
             })
 
     if show_priorities:
         for n in range(1, 6,):
             columns.append({
                 'heading': 'P%i' % n,
-                'value_getter': lambda recs: len([r for r in recs if r.priority == n]),
-                'value_getter2': lambda recs: time_format(sum([r.time_budget_mins or 0.
-                                                               for r in recs if r.priority == n])),
+                'value_getter': lambda recs: len([r for r in recs
+                                                  if r.priority == n]),
+                'value_getter2': (lambda recs:
+                                  time_format(sum([r.time_budget_mins or 0.
+                                                   for r in recs
+                                                   if r.priority == n]))
+                                  ),
                 'style_getter': lambda col_index: [],
                 'width': num_column_width
             })
 
         columns.append({
             'heading': '>P5',
-            'value_getter': lambda recs: len([r for r in recs if (r.priority or 5) > 5]),
-            'value_getter2': lambda recs: time_format(sum([r.time_budget_mins or 0.
-                                                           for r in recs if (r.priority or 5) > 5])),
+            'value_getter': lambda recs: len([r for r in recs
+                                              if (r.priority or 5) > 5]),
+            'value_getter2': (lambda recs:
+                              time_format(sum([r.time_budget_mins or 0.
+                                               for r in recs
+                                               if (r.priority or 5) > 5]))
+                              ),
             'style_getter': lambda col_index: [],
             'width': num_column_width
         })
 
     if include_omitted:
         columns.append({
             'heading': 'Omit',
             'value_getter': lambda recs: len([r for r in recs if r.omitted]),
-            'value_getter2': lambda recs: time_format(sum([r.time_budget_mins or 0.
-                                                           for r in recs if r.omitted])),
-            'style_getter': lambda col_index: [('ALIGN', (col_index, 0), (col_index, -1), 'CENTER')],
+            'value_getter2': (lambda recs:
+                              time_format(sum([r.time_budget_mins or 0.
+                                               for r in recs if r.omitted]))),
+            'style_getter': (lambda col_index:
+                             [('ALIGN', (col_index, 0), (col_index, -1),
+                               'CENTER')]
+                             ),
             'width': num_column_width
         })
 
     columns.append({
         'heading': 'Total',
         'value_getter': lambda recs: len([r for r in recs if not r.omitted]),
-        'value_getter2': lambda recs: time_format(sum([r.time_budget_mins or 0.
-                                                       for r in recs if not r.omitted]), zero_str=None),
-        'style_getter': lambda col_index: [('LINEBEFORE', (col_index, 0), (col_index, -1), 1.0, colors.black),
-                                           ('ALIGN', (col_index, 0), (col_index, -1), 'CENTER')],
+        'value_getter2': (lambda recs:
+                          time_format(
+                              sum([r.time_budget_mins or 0.
+
+                                   for r in recs if not r.omitted])
+                          )
+                          ),
+        'style_getter': (lambda col_index:
+                         [('LINEBEFORE', (col_index, 0), (col_index, -1),
+                           1.0, colors.black),
+                          ('ALIGN', (col_index, 0), (col_index, -1),
+                           'CENTER')]
+                         ),
         'width': 0.5 * inch
     })
 
     return columns
 
 
-def populate_columns(lines: List[ADRLine], columns, include_omitted, _page_size):
+def populate_columns(lines: List[ADRLine], columns, include_omitted,
+                     _page_size):
     data = list()
     styles = list()
     columns_widths = list()
 
-    sorted_character_numbers: List[str] = sorted(set([x.character_id for x in lines]),
-                                      key=lambda x: str(x))
+    sorted_character_numbers: List[str] = sorted(
+        set([x.character_id for x in lines]),
+        key=lambda x: str(x))
 
     # construct column styles
 
     for i, c in enumerate(columns):
         styles.extend(c['style_getter'](i))
         columns_widths.append(c['width'])
 
@@ -170,16 +220,18 @@
 
             for col in columns:
                 row1_index = len(data)
                 row2_index = row1_index + 1
                 row_data.append(col['value_getter'](list(char_records)))
                 row_data2.append(col['value_getter2'](list(char_records)))
 
-                styles.extend([('TEXTCOLOR', (0, row2_index), (-1, row2_index), colors.red),
-                               ('LINEBELOW', (0, row2_index), (-1, row2_index), 0.5, colors.black)])
+                styles.extend([('TEXTCOLOR', (0, row2_index), (-1, row2_index),
+                                colors.red),
+                               ('LINEBELOW', (0, row2_index), (-1, row2_index),
+                                0.5, colors.black)])
 
             data.append(row_data)
             data.append(row_data2)
 
     summary_row1 = list()
     summary_row2 = list()
     row1_index = len(data)
@@ -188,59 +240,65 @@
         if col.get('summarize', True):
             summary_row1.append(col['value_getter'](lines))
             summary_row2.append(col['value_getter2'](lines))
         else:
             summary_row1.append("")
             summary_row2.append("")
 
-    styles.append(('LINEABOVE', (0, row1_index), (-1, row1_index), 2.0, colors.black))
+    styles.append(('LINEABOVE', (0, row1_index), (-1, row1_index), 2.0,
+                   colors.black))
 
     data.append(summary_row1)
     data.append(summary_row2)
 
     return data, styles, columns_widths
 
 
 # def build_header(column_widths):
 #     pass
 
 
-def output_report(lines: List[ADRLine], reel_list: List[str], include_omitted=False,
-                  page_size=portrait(letter), font_name='Helvetica'):
-    columns = build_columns(lines, include_omitted=include_omitted, reel_list=reel_list)
-    data, style, columns_widths = populate_columns(lines, columns, include_omitted, page_size)
+def output_report(lines: List[ADRLine], reel_list: List[str],
+                  include_omitted=False, page_size=portrait(letter),
+                  font_name='Helvetica'):
+    columns = build_columns(lines, include_omitted=include_omitted,
+                            reel_list=reel_list)
+    data, style, columns_widths = populate_columns(lines, columns,
+                                                   include_omitted, page_size)
 
     style.append(('FONTNAME', (0, 0), (-1, -1), font_name))
     style.append(('FONTSIZE', (0, 0), (-1, -1), 9.))
     style.append(('LINEBELOW', (0, 0), (-1, 0), 1.0, colors.black))
     # style.append(('LINEBELOW', (0, 1), (-1, -1), 0.25, colors.gray))
 
-    #pdfmetrics.registerFont(TTFont('Futura', 'Futura.ttc'))
+    # pdfmetrics.registerFont(TTFont('Futura', 'Futura.ttc'))
 
     title = "%s Line Count" % lines[0].title
     filename = title + '.pdf'
     doc = make_doc_template(page_size=page_size, filename=filename,
                             document_title=title, title=lines[0].title,
                             document_subheader=lines[0].spot,
                             client=lines[0].client,
                             supervisor=lines[0].supervisor,
                             document_header='Line Count')
 
     # header_data, header_style, header_widths = build_header(columns_widths)
-    # header_table = Table(data=header_data, style=header_style, colWidths=header_widths)
+    # header_table = Table(data=header_data, style=header_style,
+    # colWidths=header_widths)
 
     table = Table(data=data, style=style, colWidths=columns_widths)
 
     story = [Spacer(height=0.5 * inch, width=1.), table]
 
     style = getSampleStyleSheet()['Normal']
     style.fontName = font_name
     style.fontSize = 12.
     style.spaceBefore = 16.
     style.spaceAfter = 16.
 
     omitted_count = len([x for x in lines if x.omitted])
 
     if not include_omitted and omitted_count > 0:
-        story.append(Paragraph("* %i Omitted lines are excluded." % omitted_count, style))
+        story.append(Paragraph("* %i Omitted lines are excluded." %
+                     omitted_count, style))
 
     doc.build(story)
```

### Comparing `ptulsconv-1.0.7/ptulsconv/pdf/summary_log.py` & `ptulsconv-2.0.0/ptulsconv/pdf/summary_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,31 +23,36 @@
     if line.shot is not None:
         entries.append("Shot: " + line.shot)
 
     fg_color = 'white'
     tag_field = ""
     if line.effort:
         bg_color = 'red'
-        tag_field += "<font backColor=%s textColor=%s fontSize=11>%s</font> " % (bg_color, fg_color, "EFF")
+        tag_field += "<font backColor=%s textColor=%s fontSize=11>%s</font> " \
+            % (bg_color, fg_color, "EFF")
     elif line.tv:
         bg_color = 'blue'
-        tag_field += "<font backColor=%s textColor=%s fontSize=11>%s</font> " % (bg_color, fg_color, "TV")
+        tag_field += "<font backColor=%s textColor=%s fontSize=11>%s</font> " \
+            % (bg_color, fg_color, "TV")
     elif line.adlib:
         bg_color = 'purple'
-        tag_field += "<font backColor=%s textColor=%s fontSize=11>%s</font> " % (bg_color, fg_color, "ADLIB")
+        tag_field += "<font backColor=%s textColor=%s fontSize=11>%s</font> " \
+            % (bg_color, fg_color, "ADLIB")
     elif line.optional:
         bg_color = 'green'
-        tag_field += "<font backColor=%s textColor=%s fontSize=11>%s</font>" % (bg_color, fg_color, "OPTIONAL")
+        tag_field += "<font backColor=%s textColor=%s fontSize=11>%s</font>" \
+            % (bg_color, fg_color, "OPTIONAL")
 
     entries.append(tag_field)
 
     return "<br />".join(entries)
 
 
-def build_story(lines: List[ADRLine], tc_rate: TimecodeFormat, font_name='Helvetica'):
+def build_story(lines: List[ADRLine], tc_rate: TimecodeFormat,
+                font_name='Helvetica'):
     story = list()
 
     this_scene = None
     scene_style = getSampleStyleSheet()['Normal']
     scene_style.fontName = font_name
     scene_style.leftIndent = 0.
     scene_style.leftPadding = 0.
@@ -56,15 +61,16 @@
     line_style.fontName = font_name
 
     for line in lines:
         table_style = [('VALIGN', (0, 0), (-1, -1), 'TOP'),
                        ('LEFTPADDING', (0, 0), (0, 0), 0.0),
                        ('BOTTOMPADDING', (0, 0), (-1, -1), 24.)]
 
-        cue_number_field = "%s<br /><font fontSize=7>%s</font>" % (line.cue_number, line.character_name)
+        cue_number_field = "%s<br /><font fontSize=7>%s</font>" \
+            % (line.cue_number, line.character_name)
 
         time_data = time_format(line.time_budget_mins)
 
         if line.priority is not None:
             time_data = time_data + "<br />" + "P: " + line.priority
 
         aux_data_field = build_aux_data_field(line)
@@ -75,15 +81,16 @@
                             Paragraph(tc_data, line_style),
                             Paragraph(line.prompt, line_style),
                             Paragraph(time_data, line_style),
                             Paragraph(aux_data_field, line_style)
                             ]]
 
         line_table = Table(data=line_table_data,
-                           colWidths=[inch * 0.75, inch, inch * 3., 0.5 * inch, inch * 2.],
+                           colWidths=[inch * 0.75, inch, inch * 3., 0.5 * inch,
+                                      inch * 2.],
                            style=table_style)
 
         if (line.scene or "[No Scene]") != this_scene:
             this_scene = line.scene or "[No Scene]"
             story.append(KeepTogether([
                 Spacer(1., 0.25 * inch),
                 Paragraph("<u>" + this_scene + "</u>", scene_style),
@@ -93,33 +100,34 @@
             story.append(KeepTogether([line_table]))
 
     return story
 
 
 def build_tc_data(line: ADRLine, tc_format: TimecodeFormat):
     tc_data = tc_format.seconds_to_smpte(line.start) + "<br />" + \
-              tc_format.seconds_to_smpte(line.finish)
+        tc_format.seconds_to_smpte(line.finish)
     third_line = []
     if line.reel is not None:
         if line.reel[0:1] == 'R':
             third_line.append("%s" % line.reel)
         else:
             third_line.append("Reel %s" % line.reel)
     if line.version is not None:
         third_line.append("(%s)" % line.version)
     if len(third_line) > 0:
         tc_data = tc_data + "<br/>" + " ".join(third_line)
     return tc_data
 
 
-def generate_report(page_size, lines: List[ADRLine], tc_rate: TimecodeFormat, character_number=None,
-                    include_omitted=True):
+def generate_report(page_size, lines: List[ADRLine], tc_rate: TimecodeFormat,
+                    character_number=None, include_omitted=True):
     if character_number is not None:
         lines = [r for r in lines if r.character_id == character_number]
-        title = "%s ADR Report (%s)" % (lines[0].title, lines[0].character_name)
+        title = "%s ADR Report (%s)" % (lines[0].title,
+                                        lines[0].character_name)
         document_header = "%s ADR Report" % lines[0].character_name
     else:
         title = "%s ADR Report" % lines[0].title
         document_header = 'ADR Report'
 
     if not include_omitted:
         lines = [line for line in lines if not line.omitted]
```

### Comparing `ptulsconv-1.0.7/ptulsconv/pdf/supervisor_1pg.py` & `ptulsconv-2.0.0/ptulsconv/pdf/supervisor_1pg.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from reportlab.pdfgen.canvas import Canvas
 
-from reportlab.pdfbase import pdfmetrics
-from reportlab.pdfbase.ttfonts import TTFont
+# from reportlab.pdfbase import pdfmetrics
+# from reportlab.pdfbase.ttfonts import TTFont
 
 from reportlab.lib.units import inch
 from reportlab.lib.pagesizes import letter
 
 from reportlab.lib.styles import getSampleStyleSheet
 from reportlab.platypus import Paragraph
 
 from .__init__ import GRect
 
-from ptulsconv.broadcast_timecode import TimecodeFormat, footage_to_frame_count
+from ptulsconv.broadcast_timecode import TimecodeFormat
 from ptulsconv.docparser.adr_entity import ADRLine
 
 import datetime
 
 font_name = 'Helvetica'
 
+
 def draw_header_block(canvas, rect, record: ADRLine):
-    rect.draw_text_cell(canvas, record.cue_number, "Helvetica", 44, vertical_align='m')
+    rect.draw_text_cell(canvas, record.cue_number, "Helvetica", 44,
+                        vertical_align='m')
 
 
 def draw_character_row(canvas, rect, record: ADRLine):
     label_frame, value_frame = rect.split_x(1.25 * inch)
-    label_frame.draw_text_cell(canvas, "CHARACTER", font_name, 10, force_baseline=9.)
+    label_frame.draw_text_cell(canvas, "CHARACTER", font_name, 10,
+                               force_baseline=9.)
     line = "%s / %s" % (record.character_id, record.character_name)
     if record.actor_name is not None:
         line = line + " / " + record.actor_name
     value_frame.draw_text_cell(canvas, line, font_name, 12, force_baseline=9.)
     rect.draw_border(canvas, ['min_y', 'max_y'])
 
 
 def draw_cue_number_block(canvas, rect, record: ADRLine):
-    (label_frame, number_frame,), aux_frame = rect.divide_y([0.20 * inch, 0.375 * inch], direction='d')
+    (label_frame, number_frame,), aux_frame = \
+        rect.divide_y([0.20 * inch, 0.375 * inch], direction='d')
     label_frame.draw_text_cell(canvas, "CUE NUMBER", font_name, 10,
                                inset_y=5., vertical_align='t')
     number_frame.draw_text_cell(canvas, record.cue_number, font_name, 14,
                                 inset_x=10., inset_y=2., draw_baseline=True)
 
     tags = {'tv': 'TV',
             'optional': 'OPT',
@@ -51,26 +55,33 @@
             tag_field = tag_field + tags[key] + " "
 
     aux_frame.draw_text_cell(canvas, tag_field, font_name, 10,
                              inset_x=10., inset_y=2., vertical_align='t')
     rect.draw_border(canvas, 'max_x')
 
 
-def draw_timecode_block(canvas, rect, record: ADRLine, tc_display_format: TimecodeFormat):
+def draw_timecode_block(canvas, rect, record: ADRLine,
+                        tc_display_format: TimecodeFormat):
     (in_label_frame, in_frame, out_label_frame, out_frame), _ = rect.divide_y(
         [0.20 * inch, 0.25 * inch, 0.20 * inch, 0.25 * inch], direction='d')
 
     in_label_frame.draw_text_cell(canvas, "IN", font_name, 10,
                                   vertical_align='t', inset_y=5., inset_x=5.)
-    in_frame.draw_text_cell(canvas, tc_display_format.seconds_to_smpte(record.start), font_name, 14,
-                            inset_x=10., inset_y=2., draw_baseline=True)
+    in_frame.draw_text_cell(canvas,
+                            tc_display_format.seconds_to_smpte(record.start),
+                            font_name, 14,
+                            inset_x=10., inset_y=2.,
+                            draw_baseline=True)
     out_label_frame.draw_text_cell(canvas, "OUT", font_name, 10,
                                    vertical_align='t', inset_y=5., inset_x=5.)
-    out_frame.draw_text_cell(canvas, tc_display_format.seconds_to_smpte(record.finish), font_name, 14,
-                             inset_x=10., inset_y=2., draw_baseline=True)
+    out_frame.draw_text_cell(canvas,
+                             tc_display_format.seconds_to_smpte(record.finish),
+                             font_name, 14,
+                             inset_x=10., inset_y=2.,
+                             draw_baseline=True)
 
     rect.draw_border(canvas, 'max_x')
 
 
 def draw_reason_block(canvas, rect, record: ADRLine):
     reason_cell, notes_cell = rect.split_y(24., direction='d')
     reason_label, reason_value = reason_cell.split_x(.75 * inch)
@@ -87,21 +98,23 @@
     style = getSampleStyleSheet()['BodyText']
     style.fontName = font_name
     style.fontSize = 12
     style.leading = 14
 
     p = Paragraph(record.note or "", style)
 
-    notes_value.draw_flowable(canvas, p, draw_baselines=True, inset_x=5., inset_y=5.)
+    notes_value.draw_flowable(canvas, p, draw_baselines=True,
+                              inset_x=5., inset_y=5.)
 
 
 def draw_prompt(canvas, rect, prompt=""):
     label, block = rect.split_y(0.20 * inch, direction='d')
 
-    label.draw_text_cell(canvas, "PROMPT", font_name, 10, vertical_align='t', inset_y=5., inset_x=0.)
+    label.draw_text_cell(canvas, "PROMPT", font_name, 10, vertical_align='t',
+                         inset_y=5., inset_x=0.)
 
     style = getSampleStyleSheet()['BodyText']
     style.fontName = font_name
     style.fontSize = 14
 
     style.leading = 24
     style.leftIndent = 1.5 * inch
@@ -113,15 +126,16 @@
 
     rect.draw_border(canvas, 'max_y')
 
 
 def draw_notes(canvas, rect, note=""):
     label, block = rect.split_y(0.20 * inch, direction='d')
 
-    label.draw_text_cell(canvas, "NOTES", font_name, 10, vertical_align='t', inset_y=5., inset_x=0.)
+    label.draw_text_cell(canvas, "NOTES", font_name, 10, vertical_align='t',
+                         inset_y=5., inset_x=0.)
 
     style = getSampleStyleSheet()['BodyText']
     style.fontName = font_name
     style.fontSize = 14
     style.leading = 24
 
     prompt = Paragraph(note, style)
@@ -165,94 +179,115 @@
         canvas.drawPath(ln)
 
     rect.draw_border(canvas, 'max_x')
 
     canvas.restoreState()
 
 
-def draw_aux_block(canvas, rect, recording_time_sec_this_line, recording_time_sec):
+def draw_aux_block(canvas, rect, recording_time_sec_this_line,
+                   recording_time_sec):
     rect.draw_border(canvas, 'min_x')
 
     content_rect = rect.inset_xy(10., 10.)
-    lines, last_line = content_rect.divide_y([12., 12., 24., 24., 24., 24.], direction='d')
+    lines, last_line = content_rect.divide_y([12., 12., 24., 24., 24., 24.],
+                                             direction='d')
 
     lines[0].draw_text_cell(canvas,
-                            "Time for this line: %.1f mins" % (recording_time_sec_this_line / 60.), font_name, 9.)
-    lines[1].draw_text_cell(canvas, "Running time: %03.1f mins" % (recording_time_sec / 60.), font_name, 9.)
-    lines[2].draw_text_cell(canvas, "Actual Start: ______________", font_name, 9., vertical_align='b')
-    lines[3].draw_text_cell(canvas, "Record Date: ______________", font_name, 9., vertical_align='b')
-    lines[4].draw_text_cell(canvas, "Engineer: ______________", font_name, 9., vertical_align='b')
-    lines[5].draw_text_cell(canvas, "Location: ______________", font_name, 9., vertical_align='b')
+                            "Time for this line: %.1f mins" %
+                            (recording_time_sec_this_line / 60.),
+                            font_name, 9.)
+    lines[1].draw_text_cell(canvas, "Running time: %03.1f mins" %
+                            (recording_time_sec / 60.), font_name, 9.)
+    lines[2].draw_text_cell(canvas, "Actual Start: ______________",
+                            font_name, 9., vertical_align='b')
+    lines[3].draw_text_cell(canvas, "Record Date: ______________",
+                            font_name, 9., vertical_align='b')
+    lines[4].draw_text_cell(canvas, "Engineer: ______________",
+                            font_name, 9., vertical_align='b')
+    lines[5].draw_text_cell(canvas, "Location: ______________",
+                            font_name, 9., vertical_align='b')
 
 
-def draw_footer(canvas, rect, record: ADRLine, report_date, line_no, total_lines):
+def draw_footer(canvas, rect, record: ADRLine, report_date, line_no,
+                total_lines):
     rect.draw_border(canvas, 'max_y')
     report_date_s = [report_date.strftime("%c")]
     spotting_name = [record.spot] if record.spot is not None else []
     pages_s = ["Line %i of %i" % (line_no, total_lines)]
     footer_s = " - ".join(report_date_s + spotting_name + pages_s)
-    rect.draw_text_cell(canvas, footer_s, font_name=font_name, font_size=10., inset_y=2.)
+    rect.draw_text_cell(canvas, footer_s, font_name=font_name, font_size=10.,
+                        inset_y=2.)
 
 
-def create_report_for_character(records, report_date, tc_display_format: TimecodeFormat):
+def create_report_for_character(records, report_date,
+                                tc_display_format: TimecodeFormat):
 
     outfile = "%s_%s_%s_Log.pdf" % (records[0].title,
                                     records[0].character_id,
                                     records[0].character_name,)
     assert outfile is not None
     assert outfile[-4:] == '.pdf', "Output file must have 'pdf' extension!"
 
-    #pdfmetrics.registerFont(TTFont('Futura', 'Futura.ttc'))
+    # pdfmetrics.registerFont(TTFont('Futura', 'Futura.ttc'))
 
     page: GRect = GRect(0, 0, letter[0], letter[1])
     page = page.inset(inch * 0.5)
-    (header_row, char_row, data_row, prompt_row, notes_row, takes_row), footer = \
-        page.divide_y([0.875 * inch, 0.375 * inch, inch, 3.0 * inch, 1.5 * inch, 3 * inch], direction='d')
+    (header_row, char_row, data_row,
+     prompt_row, notes_row, takes_row), footer = \
+        page.divide_y([0.875 * inch, 0.375 * inch, inch,
+                       3.0 * inch, 1.5 * inch, 3 * inch], direction='d')
 
     cue_header_block, title_header_block = header_row.split_x(4.0 * inch)
-    (cue_number_block, timecode_block), reason_block = data_row.divide_x([1.5 * inch, 1.5 * inch])
+    (cue_number_block, timecode_block), reason_block = \
+        data_row.divide_x([1.5 * inch, 1.5 * inch])
     (take_grid_block), aux_block = takes_row.split_x(5.25 * inch)
 
     c = Canvas(outfile, pagesize=letter,)
 
-    c.setTitle("%s %s (%s) Supervisor's Log" % (records[0].title, records[0].character_name,
+    c.setTitle("%s %s (%s) Supervisor's Log" % (records[0].title,
+                                                records[0].character_name,
                                                 records[0].character_id))
     c.setAuthor(records[0].supervisor)
 
     recording_time_sec = 0.0
     total_lines = len(records)
     line_n = 1
     for record in records:
         record: ADRLine
-        recording_time_sec_this_line: float = (record.time_budget_mins or 6.0) * 60.0
+        recording_time_sec_this_line: float = (
+            record.time_budget_mins or 6.0) * 60.0
         recording_time_sec = recording_time_sec + recording_time_sec_this_line
 
         draw_header_block(c, cue_header_block, record)
         # FIXME: Draw the title
         # TODO: Integrate this report into the common DocTemplate api
 
         # draw_title_box(c, title_header_block, record)
         draw_character_row(c, char_row, record)
         draw_cue_number_block(c, cue_number_block, record)
-        draw_timecode_block(c, timecode_block, record, tc_display_format=tc_display_format)
+        draw_timecode_block(c, timecode_block, record,
+                            tc_display_format=tc_display_format)
         draw_reason_block(c, reason_block, record)
-        draw_prompt(c, prompt_row, prompt=record.prompt)
+        draw_prompt(c, prompt_row, prompt=record.prompt or "")
         draw_notes(c, notes_row, note="")
         draw_take_grid(c, take_grid_block)
-        draw_aux_block(c, aux_block, recording_time_sec_this_line, recording_time_sec)
+        draw_aux_block(c, aux_block, recording_time_sec_this_line,
+                       recording_time_sec)
 
-        draw_footer(c, footer, record, report_date, line_no=line_n, total_lines=total_lines)
+        draw_footer(c, footer, record, report_date, line_no=line_n,
+                    total_lines=total_lines)
         line_n = line_n + 1
 
         c.showPage()
 
     c.save()
 
 
 def output_report(lines, tc_display_format: TimecodeFormat):
     report_date = datetime.datetime.now()
     events = sorted(lines, key=lambda x: x.start)
     character_numbers = set([x.character_id for x in lines])
 
     for n in character_numbers:
-        create_report_for_character([e for e in events if e.character_id == n], report_date,
+        create_report_for_character([e for e in events if e.character_id == n],
+                                    report_date,
                                     tc_display_format=tc_display_format)
```

### Comparing `ptulsconv-1.0.7/ptulsconv/pdf/talent_sides.py` & `ptulsconv-2.0.0/ptulsconv/pdf/talent_sides.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 # -*- coding: utf-8 -*-
 from typing import List
 
 from .__init__ import make_doc_template
 from reportlab.lib.units import inch
 from reportlab.lib.pagesizes import letter
 
-from reportlab.platypus import Paragraph, Spacer, KeepTogether, Table, HRFlowable
+from reportlab.platypus import Paragraph, Spacer, KeepTogether, Table,\
+    HRFlowable
 from reportlab.lib.styles import getSampleStyleSheet
 from reportlab.lib import colors
 
-from reportlab.pdfbase import pdfmetrics
-from reportlab.pdfbase.ttfonts import TTFont
+# from reportlab.pdfbase import pdfmetrics
+# from reportlab.pdfbase.ttfonts import TTFont
 
 from ..broadcast_timecode import TimecodeFormat
 from ..docparser.adr_entity import ADRLine
 
 
-def output_report(lines: List[ADRLine], tc_display_format: TimecodeFormat, font_name="Helvetica"):
+def output_report(lines: List[ADRLine], tc_display_format: TimecodeFormat,
+                  font_name="Helvetica"):
     character_numbers = set([n.character_id for n in lines])
-    #pdfmetrics.registerFont(TTFont('Futura', 'Futura.ttc'))
+    # pdfmetrics.registerFont(TTFont('Futura', 'Futura.ttc'))
 
     for n in character_numbers:
-        char_lines = [line for line in lines if not line.omitted and line.character_id == n]
+        char_lines = [line for line in lines
+                      if not line.omitted and line.character_id == n]
         character_name = char_lines[0].character_name
 
         char_lines = sorted(char_lines, key=lambda line: line.start)
 
-        title = "%s (%s) %s ADR Script" % (char_lines[0].title, character_name, n)
-        filename = "%s_%s_%s_ADR Script.pdf" % (char_lines[0].title, n, character_name)
+        title = "%s (%s) %s ADR Script" % (char_lines[0].title,
+                                           character_name, n)
+        filename = "%s_%s_%s_ADR Script.pdf" % (char_lines[0].title,
+                                                n, character_name)
 
-        doc = make_doc_template(page_size=letter, filename=filename, document_title=title,
+        doc = make_doc_template(page_size=letter, filename=filename,
+                                document_title=title,
                                 title=char_lines[0].title,
-                                document_subheader=char_lines[0].spot,
-                                supervisor=char_lines[0].supervisor,
-                                client=char_lines[0].client,
-                                document_header=character_name)
+                                document_subheader=char_lines[0].spot or "",
+                                supervisor=char_lines[0].supervisor or "",
+                                client=char_lines[0].client or "",
+                                document_header=character_name or "")
 
         story = []
 
         prompt_style = getSampleStyleSheet()['Normal']
         prompt_style.fontName = font_name
         prompt_style.fontSize = 18.
 
@@ -54,15 +60,16 @@
         number_style.leftIndent = 0.
         number_style.rightIndent = 0.
 
         for line in char_lines:
             start_tc = tc_display_format.seconds_to_smpte(line.start)
             finish_tc = tc_display_format.seconds_to_smpte(line.finish)
             data_block = [[Paragraph(line.cue_number, number_style),
-                           Paragraph(start_tc + " - " + finish_tc, number_style)
+                           Paragraph(start_tc + " - " + finish_tc,
+                                     number_style)
                            ]]
 
 # RIGHTWARDS ARROW →
 # Unicode: U+2192, UTF-8: E2 86 92
             story.append(
                 KeepTogether(
                     [HRFlowable(width='50%', color=colors.black),
```

### Comparing `ptulsconv-1.0.7/ptulsconv/reporting.py` & `ptulsconv-2.0.0/ptulsconv/reporting.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 def print_warning(warning_string):
     if sys.stderr.isatty():
         sys.stderr.write("\033[3m - %s\033[0m\n" % warning_string)
     else:
         sys.stderr.write(" - %s\n" % warning_string)
 
 
-def print_advisory_tagging_error(failed_string, position, parent_track_name=None, clip_time=None):
+def print_advisory_tagging_error(failed_string, position,
+                                 parent_track_name=None, clip_time=None):
     if sys.stderr.isatty():
         sys.stderr.write("\n")
         sys.stderr.write(" ! \033[33;1mTagging error: \033[0m")
         ok_string = failed_string[:position]
         not_ok_string = failed_string[position:]
-        sys.stderr.write("\033[32m\"%s\033[31;1m%s\"\033[0m\n" % (ok_string, not_ok_string))
+        sys.stderr.write("\033[32m\"%s\033[31;1m%s\"\033[0m\n" %
+                         (ok_string, not_ok_string))
 
         if parent_track_name is not None:
             sys.stderr.write(" !   > On track \"%s\"\n" % parent_track_name)
 
         if clip_time is not None:
             sys.stderr.write(" !   > In clip name at %s\n" % clip_time)
     else:
```

### Comparing `ptulsconv-1.0.7/ptulsconv/validations.py` & `ptulsconv-2.0.0/ptulsconv/validations.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,64 +10,75 @@
 @dataclass
 class ValidationError:
     message: str
     event: Optional[ADRLine] = None
 
     def report_message(self):
         if self.event is not None:
-            return f"{self.message}: event at {self.event.start} with number {self.event.cue_number}"
+            return (f"{self.message}: event at {self.event.start} with number"
+                    "{self.event.cue_number}")
         else:
             return self.message
 
 
-def validate_unique_count(input_lines: Iterator[ADRLine], field='title', count=1):
+def validate_unique_count(input_lines: Iterator[ADRLine], field='title',
+                          count=1):
     values = set(list(map(lambda e: getattr(e, field), input_lines)))
     if len(values) > count:
-        yield ValidationError(message="Field {} has too many values (max={}): {}".format(field, count, values))
+        yield ValidationError(
+            message="Field {} has too many values (max={}): {}"
+            .format(field, count, values)
+        )
 
 
 def validate_value(input_lines: Iterator[ADRLine], key_field, predicate):
     for event in input_lines:
         val = getattr(event, key_field)
         if not predicate(val):
             yield ValidationError(message='Field {} not in range'.format(val),
                                   event=event)
 
 
-def validate_unique_field(input_lines: Iterator[ADRLine], field='cue_number', scope=None):
+def validate_unique_field(input_lines: Iterator[ADRLine], field='cue_number',
+                          scope=None):
     values = dict()
     for event in input_lines:
         this = getattr(event, field)
         if scope is not None:
             key = getattr(event, scope)
         else:
             key = '_values'
 
         values.setdefault(key, set())
         if this in values[key]:
-            yield ValidationError(message='Re-used {}'.format(field), event=event)
+            yield ValidationError(message='Re-used {}'.format(field),
+                                  event=event)
         else:
             values[key].update(this)
 
 
-def validate_non_empty_field(input_lines: Iterator[ADRLine], field='cue_number'):
+def validate_non_empty_field(input_lines: Iterator[ADRLine],
+                             field='cue_number'):
     for event in input_lines:
         if getattr(event, field, None) is None:
-            yield ValidationError(message='Empty field {}'.format(field), event=event)
+            yield ValidationError(message='Empty field {}'.format(field),
+                                  event=event)
 
 
-def validate_dependent_value(input_lines: Iterator[ADRLine], key_field, dependent_field):
+def validate_dependent_value(input_lines: Iterator[ADRLine], key_field,
+                             dependent_field):
     """
-    Validates that two events with the same value in `key_field` always have the
-    same value in `dependent_field`
+    Validates that two events with the same value in `key_field` always have
+    the same value in `dependent_field`
     """
     key_values = set((getattr(x, key_field) for x in input_lines))
 
     for key_value in key_values:
-        rows = [(getattr(x, key_field), getattr(x, dependent_field)) for x in input_lines
+        rows = [(getattr(x, key_field), getattr(x, dependent_field))
+                for x in input_lines
                 if getattr(x, key_field) == key_value]
         unique_rows = set(rows)
         if len(unique_rows) > 1:
             message = "Non-unique values for key {} = ".format(key_field)
             for u in unique_rows:
                 message = message + "\n - {} -> {}".format(u[0], u[1])
```

### Comparing `ptulsconv-1.0.7/ptulsconv/xml/common.py` & `ptulsconv-2.0.0/ptulsconv/xml/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 from xml.etree.ElementTree import TreeBuilder, tostring
 from typing import List
 
 import ptulsconv
 from ptulsconv.docparser.adr_entity import ADRLine
 
 # TODO Get a third-party test for Avid Marker lists
-def avid_marker_list(lines: List[ADRLine], report_date=datetime.datetime.now(), reel_start_frame=0, fps=24):
+
+
+def avid_marker_list(lines: List[ADRLine], report_date=datetime.datetime.now(),
+                     reel_start_frame=0, fps=24):
     doc = TreeBuilder(element_factory=None)
 
     doc.start('Avid:StreamItems', {'xmlns:Avid': 'http://www.avid.com'})
     doc.start('Avid:XMLFileData', {})
     doc.start('AvProp', {'name': 'DomainMagic', 'type': 'string'})
     doc.data("Domain")
     doc.end('AvProp')
@@ -44,69 +47,84 @@
         doc.data(value)
         doc.end('AvProp')
 
         doc.end('ListElem')
 
     for line in lines:
         doc.start('AvClass', {'id': 'ATTR'})
-        doc.start('AvProp', {'id': 'ATTR', 'name': '__OMFI:ATTR:NumItems', 'type': 'int32'})
+        doc.start('AvProp', {'id': 'ATTR',
+                             'name': '__OMFI:ATTR:NumItems',
+                             'type': 'int32'})
         doc.data('7')
         doc.end('AvProp')
 
         doc.start('List', {'id': 'OMFI:ATTR:AttrRefs'})
 
-        insert_elem('1', 'OMFI:ATTB:IntAttribute', 'int32', '_ATN_CRM_LONG_CREATE_DATE', report_date.strftime("%s"))
-        insert_elem('2', 'OMFI:ATTB:StringAttribute', 'string', '_ATN_CRM_COLOR', 'yellow')
-        insert_elem('2', 'OMFI:ATTB:StringAttribute', 'string', '_ATN_CRM_USER', line.supervisor or "")
+        insert_elem('1', 'OMFI:ATTB:IntAttribute', 'int32',
+                    '_ATN_CRM_LONG_CREATE_DATE', report_date.strftime("%s"))
+        insert_elem('2', 'OMFI:ATTB:StringAttribute', 'string',
+                    '_ATN_CRM_COLOR', 'yellow')
+        insert_elem('2', 'OMFI:ATTB:StringAttribute', 'string',
+                    '_ATN_CRM_USER', line.supervisor or "")
 
         marker_name = "%s: %s" % (line.cue_number, line.prompt)
-        insert_elem('2', 'OMFI:ATTB:StringAttribute', 'string', '_ATN_CRM_COM', marker_name)
+        insert_elem('2', 'OMFI:ATTB:StringAttribute', 'string',
+                    '_ATN_CRM_COM', marker_name)
 
         start_frame = int(line.start * fps)
 
-        insert_elem('2', "OMFI:ATTB:StringAttribute", 'string', '_ATN_CRM_TC',
+        insert_elem('2', "OMFI:ATTB:StringAttribute", 'string',
+                    '_ATN_CRM_TC',
                     str(start_frame - reel_start_frame))
 
-        insert_elem('2', "OMFI:ATTB:StringAttribute", 'string', '_ATN_CRM_TRK', 'V1')
-        insert_elem('1', "OMFI:ATTB:IntAttribute", 'int32', '_ATN_CRM_LENGTH', '1')
+        insert_elem('2', "OMFI:ATTB:StringAttribute", 'string',
+                    '_ATN_CRM_TRK', 'V1')
+        insert_elem('1', "OMFI:ATTB:IntAttribute", 'int32',
+                    '_ATN_CRM_LENGTH', '1')
 
         doc.start('ListElem', {})
         doc.end('ListElem')
 
         doc.end('List')
         doc.end('AvClass')
 
     doc.end('Avid:XMLFileData')
     doc.end('Avid:StreamItems')
 
 
 def dump_fmpxml(data, input_file_name, output, adr_field_map):
     doc = TreeBuilder(element_factory=None)
 
-    doc.start('FMPXMLRESULT', {'xmlns': 'http://www.filemaker.com/fmpxmlresult'})
+    doc.start('FMPXMLRESULT', {'xmlns':
+                               'http://www.filemaker.com/fmpxmlresult'})
 
     doc.start('ERRORCODE', {})
     doc.data('0')
     doc.end('ERRORCODE')
 
-    doc.start('PRODUCT', {'NAME': ptulsconv.__name__, 'VERSION': ptulsconv.__version__})
+    doc.start('PRODUCT', {'NAME': ptulsconv.__name__,
+                          'VERSION': ptulsconv.__version__})
     doc.end('PRODUCT')
 
-    doc.start('DATABASE', {'DATEFORMAT': 'MM/dd/yy', 'LAYOUT': 'summary', 'TIMEFORMAT': 'hh:mm:ss',
-                           'RECORDS': str(len(data['events'])), 'NAME': os.path.basename(input_file_name)})
+    doc.start('DATABASE', {'DATEFORMAT': 'MM/dd/yy',
+                           'LAYOUT': 'summary',
+                           'TIMEFORMAT': 'hh:mm:ss',
+                           'RECORDS': str(len(data['events'])),
+                           'NAME': os.path.basename(input_file_name)})
     doc.end('DATABASE')
 
     doc.start('METADATA', {})
     for field in adr_field_map:
         tp = field[2]
         ft = 'TEXT'
         if tp is int or tp is float:
             ft = 'NUMBER'
 
-        doc.start('FIELD', {'EMPTYOK': 'YES', 'MAXREPEAT': '1', 'NAME': field[1], 'TYPE': ft})
+        doc.start('FIELD', {'EMPTYOK': 'YES', 'MAXREPEAT': '1',
+                            'NAME': field[1], 'TYPE': ft})
         doc.end('FIELD')
     doc.end('METADATA')
 
     doc.start('RESULTSET', {'FOUND': str(len(data['events']))})
     for event in data['events']:
         doc.start('ROW', {})
         for field in adr_field_map:
@@ -153,12 +171,13 @@
     dump_fmpxml(data, input_file, pipe, adr_field_map)
 
     str_data = pipe.getvalue()
     print_status_style("Base XML size %i" % (len(str_data)))
 
     print_status_style("Running xsltproc")
 
-    xsl_path = os.path.join(pathlib.Path(__file__).parent.absolute(), 'xslt', xsl_name + ".xsl")
+    xsl_path = os.path.join(pathlib.Path(__file__).parent.absolute(), 'xslt',
+                            xsl_name + ".xsl")
     print_status_style("Using xsl: %s" % xsl_path)
     subprocess.run(['xsltproc', xsl_path, '-'],
                    input=str_data, text=True,
                    stdout=output, shell=False, check=True)
```

### Comparing `ptulsconv-1.0.7/ptulsconv/xslt/AvidMarkers.xsl` & `ptulsconv-2.0.0/ptulsconv/xslt/AvidMarkers.xsl`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.7/ptulsconv/xslt/SRT.xsl` & `ptulsconv-2.0.0/ptulsconv/xslt/SRT.xsl`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.7/pyproject.toml` & `ptulsconv-2.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Topic :: Multimedia',
     'Topic :: Multimedia :: Sound/Audio',
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Development Status :: 5 - Production/Stable",
     "Topic :: Text Processing :: Filters"
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ["version", "description"]
 keywords = ["text-processing", "parsers", "film", 
     "broadcast", "editing", "editorial"]
-dependencies = ['parsimonious', 'tqdm', 'reportlab']
+dependencies = [
+  'parsimonious',
+  'tqdm',
+  'reportlab',
+  'py-ptsl >= 101.1.0'
+  ]
 
 [project.optional-dependencies]
 doc = [
     "Sphinx ~= 5.3.0",
     "sphinx-rtd-theme >= 1.1.1"
 ]
```

### Comparing `ptulsconv-1.0.7/PKG-INFO` & `ptulsconv-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: ptulsconv
-Version: 1.0.7
+Version: 2.0.0
 Summary: Parse and convert Pro Tools text exports
 Keywords: text-processing,parsers,film,broadcast,editing,editorial
 Author-email: Jamie Hardt <jamiehardt@me.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Text Processing :: Filters
 Requires-Dist: parsimonious
 Requires-Dist: tqdm
 Requires-Dist: reportlab
+Requires-Dist: py-ptsl >= 101.1.0
 Requires-Dist: Sphinx ~= 5.3.0 ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme >= 1.1.1 ; extra == "doc"
 Project-URL: Documentation, https://ptulsconv.readthedocs.io/
 Project-URL: Issues, https://github.com/iluvcapra/ptulsconv/issues
 Project-URL: Source, https://github.com/iluvcapra/ptulsconv
 Provides-Extra: doc
```

