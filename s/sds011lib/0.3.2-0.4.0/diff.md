# Comparing `tmp/sds011lib-0.3.2.tar.gz` & `tmp/sds011lib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sds011lib-0.3.2.tar", max compression
+gzip compressed data, was "sds011lib-0.4.0.tar", max compression
```

## Comparing `sds011lib-0.3.2.tar` & `sds011lib-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-14 18:45:11.075500 sds011lib-0.3.2/LICENSE
--rw-r--r--   0        0        0     1163 2023-05-14 18:45:11.075500 sds011lib-0.3.2/README.md
--rw-r--r--   0        0        0      977 2023-05-14 18:45:11.075500 sds011lib-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    26710 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/_constants.py
--rw-r--r--   0        0        0     2332 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/py.typed
--rw-r--r--   0        0        0     1974 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/responses.py
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 sds011lib-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-16 05:25:01.355119 sds011lib-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1163 2023-05-16 05:25:01.355119 sds011lib-0.4.0/README.md
+-rw-r--r--   0        0        0      977 2023-05-16 05:25:01.359119 sds011lib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    28367 2023-05-16 05:25:01.359119 sds011lib-0.4.0/sds011lib/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-16 05:25:01.359119 sds011lib-0.4.0/sds011lib/_constants.py
+-rw-r--r--   0        0        0     2943 2023-05-16 05:25:01.359119 sds011lib-0.4.0/sds011lib/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:25:01.359119 sds011lib-0.4.0/sds011lib/py.typed
+-rw-r--r--   0        0        0     1974 2023-05-16 05:25:01.359119 sds011lib-0.4.0/sds011lib/responses.py
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 sds011lib-0.4.0/PKG-INFO
```

### Comparing `sds011lib-0.3.2/LICENSE` & `sds011lib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.2/README.md` & `sds011lib-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.2/pyproject.toml` & `sds011lib-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sds011lib"
-version = "0.3.2"
+version = "0.4.0"
 description = "SDS011 Library"
 authors = ["Tim Orme <TimothyOrme@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyserial = "^3.5"
```

### Comparing `sds011lib-0.3.2/sds011lib/__init__.py` & `sds011lib-0.4.0/sds011lib/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,18 +35,20 @@
 )
 from .exceptions import (
     IncompleteReadException,
     IncorrectCommandException,
     IncorrectCommandCodeException,
     ChecksumFailedException,
     IncorrectWrapperException,
+    MissingResponseException,
 )
 
-from typing import Protocol, Union, Optional, runtime_checkable
+from typing import Protocol, Union, Optional, runtime_checkable, Generator
 from dataclasses import dataclass
+from contextlib import contextmanager
 
 # We lift this out of the private constants module, since its part of the contracts as defaults, and users might want to
 # leverage it.
 ALL_SENSORS: bytes = ALL_SENSOR_ID
 
 
 @runtime_checkable
@@ -87,49 +89,197 @@
     device_id: bytes
     checksum: int
     tail: bytes
     expected_command_code: Command
     expected_response_type: ResponseType
 
 
