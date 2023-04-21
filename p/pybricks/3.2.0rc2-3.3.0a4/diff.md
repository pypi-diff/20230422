# Comparing `tmp/pybricks-3.2.0rc2.tar.gz` & `tmp/pybricks-3.3.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybricks-3.2.0rc2.tar", max compression
+gzip compressed data, was "pybricks-3.3.0a4.tar", max compression
```

## Comparing `pybricks-3.2.0rc2.tar` & `pybricks-3.3.0a4.tar`

### file list

```diff
@@ -1,38 +1,36 @@
--rw-r--r--   0        0        0     1082 2022-12-20 15:10:19.722150 pybricks-3.2.0rc2/LICENSE
--rw-r--r--   0        0        0      890 2022-12-20 15:10:19.722150 pybricks-3.2.0rc2/README.rst
--rw-r--r--   0        0        0     1352 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4264 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/micropython/__init__.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/micropython/py.typed
--rw-r--r--   0        0        0      122 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/__init__.py
--rw-r--r--   0        0        0    34829 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/_common.py
--rw-r--r--   0        0        0     4511 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/ev3dev/_speaker.py
--rw-r--r--   0        0        0     6651 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/ev3devices.py
--rw-r--r--   0        0        0     3150 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/geometry.py
--rw-r--r--   0        0        0     4760 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/hubs.py
--rw-r--r--   0        0        0     8418 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/iodevices.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/media/__init__.py
--rw-r--r--   0        0        0    20861 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/media/ev3dev.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/media/py.typed
--rw-r--r--   0        0        0     6524 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/messaging.py
--rw-r--r--   0        0        0     6671 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/nxtdevices.py
--rw-r--r--   0        0        0    12046 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/parameters.py
--rw-r--r--   0        0        0    11285 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/pupdevices.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/py.typed
--rw-r--r--   0        0        0     7539 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/robotics.py
--rw-r--r--   0        0        0     2589 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/pybricks/tools.py
--rw-r--r--   0        0        0     1409 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/uerrno/__init__.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/uerrno/py.typed
--rw-r--r--   0        0        0     2523 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/uio/__init__.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/uio/py.typed
--rw-r--r--   0        0        0     2007 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/ujson/__init__.py
--rw-r--r--   0        0        0     6378 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/umath/__init__.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/umath/py.typed
--rw-r--r--   0        0        0     3156 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/urandom/__init__.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/urandom/py.typed
--rw-r--r--   0        0        0     4952 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/uselect/__init__.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/uselect/py.typed
--rw-r--r--   0        0        0     2280 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/ustruct/__init__.py
--rw-r--r--   0        0        0     1402 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/usys/__init__.py
--rw-r--r--   0        0        0        0 2022-12-20 15:10:19.846148 pybricks-3.2.0rc2/src/usys/py.typed
--rw-r--r--   0        0        0     1942 1970-01-01 00:00:00.000000 pybricks-3.2.0rc2/setup.py
--rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 pybricks-3.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-21 22:02:04.318688 pybricks-3.3.0a4/LICENSE
+-rw-r--r--   0        0        0     1185 2023-04-21 22:02:04.318688 pybricks-3.3.0a4/README.rst
+-rw-r--r--   0        0        0     1352 2023-04-21 22:02:04.442687 pybricks-3.3.0a4/pyproject.toml
+-rw-r--r--   0        0        0     4264 2023-04-21 22:02:04.442687 pybricks-3.3.0a4/src/micropython/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.442687 pybricks-3.3.0a4/src/micropython/py.typed
+-rw-r--r--   0        0        0      122 2023-04-21 22:02:04.442687 pybricks-3.3.0a4/src/pybricks/__init__.py
+-rw-r--r--   0        0        0    41142 2023-04-21 22:02:04.442687 pybricks-3.3.0a4/src/pybricks/_common.py
+-rw-r--r--   0        0        0     4511 2023-04-21 22:02:04.442687 pybricks-3.3.0a4/src/pybricks/ev3dev/_speaker.py
+-rw-r--r--   0        0        0     6619 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/ev3devices.py
+-rw-r--r--   0        0        0     4739 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/hubs.py
+-rw-r--r--   0        0        0     8418 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/iodevices.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/media/__init__.py
+-rw-r--r--   0        0        0    20861 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/media/ev3dev.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/media/py.typed
+-rw-r--r--   0        0        0     6524 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/messaging.py
+-rw-r--r--   0        0        0     6671 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/nxtdevices.py
+-rw-r--r--   0        0        0    12332 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/parameters.py
+-rw-r--r--   0        0        0    11610 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/pupdevices.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/py.typed
+-rw-r--r--   0        0        0     7961 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/robotics.py
+-rw-r--r--   0        0        0     5611 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/pybricks/tools.py
+-rw-r--r--   0        0        0     1409 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/uerrno/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/uerrno/py.typed
+-rw-r--r--   0        0        0     2523 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/uio/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/uio/py.typed
+-rw-r--r--   0        0        0     2007 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/ujson/__init__.py
+-rw-r--r--   0        0        0     6378 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/umath/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/umath/py.typed
+-rw-r--r--   0        0        0     3153 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/urandom/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/urandom/py.typed
+-rw-r--r--   0        0        0     4952 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/uselect/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/uselect/py.typed
+-rw-r--r--   0        0        0     2280 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/ustruct/__init__.py
+-rw-r--r--   0        0        0     1402 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/usys/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:02:04.446687 pybricks-3.3.0a4/src/usys/py.typed
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 pybricks-3.3.0a4/PKG-INFO
```

### Comparing `pybricks-3.2.0rc2/LICENSE` & `pybricks-3.3.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/pyproject.toml` & `pybricks-3.3.0a4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybricks"
-version = "3.2.0c2"
+version = "3.3.0a4"
 description = "Documentation and user-API stubs for Pybricks MicroPython"
 authors = ["The Pybricks Authors <dev@pybricks.com>"]
 maintainers = ["Laurens Valk <laurens@pybricks.com>", "David Lechner <david@pybricks.com>" ]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://pybricks.com"
 repository = "https://github.com/pybricks/pybricks-api"
