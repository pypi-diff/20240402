# Comparing `tmp/aiocomfoconnect-0.1.8.tar.gz` & `tmp/aiocomfoconnect-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocomfoconnect-0.1.8.tar", max compression
+gzip compressed data, was "aiocomfoconnect-0.1.9.tar", max compression
```

## Comparing `aiocomfoconnect-0.1.8.tar` & `aiocomfoconnect-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1133 2022-11-14 19:35:15.185394 aiocomfoconnect-0.1.8/LICENSE
--rw-r--r--   0        0        0     6041 2023-08-01 09:43:05.497255 aiocomfoconnect-0.1.8/README.md
--rw-r--r--   0        0        0      263 2022-12-16 20:50:33.736818 aiocomfoconnect-0.1.8/aiocomfoconnect/__init__.py
--rw-r--r--   0        0        0    11086 2023-08-01 09:43:05.497255 aiocomfoconnect-0.1.8/aiocomfoconnect/__main__.py
--rw-r--r--   0        0        0    20942 2023-07-31 13:34:19.888514 aiocomfoconnect-0.1.8/aiocomfoconnect/bridge.py
--rw-r--r--   0        0        0    19319 2023-04-06 04:27:11.595081 aiocomfoconnect-0.1.8/aiocomfoconnect/comfoconnect.py
--rw-r--r--   0        0        0     9341 2022-12-16 20:52:49.305149 aiocomfoconnect-0.1.8/aiocomfoconnect/const.py
--rw-r--r--   0        0        0     2796 2022-12-16 20:52:49.294316 aiocomfoconnect-0.1.8/aiocomfoconnect/discovery.py
--rw-r--r--   0        0        0     1297 2023-04-11 07:07:54.292758 aiocomfoconnect-0.1.8/aiocomfoconnect/exceptions.py
--rw-r--r--   0        0        0     1193 2023-07-31 14:37:20.656155 aiocomfoconnect-0.1.8/aiocomfoconnect/properties.py
--rw-r--r--   0        0        0     2776 2022-12-16 19:59:11.317713 aiocomfoconnect-0.1.8/aiocomfoconnect/protobuf/nanopb_pb2.py
--rw-r--r--   0        0        0    29853 2022-11-08 09:06:10.920864 aiocomfoconnect-0.1.8/aiocomfoconnect/protobuf/zehnder_pb2.py
--rw-r--r--   0        0        0    10197 2023-08-01 09:43:05.497255 aiocomfoconnect-0.1.8/aiocomfoconnect/sensors.py
--rw-r--r--   0        0        0     3375 2023-08-01 09:43:05.497255 aiocomfoconnect-0.1.8/aiocomfoconnect/util.py
--rw-r--r--   0        0        0     2395 2023-08-01 09:43:28.998138 aiocomfoconnect-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6797 1970-01-01 00:00:00.000000 aiocomfoconnect-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1133 2022-11-14 19:35:15.185394 aiocomfoconnect-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6042 2023-11-09 14:39:55.109255 aiocomfoconnect-0.1.9/README.md
+-rw-r--r--   0        0        0      263 2022-12-16 20:50:33.736818 aiocomfoconnect-0.1.9/aiocomfoconnect/__init__.py
+-rw-r--r--   0        0        0    16001 2023-11-09 14:39:55.109255 aiocomfoconnect-0.1.9/aiocomfoconnect/__main__.py
+-rw-r--r--   0        0        0    20942 2023-09-04 10:23:42.649406 aiocomfoconnect-0.1.9/aiocomfoconnect/bridge.py
+-rw-r--r--   0        0        0    21673 2023-11-09 14:39:55.109255 aiocomfoconnect-0.1.9/aiocomfoconnect/comfoconnect.py
+-rw-r--r--   0        0        0     9427 2023-11-09 14:39:55.109255 aiocomfoconnect-0.1.9/aiocomfoconnect/const.py
+-rw-r--r--   0        0        0     2796 2022-12-16 20:52:49.294316 aiocomfoconnect-0.1.9/aiocomfoconnect/discovery.py
+-rw-r--r--   0        0        0     1297 2023-04-11 07:07:54.292758 aiocomfoconnect-0.1.9/aiocomfoconnect/exceptions.py
+-rw-r--r--   0        0        0     1246 2023-11-09 14:39:55.109255 aiocomfoconnect-0.1.9/aiocomfoconnect/properties.py
+-rw-r--r--   0        0        0     2776 2022-12-16 19:59:11.317713 aiocomfoconnect-0.1.9/aiocomfoconnect/protobuf/nanopb_pb2.py
+-rw-r--r--   0        0        0    29853 2022-11-08 09:06:10.920864 aiocomfoconnect-0.1.9/aiocomfoconnect/protobuf/zehnder_pb2.py
+-rw-r--r--   0        0        0    10774 2023-11-09 14:39:55.109255 aiocomfoconnect-0.1.9/aiocomfoconnect/sensors.py
+-rw-r--r--   0        0        0     4405 2023-11-09 14:39:55.109255 aiocomfoconnect-0.1.9/aiocomfoconnect/util.py
+-rw-r--r--   0        0        0     2388 2023-11-09 14:40:02.200920 aiocomfoconnect-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6699 1970-01-01 00:00:00.000000 aiocomfoconnect-0.1.9/PKG-INFO
```

### Comparing `aiocomfoconnect-0.1.8/LICENSE` & `aiocomfoconnect-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.8/README.md` & `aiocomfoconnect-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # aiocomfoconnect
 
 `aiocomfoconnect` is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system. It's the successor of
 [comfoconnect](https://github.com/michaelarnauts/comfoconnect).
 
-It's compatible with Python 3.8 and higher.
+It's compatible with Python 3.10 and higher.
 
 ## Installation
 
 ```shell
 pip3 install aiocomfoconnect
 ```
 
@@ -145,15 +145,15 @@
 ### Decode network traffic
 
 You can use the `scripts/decode_pcap.py` file to decode network traffic between the Mobile App and the ComfoConnect LAN C.
 Make sure that the first TCP session in the capture is the connection between the bridge and the app. It's therefore recommended to start the capture before you open the app.
 
 ```shell
 $ sudo tcpdump -i any -s 0 -w /tmp/capture.pcap tcp and port 56747
-$ python scripts/decode_pcap.py /tmp/capture.pcap
+$ python3 script/decode_pcap.py /tmp/capture.pcap
 ```
 
 ### Generate zehnder_pb2.py file
 
 ```shell
 pip3 install grpcio-tools
 python3 -m grpc_tools.protoc -Iprotobuf protobuf/nanopb.proto --python_out=aiocomfoconnect/protobuf
```

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/__main__.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,58 +12,70 @@
 from aiocomfoconnect.comfoconnect import ComfoConnect
 from aiocomfoconnect.discovery import discover_bridges
 from aiocomfoconnect.exceptions import (
     AioComfoConnectNotConnected,
     AioComfoConnectTimeout,
     ComfoConnectNotAllowed,
 )
-from aiocomfoconnect.sensors import SENSORS
 from aiocomfoconnect.properties import Property
+from aiocomfoconnect.sensors import SENSORS
 
 _LOGGER = logging.getLogger(__name__)
 
 
 async def main(args):
     """Main function."""
     if args.action == "discover":
         await run_discover(args.host)
 
     elif args.action == "register":
         await run_register(args.host, args.uuid, args.name, args.pin)
 
+    elif args.action == "deregister":
+        await run_deregister(args.host, args.uuid, args.uuid2)
+
     elif args.action == "set-speed":
         await run_set_speed(args.host, args.uuid, args.speed)
 
     elif args.action == "set-mode":
         await run_set_mode(args.host, args.uuid, args.mode)
 
+    elif args.action == "set-comfocool":
+        await run_set_comfocool(args.host, args.uuid, args.mode)
+
     elif args.action == "show-sensors":
         await run_show_sensors(args.host, args.uuid)
 
     elif args.action == "show-sensor":
         await run_show_sensor(args.host, args.uuid, args.sensor, args.follow)
 
     elif args.action == "get-property":
         await run_get_property(args.host, args.uuid, args.node_id, args.unit, args.subunit, args.property_id, args.property_type)
 
+    elif args.action == "get-flow-for-speed":
+        await run_get_flow_for_speed(args.host, args.uuid, args.speed)
+
+    elif args.action == "set-flow-for-speed":
+        await run_set_flow_for_speed(args.host, args.uuid, args.speed, args.flow)
+
     else:
         raise Exception("Unknown action: " + args.action)
 
 
 async def run_discover(host: str = None):
     """Discover all bridges on the network."""
     bridges = await discover_bridges(host)
     print("Discovered bridges:")
     for bridge in bridges:
         print(bridge)
         print()
 
 
 async def run_register(host: str, uuid: str, name: str, pin: int):
-    """Connect to a bridge."""
+    """Register an app on the bridge."""
     # Discover bridge so we know the UUID
     bridges = await discover_bridges(host)
     if not bridges:
         raise Exception("No bridge found")
 
     # Connect to the bridge
     comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid)
