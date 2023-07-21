# Comparing `tmp/divideandscan-0.3.7.tar.gz` & `tmp/divideandscan-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divideandscan-0.3.7.tar", max compression
+gzip compressed data, was "divideandscan-0.3.8.tar", max compression
```

## Comparing `divideandscan-0.3.7.tar` & `divideandscan-0.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1320 2023-07-07 21:28:52.598816 divideandscan-0.3.7/LICENSE
--rw-r--r--   0        0        0    14973 2023-07-07 21:28:52.598816 divideandscan-0.3.7/README.md
--rw-r--r--   0        0        0       29 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/__init__.py
--rw-r--r--   0        0        0     3895 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/common.py
--rwxr-xr-x   0        0        0    12593 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/divideandscan.py
--rw-r--r--   0        0        0     1406 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/dns.py
--rw-r--r--   0        0        0     7856 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/drawnmap.py
--rw-r--r--   0        0        0     2247 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsenmap.py
--rw-r--r--   0        0        0     1737 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/__init__.py
--rw-r--r--   0        0        0      669 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/masscan.py
--rw-r--r--   0        0        0      599 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/naabu.py
--rw-r--r--   0        0        0      868 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/nimscan.py
--rw-r--r--   0        0        0      648 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/nmap.py
--rw-r--r--   0        0        0      660 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/rustscan.py
--rw-r--r--   0        0        0      590 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/sx.py
--rw-r--r--   0        0        0     9261 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/report.py
--rw-r--r--   0        0        0     7144 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/scan.py
--rw-r--r--   0        0        0     1139 2023-07-07 21:28:52.602816 divideandscan-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    16143 1970-01-01 00:00:00.000000 divideandscan-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1320 2023-07-21 11:08:15.000629 divideandscan-0.3.8/LICENSE
+-rw-r--r--   0        0        0    14973 2023-07-21 11:08:15.000629 divideandscan-0.3.8/README.md
+-rw-r--r--   0        0        0       29 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/__init__.py
+-rw-r--r--   0        0        0     3895 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/common.py
+-rwxr-xr-x   0        0        0    12593 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/divideandscan.py
+-rw-r--r--   0        0        0     1406 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/dns.py
+-rw-r--r--   0        0        0     7856 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/drawnmap.py
+-rw-r--r--   0        0        0     2314 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/parsenmap.py
+-rw-r--r--   0        0        0     1737 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/parsers/__init__.py
+-rw-r--r--   0        0        0      669 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/parsers/masscan.py
+-rw-r--r--   0        0        0      599 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/parsers/naabu.py
+-rw-r--r--   0        0        0      868 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/parsers/nimscan.py
+-rw-r--r--   0        0        0      648 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/parsers/nmap.py
+-rw-r--r--   0        0        0      660 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/parsers/rustscan.py
+-rw-r--r--   0        0        0      590 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/parsers/sx.py
+-rw-r--r--   0        0        0     9261 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/report.py
+-rw-r--r--   0        0        0     7224 2023-07-21 11:08:15.000629 divideandscan-0.3.8/das/scan.py
+-rw-r--r--   0        0        0     1139 2023-07-21 11:08:15.004629 divideandscan-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0    16143 1970-01-01 00:00:00.000000 divideandscan-0.3.8/PKG-INFO
```

### Comparing `divideandscan-0.3.7/LICENSE` & `divideandscan-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/README.md` & `divideandscan-0.3.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </p>
 
 <p align="center">
   <strong>Divide <strike>Et Impera</strike> And Scan (and also merge the scan results)</strong>
 </p>
 
 <p align="center">
