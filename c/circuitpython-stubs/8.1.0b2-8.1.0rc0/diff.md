# Comparing `tmp/circuitpython-stubs-8.1.0b2.tar.gz` & `tmp/circuitpython-stubs-8.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-stubs-8.1.0b2.tar", last modified: Wed Apr 26 22:56:15 2023, max compression
+gzip compressed data, was "circuitpython-stubs-8.1.0rc0.tar", last modified: Tue May 16 23:35:58 2023, max compression
```

## Comparing `circuitpython-stubs-8.1.0b2.tar` & `circuitpython-stubs-8.1.0rc0.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.924837 circuitpython-stubs-8.1.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-26 22:56:15.924837 circuitpython-stubs-8.1.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_bleio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_eve/
--rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_eve/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_pew/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_pew/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_pixelmap/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_pixelmap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_stage/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_stage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/adafruit_bus_device/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/adafruit_bus_device/i2c_device/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/adafruit_bus_device/i2c_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/adafruit_bus_device/spi_device/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/adafruit_bus_device/spi_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/adafruit_pixelbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/aesio/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/aesio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/alarm/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/alarm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/alarm/pin/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/alarm/pin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/alarm/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/alarm/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/alarm/touch/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/alarm/touch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/analogbufio/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/analogbufio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/analogio/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/analogio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/atexit/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/atexit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiobusio/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiobusio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiocore/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audioio/
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audioio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiomixer/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiomixer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiomp3/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiomp3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiopwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiopwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/bitbangio/
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/bitbangio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/bitmaptools/
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/bitmaptools/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/bitops/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/bitops/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/board/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/busio/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/busio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/camera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/canio/
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/canio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.924837 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/countio/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/countio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/cyw43/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/cyw43/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/digitalio/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/digitalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/displayio/
--rw-r--r--   0 runner    (1001) docker     (123)    40051 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/displayio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/dualbank/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/dualbank/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/espcamera/
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/espcamera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/espidf/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/espidf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/espnow/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/espnow/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/espulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/espulp/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/floppyio/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/floppyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/fontio/
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/fontio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/framebufferio/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/framebufferio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/frequencyio/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/frequencyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/getpass/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/getpass/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/gifio/
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/gifio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/gnss/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/gnss/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/hashlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/hashlib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/i2ctarget/
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/i2ctarget/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/imagecapture/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/imagecapture/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/ipaddress/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/ipaddress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/is31fl3741/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/is31fl3741/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/keypad/
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/keypad/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/math/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/mdns/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/mdns/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/memorymap/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/memorymap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/memorymonitor/
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/memorymonitor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/microcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/microcontroller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/msgpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/msgpack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/neopixel_write/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/neopixel_write/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/nvm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/nvm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/onewireio/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/onewireio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/os/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/os/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/paralleldisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/picodvi/
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/picodvi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/ps2io/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/ps2io/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/pulseio/
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/pulseio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/pwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/pwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/qrio/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/qrio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rainbowio/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/rainbowio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/random/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/random/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rgbmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rotaryio/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/rotaryio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rp2pio/
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/rp2pio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/rtc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/samd/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/samd/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/sdcardio/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/sdcardio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/sdioio/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/sdioio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:56:15.924837 circuitpython-stubs-8.1.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/sharpdisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/socketpool/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/socketpool/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/ssl/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/storage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/struct/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/struct/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/supervisor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/synthio/
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/synthio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/terminalio/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/terminalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/time/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/touchio/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/touchio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/traceback/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/traceback/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/uheap/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/uheap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/numpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/numpy/carray/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/numpy/carray/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/numpy/fft/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/numpy/fft/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/numpy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/numpy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/scipy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/scipy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/scipy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/scipy/optimize/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/user/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb_cdc/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb_cdc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb_hid/
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb_hid/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb_host/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb_host/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb_midi/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb_midi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ustack/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/ustack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/vectorio/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/vectorio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/watchdog/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/wifi/
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/wifi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/zlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.447275 circuitpython-stubs-8.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 23:35:58.447275 circuitpython-stubs-8.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.431276 circuitpython-stubs-8.1.0rc0/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_bleio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.431276 circuitpython-stubs-8.1.0rc0/_eve/
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_eve/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.431276 circuitpython-stubs-8.1.0rc0/_pew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_pew/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.431276 circuitpython-stubs-8.1.0rc0/_pixelmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_pixelmap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/_stage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/i2c_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/i2c_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/spi_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/adafruit_bus_device/spi_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/adafruit_pixelbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/aesio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/aesio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/alarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/alarm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/alarm/pin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/alarm/pin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/alarm/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/alarm/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/alarm/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/alarm/touch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/analogbufio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/analogbufio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/analogio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/analogio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/atexit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/atexit/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiobusio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiobusio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiocore/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audioio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiomixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiomixer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiomp3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiomp3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/audiopwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-16 23:35:47.000000 circuitpython-stubs-8.1.0rc0/audiopwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/bitbangio/
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/bitbangio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/bitmaptools/
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/bitmaptools/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/bitops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/bitops/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/board/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/busio/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/busio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/camera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/canio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.447275 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 23:35:57.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-16 23:35:58.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:35:57.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:35:57.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 23:35:57.000000 circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/countio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/countio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/cyw43/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/cyw43/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/digitalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/digitalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/displayio/
+-rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/displayio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/dualbank/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/dualbank/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/espcamera/
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/espcamera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/espidf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/espidf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/espnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/espnow/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/espulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/espulp/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.435276 circuitpython-stubs-8.1.0rc0/floppyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/floppyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/fontio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/fontio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/framebufferio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/framebufferio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/frequencyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/frequencyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/getpass/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/getpass/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/gifio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/gifio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/gnss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/gnss/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/hashlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/i2ctarget/
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/i2ctarget/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/imagecapture/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/imagecapture/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/ipaddress/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/ipaddress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/is31fl3741/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/is31fl3741/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/keypad/
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/keypad/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/math/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/mdns/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/mdns/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/memorymap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/memorymap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/memorymonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/memorymonitor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/microcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/microcontroller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/msgpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/msgpack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/neopixel_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/neopixel_write/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/nvm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/nvm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/onewireio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/onewireio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/os/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/os/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/paralleldisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/picodvi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/picodvi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/ps2io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/ps2io/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/pulseio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/pulseio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/pwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/pwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/qrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/qrio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rainbowio/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/rainbowio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/random/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rgbmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rotaryio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/rotaryio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rp2pio/
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/rp2pio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/rtc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/samd/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/samd/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/sdcardio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/sdcardio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.439276 circuitpython-stubs-8.1.0rc0/sdioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/sdioio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 23:35:58.447275 circuitpython-stubs-8.1.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-16 23:35:50.000000 circuitpython-stubs-8.1.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/sharpdisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/socketpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/socketpool/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/ssl/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/storage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/struct/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-16 23:35:48.000000 circuitpython-stubs-8.1.0rc0/supervisor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/synthio/
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/synthio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/terminalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/terminalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/touchio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/touchio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/traceback/
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/traceback/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/uheap/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/uheap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/numpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/numpy/carray/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/numpy/carray/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/numpy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/numpy/fft/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/numpy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/numpy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/scipy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/scipy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/scipy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/scipy/optimize/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/user/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ulab/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ulab/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb_cdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb_cdc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb_hid/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb_host/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb_host/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/usb_midi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/usb_midi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/ustack/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/ustack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/vectorio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/vectorio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/watchdog/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/wifi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:35:58.443276 circuitpython-stubs-8.1.0rc0/zlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-16 23:35:49.000000 circuitpython-stubs-8.1.0rc0/zlib/__init__.pyi
```

### Comparing `circuitpython-stubs-8.1.0b2/README.rst` & `circuitpython-stubs-8.1.0rc0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/_bleio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/_eve/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/_pew/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/_pixelmap/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/_stage/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/adafruit_bus_device/i2c_device/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/adafruit_bus_device/i2c_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/adafruit_bus_device/spi_device/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/adafruit_bus_device/spi_device/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 
+from typing import Optional
+
 import busio
 import digitalio
 
 class SPIDevice:
     """SPI Device Manager"""
 
     def __init__(
         self,
         spi: busio.SPI,
-        chip_select: digitalio.DigitalInOut,
+        chip_select: Optional[digitalio.DigitalInOut] = None,
         *,
         baudrate: int = 100000,
         polarity: int = 0,
         phase: int = 0,
         extra_clocks: int = 0,
     ) -> None:
         """
         Represents a single SPI device and manages locking the bus and the device address.
 
         :param ~busio.SPI spi: The SPI bus the device is on
-        :param ~digitalio.DigitalInOut chip_select: The chip select pin object that implements the DigitalInOut API.
+        :param ~digitalio.DigitalInOut chip_select: The chip select pin object that implements the DigitalInOut API. ``None`` if a chip select pin is not being used.
         :param bool cs_active_value: Set to true if your device requires CS to be active high. Defaults to false.
         :param int extra_clocks: The minimum number of clock cycles to cycle the bus after CS is high. (Used for SD cards.)
 
         Example::
 
             import busio
             import digitalio
```

### Comparing `circuitpython-stubs-8.1.0b2/adafruit_pixelbuf/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/aesio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/alarm/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/alarm/pin/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/alarm/pin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/alarm/time/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/alarm/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/alarm/touch/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/alarm/touch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/analogbufio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/analogio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/atexit/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/audiobusio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/audiocore/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/audioio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/audiomixer/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/audiomp3/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/audiopwmio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/bitbangio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/bitmaptools/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/bitops/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/board/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/busio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/camera/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/canio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/SOURCES.txt` & `circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/top_level.txt` & `circuitpython-stubs-8.1.0rc0/circuitpython_stubs.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/countio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/cyw43/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/cyw43/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/digitalio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/displayio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/displayio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 refer to `this Learn guide
 <https://learn.adafruit.com/circuitpython-display-support-using-displayio>`_.
 """
 
 from __future__ import annotations
 
 import typing
