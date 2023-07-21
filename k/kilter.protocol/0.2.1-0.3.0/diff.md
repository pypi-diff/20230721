# Comparing `tmp/kilter.protocol-0.2.1.tar.gz` & `tmp/kilter_protocol-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilter.protocol-0.2.1.tar", last modified: Mon Jan 30 02:57:32 2023, max compression
+gzip compressed data, was "kilter_protocol-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `kilter.protocol-0.2.1.tar` & `kilter_protocol-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    16726 2023-01-26 21:08:48.649002 kilter.protocol-0.2.1/LICENCE.txt
--rw-r--r--   0        0        0     4089 2023-01-26 23:51:42.432052 kilter.protocol-0.2.1/README.md
--rw-r--r--   0        0        0      673 2023-01-30 02:53:17.328622 kilter.protocol-0.2.1/kilter/protocol/__init__.py
--rw-r--r--   0        0        0     5161 2023-01-26 21:08:48.653002 kilter.protocol-0.2.1/kilter/protocol/buffer.py
--rw-r--r--   0        0        0     7254 2023-01-30 02:53:17.328622 kilter.protocol-0.2.1/kilter/protocol/core.py
--rw-r--r--   0        0        0     1114 2023-01-26 21:08:48.653002 kilter.protocol-0.2.1/kilter/protocol/exceptions.py
--rw-r--r--   0        0        0    23042 2023-01-26 21:08:48.653002 kilter.protocol-0.2.1/kilter/protocol/messages.py
--rw-r--r--   0        0        0        0 2023-01-26 21:08:48.653002 kilter.protocol-0.2.1/kilter/protocol/py.typed
--rw-r--r--   0        0        0     2575 2023-01-26 21:08:48.653002 kilter.protocol-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5124 1970-01-01 00:00:00.000000 kilter.protocol-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    16726 2023-07-13 19:10:45.307281 kilter_protocol-0.3.0/LICENCE.txt
+-rw-r--r--   0        0        0     4096 2023-07-20 00:12:58.721981 kilter_protocol-0.3.0/README.md
+-rw-r--r--   0        0        0      673 2023-07-19 23:56:33.555128 kilter_protocol-0.3.0/kilter/protocol/__init__.py
+-rw-r--r--   0        0        0     5161 2023-07-13 19:10:45.315281 kilter_protocol-0.3.0/kilter/protocol/buffer.py
+-rw-r--r--   0        0        0     9225 2023-07-19 23:56:33.555128 kilter_protocol-0.3.0/kilter/protocol/core.py
+-rw-r--r--   0        0        0     1932 2023-07-19 23:56:33.559128 kilter_protocol-0.3.0/kilter/protocol/exceptions.py
+-rw-r--r--   0        0        0    22146 2023-07-19 23:56:33.559128 kilter_protocol-0.3.0/kilter/protocol/messages.py
+-rw-r--r--   0        0        0        0 2023-07-13 19:10:45.315281 kilter_protocol-0.3.0/kilter/protocol/py.typed
+-rw-r--r--   0        0        0     2617 2023-07-13 22:40:33.359295 kilter_protocol-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5164 1970-01-01 00:00:00.000000 kilter_protocol-0.3.0/PKG-INFO
```

### Comparing `kilter.protocol-0.2.1/LICENCE.txt` & `kilter_protocol-0.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `kilter.protocol-0.2.1/README.md` & `kilter_protocol-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
   https://code.kodo.org.uk/kilter/kilter.protocol/pipelines/latest
   "Pipelines"
 
 [coverage status]:
   https://code.kodo.org.uk/kilter/kilter.protocol/badges/main/coverage.svg
 
 [coverage report]:
-  https://code.kodo.org.uk/kilter/kilter.protocol/-/jobs/artifacts/main/file/results/coverage/index.html?job=Unit+Tests
+  https://code.kodo.org.uk/kilter/kilter.protocol/-/jobs/artifacts/main/file/results/coverage.html.d/index.html?job=Unit+Tests
 
 
 Usage
 =====
 
 Most users will be looking for an asynchronous API using Python coroutines: this is 
 available with the [`kilter.service`][] package.  The protocol handlers provided by this
```

