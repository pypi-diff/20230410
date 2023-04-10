# Comparing `tmp/robust_serial-0.1.tar.gz` & `tmp/robust_serial-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robust_serial-0.1.tar", last modified: Sun Apr 15 17:48:50 2018, max compression
+gzip compressed data, was "robust_serial-0.2.tar", last modified: Mon Apr 10 17:17:21 2023, max compression
```

## Comparing `robust_serial-0.1.tar` & `robust_serial-0.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2018-04-15 17:48:50.000000 robust_serial-0.1/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      710 2018-04-15 17:48:50.000000 robust_serial-0.1/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1241 2018-04-15 17:48:31.000000 robust_serial-0.1/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2018-04-15 17:48:50.000000 robust_serial-0.1/robust_serial.egg-info/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2018-04-15 17:13:01.000000 robust_serial-0.1/robust_serial.egg-info/not-zip-safe
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      710 2018-04-15 17:48:50.000000 robust_serial-0.1/robust_serial.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       16 2018-04-15 17:48:50.000000 robust_serial-0.1/robust_serial.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       14 2018-04-15 17:48:50.000000 robust_serial-0.1/robust_serial.egg-info/top_level.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      343 2018-04-15 17:48:50.000000 robust_serial-0.1/robust_serial.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2018-04-15 17:48:50.000000 robust_serial-0.1/robust_serial.egg-info/dependency_links.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2018-04-15 17:48:50.000000 robust_serial-0.1/robust_serial/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2466 2018-03-10 17:43:02.000000 robust_serial-0.1/robust_serial/utils.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       49 2018-04-15 17:44:18.000000 robust_serial-0.1/robust_serial/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2720 2018-04-08 12:23:39.000000 robust_serial-0.1/robust_serial/robust_serial.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3297 2018-04-08 12:29:29.000000 robust_serial-0.1/robust_serial/threads.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      102 2018-04-15 17:48:50.000000 robust_serial-0.1/setup.cfg
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-10 17:17:21.472699 robust_serial-0.2/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1071 2018-06-06 19:45:27.000000 robust_serial-0.2/LICENSE
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      934 2023-04-10 17:17:21.472699 robust_serial-0.2/PKG-INFO
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     2649 2023-04-10 17:04:20.000000 robust_serial-0.2/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1057 2023-04-10 16:45:03.000000 robust_serial-0.2/pyproject.toml
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-10 17:17:21.472699 robust_serial-0.2/robust_serial/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)      394 2023-04-10 16:56:55.000000 robust_serial-0.2/robust_serial/__init__.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     2836 2023-04-10 16:54:27.000000 robust_serial-0.2/robust_serial/robust_serial.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     3234 2023-04-10 16:46:52.000000 robust_serial-0.2/robust_serial/threads.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     2448 2023-04-10 16:47:19.000000 robust_serial-0.2/robust_serial/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-10 17:17:21.472699 robust_serial-0.2/robust_serial.egg-info/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      934 2023-04-10 17:17:21.000000 robust_serial-0.2/robust_serial.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      391 2023-04-10 17:17:21.000000 robust_serial-0.2/robust_serial.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-10 17:17:21.000000 robust_serial-0.2/robust_serial.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-10 17:10:37.000000 robust_serial-0.2/robust_serial.egg-info/not-zip-safe
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      115 2023-04-10 17:17:21.000000 robust_serial-0.2/robust_serial.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       14 2023-04-10 17:17:21.000000 robust_serial-0.2/robust_serial.egg-info/top_level.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-10 17:17:21.472699 robust_serial-0.2/setup.cfg
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1384 2023-04-10 17:12:41.000000 robust_serial-0.2/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-10 17:17:21.472699 robust_serial-0.2/tests/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1141 2023-04-10 16:46:52.000000 robust_serial-0.2/tests/test_read_write.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `robust_serial-0.1/robust_serial/utils.py` & `robust_serial-0.2/robust_serial/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,80 @@
-from __future__ import print_function, division, absolute_import
-
-import sys
 import glob
-
-try:
-    import queue
-except ImportError:
-    import Queue as queue
+import queue
+import sys
+from typing import List, Optional
 
 import serial
 
 
 # From https://stackoverflow.com/questions/6517953/clear-all-items-from-the-queue
 class CustomQueue(queue.Queue):
     """
     A custom queue subclass that provides a :meth:`clear` method.
     """
 
-    def clear(self):
+    def clear(self) -> None:
         """
         Clears all items from the queue.
         """
 
         with self.mutex:
             unfinished = self.unfinished_tasks - len(self.queue)
             if unfinished <= 0:
                 if unfinished < 0:
-                    raise ValueError('task_done() called too many times')
+                    raise ValueError("task_done() called too many times")
                 self.all_tasks_done.notify_all()
             self.unfinished_tasks = unfinished
             self.queue.clear()
             self.not_full.notify_all()
 
 
 # From https://stackoverflow.com/questions/12090503/listing-available-com-ports-with-python
-def get_serial_ports():
+def get_serial_ports() -> List[str]:
     """
-    Lists serial ports
-    :return: [str] A list of available serial ports
+    Lists serial ports.
+
+
+    :return: A list of available serial ports
     """
-    if sys.platform.startswith('win'):
-        ports = ['COM%s' % (i + 1) for i in range(256)]
-    elif sys.platform.startswith('linux') or sys.platform.startswith('cygwin'):
+    if sys.platform.startswith("win"):
+        ports = ["COM%s" % (i + 1) for i in range(256)]
+    elif sys.platform.startswith("linux") or sys.platform.startswith("cygwin"):
         # this excludes your current terminal "/dev/tty"
-        ports = glob.glob('/dev/tty[A-Za-z]*')
-    elif sys.platform.startswith('darwin'):
-        ports = glob.glob('/dev/tty.*')
+        ports = glob.glob("/dev/tty[A-Za-z]*")
+    elif sys.platform.startswith("darwin"):
+        ports = glob.glob("/dev/tty.*")
     else:
-        raise EnvironmentError('Unsupported platform')
+        raise OSError("Unsupported platform")
 
     results = []
     for port in ports:
         try:
             s = serial.Serial(port)
             s.close()
             results.append(port)
         except (OSError, serial.SerialException):
             pass
     return results
 
 
-def open_serial_port(serial_port=None, baudrate=115200, timeout=0, write_timeout=0):
+def open_serial_port(
+    serial_port: Optional[str] = None,
+    baudrate: int = 115200,
+    timeout: Optional[int] = 0,
+    write_timeout: int = 0,
+) -> serial.Serial:
     """
     Try to open serial port with Arduino
     If not port is specified, it will be automatically detected
-    :param serial_port: (str)
-    :param baudrate: (int)
-    :param timeout: (int) None -> blocking mode
-    :param write_timeout: (int)
+
+    :param serial_port:
+    :param baudrate:
+    :param timeout: None -> blocking mode
+    :param write_timeout:
     :return: (Serial Object)
     """
     # Open serial port (for communication with Arduino)
     if serial_port is None:
         serial_port = get_serial_ports()[0]
     # timeout=0 non-blocking mode, return immediately in any case, returning zero or more,
     # up to the requested number of bytes
```