+def _calc_checksum(data: bytes) -> int:
+    """Calculate the checksum for the read data."""
+    return sum(d for d in data) % 256
+
+
+def _verify_read_response(read_response: _RawReadResponse) -> None:
+    """Verify read data.
+
+    Args:
+        read_response: The raw read data to verify.
+
+    Raises:
+        IncorrectWrapperException: If the head or tail data is incorrect
+        ChecksumFailedException: If the checksum from the response is incorrect
+        IncorrectCommandException: If the command ID in the response is not the expected one.
+        IncorrectCommandCodeException: If the command code in the response is not the expected one.
+    """
+    if read_response.head != HEAD:
+        raise IncorrectWrapperException()
+    if read_response.tail != TAIL:
+        raise IncorrectWrapperException()
+    if read_response.checksum != _calc_checksum(read_response.payload):
+        raise ChecksumFailedException(
+            expected=read_response.checksum,
+            actual=_calc_checksum(read_response.payload),
+        )
+    if read_response.cmd_id != read_response.expected_response_type.value:
+        raise IncorrectCommandException(
+            expected=read_response.expected_response_type.value,
+            actual=read_response.cmd_id,
+        )
+
+    # Query responses don't validate the command code
+    if (
+        read_response.expected_response_type != ResponseType.QUERY_RESPONSE
+        and bytes([read_response.payload[0]])
+        != read_response.expected_command_code.value
+    ):
+        raise IncorrectCommandCodeException(
+            expected=read_response.expected_command_code.value,
+            actual=read_response.payload[0:1],
+        )
+
+
+def _parse_read_response(
+    data: bytes,
+    command_code: Command,
+    response_type: ResponseType = ResponseType.GENERAL_RESPONSE,
+) -> _RawReadResponse:
+    """Parse bytes into a typed read response. Validates as well.
+
+    Args:
+        data: The raw data bytes to parse.  Must be of length 10.
+        command_code: The expected command code for the response.
+        response_type:  The expected response type for the response.
+
+    Returns:
+        A read response object with the parsed data.
+    """
+    if len(data) != 10:
+        raise IncompleteReadException()
+
+    head: bytes = data[0:1]
+    cmd_id: bytes = data[1:2]
+    payload: bytes = data[2:8]
+    device_id: bytes = data[6:8]
+    checksum: int = data[8]
+    tail: bytes = data[9:10]
+    expected_command_code: Command = command_code
+    expected_response_type: ResponseType = response_type
+    result = _RawReadResponse(
+        head=head,
+        cmd_id=cmd_id,
+        payload=payload,
+        device_id=device_id,
+        checksum=checksum,
+        tail=tail,
+        expected_command_code=expected_command_code,
+        expected_response_type=expected_response_type,
+    )
+    _verify_read_response(result)
+    return result
+
+
+def _parse_query_response(data: bytes) -> QueryResponse:
+    """Parse a query read response."""
+    raw_response = _parse_read_response(
+        data, Command.QUERY, ResponseType.QUERY_RESPONSE
+    )
+
+    pm25: float = int.from_bytes(raw_response.payload[0:2], byteorder="little") / 10
+    pm10: float = int.from_bytes(raw_response.payload[2:4], byteorder="little") / 10
+    return QueryResponse(pm25=pm25, pm10=pm10, device_id=raw_response.device_id)
+
+
+def _parse_reporting_mode_response(data: bytes) -> ReportingModeResponse:
+    """Parse a reporting mode response."""
+    raw_response = _parse_read_response(data, command_code=Command.SET_REPORTING_MODE)
+    operation_type: OperationType = OperationType(raw_response.payload[1:2])
+    state: ReportingMode = ReportingMode(raw_response.payload[2:3])
+    return ReportingModeResponse(operation_type, state)
+
+
+def _parse_device_id_response(data: bytes) -> DeviceIdResponse:
+    """Parse a device ID response."""
+    raw_response = _parse_read_response(data, command_code=Command.SET_DEVICE_ID)
+    return DeviceIdResponse(device_id=raw_response.device_id)
+
+
+def _parse_sleep_wake_response(data: bytes) -> SleepWakeReadResponse:
+    """Parse a sleep/wake response."""
+    raw_response = _parse_read_response(data, command_code=Command.SET_SLEEP)
+    operation_type: OperationType = OperationType(raw_response.payload[1:2])
+    state: SleepState = SleepState(raw_response.payload[2:3])
+    return SleepWakeReadResponse(operation_type=operation_type, state=state)
+
+
+def _parse_working_period_reponse(data: bytes) -> WorkingPeriodReadResponse:
+    """Parse a working period response."""
+    raw_response = _parse_read_response(data, command_code=Command.SET_WORKING_PERIOD)
+    operation_type: OperationType = OperationType(raw_response.payload[1:2])
+    interval: int = raw_response.payload[2]
+    return WorkingPeriodReadResponse(operation_type=operation_type, interval=interval)
+
+
+def _parse_firmware_response(data: bytes) -> CheckFirmwareResponse:
+    """Parse a firmware response."""
+    raw_response = _parse_read_response(
+        data, command_code=Command.CHECK_FIRMWARE_VERSION
+    )
+    year: int = raw_response.payload[1]
+    month: int = raw_response.payload[2]
+    day: int = raw_response.payload[3]
+    return CheckFirmwareResponse(year=year, month=month, day=day)
+
+
 class SDS011Reader:
     """NOVA PM SDS011 Reader."""
 
