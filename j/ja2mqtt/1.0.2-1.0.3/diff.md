# Comparing `tmp/ja2mqtt-1.0.2.tar.gz` & `tmp/ja2mqtt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ja2mqtt-1.0.2.tar", last modified: Thu Apr 20 20:58:26 2023, max compression
+gzip compressed data, was "ja2mqtt-1.0.3.tar", last modified: Sat Apr 22 00:02:10 2023, max compression
```

## Comparing `ja2mqtt-1.0.2.tar` & `ja2mqtt-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.125399 ja2mqtt-1.0.2/
--rw-r--r--   0 tomas      (501) staff       (20)      108 2023-04-18 13:03:48.000000 ja2mqtt-1.0.2/MANIFEST.in
--rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-20 20:58:26.125239 ja2mqtt-1.0.2/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)     1650 2023-04-18 13:03:48.000000 ja2mqtt-1.0.2/README-pypi.text
--rw-r--r--   0 tomas      (501) staff       (20)     5471 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/README.md
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.119941 ja2mqtt-1.0.2/bin/
--rwxr-xr-x   0 tomas      (501) staff       (20)      345 2023-04-17 22:42:29.000000 ja2mqtt-1.0.2/bin/env.sh
--rwxr-xr-x   0 tomas      (501) staff       (20)       31 2023-04-17 22:42:29.000000 ja2mqtt-1.0.2/bin/ja2mqtt
--rw-r--r--   0 tomas      (501) staff       (20)      107 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/bin/requirements-dev.txt
--rwxr-xr-x   0 tomas      (501) staff       (20)      700 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/bin/requirements-setup-py.sh
--rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/bin/requirements.txt
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.120272 ja2mqtt-1.0.2/config/
--rw-r--r--   0 tomas      (501) staff       (20)     3676 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/config/ja2mqtt.yaml
--rw-r--r--   0 tomas      (501) staff       (20)     1852 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/config/sample-config.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.120694 ja2mqtt-1.0.2/docker/
--rw-r--r--   0 tomas      (501) staff       (20)      975 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/docker/Dockerfile
--rw-r--r--   0 tomas      (501) staff       (20)      299 2023-04-18 22:48:03.000000 ja2mqtt-1.0.2/docker/docker-compose.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.121148 ja2mqtt-1.0.2/docker/mqtt-config/
--rw-r--r--   0 tomas      (501) staff       (20)    40475 2023-04-17 22:42:29.000000 ja2mqtt-1.0.2/docker/mqtt-config/mosquitto.conf
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.122295 ja2mqtt-1.0.2/ja2mqtt/
--rwxr-xr-x   0 tomas      (501) staff       (20)      218 2023-04-20 20:26:08.000000 ja2mqtt-1.0.2/ja2mqtt/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)      831 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/__main__.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.123896 ja2mqtt-1.0.2/ja2mqtt/commands/
--rw-r--r--   0 tomas      (501) staff       (20)     2642 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/commands/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)     1308 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/commands/config.py
--rw-r--r--   0 tomas      (501) staff       (20)      883 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/commands/run.py
--rw-r--r--   0 tomas      (501) staff       (20)     2528 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/commands/test.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.124958 ja2mqtt-1.0.2/ja2mqtt/components/
--rw-r--r--   0 tomas      (501) staff       (20)      786 2023-04-17 22:42:29.000000 ja2mqtt-1.0.2/ja2mqtt/components/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)    10530 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/components/bridge.py
--rw-r--r--   0 tomas      (501) staff       (20)     5626 2023-04-20 20:26:08.000000 ja2mqtt-1.0.2/ja2mqtt/components/mqtt.py
--rw-r--r--   0 tomas      (501) staff       (20)     7962 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/components/serial.py
--rw-r--r--   0 tomas      (501) staff       (20)     6022 2023-04-20 20:26:08.000000 ja2mqtt-1.0.2/ja2mqtt/components/simulator.py
--rw-r--r--   0 tomas      (501) staff       (20)    13192 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/config.py
--rw-r--r--   0 tomas      (501) staff       (20)     8079 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/utils.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.122990 ja2mqtt-1.0.2/ja2mqtt.egg-info/
--rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)      752 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 tomas      (501) staff       (20)        1 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/requires.txt
--rw-r--r--   0 tomas      (501) staff       (20)        8 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/top_level.txt
--rw-r--r--   0 tomas      (501) staff       (20)       38 2023-04-20 20:58:26.125443 ja2mqtt-1.0.2/setup.cfg
--rw-r--r--   0 tomas      (501) staff       (20)     1454 2023-04-18 13:03:48.000000 ja2mqtt-1.0.2/setup.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.907639 ja2mqtt-1.0.3/
+-rw-r--r--   0 tomas      (501) staff       (20)      108 2023-04-18 13:03:48.000000 ja2mqtt-1.0.3/MANIFEST.in
+-rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-22 00:02:10.907469 ja2mqtt-1.0.3/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)     1650 2023-04-18 13:03:48.000000 ja2mqtt-1.0.3/README-pypi.text
+-rw-r--r--   0 tomas      (501) staff       (20)     5128 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/README.md
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.903641 ja2mqtt-1.0.3/bin/
+-rwxr-xr-x   0 tomas      (501) staff       (20)      345 2023-04-17 22:42:29.000000 ja2mqtt-1.0.3/bin/env.sh
+-rwxr-xr-x   0 tomas      (501) staff       (20)       31 2023-04-17 22:42:29.000000 ja2mqtt-1.0.3/bin/ja2mqtt
+-rw-r--r--   0 tomas      (501) staff       (20)      107 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/bin/requirements-dev.txt
+-rwxr-xr-x   0 tomas      (501) staff       (20)      700 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/bin/requirements-setup-py.sh
+-rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/bin/requirements.txt
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.904060 ja2mqtt-1.0.3/config/
+-rw-r--r--   0 tomas      (501) staff       (20)     3916 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/config/ja2mqtt.yaml
+-rw-r--r--   0 tomas      (501) staff       (20)     2024 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/config/sample-config.yaml
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.904456 ja2mqtt-1.0.3/docker/
+-rw-r--r--   0 tomas      (501) staff       (20)      975 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/docker/Dockerfile
+-rw-r--r--   0 tomas      (501) staff       (20)      299 2023-04-18 22:48:03.000000 ja2mqtt-1.0.3/docker/docker-compose.yaml
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.904785 ja2mqtt-1.0.3/docker/mqtt-config/
+-rw-r--r--   0 tomas      (501) staff       (20)    40475 2023-04-17 22:42:29.000000 ja2mqtt-1.0.3/docker/mqtt-config/mosquitto.conf
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.905394 ja2mqtt-1.0.3/ja2mqtt/
+-rwxr-xr-x   0 tomas      (501) staff       (20)      167 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)      251 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/__main__.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.906699 ja2mqtt-1.0.3/ja2mqtt/commands/
+-rw-r--r--   0 tomas      (501) staff       (20)     1951 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)     1828 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/config.py
+-rw-r--r--   0 tomas      (501) staff       (20)     1859 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/ja2mqtt.py
+-rw-r--r--   0 tomas      (501) staff       (20)      987 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/run.py
+-rw-r--r--   0 tomas      (501) staff       (20)     2552 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/test.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.907257 ja2mqtt-1.0.3/ja2mqtt/components/
+-rw-r--r--   0 tomas      (501) staff       (20)      819 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)    11210 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/bridge.py
+-rw-r--r--   0 tomas      (501) staff       (20)     5572 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/mqtt.py
+-rw-r--r--   0 tomas      (501) staff       (20)     7857 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/serial.py
+-rw-r--r--   0 tomas      (501) staff       (20)     6477 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/simulator.py
+-rw-r--r--   0 tomas      (501) staff       (20)    13243 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/config.py
+-rw-r--r--   0 tomas      (501) staff       (20)     8079 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/ja2mqtt/utils.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.906147 ja2mqtt-1.0.3/ja2mqtt.egg-info/
+-rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)      814 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 tomas      (501) staff       (20)        1 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       61 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/requires.txt
+-rw-r--r--   0 tomas      (501) staff       (20)        8 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       38 2023-04-22 00:02:10.907680 ja2mqtt-1.0.3/setup.cfg
+-rw-r--r--   0 tomas      (501) staff       (20)     1589 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/setup.py
```

### Comparing `ja2mqtt-1.0.2/PKG-INFO` & `ja2mqtt-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ja2mqtt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Jablotron MQTT bridge
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ja2mqtt-1.0.2/README-pypi.text` & `ja2mqtt-1.0.3/README-pypi.text`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.2/README.md` & `ja2mqtt-1.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # $ ja2mqtt
 
 ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
 
-ja2mqtt enables the use of MQTT events to control Jablotron events, allowing for seamless integration with MQTT-based IoT systems and platforms. With this bridge, Jablotron alarms can be integrated into a larger IoT ecosystem, alongside other devices that use industry-standard protocols like ZigBee or MQTT. For example, by using ja2mqtt in conjunction with ZigBee2MQTT, Jablotron alarms and ZigBee devices can be connected in a single network and integrated with other systems such as Alexa, Tahoma, or Google Assistant, providing a unified and interoperable smart home or industrial automation solution.
-
 ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
 
 If you do not have access to a JA-121T interface for testing, ja2mqtt offers a simulator that can simulate the interaction with the JA-121T interface. This allows you to test and verify the functionality of ja2mqtt even without the physical JA-121T interface available.
 
 ## Features
 
 * Define Jablotron topology in the YAML configuration file, including sections with their codes, names, and peripherals' positions and names.
 * Implement declarative rules in the ja2mqtt.yaml configuration file to support the serial JA-121T protocol.
 * Read events from Jablotron, such as section arming and disarming, peripheral state changes, and convert them to MQTT events.
-* Use MQTT events to query section states and correlate request and response MQTT events.
-* Implement automated recovery from serial interface failures or MQTT broker connection failures.
-* JA-121T simulator that simulates section state changes, peripheral state changes and heartbeat messages. 
+* Use MQTT events to query section and peripheral states and correlate request and response MQTT events.
+* Implement automated recovery from serial interface connection failures or MQTT broker connection failures.
+* JA-121T simulator that simulates section state changes, peripheral state changes and heartbeat messages.
 
 ## Testing using Docker
 
 To test ja2mqtt with the JA-121T simulator, you can utilize the ja2mqtt Docker image that comes with pre-configured settings. The simulator provides a straightforward Jablotron topology with two sections: "House" with code "1" and an initial state of "ARMED", and "Garage" with code "2" and an initial state of "READY". This topology can be used to simulate changing the state or retrieving the status of the sections. The simulator also mimics Jablotron heartbeat messages by generating "OK" messages every 10 seconds.
 
 To test ja2mqtt with the simulator, follow the steps below.
 
@@ -42,32 +40,14 @@
    <-- send: ja2mqtt/section/get: {"pin": "1234", "corrid": "ca8438b82f16"}
    --> recv: ja2mqtt/section/house: {"corrid": "ca8438b82f16", "section_code": 1, "section_name": "house", "state": "ARMED"}
    --> recv: ja2mqtt/section/garage: {"corrid": "ca8438b82f16", "section_code": 2, "section_name": "garage", "state": "READY"}   
    ```
 
 4. Check the log entries in the ja2mqtt log again to see if the events were generated.
 