```

### Comparing `pybricks-3.2.0rc2/src/micropython/__init__.py` & `pybricks-3.3.0a4/src/micropython/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/pybricks/_common.py` & `pybricks-3.3.0a4/src/pybricks/_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 """Generic cross-platform module for typical devices like lights, displays,
 speakers, and batteries."""
 
 from __future__ import annotations
 
 from typing import Union, Iterable, overload, Optional, Tuple, Collection, TYPE_CHECKING
 
-from .geometry import Matrix, Axis
-from .parameters import Direction, Stop, Button, Port, Color, Side
+from .tools import Matrix
+from .parameters import Axis, Direction, Stop, Button, Port, Color, Side
 
 if TYPE_CHECKING:
     from .parameters import Number
 
 
 class System:
     """System control actions for a hub."""
@@ -215,41 +215,42 @@
 
     @overload
     def pid(
         self,
         kp: Optional[Number] = None,
         ki: Optional[Number] = None,
         kd: Optional[Number] = None,
-        reserved: Optional[Number] = None,
+        integral_deadzone: Optional[Number] = None,
         integral_rate: Optional[Number] = None,
     ) -> None:
         ...
 
     @overload
-    def pid(self) -> Tuple[int, int, int, None, int]:
+    def pid(self) -> Tuple[int, int, int, int, int]:
         ...
 
     def pid(self, *args):
-        """pid(kp, ki, kd, reserved, integral_rate)
-        pid() -> Tuple[int, int, int, None, int]
+        """pid(kp, ki, kd, integral_deadzone, integral_rate)
+        pid() -> Tuple[int, int, int, int, int]
 
         Gets or sets the PID values for position and speed control.
 
         If no arguments are given, this will return the current values.
 
         Arguments:
             kp (int): Proportional position control
                 constant. It is the feedback torque per degree of
                 error: µNm/deg.
             ki (int): Integral position control constant. It is the feedback
                 torque per accumulated degree of error: µNm/(deg s).
             kd (int): Derivative position (or proportional speed) control
                 constant. It is the feedback torque per
                 unit of speed: µNm/(deg/s).
