# Comparing `tmp/ethernetip-1.0.0.tar.gz` & `tmp/ethernetip-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethernetip-1.0.0.tar", last modified: Sun Mar 14 16:32:05 2021, max compression
+gzip compressed data, was "/home/bloc/Projects/python-ethernetip/dist/.tmp-y2y_t2qk/ethernetip-1.1.0.tar", last modified: Fri Jul 21 09:11:25 2023, max compression
```

## Comparing `ethernetip-1.0.0.tar` & `ethernetip-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 bloc      (1000) bloc      (1000)        0 2021-03-14 16:32:05.411426 ethernetip-1.0.0/
--rw-r--r--   0 bloc      (1000) bloc      (1000)      853 2021-03-14 16:32:05.411426 ethernetip-1.0.0/PKG-INFO
--rwxr-xr-x   0 bloc      (1000) bloc      (1000)       83 2021-03-14 13:04:54.000000 ethernetip-1.0.0/README.md
--rw-r--r--   0 bloc      (1000) bloc      (1000)      104 2021-03-14 15:18:44.000000 ethernetip-1.0.0/pyproject.toml
--rw-r--r--   0 bloc      (1000) bloc      (1000)      424 2021-03-14 16:32:05.411426 ethernetip-1.0.0/setup.cfg
--rw-r--r--   0 bloc      (1000) bloc      (1000)     1457 2021-03-14 16:24:39.000000 ethernetip-1.0.0/setup.py
-drwxr-xr-x   0 bloc      (1000) bloc      (1000)        0 2021-03-14 16:32:05.407426 ethernetip-1.0.0/src/
-drwxr-xr-x   0 bloc      (1000) bloc      (1000)        0 2021-03-14 16:32:05.407426 ethernetip-1.0.0/src/ethernetip/
--rwxr-xr-x   0 bloc      (1000) bloc      (1000)      677 2021-03-14 15:32:11.000000 ethernetip-1.0.0/src/ethernetip/__init__.py
--rwxr-xr-x   0 bloc      (1000) bloc      (1000)    41771 2021-03-14 13:04:54.000000 ethernetip-1.0.0/src/ethernetip/ethernetip.py
-drwxr-xr-x   0 bloc      (1000) bloc      (1000)        0 2021-03-14 16:32:05.411426 ethernetip-1.0.0/src/ethernetip.egg-info/
--rw-r--r--   0 bloc      (1000) bloc      (1000)      853 2021-03-14 16:32:05.000000 ethernetip-1.0.0/src/ethernetip.egg-info/PKG-INFO
--rw-r--r--   0 bloc      (1000) bloc      (1000)      325 2021-03-14 16:32:05.000000 ethernetip-1.0.0/src/ethernetip.egg-info/SOURCES.txt
--rw-r--r--   0 bloc      (1000) bloc      (1000)        1 2021-03-14 16:32:05.000000 ethernetip-1.0.0/src/ethernetip.egg-info/dependency_links.txt
--rw-r--r--   0 bloc      (1000) bloc      (1000)        1 2021-03-14 15:34:08.000000 ethernetip-1.0.0/src/ethernetip.egg-info/not-zip-safe
--rw-r--r--   0 bloc      (1000) bloc      (1000)        5 2021-03-14 16:32:05.000000 ethernetip-1.0.0/src/ethernetip.egg-info/requires.txt
--rw-r--r--   0 bloc      (1000) bloc      (1000)       11 2021-03-14 16:32:05.000000 ethernetip-1.0.0/src/ethernetip.egg-info/top_level.txt
+drwxr-xr-x   0 bloc      (1000) bloc      (1000)        0 2023-07-21 09:11:25.000000 ethernetip-1.1.0/
+-rwxr-xr-x   0 bloc      (1000) bloc      (1000)     1072 2021-12-19 13:11:53.000000 ethernetip-1.1.0/LICENSE
+-rw-r--r--   0 bloc      (1000) bloc      (1000)      914 2023-07-21 09:11:25.000000 ethernetip-1.1.0/PKG-INFO
+-rwxr-xr-x   0 bloc      (1000) bloc      (1000)       83 2021-12-19 13:11:53.000000 ethernetip-1.1.0/README.md
+-rw-r--r--   0 bloc      (1000) bloc      (1000)      104 2021-12-19 13:11:53.000000 ethernetip-1.1.0/pyproject.toml
+-rw-r--r--   0 bloc      (1000) bloc      (1000)      424 2023-07-21 09:11:25.000000 ethernetip-1.1.0/setup.cfg
+-rw-r--r--   0 bloc      (1000) bloc      (1000)     1601 2023-07-21 09:05:59.000000 ethernetip-1.1.0/setup.py
+drwxr-xr-x   0 bloc      (1000) bloc      (1000)        0 2023-07-21 09:11:25.000000 ethernetip-1.1.0/src/
+drwxr-xr-x   0 bloc      (1000) bloc      (1000)        0 2023-07-21 09:11:25.000000 ethernetip-1.1.0/src/ethernetip/
+-rwxr-xr-x   0 bloc      (1000) bloc      (1000)      677 2023-07-21 09:06:28.000000 ethernetip-1.1.0/src/ethernetip/__init__.py
+-rwxr-xr-x   0 bloc      (1000) bloc      (1000)    43030 2023-07-21 09:03:56.000000 ethernetip-1.1.0/src/ethernetip/ethernetip.py
+drwxr-xr-x   0 bloc      (1000) bloc      (1000)        0 2023-07-21 09:11:25.000000 ethernetip-1.1.0/src/ethernetip.egg-info/
+-rw-r--r--   0 bloc      (1000) bloc      (1000)      914 2023-07-21 09:11:25.000000 ethernetip-1.1.0/src/ethernetip.egg-info/PKG-INFO
+-rw-r--r--   0 bloc      (1000) bloc      (1000)      358 2023-07-21 09:11:25.000000 ethernetip-1.1.0/src/ethernetip.egg-info/SOURCES.txt
+-rw-r--r--   0 bloc      (1000) bloc      (1000)        1 2023-07-21 09:11:25.000000 ethernetip-1.1.0/src/ethernetip.egg-info/dependency_links.txt
+-rw-r--r--   0 bloc      (1000) bloc      (1000)        1 2022-01-06 15:46:43.000000 ethernetip-1.1.0/src/ethernetip.egg-info/not-zip-safe
+-rw-r--r--   0 bloc      (1000) bloc      (1000)        5 2023-07-21 09:11:25.000000 ethernetip-1.1.0/src/ethernetip.egg-info/requires.txt
+-rw-r--r--   0 bloc      (1000) bloc      (1000)       11 2023-07-21 09:11:25.000000 ethernetip-1.1.0/src/ethernetip.egg-info/top_level.txt
+drwxr-xr-x   0 bloc      (1000) bloc      (1000)        0 2023-07-21 09:11:25.000000 ethernetip-1.1.0/tests/
+-rw-r--r--   0 bloc      (1000) bloc      (1000)      453 2022-01-06 16:19:00.000000 ethernetip-1.1.0/tests/test_ethernetip.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ethernetip-1.0.0/PKG-INFO` & `ethernetip-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ethernetip
-Version: 1.0.0
+Version: 1.1.0
 Summary: Basic EtherNet/IP scanner
 Home-page: https://codeberg.org/paperwork/python-ethernetip
 Author: Sebastian Block
 Author-email: sebastian.block@world-wi.de
 License: MIT