-from typing import Optional, Tuple, Union
+from typing import Iterator, Optional, Tuple, Union
 
 import busio
 import circuitpython_typing
 import microcontroller
 import vectorio
 from circuitpython_typing import ReadableBuffer, WriteableBuffer
 
@@ -567,14 +567,25 @@
         layer: Union[
             vectorio.Circle, vectorio.Rectangle, vectorio.Polygon, Group, TileGrid
         ],
     ) -> None:
         """Remove the first copy of layer. Raises ValueError if it is not present."""
         ...
     def __bool__(self) -> bool: ...
+    def __contains__(
+        self,
+        item: Union[
+            vectorio.Circle, vectorio.Rectangle, vectorio.Polygon, Group, TileGrid
+        ],
+    ) -> bool: ...
+    def __iter__(
+        self,
+    ) -> Iterator[
+        Union[vectorio.Circle, vectorio.Rectangle, vectorio.Polygon, Group, TileGrid]
+    ]: ...
     def __len__(self) -> int:
         """Returns the number of layers in a Group"""
         ...
     def __getitem__(
         self, index: int
     ) -> Union[vectorio.Circle, vectorio.Rectangle, vectorio.Polygon, Group, TileGrid]:
         """Returns the value at the given index.
```

### Comparing `circuitpython-stubs-8.1.0b2/dualbank/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/espcamera/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/espcamera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/espidf/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/espidf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/espnow/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/espnow/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/espulp/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/espulp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/floppyio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/fontio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/framebufferio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/frequencyio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/getpass/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/gifio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/gnss/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/hashlib/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/i2ctarget/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/imagecapture/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/ipaddress/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/is31fl3741/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/keypad/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/math/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/mdns/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/memorymap/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/memorymonitor/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/microcontroller/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/microcontroller/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -95,16 +95,23 @@
     def __init__(self) -> None:
         """You cannot create an instance of `microcontroller.Processor`.
         Use `microcontroller.cpu` to access the sole instance available."""
         ...
     frequency: int
     """The CPU operating frequency in Hertz.
 