### Comparing `kilter.protocol-0.2.1/kilter/protocol/__init__.py` & `kilter_protocol-0.3.0/kilter/protocol/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from .core import ResponseMessage as ResponseMessage
 from .exceptions import *
 from .messages import *
 
 if TYPE_CHECKING:
 	from .buffer import FixedSizeBuffer as FixedSizeBuffer
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
```

### Comparing `kilter.protocol-0.2.1/kilter/protocol/buffer.py` & `kilter_protocol-0.3.0/kilter/protocol/buffer.py`

 * *Files identical despite different names*

### Comparing `kilter.protocol-0.2.1/kilter/protocol/messages.py` & `kilter_protocol-0.3.0/kilter/protocol/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Dominik Sekotill <dom.sekotill@kodo.org.uk>
+# Copyright 2022-2023 Dominik Sekotill <dom.sekotill@kodo.org.uk>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 Classes for representing protocol messages, and packing and unpacking them
@@ -19,26 +19,30 @@
 from collections.abc import Collection
 from collections.abc import Iterable
 from collections.abc import Iterator
 from collections.abc import Mapping
 from dataclasses import dataclass
 from dataclasses import field
 from enum import Enum
+from enum import IntFlag
 from ipaddress import IPv4Address
 from ipaddress import IPv6Address
 from ipaddress import ip_address
 from pathlib import Path
 from struct import Struct
 from typing import TYPE_CHECKING
 from typing import ClassVar
 from typing import TypeVar
 from typing import cast
 
+from typing_extensions import Self
+
 from .exceptions import InsufficientSpace
 from .exceptions import NeedsMore
+from .exceptions import UnknownMessage
 
 if TYPE_CHECKING:
 	from .buffer import FixedSizeBuffer
 
 LONG = Struct("!L")
 
 __all__ = [
@@ -110,15 +114,15 @@
 	END_MESSAGE = 5
 	END_HEADERS = 6
 
 
 BFSelf = TypeVar("BFSelf", bound="BitField")
 
 
-class BitField(int, Enum):
+class BitField(IntFlag):
 	"""
 	Base class for bit-field enums like ActionFlags and ProtocolFlags
 	"""
 
 	@classmethod
 	def pack(cls: type[BFSelf], flags: Iterable[BFSelf]) -> int:
 		rflag = 0
@@ -135,14 +139,16 @@
 	"""
 	Bit-field values for the `Negotiate.action_flags` field of the `Negotiate` message
 
 	The values correspond to the `SPFIF_*` codes as described in
 	https://pythonhosted.org/pymilter/milter_api/smfi_register.html#flags
 	"""
 
+	NONE = 0x0
+
 	ADD_HEADERS = ADDHDRS = 0x1
 	CHANGE_HEADERS = CHGHDRS = 0x10
 	CHANGE_BODY = CHGBODY = 0x2
 	ADD_RECIPIENT = ADDRCPT = 0x4
 	ADD_RECIPIENT_PAR = ADDRCPT_PAR = 0x80
 	DELETE_RECIPIENT = DELRCPT = 0x8
 	QUARANTINE = 0x20
@@ -154,14 +160,16 @@
 	"""
 	Bit-field values for the `Negotiate.protocol_flags` field of the `Negotiate` message
 
 	The values correspond to the `SMFIP_*` codes described in
 	https://pythonhosted.org/pymilter/milter_api/xxfi_negotiate.html
 	"""
 
+	NONE = 0x0
+
 	NO_CONNECT = 0x1
 	NO_HELO = 0x2
 	NO_SENDER = NO_MAIL = 0x4
 	NO_RECIPIENT = NO_RCPT = 0x8
 	NO_BODY = 0x10
 	NO_HEADERS = NO_HDRS = 0x20
 	NO_END_OF_HEADERS = NO_EOH = 0x40
@@ -226,17 +234,14 @@
 	Traceback (most recent call last):
 		...
 	BufferError: Existing exports of data: object cannot be re-sized
 	>>> message.release()
 	>>> del buf[:10]
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="Message")
-
 	ident: ClassVar[bytes]
 
 	_message_classes = dict[bytes, "type[Message]"]()
 	_hdr_struct = Struct("!lc")
 
 	@classmethod
 	def __init_subclass__(cls, /, ident: bytes = b""):