-Description: python_ethernetip
-        =================
-        
-        basic Ethernet/IP implementation for python 3
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+python_ethernetip
+=================
+
+basic Ethernet/IP implementation for python 3
```

### Comparing `ethernetip-1.0.0/setup.py` & `ethernetip-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 readme = open('README.md').read()
 requirements = ['dpkt']
 
 # PyPI Readme
 long_description = open('README.md').read()
 
 setuptools.setup(name=package_name,
-                 version="1.0.0",
+                 version="1.1.0",
                  author="Sebastian Block",
                  author_email="sebastian.block@world-wi.de",
                  url="https://codeberg.org/paperwork/python-ethernetip",
                  description=description,
                  long_description=long_description,
                  package_dir={"": "src"},
                  packages=setuptools.find_packages(where="src"),
@@ -25,8 +25,10 @@
                               'License :: OSI Approved :: MIT License',
                               'Natural Language :: English',
                               'Programming Language :: Python :: 2.7',
                               'Programming Language :: Python :: 3.5',
                               'Programming Language :: Python :: 3.6',
                               'Programming Language :: Python :: 3.7',
                               'Programming Language :: Python :: 3.8',
-                              'Programming Language :: Python :: 3.9'])
+                              'Programming Language :: Python :: 3.9',
+                              'Programming Language :: Python :: 3.10',
+                              'Programming Language :: Python :: 3.11'])
```

### Comparing `ethernetip-1.0.0/src/ethernetip/__init__.py` & `ethernetip-1.1.0/src/ethernetip/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import division
 import sys
 
 __author__ = 'Sebastian Block'
 __author_email__ = 'sebastian.block@world-wi.de'
 __license__ = 'MIT'
 __url__ = 'https://codeberg.org/paperwork/python-ethernetip'
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 
 from .ethernetip import *
 
 # Note: list() is used to get a copy of the dict in order to avoid
 # "RuntimeError: dictionary changed size during iteration"
 # exception in Python 3 caused by _mod_init() funcs that load another modules
 for name, mod in list(sys.modules.items()):
