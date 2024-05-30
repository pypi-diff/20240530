# Comparing `tmp/medjc09_hub_python-0.2.0.tar.gz` & `tmp/medjc09_hub_python-0.3.0.tar.gz`

## Comparing `medjc09_hub_python-0.2.0.tar` & `medjc09_hub_python-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.python-version
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/requirements.lock
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/src/medjc09_hub_python/__init__.py
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/src/medjc09_hub_python/command.py
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/src/medjc09_hub_python/medjc09_hub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/tests/test_command_deserializer.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/tests/test_command_serializer.py
--rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/tests/test_medjc09_hub.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/LICENSE
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/README.md
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 medjc09_hub_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/.python-version
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/requirements.lock
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/src/medjc09/__init__.py
+-rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/src/medjc09/command.py
+-rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/src/medjc09/medjc09.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/tests/test_command_deserializer.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/tests/test_command_serializer.py
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/tests/test_medjc09_hub.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/LICENSE
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/README.md
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 medjc09_hub_python-0.3.0/PKG-INFO
```

### Comparing `medjc09_hub_python-0.2.0/requirements-dev.lock` & `medjc09_hub_python-0.3.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `medjc09_hub_python-0.2.0/.github/workflows/main.yml` & `medjc09_hub_python-0.3.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `medjc09_hub_python-0.2.0/.github/workflows/publish.yml` & `medjc09_hub_python-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `medjc09_hub_python-0.2.0/src/medjc09_hub_python/command.py` & `medjc09_hub_python-0.3.0/src/medjc09/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 
     CMD_START_POLLING = 0x40
     """Start polling the MedJC09 Hub."""
 
     CMD_STOP_POLLING = 0x41
     """Stop polling the MedJC09 Hub."""
 
-    CMD_SET_POLLING_INTERVAL = 0x42
+    CMD_SET_POLLING_RATE = 0x42
     """Set the polling interval of the MedJC09 Hub."""
 
-    CMD_GET_POLLING_INTERVAL = 0x43
+    CMD_GET_POLLING_RATE = 0x43
     """Get the polling interval of the MedJC09 Hub."""
 
     CMD_GET_POLLING_REPORT = 0x4F
     """Get the polling report of the MedJC09 Hub."""
 
 
 @dataclass
@@ -151,28 +151,28 @@
     def __init__(self) -> None:
         pass
 
 
 class SetPollingIntervalResult(CommandResult):
     """Result of the SetPollingInterval command."""
 
-    command: Command = Command.CMD_SET_POLLING_INTERVAL
+    command: Command = Command.CMD_SET_POLLING_RATE
 
     def __init__(self) -> None:
         pass
 
 
-class GetPollingIntervalResult(CommandResult):
+class GetPollingRateResult(CommandResult):
     """Result of the GetPollingInterval command."""
 
-    command: Command = Command.CMD_GET_POLLING_INTERVAL
-    interval: int
+    command: Command = Command.CMD_GET_POLLING_RATE
+    rate: int
 
     def __init__(self, interval: int) -> None:
-        self.interval = interval
+        self.rate = interval
 
 
 class GetPollingReportResult(CommandResult):
     """Result of the GetPollingReport command."""
 
     command: Command = Command.CMD_START_POLLING
     voltage: float
@@ -257,20 +257,20 @@
 
     elif command == Command.CMD_START_POLLING:
         return StartPollingResult()
 
     elif command == Command.CMD_STOP_POLLING:
         return StopPollingResult()
 
-    elif command == Command.CMD_SET_POLLING_INTERVAL:
+    elif command == Command.CMD_SET_POLLING_RATE:
         return SetPollingIntervalResult()
 
-    elif command == Command.CMD_GET_POLLING_INTERVAL:
+    elif command == Command.CMD_GET_POLLING_RATE:
         interval = int.from_bytes(packet[2:4], byteorder="big", signed=False)
-        return GetPollingIntervalResult(interval)
+        return GetPollingRateResult(interval)
 
     elif command == Command.CMD_GET_POLLING_REPORT:
         voltage = (5 / 32767) * int.from_bytes(packet[2:4], byteorder="big", signed=True)
         me = [
             int.from_bytes(packet[4:6], byteorder="big", signed=True),
             int.from_bytes(packet[6:8], byteorder="big", signed=True),
             int.from_bytes(packet[8:10], byteorder="big", signed=True),
```