-            reserved: This setting is not used.
+            integral_deadzone (Number, deg or Number, mm): Zone around the
+                target where the error integral does not accumulate errors.
             integral_rate (Number, deg/s or Number, mm/s): Maximum rate at
                 which the error integral is allowed to grow.
         """
 
     @overload
     def target_tolerances(
         self, speed: Optional[Number] = None, position: Optional[Number] = None
@@ -299,31 +300,81 @@
                 cannot reach this speed for some ``time`` even with maximum
                 actuation, it is stalled.
             time (Number, ms): How long the controller has to be below this
                 minimum ``speed`` before we say it is stalled.
         """
 
 
+class Model:
+    """Class to interact with motor state observer and settings."""
+
+    def state(self) -> Tuple[float, float, float, bool]:
+        """state() -> Tuple[float, float, float, bool]
+
+        Gets the estimated angle, speed, current, and stall state of the motor,
+        using a simulation model that mimics the real motor.
+        These estimates are updated faster than the real measurements,
+        which can be useful when building your own PID controllers.
+
+        For most applications it is better to used the *measured*
+        :meth:`angle <pybricks.pupdevices.Motor.angle>`,
+        :meth:`speed <pybricks.pupdevices.Motor.speed>`,
+        :meth:`load <pybricks.pupdevices.Motor.load>`, and
+        :meth:`stall <pybricks.pupdevices.Motor.stalled>` state instead.
+
+        Returns:
+            Tuple with the estimated angle (deg), speed (deg/s), current (mA),
+            and stall state (``True`` or ``False``).
+        """
+
+    @overload
+    def settings(self, values: tuple) -> None:
+        ...
+
+    @overload
+    def settings(self) -> tuple:
+        ...
+
+    def settings(self, speed, time):
+        """settings(values)
+        settings() -> Tuple
+
+        Gets or sets model settings as a tuple of integers. If no arguments are
+        given, this will return the current values. This method is mainly used
+        to debug the motor model class. Changing these settings should not be
+        needed in user programs.
+
+        .. _model settings: https://docs.pybricks.com/projects/pbio/en/latest/struct__pbio__observer__settings__t.html
+
+        Arguments:
+            values (Tuple): Tuple with `model settings`_.
+        """
+
+
 class Motor(DCMotor):
     """Generic class to control motors with built-in rotation sensors."""
 
     control = Control()
     """The motors use PID control to accurately track the speed and
     angle targets that you specify. You can change its behavior through the
     ``control`` attribute of the motor. See :ref:`control` for an overview
     of available methods."""
 
+    model = Model()
+    """Model representing the observer that estimates the motor state."""
+
     def __init__(
         self,
         port: Port,
         positive_direction: Direction = Direction.CLOCKWISE,
         gears: Optional[Union[Collection[int], Collection[Collection[int]]]] = None,
         reset_angle: bool = True,
+        profile: Number = None,
     ):
-        """__init__(port, positive_direction=Direction.CLOCKWISE, gears=None, reset_angle=True)
+        """__init__(port, positive_direction=Direction.CLOCKWISE, gears=None, reset_angle=True, profile=None)
 
         Arguments:
             port (Port): Port to which the motor is connected.
             positive_direction (Direction): Which direction the motor should
                 turn when you give a positive speed value or
                 angle.
             gears (list):
@@ -332,36 +383,48 @@
                 For example: ``[12, 36]`` represents a gear train with a
                 12-tooth and a 36-tooth gear. Use a list of lists for multiple
                 gear trains, such as ``[[12, 36], [20, 16, 40]]``.
 
                 When you specify a gear train, all motor commands and settings
                 are automatically adjusted to account for the resulting gear
                 ratio.  The motor direction remains unchanged by this.
-            reset_angle(bool):
+            reset_angle (bool):
                 Choose ``True`` to reset the rotation sensor value to the
                 absolute marker angle (between -180 and 179).
                 Choose ``False`` to keep the
                 current value, so your program knows where it left off last
                 time.