@@ -259,22 +264,22 @@
 		assert isinstance(ident, bytes)
 		end = hdr_size + size - 1
 		if buf.filled < end:
 			raise NeedsMore
 		try:
 			msg_class = cls._message_classes[ident]
 		except KeyError:
-			raise NotImplementedError(buf[:end].tobytes())
+			raise UnknownMessage(buf[:end].tobytes())
 		else:
 			with buf[hdr_size:end] as data:
 				return msg_class.from_buffer(data), end
 
 	@classmethod
 	@abstractmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		"""
 		Construct an instance with values unpacked from a buffer
 
 		Concrete classes must implement this method to unpack the values each class needs.
 		The buffer view contains the message contents, from after the five byte header, up
 		to the length indicated by the header.
 		"""
@@ -317,37 +322,31 @@
 
 
 class NoDataMessage(Message):
 	"""
 	Base class implementing `Message` abstract methods for messages with no contents
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="NoDataMessage")
-
 	def __repr__(self) -> str:
 		return f"{self.__class__.__name__}()"
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		assert len(buf) == 0, "message has some data"
 		return cls()
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		return
 
 
 class BytesMessage(Message):
 	"""
 	Base class implementing `Message` abstract methods for messages with unstructured contents
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="BytesMessage")
-
 	content: memoryview
 
 	def __init__(self, content: bytes):
 		self.content = memoryview(content).toreadonly()
 
 	def __repr__(self) -> str:
 		content = repr(self.content.tobytes()) if len(self.content) <= 30 else \
@@ -356,15 +355,15 @@
 
 	def __eq__(self, other: object) -> bool:
 		if not isinstance(other, type(self)):
 			return NotImplemented
 		return other.content == self.content
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		return cls(buf)
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		buf[:] = self.content
 
 	def release(self) -> None:
 		self.content.release()
@@ -379,37 +378,33 @@
 
 	A session starts with an MTA connecting to a filter and sending a negotiate message with
 	the action and protocol flags it supports.  The filter then returns a negotiate message
 	with the subset of the flags it wants to use, and optionally the macros (symbols) it
 	wants before each stage.
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="Negotiate")
-
 	version: int
 
-	# TODO: use set[Enum]?
-	action_flags: int
-	protocol_flags: int
+	action_flags: ActionFlags
+	protocol_flags: ProtocolFlags
 
 	macros: Mapping[Stage, Collection[str]] = field(default_factory=dict)
 
 	_struct = Struct("!LLL")
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
-		opts = cast(tuple[int, int, int], cls._struct.unpack_from(buf))
+	def from_buffer(cls, buf: memoryview) -> Self:
+		version, actions, options = cast(tuple[int, int, int], cls._struct.unpack_from(buf))
 		buf = buf[cls._struct.size:]
 		macros = dict()
 		while len(buf) > 0:
 			stage, *_ = LONG.unpack_from(buf)
 			names, buf = split_cstring(buf[LONG.size:])