-  <a href="https://github.com/snovvcrash/DivideAndScan/blob/main/pyproject.toml#L3"><img src="https://img.shields.io/badge/version-0.3.7-success" alt="version" /></a>
+  <a href="https://github.com/snovvcrash/DivideAndScan/blob/main/pyproject.toml#L3"><img src="https://img.shields.io/badge/version-0.3.8-success" alt="version" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/search?l=python"><img src="https://img.shields.io/badge/python-3.9-blue?logo=python&logoColor=white" alt="python" /></a>
   <a href="https://www.codacy.com/gh/snovvcrash/DivideAndScan/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=snovvcrash/DivideAndScan&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/35f0bdfece9846d7aab3888b01642813" alt="codacy" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-pypi.yml"><img src="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-pypi.yml/badge.svg" alt="pypi" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-docker-hub.yml"><img src="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-docker-hub.yml/badge.svg" alt="docker" /></a>
 </p>
 
 ---
```

### Comparing `divideandscan-0.3.7/das/common.py` & `divideandscan-0.3.8/das/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 __author__ = '@snovvcrash'
 __site__ = 'https://github.com/snovvcrash/DivideAndScan'
-__version__ = '0.3.7'
+__version__ = '0.3.8'
 
 import time
 from datetime import datetime, timedelta
 
 BANNER = """\
 \033[0;37m -----------------------------------------------------------------------------------------------
 \033[0;37m|\033[1;31m  ________  \033[0;37m.__      .__    .___        \033[1;31m_____\033[0;37m              .__\033[1;31m__________\033[0;37m   \033[1;31m                    |
```

### Comparing `divideandscan-0.3.7/das/divideandscan.py` & `divideandscan-0.3.8/das/divideandscan.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/dns.py` & `divideandscan-0.3.8/das/dns.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/drawnmap.py` & `divideandscan-0.3.8/das/drawnmap.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/parsenmap.py` & `divideandscan-0.3.8/das/parsenmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 		:rtype: das.report.NmapParser
 		"""
 		self.services = services.split(',')
 		
 		self.db = None
 		if dns:
 			self.db = TinyDB(db_path)
-			self.Host = Query()
+			self.ip_domains_dict = {}
+			for item in self.db.all():
+				self.ip_domains_dict[item['ip']] = item['domains']
 
 		self.raw_output = raw_output
 
 		db_name = Path(db_path).stem
 		P = (Path.home() / '.das' / f'nmap_{db_name}').glob('*.xml')
 		P = list(P)
 
@@ -53,15 +55,15 @@
 			for ip in nm.all_hosts():
 				if 'tcp' in nm[ip]:
 					for port in nm[ip]['tcp']:
 						if nm[ip]['tcp'][port]['state'] == 'open':
 							service = nm[ip]['tcp'][port]['name']
 							if service in self.services:
 								if self.db:
-									domains = self.db.search(self.Host.ip == ip)[0]['domains']
+									domains = self.ip_domains_dict[ip]
 									if domains:
 										for domain in domains:
 											if not self.raw_output:
 												Logger.print_success(f'IP {ip} -> {service}://{domain}:{port}')
 											else:
 												print(f'{service}://{domain}:{port}')
 										continue
```

### Comparing `divideandscan-0.3.7/das/parsers/__init__.py` & `divideandscan-0.3.8/das/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/parsers/masscan.py` & `divideandscan-0.3.8/das/parsers/masscan.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/parsers/naabu.py` & `divideandscan-0.3.8/das/parsers/naabu.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/parsers/nimscan.py` & `divideandscan-0.3.8/das/parsers/nimscan.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/parsers/nmap.py` & `divideandscan-0.3.8/das/parsers/nmap.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/parsers/rustscan.py` & `divideandscan-0.3.8/das/parsers/rustscan.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/parsers/sx.py` & `divideandscan-0.3.8/das/parsers/sx.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/report.py` & `divideandscan-0.3.8/das/report.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.7/das/scan.py` & `divideandscan-0.3.8/das/scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,20 @@
 				result = self.db.all()
 			else:
 				hosts = hosts.split(',')
 				hosts = [IPNetwork(h) for h in hosts]
 				hosts = [str(ip) for ip_obj in hosts for ip in ip_obj]
 				result = self.db.search(self.Host.ip.one_of(hosts))
 