+            profile (Number, deg): Precision profile. A lower value
+                means more precise movement; a larger value means
+                smoother movement. If no value is given, a suitable profile for
+                this motor type will be selected automatically.
         """
 
     def angle(self) -> int:
         """angle() -> int: deg
 
         Gets the rotation angle of the motor.
 
         Returns:
             Motor angle.
         """
 
-    def speed(self) -> int:
-        """speed() -> int: deg/s
+    def speed(self, window: Number = 100) -> int:
+        """speed(window=100) -> int: deg/s
 
         Gets the speed of the motor.
 
+        The speed is measured as the change in the motor angle during the
+        given time window. A short window makes the speed value more
+        responsive to motor movement, but less steady. A long window makes the
+        speed value less responsive, but more steady.
+
+        Arguments:
+            window (Number, ms): The time window used to determine the speed.
+
         Returns:
             Motor speed.
 
         """
 
     def stalled(self) -> bool:
         """stalled() -> bool
@@ -727,15 +790,15 @@
 
         Each image has the same format as above. Each image is
         shown for the given interval. The animation repeats
         forever while the rest of your program keeps running.
 
         Arguments:
             matrices (iter): Sequence of
-                :class:`Matrix <pybricks.geometry.Matrix>` of intensities.
+                :class:`Matrix <pybricks.tools.Matrix>` of intensities.
             interval (Number, ms): Time to display each image in the list.
         """
 
     def pixel(self, row: Number, column: Number, brightness: Number = 100) -> None:
         """pixel(row, column, brightness=100)
 
         Turns on one pixel at the specified brightness.
@@ -924,43 +987,113 @@
         :ref:`user-specified neutral orientation <robotframe>`.
 
         The order of rotation is pitch-then-roll. This is equivalent to a
         positive rotation along the robot y-axis and then a positive rotation
         along the x-axis.
 
         Returns:
-            Tuple of pitch and roll angles.
+            Tuple of pitch and roll angles in degrees.
         """
 
 
 class IMU(Accelerometer):
+    def ready(self) -> bool:
+        """ready() -> bool
+
+        Checks if the device is calibrated and ready for use.
+
+        This becomes ``True`` when the robot has been sitting stationary for a
+        few seconds, which allows the device to re-calibrate. It is ``False``
+        if the hub has just been started, or if it hasn't had a chance to
+        calibrate for more than 10 minutes.
+
+        Returns:
+            ``True`` if it is ready for use, ``False`` if not.
+        """
+
+    def stationary(self) -> bool:
+        """stationary() -> bool
+
+        Checks if the device is currently stationary (not moving).
+
+        Returns:
+            ``True`` if stationary for at least a second, ``False`` if it is
+            moving.
+        """
+
+    @overload
+    def settings(
+        self,
+        angular_velocity_threshold: float = None,
+        acceleration_threshold: float = None,
+    ) -> None:
+        ...
+
+    @overload
+    def settings(self) -> Tuple[float, float]:
+        ...
+
+    def settings(self, *args):
+        """
+        settings(angular_velocity_threshold, acceleration_threshold)
+        settings() -> Tuple[float, float]
+
+        Configures the IMU settings. If no arguments are given,
+        this returns the current values.
+
+        The ``angular_velocity_threshold`` and ``acceleration_threshold``
+        define when the hub is considered stationary. If all
+        measurements stay below these thresholds for one second, the IMU
+        will recalibrate itself.
+
+        In a noisy room with high ambient vibrations (such as a
+        competition hall), it is recommended to increase the thresholds
+        slightly to give your robot the chance to calibrate.
+        To verify that your settings are working as expected, test that
+        the ``stationary()`` method gives ``False`` if your robot is moving,
+        and ``True`` if it is sitting still for at least a second.
+
+        Arguments:
+            angular_velocity_threshold (Number, deg/s): The threshold for
+                angular velocity. The default value is 1.5 deg/s.
+            acceleration_threshold (Number, mm/s²): The threshold for angular
+                velocity. The default value is 250 mm/s².
+        """
+
     def heading(self) -> float:
         """heading() -> float: deg
 
-        Gets the heading angle relative to the starting orientation. It is a
-        positive rotation around the :ref:`z-axis in the robot
-        frame <robotframe>`, prior to applying any tilt rotation.
+        Gets the heading angle of your robot. A positive value means a
+        clockwise turn.
 
-        For a vehicle viewed from the top, this means that
-        a positive heading value corresponds to a counterclockwise rotation.
-
-        .. note:: This method is not yet implemented.
+        The heading is 0 when your program starts. The value continues to grow
+        even as the robot turns more than 180 degrees. It does not wrap around
+        to -180 like it does in some apps.
+
+
+        .. note:: *For now, this method only keeps track of the heading while
+                  the robot is on a flat surface.*
+
+                  This means that the value is
+                  no longer correct if you lift it from the table. To solve
+                  this, you can call ``reset_heading`` to reset the heading to
+                  a known value *after* you put it back down. For example, you
+                  could align your robot with the side of the competition table
+                  and reset the heading 90 degrees as the new starting point.
 
         Returns:
             Heading angle relative to starting orientation.
 
         """
 
     def reset_heading(self, angle: Number) -> None:
         """reset_heading(angle)
 
         Resets the accumulated heading angle of the robot.
 
-        .. note:: This method is not yet implemented.
-
         Arguments:
             angle (Number, deg): Value to which the heading should be reset.
         """
 
     @overload
     def angular_velocity(self, axis: Axis) -> float:
         ...