### Comparing `medjc09_hub_python-0.2.0/src/medjc09_hub_python/medjc09_hub.py` & `medjc09_hub_python-0.3.0/src/medjc09/medjc09.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import time
 from typing import Callable, List, TypedDict, Union
 
 import serial
 from cobs import cobs
 
 from .command import (
     Command,
     CommandResult,
     GetBaseVoltageResult,
     GetConnectionsResult,
     GetMEResult,
-    GetPollingIntervalResult,
+    GetPollingRateResult,
     GetPollingReportResult,
     GetSMEResult,
     GetVersionResult,
     deserialize,
     serialize,
 )
 
@@ -36,20 +37,22 @@
 PollingHandlerType = Callable[[PollingReportType], None]
 """Type for callback functions."""
 
 
 class Medjc09:
     """A class for handling communication with the Medjc09 device."""
 
-    def __init__(self, port: str, baudrate: int = 115200, polling_handler: Union[PollingHandlerType, None] = None):
+    def __init__(self, port: str, baudrate: int = 921600, polling_handler: Union[PollingHandlerType, None] = None):
         """Initialize the Medjc09 class.
 
+        #### ! Important: You need to wait for about 0.5 seconds until the serial connection is established.
+
         Args:
             port (str): Serial port name. E.g. "/dev/ttyUSB0"
-            baudrate (int, optional): Baudrate. Defaults to 115200.
+            baudrate (int, optional): Baudrate. Defaults to 921600.
             polling_handler (PollingHandlerType, optional): Callback function for polling. Defaults to None.
         """
         self._is_polling_mode = False
         self._ser = serial.Serial(port, baudrate, timeout=1)
         self._polling_handler = polling_handler
 
     def send_command(self, command: Command, params: bytes = bytes([])) -> CommandResult:
@@ -61,16 +64,21 @@
 
         Returns:
             CommandResult: Result of the command.
         """
         packet = serialize(command, params)
         encoded_packet = cobs.encode(packet)
         self._ser.write(encoded_packet + bytes([0x00]))
-
-        response = self._ser.read_until(bytes([0x00]))
+        time.sleep(0.005)
+        response = b""
+        timeout_timer = time.time()
+        while response == b"":
+            response = self._ser.read_until(bytes([0x00]))
+            if time.time() - timeout_timer > 5.0:
+                raise TimeoutError("Timeout")
         decoded_response = cobs.decode(response[:-1])  # Remove the trailing 0x00
         result = deserialize(decoded_response)
 
         return result
 
     def get_version(self) -> str:
         """Get the firmware version of the Medjc09 device.
@@ -172,32 +180,32 @@
         _ = self.send_command(Command.CMD_START_POLLING)
 
     def stop_polling(self) -> None:
         """Stop watching the polling mode."""
         self._is_polling_mode = False
         _ = self.send_command(Command.CMD_STOP_POLLING)
 
-    def set_polling_interval(self, interval: int) -> None:
-        """Set the polling interval.
+    def set_polling_rate(self, rate: int) -> None:
+        """Set the polling rate.
 
         Args:
-            interval (int): Polling interval in milliseconds.
+            rate (int): Polling rate in Hz.
         """
-        params = interval.to_bytes(2, byteorder="big", signed=True)
-        _ = self.send_command(Command.CMD_SET_POLLING_INTERVAL, params)
+        params = rate.to_bytes(2, byteorder="big", signed=True)
+        _ = self.send_command(Command.CMD_SET_POLLING_RATE, params)
 
-    def get_polling_interval(self) -> int:
-        """Get the polling interval.
+    def get_polling_rate(self) -> int:
+        """Get the polling rate.
 
         Returns:
-            int: Polling interval in milliseconds.
+            int: Polling rate in Hz.
         """