-    **Limitations:** Setting the ``frequency`` is possible only on some i.MX boards.
-    On most boards, ``frequency`` is read-only.
+    **Limitations:** On most boards, ``frequency`` is read-only. Setting
+    the ``frequency`` is possible on RP2040 boards and some i.MX boards.
+
+    .. warning:: Overclocking likely voids your warranties and may reduce
+      the lifetime of the chip.
+
+    .. warning:: Changing the frequency may cause issues with other
+      subsystems, such as USB, PWM, and PIO. To minimize issues, set the CPU
+      frequency before initializing other systems.
     """
     reset_reason: microcontroller.ResetReason
     """The reason the microcontroller started up from reset state."""
     temperature: Optional[float]
     """The on-chip temperature, in Celsius, as a float. (read-only)
 
     Is `None` if the temperature is not available.
```

### Comparing `circuitpython-stubs-8.1.0b2/msgpack/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/neopixel_write/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/nvm/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/onewireio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/os/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/paralleldisplay/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/picodvi/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/picodvi/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Low-level routines for interacting with PicoDVI Output"""
 
 from __future__ import annotations
 
 import microcontroller
 
 class Framebuffer:
-    """A PicoDVI managed frame buffer."""
-
     def __init__(
         self,
         width: int,
         height: int,
         *,
         clk_dp: microcontroller.Pin,
         clk_dn: microcontroller.Pin,
@@ -18,44 +16,45 @@
         red_dn: microcontroller.Pin,
         green_dp: microcontroller.Pin,
         green_dn: microcontroller.Pin,
         blue_dp: microcontroller.Pin,
         blue_dn: microcontroller.Pin,
         color_depth: int = 8,
     ) -> None:
-        """Create a Framebuffer object with the given dimensions (640x480 or 800x480). Memory is
-           allocated outside of onto the heap and then moved outside on VM
-           end.
-
-        This will change the system clock speed to match the DVI signal.
-        Make sure to initialize other objects after this one so they account
-        for the changed clock. This also allocates a very large framebuffer
-        and is most likely to succeed the earlier it is attempted.
+        """Create a Framebuffer object with the given dimensions. Memory is
+        allocated outside of onto the heap and then moved outside on VM end.
+
+        .. warning:: This will change the system clock speed to match the DVI signal.
+           Make sure to initialize other objects after this one so they account
+           for the changed clock.
+
+        This allocates a very large framebuffer and is most likely to succeed
+        the earlier it is attempted.
 
         Each dp and dn pair of pins must be neighboring, such as 19 and 20.
         They must also be ordered the same way. In other words, dp must be
         less than dn for all pairs or dp must be greater than dn for all pairs.
 
         The framebuffer pixel format varies depending on color_depth:
+
         * 1 - Each bit is a pixel. Either white (1) or black (0).
         * 2 - Each 2 bits is a pixels. Grayscale between white (0x3) and black (0x0).
         * 8 - Each byte is a pixels in RGB332 format.
         * 16 - Each two bytes are a pixel in RGB565 format.
 
-        Monochrome framebuffers (color_depth=1 or 2) will be full resolution.
-        Color framebuffers will be half resolution and pixels will be
-        duplicated to create a signal with the target dimensions.
+        Two output resolutions are currently supported, 640x480 and 800x480.
+        Monochrome framebuffers (color_depth=1 or 2) must be full resolution.
+        Color framebuffers must be half resolution (320x240 or 400x240) and
+        pixels will be duplicated to create the signal.
 
         A Framebuffer is often used in conjunction with a
         `framebufferio.FramebufferDisplay`.
 
-        :param int width: the width of the target display signal. It will be halved when
-          color_depth >= 8 when creating the framebuffer. Only 640 or 800 is currently supported.
-        :param int height: the height of the target display signal. It will be halved when
-          color_depth >= 8 when creating the framebuffer. Only 480 is currently supported.
+        :param int width: the width of the target display signal. Only 320, 400, 640 or 800 is currently supported depending on color_depth.
+        :param int height: the height of the target display signal. Only 240 or 480 is currently supported depending on color_depth.
         :param ~microcontroller.Pin clk_dp: the positive clock signal pin
         :param ~microcontroller.Pin clk_dn: the negative clock signal pin
         :param ~microcontroller.Pin red_dp: the positive red signal pin
         :param ~microcontroller.Pin red_dn: the negative red signal pin
         :param ~microcontroller.Pin green_dp: the positive green signal pin
         :param ~microcontroller.Pin green_dn: the negative green signal pin
         :param ~microcontroller.Pin blue_dp: the positive blue signal pin
@@ -65,12 +64,10 @@
         """
     def deinit(self) -> None:
         """Free the resources (pins, timers, etc.) associated with this
         `picodvi.Framebuffer` instance.  After deinitialization, no further operations
         may be performed."""
         ...
     width: int