@@ -93,16 +105,44 @@
     reply = await comfoconnect.cmd_list_registered_apps()
     for app in reply.apps:
         print(f"* {app.uuid.hex()}: {app.devicename}")
 
     await comfoconnect.disconnect()
 
 
+async def run_deregister(host: str, uuid: str, uuid2: str):
+    """Deregister an app on the bridge."""
+    # Discover bridge so we know the UUID
+    bridges = await discover_bridges(host)
+    if not bridges:
+        raise Exception("No bridge found")
+
+    # Connect to the bridge
+    comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid)
+    try:
+        await comfoconnect.connect(uuid)
+    except ComfoConnectNotAllowed:
+        print("Could not connect to bridge. Please register first.")
+        sys.exit(1)
+
+    if uuid2:
+        await comfoconnect.cmd_deregister_app(uuid2)
+
+    # ListRegisteredApps
+    print()
+    print("Registered applications:")
+    reply = await comfoconnect.cmd_list_registered_apps()
+    for app in reply.apps:
+        print(f"* {app.uuid.hex()}: {app.devicename}")
+
+    await comfoconnect.disconnect()
+
+
 async def run_set_speed(host: str, uuid: str, speed: Literal["away", "low", "medium", "high"]):
-    """Connect to a bridge."""
+    """Set ventilation speed."""
     # Discover bridge so we know the UUID
     bridges = await discover_bridges(host)
     if not bridges:
         raise Exception("No bridge found")
 
     # Connect to the bridge
     comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid)
@@ -114,15 +154,15 @@
 
     await comfoconnect.set_speed(speed)
 
     await comfoconnect.disconnect()
 
 
 async def run_set_mode(host: str, uuid: str, mode: Literal["auto", "manual"]):
-    """Connect to a bridge."""
+    """Set ventilation mode."""
     # Discover bridge so we know the UUID
     bridges = await discover_bridges(host)
     if not bridges:
         raise Exception("No bridge found")
 
     # Connect to the bridge
     comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid)
@@ -133,16 +173,36 @@
         sys.exit(1)
 
     await comfoconnect.set_mode(mode)
 
     await comfoconnect.disconnect()
 
 
+async def run_set_comfocool(host: str, uuid: str, mode: Literal["auto", "off"]):
+    """Set comfocool mode."""
+    # Discover bridge so we know the UUID
+    bridges = await discover_bridges(host)
+    if not bridges:
+        raise Exception("No bridge found")
+
+    # Connect to the bridge
+    comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid)
+    try:
+        await comfoconnect.connect(uuid)
+    except ComfoConnectNotAllowed:
+        print("Could not connect to bridge. Please register first.")
+        sys.exit(1)
+
+    await comfoconnect.set_comfocool_mode(mode)
+
+    await comfoconnect.disconnect()
+
+
 async def run_show_sensors(host: str, uuid: str):
-    """Connect to a bridge."""
+    """Show all sensors."""
     # Discover bridge so we know the UUID
     bridges = await discover_bridges(host)
     if not bridges:
         raise Exception("No bridge found")
 
     def alarm_callback(node_id, errors):
         """Print alarm updates."""
@@ -187,15 +247,15 @@
         pass
 
     print("Disconnecting...")
     await comfoconnect.disconnect()
 
 
 async def run_show_sensor(host: str, uuid: str, sensor: int, follow=False):
-    """Connect to a bridge."""
+    """Show a sensor."""
     result = Future()
 
     # Discover bridge so we know the UUID
     bridges = await discover_bridges(host)
     if not bridges:
         raise Exception("No bridge found")
 
@@ -233,15 +293,15 @@
             pass
 
     # Disconnect
     await comfoconnect.disconnect()
 
 
 async def run_get_property(host: str, uuid: str, node_id: int, unit: int, subunit: int, property_id: int, property_type: int):
-    """Connect to a bridge."""
+    """Get a property."""
     # Discover bridge so we know the UUID
     bridges = await discover_bridges(host)
     if not bridges:
         raise Exception("No bridge found")
 
     # Connect to the bridge
     comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid)
@@ -252,38 +312,89 @@
         sys.exit(1)
 
     print(await comfoconnect.get_property(Property(unit, subunit, property_id, property_type), node_id))
 
     await comfoconnect.disconnect()
 
 
+async def run_get_flow_for_speed(host: str, uuid: str, speed: Literal["away", "low", "medium", "high"]):
+    """Get the configured airflow for the specified speed."""
+    # Discover bridge so we know the UUID
+    bridges = await discover_bridges(host)
+    if not bridges:
+        raise Exception("No bridge found")
+
+    # Connect to the bridge
+    comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid)
+    try:
+        await comfoconnect.connect(uuid)
+    except ComfoConnectNotAllowed:
+        print("Could not connect to bridge. Please register first.")
+        sys.exit(1)
+
+    print(await comfoconnect.get_flow_for_speed(speed))
+
+    await comfoconnect.disconnect()
+
+
+async def run_set_flow_for_speed(host: str, uuid: str, speed: Literal["away", "low", "medium", "high"], desired_flow: int):
+    """Set the configured airflow for the specified speed."""
+    # Discover bridge so we know the UUID
+    bridges = await discover_bridges(host)
+    if not bridges:
+        raise Exception("No bridge found")
+
+    # Connect to the bridge
+    comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid)
+    try:
+        await comfoconnect.connect(uuid)
+    except ComfoConnectNotAllowed:
+        print("Could not connect to bridge. Please register first.")
+        sys.exit(1)
+
+    await comfoconnect.set_flow_for_speed(speed, desired_flow)
+
+    await comfoconnect.disconnect()
+
+
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--debug", "-d", help="Enable debug logging", default=False, action="store_true")
     subparsers = parser.add_subparsers(required=True, dest="action")
 
     p_discover = subparsers.add_parser("discover", help="discover ComfoConnect LAN C devices on your network")
     p_discover.add_argument("--host", help="Host address of the bridge")
 
     p_register = subparsers.add_parser("register", help="register on a ComfoConnect LAN C device")
     p_register.add_argument("--pin", help="PIN code to register on the bridge", default=DEFAULT_PIN)
     p_register.add_argument("--host", help="Host address of the bridge")
     p_register.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
     p_register.add_argument("--name", help="Name of this app", default=DEFAULT_NAME)
 