-			macros[Stage(stage)] = names.tobytes().decode("utf-8").split()
-		return cls(*opts, macros)
+			macros[Stage(stage)] = str(names, "utf-8").split()
+		return cls(version, ActionFlags(actions), ProtocolFlags(options), macros)
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		self._struct.pack_into(
 			buf.get_free(self._struct.size), 0,
 			self.version, self.action_flags, self.protocol_flags,
 		)
 		join = " ".join
@@ -424,24 +419,21 @@
 
 @dataclass
 class Macro(Message, ident=b"D"):
 	"""
 	A message type for transferring symbol mappings prior to a stage event
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="Macro")
-
 	stage: bytes
 	macros: Mapping[str, str]
 
 	_struct = Struct("!c")
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		stage, *_ = cls._struct.unpack_from(buf)
 		macros = {}
 		with buf[1:] as buf:
 			while len(buf) > 0:
 				key, buf = split_cstring(buf)
 				val, buf = split_cstring(buf)
 				macros[key.tobytes().decode("ascii")] = val.tobytes().decode("ascii")
@@ -466,25 +458,22 @@
 	have ports.
 
 	The type of an address value indicates the address family: `ipaddress.IPv4Address` or
 	`ipaddress.IPv6Address` for INET and INET6 addresses, `pathlib.Path` for UNIX addresses,
 	or `None` for connections for which there is no known address (e.g. stdin).
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="Connect")
-
 	hostname: str
 	address: IPv4Address|IPv6Address|Path|None = None
 	port: int = 0
 
 	_struct = Struct("!H")
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		_hostname, buf = split_cstring(buf)
 		hostname = _hostname.tobytes().decode("idna")
 		family, buf = Family(buf[0:1].tobytes()), buf[1:]
 		if family == Family.UNKNOWN:
 			return cls(hostname)
 		port, *_ = cls._struct.unpack_from(buf)
 		addr, buf = split_cstring(buf[cls._struct.size:])
@@ -515,42 +504,36 @@
 
 @dataclass
 class Helo(Message, ident=b"H"):
 	"""
 	An event message reporting a client sent an SMTP HELO/EHLO command
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="Helo")
-
 	hostname: str
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		hostname, _ = split_cstring(buf)
 		return cls(hostname.tobytes().decode("idna"))
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.hostname.encode("idna"))
 
 
 @dataclass
 class EnvelopeFrom(Message, ident=b"M"):
 	"""
 	An event message reporting a client sent an SMTP "MAIL FROM" command
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="EnvelopeFrom")
-
 	sender: bytes
 	arguments: list[bytes] = field(default_factory=list)
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		args = cstring_iter(buf)
 		return cls(next(args), [*args])
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.sender)
 		for arg in self.arguments:
 			write_cstring(buf, arg)
@@ -567,22 +550,19 @@
 class EnvelopeRecipient(Message, ident=b"R"):
 	"""
 	An event message reporting a client sent an SMTP "RCPT TO" command
 
 	A client must send at least one "RCPT TO" command, and can send multiple.
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="EnvelopeRecipient")
-
 	recipient: bytes
 	arguments: list[bytes] = field(default_factory=list)
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		args = cstring_iter(buf)
 		return cls(next(args), [*args])
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.recipient)
 		for arg in self.arguments:
 			write_cstring(buf, arg)