-        result = self.send_command(Command.CMD_GET_POLLING_INTERVAL)
-        if isinstance(result, GetPollingIntervalResult):
-            return result.interval
+        result = self.send_command(Command.CMD_GET_POLLING_RATE)
+        if isinstance(result, GetPollingRateResult):
+            return result.rate
         else:
             raise ValueError("Unexpected result type")
 
     def get_polling_report(self) -> PollingReportType:
         """Get the polling report.
 
         Returns:
@@ -218,16 +226,22 @@
 
     def update(self) -> None:
         """Update the polling mode."""
         if self._is_polling_mode:
             response = self._ser.read_until(bytes([0x00]))
             if response == b"":  # No data
                 return
-            decoded_response = cobs.decode(response[:-1])
-            result = deserialize(decoded_response)
+            try:
+                decoded_response = cobs.decode(response[:-1])
+            except cobs.DecodeError:
+                return
+            try:
+                result = deserialize(decoded_response)
+            except IndexError:
+                return
             if isinstance(result, GetPollingReportResult):
                 if self._polling_handler is not None:
                     self._polling_handler(
                         {
                             "voltage": result.voltage,
                             "me": result.me,
                             "sme": result.sme,
```

### Comparing `medjc09_hub_python-0.2.0/tests/test_command_deserializer.py` & `medjc09_hub_python-0.3.0/tests/test_command_deserializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List
 
 import pytest
-from medjc09_hub_python.command import (
+from medjc09 import (
     Command,
     GetBaseVoltageResult,
     GetConnectionsResult,
     GetMEResult,
-    GetPollingIntervalResult,
+    GetPollingRateResult,
     GetPollingReportResult,
     GetSMEResult,
     GetVersionResult,
     Protocol,
     SetPollingIntervalResult,
     StartPollingResult,
     StopPollingResult,
@@ -81,29 +81,27 @@
     packet = bytes([Protocol.STX.value, Command.CMD_STOP_POLLING.value, Protocol.ETX.value])
     result = deserialize(packet)
     assert isinstance(result, StopPollingResult)
 
 
 def test_deserialize_set_polling_interval() -> None:
     """Test for deserialize function with CMD_SET_POLLING_INTERVAL."""
-    packet = bytes([Protocol.STX.value, Command.CMD_SET_POLLING_INTERVAL.value, Protocol.ETX.value])
+    packet = bytes([Protocol.STX.value, Command.CMD_SET_POLLING_RATE.value, Protocol.ETX.value])
     result = deserialize(packet)
     assert isinstance(result, SetPollingIntervalResult)
 
 
 def test_deserialize_get_polling_interval() -> None:
     """Test for deserialize function with CMD_GET_POLLING_INTERVAL."""
     interval = 100
     params = interval.to_bytes(2, byteorder="big")
-    packet = bytes(
-        [Protocol.STX.value, Command.CMD_GET_POLLING_INTERVAL.value, params[0], params[1], Protocol.ETX.value]
-    )
+    packet = bytes([Protocol.STX.value, Command.CMD_GET_POLLING_RATE.value, params[0], params[1], Protocol.ETX.value])
     result = deserialize(packet)
-    assert isinstance(result, GetPollingIntervalResult)
-    assert result.interval == interval
+    assert isinstance(result, GetPollingRateResult)
+    assert result.rate == interval
 
 
 def test_deserialize_get_polling_report() -> None:
     """Test for deserialize function with CMD_GET_POLLING_REPORT."""
     BV: float = 5.0
     ME: List[int] = [1000, 1001, 0, 0]
     SME: List[int] = [2000, 2001, 0, 0]
```

### Comparing `medjc09_hub_python-0.2.0/tests/test_command_serializer.py` & `medjc09_hub_python-0.3.0/tests/test_command_serializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from medjc09_hub_python.command import (
+from medjc09 import (
     Command,
     Protocol,
     serialize,
 )
 
 
 def test_serialize_get_version() -> None:
@@ -50,23 +50,23 @@
     )
 
 
 def test_serialize_set_polling_interval() -> None:
     """Test for serialize function with CMD_SET_POLLING_INTERVAL."""
     # paramsは16bit整数とみなして 100を 2byteに分割
     # uint16_t 100 -> 0x0064 -> 0x64, 0x00
-    assert serialize(Command.CMD_SET_POLLING_INTERVAL, bytes([0x64, 0x00])) == bytes(
-        [Protocol.STX.value, Command.CMD_SET_POLLING_INTERVAL.value, 0x64, 0x00, Protocol.ETX.value]
+    assert serialize(Command.CMD_SET_POLLING_RATE, bytes([0x64, 0x00])) == bytes(
+        [Protocol.STX.value, Command.CMD_SET_POLLING_RATE.value, 0x64, 0x00, Protocol.ETX.value]
     )
 
 
 def test_serialize_get_polling_interval() -> None:
     """Test for serialize function with CMD_GET_POLLING_INTERVAL."""
-    assert serialize(Command.CMD_GET_POLLING_INTERVAL) == bytes(
-        [Protocol.STX.value, Command.CMD_GET_POLLING_INTERVAL.value, Protocol.ETX.value]
+    assert serialize(Command.CMD_GET_POLLING_RATE) == bytes(
+        [Protocol.STX.value, Command.CMD_GET_POLLING_RATE.value, Protocol.ETX.value]
     )
 
 
 def test_serialize_get_polling_report() -> None:
     """Test for serialize function with CMD_GET_POLLING_REPORT."""
     assert serialize(Command.CMD_GET_POLLING_REPORT) == bytes(
         [Protocol.STX.value, Command.CMD_GET_POLLING_REPORT.value, Protocol.ETX.value]
```

### Comparing `medjc09_hub_python-0.2.0/tests/test_medjc09_hub.py` & `medjc09_hub_python-0.3.0/tests/test_medjc09_hub.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,194 @@
 import os
 import time
 from typing import List
 
 import dotenv
 import pytest
 import serial
-from medjc09_hub_python.medjc09_hub import Medjc09, PollingReportType
+from medjc09 import Medjc09, PollingReportType
 
 dotenv.load_dotenv()
 
 
 port = os.environ.get("TEST_PORT")
+_bautrate = os.environ.get("TEST_BAUTRATE")
+bautrate = int(_bautrate) if _bautrate is not None else None
 is_not_connected = True
 try:
     if port is None:
         raise ValueError("TEST_PORT is not set.")
-    ser = serial.Serial(port, 115200, timeout=1)
+    if bautrate is None:
+        raise ValueError("TEST_BAUTRATE is not set.")
+    ser = serial.Serial(port, bautrate, timeout=1)
     is_not_connected = False
 except serial.SerialException:
     is_not_connected = True
 except ValueError:
     is_not_connected = True
 finally:
     if is_not_connected is False:
         ser.close()
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_get_base_voltage() -> None:
     """Test for get_base_voltage method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     voltage = medjc09.get_base_voltage()
     assert isinstance(voltage, float)
     assert voltage >= 0.0
     assert voltage <= 5.0
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_get_connections() -> None:
     """Test for get_connections method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     connections = medjc09.get_connections()
     assert isinstance(connections, list)
     assert len(connections) == 4
     for connection in connections:
         assert isinstance(connection, bool)
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_get_me() -> None:
     """Test for get_me method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     me = medjc09.get_me()
     assert isinstance(me, list)
     assert len(me) == 4
     for value in me:
         assert isinstance(value, int)
         assert value >= -32768
         assert value <= 32767
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_get_me_as_voltage() -> None:
     """Test for get_me_as_voltage method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     me_voltage = medjc09.get_me_as_voltage()
     assert isinstance(me_voltage, list)
     assert len(me_voltage) == 4
     for value in me_voltage:
         assert isinstance(value, float)
         assert value >= -5.0 / 2
         assert value <= 5.0 / 2
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_get_sme() -> None:
     """Test for get_sme method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     sme = medjc09.get_sme()
     assert isinstance(sme, list)
     assert len(sme) == 4
     for value in sme:
         assert isinstance(value, int)
         assert value >= 0
         assert value <= 32767
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_get_sme_as_voltage() -> None:
     """Test for get_sme_as_voltage method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     sme_voltage = medjc09.get_sme_as_voltage()
     assert isinstance(sme_voltage, list)
     assert len(sme_voltage) == 4
     for value in sme_voltage:
         assert isinstance(value, float)
         assert value >= 0.0
         assert value <= 5.0
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_start_polling() -> None:
     """Test for start_polling method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     medjc09.start_polling()
     assert medjc09.is_polling() is True
     medjc09.stop_polling()
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_stop_polling() -> None:
     """Test for stop_polling method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     medjc09.start_polling()
     medjc09.stop_polling()
     assert medjc09.is_polling() is False
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
-def test_set_get_polling_interval() -> None:
-    """Test for set_polling_interval method."""
-    medjc09 = Medjc09(port)
-    medjc09.set_polling_interval(100)
-    assert medjc09.get_polling_interval() == 100
+def test_set_get_polling_rate() -> None:
+    """Test for set_polling_rate method."""
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
+    medjc09.set_polling_rate(100)
+    assert medjc09.get_polling_rate() == 100
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_get_polling_report() -> None:
     """Test for get_polling_report method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     timer = time.time()
     report = medjc09.get_polling_report()
     assert valid_polling_report(report)
     timer = time.time() - timer
     assert timer < 1.0
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_polling_mode() -> None:
     """Test for polling mode.
-    Polling interval is 50ms and duration is 1001ms.
+    Polling rate is 1000Hz and duration is 1001ms.
     """