-2. Inspect logs of ja2mqtt by running the following command:
-
-   ```
-   $ docker logs ja2mqtt -f
-   ```
-
-3. Publish the mqtt event to retrieve a state of sections as follows:
-
-   ```
-   $ docker exec -it ja2mqtt pub -t ja2mqtt/section/get -d pin=1234
-   ```
-
-4. Check log entries in the ja2mqtt log to see that the following entries are present:
-
-   ```
-   2023-04-17 21:59:46,203 [mqtt    ] [I] <-- send: ja2mqtt/section/house, data={"section_code": 1, "section_name": "house", "state": "ARMED"}
-   2023-04-17 21:59:46,408 [mqtt    ] [I] <-- send: ja2mqtt/section/garage, data={"section_code": 2, "section_name": "garage", "state": "READY"}
-   ```
 ## Getting Started
 
 To use ja2mqtt, you will need:
 
 * Jablotron alarms with the control unit and the JA-121T serial interface connected to a serial port on your computer. The device uses RS485 interface, which can be connected to your computer using a [USB to RS485 adapter](https://www.aliexpress.com/w/wholesale-ch340-usb-rs485.html).
 
 * A running instance of an MQTT broker. [Mosquitto](https://mosquitto.org/) is the recommended MQTT broker, but others should also work without issues. You can run the MQTT broker on the same machine as ja2mqtt, on a separate machine, or use an existing instance of MQTT broker if you have one.
@@ -75,7 +55,18 @@
 * Install ja2mqtt on a computer with access to the serial port where JA-121T is connected.
 
    ```
    $ pip install ja2mqtt
    ```
 
 * Download the sample configuration file and ja2mqtt definition file from the [config directory](https://github.com/tomvit/ja2mqtt/tree/master/config) of the ja2mqtt GitHub repository. In the sample configuration file, you only need to define your Jablotron topology, such as section names and their numbers.
+
+## Usage
+
+ja2mqtt is a CLI that provides the following commands. You can use the `--help` option to get more information on command usage.
+
+* `run` - the main command that reads/writes data from/to the serial interface and sends/receives MQTT events.
+* `pub` - publishes MQTT events and waits for the response. It uses the correlation ID to relate the event request with the event response.
+* `config main` - shows the main configuration in JSON.
+* `config ja2mqtt` - shows the ja2mqtt definition file after Jinja2 templating is processed.
+* `config env` - shows the environment variables used by ja2mqtt. You can define the variables in your system to set defaults for ja2mqtt options.
+* `config topics` - shows publishing and subscribing topics. You can subscribe to publishing topics from your client or send subscribing topics to control the operation of your Jablotron control unit.
```

### Comparing `ja2mqtt-1.0.2/bin/requirements-setup-py.sh` & `ja2mqtt-1.0.3/bin/requirements-setup-py.sh`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.2/config/ja2mqtt.yaml` & `ja2mqtt-1.0.3/config/ja2mqtt.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,25 @@
   correlation_id: 'corrid'
 
   # correlation timeout in seconds
   # when a mqtt request is received, then within this timeout the response must be collected
   # the request-response will then share the same correlation id
   correlation_timeout: 1.5
 
+  # number of bits in prfstate (default: 128)
+  prfstate_bits: 24
+
 # Definition of MQTT topics for serial output.
 # The topics defined in `serial2mqtt` will be created in MQTT broker according to events that occur in the serial output
 serial2mqtt:
 
 # MQTT heartbeat topic; Jablotron writes hearbeat 'OK' messages to serial output
 # that are converted to MQTT heartbeat events
 - name: ja2mqtt/heartbeat
-  disabled: False
+  disabled: True
   rules:
   - read: OK
     write:
       heartbeat: !py data
 
     # disable correlation for this rule
     no_correlation: True
@@ -38,22 +41,23 @@
   - read: !py pattern('STATE {{ v }} (READY|ARMED_PART|ARMED|SERVICE|BLOCKED|OFF)')
     write:
       section_code: {{ v }}
       section_name: {{ k }}
       state: !py data.match.group(1)
 {% endfor %}
 
-{% for v in topology.peripheral if v.type == 'motion-sensor' %}
-- name: ja2mqtt/motion/{{ v.name }}
+{% for v in topology.peripheral if v.type in ['motion','siren','magnet','smoke'] %}
+- name: ja2mqtt/{{ v.type }}/{{ v.name }}
   rules:
-  - read: !py prf_state({'{{ v['pos'] }}':'ON'})
+  - read: !py prf_state_change({{ v['pos'] }})
     write:
       name: {{ v.name }}
       type: {{ v.type }}
       pos: {{ v.pos }}
+      state: !py data.state
 
     # allow to process next rule when this rule matches
     process_next_rule: True
 {% endfor %}
 
 # generic error
 - name: ja2mqtt/error
@@ -82,14 +86,20 @@
 - name: ja2mqtt/section/get
   rules:
     - read:
         pin: !py pattern("^[0-9]{4}$")
       write: !py format("{pin} STATE",pin=data.pin)
       request_ttl: 99
 
+# get prfstate
+- name: ja2mqtt/prfstate/get
+  rules:
+    - write: !py write_prf_state(reset=True)
+      request_ttl: 128
+
 {% for k,v in topology.section.items() %}
 # set state to ARMED for a single section
 - name: ja2mqtt/section/{{ k }}/set
   rules:
     - read:
         pin: !py pattern("^[0-9]{4}$")
       write: !py format("{pin} SET {{ v }}",pin=data.pin)
```

### Comparing `ja2mqtt-1.0.2/config/sample-config.yaml` & `ja2mqtt-1.0.3/config/sample-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -32,46 +32,55 @@
     house: 1
     garage: 2
   peripheral:
     - name: house/central-unit
       type: central-unit
       pos: 0
     - name: house/entrance
-      type: motion-sensor
+      type: motion
       pos: 1
     - name: house/upperfloor/hall
-      type: motion-sensor
+      type: motion
       pos: 2
     - name: house/upperfloor/livingroom
-      type: motion-sensor
+      type: motion
       pos: 3
+    - name: house/upperfloor/smoke
+      type: smoke
+      pos: 4
+    - name: house/siren
+      type: siren
+      pos: 5
+    - name: garage/gate
+      type: magnet
+      pos: 6
 
 # When serial.use_simulator is True, the below configuration defines how events will be generated for ja2mqtt
 simulator:
   pin: 1234
   sections:
     - code: 1
       state: ARMED
     - code: 2
       state: READY
     - code: 3
       state: OFF
     - code: 4
       state: OFF
 
+  # positions of peripherals to be simulated
+  peripherals: 1,2,3,4,5,6
+
   # delay in seconds when responding to a command
   response_delay: 0.5
 
-  # number of bits in prfstate event
-  prf_state_bits: 24
-
   # list of rules that will generate sinulated events
   rules:
   # heartbeat every 10s
   - time_next: 10
     write: OK
 
   # prf state will occur once every 10-20 seconds
   - time_next: !py random(10,20)
-    # this will write prfstate event for peripherials on positions 1, 2, 3
+    # this will write prfstate event for peripherials on positions 1, 2, 3, 4, 5, 6
     # on_prob is a probability of the ON state, (1-on_prob) is then the probability of the OFF state
-    write: !py prf_randon_states(1,2,3, on_prob=0.8)
+    write: !py prf_random_states(on_prob=0.8)
```

### Comparing `ja2mqtt-1.0.2/docker/Dockerfile` & `ja2mqtt-1.0.3/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.2/docker/mqtt-config/mosquitto.conf` & `ja2mqtt-1.0.3/docker/mqtt-config/mosquitto.conf`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.2/ja2mqtt/commands/__init__.py` & `ja2mqtt-1.0.3/ja2mqtt/commands/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import logging
 
 import click
 from click import Option
 
 import ja2mqtt.config as ja2mqtt_config
-from ja2mqtt import get_version_string
+from ja2mqtt import __version__
 from ja2mqtt.config import Config, init_logging
 
 
 class BaseCommand(click.core.Command):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.params.insert(
@@ -47,56 +47,22 @@
     def invoke(self, ctx):
         config_file = ctx.params.pop("config")
         env_file = ctx.params.pop("env")
         config = Config(config_file, env_file)
 
         self.init_logging(config)
         log = logging.getLogger(ctx.command.name + "-loop")
-        log.info(
-            f"ja2mqtt, Jablotron JA-121 Serial MQTT bridge, version {get_version_string()}"
-        )
+        log.info(f"ja2mqtt, Jablotron JA-121 Serial MQTT bridge, version {__version__}")
 
         ctx.params["config"] = config
         ctx.params["log"] = log
         super().invoke(ctx)
 
 
 class BaseCommandLogOnly(BaseCommand):
     def init_logging(self, config):
         init_logging(
             config.get_dir_path(config.root("logs")),
             "run",
             log_level="DEBUG" if ja2mqtt_config.DEBUG else "INFO",
             handlers=["file"],
         )
-
-
-@click.group()
-@click.option(
-    "--no-ansi",
-    "no_ansi",
-    is_flag=True,
-    default=False,
-    help="Do not use ANSI colors",
-)
-@click.option(
-    "--debug",
-    "debug",
-    is_flag=True,
-    default=False,
-    help="Print debug information",
-)
-@click.version_option(version=get_version_string())
-def ja2mqtt(no_ansi, debug):
-    if no_ansi:
-        ja2mqtt_config.ANSI_COLORS = False
-    if debug:
-        ja2mqtt_config.DEBUG = True
-
-
-from .config import command_config
-from .run import command_run
-from .test import command_publish
-
-ja2mqtt.add_command(command_run)
-ja2mqtt.add_command(command_config)
-ja2mqtt.add_command(command_publish)
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/commands/config.py` & `ja2mqtt-1.0.3/ja2mqtt/commands/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 # @author: Tomas Vitvar, https://vitvar.com, tomas@vitvar.com
 
 from __future__ import absolute_import, unicode_literals
 
 import json
+import os
 
 import click
-import os
 
 from ja2mqtt.config import Config, env_variables
 from ja2mqtt.utils import Map
 
 from . import BaseCommandLogOnly
 
 
@@ -38,11 +38,25 @@
 def config_env():
     print("List of environment variables used by ja2mqtt:")
     print("")
     for e in env_variables:
         print(f"{e}={os.getenv(e)}")
     print("")
 
+@click.command("topics", help="Show MQTT topics.", cls=BaseCommandLogOnly)
+def config_topics(config, log):
+    ja2mqtt_file = config.get_dir_path(config.root("ja2mqtt"))
+    scope = Map(topology=config.root("topology"))
+    ja2mqtt = Config(ja2mqtt_file, scope=scope, use_template=True)
+
+    print("Publishing:")
+    for t in ja2mqtt("serial2mqtt"):
+        print(f"- {t['name']}")
+    print("Subscribing:")
+    for t in ja2mqtt("mqtt2serial"):
+        print(f"- {t['name']}")
+
 
 command_config.add_command(config_main)
 command_config.add_command(config_ja2mqtt)
 command_config.add_command(config_env)
+command_config.add_command(config_topics)
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/commands/run.py` & `ja2mqtt-1.0.3/ja2mqtt/commands/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 import logging
 import time
 
 import click
 
 import ja2mqtt.config as ja2mqtt_config
-from ja2mqtt import get_version_string
-from ja2mqtt.components import MQTT, Serial, SerialMQTTBridge
+from ja2mqtt.components import MQTT, Serial, SerialMQTTBridge, Simulator
 from ja2mqtt.config import Config, init_logging
 from ja2mqtt.utils import Map, randomString
 
 from . import BaseCommand
 
 
 @click.command("run", help="Run command.", cls=BaseCommand)
 def command_run(config, log):
-    serial = Serial(config)
-    mqtt = MQTT(f"ja2mqtt-client+{randomString(10)}", config)
     bridge = SerialMQTTBridge(config)
+    simulator = Simulator(config.get_part("simulator"), bridge.prfstate_bits)
+    serial = Serial(config.get_part("serial"), simulator)
+    mqtt = MQTT(f"ja2mqtt-client+{randomString(10)}", config.get_part("mqtt-broker"))
 
     bridge.set_mqtt(mqtt)
     bridge.set_serial(serial)
 
     for x in (mqtt, serial, bridge):
         x.start(ja2mqtt_config.exit_event)
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/commands/test.py` & `ja2mqtt-1.0.3/ja2mqtt/commands/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # @author: Tomas Vitvar, https://vitvar.com, tomas@vitvar.com
 
 from __future__ import absolute_import, unicode_literals
 
 import json
 import logging
-import time
 import sys
+import time
 
 import click
 
 import ja2mqtt.config as ja2mqtt_config
 from ja2mqtt import __version__ as version
 from ja2mqtt.components import MQTT
-from ja2mqtt.config import Config, init_logging, ja2mqtt_def, correlation_id
+from ja2mqtt.config import Config, correlation_id, init_logging, ja2mqtt_def
 from ja2mqtt.utils import Map, dict_from_string, randomString
 
 from . import BaseCommandLogOnly
 
 
 @click.command("pub", help="Publish a ja2mqtt topic in MQTT.", cls=BaseCommandLogOnly)
 @click.option(
@@ -67,15 +67,15 @@
         if field is None or data.get(field) == id:
             print(f"--> recv: {topic}: {payload}")
 
     def _on_connect(client, userdata, flags, rc):
         for topic in ja2mqtt.root("serial2mqtt"):
             client.subscribe(topic["name"])
 
-    mqtt = MQTT(f"ja2mqtt-test-{randomString(5)}", config)
+    mqtt = MQTT(f"ja2mqtt-test-{randomString(5)}", config.get_part("mqtt-broker"))
     mqtt.on_message_ext = _wait_for_response
     mqtt.on_connect_ext = _on_connect
     mqtt.start(ja2mqtt_config.exit_event)
     try:
         mqtt.wait_is_connected(ja2mqtt_config.exit_event)
         print(f"<-- send: {_topic['name']}: {json.dumps(_data)}")
         mqtt.publish(_topic["name"], json.dumps(_data))
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/components/__init__.py` & `ja2mqtt-1.0.3/ja2mqtt/components/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,7 +27,8 @@
         )
         self.thread.start()
 
 
 from .bridge import SerialMQTTBridge
 from .mqtt import MQTT
 from .serial import Serial
+from .simulator import Simulator
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/components/bridge.py` & `ja2mqtt-1.0.3/ja2mqtt/components/bridge.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,60 +4,65 @@
 from __future__ import absolute_import, unicode_literals
 
 import json
 import logging
 import re
 import threading
 import time
-from queue import Queue, Empty
+from queue import Empty, Queue
 
 import paho.mqtt.client as mqtt
 
 from ja2mqtt.config import Config
 from ja2mqtt.utils import Map, PythonExpression, deep_eval, deep_merge, merge_dicts
 
 from . import Component
-from .simulator import Simulator
+from .serial import SerialJA121TException, decode_prfstate
 
-from .serial import decode_prfstate, SerialJA121TException
 
 class Pattern:
+    """
+    Pattern class is used in the scope to evaluate that a data string matches the pattern
+    defined in the ja2mqtt rule. It is possible to use the equal operator to compare the data string
+    with the pattern object and then use the matcher to retrieve captured groups
+    for the `wrtie` condition of the rule.
+    """
+
     def __init__(self, pattern):
         self.match = None
         self.pattern = pattern
         self.re = re.compile(self.pattern)
 
     def __str__(self):
         return f"r'{self.pattern}'" if self.match is None else self.match.group(0)
 
     def __eq__(self, other):
         self.match = self.re.match(other)
         return self.match is not None
 
 
-class PrfState:
-    def __init__(self, prf):
-        if not isinstance(prf, dict) or len([k for k in prf.keys() if re.match('[0-9]+', k)])==0:
-            raise Exception(f"Invalid prf object format: {prf}")
-        self.prf = prf
-        self.prf_decoded = None
-        self.prf_str = None
+class PrfStateChange:
+    def __init__(self, pos, current_prfstate):
+        self.pos = pos
+        self.current_prfstate = current_prfstate
+        self.state = None
 
     def __str__(self):
-        return f"{self.prf_decoded}" if self.prf_decoded is not None else self.prf
+        return f"position={self.pos}, state={self.state}"
 
     def __eq__(self, other):
         if other.startswith("PRFSTATE"):
             d = decode_prfstate(other.split(" ")[1])
-            d_filtered = {
-                k: v for k, v in d.items() if k in self.prf.keys() and re.match(self.prf[k],v)
-            }
-            if len(d_filtered.keys()) > 0:
-                self.prf_decoded = d_filtered
-        return self.prf_decoded is not None
+            self.state = d[self.pos]
+            return (
+                self.current_prfstate is None
+                or d[self.pos] != self.current_prfstate[self.pos]
+            )
+        else:
+            return False
 
 
 class Topic:
     def __init__(self, topic):
         self.name = topic["name"]
         self.disabled = topic.get("disabled", False)
         self.rules = []
@@ -71,31 +76,38 @@
             for k, v in read.items():
                 path += [k]
                 if k not in data.keys():
                     raise Exception(f"Missing property {k}.")
                 else:
                     if not isinstance(v, PythonExpression) and type(v) != type(data[k]):
                         raise Exception(
-                            f"Invalid type of property {'.'.join(path)}, found: {type(data[k]).__name__}, expected: {type(v).__name__}"
+                            f"Invalid type of property {'.'.join(path)}, "
+                            + f"found: {type(data[k]).__name__}, expected: {type(v).__name__}"
                         )
                     if type(v) == dict:
                         self.check_rule_data(v, data[k], scope, path)
                     else:
                         if isinstance(v, PythonExpression):
                             v = v.eval(scope)
                         if v != data[k]:
                             raise Exception(
-                                f"Invalid value of property {'.'.join(path)}, found: {data[k]}, exepcted: {v}"
+                                f"Invalid value of property {'.'.join(path)}, "
+                                + f"found: {data[k]}, exepcted: {v}"
                             )
         except Exception as e:
             raise Exception(f"Topic data validation failed. {str(e)}")
 
 
 class SerialMQTTBridge(Component):
     def __init__(self, config):
+        def _list(topics):
+            return ", ".join(
+                [x.name + ("" if not x.disabled else " (disabled)") for x in topics]
+            )
+
         super().__init__(config, "bridge")
         self.mqtt = None
         self.serial = None
         self.topics_serial2mqtt = []
         self.topics_mqtt2serial = []
         self._scope = None
         self.request_queue = Queue()
@@ -105,73 +117,80 @@
         for topic_def in ja2mqtt("serial2mqtt"):
             self.topics_serial2mqtt.append(Topic(topic_def))
         for topic_def in ja2mqtt("mqtt2serial"):
             self.topics_mqtt2serial.append(Topic(topic_def))
         self.correlation_id = ja2mqtt("system.correlation_id", None)
         self.correlation_timeout = ja2mqtt("system.correlation_timeout", 0)
         self.topic_sys_error = ja2mqtt("system.topic_sys_error", None)
+        self.prfstate_bits = ja2mqtt("system.prfstate_bits", 128)
         self.request = None
+        self.prfstate = [decode_prfstate("".zfill(self.prfstate_bits))]
 
         self.log.info(f"The ja2mqtt definition file is {ja2mqtt_file}")
         self.log.info(
-            f"There are {len(self.topics_serial2mqtt)} serial2mqtt and {len(self.topics_mqtt2serial)} mqtt2serial topics."
-        )
-        self.log.debug(
-            f"The serial2mqtt topics are: {', '.join([x.name + ('' if not x.disabled else ' (disabled)') for x in self.topics_serial2mqtt])}"
-        )
-        self.log.debug(
-            f"The mqtt2serial topics are: {', '.join([x.name + ('' if not x.disabled else ' (disabled)') for x in self.topics_mqtt2serial])}"
+            f"There are {len(self.topics_serial2mqtt)} serial2mqtt and "
+            + f"{len(self.topics_mqtt2serial)} mqtt2serial topics."
         )
+        self.log.debug(f"The serial2mqtt topics are: {_list(self.topics_serial2mqtt)}")
+        self.log.debug(f"The mqtt2serial topics are: {_list(self.topics_mqtt2serial)}")
 
     def update_correlation(self, data):
         if self.request_queue.qsize() > 0:
             self.request = self.request_queue.get()
         if self.request is not None:
             if (
                 time.time() - self.request.created_time < self.correlation_timeout
                 and self.request.ttl > 0
             ):
                 if self.request.cor_id is not None:
                     data[self.correlation_id] = self.request.cor_id
                 self.request.ttl -= 1
             else:
                 self.log.debug(
-                    "Discarding the request for correlation. The correlation timeout or TTL expired."
+                    "Discarding the request for correlation. The correlation timeout "
+                    + "or TTL expired."
                 )
                 self.request = None
         return data
 
     def scope(self):
+        def _write_prf_state(reset=False):
+            if reset:
+                self.log.debug("Reseting prfstate object to None.")
+                self.prfstate = []
+            return "PRFSTATE"
+
         if self._scope is None:
             self._scope = Map(
                 topology=self.config.root("topology"),
                 pattern=lambda x: Pattern(x),
                 format=lambda x, **kwa: x.format(**kwa),
-                prf_state=lambda x: PrfState(x),
+                prf_state_change=lambda pos: PrfStateChange(
+                    str(pos), self.prfstate[-2] if len(self.prfstate) > 1 else None
+                ),
+                write_prf_state=_write_prf_state,
             )
         return self._scope
 
     def update_scope(self, key, value=None, remove=False):
         if self._scope is None:
             self.scope()
         if not remove:
             self._scope[key] = value
         else:
             if key in self._scope:
                 del self._scope[key]
 
-    def decode_prfstate(self, data_str, only_on=False):
+    def update_prfstate(self, data_str):
         try:
-            prfstate = {}
             if data_str.startswith("PRFSTATE"):
-                prfstate = decode_prfstate(data_str.split(" ")[1])
-                if only_on:
-                    prfstate = {k: v for k, v in prfstate.items() if v == "ON"}
-                self.log.debug(f"prfstate_decoded={prfstate}")
-            return prfstate
+                self.prfstate.append(decode_prfstate(data_str.split(" ")[1]))
+                if len(self.prfstate) > 1:
+                    self.prfstate = self.prfstate[-2:]
+                self.log.debug(f"prfstate_decoded={self.prfstate[-1]}")
         except SerialJA121TException as e:
             self.log.error({str(e)})
 
     def on_mqtt_connect(self, client, userdata, flags, rc):
         for topic in self.topics_mqtt2serial:
             self.mqtt.subscribe(topic.name)
 
@@ -188,18 +207,19 @@
 
         self.log.debug(f"The event data parsed as JSON object: {data}")
         for topic in self.topics_mqtt2serial:
             if topic.name == topic_name:
                 if topic.disabled:
                     continue
                 for rule in topic.rules:
-                    topic.check_rule_data(rule.read, data, self.scope())
-                    self.log.debug(
-                        "The event data is valid according to the defined rules."
-                    )
+                    if rule.read is not None:
+                        topic.check_rule_data(rule.read, data, self.scope())
+                        self.log.debug(
+                            "The event data is valid according to the defined rules."
+                        )
                     _data = Map(data)
                     self.update_scope("data", _data)
                     try:
                         s = deep_eval(rule.write, self._scope)
                         self.request_queue.put(
                             Map(
                                 cor_id=_data.get(self.correlation_id),
@@ -214,15 +234,15 @@
     def on_serial_data(self, data):
         if not self.mqtt.connected:
             self.log.warn(
                 "No events will be published. The client is not connected to the MQTT broker."
             )
             return
 
-        prfstate = self.decode_prfstate(data, only_on=True)
+        self.update_prfstate(data)
         _rule = None
         current_time = time.time()
         for topic in self.topics_serial2mqtt:
             for rule in topic.rules:
                 if isinstance(rule.read, PythonExpression):
                     _data = rule.read.eval(self.scope())
                 else:
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/components/mqtt.py` & `ja2mqtt-1.0.3/ja2mqtt/components/mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class MQTT(Component):
     """
     MQTTClient provides an interface for MQTT broker.
     """
 
     def __init__(self, name, config):
-        super().__init__(config.get_part("mqtt-broker"), "mqtt")
+        super().__init__(config, "mqtt")
         self.client_name = name
         self.address = self.config.value_str("address")
         self.port = self.config.value_int("port", default=1883)
         self.keepalive = self.config.value_int("keepalive", default=60)
         self.reconnect_after = self.config.value_int("reconnect_after", default=30)
         self.loop_timeout = self.config.value_int("loop_timeout", default=1)
         self.client = None
@@ -44,15 +44,14 @@
     def __str__(self):
         return (
             f"{self.__class__}: name={self.name}, address={self.address}, port={self.port}, keepalive={self.keepalive}, "
             + f"reconnect_after={self.reconnect_after}, loop_timeout={self.loop_timeout}, connected={self.connected}"
         )
 
     def on_error(self, exception):
-        print(str(exception))
         self.log.error(str(exception))
         if self.on_error_ext is not None:
             self.on_error_ext(exception)
 
     def on_message(self, client, userdata, message):
         topic_name = message._topic.decode("utf-8")
         payload = str(message.payload.decode("utf-8"))
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/components/serial.py` & `ja2mqtt-1.0.3/ja2mqtt/components/serial.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import threading
 import time
 from queue import Queue
 
 import paho.mqtt.client as mqtt
 import serial as py_serial
 
-from ja2mqtt.config import Config
+from ja2mqtt.config import Config, ENCODING
 from ja2mqtt.utils import Map, PythonExpression, deep_eval, deep_merge, merge_dicts
 
 from . import Component
 from .simulator import Simulator
 
 
 class SerialJA121TException(Exception):
@@ -49,56 +49,55 @@
             for k in sorted(peripherals.keys())
         }
     except Exception as e:
         raise SerialJA121TException(
             f"Cannot decode prfstate string {prfstate}. {str(e)}"
         )
 
-def encode_prfstate(prf, prf_state_bits):
+
+def encode_prfstate(prf, prf_state_bits=24):
     """
     Encode prfstate from the prf state object. This is an inverse funtion to decode_prfstate,
     i.e. it must hold that `encode_prfstate(decode_prfstate(X)) == X`
     """
-    b = ''.zfill(prf_state_bits)
+    b = "".zfill(prf_state_bits)
     for p in prf.keys():
-        if prf[p] == 'ON':
+        if prf[p] == "ON":
             index = int(p)
-            b = b[:index] + '1' + b[index + 1:]
-    r = ''
+            b = b[:index] + "1" + b[index + 1 :]
+    r = ""
     for x in range(len(b) // 8):
-        h = hex(int(b[x*8:x*8+8][::-1], 2))
+        h = hex(int(b[x * 8 : x * 8 + 8][::-1], 2))
         h2 = h[2:].upper().zfill(2)
         r += h2
     return r
 
+
 class Serial(Component):
     """
     Serial provides an interface for the serial port where JA-121T is connected.
     """
 
-    def __init__(self, config):
+    def __init__(self, config, simulator):
         """
         Initialize the serial object. It reads configuration parameters from the config
         and creates `ser` object that can be either `PySerial` or `Simulator` based on the
         `use_simulator` property in the configuration.
         """
-        super().__init__(config.get_part("serial"), "serial")
-        self.encoding = self.config.value_bool("encoding", default="ascii")
+        super().__init__(config, "serial")
         self.use_simulator = self.config.value_bool("use_simulator", default=False)
         if not self.use_simulator:
             self.ser = None
             self.port = self.config.value_str("port", required=True)
             self.wait_on_ready = self.config.value_int("wait_on_ready", default=10)
             self.log.info(f"The serial connection configured, the port is {self.port}")
         else:
             self.port = "<simulator>"
-            self.ser = Simulator(config.get_part("simulator"), self.encoding)
-            self.log.info(
-                "The simulation is enabled, events will be simulated. The serial interface is not used."
-            )
+            self.ser = simulator
+            self.log.info("The serial interface events will be simulated.")
             self.log.debug(f"The simulator object is {self.ser}")
         self.buffer = Queue()
 
     def create_serial(self):
         """
         Create serial object and initialize the parameters from the configuration.
         """
@@ -116,16 +115,16 @@
         """
         Retrun True if the serial object exist.
         """
         return self.ser is not None
 
     def open(self, exit_event):
         """
-        Open serial interface. If the interface cannot be opened due to an error, try opening it
-        with frequency of `wait_on_ready` parameter.
+        Open serial interface. If the interface cannot be opened due to an error,
+        try opening it with frequency of `wait_on_ready` parameter.
         """
         if self.ser is None:
             self.log.info(f"Opening serial port {self.port}")
             while not exit_event.is_set():
                 try:
                     if not os.path.exists(self.port):
                         raise SerialJA121TException(
@@ -157,42 +156,45 @@
     def writeline(self, line):
         """
         Write a single line of string to the seiral port. It convers the string to bytes using
         the defined `encoding` and adds a LF at the end.
         """
         self.log.debug(f"Writing to serial: {line}")
         try:
-            self.ser.write(bytes(line + "\n", self.encoding))
+            self.ser.write(bytes(line + "\n", ENCODING))
         except Exception as e:
             self.log.error(str(e))
 
     def worker(self, exit_event):
         """
         The main worker of the serial object that reads data from the serial port and
         puts them to the queue `buffer`. Althoguh the `worker` method (that only reads
         the data from the serial port) can run in parallel with the `writeline` method,
-        due to the global interpreter lock (https://docs.python.org/3/glossary.html#term-global-interpreter-lock)
-        they both should be thread-safe.
+        due to the "global interpreter lock" they both should be thread-safe.
         """
         self.open(exit_event)
         try:
             while not exit_event.is_set():
                 try:
                     x = self.ser.readline()
                 except Exception as e:
                     self.log.error(
                         f"Error occured while reading data from the serial port. {str(e)}"
                     )
                     self.close()
                     self.open(exit_event)
                     continue
-                data_str = x.decode(self.encoding).strip("\r\n").strip()
-                if data_str != "":
-                    self.log.debug(f"Received data from serial: {data_str}")
-                    self.buffer.put(data_str)
+                try:
+                    data_str = x.decode(ENCODING).strip("\r\n").strip()
+                    if data_str != "":
+                        self.log.debug(f"Received data from serial: {data_str}")
+                        self.buffer.put(data_str)
+                except UnicodeDecodeError as e:
+                    self.log.error(str(e))
+                    continue
                 else:
                     # this is necessary to allow other threads to run too
                     exit_event.wait(0.2)
         finally:
             self.close()
             self.log.info("Serial worker ended.")
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/components/simulator.py` & `ja2mqtt-1.0.3/ja2mqtt/components/simulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # -*- coding: utf-8 -*-
 # @author: Tomas Vitvar, https://vitvar.com, tomas@vitvar.com
 
 from __future__ import absolute_import, unicode_literals
 
 import json
 import logging
+import random
 import re
 import threading
 import time
-import random
 from queue import Empty, Queue
 
-import paho.mqtt.client as mqtt
-import serial as py_serial
-
-from ja2mqtt.config import Config
 from ja2mqtt.utils import Map, PythonExpression, deep_eval, deep_merge, merge_dicts
 
 ERROR_INVALID_VALUE = "ERROR: 4 INVALID_VALUE"
 ERROR_NO_ACCESS = "ERROR: 3 NO_ACCESS"
 
+from ja2mqtt.config import ENCODING
 
-class SimilatorException(Exception):
+
+class SimulatorException(Exception):
     pass
 
 
 class Section:
     def __init__(self, data):
         self.code = data.code
         self.state = data.state
@@ -38,54 +36,63 @@
 
     def set(self):
         if self.state == "ARMED":
             return ERROR_INVALID_VALUE
         if self.state == "READY":
             self.state = "ARMED"
             return self.__str__()
-        raise SimilatorException(f"Cannot run command SET. Invalid state {self.state}.")
+        raise SimulatorException(f"Cannot run command SET. Invalid state {self.state}.")
 
     def unset(self):
         if self.state == "READY":
             return ERROR_INVALID_VALUE
         if self.state == "ARMED":
             self.state = "READY"
             return self.__str__()
-        raise SimilatorException(
+        raise SimulatorException(
             f"Cannot run command UNSET. Invalid state {self.state}."
         )
 
 
 class Simulator:
-    def __init__(self, config, encoding):
+    def __init__(self, config, prfstate_bits):
         self.log = logging.getLogger("simulator")
         self.config = config
         self.response_delay = config.value_int("response_delay", default=0.5)
-        self.prf_state_bits = config.value_int("prf_state_bits", default=24)
+        self.prfstate_bits = prfstate_bits
         self.rules = [Map(x) for x in config.value("rules")]
         self.sections = {
             str(x["code"]): Section(Map(x)) for x in config.value("sections")
         }
+        self.peripherals = [
+            int(x.strip())
+            for x in config.value("peripherals", default="1", required=False).split(",")
+        ]
         self.pin = config.value("pin")
         self.timeout = 1
         self.buffer = Queue()
-        self.encoding = encoding
 
     def __str__(self):
         return (
             f"{self.__class__}: pin={self.pin}, timeout={self.timeout}, response_delay={self.response_delay}, "
-            + f"prf_state_bits={self.prf_state_bits}, sections={[str(x) for x in self.sections.values()]}, rules={self.rules}"
+            + f"prfstate_bits={self.prfstate_bits}, sections={[str(x) for x in self.sections.values()]}, rules={self.rules}"
         )
 
     def open(self, exit_event):
         pass
 
     def close(self):
         pass
 
+    def generate_prfstate(self, on_prob=0.5):
+        return {
+            str(p): ("ON" if random.random() < on_prob else "OFF")
+            for p in self.peripherals
+        }
+
     def _add_to_buffer(self, data):
         time.sleep(self.response_delay)
         self.buffer.put(data)
 
     def write(self, data):
         def _match(pattern, data_str):
             m = re.compile(pattern).match(data_str)
@@ -96,73 +103,80 @@
 
         def _check_pin(command):
             if command.pin != str(self.pin):
                 self._add_to_buffer(ERROR_NO_ACCESS)
                 return False
             return True
 
-        data_str = data.decode(self.encoding).strip("\n")
+        data_str = data.decode(ENCODING).strip("\n")
 
         # SET and UNSET commands
         command = _match(
             "^(?P<pin>[0-9]+) (?P<command>SET|UNSET) (?P<code>[0-9]+)$",
             data_str,
         )
         if command is not None and _check_pin(command):
             section = self.sections.get(command.code)
             if section is not None:
                 data = {
                     "SET": lambda _: section.set(),
                     "UNSET": lambda _: section.unset(),
                     "N/A": lambda x: (_ for _ in ()).throw(
-                        SimilatorException(f"The command {x} is not implemented.")
+                        SimulatorException(f"The command {x} is not implemented.")
                     ),
                 }.get(command.command, "N/A")(command.command)
                 self._add_to_buffer(data)
             else:
                 self._add_to_buffer(ERROR_INVALID_VALUE)
             return
 
         # STATE command
         command = _match(
             "^(?P<pin>[0-9]+) (?P<command>STATE)( (?P<code>[0-9]+))?$", data_str
         )
         if command is not None and _check_pin(command):
-            print(command)
             sections = [
                 x
                 for x in self.sections.values()
                 if command.code is None or str(x.code) == str(command.code)
             ]
             time.sleep(self.response_delay)
             for section in sections:
                 self.buffer.put(str(section))
             return
 
+        # PRFSTATE command
+        command = _match("^(?P<command>PRFSTATE)$", data_str)
+        if command is not None:
+            from .serial import encode_prfstate
+
+            self._add_to_buffer(
+                "PRFSTATE " + encode_prfstate(self.generate_prfstate(on_prob=0.5))
+            )
+            return
+
     def readline(self):
         try:
-            return bytes(self.buffer.get(timeout=self.timeout), self.encoding)
+            return bytes(self.buffer.get(timeout=self.timeout), ENCODING)
         except Empty:
             return b""
 
     def scope(self):
-
         from .serial import encode_prfstate
 
         def _prf_random_states(*pos, on_prob=0.5):
-            prf = { str(p):("ON" if random.random() < on_prob else "OFF") for p in pos }
-            return "PRFSTATE " + encode_prfstate(prf, self.prf_state_bits)
+            prf = self.generate_prfstate(on_prob)
+            return "PRFSTATE " + encode_prfstate(prf, self.prfstate_bits)
 
         return Map(
-            random = lambda a,b: a+round(random.random()*b),
-            prf_randon_states = _prf_random_states,
+            random=lambda a, b: a + round(random.random() * b),
+            prf_random_states=_prf_random_states,
         )
 
     def worker(self, exit_event):
-
         _scope = self.scope()
 
         def _value(v):
             if isinstance(v, PythonExpression):
                 return v.eval(_scope)
             else:
                 return v
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/config.py` & `ja2mqtt-1.0.3/ja2mqtt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 DEBUG = str2bool(os.getenv("JA2MQTT_DEBUG", "False"))
 ANSI_COLORS = not str2bool(os.getenv("JA2MQTT_NO_ANSI", "False"))
 CONFIG_FILE = os.getenv("JA2MQTT_CONFIG", None)
 CONFIG_ENV = os.getenv("JA2MQTT_ENV", None)
 
 env_variables = ["JA2MQTT_DEBUG", "JA2MQTT_NO_ANSI", "JA2MQTT_CONFIG", "JA2MQTT_ENV"]
 
+ENCODING = "ascii"
+
 # global exit event
 exit_event = Event()
 
 
 class Jinja2TemplateLoader(jinja2.BaseLoader):
     def get_source(self, environment, template):
         if not os.path.exists(template):
@@ -230,15 +232,17 @@
             self,
             path,
             self.raw_config,
             self.config_dir,
         )
 
     def __call__(self, path, default=None, type=None, required=True, no_eval=False):
-        return self.root(path, default=None, type=None, required=True, no_eval=False)
+        return self.root(
+            path, default=default, type=type, required=required, no_eval=no_eval
+        )
 
 
 class ConfigPart:
     def __init__(self, parent, base_path, config, config_dir):
         self.parent = parent
         self.config_dir = config_dir
         self.base_path = base_path
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt/utils.py` & `ja2mqtt-1.0.3/ja2mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.2/ja2mqtt.egg-info/PKG-INFO` & `ja2mqtt-1.0.3/ja2mqtt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ja2mqtt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Jablotron MQTT bridge
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ja2mqtt-1.0.2/ja2mqtt.egg-info/SOURCES.txt` & `ja2mqtt-1.0.3/ja2mqtt.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 ja2mqtt/__init__.py
 ja2mqtt/__main__.py
 ja2mqtt/config.py
 ja2mqtt/utils.py
 ja2mqtt.egg-info/PKG-INFO
 ja2mqtt.egg-info/SOURCES.txt
 ja2mqtt.egg-info/dependency_links.txt
+ja2mqtt.egg-info/entry_points.txt
 ja2mqtt.egg-info/requires.txt
 ja2mqtt.egg-info/top_level.txt
 ja2mqtt/commands/__init__.py
 ja2mqtt/commands/config.py
+ja2mqtt/commands/ja2mqtt.py
 ja2mqtt/commands/run.py
 ja2mqtt/commands/test.py
 ja2mqtt/components/__init__.py
 ja2mqtt/components/bridge.py
 ja2mqtt/components/mqtt.py
 ja2mqtt/components/serial.py
 ja2mqtt/components/simulator.py
```

### Comparing `ja2mqtt-1.0.2/setup.py` & `ja2mqtt-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,21 +37,26 @@
 ]
 
 setup(
     name='ja2mqtt',
     version=__version__,
     description='Jablotron MQTT bridge',
     long_description=read('README-pypi.text'),
+    py_modules=['ja2mqtt'],
     author='Tomas Vitvar',
     author_email='tomas@vitvar.com',
     packages=find_packages(exclude=['tests.*', 'tests']),
     include_package_data=True,
     install_requires=install_requires,
     python_requires='>=3.6.0',
-    scripts=['bin/ja2mqtt'],
+    #scripts=['bin/ja2mqtt'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.7',
-    ]
+    ],
+    entry_points='''
+        [console_scripts]
+        ja2mqtt=ja2mqtt.commands.ja2mqtt:ja2mqtt
+    ''',
 )
```