-    def __init__(self, ser_dev: Union[str, SerialLike], send_command_sleep: int = 1):
+    def __init__(
+        self,
+        ser_dev: Union[str, SerialLike],
+        send_command_sleep: int = 1,
+        max_loop_count: int = 30,
+    ):
         """Create a basic device.
 
         This is mostly a low level implementation. For practical purposes, most users will want to use the
         SDS011QueryReader or SDS011ActiveReader.  This implementation would only be useful for very special cases, and
         serves as the base class for the other reader implementations anyways.
 
         Args:
             ser_dev: A path to a serial device, or an instance of serial.Serial.
             send_command_sleep: The number of seconds to sleep after sending a command to the device.
+            max_loop_count: The maximum number of reads to search through to find a desired response command.
         """
         if isinstance(ser_dev, str):
             self.ser: SerialLike = serial.Serial(ser_dev, timeout=2)
         elif isinstance(ser_dev, SerialLike):
             self.ser = ser_dev
         else:
             raise AttributeError("ser_dev must be a string or Serial-like object.")
         self.send_command_sleep = send_command_sleep
+        self.max_loop_count = max_loop_count
 
     def request_data(self, device_id: bytes = ALL_SENSORS) -> None:
         """Submit a request to the device to return pollutant data."""
         cmd = Command.QUERY.value + (b"\x00" * 12) + device_id
         self._send_command(cmd)
 
     def query_data(self) -> QueryResponse:
         """Query the device for pollutant data.
 
         Returns:
             Pollutant data from the device.
 
         """
