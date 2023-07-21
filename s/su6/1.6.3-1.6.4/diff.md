# Comparing `tmp/su6-1.6.3.tar.gz` & `tmp/su6-1.6.4.tar.gz`

## Comparing `su6-1.6.3.tar` & `su6-1.6.4.tar`

### file list

```diff
@@ -1,1517 +1,1517 @@
--rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 su6-1.6.3/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6-1.6.3/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 su6-1.6.3/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/colorsys.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/colorsys.meta.json
--rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/hashlib.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/hashlib.meta.json
--rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/hmac.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/hmac.meta.json
--rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/linecache.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/linecache.meta.json
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mypy_extensions.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mypy_extensions.meta.json
--rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pty.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pty.meta.json
--rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pydoc.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pydoc.meta.json
--rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/secrets.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/secrets.meta.json
--rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/struct.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/struct.meta.json
--rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sysconfig.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/sysconfig.meta.json
--rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/token.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/token.meta.json
--rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tokenize.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tokenize.meta.json
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/zlib.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/zlib.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/__init__.data.json
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/__init__.meta.json
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/_width_table.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/_width_table.meta.json
--rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/brackets.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/brackets.meta.json
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/cache.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/cache.meta.json
--rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/comments.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/comments.meta.json
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/concurrency.data.json
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/concurrency.meta.json
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/const.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/const.meta.json
--rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/files.data.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/files.meta.json
--rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
--rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/linegen.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/linegen.meta.json
--rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/lines.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/lines.meta.json
--rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/mode.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/mode.meta.json
--rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/nodes.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/nodes.meta.json
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/numerics.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/numerics.meta.json
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/output.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/output.meta.json
--rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/parsing.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/parsing.meta.json
--rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/report.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/report.meta.json
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/rusty.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/rusty.meta.json
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/strings.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/strings.meta.json
--rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/trans.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/black/trans.meta.json
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/__init__.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/__init__.meta.json
--rw-r--r--   0        0        0    28796 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/cls.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/cls.meta.json
--rw-r--r--   0        0        0    37237 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/core.data.json
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/core.meta.json
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/dump.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/dump.meta.json
--rw-r--r--   0        0        0    33281 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/errors.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/errors.meta.json
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/helpers.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/helpers.meta.json
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/postpone.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/postpone.meta.json
--rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/singleton.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/singleton.meta.json
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/type_converters.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/type_converters.meta.json
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/_types.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json
--rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/register.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/register.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/__init__.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/__init__.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/ipython.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/ipython.meta.json
--rw-r--r--   0        0        0    23574 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/main.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/main.meta.json
--rw-r--r--   0        0        0    52407 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/parser.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/parser.meta.json
--rw-r--r--   0        0        0    14742 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/variables.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/dotenv/variables.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/html/entities.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/html/entities.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/util.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/util.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0    32124 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/main.data.json
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/main.meta.json
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0    20473 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    31787 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0    24762 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/token.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/token.meta.json
--rw-r--r--   0        0        0    38285 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    17455 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    17494 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    37554 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_format.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_format.meta.json
--rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_url.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/mdurl/_url.meta.json
--rw-r--r--   0        0        0    31404 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/tags.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/tags.meta.json
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/utils.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/utils.meta.json
--rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/__init__.meta.json
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/_meta.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/_meta.meta.json
--rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/gitignore.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/gitignore.meta.json
--rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/pathspec.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/pathspec.meta.json
--rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/pattern.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/pattern.meta.json
--rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/util.data.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/util.meta.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
--rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
--rw-r--r--   0        0        0    27179 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/__init__.meta.json
--rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/android.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/android.meta.json
--rw-r--r--   0        0        0    42401 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/api.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/api.meta.json
--rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/unix.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/unix.meta.json
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/version.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/platformdirs/version.meta.json
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/__init__.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/__init__.meta.json
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/__main__.data.json
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/__main__.meta.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_export_format.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_extension.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_extension.meta.json
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_fileno.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_fileno.meta.json
--rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_inspect.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_inspect.meta.json
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_log_render.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_log_render.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_loop.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_loop.meta.json
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_null_file.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_palettes.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_pick.data.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_pick.meta.json
--rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_ratio.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_spinners.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_spinners.meta.json
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_stack.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_stack.meta.json
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_timer.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_timer.meta.json
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_windows.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_windows.meta.json
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_wrap.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/_wrap.meta.json
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/abc.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/abc.meta.json
--rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/align.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/align.meta.json
--rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/ansi.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/ansi.meta.json
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/box.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/box.meta.json
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/cells.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/cells.meta.json
--rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/color.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/color.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/columns.data.json
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/columns.meta.json
--rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/console.data.json
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/console.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/constrain.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/constrain.meta.json
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/containers.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/containers.meta.json
--rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/control.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/control.meta.json
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/default_styles.data.json
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/emoji.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/emoji.meta.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/errors.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/errors.meta.json
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/highlighter.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/json.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/json.meta.json
--rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/jupyter.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/jupyter.meta.json
--rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/live.data.json
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/live.meta.json
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/live_render.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/live_render.meta.json
--rw-r--r--   0        0        0    82219 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/markdown.data.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/markdown.meta.json
--rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/markup.data.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/markup.meta.json
--rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/measure.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/measure.meta.json
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/padding.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/padding.meta.json
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/pager.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/pager.meta.json
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/palette.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/palette.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/panel.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/panel.meta.json
--rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/pretty.data.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/pretty.meta.json
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/protocol.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/protocol.meta.json
--rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/region.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/region.meta.json
--rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/repr.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/repr.meta.json
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/rule.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/rule.meta.json
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/scope.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/scope.meta.json
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/screen.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/screen.meta.json
--rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/segment.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/segment.meta.json
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/spinner.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/spinner.meta.json
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/status.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/status.meta.json
--rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/style.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/style.meta.json
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/styled.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/styled.meta.json
--rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/syntax.data.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/syntax.meta.json
--rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/table.data.json
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/table.meta.json
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/text.data.json
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/text.meta.json
--rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/theme.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/theme.meta.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/themes.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/themes.meta.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/traceback.data.json
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/rich/traceback.meta.json
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/__about__.data.json
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/__about__.meta.json
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/__init__.data.json
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/__init__.meta.json
--rw-r--r--   0        0        0    26556 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/cli.data.json
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/cli.meta.json
--rw-r--r--   0        0        0    56908 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/core.data.json
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/core.meta.json
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/helpers.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/helpers.meta.json
--rw-r--r--   0        0        0    49469 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/plugins.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/su6/plugins.meta.json
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli/__init__.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli/__init__.meta.json
--rw-r--r--   0        0        0    52646 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli/_parser.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli/_parser.meta.json
--rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli/_re.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli/_re.meta.json
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli/_types.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli/_types.meta.json
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli_w/__init__.data.json
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli_w/__init__.meta.json
--rw-r--r--   0        0        0    31248 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli_w/_writer.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomli_w/_writer.meta.json
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/__init__.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/__init__.meta.json
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/_compat.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/_compat.meta.json
--rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/_utils.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/_utils.meta.json
--rw-r--r--   0        0        0    19946 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/api.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/api.meta.json
--rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/container.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/container.meta.json
--rw-r--r--   0        0        0    33007 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/exceptions.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/exceptions.meta.json
--rw-r--r--   0        0        0   221620 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/items.data.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/items.meta.json
--rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/parser.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/parser.meta.json
--rw-r--r--   0        0        0    22900 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/source.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/source.meta.json
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/toml_char.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/toml_char.meta.json
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/toml_document.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/tomlkit/toml_document.meta.json
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/__init__.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/__init__.meta.json
--rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_checkers.data.json
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_checkers.meta.json
--rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_config.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_config.meta.json
--rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_decorators.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_decorators.meta.json
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_exceptions.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_exceptions.meta.json
--rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_functions.data.json
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_functions.meta.json
--rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_importhook.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_importhook.meta.json
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_memo.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_memo.meta.json
--rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_suppression.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_suppression.meta.json
--rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_transformer.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_transformer.meta.json
--rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_utils.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typeguard/_utils.meta.json
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_completion_click7.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_completion_click7.meta.json
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_completion_click8.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_completion_click8.meta.json
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/mock.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/mock.meta.json
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.6.3/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-1.6.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-1.6.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-1.6.3/.pytest_cache/README.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 su6-1.6.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 su6-1.6.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.6.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/10595a931c3c881e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1065c8b44fadc39a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1086635a5970b925
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/10ab08017438a66a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/10c2ae33c509be23
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/11152902676027343458
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/11f25cfda4e2f210
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/122419b0bc04bb24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1322b93a2154c54a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/134e5e8c29726e7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/13985ae090677282
--rw-r--r--   0        0        0    44502 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/14681219216720271199
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/146952ec4263c5d9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/150d086b8b4de9d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/156301591af184f1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1663be342a34f83
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1895bed4a0ed65d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1996a22aec44a5c0
--rw-r--r--   0        0        0    16044 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1a4449eb8b26a401
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1a4db4c4834af592
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1b0530edc3fe075e
--rw-r--r--   0        0        0    21464 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1b7872d6314f48b7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1ce202f3daa889d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1cfd31ba4b0b7ef9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1d75413e215f93c6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1dcbdc62e66ccf0e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1edace855ae3c841
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1f7ac4f892285f60
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1f88fbdfcbf2d8d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/1fbfdffa4078f509
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/20b40aca78f395e8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/219bf1f8f2938bd4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/21b248d368a93ac8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/21cf950ddc412c7b
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/22a98eb4527b8ca5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/22d9a59d8d30ba9d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/22db1408b8f4a4b2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/232d0222563916a6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/23680c0655621b13
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/23da3e9165a5513d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/247546336fc4bd59
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/248d23bfc4586461
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/24e2ebef92fa75b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/25d9504d2b6847d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/26657ed11f8e66de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/269f98f304a03fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/27ca2458f5ee73fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/28caf6cfecd38c1a
--rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/294d5a468695eb7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/29531d612e8a868a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2a383abdede299d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2a5d8d1386804aed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2a630c7d6d7faa40
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2b0cdebce71424f0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2bc4a20be77b881b
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2bf27b960bc3ded1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2c189a9882594507
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2c6eeab804b5c1f1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2c9bbc6bae6b0f41
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2d77da04c7119543
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2e4746b83d2d1cf8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2e6b6d5e70ae29db
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2e8708077cd0413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2f9e25dc2ce777cc
--rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/2face4e073dced28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/300f9a816018d49f
--rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/30e241b2876dc71f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/31813abf4ed82b53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3271e344462a0ee3
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/33004598889f4950
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/349f044f89b94587
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/34a4aaded634d537
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/34e1109d49bf09f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/356d28a11355e7a5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/357e837fe90ee680
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/35ab5ee4981cdf8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/35ba35b3f04c192f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/36372ef94f8716cd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/36e48551be186a66
--rw-r--r--   0        0        0    16058 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/36f0bdaeef592d9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/380a13ecd1a2af25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/38962215221b245a
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/38b035e004ea9f4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/38d9da4e93811c4f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/39285e72757cc499
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/399d3b28a1a1db47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3a74e1b5704e9b3f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3af645c926072f97
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3c6b70c96e832bc1
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3c7fb493febe6a55
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3c9bb20c3b57bae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3ca706f99b2d38bf
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3ccdd2336c8c80e9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3cf13d9d13babf93
--rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3db675ebeb97b2fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3dfac0c0edd78d53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3e0ec316d612ddc6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3e35311bfb3345f8
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3f10d9d7687f3999
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/3f12e7a3fe46c220
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/417040cdeaa7bd81
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/429010e306ea9808
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/42f337caed884834
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/431bdba29473eca0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4536434fd84cdba5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/454cfd5b3ba01a90
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/467fc2e82c277fd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/47affd4e531897a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/47ca38fe0242f05d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/47e54ee652d2f4c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4843e1c724479e6a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/484730e7d1a4dcd9
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4880724f1f6a1ac8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/48bda5931a9eb062
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/49b4fe40533bd678
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/49fafbbbbadedf00
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4a63ed784e7c5ec0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4ac8c08e5b1b6650
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4b5890a0c8dc15df
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4cd4c52ee1dc7ffe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4cdd16a7f9738f22
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4d5914600f7e99c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4eaf3b155fae0dfb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4f16c6852dea8eca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4f2c663677c63589
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4f75816f4078d31b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4f8371badac33c92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/4fafe0dbefb778fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/50373733f4645c5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/514fb27e4aef5783
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/519ab6ce866ef11b
--rw-r--r--   0        0        0    18347 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/51de14ac05bcd5d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/529312a72d1177a1
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/534b8acecf74c47
--rw-r--r--   0        0        0    20136 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/536320baecd03af6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/538fc0618c4d4c31
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/53c0f85a3179a38f
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5436d767d06cf116
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/54637ff0aaaaf6b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/552fa1eb2057eecc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5548c3ce5fff0cca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/556b5cfaac0c49bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/55c947c0fa59929
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/568d77a0a0a64dbc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/56e83f1c5eeb3eba
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/572ba1efb5bb3fd6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/58240cde188220d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/584058f21d3e2fa1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/594d55ee247cbdef
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/59cfab1472b544fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5a6dc8ef65620223
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5af13ad9cc04e932
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5b7183ee842066de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5b8fb96822a8f127
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5b965ef6adf36c8f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5badc1835a2b80e1
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5cc5d54a963753bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5da466fd7e3b19f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5e83ab1d520dc773
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5efe825a5e773b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5f4cf7812d590c90
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/5fb3763e0810c38a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/62396a4dea084957
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/624348590d33bdc9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6278996c2e6b2a87
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/63dbabe01e9e6756
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6550bbd98b1711bd
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6644351985978373760
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6791fc0114ddc05
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6845ca4e0c56952b
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/684d0841c18787fb
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/68c4553df91c1f5e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/69bb9ea6355c0c25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/69ffc3e7ad0aa6b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6a4adfab73a8d4b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6a74d0efd6350f1e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6b596d4ac1166741
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6b9f30172d33b6a3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6bcca98e41cda3f4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6beed9d45ff1a491
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6c989c6e4eea10bd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6db20c27780d4a5f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6db875fe1541793e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6eab8cdd7b4ae170
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/6fc044c94dc3532a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/701212523f7b3b9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/70963c0c68bf76ac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/70bd045859d6cb20
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/70d6f3b95738758d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/729f212cc9c6cd5d
--rw-r--r--   0        0        0    20572 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/72a6612daca66426
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/72de7bec9ecb53aa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/733b2373fa4ae335
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7396a954cc3b124a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7485843a948a75b0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/755c9c217a06f932
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/75bb48e114159509
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/76d56794deeb084d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/76fbe2af0f71bd4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/79a22043e5c16946
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/79c3fb2c81fd59a0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7a19353a5daa4a37
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7b3a1bf0b652398a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7bf45647f43eaf85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7c01d9689dd16a64
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7c37d34a0c059ec7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7c806e58272a88ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7cbc35f4e814db65
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7cc3783d00621498
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7cf495b196c50222
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7dc27d897f910c11
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7e138932f0b9a1bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7eb1422c10ced038
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7eb17a25b4fa1d13
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7f0f63895e369318
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/7f75cbd11ebac70a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8012caf4fb290dc8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/80844117d21fe12b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/809075c58fb87c61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/80dbccb0d26b4b4f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/80ded2016f4f413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/81e3edf198d6c468
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/81e6f787866d0ecf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/82ab0276d38aec9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/835f19fb8c240dbe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/83a59cf9aceae1d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/83cdfb5da134b21f
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8479781080806744663
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/84bb9d90fe3a6595
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/84e2e26fc69ab274
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/84e8c31ce428d3ee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/858df3976aef9624
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/868699acd08be339
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/86c3e5b9f79f490f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/87a7b0840a5cf8c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/87d9b6d5e7bcb6c7
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/881c84062ed51136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/886d14b97dbd4f2e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8944dfd1b590bdd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/89c7a4d643f68517
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/89e58e5ee0d7d864
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8a0279b11d098d9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8a437c05421c6cb5
--rw-r--r--   0        0        0    20054 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8a5ec4ca9660671c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8b8acf1607bcb3f9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8c34e85d573e230f
--rw-r--r--   0        0        0    17871 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8ccd539b7f96dff8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8d2f83aae152de29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8df3988e9368cbe6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/8f33397e19bead30
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9019e33ca68d8935
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/902eb6f99ee41131
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/906cef8208fbf28f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9080aaa3f2416b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/922bfc03482db456
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/92db151fe9967fd3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9352425265579062
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/93fed7ae4120c88e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/945994955724de24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/94ffcc82bc7ee370
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/95df46a8e947b100
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9613cbbc5a7c60a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/968b32ac9319cc53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/97a72bc70808d2f9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/97cbf45b388709d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/97df9d79e599f082
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/981eb70eb69fb3ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/98392e87ef3eb254
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/99d5decc6ca01825
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9a5552199a8b8bd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9bd08ae684645cf6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9c1285d5b3178abe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9cbaa57406e65f63
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9d0f65e1ab7ca23
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9db15fb6e71bec4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9dda9185d48774f2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9e3b1a7c0f34103b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9e50a4d6fb3c9688
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9e558f66f216c4eb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9e915e4e576201bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9ec2a872083329d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9edacb4de19eeb8b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9f0f8b1c56898117
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9f2c57bc030e0b04
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/9f330edc61f02d3c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a0572377dc282cac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a113f7e28da04408
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a24edf91b0bcff12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a2fe93c3bba310b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a38eff4f06853e65
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a3b201bbf3062966
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a78089cbf54aff62
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a8da9d8efa986532
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a8e4cc571bdde4c0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a925b8cd7505ac0a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a92bb1bdda49ef61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/a943564382aec90a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/aa2551751b9adb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/aa3f7accc1718239
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ab360402eb2d795e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ab4a97b5d68b837a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/abc8db1325696a17
--rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/abe0d13d37518e58
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ac5b9f591ce9edec
--rw-r--r--   0        0        0    10535 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ac8c237c67408442
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/acbc9f45cfeee4dc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/acecedeb9f4dd91a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ad02b8e4575abc6b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ae5a30e888e80958
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/aff288abf6945582
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b03db5008e4f8099
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b08de429bee9ce93
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b2d26e3968f3c218
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b2f061a9d80cfa8f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b4228843afe3d2eb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b56a01688e02e5f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b5c4e8c097cbf198
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b5f69f56d932f0d1
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b6191d72e3d9a646
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b61cd4b71d14e881
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b7331c702909633
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b780a63a1663add6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b7b1c8254943be90
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b7bcb1e4c5eea72b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b81f55dc9d767e8f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b82ae772ad3347b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b89a404ae8aaa495
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b89dc34e1d21508f
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b8ab8c7df580ad75
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b8d965aa2b8fd993
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/b990e7d90d89db2a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ba0f74a0540d9a5a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ba66feb1819b5312
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/bae3ebdf4629f324
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/bbd87fc7f90c1f28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/bd12e3fd28591ae6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/bd1e909ba96cca61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/bdd37795dc331d56
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/bde6d6e902485336
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/bdeb811362915192
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/be4a1815dbb4c4
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/be5eb6e8ff99feab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/be9c428a6192e049
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/beb37e84505d7dd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c027ebb9dc0ed2f1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c0d14d0162a80714
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c10a38d72f60e675
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c121acc012633d2f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c18d3e52506df649
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c250dc207334d18
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c25779f3e34a584a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c293dd30723003b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c3329258d804dff6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c40a4c8f88b65414
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c55a79e89225a078
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c62dd73faf917878
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c6dc2ffa42b39365
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c766d7d105d53e92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c82d4fd611732d02
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c88465e3c1dc503e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c8c7b8092b03fdd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/c9d297807d108576
--rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ca3d1e0ddece82f5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/cb0e3b769b6a1727
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/cb2f84958966b77c
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/cb326dd0ee5910c6
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/cb3dc0c020e8e656
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/cbb8b9fccd8c8746
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/cc518cf199497e9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ccc4c37cd56e46e5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ccf15ba8d3af2d15
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/cd61466cc4a76933
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ce0a51ca403a72f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ce7ae4869b72ad31
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/cee8b7a480495342
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/cfa33b7a8aeb793e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d085b6ebe7bb0389
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d0be3a4705e047c2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d0fd170547b6bb47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d1c81941e3ef2e1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d1d63b74d8d929b9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d203b8acf8460019
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d2cceb9cc8265e7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d3a20b1509715554
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d551c518ebaaf23a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d5a9ce7dc11e5edc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d6b8c7cba735b946
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d825cf3987ee9f33
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d8444fda03b67f2b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d86a45eca9289fa5
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d8fb97841110c062
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d9198ab6e1ae45a0
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d954f2ee22d56fd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d9b321d36a255169
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/d9cd4c2a9ad4580d
--rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/da0cf7e13e17e6a6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/da4aff17737df0c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/da94ab81ae4dffd1
--rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/db73ef232740be87
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/dc4a4b4b55cceada
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/dcb2ce27d1f7cc70
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/de1238012a6853f3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/dec4fb820d1aee1f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/decdb847958ce882
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/df3de5bc83871643
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/dfc2e498a5736fb3
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e067c98663409f12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e07d7deee3f2b1ed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e1bee9edded3d8bd
--rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e24118b3523194dc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e316b4f368a31a2
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e363170c3d5c3781
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e4a016e6cc51d759
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e5693a808221c1e0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e59ac15827b7f1c1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e6237a2dffed4f5f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e6e7d13cd57b4fd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e832a8f80eaf16d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e8ab3d919ff04fd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e8cd5143f259cdce
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/e98cf82519b9efc2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ea450af950172f80
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/eb7748459bd6fe5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ebd9c23038b8db35
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ebe1cb14f0d7ffa9
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ec04e1ad73846b2a
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ed03e948b89996b8
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ed645de094b6d7bb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/edbe26c4bd7599ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/ee965a83d6cd2aaa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f002d9727bf66a12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f1af1d1ebb07ad61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f2942d8cb87b15e9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f333286a82db220d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f4088198fa879c9c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f41987c18d73e01d
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f4d6392808939633
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f4e7c96257c9d24f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f586c8a0f5c58b3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f58e778cbde5b210
--rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f5d61064e60c404b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/f9ab84e0c6669bed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/fa23c022574446ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/fa2e112681e24616
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/fa354595b122bf9c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/faa3132a8644ec4d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/fad49b925cd80258
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/fb9901f753a46f52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/fbd81c0d9b22b507
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/fd089a45384d0959
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 su6-1.6.3/.ruff_cache/content/fd17e608110a0864
--rw-r--r--   0        0        0    25198 2020-02-02 00:00:00.000000 su6-1.6.3/_static/su6.png
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 su6-1.6.3/_static/su6.svg
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 su6-1.6.3/docs/plugins.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_2602a302b50854cf___about___py.html
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_2602a302b50854cf___init___py.html
--rw-r--r--   0        0        0   129856 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_2602a302b50854cf_cli_py.html
--rw-r--r--   0        0        0   148094 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_2602a302b50854cf_core_py.html
--rw-r--r--   0        0        0   102233 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_2602a302b50854cf_plugins_py.html
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_a44f0ac069e85531__shared_py.html
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_a44f0ac069e85531_test_about_py.html
--rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_a44f0ac069e85531_test_cli_py.html
--rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/d_a44f0ac069e85531_test_core_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-1.6.3/htmlcov/style.css
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/bad.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/black_good_mypy_bad.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/empty.toml
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/except_pytest.toml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/fake_module.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/good.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/invalid.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/only_black.toml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/only_mypy.toml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/stop_after_first.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/bad.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/bad.meta.json
--rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.6.3/pytest_examples/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-1.6.3/src/su6/__about__.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 su6-1.6.3/src/su6/__init__.py
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 su6-1.6.3/src/su6/cli.py
--rw-r--r--   0        0        0    18701 2020-02-02 00:00:00.000000 su6-1.6.3/src/su6/core.py
--rw-r--r--   0        0        0    11295 2020-02-02 00:00:00.000000 su6-1.6.3/src/su6/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 su6-1.6.3/src/su6/py.typed
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-1.6.3/tests/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-1.6.3/tests/_shared.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-1.6.3/tests/test_about.py
--rw-r--r--   0        0        0    10098 2020-02-02 00:00:00.000000 su6-1.6.3/tests/test_cli.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 su6-1.6.3/tests/test_core.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 su6-1.6.3/tests/test_plugins.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 su6-1.6.3/tests/test_plugins_config.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-1.6.3/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-1.6.3/LICENSE.txt
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 su6-1.6.3/README.md
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 su6-1.6.3/pyproject.toml
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 su6-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 su6-1.6.4/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6-1.6.4/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 su6-1.6.4/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_socket.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_socket.meta.json
+-rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/colorsys.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/colorsys.meta.json
+-rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/contextvars.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/contextvars.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/copyreg.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/copyreg.meta.json
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/hashlib.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/hashlib.meta.json
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/hmac.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/hmac.meta.json
+-rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/linecache.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/linecache.meta.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mypy_extensions.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mypy_extensions.meta.json
+-rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pty.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pty.meta.json
+-rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pydoc.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pydoc.meta.json
+-rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/queue.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/queue.meta.json
+-rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/secrets.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/secrets.meta.json
+-rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/selectors.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/selectors.meta.json
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/socket.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/socket.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/ssl.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/ssl.meta.json
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/struct.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/struct.meta.json
+-rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sysconfig.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/sysconfig.meta.json
+-rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/token.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/token.meta.json
+-rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tokenize.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tokenize.meta.json
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/zlib.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/zlib.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/events.data.json
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/locks.meta.json
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/mixins.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/mixins.meta.json
+-rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/queues.meta.json
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/taskgroups.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/taskgroups.meta.json
+-rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/threads.meta.json
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/timeouts.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/timeouts.meta.json
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/__init__.data.json
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/__init__.meta.json
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/_width_table.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/_width_table.meta.json
+-rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/brackets.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/brackets.meta.json
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/cache.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/cache.meta.json
+-rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/comments.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/comments.meta.json
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/concurrency.data.json
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/concurrency.meta.json
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/const.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/const.meta.json
+-rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/files.data.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/files.meta.json
+-rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
+-rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/linegen.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/linegen.meta.json
+-rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/lines.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/lines.meta.json
+-rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/mode.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/mode.meta.json
+-rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/nodes.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/nodes.meta.json
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/numerics.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/numerics.meta.json
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/output.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/output.meta.json
+-rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/parsing.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/parsing.meta.json
+-rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/report.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/report.meta.json
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/rusty.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/rusty.meta.json
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/strings.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/strings.meta.json
+-rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/trans.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/black/trans.meta.json
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/__init__.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/__init__.meta.json
+-rw-r--r--   0        0        0    29124 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/cls.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/cls.meta.json
+-rw-r--r--   0        0        0    37587 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/core.data.json
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/core.meta.json
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/dump.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/dump.meta.json
+-rw-r--r--   0        0        0    33281 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/errors.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/errors.meta.json
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/helpers.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/helpers.meta.json
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/postpone.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/postpone.meta.json
+-rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/singleton.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/singleton.meta.json
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/type_converters.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/type_converters.meta.json
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/_types.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json
+-rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/register.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/register.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/__init__.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/__init__.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/ipython.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/ipython.meta.json
+-rw-r--r--   0        0        0    23574 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/main.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/main.meta.json
+-rw-r--r--   0        0        0    52407 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/parser.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/parser.meta.json
+-rw-r--r--   0        0        0    14742 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/variables.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/dotenv/variables.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/html/entities.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/html/entities.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/util.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/util.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0    32124 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0    20473 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    31787 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0    24762 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    38285 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    17455 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    17494 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    37554 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/mdurl/_url.meta.json
+-rw-r--r--   0        0        0    31404 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/tags.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/tags.meta.json
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/utils.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/utils.meta.json
+-rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/__init__.meta.json
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/_meta.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/_meta.meta.json
+-rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/gitignore.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/gitignore.meta.json
+-rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/pathspec.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/pathspec.meta.json
+-rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/pattern.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/pattern.meta.json
+-rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/util.data.json
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/util.meta.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
+-rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
+-rw-r--r--   0        0        0    27179 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/__init__.meta.json
+-rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/android.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/android.meta.json
+-rw-r--r--   0        0        0    42401 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/api.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/api.meta.json
+-rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/unix.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/unix.meta.json
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/version.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/platformdirs/version.meta.json
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/__init__.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/__main__.data.json
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_extension.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_fileno.meta.json
+-rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_inspect.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_inspect.meta.json
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_loop.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_loop.meta.json
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_pick.data.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_stack.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_timer.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_timer.meta.json
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_windows.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/abc.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/abc.meta.json
+-rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/align.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/align.meta.json
+-rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/ansi.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/ansi.meta.json
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/box.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/box.meta.json
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/cells.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/cells.meta.json
+-rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/color.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/color.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/columns.data.json
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/columns.meta.json
+-rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/console.data.json
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/console.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/constrain.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/constrain.meta.json
+-rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/containers.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/containers.meta.json
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/control.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/control.meta.json
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/default_styles.data.json
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/emoji.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/errors.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/errors.meta.json
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/json.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/json.meta.json
+-rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/live.data.json
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/live.meta.json
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/live_render.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/live_render.meta.json
+-rw-r--r--   0        0        0    82219 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/markdown.data.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/markdown.meta.json
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/markup.data.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/markup.meta.json
+-rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/measure.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/measure.meta.json
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/padding.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/padding.meta.json
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/pager.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/pager.meta.json
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/palette.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/palette.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/panel.data.json
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/panel.meta.json
+-rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/pretty.data.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/protocol.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/protocol.meta.json
+-rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/region.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/region.meta.json
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/repr.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/repr.meta.json
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/rule.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/rule.meta.json
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/scope.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/scope.meta.json
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/screen.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/screen.meta.json
+-rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/segment.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/segment.meta.json
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/spinner.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/spinner.meta.json
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/status.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/status.meta.json
+-rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/style.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/style.meta.json
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/styled.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/styled.meta.json
+-rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/syntax.data.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/syntax.meta.json
+-rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/table.data.json
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/table.meta.json
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/text.data.json
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/text.meta.json
+-rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/theme.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/theme.meta.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/themes.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/themes.meta.json
+-rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/traceback.data.json
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/rich/traceback.meta.json
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/__about__.data.json
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/__about__.meta.json
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/__init__.data.json
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/__init__.meta.json
+-rw-r--r--   0        0        0    26556 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/cli.data.json
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/cli.meta.json
+-rw-r--r--   0        0        0    56204 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/core.data.json
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/core.meta.json
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/helpers.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/helpers.meta.json
+-rw-r--r--   0        0        0    49469 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/plugins.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/su6/plugins.meta.json
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli/__init__.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli/__init__.meta.json
+-rw-r--r--   0        0        0    52646 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli/_parser.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli/_parser.meta.json
+-rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli/_re.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli/_re.meta.json
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli/_types.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli/_types.meta.json
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli_w/__init__.data.json
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli_w/__init__.meta.json
+-rw-r--r--   0        0        0    31248 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli_w/_writer.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomli_w/_writer.meta.json
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/__init__.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/__init__.meta.json
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/_compat.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/_compat.meta.json
+-rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/_utils.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/_utils.meta.json
+-rw-r--r--   0        0        0    19946 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/api.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/api.meta.json
+-rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/container.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/container.meta.json
+-rw-r--r--   0        0        0    33007 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/exceptions.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/exceptions.meta.json
+-rw-r--r--   0        0        0   221620 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/items.data.json
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/items.meta.json
+-rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/parser.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/parser.meta.json
+-rw-r--r--   0        0        0    22900 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/source.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/source.meta.json
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/toml_char.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/toml_char.meta.json
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/toml_document.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/tomlkit/toml_document.meta.json
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/__init__.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/__init__.meta.json
+-rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_checkers.data.json
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_checkers.meta.json
+-rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_config.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_config.meta.json
+-rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_decorators.data.json
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_decorators.meta.json
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_exceptions.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_exceptions.meta.json
+-rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_functions.data.json
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_functions.meta.json
+-rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_importhook.data.json
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_importhook.meta.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_memo.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_memo.meta.json
+-rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_suppression.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_suppression.meta.json
+-rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_transformer.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_transformer.meta.json
+-rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_utils.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typeguard/_utils.meta.json
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/mock.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/mock.meta.json
+-rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.6.4/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-1.6.4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-1.6.4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-1.6.4/.pytest_cache/README.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 su6-1.6.4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 su6-1.6.4/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.6.4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/10595a931c3c881e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1065c8b44fadc39a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1086635a5970b925
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/10ab08017438a66a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/10c2ae33c509be23
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/11152902676027343458
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/11f25cfda4e2f210
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/122419b0bc04bb24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1322b93a2154c54a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/134e5e8c29726e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/13985ae090677282
+-rw-r--r--   0        0        0    44502 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/14681219216720271199
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/146952ec4263c5d9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/150d086b8b4de9d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/156301591af184f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1663be342a34f83
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1895bed4a0ed65d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1996a22aec44a5c0
+-rw-r--r--   0        0        0    16044 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1a4449eb8b26a401
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1a4db4c4834af592
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1b0530edc3fe075e
+-rw-r--r--   0        0        0    21464 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1b7872d6314f48b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1ce202f3daa889d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1cfd31ba4b0b7ef9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1d75413e215f93c6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1dcbdc62e66ccf0e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1edace855ae3c841
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1f7ac4f892285f60
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1f88fbdfcbf2d8d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/1fbfdffa4078f509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/20b40aca78f395e8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/219bf1f8f2938bd4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/21b248d368a93ac8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/21cf950ddc412c7b
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/22a98eb4527b8ca5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/22d9a59d8d30ba9d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/22db1408b8f4a4b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/232d0222563916a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/23680c0655621b13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/23da3e9165a5513d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/247546336fc4bd59
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/248d23bfc4586461
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/24e2ebef92fa75b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/25d9504d2b6847d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/26657ed11f8e66de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/269f98f304a03fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/27ca2458f5ee73fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/28caf6cfecd38c1a
+-rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/294d5a468695eb7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/29531d612e8a868a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2a383abdede299d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2a5d8d1386804aed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2a630c7d6d7faa40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2b0cdebce71424f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2bc4a20be77b881b
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2bf27b960bc3ded1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2c189a9882594507
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2c6eeab804b5c1f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2c9bbc6bae6b0f41
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2d77da04c7119543
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2e4746b83d2d1cf8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2e6b6d5e70ae29db
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2e8708077cd0413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2f9e25dc2ce777cc
+-rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/2face4e073dced28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/300f9a816018d49f
+-rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/30e241b2876dc71f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/31813abf4ed82b53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3271e344462a0ee3
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/33004598889f4950
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/349f044f89b94587
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/34a4aaded634d537
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/34e1109d49bf09f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/356d28a11355e7a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/357e837fe90ee680
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/35ab5ee4981cdf8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/35ba35b3f04c192f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/36372ef94f8716cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/36e48551be186a66
+-rw-r--r--   0        0        0    16058 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/36f0bdaeef592d9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/380a13ecd1a2af25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/38962215221b245a
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/38b035e004ea9f4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/38d9da4e93811c4f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/39285e72757cc499
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/399d3b28a1a1db47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3a74e1b5704e9b3f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3af645c926072f97
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3c6b70c96e832bc1
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3c7fb493febe6a55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3c9bb20c3b57bae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3ca706f99b2d38bf
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3ccdd2336c8c80e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3cf13d9d13babf93
+-rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3db675ebeb97b2fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3dfac0c0edd78d53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3e0ec316d612ddc6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3e35311bfb3345f8
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3f10d9d7687f3999
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/3f12e7a3fe46c220
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/417040cdeaa7bd81
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/429010e306ea9808
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/42f337caed884834
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/431bdba29473eca0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4536434fd84cdba5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/454cfd5b3ba01a90
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/467fc2e82c277fd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/47affd4e531897a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/47ca38fe0242f05d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/47e54ee652d2f4c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4843e1c724479e6a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/484730e7d1a4dcd9
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4880724f1f6a1ac8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/48bda5931a9eb062
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/49b4fe40533bd678
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/49fafbbbbadedf00
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4a63ed784e7c5ec0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4ac8c08e5b1b6650
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4b5890a0c8dc15df
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4cd4c52ee1dc7ffe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4cdd16a7f9738f22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4d5914600f7e99c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4eaf3b155fae0dfb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4f16c6852dea8eca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4f2c663677c63589
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4f75816f4078d31b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4f8371badac33c92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/4fafe0dbefb778fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/50373733f4645c5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/514fb27e4aef5783
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/519ab6ce866ef11b
+-rw-r--r--   0        0        0    18347 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/51de14ac05bcd5d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/529312a72d1177a1
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/534b8acecf74c47
+-rw-r--r--   0        0        0    20136 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/536320baecd03af6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/538fc0618c4d4c31
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/53c0f85a3179a38f
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5436d767d06cf116
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/54637ff0aaaaf6b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/552fa1eb2057eecc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5548c3ce5fff0cca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/556b5cfaac0c49bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/55c947c0fa59929
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/568d77a0a0a64dbc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/56e83f1c5eeb3eba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/572ba1efb5bb3fd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/58240cde188220d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/584058f21d3e2fa1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/594d55ee247cbdef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/59cfab1472b544fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5a6dc8ef65620223
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5af13ad9cc04e932
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5b7183ee842066de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5b8fb96822a8f127
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5b965ef6adf36c8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5badc1835a2b80e1
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5cc5d54a963753bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5da466fd7e3b19f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5e83ab1d520dc773
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5efe825a5e773b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5f4cf7812d590c90
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/5fb3763e0810c38a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/62396a4dea084957
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/624348590d33bdc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6278996c2e6b2a87
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/63dbabe01e9e6756
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6550bbd98b1711bd
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6644351985978373760
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6791fc0114ddc05
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6845ca4e0c56952b
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/684d0841c18787fb
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/68c4553df91c1f5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/69bb9ea6355c0c25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/69ffc3e7ad0aa6b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6a4adfab73a8d4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6a74d0efd6350f1e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6b596d4ac1166741
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6b9f30172d33b6a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6bcca98e41cda3f4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6beed9d45ff1a491
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6c989c6e4eea10bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6db20c27780d4a5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6db875fe1541793e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6eab8cdd7b4ae170
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/6fc044c94dc3532a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/701212523f7b3b9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/70963c0c68bf76ac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/70bd045859d6cb20
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/70d6f3b95738758d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/729f212cc9c6cd5d
+-rw-r--r--   0        0        0    20572 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/72a6612daca66426
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/72de7bec9ecb53aa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/733b2373fa4ae335
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7396a954cc3b124a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7485843a948a75b0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/755c9c217a06f932
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/75bb48e114159509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/76d56794deeb084d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/76fbe2af0f71bd4a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/79a22043e5c16946
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/79c3fb2c81fd59a0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7a19353a5daa4a37
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7b3a1bf0b652398a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7bf45647f43eaf85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7c01d9689dd16a64
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7c37d34a0c059ec7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7c806e58272a88ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7cbc35f4e814db65
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7cc3783d00621498
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7cf495b196c50222
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7dc27d897f910c11
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7e138932f0b9a1bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7eb1422c10ced038
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7eb17a25b4fa1d13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7f0f63895e369318
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/7f75cbd11ebac70a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8012caf4fb290dc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/80844117d21fe12b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/809075c58fb87c61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/80dbccb0d26b4b4f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/80ded2016f4f413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/81e3edf198d6c468
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/81e6f787866d0ecf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/82ab0276d38aec9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/835f19fb8c240dbe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/83a59cf9aceae1d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/83cdfb5da134b21f
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8479781080806744663
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/84bb9d90fe3a6595
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/84e2e26fc69ab274
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/84e8c31ce428d3ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/858df3976aef9624
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/868699acd08be339
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/86c3e5b9f79f490f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/87a7b0840a5cf8c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/87d9b6d5e7bcb6c7
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/881c84062ed51136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/886d14b97dbd4f2e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8944dfd1b590bdd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/89c7a4d643f68517
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/89e58e5ee0d7d864
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8a0279b11d098d9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8a437c05421c6cb5
+-rw-r--r--   0        0        0    20054 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8a5ec4ca9660671c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8b8acf1607bcb3f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8c34e85d573e230f
+-rw-r--r--   0        0        0    17871 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8ccd539b7f96dff8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8d2f83aae152de29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8df3988e9368cbe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/8f33397e19bead30
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9019e33ca68d8935
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/902eb6f99ee41131
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/906cef8208fbf28f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9080aaa3f2416b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/922bfc03482db456
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/92db151fe9967fd3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9352425265579062
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/93fed7ae4120c88e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/945994955724de24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/94ffcc82bc7ee370
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/95df46a8e947b100
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9613cbbc5a7c60a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/968b32ac9319cc53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/97a72bc70808d2f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/97cbf45b388709d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/97df9d79e599f082
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/981eb70eb69fb3ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/98392e87ef3eb254
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/99d5decc6ca01825
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9a5552199a8b8bd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9bd08ae684645cf6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9c1285d5b3178abe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9cbaa57406e65f63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9d0f65e1ab7ca23
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9db15fb6e71bec4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9dda9185d48774f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9e3b1a7c0f34103b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9e50a4d6fb3c9688
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9e558f66f216c4eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9e915e4e576201bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9ec2a872083329d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9edacb4de19eeb8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9f0f8b1c56898117
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9f2c57bc030e0b04
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/9f330edc61f02d3c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a0572377dc282cac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a113f7e28da04408
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a24edf91b0bcff12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a2fe93c3bba310b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a38eff4f06853e65
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a3b201bbf3062966
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a78089cbf54aff62
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a8da9d8efa986532
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a8e4cc571bdde4c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a925b8cd7505ac0a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a92bb1bdda49ef61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/a943564382aec90a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/aa2551751b9adb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/aa3f7accc1718239
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ab360402eb2d795e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ab4a97b5d68b837a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/abc8db1325696a17
+-rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/abe0d13d37518e58
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ac5b9f591ce9edec
+-rw-r--r--   0        0        0    10535 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ac8c237c67408442
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/acbc9f45cfeee4dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/acecedeb9f4dd91a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ad02b8e4575abc6b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ae5a30e888e80958
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/aff288abf6945582
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b03db5008e4f8099
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b08de429bee9ce93
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b2d26e3968f3c218
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b2f061a9d80cfa8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b4228843afe3d2eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b56a01688e02e5f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b5c4e8c097cbf198
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b5f69f56d932f0d1
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b6191d72e3d9a646
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b61cd4b71d14e881
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b7331c702909633
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b780a63a1663add6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b7b1c8254943be90
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b7bcb1e4c5eea72b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b81f55dc9d767e8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b82ae772ad3347b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b89a404ae8aaa495
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b89dc34e1d21508f
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b8ab8c7df580ad75
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b8d965aa2b8fd993
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/b990e7d90d89db2a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ba0f74a0540d9a5a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ba66feb1819b5312
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/bae3ebdf4629f324
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/bbd87fc7f90c1f28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/bd12e3fd28591ae6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/bd1e909ba96cca61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/bdd37795dc331d56
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/bde6d6e902485336
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/bdeb811362915192
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/be4a1815dbb4c4
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/be5eb6e8ff99feab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/be9c428a6192e049
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/beb37e84505d7dd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c027ebb9dc0ed2f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c0d14d0162a80714
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c10a38d72f60e675
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c121acc012633d2f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c18d3e52506df649
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c250dc207334d18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c25779f3e34a584a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c293dd30723003b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c3329258d804dff6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c40a4c8f88b65414
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c55a79e89225a078
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c62dd73faf917878
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c6dc2ffa42b39365
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c766d7d105d53e92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c82d4fd611732d02
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c88465e3c1dc503e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c8c7b8092b03fdd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/c9d297807d108576
+-rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ca3d1e0ddece82f5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/cb0e3b769b6a1727
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/cb2f84958966b77c
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/cb326dd0ee5910c6
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/cb3dc0c020e8e656
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/cbb8b9fccd8c8746
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/cc518cf199497e9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ccc4c37cd56e46e5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ccf15ba8d3af2d15
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/cd61466cc4a76933
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ce0a51ca403a72f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ce7ae4869b72ad31
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/cee8b7a480495342
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/cfa33b7a8aeb793e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d085b6ebe7bb0389
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d0be3a4705e047c2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d0fd170547b6bb47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d1c81941e3ef2e1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d1d63b74d8d929b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d203b8acf8460019
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d2cceb9cc8265e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d3a20b1509715554
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d551c518ebaaf23a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d5a9ce7dc11e5edc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d6b8c7cba735b946
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d825cf3987ee9f33
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d8444fda03b67f2b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d86a45eca9289fa5
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d8fb97841110c062
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d9198ab6e1ae45a0
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d954f2ee22d56fd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d9b321d36a255169
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/d9cd4c2a9ad4580d
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/da0cf7e13e17e6a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/da4aff17737df0c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/da94ab81ae4dffd1
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/db73ef232740be87
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/dc4a4b4b55cceada
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/dcb2ce27d1f7cc70
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/de1238012a6853f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/dec4fb820d1aee1f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/decdb847958ce882
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/df3de5bc83871643
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/dfc2e498a5736fb3
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e067c98663409f12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e07d7deee3f2b1ed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e1bee9edded3d8bd
+-rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e24118b3523194dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e316b4f368a31a2
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e363170c3d5c3781
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e4a016e6cc51d759
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e5693a808221c1e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e59ac15827b7f1c1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e6237a2dffed4f5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e6e7d13cd57b4fd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e832a8f80eaf16d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e8ab3d919ff04fd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e8cd5143f259cdce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/e98cf82519b9efc2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ea450af950172f80
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/eb7748459bd6fe5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ebd9c23038b8db35
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ebe1cb14f0d7ffa9
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ec04e1ad73846b2a
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ed03e948b89996b8
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ed645de094b6d7bb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/edbe26c4bd7599ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/ee965a83d6cd2aaa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f002d9727bf66a12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f1af1d1ebb07ad61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f2942d8cb87b15e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f333286a82db220d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f4088198fa879c9c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f41987c18d73e01d
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f4d6392808939633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f4e7c96257c9d24f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f586c8a0f5c58b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f58e778cbde5b210
+-rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f5d61064e60c404b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/f9ab84e0c6669bed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/fa23c022574446ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/fa2e112681e24616
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/fa354595b122bf9c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/faa3132a8644ec4d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/fad49b925cd80258
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/fb9901f753a46f52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/fbd81c0d9b22b507
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/fd089a45384d0959
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 su6-1.6.4/.ruff_cache/content/fd17e608110a0864
+-rw-r--r--   0        0        0    25198 2020-02-02 00:00:00.000000 su6-1.6.4/_static/su6.png
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 su6-1.6.4/_static/su6.svg
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 su6-1.6.4/docs/plugins.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_2602a302b50854cf___about___py.html
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_2602a302b50854cf___init___py.html
+-rw-r--r--   0        0        0   129856 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_2602a302b50854cf_cli_py.html
+-rw-r--r--   0        0        0   148094 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_2602a302b50854cf_core_py.html
+-rw-r--r--   0        0        0   102233 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_2602a302b50854cf_plugins_py.html
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_a44f0ac069e85531__shared_py.html
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_a44f0ac069e85531_test_about_py.html
+-rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_a44f0ac069e85531_test_cli_py.html
+-rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/d_a44f0ac069e85531_test_core_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-1.6.4/htmlcov/style.css
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/bad.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/black_good_mypy_bad.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/empty.toml
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/except_pytest.toml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/fake_module.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/good.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/invalid.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/only_black.toml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/only_mypy.toml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/stop_after_first.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/bad.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/bad.meta.json
+-rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.6.4/pytest_examples/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-1.6.4/src/su6/__about__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 su6-1.6.4/src/su6/__init__.py
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 su6-1.6.4/src/su6/cli.py
+-rw-r--r--   0        0        0    18511 2020-02-02 00:00:00.000000 su6-1.6.4/src/su6/core.py
+-rw-r--r--   0        0        0    11295 2020-02-02 00:00:00.000000 su6-1.6.4/src/su6/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 su6-1.6.4/src/su6/py.typed
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-1.6.4/tests/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-1.6.4/tests/_shared.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-1.6.4/tests/test_about.py
+-rw-r--r--   0        0        0    10098 2020-02-02 00:00:00.000000 su6-1.6.4/tests/test_cli.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 su6-1.6.4/tests/test_core.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 su6-1.6.4/tests/test_plugins.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 su6-1.6.4/tests/test_plugins_config.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-1.6.4/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-1.6.4/LICENSE.txt
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 su6-1.6.4/README.md
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 su6-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 su6-1.6.4/PKG-INFO
```