### Comparing `robust_serial-0.1/robust_serial/robust_serial.py` & `robust_serial-0.2/robust_serial/robust_serial.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,118 +1,122 @@
-from __future__ import print_function, division, unicode_literals, absolute_import
-
 import struct
-
 from enum import Enum
+from typing import BinaryIO
 
 
 class Order(Enum):
+    """
+    Pre-defined orders
+    """
+
     HELLO = 0
     SERVO = 1
     MOTOR = 2
     ALREADY_CONNECTED = 3
     ERROR = 4
     RECEIVED = 5
     STOP = 6
 
-def read_order(f):
+
+def read_order(f: BinaryIO) -> Order:
     """
     :param f: file handler or serial file
     :return: (Order Enum Object)
     """
     return Order(read_i8(f))
 
-def read_i8(f):
+
+def read_i8(f: BinaryIO) -> Order:
     """
     :param f: file handler or serial file
     :return: (int8_t)
     """
-    return struct.unpack('<b', bytearray(f.read(1)))[0]
+    return struct.unpack("<b", bytearray(f.read(1)))[0]
 
 
-def read_i16(f):
+def read_i16(f: BinaryIO) -> Order:
     """
     :param f: file handler or serial file
     :return: (int16_t)
     """
-    return struct.unpack('<h', bytearray(f.read(2)))[0]
+    return struct.unpack("<h", bytearray(f.read(2)))[0]
 
 
 def read_i32(f):
     """
     :param f: file handler or serial file
     :return: (int32_t)
     """