-			self.ip_dict = defaultdict(set)
+			self.ip_ports_dict, self.ip_domains_dict = defaultdict(set), {}
 			for item in result:
-				self.ip_dict[item['ip']].add(item['port'])
+				self.ip_ports_dict[item['ip']].add(item['port'])
+				self.ip_domains_dict[item['ip']] = item['domains']
 
-			self.total_scans += len(self.ip_dict)
+			self.total_scans += len(self.ip_ports_dict)
 
 		elif ports:
 			try:
 				if Path(ports).exists():
 					with open(ports, 'r') as fd:
 						ports = ','.join(i.strip() for i in fd.read().splitlines())
 			except OSError:  # catching [Errno 36] File name too long
@@ -70,19 +71,19 @@
 
 			if ports == 'all':
 				result = self.db.all()
 			else:
 				ports = [int(p) for p in ports.split(',')]
 				result = self.db.search(self.Host.port.one_of(ports))
 
-			self.port_dict = defaultdict(set)
+			self.port_ip_dict = defaultdict(set)
 			for item in result:
-				self.port_dict[item['port']].add(item['ip'])
+				self.port_ip_dict[item['port']].add(item['ip'])
 
-			self.total_scans += len(self.port_dict)
+			self.total_scans += len(self.port_ip_dict)
 
 		self.limit = limit
 		self.raw_output = raw_output
 		if not self.raw_output:
 			Logger.print_info(f'Total scans -> {self.total_scans}')
 
 	@abstractmethod
@@ -102,32 +103,31 @@
 	def nmap_by_hosts(self, dns):
 		"""
 		Search DB by hosts and print mapping "live_host -> [open_ports]". No Nmap scan is launched.
 		
 		:param dns: a boolean flag which, when presented, indicates that domain names associated with corresponding IPs must be printed
 		:type dns: bool
 		"""
-		for ip, ports in sorted(self.ip_dict.items(), key=lambda x: socket.inet_aton(x[0])):
+		for ip, ports in sorted(self.ip_ports_dict.items(), key=lambda x: socket.inet_aton(x[0])):
 			if self.limit is not None and len(ports) >= self.limit:
 				continue
 
 			sorted_ports = sorted(ports)
 			if self.raw_output:
 				for port in sorted_ports:
 					print(f'{ip}:{port}')
 			elif dns:
-				domains = self.db.search(self.Host.ip == ip)[0]['domains']
-				domains = f'[{",".join(domains)}]'
+				domains = f'[{",".join(self.ip_domains_dict[ip])}]'
 				Logger.print_success(f'IP {ip}, Domains {domains} ({len(ports)}) -> [{",".join([str(p) for p in sorted_ports])}]')
 			else:
 				Logger.print_success(f'IP {ip} ({len(ports)}) -> [{",".join([str(p) for p in sorted_ports])}]')
 
 	def nmap_by_ports(self):
 		"""Search DB by ports and print mapping "open_port -> [live_hosts]". No Nmap scan is launched."""
-		for port, ip_list in sorted(self.port_dict.items()):
+		for port, ip_list in sorted(self.port_ip_dict.items()):
 			sorted_ip_list = ','.join(sorted(ip_list, key=socket.inet_aton))
 			if self.raw_output:
 				print(sorted_ip_list.replace(',', '\n'))
 			else:
 				Logger.print_success(f'Port {port} ({len(ip_list)}) -> [{sorted_ip_list}]')
 
 