-        return self._parse_query_response(self._read_response())
+        return _parse_query_response(
+            self._read_until_response(
+                expected_command=Command.QUERY,
+                response_type=ResponseType.QUERY_RESPONSE,
+            )
+        )
 
     def request_reporting_mode(self, device_id: bytes = ALL_SENSORS) -> None:
         """Submit a request to the device to return the current reporting mode."""
         cmd = (
             Command.SET_REPORTING_MODE.value
             + OperationType.QUERY.value
             + ReportingMode.ACTIVE.value
@@ -141,37 +291,25 @@
     def query_reporting_mode(self) -> ReportingModeResponse:
         """Get the current reporting mode of the device.
 
         Returns:
             The current reporting mode of the device.
 
         """
-        return self._parse_reporting_mode_response(self._read_response())
+        return _parse_reporting_mode_response(
+            self._read_until_response(expected_command=Command.SET_REPORTING_MODE)
+        )
 
     def set_active_mode(self) -> None:
         """Set the reporting mode to active."""
         self._set_reporting_mode(ReportingMode.ACTIVE)
-        try:
-            self.query_reporting_mode()
-        except IncorrectCommandException:
-            pass
-        except IncompleteReadException:
-            pass
 
     def set_query_mode(self) -> None:
         """Set the reporting mode to querying."""
         self._set_reporting_mode(ReportingMode.QUERYING)
-        try:
-            self.query_reporting_mode()
-        except IncorrectCommandException:
-            pass
-        except IncompleteReadException:
-            pass
-        except IncorrectCommandCodeException:
-            pass
 
     def _set_reporting_mode(
         self, reporting_mode: ReportingMode, device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the reporting mode, either ACTIVE or QUERYING.
 
         ACTIVE mode means the device will always return a Query command response when data is asked for, regardless of
@@ -189,17 +327,14 @@
             Command.SET_REPORTING_MODE.value
             + OperationType.SET_MODE.value
             + reporting_mode.value
             + (b"\x00" * 10)
             + device_id
         )
         self._send_command(cmd)
-        # Switching between reporting modes is finicky; resetting the serial connection seems to address issues.
-        self.ser.close()
-        self.ser.open()
 
     def request_sleep_state(self, device_id: bytes = ALL_SENSORS) -> None:
         """Submit a request to get the current sleep state."""
         cmd = (
             Command.SET_SLEEP.value
             + OperationType.QUERY.value
             + b"\x00"
@@ -210,15 +345,17 @@
 
     def query_sleep_state(self) -> SleepWakeReadResponse:
         """Get the current sleep state.
 
         Returns:
             The current sleep state of the device.
         """
-        return self._parse_sleep_wake_response(self._read_response())
+        return _parse_sleep_wake_response(
+            self._read_until_response(expected_command=Command.SET_SLEEP)
+        )
 
     def set_sleep_state(
         self, sleep_state: SleepState, device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the sleep state, either wake or sleep.
 
         Args:
@@ -247,15 +384,18 @@
 
         This operates as a fire-and-forget, even in query mode.  You shouldn't have to (and can't) query for a response
         after this command.
         """
         self.wake(device_id=device_id)
         # If we were in query mode, this would flush out the response.  If in active mode, this would be return read
         # data, but we don't care.
-        self.ser.read(10)
+        try:
+            self._read_until_response(expected_command=Command.SET_SLEEP)
+        except IncompleteReadException:
+            pass
 
     def set_device_id(
         self, device_id: bytes, target_device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the device ID.
 
         Args:
@@ -275,15 +415,17 @@
     def query_device_id(self) -> DeviceIdResponse:
         """Retrieve the current device ID.
 
         Returns:
             The current device ID.
 
         """
-        return self._parse_device_id_response(self._read_response())
+        return _parse_device_id_response(
+            self._read_until_response(expected_command=Command.SET_DEVICE_ID)
+        )
 
     def request_working_period(self, device_id: bytes = ALL_SENSORS) -> None:
         """Submit a request to retrieve the current working period for the device."""
         cmd = (
             Command.SET_WORKING_PERIOD.value
             + OperationType.QUERY.value
             + (b"\x00" * 11)
@@ -294,15 +436,17 @@
     def query_working_period(self) -> WorkingPeriodReadResponse:
         """Retrieve the current working period for the device.
 
         Returns:
             The current working period set for the device.
 
         """
-        return self._parse_working_period_reponse(self._read_response())
+        return _parse_working_period_reponse(
+            self._read_until_response(expected_command=Command.SET_WORKING_PERIOD)
+        )
 
     def set_working_period(
         self, working_period: int, device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the working period for the device.
 
         Working period must be between 0 and 30.
@@ -333,15 +477,17 @@
     def query_firmware_version(self) -> CheckFirmwareResponse:
         """Retrieve the firmware version from the device.
 
         Returns:
             The firmware version from the device.
 
         """
-        return self._parse_firmware_response(self._read_response())
+        return _parse_firmware_response(
+            self._read_until_response(expected_command=Command.CHECK_FIRMWARE_VERSION)
+        )
 
     def _send_command(self, cmd: bytes) -> None:
         """Send a command to the device as bytes.
 
         Manages all the wrapper needed to send data to the device, including checksum.
 
         Args:
@@ -354,181 +500,71 @@
         head = HEAD + SUBMIT_TYPE
         full_command = head + cmd + bytes([self._cmd_checksum(cmd)]) + TAIL
         if len(full_command) != 19:
             raise Exception(f"Command length must be 19, but was {len(full_command)}")
         self.ser.write(full_command)
         time.sleep(self.send_command_sleep)
 
-    def _read_response(self) -> bytes:
-        """Read a response from the device.
-
-        Responses from the device should always be 10 bytes in length.
-
-        Returns:
-            Bytes from the device.
-
-        Raises:
-            IncompleteReadException: If the number of bytes read is not 10.
-
-        """
-        result = self.ser.read(10)
-        if len(result) != 10:
-            raise IncompleteReadException(len(result))
-        return result
-
     def _cmd_checksum(self, data: bytes) -> int:
         """Generate a checksum for the data bytes of a command.
 
         Args:
             data: The data bytes of write command.
 
         Returns:
             An integer checksum of the bytes passed.
 
         """
         if len(data) != 15:
             raise AttributeError("Invalid checksum length.")
         return sum(d for d in data) % 256
 
-    def _parse_read_response(
+    def _read_until_response(
         self,
-        data: bytes,
-        command_code: Command,
+        expected_command: Command,
         response_type: ResponseType = ResponseType.GENERAL_RESPONSE,
-    ) -> _RawReadResponse:
-        """Parse bytes into a typed read response. Validates as well.
-
-        Args:
-            data: The raw data bytes to parse.  Must be of length 10.
-            command_code: The expected command code for the response.
-            response_type:  The expected response type for the response.
-
-        Returns:
-            A read response object with the parsed data.
-        """
-        if len(data) != 10:
-            raise IncompleteReadException()
-
-        head: bytes = data[0:1]
-        cmd_id: bytes = data[1:2]
-        payload: bytes = data[2:8]
-        device_id: bytes = data[6:8]
-        checksum: int = data[8]
-        tail: bytes = data[9:10]
-        expected_command_code: Command = command_code
-        expected_response_type: ResponseType = response_type
-        result = _RawReadResponse(
-            head=head,
-            cmd_id=cmd_id,
-            payload=payload,
-            device_id=device_id,
-            checksum=checksum,
-            tail=tail,
-            expected_command_code=expected_command_code,
-            expected_response_type=expected_response_type,
-        )
-        self._verify(result)
-        return result
-
-    def _parse_query_response(self, data: bytes) -> QueryResponse:
-        """Parse a query read response."""
-        raw_response = self._parse_read_response(
-            data, Command.QUERY, ResponseType.QUERY_RESPONSE
-        )
-
-        pm25: float = int.from_bytes(raw_response.payload[0:2], byteorder="little") / 10
-        pm10: float = int.from_bytes(raw_response.payload[2:4], byteorder="little") / 10
-        return QueryResponse(pm25=pm25, pm10=pm10, device_id=raw_response.device_id)
-
-    def _parse_reporting_mode_response(self, data: bytes) -> ReportingModeResponse:
-        """Parse a reporting mode response."""
-        raw_response = self._parse_read_response(
-            data, command_code=Command.SET_REPORTING_MODE
-        )
-        operation_type: OperationType = OperationType(raw_response.payload[1:2])
-        state: ReportingMode = ReportingMode(raw_response.payload[2:3])
-        return ReportingModeResponse(operation_type, state)
-
-    def _parse_device_id_response(self, data: bytes) -> DeviceIdResponse:
-        """Parse a device ID response."""
-        raw_response = self._parse_read_response(
-            data, command_code=Command.SET_DEVICE_ID
-        )
-        return DeviceIdResponse(device_id=raw_response.device_id)
-
-    def _parse_sleep_wake_response(self, data: bytes) -> SleepWakeReadResponse:
-        """Parse a sleep/wake response."""
-        raw_response = self._parse_read_response(data, command_code=Command.SET_SLEEP)
-        operation_type: OperationType = OperationType(raw_response.payload[1:2])
-        state: SleepState = SleepState(raw_response.payload[2:3])
-        return SleepWakeReadResponse(operation_type=operation_type, state=state)
-
-    def _parse_working_period_reponse(self, data: bytes) -> WorkingPeriodReadResponse:
-        """Parse a working period response."""
-        raw_response = self._parse_read_response(
-            data, command_code=Command.SET_WORKING_PERIOD
-        )
-        operation_type: OperationType = OperationType(raw_response.payload[1:2])
-        interval: int = raw_response.payload[2]
-        return WorkingPeriodReadResponse(
-            operation_type=operation_type, interval=interval
-        )
-
-    def _parse_firmware_response(self, data: bytes) -> CheckFirmwareResponse:
-        """Parse a firmware response."""
-        raw_response = self._parse_read_response(
-            data, command_code=Command.CHECK_FIRMWARE_VERSION
-        )
-        year: int = raw_response.payload[1]
-        month: int = raw_response.payload[2]
-        day: int = raw_response.payload[3]
-        return CheckFirmwareResponse(year=year, month=month, day=day)
+    ) -> bytes:
+        """Read from the serial buffer until we find the expected command.
 
-    def _verify(self, read_response: _RawReadResponse) -> None:
-        """Verify read data.
+        This effectively allows us to send commands in active mode; even if the device has filled the buffer with read
+        data, we can still find our responses.
 
         Args:
-            read_response: The raw read data to verify.
+            expected_command: The expected command were looking for
+            response_type: The expected response type were looking for
+
+        Returns:
+            bytes of the matched command
 
         Raises:
-            IncorrectWrapperException: If the head or tail data is incorrect
-            ChecksumFailedException: If the checksum from the response is incorrect
-            IncorrectCommandException: If the command ID in the response is not the expected one.
-            IncorrectCommandCodeException: If the command code in the response is not the expected one.
+            MissingResponseException: If the command couldn't be found in `self.max_loop_count` iterations.
+            IncompleteReadException: If the buffer was empty.
 
         """
-        if read_response.head != HEAD:
-            raise IncorrectWrapperException()
-        if read_response.tail != TAIL:
-            raise IncorrectWrapperException()
-        if read_response.checksum != self._calc_checksum(read_response.payload):
-            raise ChecksumFailedException(
-                expected=read_response.checksum,
-                actual=self._calc_checksum(read_response.payload),
-            )
-        if read_response.cmd_id != read_response.expected_response_type.value:
-            raise IncorrectCommandException(
-                expected=read_response.expected_response_type.value,
-                actual=read_response.cmd_id,
-            )
-
-        # Query responses don't validate the command code
-        if (
-            read_response.expected_response_type != ResponseType.QUERY_RESPONSE
-            and bytes([read_response.payload[0]])
-            != read_response.expected_command_code.value
-        ):
-            raise IncorrectCommandCodeException(
-                expected=read_response.expected_command_code.value,
-                actual=read_response.payload[0:1],
-            )
+        loop_count = 0
+        while output := self.ser.read(10):
+            try:
+                # Validate the response
+                _parse_read_response(
+                    data=output,
+                    command_code=expected_command,
+                    response_type=response_type,
+                )
+                return output
+            except (IncorrectCommandException, IncorrectCommandCodeException):
+                pass
+            # Make sure we dont loop forever.
+            if loop_count >= self.max_loop_count:
+                raise MissingResponseException(
+                    iteration_count=loop_count, expected_command=expected_command.value
+                )
+            loop_count += 1
 
-    def _calc_checksum(self, data: bytes) -> int:
-        """Calculate the checksum for the read data."""
-        return sum(d for d in data) % 256
+        # Loop exited since nothing was assigned to output, meaning no data left.
+        raise IncompleteReadException()
 
 
 class SDS011QueryReader:
     """Reader working in query mode."""
 
     def __init__(self, ser_dev: Union[str, SerialLike], send_command_sleep: int = 1):
         """Create a reader which operates exclusively in query mode.
@@ -536,15 +572,15 @@
         Args:
             ser_dev: A path to a serial device, or an instance of serial.Serial.
             send_command_sleep: The number of seconds to sleep after sending a command to the device.
         """
         self.base_reader = SDS011Reader(
             ser_dev=ser_dev, send_command_sleep=send_command_sleep
         )
-        self.base_reader.safe_wake(device_id=ALL_SENSORS)
+        self.base_reader.safe_wake()
         self.base_reader.set_query_mode()
 
     def query(self, device_id: bytes = ALL_SENSORS) -> QueryResponse:
         """Query the device for pollutant data.
 
         Args:
             device_id: The device ID to get pollutant data for.
@@ -677,15 +713,16 @@
         self.base_reader.request_firmware_version(device_id=device_id)
         return self.base_reader.query_firmware_version()
 
 
 class SDS011ActiveReader:
     """Active Mode Reader.
 
-    Use with caution! Active mode is unpredictable.  Query mode is much preferred.
+    Note that because active mode readers will constantly return data, this implementation opens and closes the serial
+    port for each command.
     """
 
     def __init__(self, ser_dev: Union[str, SerialLike], send_command_sleep: int = 2):
         """Create a reader which operates exclusively in active mode.
 
         Args:
             ser_dev: A path to a serial device, or an instance of serial.Serial.
@@ -693,74 +730,91 @@
         """
         self.base_reader = SDS011Reader(
             ser_dev=ser_dev, send_command_sleep=send_command_sleep
         )
         self.ser_dev: SerialLike = self.base_reader.ser
         self.base_reader.safe_wake()
         self.base_reader.set_active_mode()
+        # We always want to keep the serial device closed in active mode, since otherwise it'll continually send back
+        # read data and we'll run out of memory.
+        self.ser_dev.close()
+        self.max_loop_count = 10
+
+    @contextmanager
+    def _connect(self) -> Generator[None, None, None]:
+        """Connection manager for active mode.
+
+        Opens the serial connection to execute the command, and then closes it afterwards.  In active mode, we don't
+        want to leave the connection open as it will fill up the buffer with read data.
+        """
+        self.ser_dev.open()
+        try:
+            yield
+        finally:
+            self.ser_dev.close()
 
     def query(self) -> QueryResponse:
         """Query the device for pollutant data.
 
         Returns:
             The latest pollutant data.
 
         """
-        return self.base_reader.query_data()
+        with self._connect():
+            return self.base_reader.query_data()
 
-    def sleep(self, device_id: bytes = ALL_SENSORS) -> None:
+    def sleep(self, device_id: bytes = ALL_SENSORS) -> SleepWakeReadResponse:
         """Put the device to sleep, turning off fan and diode.
 
         Args:
             device_id: The device ID to put to sleep.
         """
-        self.base_reader.sleep(device_id)
+        with self._connect():
+            self.base_reader.sleep(device_id)
+            return self.base_reader.query_sleep_state()
 
-        # Sleep seems to behave very strangely in active mode.  It continually outputs data for old commands for quite
-        # a while before eventually having nothing to report.  This forces it to "drain" whatever it was doing before
-        # returning, but also feels quite dangerous.
-        while len(self.ser_dev.read(10)) == 10:
-            pass
-
-    def wake(self, device_id: bytes = ALL_SENSORS) -> None:
+    def wake(self, device_id: bytes = ALL_SENSORS) -> SleepWakeReadResponse:
         """Wake the device up to start reading, turning on the fan and diode.
 
         Args:
             device_id: The device ID to wake up.
         """
-        self.base_reader.wake(device_id)
-        self.ser_dev.read(10)
+        with self._connect():
+            self.base_reader.wake(device_id)
+            return self.base_reader.query_sleep_state()
 
     def set_device_id(
         self, device_id: bytes, target_device_id: bytes = ALL_SENSORS
-    ) -> None:
+    ) -> DeviceIdResponse:
         """Set the device ID.
 
         Args:
             device_id: The new, 4-byte device ID to set.
             target_device_id: The target device ID.
 
         Returns:
             A response with the new device ID.
         """
-        self.base_reader.set_device_id(device_id, target_device_id)
-        self.ser_dev.read(10)
+        with self._connect():
+            self.base_reader.set_device_id(device_id, target_device_id)
+            return self.base_reader.query_device_id()
 
     def set_working_period(
         self, working_period: int, device_id: bytes = ALL_SENSORS
-    ) -> None:
+    ) -> WorkingPeriodReadResponse:
         """Set the working period for the device.
 
         Working period must be between 0 and 30.
 
         0 means the device will read continuously.
         Any value 1-30 means the device will wake and read for 30 seconds every n*60-30 seconds.
 
         Args:
             working_period: A value 0-30 to set as the new working period
             device_id: The device ID to set the working period for.
 
         Returns:
             A response with the new working period
         """