### Comparing `su6-1.6.3/CHANGELOG.md` & `su6-1.6.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.6.4 (2023-07-21)
+
+### Refactor
+
+* refactor: moved pyproject logic to configuraptor and bumped dependency version
+
 ## v1.6.3 (2023-07-17)
 
 ### Documentation
 
-* **plugins:** Added `prettier` extra ([`f1f0d34`](https://github.com/robinvandernoord/su6-checker/commit/f1f0d3402bc5b8eb5ffc6eceedce6ef83ba30141))
+* **plugins:** Added `prettier`
+  extra ([`f1f0d34`](https://github.com/robinvandernoord/su6-checker/commit/f1f0d3402bc5b8eb5ffc6eceedce6ef83ba30141))
 
 ## v1.6.2 (2023-07-17)
 
 ### Feature
 
-* Add su6[svelte-check] as extra ([`558a2be`](https://github.com/robinvandernoord/su6-checker/commit/558a2bee214f5294e8193765d5a4566a85afdc6f))
+* Add su6[svelte-check] as
+  extra ([`558a2be`](https://github.com/robinvandernoord/su6-checker/commit/558a2bee214f5294e8193765d5a4566a85afdc6f))
 
 ## v1.6.1 (2023-07-17)
 
 ### Fix
 
-* **tool:** Don't show full executable path in output, only tool name ([`2ec226f`](https://github.com/robinvandernoord/su6-checker/commit/2ec226f62349c048221a056d2b504e38048c5706))
+* **tool:** Don't show full executable path in output, only tool
+  name ([`2ec226f`](https://github.com/robinvandernoord/su6-checker/commit/2ec226f62349c048221a056d2b504e38048c5706))
 
 ## v1.6.0 (2023-07-17)
 
 ### Feature
 
-* Allow `add_to_all` and `add_to_fix` to plugin registration ([`f0c501b`](https://github.com/robinvandernoord/su6-checker/commit/f0c501b76c9e8baad37178f45ec83fd23f91d446))
+* Allow `add_to_all` and `add_to_fix` to plugin
+  registration ([`f0c501b`](https://github.com/robinvandernoord/su6-checker/commit/f0c501b76c9e8baad37178f45ec83fd23f91d446))
 
 ### Documentation
 
-* **plugins:** Added more info about `add_to_*` and the svelte-check plugin ([`3e0051c`](https://github.com/robinvandernoord/su6-checker/commit/3e0051c968f97883ef7dc7859bdf5b3138753c73))
-* **pypi:** Indicate 3.10 support ([`a547da0`](https://github.com/robinvandernoord/su6-checker/commit/a547da0783cfccfa058b780bcdbe8130e9cf3e62))
+* **plugins:** Added more info about `add_to_*` and the svelte-check
+  plugin ([`3e0051c`](https://github.com/robinvandernoord/su6-checker/commit/3e0051c968f97883ef7dc7859bdf5b3138753c73))
+* **pypi:** Indicate 3.10
+  support ([`a547da0`](https://github.com/robinvandernoord/su6-checker/commit/a547da0783cfccfa058b780bcdbe8130e9cf3e62))
 
 ## v1.5.2 (2023-06-21)
 
-
-
 ## v1.5.1 (2023-06-20)
 
 ### Documentation
 
-* **logo:** Use png instead of svg because that was being funky ([`89d71a5`](https://github.com/robinvandernoord/su6-checker/commit/89d71a59a74f046f5daa5da2180505676b273318))
-* **changelog:** Manually added change for 1.5.0 ([`3713a6b`](https://github.com/robinvandernoord/su6-checker/commit/3713a6bc61ef2eaa930721f7a7e6caa9cbbefe22))
+* **logo:** Use png instead of svg because that was being
+  funky ([`89d71a5`](https://github.com/robinvandernoord/su6-checker/commit/89d71a59a74f046f5daa5da2180505676b273318))
+* **changelog:** Manually added change for
+  1.5.0 ([`3713a6b`](https://github.com/robinvandernoord/su6-checker/commit/3713a6bc61ef2eaa930721f7a7e6caa9cbbefe22))
 
 ## v1.5.0 (2023-06-20)
 
 ### Feature
 
 * Support Python 3.10
```

### Comparing `su6-1.6.3/coverage.svg` & `su6-1.6.4/coverage.svg`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/__future__.data.json` & `su6-1.6.4/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/__future__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_ast.data.json` & `su6-1.6.4/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_ast.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_codecs.data.json` & `su6-1.6.4/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_codecs.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_collections_abc.data.json` & `su6-1.6.4/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_csv.data.json` & `su6-1.6.4/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_csv.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_ctypes.data.json` & `su6-1.6.4/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_ctypes.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_decimal.data.json` & `su6-1.6.4/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_decimal.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_operator.data.json` & `su6-1.6.4/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_operator.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_random.data.json` & `su6-1.6.4/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_random.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_socket.data.json` & `su6-1.6.4/.mypy_cache/3.11/_socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_socket.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_stat.data.json` & `su6-1.6.4/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_stat.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_thread.data.json` & `su6-1.6.4/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_thread.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_warnings.data.json` & `su6-1.6.4/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_warnings.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_weakref.data.json` & `su6-1.6.4/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_weakref.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_weakrefset.data.json` & `su6-1.6.4/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_weakrefset.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/abc.data.json` & `su6-1.6.4/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/abc.meta.json` & `su6-1.6.4/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/argparse.data.json` & `su6-1.6.4/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/argparse.meta.json` & `su6-1.6.4/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/array.data.json` & `su6-1.6.4/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/array.meta.json` & `su6-1.6.4/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/ast.data.json` & `su6-1.6.4/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/ast.meta.json` & `su6-1.6.4/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/builtins.data.json` & `su6-1.6.4/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/builtins.meta.json` & `su6-1.6.4/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/codecs.data.json` & `su6-1.6.4/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/codecs.meta.json` & `su6-1.6.4/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/colorsys.data.json` & `su6-1.6.4/.mypy_cache/3.11/colorsys.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/colorsys.meta.json` & `su6-1.6.4/.mypy_cache/3.11/colorsys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configparser.data.json` & `su6-1.6.4/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configparser.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/contextlib.data.json` & `su6-1.6.4/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/contextlib.meta.json` & `su6-1.6.4/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/contextvars.data.json` & `su6-1.6.4/.mypy_cache/3.11/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/contextvars.meta.json` & `su6-1.6.4/.mypy_cache/3.11/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/copy.data.json` & `su6-1.6.4/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/copy.meta.json` & `su6-1.6.4/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/copyreg.data.json` & `su6-1.6.4/.mypy_cache/3.11/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/copyreg.meta.json` & `su6-1.6.4/.mypy_cache/3.11/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/csv.data.json` & `su6-1.6.4/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/csv.meta.json` & `su6-1.6.4/.mypy_cache/3.11/csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dataclasses.data.json` & `su6-1.6.4/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dataclasses.meta.json` & `su6-1.6.4/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/datetime.data.json` & `su6-1.6.4/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/datetime.meta.json` & `su6-1.6.4/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/decimal.data.json` & `su6-1.6.4/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/decimal.meta.json` & `su6-1.6.4/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/difflib.data.json` & `su6-1.6.4/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/difflib.meta.json` & `su6-1.6.4/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dis.data.json` & `su6-1.6.4/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dis.meta.json` & `su6-1.6.4/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/enum.data.json` & `su6-1.6.4/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/enum.meta.json` & `su6-1.6.4/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/errno.data.json` & `su6-1.6.4/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/errno.meta.json` & `su6-1.6.4/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/fractions.data.json` & `su6-1.6.4/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/fractions.meta.json` & `su6-1.6.4/.mypy_cache/3.11/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/functools.data.json` & `su6-1.6.4/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/functools.meta.json` & `su6-1.6.4/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/genericpath.data.json` & `su6-1.6.4/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/genericpath.meta.json` & `su6-1.6.4/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/getpass.data.json` & `su6-1.6.4/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/getpass.meta.json` & `su6-1.6.4/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/gettext.data.json` & `su6-1.6.4/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/gettext.meta.json` & `su6-1.6.4/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/glob.data.json` & `su6-1.6.4/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/glob.meta.json` & `su6-1.6.4/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/good.data.json` & `su6-1.6.4/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/good.meta.json` & `su6-1.6.4/.mypy_cache/3.11/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/hashlib.data.json` & `su6-1.6.4/.mypy_cache/3.11/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/hashlib.meta.json` & `su6-1.6.4/.mypy_cache/3.11/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/hmac.data.json` & `su6-1.6.4/.mypy_cache/3.11/hmac.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/hmac.meta.json` & `su6-1.6.4/.mypy_cache/3.11/hmac.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/inspect.data.json` & `su6-1.6.4/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/inspect.meta.json` & `su6-1.6.4/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/io.data.json` & `su6-1.6.4/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/io.meta.json` & `su6-1.6.4/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/itertools.data.json` & `su6-1.6.4/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/itertools.meta.json` & `su6-1.6.4/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/linecache.data.json` & `su6-1.6.4/.mypy_cache/3.11/linecache.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/linecache.meta.json` & `su6-1.6.4/.mypy_cache/3.11/linecache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/marshal.data.json` & `su6-1.6.4/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/marshal.meta.json` & `su6-1.6.4/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/math.data.json` & `su6-1.6.4/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/math.meta.json` & `su6-1.6.4/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mmap.data.json` & `su6-1.6.4/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mmap.meta.json` & `su6-1.6.4/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/msvcrt.data.json` & `su6-1.6.4/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/msvcrt.meta.json` & `su6-1.6.4/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mypy_extensions.data.json` & `su6-1.6.4/.mypy_cache/3.11/mypy_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mypy_extensions.meta.json` & `su6-1.6.4/.mypy_cache/3.11/mypy_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/numbers.data.json` & `su6-1.6.4/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/numbers.meta.json` & `su6-1.6.4/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/opcode.data.json` & `su6-1.6.4/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/opcode.meta.json` & `su6-1.6.4/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/operator.data.json` & `su6-1.6.4/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/operator.meta.json` & `su6-1.6.4/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathlib.data.json` & `su6-1.6.4/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathlib.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pickle.data.json` & `su6-1.6.4/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pickle.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platform.data.json` & `su6-1.6.4/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platform.meta.json` & `su6-1.6.4/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/posixpath.data.json` & `su6-1.6.4/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/posixpath.meta.json` & `su6-1.6.4/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pty.data.json` & `su6-1.6.4/.mypy_cache/3.11/pty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pty.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pydoc.data.json` & `su6-1.6.4/.mypy_cache/3.11/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pydoc.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pydoc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/queue.data.json` & `su6-1.6.4/.mypy_cache/3.11/queue.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/queue.meta.json` & `su6-1.6.4/.mypy_cache/3.11/queue.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/random.data.json` & `su6-1.6.4/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/random.meta.json` & `su6-1.6.4/.mypy_cache/3.11/random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/re.data.json` & `su6-1.6.4/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/re.meta.json` & `su6-1.6.4/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/reprlib.data.json` & `su6-1.6.4/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/reprlib.meta.json` & `su6-1.6.4/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/secrets.data.json` & `su6-1.6.4/.mypy_cache/3.11/secrets.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/secrets.meta.json` & `su6-1.6.4/.mypy_cache/3.11/secrets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/selectors.data.json` & `su6-1.6.4/.mypy_cache/3.11/selectors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/selectors.meta.json` & `su6-1.6.4/.mypy_cache/3.11/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/shlex.data.json` & `su6-1.6.4/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/shlex.meta.json` & `su6-1.6.4/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/shutil.data.json` & `su6-1.6.4/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/shutil.meta.json` & `su6-1.6.4/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/signal.data.json` & `su6-1.6.4/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/signal.meta.json` & `su6-1.6.4/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/socket.data.json` & `su6-1.6.4/.mypy_cache/3.11/socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/socket.meta.json` & `su6-1.6.4/.mypy_cache/3.11/socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sre_compile.data.json` & `su6-1.6.4/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sre_compile.meta.json` & `su6-1.6.4/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sre_constants.data.json` & `su6-1.6.4/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sre_constants.meta.json` & `su6-1.6.4/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sre_parse.data.json` & `su6-1.6.4/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sre_parse.meta.json` & `su6-1.6.4/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/ssl.data.json` & `su6-1.6.4/.mypy_cache/3.11/ssl.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/ssl.meta.json` & `su6-1.6.4/.mypy_cache/3.11/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/stat.data.json` & `su6-1.6.4/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/stat.meta.json` & `su6-1.6.4/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/string.data.json` & `su6-1.6.4/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/string.meta.json` & `su6-1.6.4/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/struct.data.json` & `su6-1.6.4/.mypy_cache/3.11/struct.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/struct.meta.json` & `su6-1.6.4/.mypy_cache/3.11/struct.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/subprocess.data.json` & `su6-1.6.4/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/subprocess.meta.json` & `su6-1.6.4/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sys.data.json` & `su6-1.6.4/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sys.meta.json` & `su6-1.6.4/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sysconfig.data.json` & `su6-1.6.4/.mypy_cache/3.11/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/sysconfig.meta.json` & `su6-1.6.4/.mypy_cache/3.11/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tempfile.data.json` & `su6-1.6.4/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tempfile.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/termios.data.json` & `su6-1.6.4/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/termios.meta.json` & `su6-1.6.4/.mypy_cache/3.11/termios.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/textwrap.data.json` & `su6-1.6.4/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/textwrap.meta.json` & `su6-1.6.4/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/this.data.json` & `su6-1.6.4/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/this.meta.json` & `su6-1.6.4/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/threading.data.json` & `su6-1.6.4/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/threading.meta.json` & `su6-1.6.4/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/time.data.json` & `su6-1.6.4/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/time.meta.json` & `su6-1.6.4/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/token.data.json` & `su6-1.6.4/.mypy_cache/3.11/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/token.meta.json` & `su6-1.6.4/.mypy_cache/3.11/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tokenize.data.json` & `su6-1.6.4/.mypy_cache/3.11/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tokenize.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomllib.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomllib.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomllib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/traceback.data.json` & `su6-1.6.4/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/traceback.meta.json` & `su6-1.6.4/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tty.data.json` & `su6-1.6.4/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tty.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/types.data.json` & `su6-1.6.4/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/types.meta.json` & `su6-1.6.4/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typing.data.json` & `su6-1.6.4/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typing.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typing_extensions.data.json` & `su6-1.6.4/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/uuid.data.json` & `su6-1.6.4/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/uuid.meta.json` & `su6-1.6.4/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/warnings.data.json` & `su6-1.6.4/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/warnings.meta.json` & `su6-1.6.4/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/weakref.data.json` & `su6-1.6.4/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/weakref.meta.json` & `su6-1.6.4/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/webbrowser.data.json` & `su6-1.6.4/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/webbrowser.meta.json` & `su6-1.6.4/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/zlib.data.json` & `su6-1.6.4/.mypy_cache/3.11/zlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/zlib.meta.json` & `su6-1.6.4/.mypy_cache/3.11/zlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/base_events.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/base_events.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/coroutines.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/coroutines.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/events.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/events.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/exceptions.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/exceptions.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/futures.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/futures.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/locks.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/locks.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/mixins.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/mixins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/mixins.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/protocols.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/protocols.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/queues.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/queues.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/runners.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/runners.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/selector_events.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/selector_events.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/streams.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/streams.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/subprocess.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/subprocess.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/taskgroups.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/taskgroups.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/taskgroups.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/taskgroups.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/tasks.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/tasks.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/threads.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/threads.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/threads.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/threads.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/timeouts.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/timeouts.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/timeouts.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/timeouts.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/transports.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/transports.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/unix_events.data.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/asyncio/unix_events.meta.json` & `su6-1.6.4/.mypy_cache/3.11/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/_width_table.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/_width_table.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/_width_table.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/_width_table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/brackets.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/brackets.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/brackets.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/brackets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/cache.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/cache.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/cache.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/cache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/comments.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/comments.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/comments.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/comments.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/concurrency.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/concurrency.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/concurrency.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/concurrency.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/const.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/const.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/const.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/const.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/files.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/files.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/files.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/files.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/handle_ipynb_magics.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/handle_ipynb_magics.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/linegen.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/linegen.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/linegen.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/linegen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/lines.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/lines.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/lines.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/lines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/mode.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/mode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/mode.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/mode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/nodes.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/nodes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/nodes.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/numerics.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/numerics.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/numerics.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/numerics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/output.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/output.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/output.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/output.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/parsing.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/parsing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/parsing.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/parsing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/report.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/report.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/report.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/report.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/rusty.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/rusty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/rusty.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/rusty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/strings.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/strings.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/strings.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/strings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/trans.data.json` & `su6-1.6.4/.mypy_cache/3.11/black/trans.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/black/trans.meta.json` & `su6-1.6.4/.mypy_cache/3.11/black/trans.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/_compat.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/_compat.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/_termui_impl.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/_termui_impl.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/_textwrap.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/_textwrap.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/core.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/core.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/decorators.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/decorators.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/exceptions.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/exceptions.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/formatting.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/formatting.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/globals.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/globals.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/parser.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/parser.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/shell_completion.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/shell_completion.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/termui.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/termui.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/types.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/types.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/utils.data.json` & `su6-1.6.4/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/click/utils.meta.json` & `su6-1.6.4/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/collections/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/collections/abc.data.json` & `su6-1.6.4/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/collections/abc.meta.json` & `su6-1.6.4/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/futures/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/futures/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/futures/_base.data.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/futures/_base.meta.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/futures/process.data.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/futures/process.meta.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/futures/thread.data.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/concurrent/futures/thread.meta.json` & `su6-1.6.4/.mypy_cache/3.11/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/__init__.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1689928118'}*

```diff
@@ -36,15 +36,15 @@
         "abc",
         "typing"
     ],
     "hash": "490a0a73c5db609321b4c3ac826dc3c895ecb1befe7bdcaa39864ec90d182f5a",
     "id": "configuraptor",
     "ignore_all": true,
     "interface_hash": "a7a0819d3cf0d1a173f04a75c94215172efd007c1ab84e731c2d93c0fd9100ed",
-    "mtime": 1689592491,
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/cls.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/cls.data.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999998774064%*

 * *Differences: {"'names'": "{'TypedConfig': {'node': {'names': {'load': {'node': {'func': {'arg_kinds': {insert: "*

 * *            "[(1, 1)], delete: [0]}, 'type': {'arg_kinds': {insert: [(1, 1)], delete: [0]}, "*

 * *            "'arg_types': {1: {'.class': 'UnionType', 'items': ['builtins.str', 'pathlib.Path', "*

 * *            "OrderedDict([('.class', 'Instance'), ('args', ['builtins.str', "*

 * *            "OrderedDict([('.class', 'AnyType'), ('missing_import_name', None), ('source_any', "*

 * *            "None), ('type_of_any', 6)])]), ( […]*

```diff
@@ -408,15 +408,15 @@
                         "node": {
                             ".class": "Decorator",
                             "func": {
                                 ".class": "FuncDef",
                                 "abstract_status": 0,
                                 "arg_kinds": [
                                     0,
-                                    0,
+                                    1,
                                     1,
                                     1,
                                     1,
                                     1,
                                     1
                                 ],
                                 "arg_names": [
@@ -435,15 +435,15 @@
                                 ],
                                 "fullname": "configuraptor.cls.TypedConfig.load",
                                 "name": "load",
                                 "type": {
                                     ".class": "CallableType",
                                     "arg_kinds": [
                                         0,
-                                        0,
+                                        1,
                                         1,
                                         1,
                                         1,
                                         1,
                                         1
                                     ],
                                     "arg_names": [
@@ -471,17 +471,35 @@
                                                     "type_of_any": 2
                                                 },
                                                 "values": [],
                                                 "variance": 0
                                             }
                                         },
                                         {
-                                            ".class": "TypeAliasType",
-                                            "args": [],
-                                            "type_ref": "configuraptor.core.T_data"
+                                            ".class": "UnionType",
+                                            "items": [
+                                                "builtins.str",
+                                                "pathlib.Path",
+                                                {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "AnyType",
+                                                            "missing_import_name": null,
+                                                            "source_any": null,
+                                                            "type_of_any": 6
+                                                        }
+                                                    ],
+                                                    "type_ref": "builtins.dict"
+                                                },
+                                                {
+                                                    ".class": "NoneType"
+                                                }
+                                            ]
                                         },
                                         {
                                             ".class": "UnionType",
                                             "items": [
                                                 "builtins.str",
                                                 {
                                                     ".class": "NoneType"
@@ -569,15 +587,15 @@
                                 ],
                                 "fullname": "configuraptor.cls.TypedConfig.load",
                                 "name": "load",
                                 "type": {
                                     ".class": "CallableType",
                                     "arg_kinds": [
                                         0,
-                                        0,
+                                        1,
                                         1,
                                         1,
                                         1,
                                         1,
                                         1
                                     ],
                                     "arg_names": [
@@ -605,17 +623,35 @@
                                                     "type_of_any": 2
                                                 },
                                                 "values": [],
                                                 "variance": 0
                                             }
                                         },
                                         {
-                                            ".class": "TypeAliasType",
-                                            "args": [],
-                                            "type_ref": "configuraptor.core.T_data"
+                                            ".class": "UnionType",
+                                            "items": [
+                                                "builtins.str",
+                                                "pathlib.Path",
+                                                {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "AnyType",
+                                                            "missing_import_name": null,
+                                                            "source_any": null,
+                                                            "type_of_any": 6
+                                                        }
+                                                    ],
+                                                    "type_ref": "builtins.dict"
+                                                },
+                                                {
+                                                    ".class": "NoneType"
+                                                }
+                                            ]
                                         },
                                         {
                                             ".class": "UnionType",
                                             "items": [
                                                 "builtins.str",
                                                 {
                                                     ".class": "NoneType"
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/cls.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/dump.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7115277777777778%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 11), (1, 12), (3, 6), (4, 8), (11, 9)], delete: [4, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 10), (3, 10), (4, 10), (11, 10)], delete: [5, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'configuraptor.helpers'), (2, 'json'), (4, 'tomli_w'), (9, "*

 * *                   "'json.encoder'), (10, 'types')], delete: [10, 9, 8, 2, 0]}",*

 * * "'hash'": "'2b9a9164b8eacc5d1e19f1959ce8cb1596d2e788913ebe790bc0406cfd93b125'",*

 * * "'id'": "'configuraptor.dump'",*

 * * "'interface_hash'": "'46f0032b3d3b5500f2 […]*

```diff
@@ -1,53 +1,55 @@
 {
     "data_mtime": 1689594458,
     "dep_lines": [
-        6,
-        9,
-        10,
+        11,
+        12,
         5,
+        6,
+        8,
         1,
         1,
         1,
         1,
         1,
         1,
-        1
+        9
     ],
     "dep_prios": [
         5,
         5,
-        5,
-        5,
+        10,
+        10,
+        10,
         5,
         30,
         30,
         30,
         30,
         30,
-        30
+        10
     ],
     "dependencies": [
-        "collections.abc",
         "configuraptor.core",
-        "configuraptor.errors",
+        "configuraptor.helpers",
+        "json",
         "typing",
+        "tomli_w",
         "builtins",
         "_collections_abc",
         "_typeshed",
         "abc",
-        "os",
-        "pathlib",
-        "typing_extensions"
+        "json.encoder",
+        "types"
     ],
-    "hash": "0c664c0e1adce2951aa17fca1d4ecb2be8a728066cf6b20721b0ecf6ecf038dc",
-    "id": "configuraptor.cls",
+    "hash": "2b9a9164b8eacc5d1e19f1959ce8cb1596d2e788913ebe790bc0406cfd93b125",
+    "id": "configuraptor.dump",
     "ignore_all": true,
-    "interface_hash": "5004f35feafbf5aacd431795cc4228215ab223376cb70d073c501fa6a68389ca",
-    "mtime": 1689592491,
+    "interface_hash": "46f0032b3d3b5500f202f71ccec2f1a22251a875ddec3625cd5fd4605a21a6d6",
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -81,13 +83,15 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/cls.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/dump.py",
     "plugin_data": null,
-    "size": 5290,
-    "suppressed": [],
+    "size": 1783,
+    "suppressed": [
+        "yaml"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/core.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/core.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987828879381614%*

 * *Differences: {"'names'": "{'T_data': {'node': {'target': {'items': {insert: [(3, OrderedDict([('.class', "*

 * *            "'NoneType')]))]}}}}, 'T_init': {'node': {'line': 443}}, 'T_init_dict': {'node': "*

 * *            "{'line': 442}}, 'T_init_list': {'node': {'line': 441}}, 'Type': {'node': {'line': "*

 * *            "206}}, 'load_into': {'node': {'arg_kinds': {insert: [(1, 1)], delete: [0]}, 'type': "*

 * *            "{'arg_kinds': {insert: [(1, 1)], delete: [0]}, 'arg_types': {1: {'.class': "*

 * *            "'UnionType', 'items': [' […]*

```diff
@@ -135,28 +135,31 @@
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
                                     "type_of_any": 6
                                 }
                             ],
                             "type_ref": "builtins.dict"
+                        },
+                        {
+                            ".class": "NoneType"
                         }
                     ]
                 }
             }
         },
         "T_init": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "configuraptor.core.T_init",
-                "line": 439,
+                "line": 443,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         {
                             ".class": "TupleType",
@@ -207,15 +210,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "configuraptor.core.T_init_dict",
-                "line": 438,
+                "line": 442,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
@@ -233,15 +236,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "configuraptor.core.T_init_list",
-                "line": 437,
+                "line": 441,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "Instance",
                     "args": [
                         {
                             ".class": "AnyType",
@@ -278,15 +281,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "configuraptor.core.Type",
-                "line": 202,
+                "line": 206,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "TypeType",
                     "item": {
                         ".class": "AnyType",
                         "missing_import_name": null,
@@ -1790,14 +1793,21 @@
                             "values": [],
                             "variance": 0
                         }
                     ]
                 }
             }
         },
+        "find_pyproject_toml": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "configuraptor.helpers.find_pyproject_toml",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "instance_of_custom_class": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
@@ -2139,15 +2149,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
                     0,
-                    0,
+                    1,
                     1,
                     1,
                     1,
                     1,
                     1
                 ],
                 "arg_names": [
@@ -2163,15 +2173,15 @@
                 "flags": [],
                 "fullname": "configuraptor.core.load_into",
                 "name": "load_into",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0,
-                        0,
+                        1,
                         1,
                         1,
                         1,
                         1,
                         1
                     ],
                     "arg_names": [
@@ -2194,17 +2204,35 @@
                                 "namespace": "",
                                 "upper_bound": "builtins.object",
                                 "values": [],
                                 "variance": 0
                             }
                         },
                         {
-                            ".class": "TypeAliasType",
-                            "args": [],
-                            "type_ref": "configuraptor.core.T_data"
+                            ".class": "UnionType",
+                            "items": [
+                                "builtins.str",
+                                "pathlib.Path",
+                                {
+                                    ".class": "Instance",
+                                    "args": [
+                                        "builtins.str",
+                                        {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 6
+                                        }
+                                    ],
+                                    "type_ref": "builtins.dict"
+                                },
+                                {
+                                    ".class": "NoneType"
+                                }
+                            ]
                         },
                         {
                             ".class": "UnionType",
                             "items": [
                                 "builtins.str",
                                 {
                                     ".class": "NoneType"
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/core.meta.json` & `su6-1.6.4/.mypy_cache/3.11/su6/core.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6488171702789642%*

 * *Differences: {"'data_mtime'": '1689928121',*

 * * "'dep_lines'": '{insert: [(0, 20), (1, 26), (2, 4), (10, 12), (11, 15), (12, 17), (13, 18), (14, '*

 * *                '23), (15, 1), (16, 1), (34, 16), (35, 16), (36, 22), (37, 16)], delete: [13, 12, '*

 * *                '4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 25), (2, 10), (3, 10), (12, 10), (13, 10), (14, 5), (16, 30), (17, '*

 * *                '30), (34, 10), (35, 20), (36, 5), (37, 5)], delete: [13, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'su6.plugins'), (2, 'en […]*

```diff
@@ -1,24 +1,27 @@
 {
-    "data_mtime": 1689594458,
+    "data_mtime": 1689928121,
     "dep_lines": [
-        16,
-        17,
-        22,
-        23,
-        24,
+        20,
+        26,
+        4,
         5,
         6,
         7,
         8,
         9,
         10,
         11,
-        13,
-        16,
+        12,
+        15,
+        17,
+        18,
+        23,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
@@ -27,31 +30,36 @@
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1
+        1,
+        16,
+        16,
+        22,
+        16
     ],
     "dep_prios": [
-        10,
-        5,
-        5,
-        5,
         5,
+        25,
+        10,
+        10,
         10,
         10,
         10,
         10,
         10,
         5,
         5,
         5,
-        20,
+        10,
+        10,
+        5,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
@@ -60,54 +68,63 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30
+        30,
+        30,
+        30,
+        10,
+        20,
+        5,
+        5
     ],
     "dependencies": [
-        "configuraptor.loaders",
-        "configuraptor.errors",
         "configuraptor.helpers",
-        "configuraptor.postpone",
-        "configuraptor.type_converters",
-        "dataclasses",
-        "math",
+        "su6.plugins",
+        "enum",
+        "functools",
+        "inspect",
+        "json",
+        "operator",
+        "sys",
         "types",
         "typing",
-        "warnings",
-        "collections",
-        "pathlib",
-        "typeguard",
+        "dataclasses",
         "configuraptor",
+        "tomli",
+        "typer",
+        "rich",
         "builtins",
         "_collections_abc",
+        "_operator",
         "_typeshed",
         "abc",
         "array",
+        "click",
+        "click.exceptions",
+        "configuraptor.cls",
+        "configuraptor.core",
         "configuraptor.singleton",
         "ctypes",
-        "enum",
         "io",
+        "json.encoder",
         "mmap",
         "os",
+        "pathlib",
         "pickle",
-        "typeguard._config",
-        "typeguard._exceptions",
-        "typeguard._functions",
-        "typeguard._memo",
         "typing_extensions"
     ],
-    "hash": "78e72b3de2b2e63da9ca38e8928122a257043c456f28d6a9a228315e5167ad3f",
-    "id": "configuraptor.core",
-    "ignore_all": true,
-    "interface_hash": "28458702db1775f5fcb20c688c5180d473698b49b0aa197c471497931a4410f6",
-    "mtime": 1689592491,
+    "hash": "06870682544b1b1d2a1e36d94a19585fa1a9c952efc9813ecd1aecfc8aa003ce",
+    "id": "su6.core",
+    "ignore_all": false,
+    "interface_hash": "2b11007dcd3f336dd0560f93fd19a3026456581cf4f0ae7c0fb09d0052fcf4c7",
+    "mtime": 1689927449,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -141,13 +158,18 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/core.py",
+    "path": "src/su6/core.py",
     "plugin_data": null,
-    "size": 19056,
-    "suppressed": [],
+    "size": 18511,
+    "suppressed": [
+        "plumbum.commands.processes",
+        "plumbum.commands",
+        "plumbum.machines",
+        "plumbum"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/dump.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/dump.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/dump.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/themes.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6672649572649573%*

 * *Differences: {"'data_mtime'": '1686754986',*

 * * "'dep_lines'": '{insert: [(1, 2)], delete: [11, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [11, 7, 6, 4, 3, 2]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.default_styles'), (1, 'rich.theme'), (4, 'rich.style'), "*

 * *                   "(5, 'typing')], delete: [10, 9, 7, 6, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'d318132e8cdf69b79b62d709b43742e50917e4855411abe2a83509261e185459'",*

 * * "'id'": "'rich.themes'",*

 * * "'interface_hash'": "'c7645ea79e02f663c3e35494c3e38d3edbfed0d874cd39434350c8e598 […]*

```diff
@@ -1,55 +1,38 @@
 {
-    "data_mtime": 1689594458,
+    "data_mtime": 1686754986,
     "dep_lines": [
-        11,
-        12,
-        5,
-        6,
-        8,
-        1,
         1,
+        2,
         1,
         1,
         1,
-        1,
-        9
+        1
     ],
     "dep_prios": [
         5,
         5,
-        10,
-        10,
-        10,
         5,
         30,
         30,
-        30,
-        30,
-        30,
-        10
+        30
     ],
     "dependencies": [
-        "configuraptor.core",
-        "configuraptor.helpers",
-        "json",
-        "typing",
-        "tomli_w",
+        "rich.default_styles",
+        "rich.theme",
         "builtins",
-        "_collections_abc",
-        "_typeshed",
         "abc",
-        "json.encoder",
-        "types"
+        "rich.style",
+        "typing"
     ],
-    "hash": "2b9a9164b8eacc5d1e19f1959ce8cb1596d2e788913ebe790bc0406cfd93b125",
-    "id": "configuraptor.dump",
+    "hash": "d318132e8cdf69b79b62d709b43742e50917e4855411abe2a83509261e185459",
+    "id": "rich.themes",
     "ignore_all": true,
-    "interface_hash": "46f0032b3d3b5500f202f71ccec2f1a22251a875ddec3625cd5fd4605a21a6d6",
-    "mtime": 1689592491,
+    "interface_hash": "c7645ea79e02f663c3e35494c3e38d3edbfed0d874cd39434350c8e598165d3a",
+    "mtime": 1686754199,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -83,15 +66,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/dump.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/themes.py",
     "plugin_data": null,
-    "size": 1783,
-    "suppressed": [
-        "yaml"
-    ],
+    "size": 102,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/errors.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/errors.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/errors.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1689928118'}*

```diff
@@ -30,15 +30,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "3358dc161f119f40b23b74e39a8e4485ea323d8287ffe094f6fd04833f5e5a5a",
     "id": "configuraptor.errors",
     "ignore_all": true,
     "interface_hash": "541a2960b83a952f08fe7fa56590169f7592bdccbec7f6a790ca6e23a48dad71",
-    "mtime": 1689592491,
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/helpers.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/helpers.data.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.974025974025974%*

 * *Differences: {"'names'": "{'black': OrderedDict([('.class', 'SymbolTableNode'), ('cross_ref', 'black'), "*

 * *            "('kind', 'Gdef'), ('module_hidden', True), ('module_public', False)]), "*

 * *            "'find_pyproject_toml': OrderedDict([('.class', 'SymbolTableNode'), ('kind', 'Gdef'), "*

 * *            "('node', OrderedDict([('.class', 'FuncDef'), ('abstract_status', 0), ('arg_kinds', "*

 * *            "[]), ('arg_names', []), ('dataclass_transform_spec', None), ('flags', []), "*

 * *            "('fullname', 'configuraptor.help […]*

```diff
@@ -79,14 +79,21 @@
                     "is_ready"
                 ],
                 "fullname": "configuraptor.helpers.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
+        "black": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "black",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "camel_to_snake": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
@@ -121,11 +128,66 @@
                     "name": "camel_to_snake",
                     "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
+        },
+        "find_pyproject_toml": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [],
+                "arg_names": [],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "configuraptor.helpers.find_pyproject_toml",
+                "name": "find_pyproject_toml",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [],
+                    "arg_names": [],
+                    "arg_types": [],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "find_pyproject_toml",
+                    "ret_type": {
+                        ".class": "UnionType",
+                        "items": [
+                            "builtins.str",
+                            {
+                                ".class": "NoneType"
+                            }
+                        ]
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "os": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "os",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "typing": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
         }
     },
     "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/helpers.py"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/helpers.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/__init__.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7416666666666667%*

 * *Differences: {"'data_mtime'": '1686754985',*

 * * "'dep_lines'": '{insert: [(0, 5)]}',*

 * * "'dep_prios'": '{insert: [(0, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'markdown_it.main')]}",*

 * * "'hash'": "'f6fdef083ed7409ba37192d4d85d784fc3bcf0924ef77ad9694a0abbb728707f'",*

 * * "'id'": "'markdown_it'",*

 * * "'interface_hash'": "'372ee22c04add3a2da64dbf94c774114609dbe8c4cb316069d563032a161d10f'",*

 * * "'mtime'": '1686754199',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/__init__.py'",*

 * * "'size'": '11 […]*

```diff
@@ -1,29 +1,32 @@
 {
-    "data_mtime": 1686754983,
+    "data_mtime": 1686754985,
     "dep_lines": [
+        5,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
         30,
         30
     ],
     "dependencies": [
+        "markdown_it.main",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "32ed36840fbe0e18b032d8f86ca33c819ea7e7d9d03e44b97f6c3a7dfd5133e5",
-    "id": "configuraptor.helpers",
+    "hash": "f6fdef083ed7409ba37192d4d85d784fc3bcf0924ef77ad9694a0abbb728707f",
+    "id": "markdown_it",
     "ignore_all": true,
-    "interface_hash": "fa6a613a7e56d42069a3559eed13704a7e16ad1e811c5e6ce4b0e40d2372f0fc",
-    "mtime": 1689592491,
+    "interface_hash": "372ee22c04add3a2da64dbf94c774114609dbe8c4cb316069d563032a161d10f",
+    "mtime": 1686754199,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/helpers.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/__init__.py",
     "plugin_data": null,
-    "size": 344,
+    "size": 113,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/postpone.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/postpone.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/postpone.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/postpone.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1689928118'}*

```diff
@@ -24,15 +24,15 @@
         "builtins",
         "abc"
     ],
     "hash": "195447d25e52ae78402e55c721433bad75cc34f309fb09e48b882ec0f38d1259",
     "id": "configuraptor.postpone",
     "ignore_all": true,
     "interface_hash": "4379518bff44bb910275ee367d4c75b8a8a11ea64203fd6437e08af684feadfb",
-    "mtime": 1689592491,
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/singleton.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/singleton.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/singleton.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/singleton.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1689928118'}*

```diff
@@ -15,15 +15,15 @@
         "builtins",
         "abc"
     ],
     "hash": "bcc3654762a9d40463892181086c999397aaf1934f2d8eb3f797a369e022c5c1",
     "id": "configuraptor.singleton",
     "ignore_all": true,
     "interface_hash": "1e9b57b328d77b36afe7c59a728bb0d5daba31fa44c2d512e88dc79021df5182",
-    "mtime": 1689592491,
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/type_converters.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/type_converters.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/type_converters.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/_utils.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7168055555555556%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(1, 13), (2, 1), (3, 3), (5, 11), (6, 1), (7, 1), (8, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (4, 5), (7, 30), (8, 30), (9, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'tomlkit._compat'), (2, '__future__'), "*

 * *                   "(3, 're'), (4, 'datetime'), (7, '_collections_abc'), (8, '_typeshed'), (14, "*

 * *                   "'typing_extensions')], delete: [0]}",*

 * * "'hash'": "'7d7d67edba028bbfdb05505e99acb09347b2 […]*

```diff
@@ -1,44 +1,65 @@
 {
-    "data_mtime": 1689594458,
+    "data_mtime": 1686754984,
     "dep_lines": [
         5,
+        13,
+        1,
+        3,
         6,
+        11,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
+        5,
+        5,
         10,
         5,
         5,
+        5,
+        30,
+        30,
+        30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "types",
+        "collections.abc",
+        "tomlkit._compat",
+        "__future__",
+        "re",
+        "datetime",
         "typing",
         "builtins",
+        "_collections_abc",
+        "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
-        "pickle"
+        "pickle",
+        "typing_extensions"
     ],
-    "hash": "bebe5e7d07b9ce305e6f0b69cb68e5213f622350d86ba2fdbdf7f67717d7bbbe",
-    "id": "configuraptor.type_converters",
+    "hash": "7d7d67edba028bbfdb05505e99acb09347b2c6a8536276563e10991c980166ff",
+    "id": "tomlkit._utils",
     "ignore_all": true,
-    "interface_hash": "dbcaaec299ca916f5edb02ba65d22b75b29d702a46b15230e10f98f055da7ae1",
-    "mtime": 1689592491,
+    "interface_hash": "45431f8929f73a2c5625b9f707ed70315bad82515082caf54c17d64631be18a5",
+    "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +93,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/type_converters.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/_utils.py",
     "plugin_data": null,
-    "size": 2006,
+    "size": 4021,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1689928118'}*

```diff
@@ -27,15 +27,15 @@
         "pathlib",
         "typing"
     ],
     "hash": "7736c31fb66b001201caf25e4456bd56e1a672b4399b03c2b86b4836f9240501",
     "id": "configuraptor.loaders",
     "ignore_all": true,
     "interface_hash": "f5ef6079b340aee3666d2e167c7e4c593a352eeb03cb496f4855fc8bca9ea07c",
-    "mtime": 1689592491,
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/_types.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/_types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1689928118'}*

```diff
@@ -18,15 +18,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "428a5bf57416d66fc0b2d023a49c5b0a311caa051d92180a885653dc4668e8d2",
     "id": "configuraptor.loaders._types",
     "ignore_all": true,
     "interface_hash": "ff8bf54ace6de15cec9f2eb2c19a18138007d71a654544edb632d48f8f96a653",
-    "mtime": 1689592491,
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1689928118'}*

```diff
@@ -59,15 +59,15 @@
         "os",
         "typing_extensions"
     ],
     "hash": "01015cacec184ac0402b22702f8f58facb68d63a5f042a020a8cc4fe451df6cd",
     "id": "configuraptor.loaders.loaders_shared",
     "ignore_all": true,
     "interface_hash": "479ec02b20d7ed503f1df829962becf8b46750d2d1a1c55435d094f50c996299",
-    "mtime": 1689592491,
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/register.data.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/register.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/configuraptor/loaders/register.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/loaders/register.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1689928118'}*

```diff
@@ -45,15 +45,15 @@
         "types",
         "typing_extensions"
     ],
     "hash": "02cad53db20c5a116a8c9bfc860cb6fceaa7aef9f2b9c93dd220131b49ffe926",
     "id": "configuraptor.loaders.register",
     "ignore_all": true,
     "interface_hash": "3fede2b0bbcd1fd0d76b294b11aa7c2f27bef782516171b291705972665bdad7",
-    "mtime": 1689592491,
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/ctypes/wintypes.data.json` & `su6-1.6.4/.mypy_cache/3.11/ctypes/wintypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/ctypes/wintypes.meta.json` & `su6-1.6.4/.mypy_cache/3.11/ctypes/wintypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/ipython.data.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/ipython.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/ipython.meta.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/ipython.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/main.data.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/main.meta.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/parser.data.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/parser.meta.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/variables.data.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/variables.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/dotenv/variables.meta.json` & `su6-1.6.4/.mypy_cache/3.11/dotenv/variables.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/charset.data.json` & `su6-1.6.4/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/charset.meta.json` & `su6-1.6.4/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-1.6.4/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-1.6.4/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/errors.data.json` & `su6-1.6.4/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/errors.meta.json` & `su6-1.6.4/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/header.data.json` & `su6-1.6.4/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/header.meta.json` & `su6-1.6.4/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/message.data.json` & `su6-1.6.4/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/message.meta.json` & `su6-1.6.4/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/policy.data.json` & `su6-1.6.4/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/email/policy.meta.json` & `su6-1.6.4/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/html/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/html/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/html/entities.data.json` & `su6-1.6.4/.mypy_cache/3.11/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/html/entities.meta.json` & `su6-1.6.4/.mypy_cache/3.11/html/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/abc.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/util.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/util.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_adapters.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_adapters.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_collections.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_collections.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_collections.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_compat.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_compat.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_functools.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_functools.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_itertools.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_meta.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_meta.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_text.data.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_text.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/importlib_metadata/_text.meta.json` & `su6-1.6.4/.mypy_cache/3.11/importlib_metadata/_text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/json/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/json/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/json/decoder.data.json` & `su6-1.6.4/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/json/decoder.meta.json` & `su6-1.6.4/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/json/encoder.data.json` & `su6-1.6.4/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/json/encoder.meta.json` & `su6-1.6.4/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/logging/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/logging/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/errors.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.775%*

 * *Differences: {"'data_mtime'": '1686754983',*

 * * "'dep_lines'": '{delete: [0]}',*

 * * "'dep_prios'": '{delete: [0]}',*

 * * "'dependencies'": '{delete: [0]}',*

 * * "'hash'": "'e693f729ce5de1027f734285b31adfca18e23d57bb275ccea9215b140cdc57e6'",*

 * * "'id'": "'rich.errors'",*

 * * "'interface_hash'": "'534ee3082dbc4ad481e7299060952717c174935b937136d76df876eaf8407f10'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/errors.py'",*

 * * "'size'": '642'}*

```diff
@@ -1,31 +1,28 @@
 {
-    "data_mtime": 1686754985,
+    "data_mtime": 1686754983,
     "dep_lines": [
-        5,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "markdown_it.main",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "f6fdef083ed7409ba37192d4d85d784fc3bcf0924ef77ad9694a0abbb728707f",
-    "id": "markdown_it",
+    "hash": "e693f729ce5de1027f734285b31adfca18e23d57bb275ccea9215b140cdc57e6",
+    "id": "rich.errors",
     "ignore_all": true,
-    "interface_hash": "372ee22c04add3a2da64dbf94c774114609dbe8c4cb316069d563032a161d10f",
+    "interface_hash": "534ee3082dbc4ad481e7299060952717c174935b937136d76df876eaf8407f10",
     "mtime": 1686754199,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -60,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/__init__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/errors.py",
     "plugin_data": null,
-    "size": 113,
+    "size": 642,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/_compat.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/_compat.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/_punycode.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/_punycode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/_punycode.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/_punycode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/main.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/main.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_block.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_block.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_core.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_core.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_inline.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/parser_inline.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/parser_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/renderer.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/renderer.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/ruler.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/ruler.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/ruler.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/ruler.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/token.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/token.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/utils.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/utils.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/entities.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/entities.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/html_re.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/html_re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/html_re.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/html_re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/utils.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/common/utils.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/common/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/default.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/default.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/default.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/default.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/zero.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/zero.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/presets/zero.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/presets/zero.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/code.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/code.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/list.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/list.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/table.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/block.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json` & `su6-1.6.4/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_decode.data.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_decode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_decode.meta.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_decode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_encode.data.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_encode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_encode.meta.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_encode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_format.data.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_format.meta.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_parse.data.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_parse.meta.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_url.data.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/mdurl/_url.meta.json` & `su6-1.6.4/.mypy_cache/3.11/mdurl/_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/connection.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/connection.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/context.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/context.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/managers.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/managers.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/pool.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/pool.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_fork.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/process.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/process.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/queues.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/queues.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/reduction.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/reduction.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/shared_memory.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/spawn.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/spawn.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/synchronize.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/synchronize.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/util.data.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/multiprocessing/util.meta.json` & `su6-1.6.4/.mypy_cache/3.11/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/os/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/os/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/os/path.data.json` & `su6-1.6.4/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/os/path.meta.json` & `su6-1.6.4/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/_elffile.data.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/_elffile.meta.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/_manylinux.data.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/_manylinux.meta.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/_musllinux.data.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/_musllinux.meta.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/_structures.data.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/_structures.meta.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/specifiers.data.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/specifiers.meta.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/tags.data.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/tags.meta.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/utils.data.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/utils.meta.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/version.data.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/packaging/version.meta.json` & `su6-1.6.4/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/_meta.data.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/_meta.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/gitignore.data.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/gitignore.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/gitignore.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/gitignore.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/pathspec.data.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/pathspec.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/pathspec.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/pathspec.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/pattern.data.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/pattern.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/pattern.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/pattern.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/util.data.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/util.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/patterns/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/patterns/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json` & `su6-1.6.4/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/android.data.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/android.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/android.meta.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/android.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/api.data.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/api.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/api.meta.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/unix.data.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/unix.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/unix.meta.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/unix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/version.data.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/platformdirs/version.meta.json` & `su6-1.6.4/.mypy_cache/3.11/platformdirs/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/__main__.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/__main__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/__main__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/__main__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_cell_widths.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_cell_widths.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_cell_widths.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_cell_widths.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_emoji_codes.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_emoji_codes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_emoji_codes.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_emoji_codes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_emoji_replace.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_emoji_replace.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_emoji_replace.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_emoji_replace.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_export_format.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_export_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_export_format.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_export_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_extension.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_extension.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_extension.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_extension.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_fileno.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_fileno.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_fileno.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_fileno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_inspect.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_inspect.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_log_render.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_log_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_log_render.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_log_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_loop.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_loop.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_loop.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_loop.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_null_file.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_null_file.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_null_file.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_null_file.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_palettes.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_palettes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_palettes.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_palettes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_pick.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_pick.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_pick.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_pick.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_ratio.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_ratio.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_ratio.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_ratio.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_spinners.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_spinners.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_spinners.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_spinners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_stack.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_stack.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_stack.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_stack.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_timer.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_timer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_timer.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_timer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_win32_console.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_win32_console.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_win32_console.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_win32_console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_windows.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_windows.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_windows.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_windows.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_windows_renderer.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_windows_renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_windows_renderer.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_windows_renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_wrap.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_wrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/_wrap.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/_wrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/abc.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/abc.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/align.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/align.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/align.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/align.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/ansi.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/ansi.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/ansi.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/box.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/box.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/box.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/box.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/cells.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/cells.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/cells.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/cells.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/color.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/color.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/color.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/color.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/color_triplet.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/color_triplet.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/color_triplet.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/color_triplet.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/columns.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/columns.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/columns.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/columns.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/console.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/console.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/console.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/constrain.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/constrain.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/constrain.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/constrain.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/containers.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/containers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/containers.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/containers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/control.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/control.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/control.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/control.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/default_styles.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/default_styles.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/default_styles.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/default_styles.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/emoji.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/emoji.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/emoji.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/emoji.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/errors.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/errors.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7416666666666667%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(0, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'tomlkit.api')]}",*

 * * "'hash'": "'feee93b1ddf737d85ff86840869aa3eadd2ca0d9d33b92cfdae31d5b05fdc46d'",*

 * * "'id'": "'tomlkit'",*

 * * "'interface_hash'": "'931319b0d54715d34e26f52d066c2f348b156844b23e01c31fc62e15115262c7'",*

 * * "'mtime'": '1686754196',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/__init__.py'",*

 * * "'size'": '1148'}*

```diff
@@ -1,29 +1,32 @@
 {
-    "data_mtime": 1686754983,
+    "data_mtime": 1686754984,
     "dep_lines": [
         1,
         1,
+        1,
         1
     ],
     "dep_prios": [
         5,
+        5,
         30,
         30
     ],
     "dependencies": [
+        "tomlkit.api",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "e693f729ce5de1027f734285b31adfca18e23d57bb275ccea9215b140cdc57e6",
-    "id": "rich.errors",
+    "hash": "feee93b1ddf737d85ff86840869aa3eadd2ca0d9d33b92cfdae31d5b05fdc46d",
+    "id": "tomlkit",
     "ignore_all": true,
-    "interface_hash": "534ee3082dbc4ad481e7299060952717c174935b937136d76df876eaf8407f10",
-    "mtime": 1686754199,
+    "interface_hash": "931319b0d54715d34e26f52d066c2f348b156844b23e01c31fc62e15115262c7",
+    "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/errors.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/__init__.py",
     "plugin_data": null,
-    "size": 642,
+    "size": 1148,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/file_proxy.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/file_proxy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/file_proxy.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/file_proxy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/highlighter.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/highlighter.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/highlighter.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/highlighter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/json.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/json.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/json.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/json.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/jupyter.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/jupyter.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/jupyter.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/jupyter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/live.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/live.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/live.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/live.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/live_render.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/live_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/live_render.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/live_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/markdown.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/markdown.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/markdown.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/markdown.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/markup.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/markup.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/markup.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/markup.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/measure.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/measure.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/measure.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/measure.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/padding.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/padding.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/padding.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/padding.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/pager.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/pager.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/pager.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/pager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/palette.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/palette.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/palette.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/palette.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/panel.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/panel.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/panel.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/panel.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/pretty.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/pretty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/pretty.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/pretty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/protocol.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/protocol.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/protocol.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/protocol.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/region.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/region.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/region.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/region.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/repr.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/repr.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/repr.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/repr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/rule.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/rule.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/rule.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/rule.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/scope.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/scope.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/scope.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/screen.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/screen.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/screen.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/screen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/segment.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/segment.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/segment.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/segment.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/spinner.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/spinner.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/spinner.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/spinner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/status.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/status.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/status.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/status.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/style.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/style.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/style.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/style.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/styled.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/styled.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/styled.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/styled.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/syntax.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/syntax.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/syntax.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/syntax.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/table.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/table.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/terminal_theme.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/terminal_theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/terminal_theme.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/terminal_theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/text.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/text.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/theme.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/theme.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/themes.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/themes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/themes.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomli_w/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7174603174603175%*

 * *Differences: {"'data_mtime'": '1687249414',*

 * * "'dep_lines'": '{insert: [(0, 4)], delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [3, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'tomli_w._writer')], delete: [4, 1, 0]}",*

 * * "'hash'": "'c3cdef9f865651a478788c5258258e5643d8f2a18943ebae5699c8b5dce69245'",*

 * * "'id'": "'tomli_w'",*

 * * "'interface_hash'": "'ed818460546f71f4107d04c1605d8fbbb0fe158c708f3dac618afd4533fadfd2'",*

 * * "'mtime'": '1686754196',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomli_w/__ […]*

```diff
@@ -1,38 +1,32 @@
 {
-    "data_mtime": 1686754986,
+    "data_mtime": 1687249414,
     "dep_lines": [
-        1,
-        2,
-        1,
+        4,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "rich.default_styles",
-        "rich.theme",
+        "tomli_w._writer",
         "builtins",
         "abc",
-        "rich.style",
         "typing"
     ],
-    "hash": "d318132e8cdf69b79b62d709b43742e50917e4855411abe2a83509261e185459",
-    "id": "rich.themes",
+    "hash": "c3cdef9f865651a478788c5258258e5643d8f2a18943ebae5699c8b5dce69245",
+    "id": "tomli_w",
     "ignore_all": true,
-    "interface_hash": "c7645ea79e02f663c3e35494c3e38d3edbfed0d874cd39434350c8e598165d3a",
-    "mtime": 1686754199,
+    "interface_hash": "ed818460546f71f4107d04c1605d8fbbb0fe158c708f3dac618afd4533fadfd2",
+    "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/themes.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomli_w/__init__.py",
     "plugin_data": null,
-    "size": 102,
+    "size": 157,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/traceback.data.json` & `su6-1.6.4/.mypy_cache/3.11/rich/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/rich/traceback.meta.json` & `su6-1.6.4/.mypy_cache/3.11/rich/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/__about__.data.json` & `su6-1.6.4/.mypy_cache/3.11/su6/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/__about__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/cls.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.657070707070707%*

 * *Differences: {"'data_mtime'": '1689928121',*

 * * "'dep_lines'": '{insert: [(0, 6), (1, 9), (2, 10), (3, 5), (4, 1), (5, 1), (6, 1), (7, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (3, 5), (5, 30), (6, 30), (7, 30), (8, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'configuraptor.core'), (2, "*

 * *                   "'configuraptor.errors'), (3, 'typing'), (5, '_collections_abc'), (6, "*

 * *                   "'_typeshed'), (8, 'os'), (9, 'pathlib'), (10, 'typing_extensions')], delete: "*

 * *            […]*

```diff
@@ -1,29 +1,53 @@
 {
-    "data_mtime": 1686754983,
+    "data_mtime": 1689928121,
     "dep_lines": [
+        6,
+        9,
+        10,
+        5,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        5,
+        5,
+        5,
+        30,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
+        "collections.abc",
+        "configuraptor.core",
+        "configuraptor.errors",
+        "typing",
         "builtins",
+        "_collections_abc",
+        "_typeshed",
         "abc",
-        "typing"
+        "os",
+        "pathlib",
+        "typing_extensions"
     ],
-    "hash": "7d448d27f35f88711aae137bf1d751b28d1ffa63610ee527430d206aebb854de",
-    "id": "su6.__about__",
-    "ignore_all": false,
-    "interface_hash": "f585c505c8d50598658e61be6359ebe7fcc6381e8be269711f79d29222dffbf9",
-    "mtime": 1689601040,
+    "hash": "418b3333ccf469977835b048dc2f01169bc4b722676f59d5042ed6940f8c0c9a",
+    "id": "configuraptor.cls",
+    "ignore_all": true,
+    "interface_hash": "fda25e417987a026fe51a8913707041a054869eca047a1803bd2398ae98cc0cc",
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +81,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/su6/__about__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/cls.py",
     "plugin_data": null,
-    "size": 206,
+    "size": 5297,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/su6/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/su6/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/cli.data.json` & `su6-1.6.4/.mypy_cache/3.11/su6/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/cli.meta.json` & `su6-1.6.4/.mypy_cache/3.11/su6/cli.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/core.data.json` & `su6-1.6.4/.mypy_cache/3.11/su6/core.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975107106052649%*

 * *Differences: {"'names'": "{'ApplicationState': {'node': {'metadata': {'dataclass': {'attributes': {0: {'line': "*

 * *            "483}, 1: {'line': 484}, 2: {'line': 485}, 3: {'line': 486}}}}}}, 'Config': {'node': "*

 * *            "{'metadata': {'dataclass': {'attributes': {0: {'line': 298}, 1: {'line': 299}, 2: "*

 * *            "{'line': 300}, 3: {'line': 301}, 4: {'line': 302}, 5: {'line': 303}, 6: {'line': "*

 * *            "306}, 7: {'line': 307}}}}}}, 'MaybeConfig': {'node': {'line': 358}}, 'T_Command': "*

 * *            "{'node': { […]*

```diff
@@ -110,39 +110,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 491,
+                                "line": 483,
                                 "name": "verbosity",
                                 "type": "su6.core.Verbosity"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 492,
+                                "line": 484,
                                 "name": "output_format",
                                 "type": "su6.core.Format"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 493,
+                                "line": 485,
                                 "name": "config_file",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.str",
                                         {
                                             ".class": "NoneType"
@@ -154,15 +154,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 494,
+                                "line": 486,
                                 "name": "config",
                                 "type": {
                                     ".class": "TypeAliasType",
                                     "args": [],
                                     "type_ref": "su6.core.MaybeConfig"
                                 }
                             }
@@ -911,39 +911,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 299,
+                                "line": 298,
                                 "name": "directory",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 300,
+                                "line": 299,
                                 "name": "pyproject",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 301,
+                                "line": 300,
                                 "name": "include",
                                 "type": {
                                     ".class": "Instance",
                                     "args": [
                                         "builtins.str"
                                     ],
                                     "type_ref": "builtins.list"
@@ -953,15 +953,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 302,
+                                "line": 301,
                                 "name": "exclude",
                                 "type": {
                                     ".class": "Instance",
                                     "args": [
                                         "builtins.str"
                                     ],
                                     "type_ref": "builtins.list"
@@ -971,39 +971,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 303,
+                                "line": 302,
                                 "name": "stop_after_first_failure",
                                 "type": "builtins.bool"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 304,
+                                "line": 303,
                                 "name": "json_indent",
                                 "type": "builtins.int"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 307,
+                                "line": 306,
                                 "name": "coverage",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.float",
                                         {
                                             ".class": "NoneType"
@@ -1015,15 +1015,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 308,
+                                "line": 307,
                                 "name": "badge",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.bool",
                                         "builtins.str"
                                     ]
@@ -2182,15 +2182,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.MaybeConfig",
-                "line": 359,
+                "line": 358,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "su6.core.Config",
                         {
@@ -2301,15 +2301,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.T_Command",
-                "line": 43,
+                "line": 42,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         2,
                         4
@@ -2354,15 +2354,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.T_Command_Return",
-                "line": 40,
+                "line": 39,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "builtins.bool",
                         "builtins.int",
@@ -2377,15 +2377,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.T_Inner_Wrapper",
-                "line": 45,
+                "line": 44,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         2,
                         4
@@ -2434,15 +2434,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.T_Outer_Wrapper",
-                "line": 48,
+                "line": 47,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0
                     ],
@@ -2478,15 +2478,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.T_typelike",
-                "line": 361,
+                "line": 360,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "builtins.type",
                         "types.UnionType",
@@ -3143,15 +3143,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.Verbosity_Comparable",
-                "line": 243,
+                "line": 242,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "su6.core.Verbosity",
                         "builtins.str",
@@ -3320,21 +3320,14 @@
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "black": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "black",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
         "configuraptor": {
             ".class": "SymbolTableNode",
             "cross_ref": "configuraptor",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
@@ -3484,52 +3477,18 @@
             "cross_ref": "dataclasses.field",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
         "find_pyproject_toml": {
             ".class": "SymbolTableNode",
+            "cross_ref": "configuraptor.helpers.find_pyproject_toml",
             "kind": "Gdef",
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [],
-                "arg_names": [],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "su6.core.find_pyproject_toml",
-                "name": "find_pyproject_toml",
-                "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [],
-                    "arg_names": [],
-                    "arg_types": [],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "find_pyproject_toml",
-                    "ret_type": {
-                        ".class": "UnionType",
-                        "items": [
-                            "builtins.str",
-                            {
-                                ".class": "NoneType"
-                            }
-                        ]
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
+            "module_hidden": true,
+            "module_public": false
         },
         "functools": {
             ".class": "SymbolTableNode",
             "cross_ref": "functools",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
@@ -3795,21 +3754,14 @@
         "operator": {
             ".class": "SymbolTableNode",
             "cross_ref": "operator",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "os": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "os",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
         "pb": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false,
             "node": {
                 ".class": "Var",
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/core.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomli/_parser.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6312427409988385%*

 * *Differences: {"'data_mtime'": '1687249414',*

 * * "'dep_lines'": '{insert: [(1, 12), (2, 20), (3, 5)], delete: [38, 37, 36, 35, 24, 23, 22, 21, 20, '*

 * *                '19, 18, 17, 16, 15, 14, 13, 12, 11, 10, 9, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 5), (7, 5)], delete: [38, 37, 36, 35, 25, 24, 23, 22, 21, 20, 19, '*

 * *                '18, 14, 12, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'tomli._re'), (2, 'tomli._types'), (3, "*

 * *                   "'__future__'), (4, 'st […]*

```diff
@@ -1,133 +1,71 @@
 {
-    "data_mtime": 1689600612,
+    "data_mtime": 1687249414,
     "dep_lines": [
-        16,
-        27,
-        4,
-        5,
-        6,
         7,
+        12,
+        20,
+        5,
         8,
         9,
         10,
-        11,
-        12,
-        13,
-        16,
-        17,
-        19,
-        20,
-        24,
-        1,
-        1,
-        1,
-        1,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
-        1,
-        1,
-        1,
-        18,
-        18,
-        23,
-        18
+        1
     ],
     "dep_prios": [
-        10,
-        25,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
         5,
         5,
-        20,
         5,
-        10,
+        5,
         10,
         5,
         5,
+        5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        10,
-        20,
-        5,
-        5
+        30
     ],
     "dependencies": [
-        "black.files",
-        "su6.plugins",
-        "enum",
-        "functools",
-        "inspect",
-        "json",
-        "operator",
-        "os",
-        "sys",
+        "collections.abc",
+        "tomli._re",
+        "tomli._types",
+        "__future__",
+        "string",
         "types",
         "typing",
-        "dataclasses",
-        "black",
-        "configuraptor",
-        "tomli",
-        "typer",
-        "rich",
         "builtins",
-        "_collections_abc",
-        "_operator",
         "_typeshed",
         "abc",
         "array",
-        "click",
-        "click.exceptions",
-        "configuraptor.cls",
-        "configuraptor.core",
-        "configuraptor.singleton",
         "ctypes",
-        "io",
-        "json.encoder",
+        "datetime",
         "mmap",
-        "pathlib",
         "pickle",
+        "re",
         "typing_extensions"
     ],
-    "hash": "4531074b446dd039771e488da928eadf7eb65518e85da6f89586cf06258d5607",
-    "id": "su6.core",
-    "ignore_all": false,
-    "interface_hash": "c0809d6839e6360472c0ab2be9390ab2a74a037c698b1864a3b68c3d75ded91f",
-    "mtime": 1689600630,
+    "hash": "83df8435a00b4be07c768918a42bb35056a55a5a20ed3f922183232d9496aed3",
+    "id": "tomli._parser",
+    "ignore_all": true,
+    "interface_hash": "6e31967856dd5ef6578786412e1b325abf05a6e963239c741f70f6893b66d115",
+    "mtime": 1687249184,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -161,18 +99,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/su6/core.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomli/_parser.py",
     "plugin_data": null,
-    "size": 18701,
-    "suppressed": [
-        "plumbum.commands.processes",
-        "plumbum.commands",
-        "plumbum.machines",
-        "plumbum"
-    ],
+    "size": 22633,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/helpers.data.json` & `su6-1.6.4/.mypy_cache/3.11/su6/helpers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/helpers.meta.json` & `su6-1.6.4/.mypy_cache/3.11/su6/helpers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/plugins.data.json` & `su6-1.6.4/.mypy_cache/3.11/su6/plugins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/su6/plugins.meta.json` & `su6-1.6.4/.mypy_cache/3.11/su6/plugins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomli/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomli/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli/_parser.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomli/_parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli/_parser.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomli/_types.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7862745098039216%*

 * *Differences: {"'dep_lines'": '{delete: [8, 7, 6, 5, 4, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [9, 8, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": '{delete: [15, 12, 5, 4, 3, 2, 1, 0]}',*

 * * "'hash'": "'f864c6d9552a929c7032ace654ee05ef26ca75d21b027b801d77e65907138b74'",*

 * * "'id'": "'tomli._types'",*

 * * "'interface_hash'": "'7cd825e1941eb6d89013091b7999476c34577b8469d6bc2ba00a5ab22439923b'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomli/_types.py'",*

 * * "'size'": '254'}*

```diff
@@ -1,70 +1,46 @@
 {
     "data_mtime": 1687249414,
     "dep_lines": [
-        7,
-        12,
-        20,
         5,
-        8,
-        9,
-        10,
-        1,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5,
-        5,
-        10,
-        5,
-        5,
-        5,
-        30,
-        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "tomli._re",
-        "tomli._types",
-        "__future__",
-        "string",
-        "types",
         "typing",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
-        "datetime",
         "mmap",
         "pickle",
-        "re",
         "typing_extensions"
     ],
-    "hash": "83df8435a00b4be07c768918a42bb35056a55a5a20ed3f922183232d9496aed3",
-    "id": "tomli._parser",
+    "hash": "f864c6d9552a929c7032ace654ee05ef26ca75d21b027b801d77e65907138b74",
+    "id": "tomli._types",
     "ignore_all": true,
-    "interface_hash": "6e31967856dd5ef6578786412e1b325abf05a6e963239c741f70f6893b66d115",
+    "interface_hash": "7cd825e1941eb6d89013091b7999476c34577b8469d6bc2ba00a5ab22439923b",
     "mtime": 1687249184,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -99,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomli/_parser.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomli/_types.py",
     "plugin_data": null,
-    "size": 22633,
+    "size": 254,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli/_re.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomli/_re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli/_re.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomli/_re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli/_types.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomli/_types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli/_types.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/mock.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6952380952380951%*

 * *Differences: {"'data_mtime'": '1686754983',*

 * * "'dep_lines'": '{insert: [(0, 2), (2, 3), (3, 4), (4, 5), (5, 6)], delete: [4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (3, 5), (4, 5), (5, 5), (6, 5)], delete: [6, 5, 4, 3, 2]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, 'contextlib'), (3, 'types'), "*

 * *                   "(5, 'typing_extensions')], delete: [8, 7, 6, 5, 4]}",*

 * * "'hash'": "'98625f75a980e4a99a6f836a6ed17e1f95c3729047bca86c6c48dfe60f8702a5'",*

 * * "'id'": "'unittest.mock'",*

 * * "'int […]*

```diff
@@ -1,47 +1,47 @@
 {
-    "data_mtime": 1687249414,
+    "data_mtime": 1686754983,
     "dep_lines": [
-        5,
-        1,
-        1,
-        1,
-        1,
+        2,
         1,
+        3,
+        4,
+        5,
+        6,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
+        5,
+        5,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
+        "collections.abc",
+        "sys",
+        "contextlib",
+        "types",
         "typing",
+        "typing_extensions",
         "builtins",
         "_typeshed",
-        "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "f864c6d9552a929c7032ace654ee05ef26ca75d21b027b801d77e65907138b74",
-    "id": "tomli._types",
+    "hash": "98625f75a980e4a99a6f836a6ed17e1f95c3729047bca86c6c48dfe60f8702a5",
+    "id": "unittest.mock",
     "ignore_all": true,
-    "interface_hash": "7cd825e1941eb6d89013091b7999476c34577b8469d6bc2ba00a5ab22439923b",
-    "mtime": 1687249184,
+    "interface_hash": "04f1a98f621dd3b651ca7b0998077573046a4805b7a93a4e825f6fc29fa3f0f3",
+    "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -75,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomli/_types.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi",
     "plugin_data": null,
-    "size": 254,
+    "size": 14406,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli_w/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomli_w/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli_w/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/toml_document.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7733333333333333%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(0, 1)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'tomlkit.container')], delete: [0]}",*

 * * "'hash'": "'3824e45977773f9f04653e120fcfdd75cd58a6431aaad952e7fb2d1d306630e2'",*

 * * "'id'": "'tomlkit.toml_document'",*

 * * "'interface_hash'": "'a0d184bdb63a66409de7c4fad331682a411a614ca9a17cee3e75584b9b68460e'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/toml_document.py'",*

 * * "'size'": '110'}*

```diff
@@ -1,31 +1,31 @@
 {
-    "data_mtime": 1687249414,
+    "data_mtime": 1686754984,
     "dep_lines": [
-        4,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "tomli_w._writer",
+        "tomlkit.container",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "c3cdef9f865651a478788c5258258e5643d8f2a18943ebae5699c8b5dce69245",
-    "id": "tomli_w",
+    "hash": "3824e45977773f9f04653e120fcfdd75cd58a6431aaad952e7fb2d1d306630e2",
+    "id": "tomlkit.toml_document",
     "ignore_all": true,
-    "interface_hash": "ed818460546f71f4107d04c1605d8fbbb0fe158c708f3dac618afd4533fadfd2",
+    "interface_hash": "a0d184bdb63a66409de7c4fad331682a411a614ca9a17cee3e75584b9b68460e",
     "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -60,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomli_w/__init__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/toml_document.py",
     "plugin_data": null,
-    "size": 157,
+    "size": 110,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli_w/_writer.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomli_w/_writer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomli_w/_writer.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomli_w/_writer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.74%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 5), (2, 2), (3, 3), (4, 4)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 10), (3, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.case'), (1, 'logging'), (2, 'sys'), (3, 'types'), (4, "*

 * *                   "'typing'), (6, '_typeshed')], delete: [3, 0]}",*

 * * "'hash'": "'297a51a36613ffcd84bcef772c3f0dd0fdb57a1a9acc544a72840468647d968c'",*

 * * "'id'": "'unittest._log'",*

 * * "'interface_hash'": "'20b576be7b25765af8108589e0827b19be51be5c76414d2ce9027946fcb1ee5c'",*

 * * "'mtime'": '16867 […]*

```diff
@@ -1,32 +1,44 @@
 {
     "data_mtime": 1686754984,
     "dep_lines": [
+        5,
         1,
+        2,
+        3,
+        4,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        10,
+        5,
+        5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "tomlkit.api",
+        "unittest.case",
+        "logging",
+        "sys",
+        "types",
+        "typing",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "feee93b1ddf737d85ff86840869aa3eadd2ca0d9d33b92cfdae31d5b05fdc46d",
-    "id": "tomlkit",
+    "hash": "297a51a36613ffcd84bcef772c3f0dd0fdb57a1a9acc544a72840468647d968c",
+    "id": "unittest._log",
     "ignore_all": true,
-    "interface_hash": "931319b0d54715d34e26f52d066c2f348b156844b23e01c31fc62e15115262c7",
-    "mtime": 1686754196,
+    "interface_hash": "20b576be7b25765af8108589e0827b19be51be5c76414d2ce9027946fcb1ee5c",
+    "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/__init__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/_log.pyi",
     "plugin_data": null,
-    "size": 1148,
+    "size": 892,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/_compat.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/_compat.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/_utils.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/_utils.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.726797385620915%*

 * *Differences: {"'data_mtime'": '1687356209',*

 * * "'dep_lines'": '{delete: [5, 4, 3, 1, 0]}',*

 * * "'dep_prios'": '{delete: [5, 4, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'click'), (8, 'typing')], delete: [7, 5, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a'",*

 * * "'id'": "'typer._compat_utils'",*

 * * "'interface_hash'": "'f13939f83ff3c74c0b399e38a0f09049771195ed55e4e7d096d0f5225ca3996b'",*

 * * "'mtime'": '1686754198',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.1 […]*

```diff
@@ -1,65 +1,50 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1687356209,
     "dep_lines": [
-        5,
-        13,
         1,
-        3,
-        6,
-        11,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        5,
-        5,
         10,
         5,
-        5,
-        5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "tomlkit._compat",
-        "__future__",
-        "re",
-        "datetime",
-        "typing",
+        "click",
         "builtins",
-        "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle",
+        "typing",
         "typing_extensions"
     ],
-    "hash": "7d7d67edba028bbfdb05505e99acb09347b2c6a8536276563e10991c980166ff",
-    "id": "tomlkit._utils",
+    "hash": "929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a",
+    "id": "typer._compat_utils",
     "ignore_all": true,
-    "interface_hash": "45431f8929f73a2c5625b9f707ed70315bad82515082caf54c17d64631be18a5",
-    "mtime": 1686754196,
+    "interface_hash": "f13939f83ff3c74c0b399e38a0f09049771195ed55e4e7d096d0f5225ca3996b",
+    "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -93,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/_utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_compat_utils.py",
     "plugin_data": null,
-    "size": 4021,
+    "size": 94,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/api.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/api.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/api.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/container.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/container.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/container.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/container.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/exceptions.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/exceptions.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/items.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/items.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/items.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/items.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/parser.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/parser.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/source.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/source.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/source.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/source.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/toml_char.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/toml_char.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/toml_char.meta.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/toml_char.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/toml_document.data.json` & `su6-1.6.4/.mypy_cache/3.11/tomlkit/toml_document.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/tomlkit/toml_document.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7416666666666667%*

 * *Differences: {"'data_mtime'": '1686754983',*

 * * "'dep_lines'": '{delete: [0]}',*

 * * "'dep_prios'": '{delete: [0]}',*

 * * "'dependencies'": '{delete: [0]}',*

 * * "'hash'": "'7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f'",*

 * * "'id'": "'typer.colors'",*

 * * "'interface_hash'": "'27b284b26e724e12cf37260c1baa2dfb8b4eacd2f12a30cc5a22b69d7b95ad25'",*

 * * "'mtime'": '1686754198',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/colors.py'",*

 * * "'size'": '430'}*

```diff
@@ -1,32 +1,29 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1686754983,
     "dep_lines": [
         1,
         1,
-        1,
         1
     ],
     "dep_prios": [
         5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "tomlkit.container",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "3824e45977773f9f04653e120fcfdd75cd58a6431aaad952e7fb2d1d306630e2",
-    "id": "tomlkit.toml_document",
+    "hash": "7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f",
+    "id": "typer.colors",
     "ignore_all": true,
-    "interface_hash": "a0d184bdb63a66409de7c4fad331682a411a614ca9a17cee3e75584b9b68460e",
-    "mtime": 1686754196,
+    "interface_hash": "27b284b26e724e12cf37260c1baa2dfb8b4eacd2f12a30cc5a22b69d7b95ad25",
+    "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/toml_document.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/colors.py",
     "plugin_data": null,
-    "size": 110,
+    "size": 430,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_checkers.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_checkers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_checkers.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_checkers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_config.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_config.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_config.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_config.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_decorators.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_decorators.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_exceptions.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_exceptions.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_functions.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_functions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_functions.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_functions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_importhook.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_importhook.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_importhook.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_importhook.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_memo.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_memo.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_memo.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_memo.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_suppression.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_suppression.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_suppression.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_suppression.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_transformer.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_transformer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_transformer.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_transformer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_utils.data.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typeguard/_utils.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typeguard/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_compat_utils.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/params.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7656410256410257%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 5), (1, 8), (3, 3)], delete: [4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 25), (2, 5)], delete: [6, 5, 4, 3, 2]}',*

 * * "'dependencies'": "{insert: [(0, 'typer.models'), (1, 'click.shell_completion'), (2, 'typing'), "*

 * *                   "(6, 'click.core'), (7, 'click.types')], delete: [9, 8, 7, 6, 5, 4, 2]}",*

 * * "'hash'": "'fcf07893bfc8bf4aa53628a147a0b9383364d9146d16d97b31bf5d993a818c4c'",*

 * * "'id'": "'typer.params'",*

 * * "'interface_hash'": "'e8e28933e640b7a78446e418ed017d […]*

```diff
@@ -1,49 +1,43 @@
 {
     "data_mtime": 1687356209,
     "dep_lines": [
+        5,
+        8,
         1,
-        1,
-        1,
-        1,
-        1,
-        1,
+        3,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
+        25,
+        5,
         10,
         5,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
+        "typer.models",
+        "click.shell_completion",
+        "typing",
         "click",
         "builtins",
-        "_typeshed",
         "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle",
-        "typing",
-        "typing_extensions"
+        "click.core",
+        "click.types"
     ],
-    "hash": "929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a",
-    "id": "typer._compat_utils",
+    "hash": "fcf07893bfc8bf4aa53628a147a0b9383364d9146d16d97b31bf5d993a818c4c",
+    "id": "typer.params",
     "ignore_all": true,
-    "interface_hash": "f13939f83ff3c74c0b399e38a0f09049771195ed55e4e7d096d0f5225ca3996b",
+    "interface_hash": "e8e28933e640b7a78446e418ed017d302c5b8ec515ab27ca1c0cc9c2eac83b45",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -78,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_compat_utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/params.py",
     "plugin_data": null,
-    "size": 94,
+    "size": 13401,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_completion_click7.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_completion_click7.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_completion_click7.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_completion_click7.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_completion_click8.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_completion_click8.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_completion_click8.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_completion_click8.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_completion_shared.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_typing.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/_typing.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/colors.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/colors.meta.json` & `su6-1.6.4/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'hash'": "'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'",*

 * * "'id'": "'urllib'",*

 * * "'interface_hash'": "'697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi'",*

 * * "'size'": '0'}*

```diff
@@ -11,18 +11,18 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f",
-    "id": "typer.colors",
+    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
+    "id": "urllib",
     "ignore_all": true,
-    "interface_hash": "27b284b26e724e12cf37260c1baa2dfb8b4eacd2f12a30cc5a22b69d7b95ad25",
+    "interface_hash": "697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -57,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/colors.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi",
     "plugin_data": null,
-    "size": 430,
+    "size": 0,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/completion.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/completion.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/core.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/core.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/main.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/main.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/models.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/models.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/models.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/params.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/params.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/helpers.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6981818181818181%*

 * *Differences: {"'data_mtime'": '1689928121',*

 * * "'dep_lines'": '{insert: [(0, 8), (2, 6)], delete: [5, 4, 3, 2]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 10), (3, 20)], delete: [6, 5, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'black.files'), (1, 'os'), (3, 'black')], delete: [7, 6, 3, 1, "*

 * *                   '0]}',*

 * * "'hash'": "'1d469a327f98f7243c857e6aba72a4c1fd967703adc663110892794cebfad902'",*

 * * "'id'": "'configuraptor.helpers'",*

 * * "'interface_hash'": "'f84351965c73017b1ec9d03f5cf408c235a4dc7e2507fc75039fa0fadcc2eba7'" […]*

```diff
@@ -1,44 +1,38 @@
 {
-    "data_mtime": 1687356209,
+    "data_mtime": 1689928121,
     "dep_lines": [
+        8,
         5,
+        6,
         8,
         1,
-        3,
-        1,
-        1,
-        1,
         1
     ],
     "dep_prios": [
-        5,
-        25,
-        5,
         10,
+        10,
+        10,
+        20,
         5,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "typer.models",
-        "click.shell_completion",
+        "black.files",
+        "os",
         "typing",
-        "click",
+        "black",
         "builtins",
-        "abc",
-        "click.core",
-        "click.types"
+        "abc"
     ],
-    "hash": "fcf07893bfc8bf4aa53628a147a0b9383364d9146d16d97b31bf5d993a818c4c",
-    "id": "typer.params",
+    "hash": "1d469a327f98f7243c857e6aba72a4c1fd967703adc663110892794cebfad902",
+    "id": "configuraptor.helpers",
     "ignore_all": true,
-    "interface_hash": "e8e28933e640b7a78446e418ed017d302c5b8ec515ab27ca1c0cc9c2eac83b45",
-    "mtime": 1686754198,
+    "interface_hash": "f84351965c73017b1ec9d03f5cf408c235a4dc7e2507fc75039fa0fadcc2eba7",
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/params.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/helpers.py",
     "plugin_data": null,
-    "size": 13401,
+    "size": 611,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/rich_utils.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/rich_utils.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/utils.data.json` & `su6-1.6.4/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/typer/utils.meta.json` & `su6-1.6.4/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/__init__.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/_log.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/_log.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7742647058823529%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 3), (2, 31), (7, 6), (8, 7), (9, 8), (10, 9), (11, 10), (12, 11)], '*

 * *                'delete: [5]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5), (5, 20), (9, 5), (10, 5), (11, 5), (12, 5), (13, 5)], '*

 * *                'delete: [6]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.result'), (1, 'collections.abc'), (2, "*

 * *                   "'unittest._log'), (5, 'unittest'), (6, '_typeshed'), (7, 'contextlib'), (8, "*

 * *                   "'re'), (11, 'typing_extensions'), (12, 'warnin […]*

```diff
@@ -1,43 +1,64 @@
 {
     "data_mtime": 1686754984,
     "dep_lines": [
+        3,
         5,
+        31,
         1,
         2,
         3,
         4,
-        1,
+        6,
+        7,
+        8,
+        9,
+        10,
+        11,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
         5,
         10,
         10,
+        20,
+        5,
+        5,
+        5,
+        5,
+        5,
         5,
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
-        "unittest.case",
+        "unittest.result",
+        "collections.abc",
+        "unittest._log",
         "logging",
         "sys",
+        "unittest",
+        "_typeshed",
+        "contextlib",
+        "re",
         "types",
         "typing",
+        "typing_extensions",
+        "warnings",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "297a51a36613ffcd84bcef772c3f0dd0fdb57a1a9acc544a72840468647d968c",
-    "id": "unittest._log",
+    "hash": "2e896b10930c0bd8849a3e6b4c584e7eba9265f85efeffa0ba24a2e732a8967b",
+    "id": "unittest.case",
     "ignore_all": true,
-    "interface_hash": "20b576be7b25765af8108589e0827b19be51be5c76414d2ce9027946fcb1ee5c",
+    "interface_hash": "6211186fbeefd54fdb8566dd5541d7ca569758703d677367662f6b6bc3b59b68",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +93,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/_log.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/case.pyi",
     "plugin_data": null,
-    "size": 892,
+    "size": 13905,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/async_case.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/async_case.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/case.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/case.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7769444444444444%*

 * *Differences: {"'dep_lines'": '{insert: [(2, 1)], delete: [12, 11, 10, 9, 8, 7, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [10, 9, 8, 7, 6, 4, 3, 1]}',*

 * * "'dependencies'": '{delete: [12, 9, 8, 7, 6, 4, 3, 2]}',*

 * * "'hash'": "'eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c'",*

 * * "'id'": "'unittest.signals'",*

 * * "'interface_hash'": "'92394d833593a182a1c8b1a7f4bbde75b454b011f0d89a59947f25f24cf7b720'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/signal […]*

```diff
@@ -1,64 +1,40 @@
 {
     "data_mtime": 1686754984,
     "dep_lines": [
-        3,
-        5,
-        31,
         1,
         2,
+        1,
         3,
         4,
-        6,
-        7,
-        8,
-        9,
-        10,
-        11,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
-        5,
-        10,
-        10,
         20,
         5,
         5,
         5,
-        5,
-        5,
-        5,
-        5,
-        5,
         30
     ],
     "dependencies": [
         "unittest.result",
         "collections.abc",
-        "unittest._log",
-        "logging",
-        "sys",
         "unittest",
-        "_typeshed",
-        "contextlib",
-        "re",
-        "types",
         "typing",
         "typing_extensions",
-        "warnings",
         "builtins",
         "abc"
     ],
-    "hash": "2e896b10930c0bd8849a3e6b4c584e7eba9265f85efeffa0ba24a2e732a8967b",
-    "id": "unittest.case",
+    "hash": "eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c",
+    "id": "unittest.signals",
     "ignore_all": true,
-    "interface_hash": "6211186fbeefd54fdb8566dd5541d7ca569758703d677367662f6b6bc3b59b68",
+    "interface_hash": "92394d833593a182a1c8b1a7f4bbde75b454b011f0d89a59947f25f24cf7b720",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -93,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/case.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi",
     "plugin_data": null,
-    "size": 13905,
+    "size": 488,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/loader.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/loader.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/main.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/main.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/mock.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/mock.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/mock.meta.json` & `su6-1.6.4/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8096296296296296%*

 * *Differences: {"'dep_lines'": '{insert: [(4, 7)], delete: [5, 4]}',*

 * * "'dep_prios'": '{delete: [2]}',*

 * * "'dependencies'": "{insert: [(4, 'types')], delete: [3, 2]}",*

 * * "'hash'": "'9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1'",*

 * * "'id'": "'urllib.parse'",*

 * * "'interface_hash'": "'02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi'",*

 * * "'size'": '6532'}*

```diff
@@ -1,46 +1,43 @@
 {
     "data_mtime": 1686754983,
     "dep_lines": [
         2,
         1,
         3,
         4,
-        5,
-        6,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
         5,
-        5,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "contextlib",
-        "types",
         "typing",
         "typing_extensions",
+        "types",
         "builtins",
         "_typeshed",
         "abc"
     ],
-    "hash": "98625f75a980e4a99a6f836a6ed17e1f95c3729047bca86c6c48dfe60f8702a5",
-    "id": "unittest.mock",
+    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
+    "id": "urllib.parse",
     "ignore_all": true,
-    "interface_hash": "04f1a98f621dd3b651ca7b0998077573046a4805b7a93a4e825f6fc29fa3f0f3",
+    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -75,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
     "plugin_data": null,
-    "size": 14406,
+    "size": 6532,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/result.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/result.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/runner.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/runner.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/signals.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/signals.meta.json` & `su6-1.6.4/.mypy_cache/3.11/configuraptor/type_converters.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6992424242424242%*

 * *Differences: {"'data_mtime'": '1689594458',*

 * * "'dep_lines'": '{insert: [(0, 5), (1, 6), (4, 1), (5, 1)], delete: [4, 3, 1]}',*

 * * "'dep_prios'": '{insert: [(3, 30), (4, 30), (5, 30), (6, 30)], delete: [3, 2, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'types'), (4, 'array'), (5, 'ctypes'), (6, 'mmap'), (7, "*

 * *                   "'pickle')], delete: [4, 2, 1, 0]}",*

 * * "'hash'": "'bebe5e7d07b9ce305e6f0b69cb68e5213f622350d86ba2fdbdf7f67717d7bbbe'",*

 * * "'id'": "'configuraptor.type_converters'",*

 * * "'interface_hash'": "'dbcaaec299ca916f5ed […]*

```diff
@@ -1,41 +1,44 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1689594458,
     "dep_lines": [
+        5,
+        6,
+        1,
+        1,
         1,
-        2,
         1,
-        3,
-        4,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
-        20,
-        5,
-        5,
         5,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "unittest.result",
-        "collections.abc",
-        "unittest",
+        "types",
         "typing",
-        "typing_extensions",
         "builtins",
-        "abc"
+        "abc",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c",
-    "id": "unittest.signals",
+    "hash": "bebe5e7d07b9ce305e6f0b69cb68e5213f622350d86ba2fdbdf7f67717d7bbbe",
+    "id": "configuraptor.type_converters",
     "ignore_all": true,
-    "interface_hash": "92394d833593a182a1c8b1a7f4bbde75b454b011f0d89a59947f25f24cf7b720",
-    "mtime": 1686754198,
+    "interface_hash": "dbcaaec299ca916f5edb02ba65d22b75b29d702a46b15230e10f98f055da7ae1",
+    "mtime": 1689928118,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/type_converters.py",
     "plugin_data": null,
-    "size": 488,
+    "size": 2006,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/suite.data.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/unittest/suite.meta.json` & `su6-1.6.4/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/urllib/__init__.data.json` & `su6-1.6.4/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/urllib/__init__.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7035409035409035%*

 * *Differences: {"'data_mtime'": '1685433917',*

 * * "'dep_lines'": '{insert: [(0, 1), (1, 2), (2, 3)]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5), (2, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (1, 'typing'), (2, 'typing_extensions'), (4, "*

 * *                   "'_typeshed')], delete: [2]}",*

 * * "'hash'": "'cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c'",*

 * * "'id'": "'sre_constants'",*

 * * "'interface_hash'": "'9712b3c3ae06b67272c232e1379bf306d8606ccbd5bb6d332f741942b043edb8'",*

 * * "'mtime'": '1685293614',*

 * * "'opti […]*

```diff
@@ -1,69 +1,78 @@
 {
-    "data_mtime": 1686754983,
+    "data_mtime": 1685433917,
     "dep_lines": [
         1,
+        2,
+        3,
+        1,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
+        5,
         5,
         30,
         30
     ],
     "dependencies": [
+        "sys",
+        "typing",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
-    "id": "urllib",
+    "hash": "cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c",
+    "id": "sre_constants",
     "ignore_all": true,
-    "interface_hash": "697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3",
-    "mtime": 1686754198,
+    "interface_hash": "9712b3c3ae06b67272c232e1379bf306d8606ccbd5bb6d332f741942b043edb8",
+    "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
-        "check_untyped_defs": true,
+        "check_untyped_defs": false,
         "disable_bytearray_promotion": false,
         "disable_error_code": [],
         "disable_memoryview_promotion": false,
         "disabled_error_codes": [],
         "disallow_any_decorated": false,
         "disallow_any_explicit": false,
         "disallow_any_expr": false,
-        "disallow_any_generics": true,
+        "disallow_any_generics": false,
         "disallow_any_unimported": false,
-        "disallow_incomplete_defs": true,
-        "disallow_subclassing_any": true,
-        "disallow_untyped_calls": true,
-        "disallow_untyped_decorators": true,
-        "disallow_untyped_defs": true,
+        "disallow_incomplete_defs": false,
+        "disallow_subclassing_any": false,
+        "disallow_untyped_calls": false,
+        "disallow_untyped_decorators": false,
+        "disallow_untyped_defs": false,
         "enable_error_code": [],
         "enabled_error_codes": [],
         "follow_imports": "normal",
         "follow_imports_for_stubs": false,
         "ignore_errors": false,
-        "ignore_missing_imports": true,
-        "implicit_optional": true,
-        "implicit_reexport": false,
+        "ignore_missing_imports": false,
+        "implicit_optional": false,
+        "implicit_reexport": true,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
-        "strict_concatenate": true,
-        "strict_equality": true,
+        "strict_concatenate": false,
+        "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
-        "warn_return_any": true,
+        "warn_return_any": false,
         "warn_unreachable": false,
-        "warn_unused_ignores": true
+        "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_constants.pyi",
     "plugin_data": null,
-    "size": 0,
+    "size": 3986,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.mypy_cache/3.11/urllib/parse.data.json` & `su6-1.6.4/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.mypy_cache/3.11/urllib/parse.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/os/path.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7123504273504274%*

 * *Differences: {"'data_mtime'": '1685433917',*

 * * "'dep_lines'": '{delete: [3, 2, 0]}',*

 * * "'dep_prios'": '{delete: [3, 2, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'posixpath'), (4, 'typing')], delete: [6, 4, 3, 2, 0]}",*

 * * "'hash'": "'1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433'",*

 * * "'id'": "'os.path'",*

 * * "'interface_hash'": "'a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e'",*

 * * "'mtime'": '1685293614',*

 * * "'options'": "{'strict_equality': False, 'disallow_incomplete_defs': False, "*

 * *              […]*

```diff
@@ -1,84 +1,75 @@
 {
-    "data_mtime": 1686754983,
+    "data_mtime": 1685433917,
     "dep_lines": [
-        2,
         1,
-        3,
-        4,
         7,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
         10,
         5,
         5,
-        5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
         "sys",
-        "typing",
-        "typing_extensions",
-        "types",
+        "posixpath",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
-    "id": "urllib.parse",
+    "hash": "1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433",
+    "id": "os.path",
     "ignore_all": true,
-    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
-    "mtime": 1686754198,
+    "interface_hash": "a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e",
+    "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
-        "check_untyped_defs": true,
+        "check_untyped_defs": false,
         "disable_bytearray_promotion": false,
         "disable_error_code": [],
         "disable_memoryview_promotion": false,
         "disabled_error_codes": [],
         "disallow_any_decorated": false,
         "disallow_any_explicit": false,
         "disallow_any_expr": false,
-        "disallow_any_generics": true,
+        "disallow_any_generics": false,
         "disallow_any_unimported": false,
-        "disallow_incomplete_defs": true,
-        "disallow_subclassing_any": true,
-        "disallow_untyped_calls": true,
-        "disallow_untyped_decorators": true,
-        "disallow_untyped_defs": true,
+        "disallow_incomplete_defs": false,
+        "disallow_subclassing_any": false,
+        "disallow_untyped_calls": false,
+        "disallow_untyped_decorators": false,
+        "disallow_untyped_defs": false,
         "enable_error_code": [],
         "enabled_error_codes": [],
         "follow_imports": "normal",
         "follow_imports_for_stubs": false,
         "ignore_errors": false,
-        "ignore_missing_imports": true,
-        "implicit_optional": true,
-        "implicit_reexport": false,
+        "ignore_missing_imports": false,
+        "implicit_optional": false,
+        "implicit_reexport": true,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
-        "strict_concatenate": true,
-        "strict_equality": true,
+        "strict_concatenate": false,
+        "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
-        "warn_return_any": true,
+        "warn_return_any": false,
         "warn_unreachable": false,
-        "warn_unused_ignores": true
+        "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/path.pyi",
     "plugin_data": null,
-    "size": 6532,
+    "size": 186,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/.pytest_cache/v/cache/lastfailed` & `su6-1.6.4/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.pytest_cache/v/cache/nodeids` & `su6-1.6.4/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/122419b0bc04bb24` & `su6-1.6.4/.ruff_cache/content/122419b0bc04bb24`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/14681219216720271199` & `su6-1.6.4/.ruff_cache/content/14681219216720271199`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/1a4449eb8b26a401` & `su6-1.6.4/.ruff_cache/content/1a4449eb8b26a401`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/1b7872d6314f48b7` & `su6-1.6.4/.ruff_cache/content/1b7872d6314f48b7`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/1f88fbdfcbf2d8d6` & `su6-1.6.4/.ruff_cache/content/1f88fbdfcbf2d8d6`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/294d5a468695eb7e` & `su6-1.6.4/.ruff_cache/content/294d5a468695eb7e`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/2bf27b960bc3ded1` & `su6-1.6.4/.ruff_cache/content/2bf27b960bc3ded1`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/2face4e073dced28` & `su6-1.6.4/.ruff_cache/content/2face4e073dced28`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/30e241b2876dc71f` & `su6-1.6.4/.ruff_cache/content/30e241b2876dc71f`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/33004598889f4950` & `su6-1.6.4/.ruff_cache/content/33004598889f4950`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/36f0bdaeef592d9` & `su6-1.6.4/.ruff_cache/content/36f0bdaeef592d9`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/38b035e004ea9f4` & `su6-1.6.4/.ruff_cache/content/38b035e004ea9f4`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/3c7fb493febe6a55` & `su6-1.6.4/.ruff_cache/content/3c7fb493febe6a55`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/3ccdd2336c8c80e9` & `su6-1.6.4/.ruff_cache/content/3ccdd2336c8c80e9`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/3db675ebeb97b2fe` & `su6-1.6.4/.ruff_cache/content/3db675ebeb97b2fe`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/3f10d9d7687f3999` & `su6-1.6.4/.ruff_cache/content/3f10d9d7687f3999`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/42f337caed884834` & `su6-1.6.4/.ruff_cache/content/42f337caed884834`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/51de14ac05bcd5d1` & `su6-1.6.4/.ruff_cache/content/51de14ac05bcd5d1`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/534b8acecf74c47` & `su6-1.6.4/.ruff_cache/content/534b8acecf74c47`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/536320baecd03af6` & `su6-1.6.4/.ruff_cache/content/536320baecd03af6`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/5436d767d06cf116` & `su6-1.6.4/.ruff_cache/content/5436d767d06cf116`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/5cc5d54a963753bf` & `su6-1.6.4/.ruff_cache/content/5cc5d54a963753bf`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/684d0841c18787fb` & `su6-1.6.4/.ruff_cache/content/684d0841c18787fb`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/68c4553df91c1f5e` & `su6-1.6.4/.ruff_cache/content/68c4553df91c1f5e`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/72a6612daca66426` & `su6-1.6.4/.ruff_cache/content/72a6612daca66426`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/81e6f787866d0ecf` & `su6-1.6.4/.ruff_cache/content/81e6f787866d0ecf`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/84e2e26fc69ab274` & `su6-1.6.4/.ruff_cache/content/84e2e26fc69ab274`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/881c84062ed51136` & `su6-1.6.4/.ruff_cache/content/881c84062ed51136`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/8a5ec4ca9660671c` & `su6-1.6.4/.ruff_cache/content/8a5ec4ca9660671c`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/8ccd539b7f96dff8` & `su6-1.6.4/.ruff_cache/content/8ccd539b7f96dff8`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/9019e33ca68d8935` & `su6-1.6.4/.ruff_cache/content/9019e33ca68d8935`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/95df46a8e947b100` & `su6-1.6.4/.ruff_cache/content/95df46a8e947b100`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/9613cbbc5a7c60a4` & `su6-1.6.4/.ruff_cache/content/9613cbbc5a7c60a4`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/abe0d13d37518e58` & `su6-1.6.4/.ruff_cache/content/abe0d13d37518e58`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/ac8c237c67408442` & `su6-1.6.4/.ruff_cache/content/ac8c237c67408442`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/b780a63a1663add6` & `su6-1.6.4/.ruff_cache/content/b780a63a1663add6`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/b8ab8c7df580ad75` & `su6-1.6.4/.ruff_cache/content/b8ab8c7df580ad75`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/b8d965aa2b8fd993` & `su6-1.6.4/.ruff_cache/content/b8d965aa2b8fd993`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/b990e7d90d89db2a` & `su6-1.6.4/.ruff_cache/content/b990e7d90d89db2a`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/bde6d6e902485336` & `su6-1.6.4/.ruff_cache/content/bde6d6e902485336`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/be4a1815dbb4c4` & `su6-1.6.4/.ruff_cache/content/be4a1815dbb4c4`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/be5eb6e8ff99feab` & `su6-1.6.4/.ruff_cache/content/be5eb6e8ff99feab`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/ca3d1e0ddece82f5` & `su6-1.6.4/.ruff_cache/content/ca3d1e0ddece82f5`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/cb326dd0ee5910c6` & `su6-1.6.4/.ruff_cache/content/cb326dd0ee5910c6`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/d8fb97841110c062` & `su6-1.6.4/.ruff_cache/content/d8fb97841110c062`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/d954f2ee22d56fd0` & `su6-1.6.4/.ruff_cache/content/d954f2ee22d56fd0`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/da0cf7e13e17e6a6` & `su6-1.6.4/.ruff_cache/content/da0cf7e13e17e6a6`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/db73ef232740be87` & `su6-1.6.4/.ruff_cache/content/db73ef232740be87`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/dc4a4b4b55cceada` & `su6-1.6.4/.ruff_cache/content/dc4a4b4b55cceada`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/df3de5bc83871643` & `su6-1.6.4/.ruff_cache/content/df3de5bc83871643`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/e067c98663409f12` & `su6-1.6.4/.ruff_cache/content/e067c98663409f12`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/e24118b3523194dc` & `su6-1.6.4/.ruff_cache/content/e24118b3523194dc`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/ed03e948b89996b8` & `su6-1.6.4/.ruff_cache/content/ed03e948b89996b8`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/ed645de094b6d7bb` & `su6-1.6.4/.ruff_cache/content/ed645de094b6d7bb`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/f5d61064e60c404b` & `su6-1.6.4/.ruff_cache/content/f5d61064e60c404b`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/.ruff_cache/content/fd17e608110a0864` & `su6-1.6.4/.ruff_cache/content/fd17e608110a0864`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/_static/su6.png` & `su6-1.6.4/_static/su6.png`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/_static/su6.svg` & `su6-1.6.4/_static/su6.svg`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/docs/plugins.md` & `su6-1.6.4/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/coverage_html.js` & `su6-1.6.4/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_2602a302b50854cf___about___py.html` & `su6-1.6.4/htmlcov/d_2602a302b50854cf___about___py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_2602a302b50854cf___init___py.html` & `su6-1.6.4/htmlcov/d_2602a302b50854cf___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_2602a302b50854cf_cli_py.html` & `su6-1.6.4/htmlcov/d_2602a302b50854cf_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_2602a302b50854cf_core_py.html` & `su6-1.6.4/htmlcov/d_2602a302b50854cf_core_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_2602a302b50854cf_plugins_py.html` & `su6-1.6.4/htmlcov/d_2602a302b50854cf_plugins_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_a44f0ac069e85531___init___py.html` & `su6-1.6.4/htmlcov/d_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_a44f0ac069e85531__shared_py.html` & `su6-1.6.4/htmlcov/d_a44f0ac069e85531__shared_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_a44f0ac069e85531_test_about_py.html` & `su6-1.6.4/htmlcov/d_a44f0ac069e85531_test_about_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_a44f0ac069e85531_test_cli_py.html` & `su6-1.6.4/htmlcov/d_a44f0ac069e85531_test_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/d_a44f0ac069e85531_test_core_py.html` & `su6-1.6.4/htmlcov/d_a44f0ac069e85531_test_core_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/favicon_32.png` & `su6-1.6.4/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/index.html` & `su6-1.6.4/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/keybd_closed.png` & `su6-1.6.4/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/keybd_open.png` & `su6-1.6.4/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/status.json` & `su6-1.6.4/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/htmlcov/style.css` & `su6-1.6.4/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/except_pytest.toml` & `su6-1.6.4/pytest_examples/except_pytest.toml`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_ast.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_ast.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_codecs.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_codecs.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_ctypes.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/abc.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/abc.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/array.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/array.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/bad.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/bad.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/bad.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/bad.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/builtins.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/builtins.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/codecs.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/codecs.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/contextlib.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/contextlib.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/dataclasses.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/enum.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/enum.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/genericpath.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/genericpath.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/good.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/good.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/io.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/io.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/mmap.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/mmap.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/pathlib.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/pathlib.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/pickle.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/pickle.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/posixpath.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/posixpath.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/re.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/re.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_compile.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_constants.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7926587301587301%*

 * *Differences: {"'dep_lines'": '{delete: [3]}',*

 * * "'dep_prios'": '{insert: [(3, 5)], delete: [4, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'email.message')], delete: [4, 2, 0]}",*

 * * "'hash'": "'53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf'",*

 * * "'id'": "'email.contentmanager'",*

 * * "'interface_hash'": "'86a7db72494c58ed2d0e5e9f95b2906da6e78e83aa31e5d85859dcbc0d594fad'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmana […]*

```diff
@@ -1,37 +1,34 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
         1,
         2,
         3,
         1,
-        1,
         1
     ],
     "dep_prios": [
-        10,
         5,
         5,
         5,
-        30,
+        5,
         30
     ],
     "dependencies": [
-        "sys",
+        "collections.abc",
+        "email.message",
         "typing",
-        "typing_extensions",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c",
-    "id": "sre_constants",
+    "hash": "53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf",
+    "id": "email.contentmanager",
     "ignore_all": true,
-    "interface_hash": "9712b3c3ae06b67272c232e1379bf306d8606ccbd5bb6d332f741942b043edb8",
+    "interface_hash": "86a7db72494c58ed2d0e5e9f95b2906da6e78e83aa31e5d85859dcbc0d594fad",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -66,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_constants.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi",
     "plugin_data": null,
-    "size": 3986,
+    "size": 480,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_parse.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/subprocess.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/subprocess.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/sys.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/sys.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/this.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/this.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/types.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/types.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/typing.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/typing.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/collections/abc.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/__init__.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/charset.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/charset.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8133333333333332%*

 * *Differences: {"'dep_lines'": '{delete: [2]}',*

 * * "'dep_prios'": '{delete: [0]}',*

 * * "'dependencies'": '{delete: [1]}',*

 * * "'hash'": "'2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4'",*

 * * "'id'": "'importlib.metadata._meta'",*

 * * "'interface_hash'": "'c88463ed7df95bf0015736581082e5a7cd111fdf7879efce7252e1872cba96cd'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi'",*

 * * "'size'": '842'}*

```diff
@@ -1,34 +1,31 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
         1,
         2,
-        3,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
-        5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "email.message",
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf",
-    "id": "email.contentmanager",
+    "hash": "2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4",
+    "id": "importlib.metadata._meta",
     "ignore_all": true,
-    "interface_hash": "86a7db72494c58ed2d0e5e9f95b2906da6e78e83aa31e5d85859dcbc0d594fad",
+    "interface_hash": "c88463ed7df95bf0015736581082e5a7cd111fdf7879efce7252e1872cba96cd",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -63,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi",
     "plugin_data": null,
-    "size": 480,
+    "size": 842,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/errors.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/errors.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/header.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/header.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/message.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/message.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/policy.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/email/policy.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-1.6.4/.mypy_cache/3.11/su6/__about__.meta.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6790170940170941%*

 * *Differences: {"'data_mtime'": '1686754983',*

 * * "'dep_lines'": '{delete: [1]}',*

 * * "'dep_prios'": '{insert: [(1, 30)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(2, 'typing')], delete: [1, 0]}",*

 * * "'hash'": "'ff4e71a4c1c9eef82261765cce11cc26ea483b052d21dd06497b3d28d9ebf5d2'",*

 * * "'id'": "'su6.__about__'",*

 * * "'ignore_all'": 'False',*

 * * "'interface_hash'": "'f585c505c8d50598658e61be6359ebe7fcc6381e8be269711f79d29222dffbf9'",*

 * * "'mtime'": '1689613962',*

 * * "'options'": "{'check_untyped_defs': True, 'disallow_any_generics': True, "*

 * * […]*

```diff
@@ -1,72 +1,69 @@
 {
-    "data_mtime": 1685433917,
+    "data_mtime": 1686754983,
     "dep_lines": [
         1,
-        2,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "typing",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4",
-    "id": "importlib.metadata._meta",
-    "ignore_all": true,
-    "interface_hash": "c88463ed7df95bf0015736581082e5a7cd111fdf7879efce7252e1872cba96cd",
-    "mtime": 1685293614,
+    "hash": "ff4e71a4c1c9eef82261765cce11cc26ea483b052d21dd06497b3d28d9ebf5d2",
+    "id": "su6.__about__",
+    "ignore_all": false,
+    "interface_hash": "f585c505c8d50598658e61be6359ebe7fcc6381e8be269711f79d29222dffbf9",
+    "mtime": 1689613962,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
-        "check_untyped_defs": false,
+        "check_untyped_defs": true,
         "disable_bytearray_promotion": false,
         "disable_error_code": [],
         "disable_memoryview_promotion": false,
         "disabled_error_codes": [],
         "disallow_any_decorated": false,
         "disallow_any_explicit": false,
         "disallow_any_expr": false,
-        "disallow_any_generics": false,
+        "disallow_any_generics": true,
         "disallow_any_unimported": false,
-        "disallow_incomplete_defs": false,
-        "disallow_subclassing_any": false,
-        "disallow_untyped_calls": false,
-        "disallow_untyped_decorators": false,
-        "disallow_untyped_defs": false,
+        "disallow_incomplete_defs": true,
+        "disallow_subclassing_any": true,
+        "disallow_untyped_calls": true,
+        "disallow_untyped_decorators": true,
+        "disallow_untyped_defs": true,
         "enable_error_code": [],
         "enabled_error_codes": [],
         "follow_imports": "normal",
         "follow_imports_for_stubs": false,
         "ignore_errors": false,
-        "ignore_missing_imports": false,
-        "implicit_optional": false,
-        "implicit_reexport": true,
+        "ignore_missing_imports": true,
+        "implicit_optional": true,
+        "implicit_reexport": false,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
-        "strict_concatenate": false,
-        "strict_equality": false,
+        "strict_concatenate": true,
+        "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
-        "warn_return_any": false,
+        "warn_return_any": true,
         "warn_unreachable": false,
-        "warn_unused_ignores": false
+        "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi",
+    "path": "src/su6/__about__.py",
     "plugin_data": null,
-    "size": 842,
+    "size": 206,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/os/__init__.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pytest_examples/.mypy_cache/3.11/os/path.data.json` & `su6-1.6.4/pytest_examples/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/src/su6/cli.py` & `su6-1.6.4/src/su6/cli.py`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/src/su6/core.py` & `su6-1.6.4/src/su6/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 This file contains internal helpers used by cli.py.
 """
 import enum
 import functools
 import inspect
 import json
 import operator
-import os
 import sys
 import types
 import typing
 from dataclasses import dataclass, field
 from typing import Any, Callable, Optional, TypeAlias, Union
 
-import black.files
 import configuraptor
 import plumbum.commands.processes as pb
 import tomli
 import typer
 from configuraptor import convert_config
+from configuraptor.helpers import find_pyproject_toml
 from plumbum import local
 from plumbum.machines import LocalCommand
 from rich import print
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     from .plugins import AnyRegistration
 
@@ -357,21 +356,14 @@
 
 
 MaybeConfig: TypeAlias = Optional[Config]
 
 T_typelike: TypeAlias = type | types.UnionType | types.UnionType
 
 
-def find_pyproject_toml() -> Optional[str]:
-    """
-    Find the project's config toml, looks up until it finds the project root (black's logic).
-    """
-    return black.files.find_pyproject_toml((os.getcwd(),))
-
-
 def _get_su6_config(overwrites: dict[str, Any], toml_path: str = None) -> MaybeConfig:
     """
     Parse the users pyproject.toml (found using black's logic) and extract the tool.su6 part.
 
     The types as entered in the toml are checked using _ensure_types,
     to make sure there isn't a string implicitly converted to a list of characters or something.
```

### Comparing `su6-1.6.3/src/su6/plugins.py` & `su6-1.6.4/src/su6/plugins.py`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/tests/test_cli.py` & `su6-1.6.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/tests/test_core.py` & `su6-1.6.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/tests/test_plugins.py` & `su6-1.6.4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/tests/test_plugins_config.py` & `su6-1.6.4/tests/test_plugins_config.py`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/LICENSE.txt` & `su6-1.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/README.md` & `su6-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `su6-1.6.3/pyproject.toml` & `su6-1.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "typer[all]",
     "plumbum",
-    "black", # for 'find_pyproject_toml'
-    "configuraptor >= 1.7", # for config, should include 'tomlkit'
+    "configuraptor >= 1.14",
 ]
 
 [template.plugins.default]
 src-layout = true
 
 [tool.setuptools.package-data]
 "su6" = ["py.typed"]
```

### Comparing `su6-1.6.3/PKG-INFO` & `su6-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python cli tool to use tools for some common code quality checks (opinionated)
 Project-URL: Documentation, https://github.com/trialandsuccess/su6#readme
 Project-URL: Issues, https://github.com/trialandsuccess/su6/issues
 Project-URL: Source, https://github.com/trialandsuccess/su6
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -12,16 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: black
-Requires-Dist: configuraptor>=1.7
+Requires-Dist: configuraptor>=1.14
 Requires-Dist: plumbum
 Requires-Dist: typer[all]
 Provides-Extra: all
 Requires-Dist: bandit; extra == 'all'
 Requires-Dist: black; extra == 'all'
 Requires-Dist: contextlib-chdir; python_version < '3.11' and extra == 'all'
 Requires-Dist: coverage-badge; extra == 'all'
```

#### html2text {}

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1 Name: su6 Version: 1.6.3 Summary: Python cli tool to use
+Metadata-Version: 2.1 Name: su6 Version: 1.6.4 Summary: Python cli tool to use
 tools for some common code quality checks (opinionated) Project-URL:
 Documentation, https://github.com/trialandsuccess/su6#readme Project-URL:
 Issues, https://github.com/trialandsuccess/su6/issues Project-URL: Source,
 https://github.com/trialandsuccess/su6 Author-email: Robin van der Noord
 gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Python: >=3.10 Requires-Dist: black Requires-Dist: configuraptor>=1.7 Requires-
-Dist: plumbum Requires-Dist: typer[all] Provides-Extra: all Requires-Dist:
-bandit; extra == 'all' Requires-Dist: black; extra == 'all' Requires-Dist:
-contextlib-chdir; python_version < '3.11' and extra == 'all' Requires-Dist:
-coverage-badge; extra == 'all' Requires-Dist: isort; extra == 'all' Requires-
-Dist: mypy; extra == 'all' Requires-Dist: pydocstyle; extra == 'all' Requires-
-Dist: pytest; extra == 'all' Requires-Dist: pytest-cov; extra == 'all'
-Requires-Dist: ruff; extra == 'all' Provides-Extra: bandit Requires-Dist:
-bandit; extra == 'bandit' Provides-Extra: black Requires-Dist: black; extra ==
-'black' Provides-Extra: dev Requires-Dist: hatch; extra == 'dev' Requires-Dist:
-python-semantic-release; extra == 'dev' Requires-Dist: su6-plugin-demo; extra
-== 'dev' Provides-Extra: isort Requires-Dist: isort; extra == 'isort' Provides-
-Extra: mypy Requires-Dist: mypy; extra == 'mypy' Provides-Extra: prettier
-Requires-Dist: su6-plugin-prettier; extra == 'prettier' Provides-Extra:
-pydocstyle Requires-Dist: pydocstyle; extra == 'pydocstyle' Provides-Extra:
-pytest Requires-Dist: contextlib-chdir; python_version < '3.11' and extra ==
-'pytest' Requires-Dist: coverage-badge; extra == 'pytest' Requires-Dist:
-pytest; extra == 'pytest' Requires-Dist: pytest-cov; extra == 'pytest'
-Provides-Extra: ruff Requires-Dist: ruff; extra == 'ruff' Provides-Extra:
-svelte-check Requires-Dist: su6-plugin-svelte-check; extra == 'svelte-check'
-Description-Content-Type: text/markdown
+Python: >=3.10 Requires-Dist: configuraptor>=1.14 Requires-Dist: plumbum
+Requires-Dist: typer[all] Provides-Extra: all Requires-Dist: bandit; extra ==
+'all' Requires-Dist: black; extra == 'all' Requires-Dist: contextlib-chdir;
+python_version < '3.11' and extra == 'all' Requires-Dist: coverage-badge; extra
+== 'all' Requires-Dist: isort; extra == 'all' Requires-Dist: mypy; extra ==
+'all' Requires-Dist: pydocstyle; extra == 'all' Requires-Dist: pytest; extra ==
+'all' Requires-Dist: pytest-cov; extra == 'all' Requires-Dist: ruff; extra ==
+'all' Provides-Extra: bandit Requires-Dist: bandit; extra == 'bandit' Provides-
+Extra: black Requires-Dist: black; extra == 'black' Provides-Extra: dev
+Requires-Dist: hatch; extra == 'dev' Requires-Dist: python-semantic-release;
+extra == 'dev' Requires-Dist: su6-plugin-demo; extra == 'dev' Provides-Extra:
+isort Requires-Dist: isort; extra == 'isort' Provides-Extra: mypy Requires-
+Dist: mypy; extra == 'mypy' Provides-Extra: prettier Requires-Dist: su6-plugin-
+prettier; extra == 'prettier' Provides-Extra: pydocstyle Requires-Dist:
+pydocstyle; extra == 'pydocstyle' Provides-Extra: pytest Requires-Dist:
+contextlib-chdir; python_version < '3.11' and extra == 'pytest' Requires-Dist:
+coverage-badge; extra == 'pytest' Requires-Dist: pytest; extra == 'pytest'
+Requires-Dist: pytest-cov; extra == 'pytest' Provides-Extra: ruff Requires-
+Dist: ruff; extra == 'ruff' Provides-Extra: svelte-check Requires-Dist: su6-
+plugin-svelte-check; extra == 'svelte-check' Description-Content-Type: text/
+markdown
                                  [su6 checker]
                                ****** su6 ******
     6 is pronounced as '/zÉs/' in Dutch, so 'su6' is basically 'success'.
                 This package will hopefully help achieve that!
 
                    [PyPI_-_Version] [PyPI_-_Python_Version]
                       [Code_style:_black] [License:_MIT]
```