@@ -981,14 +1114,49 @@
             axis (Axis): Axis along which the angular velocity should be
                          measured.
         Returns:
             Angular velocity along the specified axis. If you specify no axis,
             this returns a vector of accelerations along all axes.
         """
 
+    def rotation(self, axis: Axis) -> float:
+        """
+        rotation(axis) -> float: deg
+
+        Gets the rotation of the device along a given axis in
+        the :ref:`robot reference frame <robotframe>`.
+
+        This value is useful if your robot *only* rotates along the requested
+        axis. For general three-dimensional motion, use the
+        ``orientation()`` method instead.
+
+        The value starts counting from ``0`` when you initialize this class.
+
+        Arguments:
+            axis (Axis): Axis along which the rotation should be measured.
+        Returns:
+            The rotation angle.
+        """
+
+    def orientation(self) -> Matrix:
+        """
+        orientation() -> Matrix
+
+        Gets the three-dimensional orientation of the robot in
+        the :ref:`robot reference frame <robotframe>`.
+
+        It returns a rotation matrix whose columns represent the ``X``, ``Y``,
+        and ``Z`` axis of the robot.
+
+        .. note:: This method is not yet implemented.
+
+        Returns:
+            The rotation matrix.
+        """
+
 
 class CommonColorSensor:
     """Generic color sensor that supports Pybricks color calibration."""
 
     def __init__(self, port: Port):
         """__init__(port)
```

### Comparing `pybricks-3.2.0rc2/src/pybricks/ev3dev/_speaker.py` & `pybricks-3.3.0a4/src/pybricks/ev3dev/_speaker.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/pybricks/ev3devices.py` & `pybricks-3.3.0a4/src/pybricks/ev3devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,22 +164,20 @@
             List of pressed buttons.
         """
 
 
 class GyroSensor:
     """LEGO® MINDSTORMS® EV3 Gyro Sensor."""
 
-    def __init__(
-        self, port: _Port, positive_direction: _Direction = _Direction.CLOCKWISE
-    ):
+    def __init__(self, port: _Port, direction: _Direction = _Direction.CLOCKWISE):
         """GyroSensor(port)
 
         Arguments:
             port (Port): Port to which the sensor is connected.
-            positive_direction (Direction):
+            direction (Direction):
                 Positive rotation direction when looking at the red dot on top
                 of the sensor.
 
         """
 
     def speed(self) -> int:
         """speed() -> int: deg/s
```

### Comparing `pybricks-3.2.0rc2/src/pybricks/hubs.py` & `pybricks-3.3.0a4/src/pybricks/hubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2018-2022 The Pybricks Authors
 
 """LEGO® Programmable Hubs."""
 from . import _common
 from .ev3dev import _speaker
-from .geometry import Axis
 from .media.ev3dev import Image as _Image