+    p_register = subparsers.add_parser("deregister", help="deregister on a ComfoConnect LAN C device")
+    p_register.add_argument("uuid2", help="UUID of the app to deregister", default=None)
+    p_register.add_argument("--pin", help="PIN code to register on the bridge", default=DEFAULT_PIN)
+    p_register.add_argument("--host", help="Host address of the bridge")
+    p_register.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
+
     p_set_speed = subparsers.add_parser("set-speed", help="set the fan speed")
     p_set_speed.add_argument("speed", help="Fan speed", choices=["low", "medium", "high", "away"])
     p_set_speed.add_argument("--host", help="Host address of the bridge")
     p_set_speed.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
 
     p_set_mode = subparsers.add_parser("set-mode", help="set operation mode")
     p_set_mode.add_argument("mode", help="Operation mode", choices=["auto", "manual"])
     p_set_mode.add_argument("--host", help="Host address of the bridge")
     p_set_mode.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
 
+    p_set_mode = subparsers.add_parser("set-comfocool", help="set comfocool mode")
+    p_set_mode.add_argument("mode", help="Comfocool mode", choices=["auto", "off"])
+    p_set_mode.add_argument("--host", help="Host address of the bridge")
+    p_set_mode.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
+
     p_sensors = subparsers.add_parser("show-sensors", help="show the sensor values")
     p_sensors.add_argument("--host", help="Host address of the bridge")
     p_sensors.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
 
     p_sensor = subparsers.add_parser("show-sensor", help="show a single sensor value")
     p_sensor.add_argument("sensor", help="The ID of the sensor", type=int)
     p_sensor.add_argument("--host", help="Host address of the bridge")
@@ -296,14 +407,25 @@
     p_sensor.add_argument("property_id", help="The id of the property", type=int)
     p_sensor.add_argument("property_type", help="The type of the property", type=int, default=0x09)
 
     p_sensor.add_argument("--node_id", help="The Node ID of the query", type=int, default=0x01)
     p_sensor.add_argument("--host", help="Host address of the bridge")
     p_sensor.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
 
+    p_get_flow_speed = subparsers.add_parser("get-flow-for-speed", help="Get m³/h for given speed")
+    p_get_flow_speed.add_argument("speed", help="Fan speed", choices=["low", "medium", "high", "away"])
+    p_get_flow_speed.add_argument("--host", help="Host address of the bridge")
+    p_get_flow_speed.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
+
+    p_set_flow_speed = subparsers.add_parser("set-flow-for-speed", help="Set m³/h for given speed")
+    p_set_flow_speed.add_argument("speed", help="Fan speed", choices=["low", "medium", "high", "away"])
+    p_set_flow_speed.add_argument("flow", help="Desired airflow in m³/h", type=int)
+    p_set_flow_speed.add_argument("--host", help="Host address of the bridge")
+    p_set_flow_speed.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
+
     arguments = parser.parse_args()
 
     if arguments.debug:
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.WARNING)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/bridge.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/bridge.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/comfoconnect.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/comfoconnect.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,37 +7,32 @@
 from aiocomfoconnect import Bridge
 from aiocomfoconnect.const import (
     ERRORS,
     ERRORS_140,
     SUBUNIT_01,
     SUBUNIT_02,
     SUBUNIT_03,
+    SUBUNIT_05,
     SUBUNIT_06,
     SUBUNIT_07,
     SUBUNIT_08,
-    TYPE_CN_BOOL,
-    TYPE_CN_INT8,
-    TYPE_CN_INT16,
-    TYPE_CN_INT64,
-    TYPE_CN_STRING,
-    TYPE_CN_UINT8,
-    TYPE_CN_UINT16,
-    TYPE_CN_UINT32,
+    PdoType,
     UNIT_ERROR,
     UNIT_SCHEDULE,
     UNIT_TEMPHUMCONTROL,
+    UNIT_VENTILATIONCONFIG,
     VentilationBalance,
     VentilationMode,
     VentilationSetting,
     VentilationSpeed,
     VentilationTemperatureProfile,
 )
 from aiocomfoconnect.properties import Property
 from aiocomfoconnect.sensors import Sensor
-from aiocomfoconnect.util import bytearray_to_bits, bytestring
+from aiocomfoconnect.util import bytearray_to_bits, bytestring, encode_pdo_value
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ComfoConnect(Bridge):
     """Abstraction layer over the ComfoConnect LAN C API."""
 
@@ -97,21 +92,21 @@
         """Get a property and convert to the right type."""
         return await self.get_single_property(prop.unit, prop.subunit, prop.property_id, prop.property_type, node_id=node_id)
 
     async def get_single_property(self, unit: int, subunit: int, property_id: int, property_type: int = None, node_id=1) -> any:
         """Get a property and convert to the right type."""
         result = await self.cmd_rmi_request(bytes([0x01, unit, subunit, 0x10, property_id]), node_id=node_id)
 
-        if property_type == TYPE_CN_STRING:
+        if property_type == PdoType.TYPE_CN_STRING:
             return result.message.decode("utf-8").rstrip("\x00")
-        if property_type in [TYPE_CN_INT8, TYPE_CN_INT16, TYPE_CN_INT64]:
+        if property_type in [PdoType.TYPE_CN_INT8, PdoType.TYPE_CN_INT16, PdoType.TYPE_CN_INT64]:
             return int.from_bytes(result.message, byteorder="little", signed=True)
-        if property_type in [TYPE_CN_UINT8, TYPE_CN_UINT16, TYPE_CN_UINT32]:
+        if property_type in [PdoType.TYPE_CN_UINT8, PdoType.TYPE_CN_UINT16, PdoType.TYPE_CN_UINT32]:
             return int.from_bytes(result.message, byteorder="little", signed=False)
-        if property_type in [TYPE_CN_BOOL]:
+        if property_type in [PdoType.TYPE_CN_BOOL]:
             return result.message[0] == 1
 
         return result.message
 
     async def get_multiple_properties(self, unit: int, subunit: int, property_ids: List[int], node_id=1) -> any:
         """Get multiple properties."""
         result = await self.cmd_rmi_request(bytestring([0x02, unit, subunit, 0x01, 0x10 | len(property_ids), bytes(property_ids)]), node_id=node_id)
@@ -120,14 +115,23 @@
 
     async def set_property(self, unit: int, subunit: int, property_id: int, value: int, node_id=1) -> any:
         """Set a property."""
         result = await self.cmd_rmi_request(bytes([0x03, unit, subunit, property_id, value]), node_id=node_id)
 
         return result.message
 
+    async def set_property_typed(self, unit: int, subunit: int, property_id: int, value: int, pdo_type: PdoType, node_id=1) -> any:
+        """Set a typed property."""
+        value_bytes = encode_pdo_value(value, pdo_type)
+        message_bytes = bytes([0x03, unit, subunit, property_id]) + value_bytes
+
+        result = await self.cmd_rmi_request(message_bytes, node_id=node_id)
+
+        return result.message
+
     def _sensor_callback(self, sensor_id, sensor_value):
         """Callback function for sensor updates."""
         if self._sensor_callback_fn is None:
             return
 
         sensor = self._sensors.get(sensor_id)
         if sensor is None:
