# Comparing `tmp/pyftms-0.1.1.tar.gz` & `tmp/pyftms-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftms-0.1.1.tar", max compression
+gzip compressed data, was "pyftms-0.2.0.tar", max compression
```

## Comparing `pyftms-0.1.1.tar` & `pyftms-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11374 2024-05-28 12:37:45.517955 pyftms-0.1.1/LICENSE
--rw-r--r--   0        0        0      861 2024-05-28 12:37:45.517955 pyftms-0.1.1/README.md
--rw-r--r--   0        0        0     1604 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/__init__.py
--rw-r--r--   0        0        0      943 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/__main__.py
--rw-r--r--   0        0        0     3627 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/__init__.py
--rw-r--r--   0        0        0      695 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/backends/__init__.py
--rw-r--r--   0        0        0     8214 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/backends/controller.py
--rw-r--r--   0        0        0     5876 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/backends/event.py
--rw-r--r--   0        0        0     2039 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/backends/updater.py
--rw-r--r--   0        0        0    11059 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/client.py
--rw-r--r--   0        0        0     4841 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/const.py
--rw-r--r--   0        0        0      867 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/__init__.py
--rw-r--r--   0        0        0      599 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/cross_trainer.py
--rw-r--r--   0        0        0      576 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/indoor_bike.py
--rw-r--r--   0        0        0      542 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/rower.py
--rw-r--r--   0        0        0      553 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/treadmill.py
--rw-r--r--   0        0        0    10036 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/manager.py
--rw-r--r--   0        0        0      685 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/properties/__init__.py
--rw-r--r--   0        0        0     1063 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/properties/device_info.py
--rw-r--r--   0        0        0     5826 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/properties/features.py
--rw-r--r--   0        0        0     2448 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/properties/machine_type.py
--rw-r--r--   0        0        0     1117 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/__init__.py
--rw-r--r--   0        0        0     2530 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/common.py
--rw-r--r--   0        0        0     8956 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/control_point.py
--rw-r--r--   0        0        0     6442 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/machine_status.py
--rw-r--r--   0        0        0      374 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/__init__.py
--rw-r--r--   0        0        0     2823 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/common.py
--rw-r--r--   0        0        0     3075 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/cross_trainer.py
--rw-r--r--   0        0        0     2324 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/indoor_bike.py
--rw-r--r--   0        0        0     2973 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/rower.py
--rw-r--r--   0        0        0     2701 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/treadmill.py
--rw-r--r--   0        0        0     1255 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/models/spin_down.py
--rw-r--r--   0        0        0     2168 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/models/training_status.py
--rw-r--r--   0        0        0      471 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/__init__.py
--rw-r--r--   0        0        0      783 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/list.py
--rw-r--r--   0        0        0     7662 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/model.py
--rw-r--r--   0        0        0     2080 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/num.py
--rw-r--r--   0        0        0      594 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/serializer.py
--rw-r--r--   0        0        0      480 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 pyftms-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11374 2024-05-29 11:20:47.502093 pyftms-0.2.0/LICENSE
+-rw-r--r--   0        0        0      793 2024-05-29 11:20:47.502093 pyftms-0.2.0/README.md
+-rw-r--r--   0        0        0     1604 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/__init__.py
+-rw-r--r--   0        0        0      939 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/__main__.py
+-rw-r--r--   0        0        0     3573 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/backends/__init__.py
+-rw-r--r--   0        0        0     8214 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/backends/controller.py
+-rw-r--r--   0        0        0     6245 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/backends/event.py
+-rw-r--r--   0        0        0     2039 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/backends/updater.py
+-rw-r--r--   0        0        0    11045 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/client.py
+-rw-r--r--   0        0        0     4841 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/const.py
+-rw-r--r--   0        0        0      867 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/__init__.py
+-rw-r--r--   0        0        0      599 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/cross_trainer.py
+-rw-r--r--   0        0        0      576 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/indoor_bike.py
+-rw-r--r--   0        0        0      542 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/rower.py
+-rw-r--r--   0        0        0      553 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/treadmill.py
+-rw-r--r--   0        0        0    10069 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/manager.py
+-rw-r--r--   0        0        0      685 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/properties/__init__.py
+-rw-r--r--   0        0        0     1216 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/properties/device_info.py
+-rw-r--r--   0        0        0     5838 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/properties/features.py
+-rw-r--r--   0        0        0     2448 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/properties/machine_type.py
+-rw-r--r--   0        0        0     1117 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/__init__.py
+-rw-r--r--   0        0        0     2530 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/common.py
+-rw-r--r--   0        0        0     8956 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/control_point.py
+-rw-r--r--   0        0        0     6446 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/machine_status.py
+-rw-r--r--   0        0        0      374 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/__init__.py
+-rw-r--r--   0        0        0     2823 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/common.py
+-rw-r--r--   0        0        0     3075 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/cross_trainer.py
+-rw-r--r--   0        0        0     2324 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/indoor_bike.py
+-rw-r--r--   0        0        0     2973 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/rower.py
+-rw-r--r--   0        0        0     2701 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/treadmill.py
+-rw-r--r--   0        0        0     1350 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/spin_down.py
+-rw-r--r--   0        0        0     2194 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/training_status.py
+-rw-r--r--   0        0        0      471 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/list.py
+-rw-r--r--   0        0        0     7662 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/model.py
+-rw-r--r--   0        0        0     2080 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/num.py
+-rw-r--r--   0        0        0      594 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/serializer.py
+-rw-r--r--   0        0        0      480 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1289 1970-01-01 00:00:00.000000 pyftms-0.2.0/PKG-INFO
```

### Comparing `pyftms-0.1.1/LICENSE` & `pyftms-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/README.md` & `pyftms-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,22 @@
  1. **Treadmill**
  2. **Cross Trainer** (Elliptical Trainer)
  3. **Rower** (Rowing Machine)
  4. **Indoor Bike** (Spin Bike)
 
 **Step Climber** and **Stair Climber** machines are **not supported** due to incomplete protocol information and low popularity.
 