-from .parameters import Button as _Button
+from .parameters import Button as _Button, Axis
 
 
 class EV3Brick:
     """LEGO® MINDSTORMS® EV3 Brick."""
 
     # These class attributes are here for auto-documentation only.
     # In reality, they are instance attributes created by __init__.
```

### Comparing `pybricks-3.2.0rc2/src/pybricks/iodevices.py` & `pybricks-3.3.0a4/src/pybricks/iodevices.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/pybricks/media/ev3dev.py` & `pybricks-3.3.0a4/src/pybricks/media/ev3dev.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/pybricks/messaging.py` & `pybricks-3.3.0a4/src/pybricks/messaging.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/pybricks/nxtdevices.py` & `pybricks-3.3.0a4/src/pybricks/nxtdevices.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/pybricks/parameters.py` & `pybricks-3.3.0a4/src/pybricks/parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Union, TYPE_CHECKING
 import os
 
-from .geometry import Matrix as _Matrix
+from .tools import Matrix as _Matrix, vector as _vector
 
 if TYPE_CHECKING or os.environ.get("SPHINX_BUILD") == "True":
     Number = Union[int, float]
     """
     Numbers can be represented as integers or floating point values:
 
         * Integers (:class:`int <ubuiltins.int>`) are whole numbers
@@ -53,14 +53,28 @@
     def __str__(self):
         return "{}.{}".format(type(self).__name__, self.name)
 
     def __repr__(self):
         return str(self)
 
 
+class Axis:
+    """Unit axes of a coordinate system.
+
+    .. data:: X = vector(1, 0, 0)
+    .. data:: Y = vector(0, 1, 0)
+    .. data:: Z = vector(0, 0, 1)
+
+    """
+
+    X: _Matrix = _vector(1, 0, 0)
+    Y: _Matrix = _vector(0, 1, 0)
+    Z: _Matrix = _vector(0, 0, 1)
+
+
 class Color:
     """Light or surface color."""
 
     NONE: Color = ...
     BLACK: Color = ...
     GRAY: Color = ...
     WHITE: Color = ...
```

### Comparing `pybricks-3.2.0rc2/src/pybricks/pupdevices.py` & `pybricks-3.3.0a4/src/pybricks/pupdevices.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,17 @@
     # HACK: jedi can't find inherited __init__ so we have to duplicate docs
     def __init__(
         self,
         port: Port,
         positive_direction: Direction = Direction.CLOCKWISE,
         gears: Optional[Union[Collection[int], Collection[Collection[int]]]] = None,
         reset_angle: bool = True,
+        profile: Number = None,
     ):
-        """__init__(port, positive_direction=Direction.CLOCKWISE, gears=None, reset_angle=True)
+        """__init__(port, positive_direction=Direction.CLOCKWISE, gears=None, reset_angle=True, profile=None)
 
         Arguments:
             port (Port): Port to which the motor is connected.
             positive_direction (Direction): Which direction the motor should
                 turn when you give a positive speed value or
                 angle.
             gears (list):
@@ -52,20 +53,24 @@
                 For example: ``[12, 36]`` represents a gear train with a
                 12-tooth and a 36-tooth gear. Use a list of lists for multiple
                 gear trains, such as ``[[12, 36], [20, 16, 40]]``.
 
                 When you specify a gear train, all motor commands and settings
                 are automatically adjusted to account for the resulting gear
                 ratio.  The motor direction remains unchanged by this.
-            reset_angle(bool):
+            reset_angle (bool):
                 Choose ``True`` to reset the rotation sensor value to the
                 absolute marker angle (between -180 and 179).
                 Choose ``False`` to keep the
                 current value, so your program knows where it left off last
                 time.
+            profile (Number, deg): Precision profile. A lower value
+                means more precise movement; a larger value means
+                smoother movement. If no value is given, a suitable profile for
+                this motor type will be selected automatically.
         """
 
     def reset_angle(self, angle: Optional[Number] = None) -> None:
         """reset_angle(angle=None)
 
         Sets the accumulated rotation angle of the motor to a desired value.
```

### Comparing `pybricks-3.2.0rc2/src/pybricks/robotics.py` & `pybricks-3.3.0a4/src/pybricks/robotics.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     number of degrees.
 
     **Positive** distances, radii, or drive speeds mean
     driving **forward**. **Negative** means **backward**.
 
     **Positive** angles and turn rates mean turning **right**.
     **Negative** means **left**. So when viewed from the top,
-    positive means clockwise and negative means counterclockwise. If desired,
-    you can flip this convention by reversing the ``left_motor`` and
-    ``right_motor`` when you initialize this class.
+    positive means clockwise and negative means counterclockwise.
 
     See the `measuring`_ section for tips to measure and adjust the diameter
     and axle track values.
     """
 
     distance_control = _common.Control()
     """The traveled distance and drive speed are controlled by a PID
@@ -131,33 +129,38 @@
         ...
 
     @overload
     def settings(self) -> Tuple[int, int, int, int]:
         ...
 
     def settings(self, *args):
-        """settings(straight_speed, straight_acceleration, turn_rate, turn_acceleration)
+        """
+        settings(straight_speed, straight_acceleration, turn_rate, turn_acceleration)
         settings() -> Tuple[int, int, int, int]
 
-        Configures the speed and acceleration used
-        by :meth:`.straight`, :meth:`.turn`, and  :meth:`.curve`.
+        Configures the drive base speed and acceleration.
 
         If you give no arguments, this returns the current values as a tuple.
 
-        The default values are automatically configured based on your wheel
+        The initial values are automatically configured based on your wheel
         diameter and axle track. They are selected such that your robot
         drives at about 40% of its maximum speed.
 
+        The speed values given here do not apply to the :meth:`.drive` method,
+        since you provide your own speed values as arguments in that method.
+
         Arguments:
             straight_speed (Number, mm/s): Straight-line speed of the robot.
             straight_acceleration (Number, mm/s²): Straight-line
-                acceleration and deceleration of the robot.
+                acceleration and deceleration of the robot. Provide a tuple with
+                two values to set acceleration and deceleration separately.
             turn_rate (Number, deg/s): Turn rate of the robot.
             turn_acceleration (Number, deg/s²): Angular acceleration and
-                deceleration of the robot.
+                deceleration of the robot. Provide a tuple with
+                two values to set acceleration and deceleration separately.
         """
 
     def straight(
         self, distance: Number, then: Stop = Stop.HOLD, wait: bool = True
     ) -> None:
         """straight(distance, then=Stop.HOLD, wait=True)
 
@@ -215,12 +218,18 @@
         with the maximum actuation signal.
 
         Returns:
             ``True`` if the drivebase is stalled, ``False`` if not.
         """
 
 