@@ -207,14 +211,44 @@
         elif speed == VentilationSpeed.MEDIUM:
             await self.cmd_rmi_request(bytes([0x84, UNIT_SCHEDULE, SUBUNIT_01, 0x01, 0x00, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x02]))
         elif speed == VentilationSpeed.HIGH:
             await self.cmd_rmi_request(bytes([0x84, UNIT_SCHEDULE, SUBUNIT_01, 0x01, 0x00, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x03]))
         else:
             raise ValueError(f"Invalid speed: {speed}")
 
+    async def get_flow_for_speed(self, speed: Literal["away", "low", "medium", "high"]) -> int:
+        """Get the targeted airflow in m³/h for the given VentilationSpeed (away / low / medium / high)."""
+
+        match speed:
+            case VentilationSpeed.AWAY:
+                property_id = 3
+            case VentilationSpeed.LOW:
+                property_id = 4
+            case VentilationSpeed.MEDIUM:
+                property_id = 5
+            case VentilationSpeed.HIGH:
+                property_id = 6
+
+        return await self.get_single_property(UNIT_VENTILATIONCONFIG, SUBUNIT_01, property_id, PdoType.TYPE_CN_INT16)
+
+    async def set_flow_for_speed(self, speed: Literal["away", "low", "medium", "high"], desired_flow: int):
+        """Set the targeted airflow in m³/h for the given VentilationSpeed (away / low / medium / high)."""
+
+        match speed:
+            case VentilationSpeed.AWAY:
+                property_id = 3
+            case VentilationSpeed.LOW:
+                property_id = 4
+            case VentilationSpeed.MEDIUM:
+                property_id = 5
+            case VentilationSpeed.HIGH:
+                property_id = 6
+
+        await self.set_property_typed(UNIT_VENTILATIONCONFIG, SUBUNIT_01, property_id, desired_flow, PdoType.TYPE_CN_INT16)
+
     async def get_bypass(self):
         """Get the bypass mode (auto / on / off)."""
         result = await self.cmd_rmi_request(bytes([0x83, UNIT_SCHEDULE, SUBUNIT_02, 0x01]))
         # 0000000000080700000000000000 = auto
         # 0100000000100e00000b0e000001 = open
         # 0100000000100e00000d0e000002 = close
         mode = result.message[-1]
@@ -306,14 +340,27 @@
     async def set_away(self, mode: bool, timeout=3600):
         """Activate away mode."""
         if mode:
             await self.cmd_rmi_request(bytestring([0x84, UNIT_SCHEDULE, SUBUNIT_01, 0x0B, 0x00, 0x00, 0x00, 0x00, timeout.to_bytes(4, "little", signed=True), 0x00]))
         else:
             await self.cmd_rmi_request(bytes([0x85, UNIT_SCHEDULE, SUBUNIT_01, 0x0B]))
 
+    async def get_comfocool_mode(self):
+        """Get the current comfocool mode."""
+        result = await self.cmd_rmi_request(bytes([0x83, UNIT_SCHEDULE, SUBUNIT_05, 0x01]))
+        mode = result.message[0]
+        return mode == 0
+
+    async def set_comfocool_mode(self, mode: Literal["auto", "off"], timeout=-1):
+        """Set the comfocool mode (auto / off)."""
+        if mode == "auto":
+            await self.cmd_rmi_request(bytes([0x85, UNIT_SCHEDULE, SUBUNIT_05, 0x01]))
+        else:
+            await self.cmd_rmi_request(bytestring([0x84, UNIT_SCHEDULE, SUBUNIT_05, 0x01, 0x00, 0x00, 0x00, 0x00, timeout.to_bytes(4, "little", signed=True), 0x00]))
+
     async def get_temperature_profile(self):
         """Get the temperature profile (warm / normal / cool)."""
         result = await self.cmd_rmi_request(bytes([0x83, UNIT_SCHEDULE, SUBUNIT_03, 0x01]))
         # 0100000000ffffffffffffffff02 = warm
         # 0100000000ffffffffffffffff00 = normal
         # 0100000000ffffffffffffffff01 = cool
         mode = result.message[-1]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/const.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """ Constants """
 
 # PDO Types
-TYPE_CN_BOOL = 0x00
-TYPE_CN_UINT8 = 0x01
-TYPE_CN_UINT16 = 0x02
-TYPE_CN_UINT32 = 0x03
-TYPE_CN_INT8 = 0x05
-TYPE_CN_INT16 = 0x06
-TYPE_CN_INT64 = 0x08
-TYPE_CN_STRING = 0x09
-TYPE_CN_TIME = 0x10
-TYPE_CN_VERSION = 0x11
+class PdoType:
+    """Defines a PDO type."""
+
+    TYPE_CN_BOOL = 0x00
+    TYPE_CN_UINT8 = 0x01
+    TYPE_CN_UINT16 = 0x02
+    TYPE_CN_UINT32 = 0x03
+    TYPE_CN_INT8 = 0x05
+    TYPE_CN_INT16 = 0x06
+    TYPE_CN_INT64 = 0x08
+    TYPE_CN_STRING = 0x09
+    TYPE_CN_TIME = 0x10
+    TYPE_CN_VERSION = 0x11
 
 
 # ComfoConnect Units
 UNIT_NODE = 0x01
 UNIT_COMFOBUS = 0x02
 UNIT_ERROR = 0x03
 UNIT_SCHEDULE = 0x15
```

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/discovery.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/discovery.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/exceptions.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/properties.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/properties.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ Property definitions """
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 from .const import (
-    TYPE_CN_STRING,
-    TYPE_CN_UINT32,
+    PdoType,
     UNIT_NODE,
     UNIT_NODECONFIGURATION,
     UNIT_TEMPHUMCONTROL,
 )
 
 
 @dataclass
@@ -18,19 +17,19 @@
 
     unit: int
     subunit: int
     property_id: int
     property_type: int
 
 
-PROPERTY_SERIAL_NUMBER = Property(UNIT_NODE, 0x01, 0x04, TYPE_CN_STRING)
-PROPERTY_FIRMWARE_VERSION = Property(UNIT_NODE, 0x01, 0x06, TYPE_CN_UINT32)
-PROPERTY_MODEL = Property(UNIT_NODE, 0x01, 0x08, TYPE_CN_STRING)
-PROPERTY_ARTICLE = Property(UNIT_NODE, 0x01, 0x0B, TYPE_CN_STRING)
-PROPERTY_COUNTRY = Property(UNIT_NODE, 0x01, 0x0D, TYPE_CN_STRING)
-PROPERTY_NAME = Property(UNIT_NODE, 0x01, 0x14, TYPE_CN_STRING)
-
-PROPERTY_MAINTAINER_PASSWORD = Property(UNIT_NODECONFIGURATION, 0x01, 0x03, TYPE_CN_STRING)
-
-PROPERTY_SENSOR_VENTILATION_TEMP_PASSIVE = Property(UNIT_TEMPHUMCONTROL, 0x01, 0x04, TYPE_CN_UINT32)
-PROPERTY_SENSOR_VENTILATION_HUMIDITY_COMFORT = Property(UNIT_TEMPHUMCONTROL, 0x01, 0x06, TYPE_CN_UINT32)
-PROPERTY_SENSOR_VENTILATION_HUMIDITY_PROTECTION = Property(UNIT_TEMPHUMCONTROL, 0x01, 0x07, TYPE_CN_UINT32)
+PROPERTY_SERIAL_NUMBER = Property(UNIT_NODE, 0x01, 0x04, PdoType.TYPE_CN_STRING)
+PROPERTY_FIRMWARE_VERSION = Property(UNIT_NODE, 0x01, 0x06, PdoType.TYPE_CN_UINT32)
+PROPERTY_MODEL = Property(UNIT_NODE, 0x01, 0x08, PdoType.TYPE_CN_STRING)
+PROPERTY_ARTICLE = Property(UNIT_NODE, 0x01, 0x0B, PdoType.TYPE_CN_STRING)
+PROPERTY_COUNTRY = Property(UNIT_NODE, 0x01, 0x0D, PdoType.TYPE_CN_STRING)
+PROPERTY_NAME = Property(UNIT_NODE, 0x01, 0x14, PdoType.TYPE_CN_STRING)
+
+PROPERTY_MAINTAINER_PASSWORD = Property(UNIT_NODECONFIGURATION, 0x01, 0x03, PdoType.TYPE_CN_STRING)
+
+PROPERTY_SENSOR_VENTILATION_TEMP_PASSIVE = Property(UNIT_TEMPHUMCONTROL, 0x01, 0x04, PdoType.TYPE_CN_UINT32)
+PROPERTY_SENSOR_VENTILATION_HUMIDITY_COMFORT = Property(UNIT_TEMPHUMCONTROL, 0x01, 0x06, PdoType.TYPE_CN_UINT32)
+PROPERTY_SENSOR_VENTILATION_HUMIDITY_PROTECTION = Property(UNIT_TEMPHUMCONTROL, 0x01, 0x07, PdoType.TYPE_CN_UINT32)
```

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/protobuf/nanopb_pb2.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/protobuf/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/protobuf/zehnder_pb2.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/protobuf/zehnder_pb2.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.8/aiocomfoconnect/sensors.py` & `aiocomfoconnect-0.1.9/aiocomfoconnect/sensors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 """ Sensor definitions. """
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Callable, Dict
 