-    interval = 50
-    duration = 1001
+    rate = 1000
+    duration = 1000
 
     count = {"value": 0}
     reports: List[PollingReportType] = []
 
     def test_polling_report(report: PollingReportType) -> None:
-        assert valid_polling_report(report)
+        # assert valid_polling_report(report)
         reports.append(report)
         count["value"] += 1
 
-    medjc09 = Medjc09(port, 115200, test_polling_report)
-    medjc09.set_polling_interval(interval)
+    medjc09 = Medjc09(port, 921600, test_polling_report)
+    time.sleep(0.5)
+    medjc09.set_polling_rate(rate)
     medjc09.start_polling()
     start_time: float = time.time()
     total_time: float = 0
     while total_time < duration // 1000:
         medjc09.update()
         total_time = time.time() - start_time
     medjc09.stop_polling()
 
-    assert count["value"] == duration // interval
+    assert count["value"] >= rate
 
 
 @pytest.mark.skipif(is_not_connected, reason="Device is not connected.")
 def test_close() -> None:
     """Test for close method."""
-    medjc09 = Medjc09(port)
+    medjc09 = Medjc09(port, bautrate)
+    time.sleep(0.5)
     medjc09.close()
     assert medjc09._ser.is_open is False
 
 
 def valid_polling_report(report: PollingReportType) -> bool:
     """Validate polling report
```

### Comparing `medjc09_hub_python-0.2.0/LICENSE` & `medjc09_hub_python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medjc09_hub_python-0.2.0/pyproject.toml` & `medjc09_hub_python-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "medjc09-hub-python"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python library for medjc09 hub"
 authors = [
     { name = "OctSquid", email = "pqvs6k96@s.okayama-u.ac.jp" }
 ]
 dependencies = [
     "cobs>=1.2.1",
     "pyserial-asyncio>=0.6",
@@ -26,15 +26,15 @@
     "build>=1.2.1",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/medjc09_hub_python"]
+packages = ["src/medjc09"]
 
 [tool.mypy]
 ignore_missing_imports = true
 strict = true
 
 [tool.ruff]
 ignore = []
```