+class GyroDriveBase(DriveBase):
+    """A robotic vehicle with two powered wheels and an optional support
+    wheel or caster. It measures the heading using the hub's built-in gyroscope,
+    which can make turning and driving straight more accurate."""
+
+
 # HACK: hide from jedi
 if TYPE_CHECKING:
     del Motor
     del Number
     del Stop
```

### Comparing `pybricks-3.2.0rc2/src/uerrno/__init__.py` & `pybricks-3.3.0a4/src/uerrno/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/uio/__init__.py` & `pybricks-3.3.0a4/src/uio/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/ujson/__init__.py` & `pybricks-3.3.0a4/src/ujson/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/umath/__init__.py` & `pybricks-3.3.0a4/src/umath/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/urandom/__init__.py` & `pybricks-3.3.0a4/src/urandom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     """
 
 
 def getrandbits(k: int) -> int:
     """
     getrandbits(k) -> int
 
-    Gets a random integer :math:`N` satisfying :math:`0 \\leq N < 2^{\\text{bits}}`.
+    Gets a random integer :math:`N` satisfying :math:`0 \\leq N < 2^{\\text{k}}`.
 
     Arguments:
         k (int): How many bits to use for the result.
     """
 
 
 def choice(seq: Sequence[Any]) -> Any:
```

### Comparing `pybricks-3.2.0rc2/src/uselect/__init__.py` & `pybricks-3.3.0a4/src/uselect/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/ustruct/__init__.py` & `pybricks-3.3.0a4/src/ustruct/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.2.0rc2/src/usys/__init__.py` & `pybricks-3.3.0a4/src/usys/__init__.py`

 * *Files identical despite different names*