-    return struct.unpack('<l', bytearray(f.read(4)))[0]
+    return struct.unpack("<l", bytearray(f.read(4)))[0]
 
 
-def write_i8(f, value):
+def write_i8(f: BinaryIO, value: int) -> None:
     """
     :param f: file handler or serial file
     :param value: (int8_t)
     """
     if -128 <= value <= 127:
-        f.write(struct.pack('<b', value))
+        f.write(struct.pack("<b", value))
     else:
-        print("Value error:{}".format(value))
+        print(f"Value error:{value}")
 
 
-def write_order(f, order):
+def write_order(f: BinaryIO, order: Order) -> None:
     """
     :param f: file handler or serial file
     :param order: (Order Enum Object)
     """
     write_i8(f, order.value)
 
 
-def write_i16(f, value):
+def write_i16(f: BinaryIO, value: int) -> None:
     """
     :param f: file handler or serial file
     :param value: (int16_t)
     """
-    f.write(struct.pack('<h', value))
+    f.write(struct.pack("<h", value))
 
 
-def write_i32(f, value):
+def write_i32(f: BinaryIO, value: int) -> None:
     """
     :param f: file handler or serial file
     :param value: (int32_t)
     """
-    f.write(struct.pack('<l', value))
+    f.write(struct.pack("<l", value))
 
 
-def decode_order(f, byte, debug=False):
+def decode_order(f: BinaryIO, byte: int, debug: bool = False) -> None:
     """
     :param f: file handler or serial file
     :param byte: (int8_t)
     :param debug: (bool) whether to print or not received messages
     """
     try:
         order = Order(byte)
         if order == Order.HELLO:
             msg = "HELLO"
         elif order == Order.SERVO:
             angle = read_i16(f)
             # Bit representation
             # print('{0:016b}'.format(angle))
-            msg = "SERVO {}".format(angle)
+            msg = f"SERVO {angle}"
         elif order == Order.MOTOR:
             speed = read_i8(f)
-            msg = "motor {}".format(speed)
+            msg = f"motor {speed}"
         elif order == Order.ALREADY_CONNECTED:
             msg = "ALREADY_CONNECTED"
         elif order == Order.ERROR:
             error_code = read_i16(f)
-            msg = "Error {}".format(error_code)
+            msg = f"Error {error_code}"
         elif order == Order.RECEIVED:
             msg = "RECEIVED"
         elif order == Order.STOP:
             msg = "STOP"
         else:
             msg = ""
             print("Unknown Order", byte)
 
         if debug:
             print(msg)
     except Exception as e:
-        print("Error decoding order {}: {}".format(byte, e))
-        print('byte={0:08b}'.format(byte))
+        print(f"Error decoding order {byte}: {e}")
+        print(f"byte={byte:08b}")
```

### Comparing `robust_serial-0.1/robust_serial/threads.py` & `robust_serial-0.2/robust_serial/threads.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from __future__ import print_function, division, absolute_import
-
 import threading
 import time
 
 import serial
 
-from .robust_serial import write_order, Order, write_i8, write_i16, decode_order
+from .robust_serial import Order, decode_order, write_i8, write_i16, write_order
 from .utils import queue
 
 rate = 1 / 2000  # 2000 Hz (limit the rate of communication with the arduino)
 
 
 class CommandThread(threading.Thread):
     """
     Thread that send orders to the arduino
-    it blocks if there no more send_token left (here it is the n_received_semaphore)
+    it blocks if there no more send_token left (here it is the n_received_semaphore).
+
     :param serial_file: (Serial object)
     :param command_queue: (Queue)
     :param exit_event: (Threading.Event object)
     :param n_received_semaphore: (threading.Semaphore)
     :param serial_lock: (threading.Lock)
     """
 
@@ -54,14 +53,15 @@
         print("Command Thread Exited")
 
 
 class ListenerThread(threading.Thread):
     """
     Thread that listen to the Arduino
     It is used to add send_tokens to the n_received_semaphore
+
     :param serial_file: (Serial object)
     :param exit_event: (threading.Event object)
     :param n_received_semaphore: (threading.Semaphore)
     :param serial_lock: (threading.Lock)
     """
 
     def __init__(self, serial_file, exit_event, n_received_semaphore, serial_lock):
```