```

### Comparing `ethernetip-1.0.0/src/ethernetip/ethernetip.py` & `ethernetip-1.1.0/src/ethernetip/ethernetip.py`

 * *Files 3% similar despite different names*

```diff
@@ -394,54 +394,79 @@
         if self.typ == 1:
             self.enip.listenUDP()
         elif self.typ == 2:
             self.conn.prodThread()
 
 
 class EtherNetIP(object):
+    """
+    EtherNet/IP class
+
+    :param ip: IP address of the device
+    :type ip: str
+    """
     ENIP_IO_TYPE_INPUT  = 0
     ENIP_IO_TYPE_OUTPUT = 1
 
     def __init__(self, ip="127.0.0.1"):
         self.assembly  = {}
         self.explicit  = []
         self.udpsock   = None
         self.udpthread = None
         self.io_state  = 0
         self.ip = ip
 
     def registerAssembly(self, iotype, size, inst, conn):
-        if inst in self.assembly:
+        """
+        Register an assembly instance used to produce IO.
+
+        :param iotype: IO type to register (ENIP_IO_TYPE_INPUT/ENIP_IO_TYPE_OUTPUT)
+        :param size: size of the assembly in bytes
+        :param inst: instance of the assembly
+        :param conn: connection to use
+
+        :returns: array of bits with size of 8 times the size parameter
+        """
+        if (inst, conn) in self.assembly:
             print("Reg assembly failed for iotype=", iotype)
             return None
         bits = []
         for i in range(size * 8):
             bits.append(0)
-        self.assembly[inst] = (conn, iotype, bits)
+        self.assembly[(inst, conn)] = (conn, iotype, bits)
         if conn is not None:
             if iotype == EtherNetIP.ENIP_IO_TYPE_INPUT:
                 conn.mapIn(bits)
             elif iotype == EtherNetIP.ENIP_IO_TYPE_OUTPUT:
                 conn.mapOut(bits)
         return bits
 
     def startIO(self):
+        """
+        Start produce IO
+        """
         if self.io_state == 0:
             self.udpsock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             self.udpsock.bind(("0.0.0.0", ENIP_UDP_PORT))
             self.udpthread = EthernetIOThread(1, self)
             self.io_state = 1
             self.udpthread.start()
 
     def stopIO(self):
+        """
+        Stop producing IO
+        """
         if self.io_state == 1:
             self.io_state = 0
             self.udpsock.close()
 
     def listenUDP(self):
+        """
+        Function that is called from IO producing :class:`EthernetIOThread`
+        """
         while 1 == self.io_state:
             inp, out, err = select.select([self.udpsock], [], [], 2)
             if len(inp) != 0:
                 try:
                     buf, addr = self.udpsock.recvfrom(1024)
                 except OSError:
                     # If we close the socket asynchronously, the recv will
@@ -465,21 +490,34 @@
                                 if byte & (1 << s):
                                     bits[i] = True
                                 else:
                                     bits[i] = False
                                 i += 1
 
     def explicit_conn(self, ipaddr=None):
+        """
+        Create explicit connection
+
+        :param ipaddr: IP address used for the explicit connection
+        :type ipaddr: str, optional
+        """
         if ipaddr is None:
             ipaddr = self.ip
         exp = EtherNetIPExpConnection(ipaddr)
         self.explicit.append(exp)
         return exp
 
     def listIDUDP(self, ipaddr=None, timeout=5):