-!!! **API** !!! not stable and may be unsignifically changed.
-
 ## Requirments
 
-1. python >= 3.11;
-2. bleak >= 0.22;
-3. bleak-retry-connector >= 3.5.0.
+1. `python` >= 3.11;
+2. `bleak` >= 0.22;
+3. `bleak-retry-connector` >= 3.5.0.
 
 ## Install it from PyPI
 
 ```bash
 pip install pyftms
 ```
 
 ## Usage
 
-How to use please read the [documentation](https://dudanov.github.io/pyftms/pyftms.html).
+Please read API [documentation](https://dudanov.github.io/pyftms/pyftms.html).
```

### Comparing `pyftms-0.1.1/pyftms/__init__.py` & `pyftms-0.2.0/pyftms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/__main__.py` & `pyftms-0.2.0/pyftms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def on_event(event: FtmsEvents):
     print(f"New event: {event}")
 
 
 async def run():
-    async with await get_client_from_address(ADDRESS, on_event_callback=on_event) as c:
+    async with await get_client_from_address(ADDRESS, on_ftms_event=on_event) as c:
         properties = c.properties
         settings = c.settings
 
         print(f"Device Info: {c.device_info}")
         print(f"Supported: {c.supported_settings}")
         print(f"Supported: {c.supported_properties}")
         print(f"Available: {c.available_properties}")
```

### Comparing `pyftms-0.1.1/pyftms/client/__init__.py` & `pyftms-0.2.0/pyftms/client/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,53 +34,53 @@
 
 
 def get_client(
     ble_device: BLEDevice,
     adv_or_type: AdvertisementData | MachineType,
     *,
     timeout: float = 2.0,
-    on_event_callback: FtmsCallback | None = None,
+    on_ftms_event: FtmsCallback | None = None,
 ) -> FitnessMachine:
     """
     Creates an `FitnessMachine` instance from [Bleak](https://bleak.readthedocs.io/) discovered
     information: device and advertisement data. Instead of advertisement data, the `MachineType` can be used.
 
     Parameters:
     - `ble_device` - [BLE device](https://bleak.readthedocs.io/en/latest/api/index.html#bleak.backends.device.BLEDevice).
     - `adv_or_type` - Service [advertisement data](https://bleak.readthedocs.io/en/latest/backends/index.html#bleak.backends.scanner.AdvertisementData) or `MachineType`.
     - `timeout` - Control operation timeout. Defaults to 2.0s.
-    - `on_event_callback` - Callback for receiving fitness machine events.
+    - `on_ftms_event` - Callback for receiving fitness machine events.
 
     Return:
     - `FitnessMachine` instance.
     """
 
     if isinstance(adv_or_type, AdvertisementData):
         adv_or_type = get_machine_type_from_service_data(adv_or_type)
 
     cls = get_machine(adv_or_type)
 
-    return cls(ble_device, on_event_callback=on_event_callback, timeout=timeout)
+    return cls(ble_device, on_ftms_event=on_ftms_event, timeout=timeout)
 
 
 async def get_client_from_address(
     address: str,
     *,
     scan_timeout: float = 10.0,
     timeout: float = 2.0,
-    on_event_callback: FtmsCallback | None = None,
+    on_ftms_event: FtmsCallback | None = None,
 ) -> FitnessMachine:
     """
     Scans for fitness machine with specified BLE address. On success creates and return an `FitnessMachine` instance.
 
     Parameters:
     - `address` - The Bluetooth address of the device on this machine (UUID on macOS).
     - `scan_timeout` - Scanning timeout. Defaults to 10.0s.
     - `timeout` - Control operation timeout. Defaults to 2.0s.
-    - `on_event_callback` - Callback for receiving fitness machine events.
+    - `on_ftms_event` - Callback for receiving fitness machine events.
 
     Return:
     - `FitnessMachine` instance.
     """
 
     future: asyncio.Future[tuple[BLEDevice, AdvertisementData]] = asyncio.Future()
 
@@ -90,17 +90,15 @@
 
     scanner = BleakScanner(_on_device, [FITNESS_MACHINE_SERVICE_UUID])
 
     await scanner.start()
 
     try:
         dev, adv = await asyncio.wait_for(future, scan_timeout)
-        return get_client(
-            dev, adv, on_event_callback=on_event_callback, timeout=timeout
-        )
+        return get_client(dev, adv, on_ftms_event=on_ftms_event, timeout=timeout)
     finally:
         await scanner.stop()
 
 
 __all__ = [
     "get_client",
     "get_client_from_address",
```

### Comparing `pyftms-0.1.1/pyftms/client/backends/__init__.py` & `pyftms-0.2.0/pyftms/client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/backends/controller.py` & `pyftms-0.2.0/pyftms/client/backends/controller.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/backends/event.py` & `pyftms-0.2.0/pyftms/client/backends/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     SpinDownStatusCode,
     TrainingStatusCode,
 )
 from ..properties import MovementDirection
 
 FtmsNumbers = int | float
 ControlSource = Literal["callback", "user", "safety", "other"]
-SimpleControlEvents = Literal["start", "stop", "pause", "reset"]
+ControlEvents = Literal["start", "stop", "pause", "reset"]
 
 
 class SpinDownEventData(TypedDict, total=False):
     """`SpinDownEvent` data."""
 
     target_speed: SpinDownSpeedData
     """From fitness machine to client. Indicate successfully operation."""
@@ -39,21 +39,21 @@
 
     Units: `rpm`.
     """
     target_distance: int
     """
     Targeted distance.
 
-    Units: `meters`.
+    Units: `m`.
     """
     target_energy: int
     """
     Targeted expended energy.
 
-    Units: `kcals`.
+    Units: `kcal`.
     """
     target_heart_rate: int
     """
     Targeted heart rate.
 
     Units: `bpm`.
     """
@@ -63,15 +63,15 @@
 
     Units: `%`.
     """
     target_power: int
     """
     Targeted power.
 
-    Units: `Watts`.
+    Units: `Watt`.
     """
     target_resistance: float | int
     """
     Targeted resistance level.
 
     Units: `unitless`.
     """
@@ -81,27 +81,27 @@
 
     Units: `km/h`.
     """
     target_steps: int
     """
     Targeted number of steps.
 
-    Units: `steps`.
+    Units: `step`.
     """
     target_strides: int
     """
     Targeted number of strides.
 
-    Units: `strides`.
+    Units: `stride`.
     """
     target_time: tuple[int, ...]
     """
     Targeted training time.
 
-    Units: `seconds`.
+    Units: `s`.
     """
     wheel_circumference: float
     """
     Wheel circumference.
 
     Units: `mm`.
     """
@@ -186,75 +186,75 @@
 
     Units: `MovementDirection`.
     """
     pace_average: int | float
     """
     Average Pace.
 
-    Units: `Km/m` or `Seconds(500m)` for `Rower`.
+    Units: `km/m` or `seconds(500m)` for `Rower`.
     """
     pace_instant: int | float
     """
     Instantaneous Pace.
 
-    Units: `Km/m` or `Seconds(500m)` for `Rower`.
+    Units: `km/m` or `seconds(500m)` for `Rower`.
     """
     power_average: int
     """
     Average Power.
 
-    Units: `Watts`.
+    Units: `Watt`.
     """
     power_instant: int
     """
     Instantaneous Power.
 
-    Units: `Watts`.
+    Units: `Watt`.
     """
     power_output: int
     """
     Power Output.
 
-    Units: `Watts`.
+    Units: `Watt`.
     """
     ramp_angle: float
     """
     Ramp Angle Setting.
 
-    Units: `deg`.
+    Units: `degree`.
     """
     resistance_level: int | float
     """
     Resistance Level.
 
     Units: `unitless`.
     """
     speed_average: float
     """
     Average Speed.
 
-    Units: `Km/h`.
+    Units: `km/h`.
     """
     speed_instant: float
     """
     Instantaneous Speed.
 
-    Units: `Km/h`.
+    Units: `km/h`.
     """
     step_rate_average: int
     """
     Average Step Rate.
 
-    Units: `step_per_minute`.
+    Units: `step/m`.
     """
     step_rate_instant: int
     """
     Instantaneous Step Rate.
 
-    Units: `step_per_minute`.
+    Units: `step/m`.
     """
     stride_count: int
     """
     Stride Count.
 
     Units: `unitless`.
     """
@@ -290,51 +290,64 @@
     """
 
 
 class TrainingStatusEventData(TypedDict):
     """`TrainingStatusEvent` data."""
 
     code: TrainingStatusCode
+    """Training Status Code."""
     string: NotRequired[str]
+    """Extended string."""
 
 
 class TrainingStatusEvent(NamedTuple):
     """Training Status Event."""
 
     event_id: Literal["training_status"]
+    """Always `training_status`."""
     event_data: TrainingStatusEventData
+    """`TrainingStatusEvent` data."""
 
 
 class UpdateEvent(NamedTuple):
     """Update Event."""
 
     event_id: Literal["update"]
+    """Always `update`."""
     event_data: UpdateEventData
+    """`UpdateEvent` data."""
 
 
 class SpinDownEvent(NamedTuple):
     """Spin Down Procedure Event."""
 
     event_id: Literal["spin_down"]
+    """Always `spin_down`."""
     event_data: SpinDownEventData
+    """`SpinDownEvent` data."""
 
 
 class SetupEvent(NamedTuple):
     """Setting Event."""
 
     event_id: Literal["setup"]
+    """Always `setup`."""
     event_data: SetupEventData
+    """`SetupEvent` data."""
     event_source: ControlSource
+    """Reason of event."""
 
 
 class ControlEvent(NamedTuple):
     """Control Event."""
 
-    event_id: SimpleControlEvents
+    event_id: ControlEvents
+    """One of: `start`, `stop`, `pause`, `reset`."""
     event_source: ControlSource
+    """Reason of event."""
 
 
 FtmsEvents = (
     UpdateEvent | SetupEvent | ControlEvent | TrainingStatusEvent | SpinDownEvent
 )
 """Tagged union of FTMS events."""
```

### Comparing `pyftms-0.1.1/pyftms/client/backends/updater.py` & `pyftms-0.2.0/pyftms/client/backends/updater.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/client.py` & `pyftms-0.2.0/pyftms/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     ControlModel,
     IndoorBikeSimulationParameters,
     RealtimeData,
     ResultCode,
     SpinDownControlCode,
     StopPauseCode,
 )
+from . import const as c
 from .backends import DataUpdater, FtmsCallback, MachineController
 from .manager import PropertiesManager
 from .properties import (
     DeviceInfo,
     MachineFeatures,
     MachineSettings,
     MachineType,
@@ -69,17 +70,17 @@
     _settings_ranges: MappingProxyType[str, SettingRange]
 
     def __init__(
         self,
         ble_device: BLEDevice,
         *,
         timeout: float = 2.0,
-        on_event_callback: FtmsCallback | None = None,
+        on_ftms_event: FtmsCallback | None = None,
     ) -> None:
-        super().__init__(on_event_callback)
+        super().__init__(on_ftms_event)
 
         self._device = ble_device
         self._timeout = timeout
 
         # Updaters
         self._data_updater = DataUpdater(self._data_model, self._on_event)
         self._controller = MachineController(self._on_event)
@@ -262,119 +263,119 @@
 
     async def set_target_speed(self, value: float) -> ResultCode:
         """
         Sets target speed.
 
         Units: `km/h`.
         """
-        return await self.set_setting("target_speed", value)
+        return await self.set_setting(c.TARGET_SPEED, value)
 
     async def set_target_inclination(self, value: float) -> ResultCode:
         """
         Sets target inclination.
 
         Units: `%`.
         """
-        return await self.set_setting("target_inclination", value)
+        return await self.set_setting(c.TARGET_INCLINATION, value)
 
     async def set_target_resistance(self, value: float) -> ResultCode:
         """
         Sets target resistance level.
 
         Units: `unitless`.
         """
-        return await self.set_setting("target_resistance", value)
+        return await self.set_setting(c.TARGET_RESISTANCE, value)
 
     async def set_target_power(self, value: int) -> ResultCode:
         """
         Sets target power.
 
-        Units: `Watts`.
+        Units: `Watt`.
         """
-        return await self.set_setting("target_power", value)
+        return await self.set_setting(c.TARGET_POWER, value)
 
     async def set_target_heart_rate(self, value: int) -> ResultCode:
         """
         Sets target heart rate.
 
         Units: `bpm`.
         """
-        return await self.set_setting("target_heart_rate", value)
+        return await self.set_setting(c.TARGET_HEART_RATE, value)
 
     async def set_target_energy(self, value: int) -> ResultCode:
         """
         Sets target expended energy.
 
-        Units: `kcals`.
+        Units: `kcal`.
         """
-        return await self.set_setting("target_energy", value)
+        return await self.set_setting(c.TARGET_ENERGY, value)
 
     async def set_target_steps(self, value: int) -> ResultCode:
         """
         Sets targeted number of steps.
 
-        Units: `steps`.
+        Units: `step`.
         """
-        return await self.set_setting("target_steps", value)
+        return await self.set_setting(c.TARGET_STEPS, value)
 
     async def set_target_strides(self, value: int) -> ResultCode:
         """
         Sets targeted number of strides.
 
-        Units: `strides`.
+        Units: `stride`.
         """
-        return await self.set_setting("target_strides", value)
+        return await self.set_setting(c.TARGET_STRIDES, value)
 
     async def set_target_distance(self, value: int) -> ResultCode:
         """
         Sets targeted distance.
 
-        Units: `meters`.
+        Units: `m`.
         """
-        return await self.set_setting("target_distance", value)
+        return await self.set_setting(c.TARGET_DISTANCE, value)
 
     async def set_target_time(self, *value: int) -> ResultCode:
         """
         Set targeted training time.
 
-        Units: `seconds`.
+        Units: `s`.
         """
-        return await self.set_setting("target_time", *value)
+        return await self.set_setting(c.TARGET_TIME, *value)
 
-    async def set_bike_simulation_params(
+    async def set_indoor_bike_simulation(
         self,
         value: IndoorBikeSimulationParameters,
     ) -> ResultCode:
         """Set indoor bike simulation parameters."""
-        return await self.set_setting("indoor_bike_simulation", value)
+        return await self.set_setting(c.INDOOR_BIKE_SIMULATION, value)
 
     async def set_wheel_circumference(self, value: float) -> ResultCode:
         """
         Set wheel circumference.
 
         Units: `mm`.
         """
-        return await self.set_setting("wheel_circumference", value)
+        return await self.set_setting(c.WHEEL_CIRCUMFERENCE, value)
 
     async def spin_down_start(self) -> ResultCode:
         """
         Start Spin-Down.
 
         It can be sent either in response to a request to start Spin-Down, or separately.
         """
-        return await self.set_setting("spin_down_control", SpinDownControlCode.START)
+        return await self.set_setting(c.SPIN_DOWN, SpinDownControlCode.START)
 
     async def spin_down_ignore(self) -> ResultCode:
         """
         Ignore Spin-Down.
 
         It can be sent in response to a request to start Spin-Down.
         """
-        return await self.set_setting("spin_down_control", SpinDownControlCode.IGNORE)
+        return await self.set_setting(c.SPIN_DOWN, SpinDownControlCode.IGNORE)
 
     async def set_target_cadence(self, value: float) -> ResultCode:
         """
         Set targeted cadence.
 
         Units: `rpm`.
         """
-        return await self.set_setting("target_cadence", value)
+        return await self.set_setting(c.TARGET_CADENCE, value)
```

### Comparing `pyftms-0.1.1/pyftms/client/const.py` & `pyftms-0.2.0/pyftms/client/const.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/machines/__init__.py` & `pyftms-0.2.0/pyftms/client/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/machines/cross_trainer.py` & `pyftms-0.2.0/pyftms/client/machines/cross_trainer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/machines/indoor_bike.py` & `pyftms-0.2.0/pyftms/client/machines/indoor_bike.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/machines/rower.py` & `pyftms-0.2.0/pyftms/client/machines/rower.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/machines/treadmill.py` & `pyftms-0.2.0/pyftms/client/machines/treadmill.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/manager.py` & `pyftms-0.2.0/pyftms/client/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     _settings: SetupEventData
     """Properties dictonary"""
 
     _training_status: TrainingStatusCode
     """Last Training Status Code"""
 
-    def __init__(self, on_event_callback: FtmsCallback | None = None) -> None:
-        self._cb = on_event_callback
+    def __init__(self, on_ftms_event: FtmsCallback | None = None) -> None:
+        self._cb = on_ftms_event
         self._properties = {}
         self._settings = {}
 
     def set_callback(self, cb: FtmsCallback):
         self._cb = cb
 
     def _on_event(self, e: FtmsEvents) -> None:
@@ -48,14 +48,17 @@
             self._training_status = e.event_data["code"]
 
         return self._cb and self._cb(e)
 
     def _get_property(self, name: str) -> Any:
         return self._properties.get(name)
 
+    def _get_setting(self, name: str) -> Any:
+        return self._settings.get(name)
+
     @property
     def properties(self) -> UpdateEventData:
         """Read-only updateable properties mapping."""
         return cast(UpdateEventData, MappingProxyType(self._properties))
 
     @property
     def settings(self) -> SetupEventData:
@@ -186,60 +189,60 @@
         return self._get_property(c.MOVEMENT_DIRECTION)
 
     @property
     def pace_average(self) -> int | float:
         """
         Average Pace.
 
-        Units: `Km/m` or `Seconds(500m)` for `Rower`.
+        Units: `km/m` or `seconds(500m)` for `Rower`.
         """
         return self._get_property(c.PACE_AVERAGE)
 
     @property
     def pace_instant(self) -> int | float:
         """
         Instantaneous Pace.
 
-        Units: `Km/m` or `Seconds(500m)` for `Rower`.
+        Units: `km/m` or `seconds(500m)` for `Rower`.
         """
         return self._get_property(c.PACE_INSTANT)
 
     @property
     def power_average(self) -> int:
         """
         Average Power.
 
-        Units: `Watts`.
+        Units: `Watt`.
         """
         return self._get_property(c.POWER_AVERAGE)
 
     @property
     def power_instant(self) -> int:
         """
         Instantaneous Power.
 
-        Units: `Watts`.
+        Units: `Watt`.
         """
         return self._get_property(c.POWER_INSTANT)
 
     @property
     def power_output(self) -> int:
         """
         Power Output.
 
-        Units: `Watts`.
+        Units: `Watt`.
         """
         return self._get_property(c.POWER_OUTPUT)
 
     @property
     def ramp_angle(self) -> float:
         """
         Ramp Angle Setting.
 
-        Units: `deg`.
+        Units: `degree`.
         """
         return self._get_property(c.RAMP_ANGLE)
 
     @property
     def resistance_level(self) -> int | float:
         """
         Resistance Level.
@@ -249,42 +252,42 @@
         return self._get_property(c.RESISTANCE_LEVEL)
 
     @property
     def speed_average(self) -> float:
         """
         Average Speed.
 
-        Units: `Km/h`.
+        Units: `km/h`.
         """
         return self._get_property(c.SPEED_AVERAGE)
 
     @property
     def speed_instant(self) -> float:
         """
         Instantaneous Speed.
 
-        Units: `Km/h`.
+        Units: `km/h`.
         """
         return self._get_property(c.SPEED_INSTANT)
 
     @property
     def step_rate_average(self) -> int:
         """
         Average Step Rate.
 
-        Units: `step_per_minute`.
+        Units: `step/m`.
         """
         return self._get_property(c.STEP_RATE_AVERAGE)
 
     @property
     def step_rate_instant(self) -> int:
         """
         Instantaneous Step Rate.
 
-        Units: `step_per_minute`.
+        Units: `step/m`.
         """
         return self._get_property(c.STEP_RATE_INSTANT)
 
     @property
     def stride_count(self) -> int:
         """
         Stride Count.
@@ -339,116 +342,116 @@
         return self._get_property(c.TIME_REMAINING)
 
     # SETTINGS
 
     @property
     def indoor_bike_simulation(self) -> IndoorBikeSimulationParameters:
         """Indoor Bike Simulation Parameters."""
-        return self._get_property(c.INDOOR_BIKE_SIMULATION)
+        return self._get_setting(c.INDOOR_BIKE_SIMULATION)
 
     @property
     def target_cadence(self) -> float:
         """
         Targeted cadence.
 
         Units: `rpm`.
         """
-        return self._get_property(c.TARGET_CADENCE)
+        return self._get_setting(c.TARGET_CADENCE)
 
     @property
     def target_distance(self) -> int:
         """
         Targeted distance.
 
-        Units: `meters`.
+        Units: `m`.
         """
-        return self._get_property(c.TARGET_DISTANCE)
+        return self._get_setting(c.TARGET_DISTANCE)
 
     @property
     def target_energy(self) -> int:
         """
         Targeted expended energy.
 
-        Units: `kcals`.
+        Units: `kcal`.
         """
-        return self._get_property(c.TARGET_ENERGY)
+        return self._get_setting(c.TARGET_ENERGY)
 
     @property
     def target_heart_rate(self) -> int:
         """
         Targeted heart rate.
 
         Units: `bpm`.
         """
-        return self._get_property(c.TARGET_HEART_RATE)
+        return self._get_setting(c.TARGET_HEART_RATE)
 
     @property
     def target_inclination(self) -> float:
         """
         Targeted inclination.
 
         Units: `%`.
         """
-        return self._get_property(c.TARGET_INCLINATION)
+        return self._get_setting(c.TARGET_INCLINATION)
 
     @property
     def target_power(self) -> int:
         """
         Targeted power.
 
-        Units: `Watts`.
+        Units: `Watt`.
         """
-        return self._get_property(c.TARGET_POWER)
+        return self._get_setting(c.TARGET_POWER)
 
     @property
     def target_resistance(self) -> float:
         """
         Targeted resistance level.
 
         Units: `unitless`.
         """
-        return self._get_property(c.TARGET_RESISTANCE)
+        return self._get_setting(c.TARGET_RESISTANCE)
 
     @property
     def target_speed(self) -> float:
         """
         Targeted speed.
 
         Units: `km/h`.
         """
-        return self._get_property(c.TARGET_SPEED)
+        return self._get_setting(c.TARGET_SPEED)
 
     @property
     def target_steps(self) -> int:
         """
         Targeted number of steps.
 
-        Units: `steps`.
+        Units: `step`.
         """
-        return self._get_property(c.TARGET_STEPS)
+        return self._get_setting(c.TARGET_STEPS)
 
     @property
     def target_strides(self) -> int:
         """
         Targeted number of strides.
 
-        Units: `strides`.
+        Units: `stride`.
         """
-        return self._get_property(c.TARGET_STRIDES)
+        return self._get_setting(c.TARGET_STRIDES)
 
     @property
     def target_time(self) -> tuple[int, ...]:
         """
         Targeted training time.
 
-        Units: `seconds`.
+        Units: `s`.
         """
-        return self._get_property(c.TARGET_TIME)
+        return self._get_setting(c.TARGET_TIME)
 
     @property
     def wheel_circumference(self) -> float:
         """
         Wheel circumference.
 
         Units: `mm`.
         """
-        return self._get_property(c.WHEEL_CIRCUMFERENCE)
+        return self._get_setting(c.WHEEL_CIRCUMFERENCE)
```

### Comparing `pyftms-0.1.1/pyftms/client/properties/__init__.py` & `pyftms-0.2.0/pyftms/client/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/client/properties/device_info.py` & `pyftms-0.2.0/pyftms/client/properties/device_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,19 +17,26 @@
     "hw_version": 0x2A27,
 }
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceInfo(TypedDict, total=False):
+    """Device Information."""
+
     manufacturer: str
+    """Manufacturer."""
     model: str
+    """Model."""
     serial_number: str
+    """Serial Number."""
     sw_version: str
+    """Software Version."""
     hw_version: str
+    """Hardware Version."""
 
 
 async def read_device_info(cli: BleakClient) -> DeviceInfo:
     """Read Device Information."""
 
     _LOGGER.debug("Reading Device Information.")
```

### Comparing `pyftms-0.1.1/pyftms/client/properties/features.py` & `pyftms-0.2.0/pyftms/client/properties/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     """
     Movement direction. Used by `CrossTrainer` machine only.
 
     Described in section **4.5.1.1 Flags Field**.
     """
 
     FORWARD = auto()
-    """Forward"""
+    """Move Forward."""
     BACKWARD = auto()
-    """Backward"""
+    """Move Backward."""
 
 
 class MachineFeatures(IntFlag, boundary=STRICT):
     """
     Fitness Machine Features.
 
     Described in section `4.3.1.1: Fitness Machine Features Field`.
```

### Comparing `pyftms-0.1.1/pyftms/client/properties/machine_type.py` & `pyftms-0.2.0/pyftms/client/properties/machine_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,31 +24,31 @@
     """Fitness Machine Available"""
 
 
 class MachineType(Flag):
     """
     Fitness Machine Type.
 
-    Included in the `Service Data AD Type`.
+    Included in the Advertisement Service Data.
 
-    Described in section `3.1.2: Fitness Machine Type Field`.
+    Described in section **3.1.2: Fitness Machine Type Field**.
     """
 
     TREADMILL = auto()
-    """Treadmill Supported"""
+    """Treadmill Machine."""
     CROSS_TRAINER = auto()
-    """Cross Trainer Supported"""
+    """Cross Trainer Machine."""
     STEP_CLIMBER = auto()
-    """Step Climber Supported"""
+    """Step Climber Machine."""
     STAIR_CLIMBER = auto()
-    """Stair Climber Supported"""
+    """Stair Climber Machine."""
     ROWER = auto()
-    """Rower Supported"""
+    """Rower Machine."""
     INDOOR_BIKE = auto()
-    """Indoor Bike Supported"""
+    """Indoor Bike Machine."""
 
 
 class NotFitnessMachineError(Exception):
     """
     An exception if the FTMS service is not supported by the Bluetooth device.
 
     May be raised in `get_machine_type_from_service_data` and `get_client`
```

### Comparing `pyftms-0.1.1/pyftms/models/__init__.py` & `pyftms-0.2.0/pyftms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/models/common.py` & `pyftms-0.2.0/pyftms/models/common.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/models/control_point.py` & `pyftms-0.2.0/pyftms/models/control_point.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/models/machine_status.py` & `pyftms-0.2.0/pyftms/models/machine_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .spin_down import SpinDownStatusCode
 
 
 class MachineStatusCode(IntEnum, boundary=STRICT):
     """
     Fitness Machine Status.
 
-    Described in section `4.16.1: Fitness Machine Control Point Procedure Requirements`.
+    Described in section **4.16.1: Fitness Machine Control Point Procedure Requirements**.
     """
 
     RESET = auto()
     """Reset"""
 
     STOP_PAUSE = auto()
     """Fitness Machine Stopped or Paused by the User"""
@@ -88,15 +88,15 @@
 
 
 @dc.dataclass(frozen=True)
 class MachineStatusModel(CodeSwitchModel[MachineStatusCode]):
     """
     Structure of the Fitness Machine Status characteristic.
 
-    Described in section `4.17 Fitness Machine Status`.
+    Described in section **4.17 Fitness Machine Status**.
     """
 
     stop_pause: StopPauseCode | None = dc.field(
         default=None,
         metadata=model_meta(
             format="u1",
             code=MachineStatusCode.STOP_PAUSE,
```

### Comparing `pyftms-0.1.1/pyftms/models/realtime_data/common.py` & `pyftms-0.2.0/pyftms/models/realtime_data/common.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/models/realtime_data/cross_trainer.py` & `pyftms-0.2.0/pyftms/models/realtime_data/cross_trainer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/models/realtime_data/indoor_bike.py` & `pyftms-0.2.0/pyftms/models/realtime_data/indoor_bike.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/models/realtime_data/rower.py` & `pyftms-0.2.0/pyftms/models/realtime_data/rower.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/models/realtime_data/treadmill.py` & `pyftms-0.2.0/pyftms/models/realtime_data/treadmill.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/models/spin_down.py` & `pyftms-0.2.0/pyftms/models/spin_down.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .common import BaseModel, model_meta
 
 
 class SpinDownStatusCode(IntEnum, boundary=STRICT):
     """
     Spin Down Status.
 
-    Described in section `4.17 Fitness Machine Status. Table 4.27`.
+    Described in section **4.17 Fitness Machine Status. Table 4.27**.
     """
 
     REQUESTED = auto()
     """Spin Down Requested"""
 
     SUCCESS = auto()
     """Success"""
@@ -25,40 +25,48 @@
 
     STOP_PEDALING = auto()
     """Stop Pedaling"""
 
 
 class SpinDownControlCode(IntEnum, boundary=STRICT):
     """
-    Spin Down Status.
+    Spin Down Control Code.
 
-    Described in section `4.17 Fitness Machine Status. Table 4.27`.
+    Described in section **4.16.2.20 Spin Down Control Procedure. Table 4.21**.
     """
 
     START = auto()
-    """Spin Down Requested"""
+    """Spin Down Start."""
 
     IGNORE = auto()
-    """Success"""
+    """Spin Down Ignore."""
 
 
 @dc.dataclass(frozen=True)
 class SpinDownSpeedData(BaseModel):
     """
     Response Parameter when the Spin Down Procedure succeeds.
 
-    Described in section `4.16.2.20 Spin Down Control Procedure`.
+    Described in section `4.16.2.20 Spin Down Control Procedure. Table 4.22`.
     """
 
     low: float = dc.field(
         metadata=model_meta(
             format="u2.01",
         )
     )
-    """Target Speed Low | km/h"""
+    """
+    Target Speed Low.
+    
+    Units: `km/h`.
+    """
 
     high: float = dc.field(
         metadata=model_meta(
             format="u2.01",
         )
     )
-    """Target Speed High | km/h"""
+    """
+    Target Speed High.
+    
+    Units: `km/h`.
+    """
```

### Comparing `pyftms-0.1.1/pyftms/models/training_status.py` & `pyftms-0.2.0/pyftms/models/training_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,96 +9,96 @@
 
 class TrainingStatusFlags(IntFlag, boundary=STRICT):
     """
     Training Status.
 
     Represents the current training state while a user is exercising.
 
-    Described in section `4.10.1.2: Training Status Field`.
+    Described in section **4.10.1.2: Training Status Field**.
     """
 
     STRING_PRESENT = auto()
-    """Other"""
+    """Other."""
 
     EXTENDED_STRING = auto()
-    """Idle"""
+    """Idle."""
 
 
 class TrainingStatusCode(IntEnum, boundary=STRICT):
     """
     Training Status.
 
     Represents the current training state while a user is exercising.
 
-    Described in section `4.10.1.2: Training Status Field`.
+    Described in section **4.10.1.2: Training Status Field**.
     """
 
     OTHER = 0
-    """Other"""
+    """Other."""
 
     IDLE = auto()
-    """Idle"""
+    """Idle."""
 
     WARMING_UP = auto()
-    """Warming Up"""
+    """Warming Up."""
 
     LOW_INTENSITY_INTERVAL = auto()
-    """Low Intensity Interval"""
+    """Low Intensity Interval."""
 
     HIGH_INTENSITY_INTERVAL = auto()
-    """High Intensity Interval"""
+    """High Intensity Interval."""
 
     RECOVERY_INTERVAL = auto()
-    """Recovery Interval"""
+    """Recovery Interval."""
 
     ISOMETRIC = auto()
-    """Isometric"""
+    """Isometric."""
 
     HEART_RATE_CONTROL = auto()
-    """Heart Rate Control"""
+    """Heart Rate Control."""
 
     FITNESS_TEST = auto()
-    """Fitness Test"""
+    """Fitness Test."""
 
     SPEED_TOO_LOW = auto()
-    """Speed Outside of Control Region - Low (increase speed to return to controllable region)"""
+    """Speed Outside of Control Region - Low (increase speed to return to controllable region)."""
 
     SPEED_TOO_HIGH = auto()
-    """Speed Outside of Control Region - High (decrease speed to return to controllable region)"""
+    """Speed Outside of Control Region - High (decrease speed to return to controllable region)."""
 
     COOL_DOWN = auto()
-    """Cool Down"""
+    """Cool Down."""
 
     WATT_CONTROL = auto()
-    """Watt Control"""
+    """Watt Control."""
 
     MANUAL_MODE = auto()
-    """Manual Mode (Quick Start)"""
+    """Manual Mode (Quick Start)."""
 
     PRE_WORKOUT = auto()
-    """Pre-Workout"""
+    """Pre-Workout."""
 
     POST_WORKOUT = auto()
-    """Post-Workout"""
+    """Post-Workout."""
 
 
 @dc.dataclass(frozen=True)
 class TrainingStatusModel(BaseModel):
     """
     Structure of the Training Status Characteristic.
 
-    Described in section `4.10 Training Status`.
+    Described in section **4.10 Training Status**.
     """
 
     flags: TrainingStatusFlags = dc.field(
         metadata=model_meta(
             format="u1",
         )
     )
-    """Flags Field"""
+    """Flags Field."""
 
     code: TrainingStatusCode = dc.field(
         metadata=model_meta(
             format="u1",
         )
     )
-    """Training Status Field"""
+    """Training Status Field."""
```

### Comparing `pyftms-0.1.1/pyftms/serializer/list.py` & `pyftms-0.2.0/pyftms/serializer/list.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/serializer/model.py` & `pyftms-0.2.0/pyftms/serializer/model.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/serializer/num.py` & `pyftms-0.2.0/pyftms/serializer/num.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/pyftms/serializer/serializer.py` & `pyftms-0.2.0/pyftms/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.1.1/PKG-INFO` & `pyftms-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyftms
-Version: 0.1.1
+Version: 0.2.0
 Summary: PyFTMS - Python Fitness Machine Service client library.
 Author: Sergey V. DUDANOV
 Author-email: sergey.dudanov@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -18,25 +18,23 @@
  1. **Treadmill**
  2. **Cross Trainer** (Elliptical Trainer)
  3. **Rower** (Rowing Machine)
  4. **Indoor Bike** (Spin Bike)
 
 **Step Climber** and **Stair Climber** machines are **not supported** due to incomplete protocol information and low popularity.
 
-!!! **API** !!! not stable and may be unsignifically changed.
-
 ## Requirments
 
-1. python >= 3.11;
-2. bleak >= 0.22;
-3. bleak-retry-connector >= 3.5.0.
+1. `python` >= 3.11;
+2. `bleak` >= 0.22;
+3. `bleak-retry-connector` >= 3.5.0.
 
 ## Install it from PyPI
 
 ```bash
 pip install pyftms
 ```
 
 ## Usage
 
-How to use please read the [documentation](https://dudanov.github.io/pyftms/pyftms.html).
+Please read API [documentation](https://dudanov.github.io/pyftms/pyftms.html).
```