+from .const import PdoType
 from .util import calculate_airflow_constraints
-from .const import (
-    TYPE_CN_BOOL,
-    TYPE_CN_INT16,
-    TYPE_CN_UINT8,
-    TYPE_CN_UINT16,
-    TYPE_CN_UINT32,
-    TYPE_CN_INT64,
-)
 
 # Sensors
 SENSOR_ANALOG_INPUT_1 = 369
 SENSOR_ANALOG_INPUT_2 = 370
 SENSOR_ANALOG_INPUT_3 = 371
 SENSOR_ANALOG_INPUT_4 = 372
 SENSOR_AVOIDED_COOLING = 216
@@ -95,94 +88,94 @@
     id: int  # pylint: disable=invalid-name
     type: int
     value_fn: Callable[[int], any] = None
 
 
 # For more information, see PROTOCOL-PDO.md
 SENSORS: Dict[int, Sensor] = {
-    SENSOR_DEVICE_STATE: Sensor("Device State", None, 16, TYPE_CN_UINT8),
-    SENSOR_CHANGING_FILTERS: Sensor("Changing filters", None, 18, TYPE_CN_UINT8),
-    33: Sensor("sensor_33", None, 33, TYPE_CN_UINT8),
-    37: Sensor("sensor_37", None, 37, TYPE_CN_UINT8),
-    SENSOR_OPERATING_MODE_2: Sensor("Operating Mode", None, 49, TYPE_CN_UINT8),
-    53: Sensor("sensor_53", None, 53, TYPE_CN_UINT8),
-    SENSOR_FAN_MODE_SUPPLY_2: Sensor("Supply Fan Mode", None, 54, TYPE_CN_UINT8),
-    SENSOR_FAN_MODE_EXHAUST_2: Sensor("Exhaust Fan Mode", None, 55, TYPE_CN_UINT8),
-    SENSOR_OPERATING_MODE: Sensor("Operating Mode", None, 56, TYPE_CN_UINT8),
-    SENSOR_FAN_SPEED_MODE: Sensor("Fan Speed", None, 65, TYPE_CN_UINT8),
-    SENSOR_BYPASS_ACTIVATION_STATE: Sensor("Bypass Activation State", None, 66, TYPE_CN_UINT8),
-    SENSOR_PROFILE_TEMPERATURE: Sensor("Temperature Profile Mode", None, 67, TYPE_CN_UINT8),
-    SENSOR_FAN_MODE_SUPPLY: Sensor("Supply Fan Mode", None, 70, TYPE_CN_UINT8),
-    SENSOR_FAN_MODE_EXHAUST: Sensor("Exhaust Fan Mode", None, 71, TYPE_CN_UINT8),
-    SENSOR_NEXT_CHANGE_FAN: Sensor("Fan Speed Next Change", None, 81, TYPE_CN_UINT32),
-    SENSOR_NEXT_CHANGE_BYPASS: Sensor("Bypass Next Change", None, 82, TYPE_CN_UINT32),
-    85: Sensor("sensor_85", None, 85, TYPE_CN_UINT32),
-    SENSOR_NEXT_CHANGE_FAN_SUPPLY: Sensor("Supply Fan Next Change", None, 86, TYPE_CN_UINT32),
-    SENSOR_NEXT_CHANGE_FAN_EXHAUST: Sensor("Exhaust Fan Next Change", None, 87, TYPE_CN_UINT32),
-    SENSOR_FAN_EXHAUST_DUTY: Sensor("Exhaust Fan Duty", UNIT_PERCENT, 117, TYPE_CN_UINT8),
-    SENSOR_FAN_SUPPLY_DUTY: Sensor("Supply Fan Duty", UNIT_PERCENT, 118, TYPE_CN_UINT8),
-    SENSOR_FAN_EXHAUST_FLOW: Sensor("Exhaust Fan Flow", UNIT_M3H, 119, TYPE_CN_UINT16),
-    SENSOR_FAN_SUPPLY_FLOW: Sensor("Supply Fan Flow", UNIT_M3H, 120, TYPE_CN_UINT16),
-    SENSOR_FAN_EXHAUST_SPEED: Sensor("Exhaust Fan Speed", UNIT_RPM, 121, TYPE_CN_UINT16),
-    SENSOR_FAN_SUPPLY_SPEED: Sensor("Supply Fan Speed", UNIT_RPM, 122, TYPE_CN_UINT16),
-    SENSOR_POWER_USAGE: Sensor("Power Usage", UNIT_WATT, 128, TYPE_CN_UINT16),
-    SENSOR_POWER_USAGE_TOTAL_YEAR: Sensor("Power Usage (year)", UNIT_KWH, 129, TYPE_CN_UINT16),
-    SENSOR_POWER_USAGE_TOTAL: Sensor("Power Usage (total)", UNIT_KWH, 130, TYPE_CN_UINT16),
-    SENSOR_PREHEATER_POWER_TOTAL_YEAR: Sensor("Preheater Power Usage (year)", UNIT_KWH, 144, TYPE_CN_UINT16),
-    SENSOR_PREHEATER_POWER_TOTAL: Sensor("Preheater Power Usage (total)", UNIT_KWH, 145, TYPE_CN_UINT16),
-    SENSOR_PREHEATER_POWER: Sensor("Preheater Power Usage", UNIT_WATT, 146, TYPE_CN_UINT16),
-    SENSOR_RF_PAIRING_MODE: Sensor("RF Pairing Mode", None, 176, TYPE_CN_UINT8),
-    SENSOR_DAYS_TO_REPLACE_FILTER: Sensor("Days remaining to replace the filter", None, 192, TYPE_CN_UINT16),
-    SENSOR_UNIT_TEMPERATURE: Sensor("Device Temperature Unit", None, 208, TYPE_CN_UINT8, lambda x: "celcius" if x == 0 else "farenheit"),
-    SENSOR_RMOT: Sensor("Running Mean Outdoor Temperature (RMOT)", UNIT_CELCIUS, 209, TYPE_CN_INT16, lambda x: x / 10),
-    SENSOR_SEASON_HEATING_ACTIVE: Sensor("Heating Season is active", None, 210, TYPE_CN_BOOL, bool),
-    SENSOR_SEASON_COOLING_ACTIVE: Sensor("Cooling Season is active", None, 211, TYPE_CN_BOOL, bool),
-    SENSOR_TARGET_TEMPERATURE: Sensor("Target Temperature", UNIT_CELCIUS, 212, TYPE_CN_INT16, lambda x: x / 10),
-    SENSOR_AVOIDED_HEATING: Sensor("Avoided Heating Power Usage", UNIT_WATT, 213, TYPE_CN_UINT16),
-    SENSOR_AVOIDED_HEATING_TOTAL_YEAR: Sensor("Avoided Heating Power Usage (year)", UNIT_KWH, 214, TYPE_CN_UINT16),
-    SENSOR_AVOIDED_HEATING_TOTAL: Sensor("Avoided Heating Power Usage (total)", UNIT_KWH, 215, TYPE_CN_UINT16),
-    SENSOR_AVOIDED_COOLING: Sensor("Avoided Cooling Power Usage", UNIT_WATT, 216, TYPE_CN_UINT16),
-    SENSOR_AVOIDED_COOLING_TOTAL_YEAR: Sensor("Avoided Cooling Power Usage (year)", UNIT_KWH, 217, TYPE_CN_UINT16),
-    SENSOR_AVOIDED_COOLING_TOTAL: Sensor("Avoided Cooling Power Usage (total)", UNIT_KWH, 218, TYPE_CN_UINT16),
-    219: Sensor("sensor_219", None, 219, TYPE_CN_UINT16),
-    220: Sensor("Outdoor Air Temperature (?)", None, 220, TYPE_CN_INT16, lambda x: x / 10),
-    SENSOR_TEMPERATURE_SUPPLY: Sensor("Supply Air Temperature", UNIT_CELCIUS, 221, TYPE_CN_INT16, lambda x: x / 10),
-    SENSOR_UNIT_AIRFLOW: Sensor("Device Airflow Unit", None, 224, TYPE_CN_UINT8, lambda x: "m3ph" if x == 3 else "lps"),
-    SENSOR_COMFORTCONTROL_MODE: Sensor("Sensor based ventilation mode", None, 225, TYPE_CN_UINT8),
-    SENSOR_FAN_SPEED_MODE_MODULATED: Sensor("Fan Speed (modulated)", None, 226, TYPE_CN_UINT16),
-    SENSOR_BYPASS_STATE: Sensor("Bypass State", UNIT_PERCENT, 227, TYPE_CN_UINT8),
-    SENSOR_FROSTPROTECTION_UNBALANCE: Sensor("frostprotection_unbalance", None, 228, TYPE_CN_UINT8),
-    SENSOR_AIRFLOW_CONSTRAINTS: Sensor("Airflow constraints", None, 230, TYPE_CN_INT64, calculate_airflow_constraints),
-    SENSOR_TEMPERATURE_EXTRACT: Sensor("Extract Air Temperature", UNIT_CELCIUS, 274, TYPE_CN_INT16, lambda x: x / 10),
-    SENSOR_TEMPERATURE_EXHAUST: Sensor("Exhaust Air Temperature", UNIT_CELCIUS, 275, TYPE_CN_INT16, lambda x: x / 10),
-    SENSOR_TEMPERATURE_OUTDOOR: Sensor("Outdoor Air Temperature", UNIT_CELCIUS, 276, TYPE_CN_INT16, lambda x: x / 10),
-    277: Sensor("Outdoor Air Temperature (?)", UNIT_CELCIUS, 277, TYPE_CN_INT16, lambda x: x / 10),
-    278: Sensor("Supply Air Temperature (?)", UNIT_CELCIUS, 278, TYPE_CN_INT16, lambda x: x / 10),
-    SENSOR_HUMIDITY_EXTRACT: Sensor("Extract Air Humidity", UNIT_PERCENT, 290, TYPE_CN_UINT8),
-    SENSOR_HUMIDITY_EXHAUST: Sensor("Exhaust Air Humidity", UNIT_PERCENT, 291, TYPE_CN_UINT8),
-    SENSOR_HUMIDITY_OUTDOOR: Sensor("Outdoor Air Humidity", UNIT_PERCENT, 292, TYPE_CN_UINT8),
-    SENSOR_HUMIDITY_AFTER_PREHEATER: Sensor("Outdoor Air Humidity (after preheater)", UNIT_PERCENT, 293, TYPE_CN_UINT8),
-    SENSOR_HUMIDITY_SUPPLY: Sensor("Supply Air Humidity", UNIT_PERCENT, 294, TYPE_CN_UINT8),
-    321: Sensor("sensor_321", None, 321, TYPE_CN_UINT16),
-    325: Sensor("sensor_325", None, 325, TYPE_CN_UINT16),
-    337: Sensor("sensor_337", None, 337, TYPE_CN_UINT32),
-    SENSOR_BYPASS_OVERRIDE: Sensor("Bypass Override", None, 338, TYPE_CN_UINT32),
-    341: Sensor("sensor_341", None, 341, TYPE_CN_UINT32),
-    SENSOR_FAN_MODE_SUPPLY_3: Sensor("Supply Fan Mode", None, 342, TYPE_CN_UINT32),
-    SENSOR_FAN_MODE_EXHAUST_3: Sensor("Exhaust Fan Mode", None, 343, TYPE_CN_UINT32),
-    SENSOR_ANALOG_INPUT_1: Sensor("Analog Input 1", None, 369, TYPE_CN_UINT8),
-    SENSOR_ANALOG_INPUT_2: Sensor("Analog Input 2", None, 370, TYPE_CN_UINT8),
-    SENSOR_ANALOG_INPUT_3: Sensor("Analog Input 3", None, 371, TYPE_CN_UINT8),
-    SENSOR_ANALOG_INPUT_4: Sensor("Analog Input 4", None, 372, TYPE_CN_UINT8),
-    384: Sensor("sensor_384", None, 384, TYPE_CN_INT16, lambda x: x / 10),
-    386: Sensor("sensor_386", None, 386, TYPE_CN_BOOL, bool),
-    400: Sensor("sensor_400", None, 400, TYPE_CN_INT16, lambda x: x / 10),
-    401: Sensor("sensor_401", None, 401, TYPE_CN_UINT8),
-    402: Sensor("sensor_402", None, 402, TYPE_CN_BOOL, bool),
-    416: Sensor("sensor_416", None, 416, TYPE_CN_INT16, lambda x: x / 10),
-    417: Sensor("sensor_417", None, 417, TYPE_CN_INT16, lambda x: x / 10),
-    418: Sensor("sensor_418", None, 418, TYPE_CN_UINT8),
-    419: Sensor("sensor_419", None, 419, TYPE_CN_BOOL, bool),
-    784: Sensor("sensor_784", None, 784, TYPE_CN_UINT8),
-    785: Sensor("sensor_785", None, 785, TYPE_CN_BOOL),
-    802: Sensor("sensor_802", None, 802, TYPE_CN_INT16, lambda x: x / 10),
+    SENSOR_DEVICE_STATE: Sensor("Device State", None, 16, PdoType.TYPE_CN_UINT8),
+    SENSOR_CHANGING_FILTERS: Sensor("Changing filters", None, 18, PdoType.TYPE_CN_UINT8),
+    33: Sensor("sensor_33", None, 33, PdoType.TYPE_CN_UINT8),
+    37: Sensor("sensor_37", None, 37, PdoType.TYPE_CN_UINT8),
+    SENSOR_OPERATING_MODE_2: Sensor("Operating Mode", None, 49, PdoType.TYPE_CN_UINT8),
+    53: Sensor("sensor_53", None, 53, PdoType.TYPE_CN_UINT8),
+    SENSOR_FAN_MODE_SUPPLY_2: Sensor("Supply Fan Mode", None, 54, PdoType.TYPE_CN_UINT8),
+    SENSOR_FAN_MODE_EXHAUST_2: Sensor("Exhaust Fan Mode", None, 55, PdoType.TYPE_CN_UINT8),
+    SENSOR_OPERATING_MODE: Sensor("Operating Mode", None, 56, PdoType.TYPE_CN_UINT8),
+    SENSOR_FAN_SPEED_MODE: Sensor("Fan Speed", None, 65, PdoType.TYPE_CN_UINT8),
+    SENSOR_BYPASS_ACTIVATION_STATE: Sensor("Bypass Activation State", None, 66, PdoType.TYPE_CN_UINT8),
+    SENSOR_PROFILE_TEMPERATURE: Sensor("Temperature Profile Mode", None, 67, PdoType.TYPE_CN_UINT8),
+    SENSOR_FAN_MODE_SUPPLY: Sensor("Supply Fan Mode", None, 70, PdoType.TYPE_CN_UINT8),
+    SENSOR_FAN_MODE_EXHAUST: Sensor("Exhaust Fan Mode", None, 71, PdoType.TYPE_CN_UINT8),
+    SENSOR_NEXT_CHANGE_FAN: Sensor("Fan Speed Next Change", None, 81, PdoType.TYPE_CN_UINT32),
+    SENSOR_NEXT_CHANGE_BYPASS: Sensor("Bypass Next Change", None, 82, PdoType.TYPE_CN_UINT32),
+    85: Sensor("sensor_85", None, 85, PdoType.TYPE_CN_UINT32),
+    SENSOR_NEXT_CHANGE_FAN_SUPPLY: Sensor("Supply Fan Next Change", None, 86, PdoType.TYPE_CN_UINT32),
+    SENSOR_NEXT_CHANGE_FAN_EXHAUST: Sensor("Exhaust Fan Next Change", None, 87, PdoType.TYPE_CN_UINT32),
+    SENSOR_FAN_EXHAUST_DUTY: Sensor("Exhaust Fan Duty", UNIT_PERCENT, 117, PdoType.TYPE_CN_UINT8),
+    SENSOR_FAN_SUPPLY_DUTY: Sensor("Supply Fan Duty", UNIT_PERCENT, 118, PdoType.TYPE_CN_UINT8),
+    SENSOR_FAN_EXHAUST_FLOW: Sensor("Exhaust Fan Flow", UNIT_M3H, 119, PdoType.TYPE_CN_UINT16),
+    SENSOR_FAN_SUPPLY_FLOW: Sensor("Supply Fan Flow", UNIT_M3H, 120, PdoType.TYPE_CN_UINT16),
+    SENSOR_FAN_EXHAUST_SPEED: Sensor("Exhaust Fan Speed", UNIT_RPM, 121, PdoType.TYPE_CN_UINT16),
+    SENSOR_FAN_SUPPLY_SPEED: Sensor("Supply Fan Speed", UNIT_RPM, 122, PdoType.TYPE_CN_UINT16),
+    SENSOR_POWER_USAGE: Sensor("Power Usage", UNIT_WATT, 128, PdoType.TYPE_CN_UINT16),
+    SENSOR_POWER_USAGE_TOTAL_YEAR: Sensor("Power Usage (year)", UNIT_KWH, 129, PdoType.TYPE_CN_UINT16),
+    SENSOR_POWER_USAGE_TOTAL: Sensor("Power Usage (total)", UNIT_KWH, 130, PdoType.TYPE_CN_UINT16),
+    SENSOR_PREHEATER_POWER_TOTAL_YEAR: Sensor("Preheater Power Usage (year)", UNIT_KWH, 144, PdoType.TYPE_CN_UINT16),
+    SENSOR_PREHEATER_POWER_TOTAL: Sensor("Preheater Power Usage (total)", UNIT_KWH, 145, PdoType.TYPE_CN_UINT16),
+    SENSOR_PREHEATER_POWER: Sensor("Preheater Power Usage", UNIT_WATT, 146, PdoType.TYPE_CN_UINT16),
+    SENSOR_RF_PAIRING_MODE: Sensor("RF Pairing Mode", None, 176, PdoType.TYPE_CN_UINT8),
+    SENSOR_DAYS_TO_REPLACE_FILTER: Sensor("Days remaining to replace the filter", None, 192, PdoType.TYPE_CN_UINT16),
+    SENSOR_UNIT_TEMPERATURE: Sensor("Device Temperature Unit", None, 208, PdoType.TYPE_CN_UINT8, lambda x: "celcius" if x == 0 else "farenheit"),
+    SENSOR_RMOT: Sensor("Running Mean Outdoor Temperature (RMOT)", UNIT_CELCIUS, 209, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    SENSOR_SEASON_HEATING_ACTIVE: Sensor("Heating Season is active", None, 210, PdoType.TYPE_CN_BOOL, bool),
+    SENSOR_SEASON_COOLING_ACTIVE: Sensor("Cooling Season is active", None, 211, PdoType.TYPE_CN_BOOL, bool),
+    SENSOR_TARGET_TEMPERATURE: Sensor("Target Temperature", UNIT_CELCIUS, 212, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    SENSOR_AVOIDED_HEATING: Sensor("Avoided Heating Power Usage", UNIT_WATT, 213, PdoType.TYPE_CN_UINT16),
+    SENSOR_AVOIDED_HEATING_TOTAL_YEAR: Sensor("Avoided Heating Power Usage (year)", UNIT_KWH, 214, PdoType.TYPE_CN_UINT16),
+    SENSOR_AVOIDED_HEATING_TOTAL: Sensor("Avoided Heating Power Usage (total)", UNIT_KWH, 215, PdoType.TYPE_CN_UINT16),
+    SENSOR_AVOIDED_COOLING: Sensor("Avoided Cooling Power Usage", UNIT_WATT, 216, PdoType.TYPE_CN_UINT16),
+    SENSOR_AVOIDED_COOLING_TOTAL_YEAR: Sensor("Avoided Cooling Power Usage (year)", UNIT_KWH, 217, PdoType.TYPE_CN_UINT16),
+    SENSOR_AVOIDED_COOLING_TOTAL: Sensor("Avoided Cooling Power Usage (total)", UNIT_KWH, 218, PdoType.TYPE_CN_UINT16),
+    219: Sensor("sensor_219", None, 219, PdoType.TYPE_CN_UINT16),
+    220: Sensor("Outdoor Air Temperature (?)", None, 220, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    SENSOR_TEMPERATURE_SUPPLY: Sensor("Supply Air Temperature", UNIT_CELCIUS, 221, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    SENSOR_UNIT_AIRFLOW: Sensor("Device Airflow Unit", None, 224, PdoType.TYPE_CN_UINT8, lambda x: "m3ph" if x == 3 else "lps"),
+    SENSOR_COMFORTCONTROL_MODE: Sensor("Sensor based ventilation mode", None, 225, PdoType.TYPE_CN_UINT8),
+    SENSOR_FAN_SPEED_MODE_MODULATED: Sensor("Fan Speed (modulated)", None, 226, PdoType.TYPE_CN_UINT16),
+    SENSOR_BYPASS_STATE: Sensor("Bypass State", UNIT_PERCENT, 227, PdoType.TYPE_CN_UINT8),
+    SENSOR_FROSTPROTECTION_UNBALANCE: Sensor("frostprotection_unbalance", None, 228, PdoType.TYPE_CN_UINT8),
+    SENSOR_AIRFLOW_CONSTRAINTS: Sensor("Airflow constraints", None, 230, PdoType.TYPE_CN_INT64, calculate_airflow_constraints),
+    SENSOR_TEMPERATURE_EXTRACT: Sensor("Extract Air Temperature", UNIT_CELCIUS, 274, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    SENSOR_TEMPERATURE_EXHAUST: Sensor("Exhaust Air Temperature", UNIT_CELCIUS, 275, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    SENSOR_TEMPERATURE_OUTDOOR: Sensor("Outdoor Air Temperature", UNIT_CELCIUS, 276, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    277: Sensor("Outdoor Air Temperature (?)", UNIT_CELCIUS, 277, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    278: Sensor("Supply Air Temperature (?)", UNIT_CELCIUS, 278, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    SENSOR_HUMIDITY_EXTRACT: Sensor("Extract Air Humidity", UNIT_PERCENT, 290, PdoType.TYPE_CN_UINT8),
+    SENSOR_HUMIDITY_EXHAUST: Sensor("Exhaust Air Humidity", UNIT_PERCENT, 291, PdoType.TYPE_CN_UINT8),
+    SENSOR_HUMIDITY_OUTDOOR: Sensor("Outdoor Air Humidity", UNIT_PERCENT, 292, PdoType.TYPE_CN_UINT8),
+    SENSOR_HUMIDITY_AFTER_PREHEATER: Sensor("Outdoor Air Humidity (after preheater)", UNIT_PERCENT, 293, PdoType.TYPE_CN_UINT8),
+    SENSOR_HUMIDITY_SUPPLY: Sensor("Supply Air Humidity", UNIT_PERCENT, 294, PdoType.TYPE_CN_UINT8),
+    321: Sensor("sensor_321", None, 321, PdoType.TYPE_CN_UINT16),
+    325: Sensor("sensor_325", None, 325, PdoType.TYPE_CN_UINT16),
+    337: Sensor("sensor_337", None, 337, PdoType.TYPE_CN_UINT32),
+    SENSOR_BYPASS_OVERRIDE: Sensor("Bypass Override", None, 338, PdoType.TYPE_CN_UINT32),
+    341: Sensor("sensor_341", None, 341, PdoType.TYPE_CN_UINT32),
+    SENSOR_FAN_MODE_SUPPLY_3: Sensor("Supply Fan Mode", None, 342, PdoType.TYPE_CN_UINT32),
+    SENSOR_FAN_MODE_EXHAUST_3: Sensor("Exhaust Fan Mode", None, 343, PdoType.TYPE_CN_UINT32),
+    SENSOR_ANALOG_INPUT_1: Sensor("Analog Input 1", None, 369, PdoType.TYPE_CN_UINT8),
+    SENSOR_ANALOG_INPUT_2: Sensor("Analog Input 2", None, 370, PdoType.TYPE_CN_UINT8),
+    SENSOR_ANALOG_INPUT_3: Sensor("Analog Input 3", None, 371, PdoType.TYPE_CN_UINT8),
+    SENSOR_ANALOG_INPUT_4: Sensor("Analog Input 4", None, 372, PdoType.TYPE_CN_UINT8),
+    384: Sensor("sensor_384", None, 384, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    386: Sensor("sensor_386", None, 386, PdoType.TYPE_CN_BOOL, bool),
+    400: Sensor("sensor_400", None, 400, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    401: Sensor("sensor_401", None, 401, PdoType.TYPE_CN_UINT8),
+    402: Sensor("sensor_402", None, 402, PdoType.TYPE_CN_BOOL, bool),
+    416: Sensor("sensor_416", None, 416, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    417: Sensor("sensor_417", None, 417, PdoType.TYPE_CN_INT16, lambda x: x / 10),
+    418: Sensor("sensor_418", None, 418, PdoType.TYPE_CN_UINT8),
+    419: Sensor("sensor_419", None, 419, PdoType.TYPE_CN_BOOL, bool),
+    784: Sensor("sensor_784", None, 784, PdoType.TYPE_CN_UINT8),
+    785: Sensor("sensor_785", None, 785, PdoType.TYPE_CN_BOOL),
+    802: Sensor("sensor_802", None, 802, PdoType.TYPE_CN_INT16, lambda x: x / 10),
 }
```

### Comparing `aiocomfoconnect-0.1.8/pyproject.toml` & `aiocomfoconnect-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "aiocomfoconnect"
-version = "0.1.8"
+version = "0.1.9"
 description = "aiocomfoconnect is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system"
 authors = ["Michaël Arnauts <michael.arnauts@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/michaelarnauts/aiocomfoconnect"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 aiohttp = "^3.8.0"
 protobuf = "^4.21.9"
 nanopb = "^0.4.6"
 
 [tool.poetry.group.dev.dependencies]
 grpcio-tools = "^1.50.0"
 dpkt = "^1.9.8"
@@ -24,15 +24,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
-target-version = ["py39", "py310"]
+target-version = ["py310"]
 line-length = 180
 
 [tool.pylint.MAIN]
 max-line-length = 180
 
 [tool.pylint."MESSAGES CONTROL"]
 # Reasons disabled:
```

### Comparing `aiocomfoconnect-0.1.8/PKG-INFO` & `aiocomfoconnect-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: aiocomfoconnect
-Version: 0.1.8
+Version: 0.1.9
 Summary: aiocomfoconnect is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system
 Home-page: https://github.com/michaelarnauts/aiocomfoconnect
 Author: Michaël Arnauts
 Author-email: michael.arnauts@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
 Requires-Dist: nanopb (>=0.4.6,<0.5.0)
 Requires-Dist: protobuf (>=4.21.9,<5.0.0)
 Description-Content-Type: text/markdown
 
 # aiocomfoconnect
 
 `aiocomfoconnect` is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system. It's the successor of
 [comfoconnect](https://github.com/michaelarnauts/comfoconnect).
 
-It's compatible with Python 3.8 and higher.
+It's compatible with Python 3.10 and higher.
 
 ## Installation
 
 ```shell
 pip3 install aiocomfoconnect
 ```
 
@@ -163,15 +161,15 @@
 ### Decode network traffic
 
 You can use the `scripts/decode_pcap.py` file to decode network traffic between the Mobile App and the ComfoConnect LAN C.
 Make sure that the first TCP session in the capture is the connection between the bridge and the app. It's therefore recommended to start the capture before you open the app.
 
 ```shell
 $ sudo tcpdump -i any -s 0 -w /tmp/capture.pcap tcp and port 56747
-$ python scripts/decode_pcap.py /tmp/capture.pcap
+$ python3 script/decode_pcap.py /tmp/capture.pcap
 ```
 
 ### Generate zehnder_pb2.py file
 
 ```shell
 pip3 install grpcio-tools
 python3 -m grpc_tools.protoc -Iprotobuf protobuf/nanopb.proto --python_out=aiocomfoconnect/protobuf
```