@@ -140,15 +140,15 @@
 
 		:param nmap_opts: custom Nmap options that will replace the default ones
 		:type nmap_opts: str
 		:param parallel: namedtuple('Parallelism', 'enabled processes')
 		:type parallel: collections.namedtuple
 		"""
 		nmap_commands, i = [], 1
-		for ip, ports in sorted(self.ip_dict.items(), key=lambda x: socket.inet_aton(x[0])):
+		for ip, ports in sorted(self.ip_ports_dict.items(), key=lambda x: socket.inet_aton(x[0])):
 			if self.limit is not None and len(ports) >= self.limit:
 				continue
 
 			if not parallel.enabled:
 				Logger.print_separator(f'IP: {ip}', prefix=f'{i}/{self.total_scans}')
 
 			nmap_out = ip.replace('.', '-')
@@ -178,15 +178,15 @@
 
 		:param nmap_opts: custom Nmap options that will replace the default ones
 		:type nmap_opts: str
 		:param parallel: namedtuple('Parallelism', 'enabled processes')
 		:type parallel: collections.namedtuple
 		"""
 		nmap_commands, i = [], 1
-		for port, ip_list in sorted(self.port_dict.items()):
+		for port, ip_list in sorted(self.port_ip_dict.items()):
 			if not parallel.enabled:
 				Logger.print_separator(f'Port: {port}', prefix=f'{i}/{self.total_scans}')
 
 			nmap_out = f'port{port}'
 			with NamedTemporaryFile('w+') as tmp:
 				tmp.writelines(f'{i}\n' for i in ip_list)
 				tmp.seek(0)
```

### Comparing `divideandscan-0.3.7/pyproject.toml` & `divideandscan-0.3.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "divideandscan"
-version = "0.3.7"
+version = "0.3.8"
 description = "Divide full port scan results and use it for targeted Nmap runs"
 authors = ["Sam Freeside <snovvcrash@protonmail.ch>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 homepage = "https://github.com/snovvcrash/DivideAndScan"
 repository = "https://github.com/snovvcrash/DivideAndScan"
 keywords = ["pentest", "scan", "nmap", "masscan", "rustscan"]
```

### Comparing `divideandscan-0.3.7/PKG-INFO` & `divideandscan-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divideandscan
-Version: 0.3.7
+Version: 0.3.8
 Summary: Divide full port scan results and use it for targeted Nmap runs
 Home-page: https://github.com/snovvcrash/DivideAndScan
 License: BSD-2-Clause
 Keywords: pentest,scan,nmap,masscan,rustscan
 Author: Sam Freeside
 Author-email: snovvcrash@protonmail.ch
 Requires-Python: >=3.9,<3.12
@@ -33,15 +33,15 @@
 </p>
 
 <p align="center">
   <strong>Divide <strike>Et Impera</strike> And Scan (and also merge the scan results)</strong>
 </p>
 
 <p align="center">
-  <a href="https://github.com/snovvcrash/DivideAndScan/blob/main/pyproject.toml#L3"><img src="https://img.shields.io/badge/version-0.3.7-success" alt="version" /></a>
+  <a href="https://github.com/snovvcrash/DivideAndScan/blob/main/pyproject.toml#L3"><img src="https://img.shields.io/badge/version-0.3.8-success" alt="version" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/search?l=python"><img src="https://img.shields.io/badge/python-3.9-blue?logo=python&logoColor=white" alt="python" /></a>
   <a href="https://www.codacy.com/gh/snovvcrash/DivideAndScan/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=snovvcrash/DivideAndScan&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/35f0bdfece9846d7aab3888b01642813" alt="codacy" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-pypi.yml"><img src="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-pypi.yml/badge.svg" alt="pypi" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-docker-hub.yml"><img src="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-docker-hub.yml/badge.svg" alt="docker" /></a>
 </p>
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: divideandscan Version: 0.3.7 Summary: Divide full
+Metadata-Version: 2.1 Name: divideandscan Version: 0.3.8 Summary: Divide full
 port scan results and use it for targeted Nmap runs Home-page: https://
 github.com/snovvcrash/DivideAndScan License: BSD-2-Clause Keywords:
 pentest,scan,nmap,masscan,rustscan Author: Sam Freeside Author-email:
 snovvcrash@protonmail.ch Requires-Python: >=3.9,<3.12 Classifier: Environment
 :: Console Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