+        """
+        Send ListIdentify requeset to ipaddr.
+
+        :param ipaddr: IP address to send ListIdentify request to
+        :param timeout: Timeout until answer needs to be received (default 5s)
+        :return: ListIdentify reply or None if no answer received within timeout.
+        """
         udpsock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         udpsock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         context = random.randint(1, 4026531839)
         pkt = EncapsulationPacket(command=EncapsulationPacket.ENCAP_CMD_LISTIDENTITY,
                                   sender_context=context.to_bytes(8, byteorder='big'))
         if ipaddr is None:
             ipaddr = self.ip
@@ -494,14 +532,17 @@
                 if csd.type_id == CommandSpecificData.TYPE_ID_LIST_IDENT_RESPONSE:
                     lid = ListIdentifyReply(csd.data)
                     return lid
         return None
 
 
 class EtherNetIPSocket(object):
+    """
+    Socket class
+    """
     def __init__(self, ip):
         self.ipaddr = ip
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.sock.connect((self.ipaddr, ENIP_TCP_PORT))
         self.conn_serial_num = 0
 
     def delete(self):
@@ -658,15 +699,15 @@
                     csd = CommandSpecificData(srr.data)
                     cpf = UnconnectedDataItemResp(csd.data)
                     ret = [cpf.status, cpf.data]
                     if chk != 0:
                         rsppkt = self.unconnSendValidRsp(service, chkdata, context)
                         if str(rsppkt) != str(pkt):
                             print("Packets differ")
-                            assert(0)
+                            assert (0)
                     return ret
         return None
 
     def unconnSendValidRsp(self, service, data, context=0):
         # sz = len(data) + 17
         dsz = len(data) + 1
         cpf2 = UnconnectedDataItem(type_id=CommandSpecificData.TYPE_ID_UNCONNECTED_MESSAGE,
@@ -876,29 +917,31 @@
                     return 0
                 elif udi.data[1] == 0x01:  # Forward open failed with Connection Failure
                     if udi.data[2] > 0:
                         extended_status, = struct.unpack("H", udi.data[3:5])
                         return extended_status
         return None
 
-    def sendFwdCloseReq(self, inputinst, outputinst, configinst, path_class=0x04, connection_serialno=None):
+    def sendFwdCloseReq(self, inputinst, outputinst, configinst, path_class=0x04,
+                        connection_serialno=None, fwdc=None):
         path = struct.pack(">BBB", 0x20, path_class, 0x24) + struct.pack("B", configinst)
         if outputinst is not None:
             path += struct.pack("B", 0x2c) + struct.pack("B", outputinst)
         if inputinst is not None:
             path += struct.pack("B", 0x2c) + struct.pack("B", inputinst)
         plen = int(len(path) / 2)
         if connection_serialno is None:
             conn_serial_num = self.conn_serial_num
         else:
             conn_serial_num = connection_serialno
-        fwdc = ForwardCloseReq(conn_serial=conn_serial_num,
-                               mkpath=self.mkReqPath(clas=0x06, inst=0x01, attr=None),
-                               plen=plen,
-                               data=path)
+        if fwdc is None:
+            fwdc = ForwardCloseReq(conn_serial=conn_serial_num,
+                                   mkpath=self.mkReqPath(clas=0x06, inst=0x01, attr=None),
+                                   plen=plen,
+                                   data=path)
         # add service field
         dsz = len(fwdc) + 1
         cpf2 = UnconnectedDataItem(type_id=CommandSpecificData.TYPE_ID_UNCONNECTED_MESSAGE,
                                    length=dsz, data=fwdc,
                                    service=(CI_SRV_FORWARD_CLOSE | UnconnectedDataItem.UNCONN_DATA_ITEM_SERVICE_REQUEST))
         cpf = CommandSpecificData(type_id=CommandSpecificData.TYPE_ID_NULL,
                                   item_count=2, length=0, data=cpf2)
```

### Comparing `ethernetip-1.0.0/src/ethernetip.egg-info/PKG-INFO` & `ethernetip-1.1.0/src/ethernetip.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ethernetip
-Version: 1.0.0
+Version: 1.1.0
 Summary: Basic EtherNet/IP scanner
 Home-page: https://codeberg.org/paperwork/python-ethernetip
 Author: Sebastian Block
 Author-email: sebastian.block@world-wi.de
 License: MIT
-Description: python_ethernetip
-        =================
-        
-        basic Ethernet/IP implementation for python 3
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+python_ethernetip
+=================
+
+basic Ethernet/IP implementation for python 3
```