@@ -614,22 +594,19 @@
 
 @dataclass
 class Header(Message, ident=b"L"):
 	"""
 	Transfers a header name and value from an email to a filter
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="Header")
-
 	name: str
 	value: bytes
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		name, buf = split_cstring(buf)
 		value, buf = split_cstring(buf)
 		assert len(buf) == 0
 		return cls(name.tobytes().decode("ascii"), value)
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.name.encode("ascii"))
@@ -721,43 +698,37 @@
 
 @dataclass
 class _AddrCmd(Message):
 	"""
 	Base class implementing `Message` abstract methods for messages with a single address
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="_AddrCmd")
-
 	address: str
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		address, buf = split_cstring(buf)
 		assert len(buf) == 0
 		return cls(address.tobytes().decode("utf-8"))
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.address.encode("utf-8"))
 
 
 @dataclass
 class _AddrParCmd(Message):
 	"""
 	Base class implementing `Message` abstract methods for messages with an address and arguments
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="_AddrParCmd")
-
 	address: str
 	args: str|None = None
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		args: memoryview|None = None
 		address, buf = split_cstring(buf)
 		if len(buf) > 0:
 			args, buf = split_cstring(buf)
 		assert len(buf) == 0
 		return cls(
 			address.tobytes().decode("utf-8"),
@@ -780,23 +751,20 @@
 
 @dataclass
 class ChangeHeader(Message, ident=b"m"):
 	"""
 	Message from a filter to request a header is modified or removed at a given index
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="ChangeHeader")
-
 	index: int
 	name: str
 	value: bytes
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		index, *_ = LONG.unpack_from(buf)
 		name, buf = split_cstring(buf[LONG.size:])
 		value, buf = split_cstring(buf)
 		assert len(buf) == 0
 		return cls(index, name.tobytes().decode("ascii"), value)
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
@@ -853,20 +821,17 @@
 
 @dataclass
 class Quarantine(Message, ident=b"q"):
 	"""
 	Request that a message is quarantined (blocked, but kept for review)
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="Quarantine")
-
 	reason: str
 
 	@classmethod
-	def from_buffer(cls: type[Self], buf: memoryview) -> Self:
+	def from_buffer(cls, buf: memoryview) -> Self:
 		reason, buf = split_cstring(buf)
 		assert len(buf) == 0
 		return cls(reason.tobytes().decode("utf-8"))
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.reason.encode("utf-8"))
```

### Comparing `kilter.protocol-0.2.1/pyproject.toml` & `kilter_protocol-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 classifiers = [
 	"Development Status :: 1 - Planning",
 	"Intended Audience :: Telecommunications Industry",
 	"License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 	"Topic :: Communications :: Email :: Filters",
 ]
 
+dependencies = [
+	"typing-extensions",
+]
+
 [project.optional-dependencies]
 docs = [
 	"sphinx ~=5.0",
 	"myst-parser",
 	"sphinx-rtd-theme",
 ]
 coverage = [
```

### Comparing `kilter.protocol-0.2.1/PKG-INFO` & `kilter_protocol-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: kilter.protocol
-Version: 0.2.1
+Version: 0.3.0
 Summary: Parsers and state machines for the Sendmail milter communications protocol
 Author-email: Dom Sekotill <dom.sekotill@kodo.org.uk>
 Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Communications :: Email :: Filters
+Requires-Dist: typing-extensions
 Requires-Dist: coverage[toml] ; extra == "coverage"
 Requires-Dist: kodo.plugins.cover-test-context ; extra == "coverage"
 Requires-Dist: sphinx ~=5.0 ; extra == "docs"
 Requires-Dist: myst-parser ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Project-URL: Documentation, http://kilter.doc.kodo.org.uk/kilter.protocol
 Project-URL: Issues, https://code.kodo.org.uk/kilter/kilter.protocol/-/issues
@@ -101,15 +102,15 @@
   https://code.kodo.org.uk/kilter/kilter.protocol/pipelines/latest
   "Pipelines"
 
 [coverage status]:
   https://code.kodo.org.uk/kilter/kilter.protocol/badges/main/coverage.svg
 
 [coverage report]:
-  https://code.kodo.org.uk/kilter/kilter.protocol/-/jobs/artifacts/main/file/results/coverage/index.html?job=Unit+Tests
+  https://code.kodo.org.uk/kilter/kilter.protocol/-/jobs/artifacts/main/file/results/coverage.html.d/index.html?job=Unit+Tests
 
 
 Usage
 =====
 
 Most users will be looking for an asynchronous API using Python coroutines: this is 
 available with the [`kilter.service`][] package.  The protocol handlers provided by this
```