-        self.base_reader.set_working_period(working_period, device_id)
-        self.ser_dev.read(10)
+        with self._connect():
+            self.base_reader.set_working_period(working_period, device_id)
+            return self.base_reader.query_working_period()
```

### Comparing `sds011lib-0.3.2/sds011lib/_constants.py` & `sds011lib-0.4.0/sds011lib/_constants.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.2/sds011lib/exceptions.py` & `sds011lib-0.4.0/sds011lib/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,7 +76,22 @@
 class InvalidDeviceIdException(Sds011Exception):
     """Thrown if the trying to set the device ID on an invalid device.
 
     This occurs if you try and send to a device ID that doesn't exist.
     """
 
     pass
+
+
+class MissingResponseException(Sds011Exception):
+    """Thrown if we are trying to find a response from the device, but it doesn't return in the max iterations.
+
+    This can occur if the device just never responds to a command thats sent.
+    """
+
+    def __init__(self, iteration_count: int, expected_command: bytes):
+        """Create exception."""
+        super().__init__(
+            f"Tried to find command response {expected_command!r} in {iteration_count} attempts, but never did."
+        )
+        self.iteration_count: int = iteration_count
+        self.expected_command: bytes = expected_command
```

### Comparing `sds011lib-0.3.2/sds011lib/responses.py` & `sds011lib-0.4.0/sds011lib/responses.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.2/PKG-INFO` & `sds011lib-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sds011lib
-Version: 0.3.2
+Version: 0.4.0
 Summary: SDS011 Library
 Author: Tim Orme
 Author-email: TimothyOrme@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