-    """The width of the framebuffer, in pixels. It may be doubled for output (and half of what
-       width was given to __init__.)"""
+    """The width of the framebuffer, in pixels. It may be doubled for output."""
     height: int
-    """The width of the framebuffer, in pixels. It may be doubled for output (and half of what
-       width was given to __init__.)"""
+    """The width of the framebuffer, in pixels. It may be doubled for output."""
```

### Comparing `circuitpython-stubs-8.1.0b2/ps2io/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/pulseio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/pwmio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/qrio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/random/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/rgbmatrix/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/rotaryio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/rp2pio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/rp2pio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/rtc/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/samd/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/samd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/sdcardio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/sdioio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/setup.py` & `circuitpython-stubs-8.1.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/sharpdisplay/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/socketpool/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/ssl/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/storage/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/struct/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/supervisor/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/terminalio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/time/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/touchio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/traceback/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/ulab/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ulab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/ulab/numpy/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ulab/numpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/ulab/numpy/carray/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ulab/numpy/carray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/ulab/numpy/fft/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ulab/numpy/fft/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/ulab/numpy/linalg/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ulab/numpy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/ulab/scipy/linalg/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ulab/scipy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/ulab/scipy/optimize/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/ulab/scipy/optimize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/usb/core/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/usb/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/usb_cdc/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/usb_hid/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/usb_host/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/usb_midi/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/vectorio/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/watchdog/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b2/wifi/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/wifi/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -224,27 +224,42 @@
         netmask: ipaddress.IPv4Address,
         gateway: ipaddress.IPv4Address,
         ipv4_dns: Optional[ipaddress.IPv4Address],
     ) -> None:
         """Sets the IP v4 address of the station. Must include the netmask and gateway. DNS address is optional.
         Setting the address manually will stop the DHCP client."""
         ...
+    def set_ipv4_address_ap(
+        self,
+        *,
+        ipv4: ipaddress.IPv4Address,
+        netmask: ipaddress.IPv4Address,
+        gateway: ipaddress.IPv4Address,
+    ) -> None:
+        """Sets the IP v4 address of the access point. Must include the netmask and gateway."""
+        ...
     ipv4_address: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the station when connected to an access point. None otherwise. (read-only)"""
     ipv4_address_ap: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the access point, when enabled. None otherwise."""
     ipv4_dns: ipaddress.IPv4Address
     """IP v4 Address of the DNS server to be used."""
     ap_info: Optional[Network]
     """Network object containing BSSID, SSID, authmode, channel, country and RSSI when connected to an access point. None otherwise."""
     def start_dhcp(self) -> None:
-        """Starts the DHCP client."""
+        """Starts the station DHCP client."""
         ...
     def stop_dhcp(self) -> None:
-        """Stops the DHCP client. Needed to assign a static IP address."""
+        """Stops the station DHCP client. Needed to assign a static IP address."""
+        ...
+    def start_dhcp_ap(self) -> None:
+        """Starts the access point DHCP server."""
+        ...
+    def stop_dhcp_ap(self) -> None:
+        """Stops the access point DHCP server. Needed to assign a static IP address."""
         ...
     def ping(
         self, ip: ipaddress.IPv4Address, *, timeout: Optional[float] = 0.5
     ) -> Optional[float]:
         """Ping an IP to test connectivity. Returns echo time in seconds.
         Returns None when it times out."""
         ...
```

### Comparing `circuitpython-stubs-8.1.0b2/zlib/__init__.pyi` & `circuitpython-stubs-8.1.0rc0/zlib/__init__.pyi`

 * *Files identical despite different names*

