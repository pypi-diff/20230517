# Comparing `tmp/pywapor-3.3.4.tar.gz` & `tmp/pywapor-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywapor-3.3.4.tar", last modified: Wed Apr 26 14:18:25 2023, max compression
+gzip compressed data, was "pywapor-3.3.5.tar", last modified: Wed May 17 15:15:42 2023, max compression
```

## Comparing `pywapor-3.3.4.tar` & `pywapor-3.3.5.tar`

### file list

```diff
@@ -1,124 +1,108 @@
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.185048 pywapor-3.3.4/
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2022-06-23 13:36:53.000000 pywapor-3.3.4/LICENSE
--rw-r--r--   0 hmcoerver   (501) staff       (20)      229 2022-08-29 07:22:20.000000 pywapor-3.3.4/MANIFEST.in
--rw-r--r--   0 hmcoerver   (501) staff       (20)      457 2023-04-26 14:18:25.184918 pywapor-3.3.4/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11246 2023-04-05 09:03:16.000000 pywapor-3.3.4/README.md
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.139938 pywapor-3.3.4/pywapor/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      416 2023-04-26 10:51:30.000000 pywapor-3.3.4/pywapor/__init__.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.141391 pywapor-3.3.4/pywapor/collect/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      241 2022-09-28 07:45:21.000000 pywapor-3.3.4/pywapor/collect/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13487 2023-01-25 04:36:11.000000 pywapor-3.3.4/pywapor/collect/accounts.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9150 2023-01-12 09:57:39.000000 pywapor-3.3.4/pywapor/collect/downloader.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.159371 pywapor-3.3.4/pywapor/collect/product/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5802 2023-01-05 11:26:49.000000 pywapor-3.3.4/pywapor/collect/product/CHIRPS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8172 2023-04-14 12:52:07.000000 pywapor-3.3.4/pywapor/collect/product/COPERNICUS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8387 2022-09-29 11:29:30.000000 pywapor-3.3.4/pywapor/collect/product/ERA5.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6154 2023-04-19 09:01:02.000000 pywapor-3.3.4/pywapor/collect/product/GEOS5.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1110900 2022-08-24 12:33:55.000000 pywapor-3.3.4/pywapor/collect/product/GLO30.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1111950 2022-08-24 12:33:41.000000 pywapor-3.3.4/pywapor/collect/product/GLO90.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5808 2023-01-06 12:00:32.000000 pywapor-3.3.4/pywapor/collect/product/GLOBCOVER.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    40234 2023-01-25 04:40:44.000000 pywapor-3.3.4/pywapor/collect/product/LANDSAT.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.164824 pywapor-3.3.4/pywapor/collect/product/Landsat/
--rw-r--r--   0 hmcoerver   (501) staff       (20)    25684 2022-09-28 09:16:32.000000 pywapor-3.3.4/pywapor/collect/product/Landsat/C2L2SP.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      250 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/product/Landsat/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8549 2023-01-05 10:39:18.000000 pywapor-3.3.4/pywapor/collect/product/MERRA2.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13898 2023-02-10 10:58:24.000000 pywapor-3.3.4/pywapor/collect/product/MODIS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1232314 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/product/MODIS_tiles.geojson
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11566 2023-01-04 09:31:52.000000 pywapor-3.3.4/pywapor/collect/product/PROBAV.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    23350 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/collect/product/SENTINEL2.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6555 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/collect/product/SENTINEL3.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7297 2022-12-22 13:02:32.000000 pywapor-3.3.4/pywapor/collect/product/SRTM.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  3610761 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/product/SRTM30_tiles.geojson
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7204 2023-01-05 10:39:59.000000 pywapor-3.3.4/pywapor/collect/product/STATICS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    20125 2023-04-13 12:04:14.000000 pywapor-3.3.4/pywapor/collect/product/VIIRSL1.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      372 2023-01-10 14:54:30.000000 pywapor-3.3.4/pywapor/collect/product/__init__.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.166393 pywapor-3.3.4/pywapor/collect/protocol/
--rw-r--r--   0 hmcoerver   (501) staff       (20)       33 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/protocol/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9062 2023-01-03 17:06:31.000000 pywapor-3.3.4/pywapor/collect/protocol/cds.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3904 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/collect/protocol/cog.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9912 2023-04-19 08:49:47.000000 pywapor-3.3.4/pywapor/collect/protocol/crawler.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9446 2023-04-19 09:02:03.000000 pywapor-3.3.4/pywapor/collect/protocol/opendap.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1572 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/protocol/projections.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12012 2023-03-17 16:51:06.000000 pywapor-3.3.4/pywapor/collect/protocol/sentinelapi.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.168783 pywapor-3.3.4/pywapor/enhancers/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      223 2022-09-30 08:36:06.000000 pywapor-3.3.4/pywapor/enhancers/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      886 2022-09-28 11:29:36.000000 pywapor-3.3.4/pywapor/enhancers/apply_enhancers.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2577 2023-01-04 13:41:38.000000 pywapor-3.3.4/pywapor/enhancers/dem.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.170422 pywapor-3.3.4/pywapor/enhancers/dms/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      175 2022-09-30 08:43:00.000000 pywapor-3.3.4/pywapor/enhancers/dms/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    36143 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/enhancers/dms/pyDMS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10174 2022-09-16 14:57:12.000000 pywapor-3.3.4/pywapor/enhancers/dms/pyDMS_utils.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15479 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/enhancers/dms/thermal_sharpener.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2066 2023-01-11 15:57:27.000000 pywapor-3.3.4/pywapor/enhancers/gap_fill.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8897 2023-01-04 14:25:21.000000 pywapor-3.3.4/pywapor/enhancers/lulc.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      616 2022-09-28 11:32:40.000000 pywapor-3.3.4/pywapor/enhancers/other.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      348 2022-09-28 11:33:29.000000 pywapor-3.3.4/pywapor/enhancers/pressure.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.171934 pywapor-3.3.4/pywapor/enhancers/smooth/
--rw-r--r--   0 hmcoerver   (501) staff       (20)        0 2023-03-02 12:28:19.000000 pywapor-3.3.4/pywapor/enhancers/smooth/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    17945 2023-04-04 12:24:13.000000 pywapor-3.3.4/pywapor/enhancers/smooth/archive.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6710 2023-04-26 10:49:45.000000 pywapor-3.3.4/pywapor/enhancers/smooth/core.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10601 2023-04-25 10:30:52.000000 pywapor-3.3.4/pywapor/enhancers/smooth/plotters.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13564 2023-04-25 12:17:43.000000 pywapor-3.3.4/pywapor/enhancers/smooth/whittaker.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10210 2022-09-28 11:37:26.000000 pywapor-3.3.4/pywapor/enhancers/temperature.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1003 2022-09-28 11:39:56.000000 pywapor-3.3.4/pywapor/enhancers/wind.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    18917 2023-01-17 16:22:18.000000 pywapor-3.3.4/pywapor/et_look.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.176347 pywapor-3.3.4/pywapor/et_look_dev/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7291 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1221 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/biomass.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12699 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/clear_sky_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3840 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/constants.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5939 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/evapotranspiration.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6371 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_dev/leaf.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    28680 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_dev/meteo.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7133 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/neutral.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13821 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     4357 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/resistance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7562 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_dev/roughness.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    31961 2022-08-23 08:30:34.000000 pywapor-3.3.4/pywapor/et_look_dev/soil_moisture.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    33779 2022-09-19 16:03:01.000000 pywapor-3.3.4/pywapor/et_look_dev/solar_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5671 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_dev/stress.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    21516 2023-01-26 11:30:09.000000 pywapor-3.3.4/pywapor/et_look_dev/unstable.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.180328 pywapor-3.3.4/pywapor/et_look_v2_v3/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7216 2022-08-23 08:57:05.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9037 2022-06-23 15:01:24.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/biomass.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12950 2022-08-30 08:32:15.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/clear_sky_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3891 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/constants.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5008 2022-08-23 08:57:03.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/evapotranspiration.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5403 2022-08-23 07:31:32.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/leaf.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    31410 2022-08-30 08:24:51.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/meteo.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7248 2022-08-23 08:57:00.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/neutral.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13996 2022-08-23 08:56:51.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3833 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/resistance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7345 2023-01-05 10:38:52.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/roughness.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32038 2022-08-30 08:22:31.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/soil_moisture.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15852 2022-09-19 16:35:35.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/solar_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5011 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/stress.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    23799 2022-08-31 14:11:30.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/unstable.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.184538 pywapor-3.3.4/pywapor/general/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      294 2022-09-21 12:21:59.000000 pywapor-3.3.4/pywapor/general/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8550 2023-04-14 09:51:55.000000 pywapor-3.3.4/pywapor/general/aligner.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    22239 2022-06-30 13:24:46.000000 pywapor-3.3.4/pywapor/general/bitmasks.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12818 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/general/compositer.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7414 2023-04-13 13:02:47.000000 pywapor-3.3.4/pywapor/general/curvilinear.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3065 2023-01-05 09:12:37.000000 pywapor-3.3.4/pywapor/general/lazifier.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    28534 2023-04-13 09:53:40.000000 pywapor-3.3.4/pywapor/general/levels.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2103 2023-04-13 09:40:27.000000 pywapor-3.3.4/pywapor/general/logger.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11401 2022-09-28 10:51:57.000000 pywapor-3.3.4/pywapor/general/network.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2352 2022-09-28 10:56:25.000000 pywapor-3.3.4/pywapor/general/performance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1885 2023-01-06 12:39:34.000000 pywapor-3.3.4/pywapor/general/pre_defaults.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    16701 2023-04-04 09:46:53.000000 pywapor-3.3.4/pywapor/general/processing_functions.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12552 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/general/reproject.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2538 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/general/units.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32644 2023-01-05 08:22:50.000000 pywapor-3.3.4/pywapor/general/variables.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    18087 2022-08-26 10:45:16.000000 pywapor-3.3.4/pywapor/post_et_look.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7145 2023-01-10 14:36:33.000000 pywapor-3.3.4/pywapor/pre_et_look.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7014 2023-04-14 09:20:37.000000 pywapor-3.3.4/pywapor/pre_se_root.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    14976 2023-01-04 08:27:07.000000 pywapor-3.3.4/pywapor/se_root.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.140725 pywapor-3.3.4/pywapor.egg-info/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      457 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3495 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/SOURCES.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/dependency_links.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)      280 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/requires.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/top_level.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2023-04-26 14:18:25.185086 pywapor-3.3.4/setup.cfg
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2001 2023-04-26 10:51:26.000000 pywapor-3.3.4/setup.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.559496 pywapor-3.3.5/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2022-06-23 13:36:53.000000 pywapor-3.3.5/LICENSE
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      229 2022-08-29 07:22:20.000000 pywapor-3.3.5/MANIFEST.in
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      457 2023-05-17 15:15:42.559370 pywapor-3.3.5/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11256 2023-04-28 08:59:15.000000 pywapor-3.3.5/README.md
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.525628 pywapor-3.3.5/pywapor/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      388 2023-05-17 14:47:19.000000 pywapor-3.3.5/pywapor/__init__.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.526633 pywapor-3.3.5/pywapor/collect/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      241 2022-09-28 07:45:21.000000 pywapor-3.3.5/pywapor/collect/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13487 2023-01-25 04:36:11.000000 pywapor-3.3.5/pywapor/collect/accounts.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9166 2023-05-17 09:36:59.000000 pywapor-3.3.5/pywapor/collect/downloader.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.548727 pywapor-3.3.5/pywapor/collect/product/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5802 2023-01-05 11:26:49.000000 pywapor-3.3.5/pywapor/collect/product/CHIRPS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8172 2023-05-17 07:52:24.000000 pywapor-3.3.5/pywapor/collect/product/COPERNICUS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8387 2022-09-29 11:29:30.000000 pywapor-3.3.5/pywapor/collect/product/ERA5.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6154 2023-04-19 09:01:02.000000 pywapor-3.3.5/pywapor/collect/product/GEOS5.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1110900 2022-08-24 12:33:55.000000 pywapor-3.3.5/pywapor/collect/product/GLO30.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1111950 2022-08-24 12:33:41.000000 pywapor-3.3.5/pywapor/collect/product/GLO90.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5808 2023-01-06 12:00:32.000000 pywapor-3.3.5/pywapor/collect/product/GLOBCOVER.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    40576 2023-05-17 08:52:40.000000 pywapor-3.3.5/pywapor/collect/product/LANDSAT.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.550471 pywapor-3.3.5/pywapor/collect/product/Landsat/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    25684 2022-09-28 09:16:32.000000 pywapor-3.3.5/pywapor/collect/product/Landsat/C2L2SP.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      250 2022-06-23 13:41:57.000000 pywapor-3.3.5/pywapor/collect/product/Landsat/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8549 2023-01-05 10:39:18.000000 pywapor-3.3.5/pywapor/collect/product/MERRA2.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13898 2023-04-28 08:55:49.000000 pywapor-3.3.5/pywapor/collect/product/MODIS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1232314 2022-06-23 13:41:57.000000 pywapor-3.3.5/pywapor/collect/product/MODIS_tiles.geojson
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11566 2023-01-04 09:31:52.000000 pywapor-3.3.5/pywapor/collect/product/PROBAV.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    24232 2023-05-17 09:31:52.000000 pywapor-3.3.5/pywapor/collect/product/SENTINEL2.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6563 2023-05-17 11:16:45.000000 pywapor-3.3.5/pywapor/collect/product/SENTINEL3.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7297 2022-12-22 13:02:32.000000 pywapor-3.3.5/pywapor/collect/product/SRTM.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  3610761 2022-06-23 13:41:57.000000 pywapor-3.3.5/pywapor/collect/product/SRTM30_tiles.geojson
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7204 2023-01-05 10:39:59.000000 pywapor-3.3.5/pywapor/collect/product/STATICS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    20125 2023-04-13 12:04:14.000000 pywapor-3.3.5/pywapor/collect/product/VIIRSL1.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      372 2023-01-10 14:54:30.000000 pywapor-3.3.5/pywapor/collect/product/__init__.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.551846 pywapor-3.3.5/pywapor/collect/protocol/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       33 2022-06-23 13:41:57.000000 pywapor-3.3.5/pywapor/collect/protocol/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9062 2023-01-03 17:06:31.000000 pywapor-3.3.5/pywapor/collect/protocol/cds.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3904 2023-04-12 12:40:20.000000 pywapor-3.3.5/pywapor/collect/protocol/cog.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9912 2023-04-19 08:49:47.000000 pywapor-3.3.5/pywapor/collect/protocol/crawler.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9445 2023-04-28 15:23:30.000000 pywapor-3.3.5/pywapor/collect/protocol/opendap.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1572 2022-06-23 13:41:57.000000 pywapor-3.3.5/pywapor/collect/protocol/projections.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12012 2023-03-17 16:51:06.000000 pywapor-3.3.5/pywapor/collect/protocol/sentinelapi.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.552888 pywapor-3.3.5/pywapor/enhancers/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      223 2022-09-30 08:36:06.000000 pywapor-3.3.5/pywapor/enhancers/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      886 2022-09-28 11:29:36.000000 pywapor-3.3.5/pywapor/enhancers/apply_enhancers.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2577 2023-01-04 13:41:38.000000 pywapor-3.3.5/pywapor/enhancers/dem.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.554108 pywapor-3.3.5/pywapor/enhancers/dms/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      175 2022-09-30 08:43:00.000000 pywapor-3.3.5/pywapor/enhancers/dms/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    36143 2023-04-12 12:40:20.000000 pywapor-3.3.5/pywapor/enhancers/dms/pyDMS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10174 2022-09-16 14:57:12.000000 pywapor-3.3.5/pywapor/enhancers/dms/pyDMS_utils.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15700 2023-05-17 11:35:35.000000 pywapor-3.3.5/pywapor/enhancers/dms/thermal_sharpener.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2066 2023-01-11 15:57:27.000000 pywapor-3.3.5/pywapor/enhancers/gap_fill.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8897 2023-01-04 14:25:21.000000 pywapor-3.3.5/pywapor/enhancers/lulc.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      616 2022-09-28 11:32:40.000000 pywapor-3.3.5/pywapor/enhancers/other.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      348 2022-09-28 11:33:29.000000 pywapor-3.3.5/pywapor/enhancers/pressure.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.555109 pywapor-3.3.5/pywapor/enhancers/smooth/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        0 2023-03-02 12:28:19.000000 pywapor-3.3.5/pywapor/enhancers/smooth/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    17945 2023-04-04 12:24:13.000000 pywapor-3.3.5/pywapor/enhancers/smooth/archive.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6710 2023-04-26 10:49:45.000000 pywapor-3.3.5/pywapor/enhancers/smooth/core.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10601 2023-04-25 10:30:52.000000 pywapor-3.3.5/pywapor/enhancers/smooth/plotters.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13753 2023-05-17 13:28:36.000000 pywapor-3.3.5/pywapor/enhancers/smooth/whittaker.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10210 2022-09-28 11:37:26.000000 pywapor-3.3.5/pywapor/enhancers/temperature.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1003 2022-09-28 11:39:56.000000 pywapor-3.3.5/pywapor/enhancers/wind.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    16322 2023-05-17 13:56:45.000000 pywapor-3.3.5/pywapor/et_look.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.557114 pywapor-3.3.5/pywapor/et_look_v2_v3/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7216 2022-08-23 08:57:05.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9037 2022-06-23 15:01:24.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/biomass.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12950 2022-08-30 08:32:15.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/clear_sky_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3891 2022-06-23 13:36:53.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/constants.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5008 2022-08-23 08:57:03.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/evapotranspiration.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5403 2022-08-23 07:31:32.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/leaf.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    31410 2022-08-30 08:24:51.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/meteo.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7248 2022-08-23 08:57:00.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/neutral.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13996 2022-08-23 08:56:51.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3833 2022-06-23 13:36:53.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/resistance.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7345 2023-01-05 10:38:52.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/roughness.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32038 2022-08-30 08:22:31.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/soil_moisture.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15852 2022-09-19 16:35:35.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/solar_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5011 2022-06-23 13:41:57.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/stress.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    23799 2022-08-31 14:11:30.000000 pywapor-3.3.5/pywapor/et_look_v2_v3/unstable.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.559187 pywapor-3.3.5/pywapor/general/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      294 2022-09-21 12:21:59.000000 pywapor-3.3.5/pywapor/general/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8807 2023-05-17 11:23:35.000000 pywapor-3.3.5/pywapor/general/aligner.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    22239 2022-06-30 13:24:46.000000 pywapor-3.3.5/pywapor/general/bitmasks.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12818 2023-04-12 12:40:20.000000 pywapor-3.3.5/pywapor/general/compositer.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7414 2023-04-13 13:02:47.000000 pywapor-3.3.5/pywapor/general/curvilinear.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3065 2023-01-05 09:12:37.000000 pywapor-3.3.5/pywapor/general/lazifier.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32301 2023-05-17 13:07:38.000000 pywapor-3.3.5/pywapor/general/levels.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2103 2023-04-13 09:40:27.000000 pywapor-3.3.5/pywapor/general/logger.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11401 2022-09-28 10:51:57.000000 pywapor-3.3.5/pywapor/general/network.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2352 2022-09-28 10:56:25.000000 pywapor-3.3.5/pywapor/general/performance.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1885 2023-01-06 12:39:34.000000 pywapor-3.3.5/pywapor/general/pre_defaults.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    16701 2023-04-04 09:46:53.000000 pywapor-3.3.5/pywapor/general/processing_functions.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12552 2023-04-12 12:40:20.000000 pywapor-3.3.5/pywapor/general/reproject.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2538 2022-06-23 13:41:57.000000 pywapor-3.3.5/pywapor/general/units.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32644 2023-01-05 08:22:50.000000 pywapor-3.3.5/pywapor/general/variables.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    18087 2022-08-26 10:45:16.000000 pywapor-3.3.5/pywapor/post_et_look.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7139 2023-05-17 07:54:32.000000 pywapor-3.3.5/pywapor/pre_et_look.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7008 2023-05-17 07:54:37.000000 pywapor-3.3.5/pywapor/pre_se_root.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11959 2023-05-17 09:02:39.000000 pywapor-3.3.5/pywapor/se_root.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-05-17 15:15:42.526253 pywapor-3.3.5/pywapor.egg-info/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      457 2023-05-17 15:15:42.000000 pywapor-3.3.5/pywapor.egg-info/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2988 2023-05-17 15:15:42.000000 pywapor-3.3.5/pywapor.egg-info/SOURCES.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2023-05-17 15:15:42.000000 pywapor-3.3.5/pywapor.egg-info/dependency_links.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      286 2023-05-17 15:15:42.000000 pywapor-3.3.5/pywapor.egg-info/requires.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2023-05-17 15:15:42.000000 pywapor-3.3.5/pywapor.egg-info/top_level.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2023-05-17 15:15:42.559530 pywapor-3.3.5/setup.cfg
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2200 2023-05-17 14:47:23.000000 pywapor-3.3.5/setup.py
```

### Comparing `pywapor-3.3.4/LICENSE` & `pywapor-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/README.md` & `pywapor-3.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This repository contains a Python implementation of the algorithm used to generate the [WaPOR](http://www.fao.org/in-action/remote-sensing-for-water-productivity/en/) [datasets](https://wapor.apps.fao.org/home/WAPOR_2/1). It can be used to calculate evaporation, transpiration and biomass production maps.
 
 ### Installation
 
 Its recommended to install in a clean [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/environments.html) and use [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/) to install all the important packages from the `conda-forge` channel.
 
 ```bash
-conda create -n my_pywapor_env --yes -c conda-forge python pip gdal pydap numpy pandas requests matplotlib pyproj scipy pycurl pyshp joblib bs4 rasterio xarray bottleneck geojson tqdm dask rioxarray pyvis shapely lxml cachetools cdsapi sentinelsat geopy numba scikit-learn beautifulsoup4 libnetcdf=4.8
+conda create -n my_pywapor_env --yes -c conda-forge python pip gdal pydap numpy "pandas<2.0.0" requests matplotlib pyproj scipy pycurl pyshp joblib bs4 rasterio xarray bottleneck geojson tqdm dask rioxarray pyvis shapely lxml cachetools cdsapi sentinelsat geopy numba scikit-learn beautifulsoup4 "libnetcdf=4.8"
 
 conda activate my_pywapor_env
 ```
 
 Then use the package manager [pip](https://pip.pypa.io/en/stable/) to install pywapor.
 
 ```bash
```

#### html2text {}

```diff
@@ -7,30 +7,30 @@
 sensing-for-water-productivity/en/) [datasets](https://wapor.apps.fao.org/home/
 WAPOR_2/1). It can be used to calculate evaporation, transpiration and biomass
 production maps. ### Installation Its recommended to install in a clean [conda
 environment](https://docs.conda.io/projects/conda/en/latest/user-guide/
 concepts/environments.html) and use [conda](https://docs.conda.io/projects/
 conda/en/latest/user-guide/install/) to install all the important packages from
 the `conda-forge` channel. ```bash conda create -n my_pywapor_env --yes -
-c conda-forge python pip gdal pydap numpy pandas requests matplotlib pyproj
-scipy pycurl pyshp joblib bs4 rasterio xarray bottleneck geojson tqdm dask
-rioxarray pyvis shapely lxml cachetools cdsapi sentinelsat geopy numba scikit-
-learn beautifulsoup4 libnetcdf=4.8 conda activate my_pywapor_env ``` Then use
-the package manager [pip](https://pip.pypa.io/en/stable/) to install pywapor.
-```bash pip install pywapor ``` ### Usage To run the model for one dekad (from
-2021-07-01 to 2021-07-11 in this case) for the Fayoum irrigation scheme in
-Egypt (but feel free to change the [boundingbox](http://bboxfinder.com) defined
-by `latlim` and `lonlim`) using mainly MODIS data, run the following code (run
-`python` in your console to activate Python and `exit()` to deactivate).
-```python import pywapor # User inputs. timelim = ["2021-07-01", "2021-07-11"]
-latlim = [28.9, 29.7] lonlim = [30.2, 31.2] project_folder = r"/
-my_first_ETLook_run/" # Download and prepare input data. ds_in =
-pywapor.pre_et_look.main(project_folder, latlim, lonlim, timelim) # Run the
-model. ds_out = pywapor.et_look.main(ds_in) ``` Check out the documentation and
-the notebooks below to learn more! ### Documentation Go [here](https://
+c conda-forge python pip gdal pydap numpy "pandas<2.0.0" requests matplotlib
+pyproj scipy pycurl pyshp joblib bs4 rasterio xarray bottleneck geojson tqdm
+dask rioxarray pyvis shapely lxml cachetools cdsapi sentinelsat geopy numba
+scikit-learn beautifulsoup4 "libnetcdf=4.8" conda activate my_pywapor_env ```
+Then use the package manager [pip](https://pip.pypa.io/en/stable/) to install
+pywapor. ```bash pip install pywapor ``` ### Usage To run the model for one
+dekad (from 2021-07-01 to 2021-07-11 in this case) for the Fayoum irrigation
+scheme in Egypt (but feel free to change the [boundingbox](http://
+bboxfinder.com) defined by `latlim` and `lonlim`) using mainly MODIS data, run
+the following code (run `python` in your console to activate Python and `exit
+()` to deactivate). ```python import pywapor # User inputs. timelim = ["2021-
+07-01", "2021-07-11"] latlim = [28.9, 29.7] lonlim = [30.2, 31.2]
+project_folder = r"/my_first_ETLook_run/" # Download and prepare input data.
+ds_in = pywapor.pre_et_look.main(project_folder, latlim, lonlim, timelim) # Run
+the model. ds_out = pywapor.et_look.main(ds_in) ``` Check out the documentation
+and the notebooks below to learn more! ### Documentation Go [here](https://
 www.fao.org/aquastat/py-wapor/) for the full pyWaPOR documentation. ####
 Notebooks
    Name              Colab
 1. Introduction      [colab]
 2. Levels            [colab]
 3. Composites        [colab]
 4. Enhancers         [colab]
```

### Comparing `pywapor-3.3.4/pywapor/collect/accounts.py` & `pywapor-3.3.5/pywapor/collect/accounts.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/downloader.py` & `pywapor-3.3.5/pywapor/collect/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,29 +88,29 @@
             try:
                 x = dler(**args)
                 attempts[(source, product_name)] += max_attempts * 10
             except Exception as e:
 
                 exception_args = getattr(e, "args", [""])
 
-                give_warnings = True
+                give_warning_only = False
 
                 if len(exception_args) > 0:
                     if "NetCDF: Filter error: unimplemented filter encountered" in str(exception_args[0]):
                         info_url = r"https://github.com/Unidata/netcdf4-python/issues/1182"
                         log.warning(f"--> Looks like you installed `netcdf4` incorrectly, see {info_url} for more info.")
 
                 if len(exception_args) > 0:
                     if "Waiting for order of" in str(exception_args[0]):
-                        give_warnings = False
+                        give_warning_only = True
                         log.info(f"--> Continuing with collection of other sources while waiting for {exception_args[1]} `{source_name}.{product_name}` scenes to finish processing.")
                         if landsat_order_only:
                             attempts[(source, product_name)] += max_attempts * 10
 
-                if attempts[(source, product_name)] < max_attempts - 1 and give_warnings:
+                if (attempts[(source, product_name)] < (max_attempts - 1)) and give_warning_only:
                     log.warning(f"--> Collect attempt {attempts[(source, product_name)] + 1} of {max_attempts} for `{source_name}.{product_name}` failed, trying again after other sources have been collected. ({type(e).__name__}: {e}).")
                 else:
                     log.warning(f"--> Collect attempt {attempts[(source, product_name)] + 1} of {max_attempts} for `{source_name}.{product_name}` failed, giving up now, see full traceback below for more info. ({type(e).__name__}: {e}).")
                     log.exception("")
 
                 attempts[(source, product_name)] += 1
```

### Comparing `pywapor-3.3.4/pywapor/collect/product/CHIRPS.py` & `pywapor-3.3.5/pywapor/collect/product/CHIRPS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/COPERNICUS.py` & `pywapor-3.3.5/pywapor/collect/product/COPERNICUS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/ERA5.py` & `pywapor-3.3.5/pywapor/collect/product/ERA5.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/GEOS5.py` & `pywapor-3.3.5/pywapor/collect/product/GEOS5.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/GLO30.txt` & `pywapor-3.3.5/pywapor/collect/product/GLO30.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/GLO90.txt` & `pywapor-3.3.5/pywapor/collect/product/GLO90.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/GLOBCOVER.py` & `pywapor-3.3.5/pywapor/collect/product/GLOBCOVER.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/LANDSAT.py` & `pywapor-3.3.5/pywapor/collect/product/LANDSAT.py`

 * *Files 9% similar despite different names*

```diff
@@ -312,79 +312,79 @@
     
     return out
 
 def default_post_processors(product_name, req_vars):
 
     post_processors = {
         "LT05_SR": {
-            'coastal': [],
-            'blue': [],
-            'green': [],
-            'red': [],
-            'nir': [],
-            'swir1': [],
-            'swir2': [],
+            'coastal': [gap_fill],
+            'blue': [gap_fill],
+            'green': [gap_fill],
+            'red': [gap_fill],
+            'nir': [gap_fill],
+            'swir1': [gap_fill],
+            'swir2': [gap_fill],
             'pixel_qa': [],
             'radsat_qa': [],
-            'ndvi': [calc_normalized_difference],
-            'r0': [partial(calc_r0, product_name = "LT05_SR")],
+            'ndvi': [calc_normalized_difference, gap_fill],
+            'r0': [partial(calc_r0, product_name = "LT05_SR"), gap_fill],
             },
         "LT05_ST": {
-            'lst': [mask_uncertainty],
+            'lst': [mask_uncertainty, gap_fill],
             'lst_qa': [],
         },
         "LE07_SR": {
-            'coastal': [],
-            'blue': [],
-            'green': [],
-            'red': [],
-            'nir': [],
-            'swir1': [],
-            'swir2': [],
+            'coastal': [gap_fill],
+            'blue': [gap_fill],
+            'green': [gap_fill],
+            'red': [gap_fill],
+            'nir': [gap_fill],
+            'swir1': [gap_fill],
+            'swir2': [gap_fill],
             'pixel_qa': [],
             'radsat_qa': [],
-            'ndvi': [calc_normalized_difference],
-            'r0': [partial(calc_r0, product_name = "LE07_SR")],
+            'ndvi': [calc_normalized_difference, gap_fill],
+            'r0': [partial(calc_r0, product_name = "LE07_SR"), gap_fill],
             },
         "LE07_ST": {
-            'lst': [mask_uncertainty, ],
+            'lst': [mask_uncertainty, gap_fill],
             'lst_qa': [],
         },
         "LC08_SR": {
-            'coastal': [],
-            'blue': [],
-            'green': [],
-            'red': [],
-            'nir': [],
-            'swir1': [],
-            'swir2': [],
+            'coastal': [gap_fill],
+            'blue': [gap_fill],
+            'green': [gap_fill],
+            'red': [gap_fill],
+            'nir': [gap_fill],
+            'swir1': [gap_fill],
+            'swir2': [gap_fill],
             'pixel_qa': [],
             'radsat_qa': [],
-            'ndvi': [calc_normalized_difference],
-            'r0': [partial(calc_r0, product_name = "LC08_SR")],
+            'ndvi': [calc_normalized_difference, gap_fill],
+            'r0': [partial(calc_r0, product_name = "LC08_SR"), gap_fill],
             },
         "LC08_ST": {
-            'lst': [mask_uncertainty],
+            'lst': [mask_uncertainty, gap_fill],
             'lst_qa': [],
         },
         "LC09_SR": {
-            'coastal': [],
-            'blue': [],
-            'green': [],
-            'red': [],
-            'nir': [],
-            'swir1': [],
-            'swir2': [],
+            'coastal': [gap_fill],
+            'blue': [gap_fill],
+            'green': [gap_fill],
+            'red': [gap_fill],
+            'nir': [gap_fill],
+            'swir1': [gap_fill],
+            'swir2': [gap_fill],
             'pixel_qa': [],
             'radsat_qa': [],
-            'ndvi': [calc_normalized_difference],
-            'r0': [partial(calc_r0, product_name = "LC09_SR")],
+            'ndvi': [calc_normalized_difference, gap_fill],
+            'r0': [partial(calc_r0, product_name = "LC09_SR"), gap_fill],
             },
         "LC09_ST": {
-            'lst': [mask_uncertainty],
+            'lst': [mask_uncertainty, gap_fill],
             'lst_qa': [],
         }
     }
 
     out = {k:v for k,v in post_processors[product_name].items() if k in req_vars}
 
     return out
```

### Comparing `pywapor-3.3.4/pywapor/collect/product/Landsat/C2L2SP.py` & `pywapor-3.3.5/pywapor/collect/product/Landsat/C2L2SP.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/MERRA2.py` & `pywapor-3.3.5/pywapor/collect/product/MERRA2.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/MODIS.py` & `pywapor-3.3.5/pywapor/collect/product/MODIS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/MODIS_tiles.geojson` & `pywapor-3.3.5/pywapor/collect/product/MODIS_tiles.geojson`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/PROBAV.py` & `pywapor-3.3.5/pywapor/collect/product/PROBAV.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/SENTINEL2.py` & `pywapor-3.3.5/pywapor/collect/product/SENTINEL2.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import xarray as xr
 import numpy as np
 from datetime import datetime as dt
 from pywapor.general.logger import log, adjust_logger
 import pywapor.collect.protocol.sentinelapi as sentinelapi
 import numpy as np
 from functools import partial
+from pywapor.enhancers.gap_fill import gap_fill
 from pywapor.general.processing_functions import open_ds, remove_ds, save_ds
 from lxml import etree
 import copy
+import warnings
 
 def apply_qa(ds, var):
     """Mask SENTINEL2 data using a qa variable.
 
     Parameters
     ----------
     ds : xr.Dataset
@@ -95,15 +97,17 @@
 
     Returns
     -------
     xr.Dataset
         Output data.
     """
     if np.all([x in ds.data_vars for x in bands]):
-        da = (ds[bands[0]] - ds[bands[1]]) / (ds[bands[0]] + ds[bands[1]])
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="All-NaN slice encountered")
+            da = (ds[bands[0]] - ds[bands[1]]) / (ds[bands[0]] + ds[bands[1]])
         ds[var] = da.clip(-1, 1)
     else:
         log.warning(f"--> Couldn't calculate `{var}`, `{'` and `'.join([x for x in bands if x not in ds.data_vars])}` is missing.")
     return ds
 
 def calc_psri(ds, var):
     """Calculate the PSRI as ("red" - "blue)/"red_edge_740".
@@ -118,15 +122,17 @@
     Returns
     -------
     xr.Dataset
         Output data.
     """
     reqs = ["red", "blue", "red_edge_740"]
     if np.all([x in ds.data_vars for x in reqs]):
-        da = (ds["red"] - ds["blue"]) / ds["red_edge_740"]
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="All-NaN slice encountered")
+            da = (ds["red"] - ds["blue"]) / ds["red_edge_740"]
         ds[var] = da.clip(-1, 1)
     else:
         log.warning(f"--> Couldn't calculate `{var}`, `{'` and `'.join([x for x in reqs if x not in ds.data_vars])}` is missing.")
     return ds
 
 def calc_nmdi(ds, var):
     """Calculate the NMDI.
@@ -190,17 +196,19 @@
     Returns
     -------
     xr.Dataset
         Output data.
     """
     reqs = ["red_edge_740", "blue", "red"]
     if np.all([x in ds.data_vars for x in reqs]):
-        n1 = ds["red_edge_740"] - 1.7 * ds["red"] + 0.7 * ds["blue"]
-        n2 = ds["red_edge_740"] + 2.3 * ds["red"] - 1.3 * ds["blue"]
-        da = n1 / n2
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="All-NaN slice encountered")
+            n1 = ds["red_edge_740"] - 1.7 * ds["red"] + 0.7 * ds["blue"]
+            n2 = ds["red_edge_740"] + 2.3 * ds["red"] - 1.3 * ds["blue"]
+            da = n1 / n2
         ds[var] = da.clip(-1, 1)
     else:
         log.warning(f"--> Couldn't calculate `{var}`, `{'` and `'.join([x for x in reqs if x not in ds.data_vars])}` is missing.")
     return ds
 
 def calc_r0(ds, var):
     """Calculate the Albedo.
@@ -224,18 +232,20 @@
         "red":      0.334,
         "nir":      0.371,
         "offset":   0.018,
     }
     
     reqs = ["blue", "green", "red", "nir"]
     if np.all([x in ds.data_vars for x in reqs]):
-        ds["offset"] = xr.ones_like(ds["blue"])
-        weights_da = xr.DataArray(data = list(weights.values()), 
-                                coords = {"band": list(weights.keys())})
-        ds["r0"] = ds[reqs + ["offset"]].to_array("band").weighted(weights_da).sum("band", skipna = False)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="All-NaN slice encountered")
+            ds["offset"] = xr.ones_like(ds["blue"])
+            weights_da = xr.DataArray(data = list(weights.values()), 
+                                    coords = {"band": list(weights.keys())})
+            ds["r0"] = ds[reqs + ["offset"]].to_array("band").weighted(weights_da).sum("band", skipna = False)
     else:
         log.warning(f"--> Couldn't calculate `{var}`, `{'` and `'.join([x for x in reqs if x not in ds.data_vars])}` is missing.")
     return ds
 
 def default_vars(product_name, req_vars):
     """Given a `product_name` and a list of requested variables, returns a dictionary
     with metadata on which exact layers need to be requested from the server, how they should
@@ -350,53 +360,53 @@
     -------
     dict
         Functions per variable that should be applied to the variable.
     """
     
     post_processors = {
         "S2MSI2A_R20m": {
-            "coastal_aerosol":  [],
-            "blue":             [],
-            "green":            [],
-            "red":              [],
-            "red_edge_703":     [],
-            "red_edge_740":     [],
-            "red_edge_782":     [],
-            "nir":              [],
+            "coastal_aerosol":  [gap_fill],
+            "blue":             [gap_fill],
+            "green":            [gap_fill],
+            "red":              [gap_fill],
+            "red_edge_703":     [gap_fill],
+            "red_edge_740":     [gap_fill],
+            "red_edge_782":     [gap_fill],
+            "nir":              [gap_fill],
             "qa":               [],
-            "swir1":            [],
-            "swir2":            [],
+            "swir1":            [gap_fill],
+            "swir2":            [gap_fill],
             "psri":             [calc_psri],
-            "ndvi":             [calc_normalized_difference],
-            "nmdi":             [calc_nmdi],
-            "vari_red_edge":    [calc_vari_red_egde],
-            "bsi":              [calc_bsi],
-            "mndwi":            [partial(calc_normalized_difference, bands = ["swir1", "green"])],
-            "r0":               [calc_r0],
+            "ndvi":             [calc_normalized_difference, gap_fill],
+            "nmdi":             [calc_nmdi, gap_fill],
+            "vari_red_edge":    [calc_vari_red_egde, gap_fill],
+            "bsi":              [calc_bsi, gap_fill],
+            "mndwi":            [partial(calc_normalized_difference, bands = ["swir1", "green"]), gap_fill],
+            "r0":               [calc_r0, gap_fill],
             },
 
         "S2MSI2A_R60m": {
-            "coastal_aerosol":  [],
-            "blue":             [],
-            "green":            [],
-            "red":              [],
-            "red_edge_703":     [],
-            "red_edge_740":     [],
-            "red_edge_782":     [],
-            "nir":              [],
+            "coastal_aerosol":  [gap_fill],
+            "blue":             [gap_fill],
+            "green":            [gap_fill],
+            "red":              [gap_fill],
+            "red_edge_703":     [gap_fill],
+            "red_edge_740":     [gap_fill],
+            "red_edge_782":     [gap_fill],
+            "nir":              [gap_fill],
             "qa":               [],
-            "swir1":            [],
-            "swir2":            [],
-            "psri":             [calc_psri],
-            "ndvi":             [calc_normalized_difference],
-            "nmdi":             [calc_nmdi],
-            "vari_red_edge":    [calc_vari_red_egde],
-            "bsi":              [calc_bsi],
-            "mndwi":            [partial(calc_normalized_difference, bands = ["swir1", "green"])],
-            "r0":               [calc_r0],
+            "swir1":            [gap_fill],
+            "swir2":            [gap_fill],
+            "psri":             [calc_psri, gap_fill],
+            "ndvi":             [calc_normalized_difference, gap_fill],
+            "nmdi":             [calc_nmdi, gap_fill],
+            "vari_red_edge":    [calc_vari_red_egde, gap_fill],
+            "bsi":              [calc_bsi, gap_fill],
+            "mndwi":            [partial(calc_normalized_difference, bands = ["swir1", "green"]), gap_fill],
+            "r0":               [calc_r0, gap_fill],
             },
     }
 
     out = {k:v for k,v in post_processors[product_name].items() if k in req_vars}
 
     return out
```

### Comparing `pywapor-3.3.4/pywapor/collect/product/SENTINEL3.py` & `pywapor-3.3.5/pywapor/collect/product/SENTINEL3.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     Returns
     -------
     xr.Dataset
         Downloaded data.
     """
     product_folder = os.path.join(folder, "SENTINEL3")
 
-    fn = os.path.join(folder, f"{product_name}.nc")
+    fn = os.path.join(product_folder, f"{product_name}.nc")
     req_vars_orig = copy.deepcopy(req_vars)
     if os.path.isfile(fn):
         existing_ds = open_ds(fn)
         req_vars_new = list(set(req_vars).difference(set(existing_ds.data_vars)))
         if len(req_vars_new) > 0:
             req_vars = req_vars_new
             existing_ds = existing_ds.close()
```

### Comparing `pywapor-3.3.4/pywapor/collect/product/SRTM.py` & `pywapor-3.3.5/pywapor/collect/product/SRTM.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/SRTM30_tiles.geojson` & `pywapor-3.3.5/pywapor/collect/product/SRTM30_tiles.geojson`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/STATICS.py` & `pywapor-3.3.5/pywapor/collect/product/STATICS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/product/VIIRSL1.py` & `pywapor-3.3.5/pywapor/collect/product/VIIRSL1.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/protocol/cds.py` & `pywapor-3.3.5/pywapor/collect/protocol/cds.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/protocol/cog.py` & `pywapor-3.3.5/pywapor/collect/protocol/cog.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/protocol/crawler.py` & `pywapor-3.3.5/pywapor/collect/protocol/crawler.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/protocol/opendap.py` & `pywapor-3.3.5/pywapor/collect/protocol/opendap.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     url = base_url + urllib.parse.quote(",".join(dims + varis))
     return url
 
 def start_session(base_url, selection, un_pw = [None, None]):
     if un_pw == [None, None]:
         warnings.filterwarnings("ignore", "password was not set. ")
     url_coords = base_url + urllib.parse.quote(",".join(selection.keys()))
-    session = setup_session(*un_pw, check_url = url_coords, verify = False)
+    session = setup_session(*un_pw, check_url = url_coords, verify = True)
     return session
 
 def download_xarray(url, fp, coords, variables, post_processors, 
                     data_source_crs = None, timedelta = None):
     """Download a OPENDaP dataset using xarray directly.
 
     Parameters
```

### Comparing `pywapor-3.3.4/pywapor/collect/protocol/projections.py` & `pywapor-3.3.5/pywapor/collect/protocol/projections.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/collect/protocol/sentinelapi.py` & `pywapor-3.3.5/pywapor/collect/protocol/sentinelapi.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/apply_enhancers.py` & `pywapor-3.3.5/pywapor/enhancers/apply_enhancers.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/dem.py` & `pywapor-3.3.5/pywapor/enhancers/dem.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/dms/pyDMS.py` & `pywapor-3.3.5/pywapor/enhancers/dms/pyDMS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/dms/pyDMS_utils.py` & `pywapor-3.3.5/pywapor/enhancers/dms/pyDMS_utils.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/dms/thermal_sharpener.py` & `pywapor-3.3.5/pywapor/enhancers/dms/thermal_sharpener.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     err=GdalErrorHandler()
     handler=err.handler
     gdal.PushErrorHandler(handler)
     gdal.UseExceptions()
 
 gdal_stop_warnings_and_raise_errors()
 
-def highres_inputs(workdir, temporal_hr_input_data, static_hr_input_data):
+def highres_inputs(workdir, temporal_hr_input_data, static_hr_input_data, filter_times = None):
     """Create VRT files with all highres inputs per datetime.
 
     Parameters
     ----------
     workdir : str
         Folder in which to store the VRT files.
     temporal_hr_input_data : list
@@ -71,14 +71,16 @@
         os.remove(output_vrt)
     ds = gdal.BuildVRT(output_vrt, temporal_hr_input_data + static_hr_input_data, options = buildvrt_options)
     ds.FlushCache()
     ds = None
 
     ds = xr.open_dataset(re.findall(r"NETCDF:(.*):.*", temporal_hr_input_data[0])[0])
     times = [x.strftime("%Y%m%d_%H%M%S") for x in pd.to_datetime(ds.time.values)]
+    if not isinstance(filter_times, type(None)):
+        times = [x for x in times if x in filter_times]
     ds = ds.close()
 
     with open(output_vrt, 'r') as f:
         data = f.read()
 
     fps = list()
     for time_index, dt in enumerate(times):
@@ -222,32 +224,34 @@
         Keys are variable names, values are (sharpened) datasets.
     """
     # Open unopened netcdf files.
     dss = {**{k: open_ds(v) for k, v in dss.items() if isinstance(v, str)}, 
             **{k:v for k,v in dss.items() if not isinstance(v, str)}}
 
     if 'cos_solar_zangle' in vars_for_sharpening and not 'cos_solar_zangle' in dss.keys():
-        dss = get_cos_solar_zangle(dss, "bt", folder)
+        dss = get_cos_solar_zangle(dss, var, folder)
         remove_cos_solar_zangle = True
     else:
         remove_cos_solar_zangle = False
 
     out_fns = list()
 
     workdir = os.path.join(folder, "DMS")
 
     temporal_lr_input_data = f"NETCDF:{dss[var].encoding['source']}:{var}"
     temporal_hr_input_data = [f"NETCDF:{y.encoding['source']}:{x}" for x, y in dss.items() if "time" in y.dims and x in vars_for_sharpening]
     static_hr_input_data = [f"NETCDF:{y.encoding['source']}:{x}" for x, y in dss.items() if "time" not in y.dims and x in vars_for_sharpening]
 
-    highResFiles = sorted(highres_inputs(workdir, temporal_hr_input_data, static_hr_input_data))
     lowResFiles = sorted(lowres_inputs(workdir, temporal_lr_input_data))
+    lowResDates = [os.path.split(x)[-1].split("_")[-2:] for x in lowResFiles]
+    filter_times = [os.path.split(x)[-1].replace(".vrt", "").replace("lowres_input_", "") for x in lowResFiles]
 
+    highResFiles = sorted(highres_inputs(workdir, temporal_hr_input_data, static_hr_input_data, filter_times = filter_times))
     highResDates = [os.path.split(x)[-1].split("_")[-2:] for x in highResFiles]
-    lowResDates = [os.path.split(x)[-1].split("_")[-2:] for x in lowResFiles]
+    
     assert np.all([x == y for x,y in zip(highResDates, lowResDates)])
 
     missing_vars = [x for x in vars_for_sharpening if x not in dss.keys()]
     if len(missing_vars) > 0:
         log.info(f"--> Sharpening {len(highResFiles)} `{var}` images, without `{'` and `'.join(missing_vars)}` features.").add()
     else:
         log.info(f"--> Sharpening {len(highResFiles)} `{var}` images.").add()
@@ -295,18 +299,15 @@
     dss[var] = fp
 
     for x in dss_:
         remove_ds(x)
     
     if 'cos_solar_zangle' in dss.keys() and remove_cos_solar_zangle:
         remove_ds(dss['cos_solar_zangle'])
-
-    for x in vars_for_sharpening:
-        if x in dss.keys():
-            _ = dss.pop(x)
+        _ = dss.pop("cos_solar_zangle")
 
     return dss
 
 @performance_check
 def thermal_sharpen(highres_fn, lowres_fn):
     """Sharpen a single lowres file using a single highres file (in which each band contains one feature).
```

### Comparing `pywapor-3.3.4/pywapor/enhancers/gap_fill.py` & `pywapor-3.3.5/pywapor/enhancers/gap_fill.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/lulc.py` & `pywapor-3.3.5/pywapor/enhancers/lulc.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/other.py` & `pywapor-3.3.5/pywapor/enhancers/other.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/smooth/archive.py` & `pywapor-3.3.5/pywapor/enhancers/smooth/archive.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/smooth/core.py` & `pywapor-3.3.5/pywapor/enhancers/smooth/core.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/smooth/plotters.py` & `pywapor-3.3.5/pywapor/enhancers/smooth/plotters.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/smooth/whittaker.py` & `pywapor-3.3.5/pywapor/enhancers/smooth/whittaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,20 +277,22 @@
         ds = save_ds(ds, out_fh, encoding = "initiate", label = f"Applying whittaker smoothing ({var}).")
 
     # Give warnings if data is outside of defined range.
     if not np.isinf(valid_drange[0]):
         min_bound = float(ds[f"{var}_smoothed"].min().values)
         if min_bound < valid_drange[0]:
             log.warning(f"--> Minimum of `{var}_smoothed` is smaller than `valid_drange` min ({min_bound:.2f} < {valid_drange[0]}).")
+            ds[f"{var}_smoothed"] = ds[f"{var}_smoothed"].clip(valid_drange[0], np.inf)
 
     if not np.isinf(valid_drange[1]):
         max_bound = float(ds[f"{var}_smoothed"].max().values)
         if max_bound > valid_drange[1]:
             log.warning(f"--> Maximum of `{var}_smoothed` is larger than `valid_drange` max ({max_bound:.2f} > {valid_drange[1]}).")
-
+            ds[f"{var}_smoothed"] = ds[f"{var}_smoothed"].clip(-np.inf, valid_drange[1])
+            
     return ds
 
 if __name__ == "__main__":
 
     import matplotlib.pyplot as plt
 
     ds = open_ds(r"/Users/hmcoerver/Local/poster_whit_data/consolidated_data.nc")
```

### Comparing `pywapor-3.3.4/pywapor/enhancers/temperature.py` & `pywapor-3.3.5/pywapor/enhancers/temperature.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/enhancers/wind.py` & `pywapor-3.3.5/pywapor/enhancers/wind.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/et_look.py` & `pywapor-3.3.5/pywapor/et_look.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 # -*- coding: utf-8 -*-
 """
 Code to run the ETLook model.
 """
 import os
-import numpy as np
-import pywapor.et_look_dev as ETLook_dev
 import pywapor.et_look_v2_v3 as ETLook_v2_v3
 import pywapor.general as g
 import datetime
 from pywapor.general.logger import log, adjust_logger
-import pywapor.general.processing_functions as PF
-import xarray as xr
-import pandas as pd
 from pywapor.general.processing_functions import save_ds, open_ds
-# from pywapor.general.compositer import calculate_ds
 import copy
 import warnings
 
 def main(input_data, et_look_version = "v2", export_vars = "default", chunks = {"time_bins": 1, "x": 1000, "y": 1000}):
     """Runs the ETLook model over the provided input data.
 
     Parameters
     ----------
     input_data : str | xr.Dataset
         Dataset generated by `pywapor.pre_et_look`.
-    et_look_version : "v2" | "v3" | "dev", optional
+    et_look_version : "v2" | "v3", optional
         Which version of the ETLook model to use, by default "v2".
     export_vars : "default" | "all" | list, optional
         Specify which variables to save inside the output file. `"Default"` stores `int_mm`,
         `t_24_mm`, `e_24_mm`, `et_24_mm`, `et_ref_24_mm`, `se_root`, `biomass_prod`,
         `epoch_ends` and `epoch_starts`. `"all"` stores all calculated variables. Use a
         list to specify a custom output set, by default "default".
     chunks : dict, optional
@@ -51,31 +45,24 @@
 
     _ = adjust_logger(True, os.path.split(input_data)[0], "INFO")
 
     t1 = datetime.datetime.now()
     log.info("> ET_LOOK").add()
 
     # Version
-    if et_look_version == "v2" or et_look_version == "v3":
-        ETLook = ETLook_v2_v3
-    elif et_look_version == "dev":
-        ETLook = ETLook_dev
+    ETLook = ETLook_v2_v3
 
     log.info(f"--> Running `et_look` ({et_look_version}).")
 
     # Allow skipping of et_look-functions if not all of its required inputs are
     # available.
     g.lazifier.decorate_submods(ETLook, g.lazifier.etlook_decorator)
 
     ds = g.variables.initiate_ds(ds)
 
-    if et_look_version == "dev":
-        ds["nd_min"] = 0.1
-        ds["tenacity"] = 1.0
-
     if ds["rs_min"].dtype == object:
         ds["rs_min"] = 100
         log.info(f"--> Setting `rs_min` to `100`.")
 
     if ds["land_mask"].dtype == object:
         ds["land_mask"] = 1
         log.info(f"--> Setting `land_mask` to `1`.")
@@ -113,50 +100,34 @@
     if ds["vp_24"].dtype == object:
         ds["vp_24"] = ETLook.meteo.vapour_pressure_from_specific_humidity_daily(ds["qv_24"], ds["p_air_24"])
     if ds["vp_24"].dtype == object:
         ds["vp_24"] = ETLook.meteo.vapour_pressure_from_dewpoint_daily(ds["t_dew_24"])
 
     if et_look_version == "v2":
         ds["svp_24"] = ETLook.meteo.saturated_vapour_pressure(ds["t_air_24"])
-    elif et_look_version == "v3" or et_look_version == "dev":
+    else:
         ds["svp_24_min"] = ETLook.meteo.saturated_vapour_pressure_minimum(ds["t_air_min_24"])
         ds["svp_24_max"] = ETLook.meteo.saturated_vapour_pressure_maximum(ds["t_air_max_24"])
         ds["svp_24"] = ETLook.meteo.saturated_vapour_pressure_average(ds["svp_24_max"], ds["svp_24_min"])
 
     ds["vpd_24"] = ETLook.meteo.vapour_pressure_deficit_daily(ds["svp_24"], ds["vp_24"])
     ds["stress_vpd"] = ETLook.stress.stress_vpd(ds["vpd_24"], ds["vpd_slope"])
     ds["stress_temp"] = ETLook.stress.stress_temperature(ds["t_air_24"], t_opt = ds["t_opt"], t_min = ds["t_min"], t_max = ds["t_max"])
 
-    if et_look_version == "dev":
-        if isinstance(ds["land_mask"], xr.DataArray):
-            ds["rs_min"] = xr.where(ds["land_mask"] == 3, 400, 100)
-        else:
-            ds["rs_min"] = np.where(ds["land_mask"] == 3, 400, 100)
-
     ds["r_canopy_0"] = ETLook.resistance.atmospheric_canopy_resistance(ds["lai_eff"], ds["stress_rad"], ds["stress_vpd"], ds["stress_temp"], rs_min = ds["rs_min"], rcan_max = ds["rcan_max"])
 
     # **net radiation canopy******************************************************
     ds["t_air_k_24"] = ETLook.meteo.air_temperature_kelvin_daily(ds["t_air_24"])
     ds["l_net"] = ETLook.radiation.longwave_radiation_fao(ds["t_air_k_24"], ds["vp_24"], ds["trans_24"], vp_slope = ds["vp_slope"], vp_offset = ds["vp_offset"], lw_slope = ds["lw_slope"], lw_offset = ds["lw_offset"])
     ds["int_mm"] = ETLook.evapotranspiration.interception_mm(ds["p_24"], ds["vc"], ds["lai"], int_max = ds["int_max"])
     ds["lh_24"] = ETLook.meteo.latent_heat_daily(ds["t_air_24"])
     ds["int_wm2"] = ETLook.radiation.interception_wm2(ds["int_mm"], ds["lh_24"])
     ds["rn_24"] = ETLook.radiation.net_radiation(ds["r0"], ds["ra_24"], ds["l_net"], ds["int_wm2"])
     ds["rn_24_canopy"] = ETLook.radiation.net_radiation_canopy(ds["rn_24"], ds["sf_soil"])
 
-    # find water region using ndvi
-    if et_look_version == "dev":
-        if ds.pixel_size < 250:
-            if isinstance(ds["land_mask"], xr.DataArray):
-                ds["land_mask"] = xr.where(ds["land_mask"] == 2, 1, ds["land_mask"])
-                ds["land_mask"] = xr.where(ds["ndvi"] < 0, 2, ds["land_mask"])
-            else:
-                ds["land_mask"] = np.where(ds["land_mask"] == 2, 1, ds["land_mask"])
-                ds["land_mask"] = np.where(ds["ndvi"] < 0, 2, ds["land_mask"])
-
     ds["stress_moist"] = ETLook.stress.stress_moisture(ds["se_root"], tenacity = ds["tenacity"])
     ds["r_canopy"] = ETLook.resistance.canopy_resistance(ds["r_canopy_0"], ds["stress_moist"], rcan_max = ds["rcan_max"])
 
     # **initial canopy aerodynamic resistance***********************************************************
     if ds["z_oro"].dtype == object: # TODO this function is wrong...
         ds["z_oro"] = 0.001
         log.info(f"--> Setting `z_oro` to `0.001`.")
@@ -186,19 +157,14 @@
     ds["disp"] = ETLook.roughness.displacement_height(ds["lai"], ds["z_obst"], land_mask = ds["land_mask"], c1 = ds["c1"])
     ds["u_star_24_init"] = ETLook.unstable.initial_friction_velocity_daily(ds["u_b_24"], ds["z0m"], ds["disp"], z_b = ds["z_b"])
 
     # **ETLook.unstable.transpiration***********************************************************
     ds["t_24"] = ETLook.unstable.transpiration(ds["rn_24_canopy"], ds["ssvp_24"], ds["ad_24"], ds["vpd_24"], ds["psy_24"], ds["r_canopy"], ds["h_canopy_24_init"], ds["t_air_k_24"], ds["u_star_24_init"], ds["z0m"], ds["disp"], ds["u_b_24"], z_obs = ds["z_obs"], z_b = ds["z_b"], iter_h = ds["iter_h"])
     ds["t_24_mm"] = ETLook.unstable.transpiration_mm(ds["t_24"], ds["lh_24"])
 
-    if et_look_version == "dev":
-        ds["r_canopy_unstressed"] = ETLook.resistance.unstressed_canopy_resistance(ds["r_canopy"], ds["stress_moist"])
-        ds["tpot_24"] = ETLook.unstable.transpiration(ds["rn_24_canopy"], ds["ssvp_24"], ds["ad_24"], ds["vpd_24"], ds["psy_24"], ds["r_canopy_unstressed"], ds["h_canopy_24_init"], ds["t_air_k_24"], ds["u_star_24_init"], ds["z0m"], ds["disp"], ds["u_b_24"], z_obs = ds["z_obs"], z_b = ds["z_b"], iter_h = ds["iter_h"])
-        ds["tpot_24_mm"] = ETLook.unstable.transpiration_mm(ds["tpot_24"], ds["lh_24"])
-
     #*******EVAPORATION COMPONENT****************************************************************
 
     # **ETLook.radiation.net_radiation_soil***********************************************************
     ds["rn_24_soil"] = ETLook.radiation.net_radiation_soil(ds["rn_24"], ds["sf_soil"])
 
     # **ETLook.resistance.soil_resistance***********************************************************
     ds["r_soil"] = ETLook.resistance.soil_resistance(ds["se_root"], land_mask = ds["land_mask"], r_soil_pow = ds["r_soil_pow"], r_soil_min = ds["r_soil_min"])
@@ -209,66 +175,51 @@
     # **ETLook.unstable.initial_friction_velocity_soil_daily***********************************************************
     ds["u_star_24_soil_init"] = ETLook.unstable.initial_friction_velocity_soil_daily(ds["u_b_24"], ds["disp"], z_b = ds["z_b"])
 
     # **ETLook.unstable.initial_sensible_heat_flux_soil_daily***********************************************************
     ds["stc"] = ETLook.radiation.soil_thermal_conductivity(ds["se_root"])
     ds["vhc"] = ETLook.radiation.volumetric_heat_capacity(ds["se_root"], porosity = ds["porosity"])    
     
-    if et_look_version == "dev":
-        ds["stc"] = ETLook.radiation.soil_thermal_conductivity(se_top = ds["se_top"])
-        ds["vhc"] = ETLook.radiation.volumetric_heat_capacity(se_top = ds["se_top"], porosity = ds["porosity"])
-
     ds["dd"] = ETLook.radiation.damping_depth(ds["stc"], ds["vhc"])
     ds["g0_bs"] = ETLook.radiation.bare_soil_heat_flux(ds["doy"], ds["dd"], ds["stc"], ds["t_amp_year"], ds["lat_rad"])
     ds["g0_24"] = ETLook.radiation.soil_heat_flux(ds["g0_bs"], ds["sf_soil"], ds["land_mask"], ds["rn_24_soil"], ds["trans_24"], ds["ra_24"], ds["l_net"], ds["rn_slope"], ds["rn_offset"])
     ds["e_24_init"] = ETLook.neutral.initial_daily_evaporation(ds["rn_24_soil"], ds["g0_24"], ds["ssvp_24"], ds["ad_24"], ds["vpd_24"], ds["psy_24"], ds["r_soil"], ds["ra_soil_init"])
     ds["h_soil_24_init"] = ETLook.unstable.initial_sensible_heat_flux_soil_daily(ds["rn_24_soil"], ds["e_24_init"], ds["g0_24"])
 
     # **ETLook.unstable.evaporation***********************************************************
     ds["e_24"] = ETLook.unstable.evaporation(ds["rn_24_soil"], ds["g0_24"], ds["ssvp_24"], ds["ad_24"], ds["vpd_24"], ds["psy_24"], ds["r_soil"], ds["h_soil_24_init"], ds["t_air_k_24"], ds["u_star_24_soil_init"], ds["disp"], ds["u_b_24"], z_b = ds["z_b"], z_obs = ds["z_obs"], iter_h = ds["iter_h"])
     ds["e_24_mm"] = ETLook.unstable.evaporation_mm(ds["e_24"], ds["lh_24"])
     ds["et_24_mm"] = ETLook.evapotranspiration.et_actual_mm(ds["e_24_mm"], ds["t_24_mm"])
-    
-    if et_look_version == "dev":
-        ds["e_24_mm"] = np.clip(ds["e_24_mm"], 0, np.inf)
-        ds["et_24_mm"] = np.clip(ds["et_24_mm"], 0, np.inf)
 
     # **ETLook.unstable.evaporation***********************************************************
     ds["rn_24_grass"] = ETLook.radiation.net_radiation_grass(ds["ra_24"], ds["l_net"], r0_grass = ds["r0_grass"])
     ds["et_ref_24"] = ETLook.evapotranspiration.et_reference(ds["rn_24_grass"], ds["ad_24"], ds["psy_24"], ds["vpd_24"], ds["ssvp_24"], ds["u_24"])
     ds["et_ref_24_mm"] = ETLook.evapotranspiration.et_reference_mm(ds["et_ref_24"], ds["lh_24"])
 
-    if et_look_version == "dev":
-        ds["lue"] = ETLook.biomass.lue(ds["lue_max"], ds["stress_temp"], ds["stress_moist"], ds["eps_a"])
-        ds["fpar"] = ETLook.leaf.fpar(ds["vc"], ds["ndvi"])
-        ds["apar"] = ETLook.leaf.apar(ds["ra_24"], ds["fpar"])       
-        ds["biomass_prod"] = ETLook.biomass.biomass(ds["apar"], ds["lue"])         
-    else:
-
-        ds["t_air_k_min"] = ETLook.meteo.air_temperature_kelvin_daily(ds["t_air_min_24"])
-        ds["t_air_k_max"] = ETLook.meteo.air_temperature_kelvin_daily(ds["t_air_max_24"])
+    ds["t_air_k_min"] = ETLook.meteo.air_temperature_kelvin_daily(ds["t_air_min_24"])
+    ds["t_air_k_max"] = ETLook.meteo.air_temperature_kelvin_daily(ds["t_air_max_24"])
 
-        ds["t_air_k_12"] = ETLook.meteo.mean_temperature_kelvin_daytime(ds["t_air_k_min"], ds["t_air_k_max"])
+    ds["t_air_k_12"] = ETLook.meteo.mean_temperature_kelvin_daytime(ds["t_air_k_min"], ds["t_air_k_max"])
 
-        ds["t_dep"] = ETLook.biomass.temperature_dependency(ds["t_air_k_12"], dh_ap=ds["dh_ap"], d_s=ds["d_s"], dh_dp=ds["dh_dp"])
-        ds["k_m"] = ETLook.biomass.affinity_constant_co2(ds["t_air_k_12"])
-        ds["k_0"] = ETLook.biomass.inhibition_constant_o2(ds["t_air_k_12"])
-        ds["tau_co2_o2"] = ETLook.biomass.co2_o2_specificity_ratio(ds["t_air_k_12"])
+    ds["t_dep"] = ETLook.biomass.temperature_dependency(ds["t_air_k_12"], dh_ap=ds["dh_ap"], d_s=ds["d_s"], dh_dp=ds["dh_dp"])
+    ds["k_m"] = ETLook.biomass.affinity_constant_co2(ds["t_air_k_12"])
+    ds["k_0"] = ETLook.biomass.inhibition_constant_o2(ds["t_air_k_12"])
+    ds["tau_co2_o2"] = ETLook.biomass.co2_o2_specificity_ratio(ds["t_air_k_12"])
 
-        ds["year"] = ds.time_bins.dt.year.chunk("auto")
+    ds["year"] = ds.time_bins.dt.year.chunk("auto")
 
-        ds["co2_act"] = ETLook.biomass.co2_level_annual(ds["year"])
-        ds["a_d"] = ETLook.biomass.autotrophic_respiration(ds["t_air_k_24"], ar_slo=ds["ar_slo"], ar_int=ds["ar_int"])
+    ds["co2_act"] = ETLook.biomass.co2_level_annual(ds["year"])
+    ds["a_d"] = ETLook.biomass.autotrophic_respiration(ds["t_air_k_24"], ar_slo=ds["ar_slo"], ar_int=ds["ar_int"])
 
-        ds["apar"] = ETLook.biomass.par(ds["ra_24"])
-        ds["f_par"] = ETLook.biomass.fpar(ds["ndvi"], fpar_slope=ds["fpar_slope"], fpar_offset=ds["fpar_offset"])
+    ds["apar"] = ETLook.biomass.par(ds["ra_24"])
+    ds["f_par"] = ETLook.biomass.fpar(ds["ndvi"], fpar_slope=ds["fpar_slope"], fpar_offset=ds["fpar_offset"])
 
-        ds["co2_fert"] = ETLook.biomass.co2_fertilisation(ds["tau_co2_o2"], ds["k_m"], ds["k_0"], ds["co2_act"], o2=ds["o2"], co2_ref=ds["co2_ref"])
-        ds["npp_max"] = ETLook.biomass.net_primary_production_max(ds["t_dep"], ds["co2_fert"], ds["a_d"], ds["apar"], gcgdm=ds["gcgdm"])
-        ds["npp"] = ETLook.biomass.net_primary_production(ds["npp_max"], ds["f_par"], ds["stress_moist"], phot_eff=ds["phot_eff"])
+    ds["co2_fert"] = ETLook.biomass.co2_fertilisation(ds["tau_co2_o2"], ds["k_m"], ds["k_0"], ds["co2_act"], o2=ds["o2"], co2_ref=ds["co2_ref"])
+    ds["npp_max"] = ETLook.biomass.net_primary_production_max(ds["t_dep"], ds["co2_fert"], ds["a_d"], ds["apar"], gcgdm=ds["gcgdm"])
+    ds["npp"] = ETLook.biomass.net_primary_production(ds["npp_max"], ds["f_par"], ds["stress_moist"], phot_eff=ds["phot_eff"])
 
     ds = ds.drop_vars([x for x in ds.variables if ds[x].dtype == object])
 
     fp, fn = os.path.split(input_data)
 
     ds = g.variables.fill_attrs(ds)
     # g.network.create_network(ds, f"et_look_{et_look_version}.html")
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/__init__.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 ===========================================
-et_look_dev functions (:mod:`et_look_dev`)
+ pywapor.et_look_v2 functions (:mod:` pywapor.et_look_v2`)
 ===========================================
 
-.. currentmodule:: et_look_dev
+.. currentmodule::  pywapor.et_look_v2
 
-Within the :mod:`et_look_dev` module all physical and empirical
+Within the :mod:` pywapor.et_look_v2` module all physical and empirical
 functions related to the calculation of the soil moisture, interceptin,
 evaporation and transpiration are provided. These functions listed here
 can be used to build function chains.
 
-Instantaneous Radiation (:mod:`et_look_dev.clear_sky_radiation`)
+Instantaneous Radiation (:mod:` pywapor.et_look_v2.clear_sky_radiation`)
 ==============================================================
-.. automodule:: et_look_dev.clear_sky_radiation
+.. automodule::  pywapor.et_look_v2.clear_sky_radiation
 
 .. autosummary::
    :toctree: generated/
 
    beam_irradiance_horizontal_clear
    beam_irradiance_normal_clear
    day_angle
@@ -29,43 +29,43 @@
    ra_clear_horizontal
    rayleigh_optical_thickness
    relative_optical_airmass
    solar_constant
    solar_elevation_angle
    solar_elevation_angle_refracted
 
-Evapotranspiration (:mod:`et_look_dev.evapotranspiration`)
+Evapotranspiration (:mod:` pywapor.et_look_v2.evapotranspiration`)
 ===========================================================================
 
-.. automodule:: et_look_dev.evapotranspiration
+.. automodule::  pywapor.et_look_v2.evapotranspiration
 
 .. autosummary::
     :toctree: generated/
 
     et_actual_mm
     et_reference
     et_reference_mm
     interception_mm
 
-Vegetation Cover (:mod:`et_look_dev.leaf`)
+Vegetation Cover (:mod:` pywapor.et_look_v2.leaf`)
 ===========================================================
 
-.. automodule:: et_look_dev.leaf
+.. automodule::  pywapor.et_look_v2.leaf
 
 .. autosummary::
    :toctree: generated/
 
    vegetation_cover
    leaf_area_index
    effective_leaf_area_index
 
-Meteorology (:mod:`et_look_dev.meteo`)
+Meteorology (:mod:` pywapor.et_look_v2.meteo`)
 ==========================================================
 
-.. automodule:: et_look_dev.meteo
+.. automodule::  pywapor.et_look_v2.meteo
 
 .. autosummary::
    :toctree: generated/
 
    air_density
    air_density_daily
    air_density_inst
@@ -102,18 +102,18 @@
    vapour_pressure_from_specific_humidity_inst
    wet_bulb_temperature_kelvin_inst
    wind_speed_blending_height
    wind_speed_blending_height_daily
 
 
 
-Net Available Energy (:mod:`et_look_dev.radiation`)
+Net Available Energy (:mod:` pywapor.et_look_v2.radiation`)
 =================================================================
 
-.. automodule:: et_look_dev.radiation
+.. automodule::  pywapor.et_look_v2.radiation
 
 .. autosummary::
     :toctree: generated/
 
     bare_soil_heat_flux
     damping_depth
     interception_wm2
@@ -124,30 +124,30 @@
     net_radiation_grass
     net_radiation_soil
     soil_fraction
     soil_heat_flux
     soil_thermal_conductivity
     volumetric_heat_capacity
 
-Roughness (:mod:`et_look_dev.roughness`)
+Roughness (:mod:` pywapor.et_look_v2.roughness`)
 =============================================
 
-.. automodule:: et_look_dev.roughness
+.. automodule::  pywapor.et_look_v2.roughness
 
 .. autosummary::
    :toctree: generated/
 
    roughness_length
    obstacle_height
    displacement_height
 
-Solar radiation (:mod:`et_look_dev.solar_radiation`)
+Solar radiation (:mod:` pywapor.et_look_v2.solar_radiation`)
 =================================================================
 
-.. automodule:: et_look_dev.solar_radiation
+.. automodule::  pywapor.et_look_v2.solar_radiation
 
 .. autosummary::
     :toctree: generated/
 
     aspect_rad
     cosine_solar_zenith_angle
     daily_solar_radiation_flat
@@ -160,60 +160,58 @@
     inst_solar_radiation_toa
     inverse_earth_sun_distance
     latitude_rad
     seasonal_correction
     slope_rad
     sunset_hour_angle
 
-Plant stress (:mod:`et_look_dev.stress`)
+Plant stress (:mod:` pywapor.et_look_v2.stress`)
 ===================================================
 
-.. automodule:: et_look_dev.stress
+.. automodule::  pywapor.et_look_v2.stress
 
 .. autosummary::
     :toctree: generated/
 
     stress_moisture
     stress_radiation
     stress_temperature
     stress_vpd
-    epsilon_soil_moisture
-    epsilon_autotrophic_respiration
-    
-Canopy and Soil Resistance (:mod:`et_look_dev.resistance`)
+
+Canopy and Soil Resistance (:mod:` pywapor.et_look_v2.resistance`)
 ===========================================================
 
-.. automodule:: et_look_dev.resistance
+.. automodule::  pywapor.et_look_v2.resistance
 
 .. autosummary::
     :toctree: generated/
 
     atmospheric_canopy_resistance
     canopy_resistance
     soil_resistance
 
-Neutral Atmosphere (:mod:`et_look_dev.neutral`)
+Neutral Atmosphere (:mod:` pywapor.et_look_v2.neutral`)
 =====================================================
 
-.. automodule:: et_look_dev.neutral
+.. automodule::  pywapor.et_look_v2.neutral
 
 .. autosummary::
     :toctree: generated/
 
     initial_canopy_aerodynamic_resistance
     initial_daily_evaporation
     initial_daily_evaporation_mm
     initial_daily_transpiration
     initial_daily_transpiration_mm
     initial_soil_aerodynamic_resistance
 
-Unstable Atmosphere (:mod:`et_look_dev.unstable`)
+Unstable Atmosphere (:mod:` pywapor.et_look_v2.unstable`)
 =======================================================
 
-.. automodule:: et_look_dev.unstable
+.. automodule::  pywapor.et_look_v2.unstable
 
 .. autosummary::
     :toctree: generated/
 
     evaporation
     evaporation_mm
     friction_velocity
@@ -227,18 +225,18 @@
     stability_factor
     stability_parameter
     stability_parameter_obs
     transpiration
     transpiration_mm
 
 
-Soil Moisture (:mod:`et_look_dev.soil_moisture`)
+Soil Moisture (:mod:` pywapor.et_look_v2.soil_moisture`)
 ====================================================================
 
-.. automodule:: et_look_dev.soil_moisture
+.. automodule::  pywapor.et_look_v2.soil_moisture
 
 .. autosummary::
     :toctree: generated/
 
     psi_m
     psi_h
     aerodynamical_resistance_bare
@@ -259,25 +257,14 @@
     sensible_heat_flux_bare
     sensible_heat_flux_full
     soil_moisture_from_maximum_temperature
     wind_speed_blending_height_bare
     wind_speed_blending_height_full_inst
     wind_speed_soil_inst
 
-Biomass Production (:mod:`et_look_dev.biomass`)
-====================================================================
-
-.. automodule:: et_look_dev.biomass
 
-.. autosummary::
-    :toctree: generated/
-    
-    lue
-    apar
-    biomass
-    
 """
-from pywapor.et_look_dev import solar_radiation, clear_sky_radiation, meteo, radiation, evapotranspiration, soil_moisture, leaf, stress, resistance, roughness, neutral, unstable, biomass, constants
+from pywapor.et_look_v2_v3 import solar_radiation, clear_sky_radiation, meteo, radiation, evapotranspiration, soil_moisture, leaf, stress, resistance, roughness, neutral, unstable, constants, biomass
 
-__all__ = ['solar_radiation', 'clear_sky_radiation', 'meteo', 'radiation', 'evapotranspiration', 'soil_moisture', 'leaf', 'stress', 'resistance', 'roughness', 'neutral', 'unstable', 'biomass', 'constants']
+__all__ = ['solar_radiation', 'clear_sky_radiation', 'meteo', 'radiation', 'evapotranspiration', 'soil_moisture', 'leaf', 'stress', 'resistance', 'roughness', 'neutral', 'unstable', 'constants', 'biomass']
 
 __version__ = '0.1'
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/clear_sky_radiation.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/clear_sky_radiation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,467 +1,467 @@
 """
-    The clear_sky_radiation module contains all functions related to the
+    The `clear_sky_radiation` module contains all functions related to the
     calculation of (instantaneous) clear sky radation. Most of these
-    functions are based upon Šúri et Hofierka, 2004. [SuHi04]_
+    functions are based upon :footcite:t:`vsuri2004new`.
 
 """
 import numpy as np
 import xarray as xr
 
 def extraterrestrial_irradiance_normal(I0, ied):
     r"""
-    Computes the extraterrestrial irradiance normal to the solar beam
+    Computes the extraterrestrial irradiance normal to the solar beam.
 
     .. math ::
-        G_{0}=I_{0}\varepsilon
+
+        G_{0} = I_{0} \cdot \varepsilon
 
     Parameters
     ----------
     I0 : float
-        solar constant
+        solar constant, 
         :math:`I_{0}`
         [W m\ :sup:`-2`\]
     ied : float
-        inverse earth sun distance
+        inverse earth sun distance, 
         :math:`\varepsilon`
         [AU\ :sup:`-1`\]
 
     Returns
     -------
     G0 : float
-        ext rad normal to solar bea,
+        ext rad normal to solar bea, 
         :math:`G_{0}`
         [W m\ :sup:`-2`\]
 
     """
     return I0*ied
 
 
 def inverse_earth_sun_distance(day_angle):
     r"""
     Computes the inverse earth sun distance
 
     .. math ::
-        \varepsilon=1+0.03344\cos\left(j^{\prime}-0.048869\right)
+
+        \varepsilon = 1 + 0.03344 \cdot \cos(j^{\prime} - 0.048869)
 
     Parameters
     ----------
     day_angle : float
-        day angle
+        day angle, 
         :math:`j^{\prime}`
         [-]
 
     Returns
     -------
     ied : float
-        inverse earth sun distance
+        inverse earth sun distance, 
         :math:`\varepsilon`
         [AU]
 
     """
     return 1 + 0.03344 * np.cos(day_angle - 0.048869)
 
 
 def day_angle(doy):
     r"""
 
     Computes the day angle. 0 is january 1\ :sup:`st`\,
     2\ :math:`\pi` is december 31\ :sup:`st`\.
 
     .. math ::
-        j^{\prime}=\frac{2\pi j}{365.25}
+
+        j^{\prime} = \frac{2 \cdot \pi \cdot j} {365.25}
 
     Parameters
     ----------
     doy : float
-        day of year
+        day of year, 
         :math:`j`
         [-]
 
     Returns
     -------
     day_angle : float
-        day angle
+        day angle, 
         :math:`j^{\prime}`
         [rad]
 
     """
     return 2 * np.pi * doy / 365.25
 
 
 def solar_constant():
     r"""
     Returns the solar constant. The solar constant is defined as the
     flux density of solar radiation at the mean distance from Sun
-    to Earth. The solar constant is estimated to be 1367 W m\ :sup:`-2`\
+    to Earth. The solar constant is estimated to be 1367 W m\ :sup:`-2`\.
 
     Parameters
     ----------
 
     Returns
     -------
     I0 : float
-        solar constant
+        solar constant, 
         :math:`I_{0}`
         [W m\ :sup:`-2`\]
     """
     return 1367.
 
 
 def declination(day_angle):
     r"""
-    Computes the solar declination. The solar declination is computed according to
-    Gruter (1984) [Gr84]_
+    Computes the solar declination. The solar declination is computed according to 
+    :footcite:t:`gruter1984radiation`.
 
     .. math ::
-       \delta=\arcsin\left(0.3978\sin\left(j^{\prime}-1.4+0.0355\sin
-              \left(j^{\prime}-0.0489\right)\right)\right)
+
+        \delta = \arcsin\left(0.3978 \cdot \sin\left(j^{\prime} - 1.4 + 0.0355 \cdot \sin
+              \left(j^{\prime} - 0.0489\right)\right)\right)
 
     Parameters
     ----------
     day_angle : float
-        day angle
+        day angle, 
         :math:`j^{\prime}`
         [rad]
 
     Returns
     -------
     decl : float
-        declination
+        declination, 
         :math:`\delta`
         [rad]
 
-    References
-    ----------
-    .. [Gr84] Gruter, J. W. (ed), 1984, Radiation Nomenclature, Brussels, CEC, Second
-        Solar Energy Programme, Project F, Solar Radiation Data
     """
     return np.arcsin(0.3978 * np.sin(day_angle - 1.4 + 0.0355 * np.sin(day_angle - 0.0489)))
 
 
 def relative_optical_airmass(p_air_i, p_air_0_i, h0ref):
     r"""
-    Computes the relative optical air mass. It is calculated according to Kasten and Young 1989 [KaYo89]_
+    Computes the relative optical air mass. It is calculated according to :footcite:t:`kasten1989revised`.
 
     .. math ::
-       m=\left(\frac{p}{p_{0}}\right)/\left(\sin h_{0}^{ref}+0.50572
-         \left(h_{0}^{ref}+6.07995\right)^{-1.6364}\right)
+
+        m = \frac{\frac{p}{p_{0}}}{\sin h_{0}^{ref}+0.50572
+         \left(h_{0}^{ref}+6.07995\right)^{-1.6364}}
 
     Parameters
     ----------
     p_air_i : float
-        actual instantaneous air pressure
+        actual instantaneous air pressure, 
         :math:`p`
         [hPa]
     p_air_0_i : float
-        air pressure at sea level
+        air pressure at sea level, 
         :math:`p_{0}`
         [-]
     h0ref : float
-        solar elevation angle corrected for refraction
+        solar elevation angle corrected for refraction, 
         :math:`h_{0}^{ref}`
         [degrees]
 
     Returns
     -------
     m : float
-        relative optical airmass
+        relative optical airmass, 
         :math:`m`
         [-]
 
-    References
-    ----------
-    .. [KaYo89] Kasten F., and T.A. Young. 1989, Revised optical air mass tables
-       and approximation formula, Applied Optics 28:4735-8
     """
     h0ref_rad = h0ref * np.pi/180.
 
     m = (p_air_i/p_air_0_i)/(np.sin(h0ref_rad) + 0.50572 * (h0ref + 6.07995)**-1.6364)
     
-    if isinstance(m, xr.DataArray):
-        m = xr.where(h0ref_rad <= 0, 64, m)
-    else:
+    if isinstance(m, np.ndarray):
         m[h0ref_rad <= 0] = 64
+    else:
+        m = m.where(h0ref_rad > 0, 64)
 
     return m
 
 
 def solar_elevation_angle_refracted(h0):
     r"""
-    Computes the solar elevation angle corrected for refraction
+    Computes the solar elevation angle corrected for refraction.
 
     .. math ::
-       h_{0}^{ref} = h_{0} + \Delta h_{0}^{ref}
 
-    where
+        h_{0}^{ref} = h_{0} + \Delta h_{0}^{ref}
+
+    where:
 
     .. math ::
-        \Delta h_{0}^{ref}=0.61359\left(0.1594+1.123h_{0}+
-        0.065656h_{0}^{2}\right)/\left(
-        1+28.9344h_{0}+277.3971h_{0}^{2}\right)
+
+        \Delta h_{0}^{ref}=0.61359 \cdot \frac{0.1594 + 1.123 \cdot h_{0} +
+        0.065656 \cdot h_{0}^{2}}{
+        1+28.9344 \cdot h_{0} + 277.3971 \cdot h_{0}^{2}}
 
     Parameters
     ----------
     h0 : float
-        solar elevation angle
+        solar elevation angle, 
         :math:`h_{0}`
         [degrees]
 
     Returns
     -------
     h0ref : float
-        solar elevation angle corrected for refrection
+        solar elevation angle corrected for refrection, 
         :math:`h_{0}^{ref}`
         [degrees]
     """
     delta_h0ref = 0.061359 * (0.1594 + 1.123*h0 + 0.065656*h0**2)/(1 + 28.9344*h0 + 277.3971*h0**2)
     h0ref = h0 + delta_h0ref
 
     return h0ref
 
 
 def hour_angle(solar_time):
     r"""
-    Computes the solar hour angle
+    Computes the solar hour angle.
 
     .. math ::
-       T=\frac{\pi}{12}\left(t-12\right)
+
+        T = \frac{\pi}{12}\left(t-12\right)
 
     Parameters
     ----------
     solar_time : float
-        solar_time
+        solar_time, 
         :math:`t`
         [hours]
 
     Returns
     -------
     ha : float
-        solar hour angle
+        solar hour angle, 
         :math:`T`
         [rad]
 
     """
     ha = np.pi / 12 * (solar_time - 12)
 
     return ha
 
 
 def solar_elevation_angle(lat, decl, ha):
     r"""
-    Computes the solar elevation angle
+    Computes the solar elevation angle.
 
     .. math ::
-        h_{0}=\arcsin\left(C_{31}\cos T+C_{33}\right)
 
-    where
+        h_{0}=\arcsin\left(C_{31} \cdot \cos(T) + C_{33}\right)
+
+    where:
 
     .. math ::
-        C_{31}=\cos\varphi\cos\delta\;;\;C_{33}=\sin\varphi\sin\delta
+
+        C_{31} &= \cos(\varphi) \cdot \cos(\delta) \\
+        C_{33} &= \sin(\varphi) \cdot \sin(\delta)
 
     Parameters
     ----------
     lat : float
-        latitude
+        latitude, 
         :math:`\varphi`
         [rad]
     decl : float
-        declination
+        declination, 
         :math:`\delta`
         [rad]
     ha : float
-        solar hour angle
+        solar hour angle, 
         :math:`T`
         [rad]
 
     Returns
     -------
     h0 : float
-        solar elevation angle
+        solar elevation angle, 
         :math:`h_0`
         [degrees]
 
     """
     C31 = np.cos(lat) * np.cos(decl)
     C33 = np.sin(lat) * np.sin(decl)
 
     sin_h0 = C31 * np.cos(ha) + C33
 
     h0_rad = np.arcsin(sin_h0)
 
     h0 = h0_rad * 180 / np.pi
 
+    if isinstance(h0, xr.DataArray):
+        h0 = h0.transpose("time", "y", "x").chunk("auto")
+
     return h0
 
 
 def rayleigh_optical_thickness(m):
     r"""
     Computes the Rayleigh optical thickness at airmass :math:`m`. It is calculated according
-    to the improved formula by Kasten (1996) [Ka96]_
+    to the improved formula by :footcite:t:`kasten1996linke`.
 
     if :math:`m` > 20:
 
     .. math ::
 
-        \delta_{R}(m)=1/\left(6.6296+1.7513m-0.1202m^{2}+0.0065m^{3}-0.00013m^{4}\right)
+        \delta_{R}(m) = \left(6.6296 + 1.7513 \cdot  m - 0.1202 \cdot m^{2} + 0.0065 \cdot m^{3} - 0.00013 \cdot m^{4}\right)^{-1}
 
     if :math:`m` < 20:
 
     .. math ::
 
-        \delta_{R}(m)=1/\left(10.4+0.718m\right)
+        \delta_{R}(m) = \left(10.4+0.718 \cdot m\right)^{-1}
 
     Parameters
     ----------
     m : float
-        relative optical airmass
+        relative optical airmass, 
         :math:`m`
         [-]
 
     Returns
     -------
     rotm : float
-        Rayleigh optical thickness at airmass m
+        Rayleigh optical thickness at airmass m, 
         :math:`\delta_{R}`
         [-]
 
-    References
-    ----------
-    .. [Ka96] Kasten F. 1996, The Linke turbidity factor based on improved values of the
-       integral Rayleigh optical thickness. Solar Energy 56: 239-44
     """
 
     rotm = 1 / (10.4 + 0.718 * m)
-
-    if isinstance(rotm, xr.DataArray):
-        rotm = xr.where(m <= 20, 1/(6.6296 + 1.7513*m - 0.1202*m**2 + 0.0065*m**3 - 0.00013*m**4), rotm)
-    else:
+    if isinstance(rotm, np.ndarray):
         rotm = np.where(m <= 20, 1/(6.6296 + 1.7513*m - 0.1202*m**2 + 0.0065*m**3 - 0.00013*m**4), rotm)
+    else:
+        rotm_star = 1/(6.6296 + 1.7513*m - 0.1202*m**2 + 0.0065*m**3 - 0.00013*m**4)
+        rotm = rotm_star.where(m <= 20, rotm)
 
     return rotm
 
 
 def beam_irradiance_normal_clear(G0, Tl2, m, rotm, h0):
     r"""
-    Computes the clear sky beam irradiance normal to the solar beam
+    Computes the clear sky beam irradiance normal to the solar beam.
 
     .. math ::
 
-        B_{0c}=G_{0}\exp\left(-0.8662T_{LK}m\delta_{R}(m)\right)
+        B_{0c}=G_{0} \cdot \exp\left(-0.8662 \cdot T_{LK} \cdot m \cdot \delta_{R}\right)
 
     Parameters
     ----------
     G0 : float
-        ext rad normal to solar beam
+        ext rad normal to solar beam, 
         :math:`G_0`
         [W/m2]
     Tl2 : float
-        airmass  2 Linke atmospheric turbidity factor
+        airmass  2 Linke atmospheric turbidity factor, 
         :math:`T_{LK}`
         [-]
     m : float
-        relative optical airmass
+        relative optical airmass, 
         :math:`m`
         [-]
     rotm : float
-        Rayleigh optical thickness at airmass m
+        Rayleigh optical thickness at airmass m, 
         :math:`\delta_{R}`
         [-]
     h0 : float
-        solar elevation angle
+        solar elevation angle, 
         :math:`h_0`
         [degrees]
 
     Returns
     -------
     B0c : float
-        beam irradiance normal to the solar beam
+        beam irradiance normal to the solar beam, 
         :math:`B_{0c}`
         [W/m2]
 
     """
     B0c = G0 * np.exp(-0.8662 * Tl2 * m * rotm)
-
-    if isinstance(B0c, xr.DataArray):
-        B0c = xr.where(h0 < 0, 0, B0c)
-    else:
+    if isinstance(B0c, np.ndarray):
         B0c[h0 < 0] = 0
+    else:
+        B0c = B0c.where(h0 >= 0, 0)
 
     return B0c
 
 
 def beam_irradiance_horizontal_clear(B0c, h0):
     r"""
-    Computes the clear sky beam irradiance on a horizontal surface
+    Computes the clear sky beam irradiance on a horizontal surface.
 
     .. math ::
-        B_{hc}=B_{0c}\sin h_{0}
+
+        B_{hc} = B_{0c} \cdot \sin\left(h_{0}\right)
 
     Parameters
     ----------
     B0c : float
-        beam irradiance normal to the solar beam
+        beam irradiance normal to the solar beam, 
         :math:`B_{0c}`
         [W/m2]
     h0 : float
-        solar elevation angle
+        solar elevation angle, 
         :math:`h_0`
         [degrees]
 
     Returns
     -------
     Bhc : float
-        beam irradiance at a horizontal surface
+        beam irradiance at a horizontal surface, 
         :math:`B_{hc}`
         [W/m2]
 
     """
     Bhc = B0c * np.sin(h0 * np.pi / 180)
-
-    if isinstance(Bhc, xr.DataArray):
-        Bhc = xr.where(h0 < 0, 0, Bhc)
-    else:
+    if isinstance(Bhc, np.ndarray):
         Bhc[h0 < 0] = 0
+    else:
+        Bhc = Bhc.where(h0 >= 0, 0)
 
     return Bhc
 
 
 def linke_turbidity(wv_i, aod550_i, p_air_i, p_air_0_i):
     r"""
-    Computes the air mass 2 Linke atmospheric turbidity factor
+    Computes the air mass 2 Linke atmospheric turbidity factor.
 
     .. math ::
 
-        p_{rel}=\frac{p}{p_{0}}
-
-        T_{LK}=3.91\tau_{550}\exp\left(0.689p_{rel}\right)+0.376\ln\left(TCWV\right)+\left(2+0.54p_{rel}-0.34p_{rel}^{2}\right)
+        p_{rel} &= \frac{p}{p_{0}} \\
+        T_{LK} &= 3.91 \cdot \tau_{550} \cdot e^{0.689p_{rel}}+0.376 \cdot \ln\left(TCWV\right)+\left(2+0.54 \cdot p_{rel}-0.34 \cdot p_{rel}^{2}\right)
 
     Parameters
     ----------
     wv_i : float
-        total column atmospheric water vapor
+        total column atmospheric water vapor, 
         :math:`TCWV`
         [kg m-2]
     aod550_i : float
-        Aerosol optical depth at 550nm
+        Aerosol optical depth at 550nm, 
         :math:`aod550`
         [-]
     p_air_i : float
-        actual instantaneous air pressure
+        actual instantaneous air pressure, 
         :math:`p`
         [hPa]
     p_air_0_i : float
-        air pressure at sea level
+        air pressure at sea level, 
         :math:`p_0`
         [-]
 
     Returns
     -------
     Tl2 : float
-        Airmass 2 Linke atmospheric turbidity factor
+        Airmass 2 Linke atmospheric turbidity factor, 
         :math:`T_{LK}`
         [-]
 
     Examples
     --------
     """
     # prel = p0 / p # Papers mixes p/p0 and p0/p????
@@ -473,113 +473,114 @@
     Tl2 = term1 + term2 + (2 + 0.54 * prel - 0.5 * prel**2 + 0.16 * prel**2)
 
     return Tl2
 
 
 def diffuse_irradiance_horizontal_clear(G0, Tl2, h0):
     r"""
-    Computes the clear sky beam irradiance on a horizontal surface
+    Computes the clear sky beam irradiance on a horizontal surface.
 
     .. math ::
 
-        D_{hc}=G_{0}Tn\left(T_{LK}\right)F_{d}\left(h_{0}\right)
+        D_{hc}=G_{0} \cdot Tn\left(T_{LK}\right) \cdot F_{d}\left(h_{0}\right)
 
     For the estimation of the transmission function :math:`Tn\left(T_{LK}\right)`
     the following function is used:
 
     .. math ::
 
-        Tn\left(T_{LK}\right)=-0.015843+0.030543T_{LK}+0.0003797T_{LK}^{2}
+        Tn\left(T_{LK}\right)=-0.015843+0.030543 \cdot T_{LK}+0.0003797 \cdot T_{LK}^{2}
 
     The solar altitude function :math:`F_{d}\left(h_{0}\right)` is evaluated using the expression:
 
     .. math ::
 
-        F_{d}\left(h_{0}\right)=A_{1}+A_{2}\sin h_{0}+A_{3}sin^{2}h_{0}
+        F_{d}\left(h_{0}\right)=A_{1}+A_{2} \cdot \sin (h_{0})+A_{3} \cdot sin^{2}(h_{0})
 
     with:
 
     .. math ::
 
-        A_{1}^{\prime}=0.26463-0.061581T_{LK}+0.0031408T_{LK}^{2}
-
-        A_{1}=0.0022/Tn\left(T_{LK}\right) \: \text{if} \: A_{1}^{\prime}Tn\left(T_{LK}\right)<0.0022
-
-        A_{1}=A_{1}^{\prime} \: \text{if} \: A_{1}^{\prime}Tn\left(T_{LK}\right)\geq0.0022
-
-        A_{2}=2.04020+0.018945T_{LK}-0.011161T_{LK}^{2}
-
-        A_{3}=-1.3025+0.039231T_{LK}+0.0085079T_{LK}^{2}
-
-
+        A_{1}^{\prime} &= 0.26463-0.061581 \cdot T_{LK}+0.0031408 \cdot T_{LK}^{2} \\
+        A_{1} &= \frac{0.0022}{Tn\left(T_{LK}\right)} \: \text{if} \: A_{1}^{\prime} \cdot Tn\left(T_{LK}\right)<0.0022 \\
+        A_{1} &= A_{1}^{\prime} \: \text{if} \: A_{1}^{\prime} \cdot Tn\left(T_{LK}\right)\geq0.0022 \\
+        A_{2} &= 2.04020+0.018945 \cdot T_{LK}-0.011161 \cdot T_{LK}^{2} \\
+        A_{3} &= -1.3025+0.039231 \cdot T_{LK}+0.0085079 \cdot T_{LK}^{2}
 
     Parameters
     ----------
     G0 : float
-        ext rad normal to solar beam
+        ext rad normal to solar beam, 
         :math:`G_0`
         [W/m2]
     Tl2 : float
-        Airmass 2 Linke atmospheric turbidity factor
+        Airmass 2 Linke atmospheric turbidity factor, 
         :math:`T_{LK}`
         [-]
     h0 : float
-        solar elevation angle
+        solar elevation angle, 
         :math:`h_0`
         [degrees]
 
     Returns
     -------
     Dhc : float
-        Diffuse irradiance at a horizontal surface
+        Diffuse irradiance at a horizontal surface, 
         :math:`D_{hc}`
         [W/m2]
 
     Examples
     --------
     """
     h0_rad = h0 * np.pi / 180.
     TnTl2 = -0.015843 + 0.030543 * Tl2 + 0.0003797 * Tl2**2
 
     A1 = 0.26463 - 0.061581 * Tl2 + 0.0031408 * Tl2**2
-    A1 = np.where((A1 * TnTl2) < 0.0022, 0.0022 / TnTl2, A1)
+    if isinstance(A1, xr.DataArray):
+        A1 = xr.where((A1 * TnTl2) < 0.0022, 0.0022 / TnTl2, A1)
+    else:
+        A1 = np.where((A1 * TnTl2) < 0.0022, 0.0022 / TnTl2, A1)
     A2 = 2.04020 + 0.018945 * Tl2 - 0.011161 * Tl2**2
     A3 = -1.3025 + 0.039231 * Tl2 + 0.0085079 * Tl2**2
 
     FdH0 = A1 + A2 * np.sin(h0_rad) + A3 * np.sin(h0_rad)**2
 
     Dhc = G0 * TnTl2 * FdH0
 
-    Dhc = np.clip(Dhc, 0, np.inf)
+    if isinstance(Dhc, np.ndarray):
+        Dhc[Dhc < 0] = 0
+    else:
+        Dhc = Dhc.where(Dhc >= 0, 0)
     
     return Dhc
 
 
 def ra_clear_horizontal(Bhc, Dhc):
     r"""    
-    Computes the clear sky beam irradiance on a horizontal surface
+    Computes the clear sky beam irradiance on a horizontal surface.
 
     .. math ::
+
         G_{hc}=B_{hc}+D_{hc}
 
     Parameters
     ----------
     Bhc : float
-        beam irradiance at a horizontal surface
+        beam irradiance at a horizontal surface, 
         :math:`B_{hc}`
         [W/m2]
     Dhc : float
-        Diffuse irradiance at a horizontal surface
+        Diffuse irradiance at a horizontal surface, 
         :math:`D_{hc}`
         [W/m2]
         
     Returns
     -------
     ra_hor_clear_i : float
-        Total clear-sky irradiance on a horizontal surface
+        Total clear-sky irradiance on a horizontal surface, 
         :math:`G_{hc}`
         [W/m2]
 
     Examples
     --------
     """
     ra_clear_hor = Bhc + Dhc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/constants.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # http://lawr.ucdavis.edu/classes/SSC100/probsets/pset01.html
 # 6. Calculate the porosity of a soil sample that has a bulk density of 1.35 g/cm3. Assume the particle density is 2.65 g/cm3.
 # Porosity = (1-(r b/r d) x 100 = (1-(1.35/2.65)) x 100 = 49%
 # page 31 flow diagram
 
 # **effective_leaf_area_index**************************************************
 # constants or predefined:
-nd_min = 0.1 # 0.125
+nd_min = 0.125
 nd_max = 0.8
 vc_pow = 0.7
 vc_min = 0
 vc_max = 0.9677324224821418
 lai_pow = -0.45
 
 # **atmospheric canopy resistance***********************************************
@@ -61,31 +61,32 @@
 rcan_max = 1000000
 
 # **net radiation canopy******************************************************
 # constants or predefined:
 vp_slope = 0.14
 vp_offset = 0.34
 lw_slope = 1.35
-lw_offset = 0.35
+lw_offset = -0.35
 int_max = 0.2
 
 # **canopy resistance***********************************************************
 # constants or predefined:
-r0_bare = 0.42 # 0.38
+r0_bare = 0.38 # used for se_root calc
 r0_bare_wet = 0.20
-r0_full = 0.18
-tenacity = 1.0
+r0_full = 0.18 # used for se_root calc
+tenacity = 1.5
 disp_bare = 0.0
 disp_full = 0.667
 fraction_h_bare = 0.65
 fraction_h_full = 0.95
 
 z_obs = 2
 z_b = 100
-z0m_bare = 0.0005 # 0.001
+z0m_bare = 0.001 # 0.0005
+z0m_full = 0.1
 
 # **initial canopy aerodynamic resistance***********************************************************
 # constants or predefined:
 ndvi_obs_min = 0.25
 ndvi_obs_max = 0.75
 obs_fr = 0.25
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/evapotranspiration.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/evapotranspiration.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,232 +1,197 @@
-from pywapor.et_look_dev import constants as c
+from pywapor.et_look_v2_v3 import constants as c
 import numpy as np
 import xarray as xr
 
-def evaporative_fraction(et_24_mm, lh_24, rn_24, g0_24):
-    r"""
-    Computes the evaporative fraction.
-
-    where the following constants are used
-
-    * :math:`d_{sec}` seconds in the day = 86400 [s]
-
-    Parameters
-    ----------
-    et_24_mm : float
-        daily actual evapotranspiration
-        :math:`ET_{ref}`
-        [mm]
-    lh_24 : float
-        daily latent heat of evaporation
-        :math:`\lambda_{24}`
-        [J/kg]
-    rn_24 : float
-        daily net radiation
-        :math:`Q^{*}`
-        [Wm-2]
-    g0_24 : float
-        daily soil heat flux
-        :math:`G`
-        [W m-2]
-        
-    Returns
-    -------
-    ef_24 : float
-        evaporative fraction
-        :math:`EF_{ref}`
-        [-]
-    """
-    et_24 = et_24_mm * lh_24/c.day_sec
-    ef_24 = et_24/(rn_24 - g0_24)
-    
-    return ef_24
-
-
 def interception_mm(P_24, vc, lai, int_max=0.2):
     r"""
     Computes the daily interception. The daily interception of a vegetated area
-    is calculated according to von Hoyningen-Hüne (1983) [Ho1983]_
-    and Braden(1985) [Br1985]_.
+    is calculated according to :footcite:t:`braden1985energiehaushalts` 
+    and :footcite:t:`hoyningen1983interception`.
 
     .. math ::
-        I^*=I_{max}*I_{lai}*\left(1-\left(\frac{1}{1+\frac{c_{veg}P24}
-        {I_{max}I_{lai}}}\right)\right)
+
+        I^*=I_{max} \cdot I_{lai} \cdot \left(1-\frac{1}{1+\frac{c_{veg} \cdot P}
+        {I_{max} \cdot I_{lai}}}\right)
 
     Parameters
     ----------
     P_24 :  float
-        daily rainfall
+        daily rainfall, 
         :math:`P`
         [mm day :math:`^{-1}`]
 
     vc : float
-        vegetation cover
+        vegetation cover, 
         :math:`c_{veg}`
         [-]
 
     lai : float
-        leaf area index
+        leaf area index, 
         :math:`I_{lai}`
         [-]
 
     int_max :  float
-        maximum interception per leaf
+        maximum interception per leaf, 
         :math:`I_{max}`
         [mm day :math:`^{-1}`]
 
     Returns
     -------
     int_mm : float
-        interception
+        interception, 
         :math:`I^*`
         [mm day :math:`^{-1}`]
 
-    References
-    ----------
-    .. [Br1985] Braden, H., Energiehaushalts- und Verdunstungsmodell für Wasser- und
-        Stoffhaushalts-untersuchungen landwirtschaftlich genutzter
-        Einzugsgebiete. Mitteilungen der Deutschen Bodenkundlichen
-        Gesellschaft, (1985), 42, 254-299
-    .. [Ho1983] von Hoyningen-Hüne, J., Die Interception des Niederschlags in
-        landwirtschaftlichen Beständen. Schriftenreihe des DVWK, 1983, 57, 1-53
-
-
     """
-    zero_mask = np.logical_or.reduce((lai == 0, vc == 0, P_24 == 0))
+    if isinstance(lai, xr.DataArray):
+        zero_mask = np.logical_or(np.logical_or(vc == 0, lai ==0), P_24 == 0)
+    else:
+        zero_mask = np.logical_or.reduce((lai == 0, vc == 0, P_24 == 0))
 
     res = int_max * lai * (1 - (1 / (1 + ((vc * P_24) / (int_max * lai)))))
 
     if isinstance(res, xr.DataArray):
         res = xr.where(zero_mask, 0.0, res)
     else:
         res[zero_mask] = 0
 
     return res
 
 
 def et_reference(rn_24_grass, ad_24, psy_24, vpd_24, ssvp_24, u_24):
     r"""
-    Computes the reference evapotranspiration. The reference evapotranspiration
-    :math:`ET_{ref}` is an important concept in irrigation science. The reference
-    evapotranspiration can be inferred from routine meteorological
-    measurements. The reference evapotranspiration is the evapotranspiration
-    of grass under well watered conditions.
-    First the aerodynamical resistance for grass :math:`r_{a,grass}` [sm :math:`^{-1}`]
-    is calculated
+    Computes the reference evapotranspiration. 
+    
+    The reference evapotranspiration :math:`ET_{ref}` is an important concept 
+    in irrigation science. The reference evapotranspiration can be inferred 
+    from routine meteorological measurements. 
+    
+    The reference evapotranspiration is the evapotranspiration of grass under 
+    well watered conditions. First the aerodynamical resistance for 
+    grass :math:`r_{a,grass}` [sm :math:`^{-1}`] is calculated:
 
     .. math ::
 
         r_{a,grass}=\frac{208}{u_{obs}}
 
     Then the reference evapotranspiration :math:`ET_{ref}` [W m :math:`^{-2}`] can be calculated
     as follows, with taking the default value for the grass surface resistance
     :math:`r_{grass}` = 70 sm :math:`^{-1}`
 
     .. math ::
-        ET_{ref}=\frac{\Delta\left(Q_{grass}^{*}\right)+
+
+        ET_{ref}=\frac{\Delta \cdot Q_{grass}^{*}+
         \rho c_{p}\frac{\Delta_{e}}{r_{a,grass}}}
-        {\Delta+\gamma\left(1+\frac{r_{grass}}{r_{a,grass}}\right)}
+        {\Delta+\gamma \cdot \left(1+\frac{r_{grass}}{r_{a,grass}}\right)}
 
     The soil heat flux is assumed to be zero or close to zero on a daily basis.
 
     Parameters
     ----------
     rn_24_grass : float
-        net radiation for reference grass surface
+        net radiation for reference grass surface, 
         :math:`Q^{*}_{grass}`
         [Wm-2]
     u_24 : float
-        daily wind speed at observation height
+        daily wind speed at observation height, 
         :math:`u_{obs}`
         [m/s]
     ad_24 : float
-        daily air density
+        daily air density, 
         :math:`\rho_{24}`
         [kg m-3]
     psy_24 : float
-        daily psychrometric constant
+        daily psychrometric constant, 
         :math:`\gamma_{24}`
         [mbar K-1]
     vpd_24 : float
-        daily vapour pressure deficit
+        daily vapour pressure deficit, 
         :math:`\Delta_{e,24}`
         [mbar]
     ssvp_24 : float
-        daily slope of saturated vapour pressure curve
+        daily slope of saturated vapour pressure curve, 
         :math:`\Delta_{24}`
         [mbar K-1]
 
     Returns
     -------
     et_ref_24 : float
-        reference evapotranspiration (well watered grass) energy equivalent
+        reference evapotranspiration (well watered grass) energy equivalent, 
         :math:`ET_{ref}`
         [W m-2]
     """
     r_grass = 70
     ra_grass = 208. / u_24
-    et_ref_24 = np.maximum(0,(ssvp_24 * rn_24_grass + ad_24 * c.sh * (vpd_24 / ra_grass)) /\
-        (ssvp_24 + psy_24 * (1 + r_grass / ra_grass)))
+    et_ref_24 = (ssvp_24 * rn_24_grass + ad_24 * c.sh * (vpd_24 / ra_grass)) /\
+        (ssvp_24 + psy_24 * (1 + r_grass / ra_grass))
     return et_ref_24
 
 
 def et_reference_mm(et_ref_24, lh_24):
     r"""
     Computes the reference evapotranspiration.
 
     .. math ::
 
-        ET_{ref}=ET_{ref}d_{sec}\lambda_{24}
+        ET_{ref}=ET_{ref} \cdot d_{sec} \cdot \lambda_{24}
 
-    where the following constants are used
+    where:
 
     * :math:`d_{sec}` seconds in the day = 86400 [s]
 
     Parameters
     ----------
     et_ref_24 : float
-        daily reference evapotranspiration energy equivalent
+        daily reference evapotranspiration energy equivalent, 
         :math:`ET_{ref}`
         [W m-2]
     lh_24 : float
-        daily latent heat of evaporation
+        daily latent heat of evaporation, 
         :math:`\lambda_{24}`
         [J/kg]
 
     Returns
     -------
     et_ref_24_mm : float
-        reference evapotranspiration (well watered grass)
+        reference evapotranspiration (well watered grass), 
         :math:`ET_{ref}`
         [mm d-1]
     """
-    return et_ref_24 * c.day_sec / lh_24
+    x = et_ref_24 * c.day_sec / lh_24
+
+    if isinstance(x, xr.DataArray):
+        et_ref_24_mm = x.clip(0, np.inf)
+    else:
+        et_ref_24_mm = np.clip(x, 0, np.inf)
+
+    return et_ref_24_mm
 
 
 def et_actual_mm(e_24_mm, t_24_mm):
     r"""
     Computes the actual evapotranspiration based on the separate calculations
-    of evaporation and transpiration:
+    of evaporation and transpiration.
 
     .. math ::
+
         ET = E + T
 
     Parameters
     ----------
     e_24_mm : float
-        daily evaporation in mm
+        daily evaporation in mm, 
         :math:`E`
         [mm d-1]
     t_24_mm : float
-        daily transpiration in mm
+        daily transpiration in mm, 
         :math:`T`
         [mm d-1]
 
     Returns
     -------
     et_24_mm : float
-        daily evapotranspiration in mm
+        daily evapotranspiration in mm, 
         :math:`ET`
         [mm d-1]
     """
     return e_24_mm + t_24_mm
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/leaf.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/leaf.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,49 +4,50 @@
 
 """
 import numpy as np
 import xarray as xr
 
 def vegetation_cover(ndvi, nd_min=0.125, nd_max=0.8, vc_pow=0.7):
     r"""
-    Computes vegetation cover based on NDVI
+    Computes vegetation cover based on NDVI.
 
     .. math ::
+
         c_{veg} =
         \begin{cases}
         \begin{array}{cc}
         0 & I_{NDVI}\leq I_{NDVI,min}\\
         1-\left(\frac{I_{NDVI,max}-I_{NDVI}}{I_{NDVI,max}-I_{NDVI,min}}\right)^
         {a} & I_{NDVI,min}<I_{NDVI}<I_{NDVI,max}\\
         1 & I_{NDVI}\geq I_{NDVI,max}
         \end{array}\end{cases}
 
     Parameters
     ----------
     ndvi : float
-        Normalized Difference Vegetation Index
+        Normalized Difference Vegetation Index, 
         :math:`I_{NDVI}`
         [-]
     nd_min : float
-        NDVI value where vegetation cover is 0
+        NDVI value where vegetation cover is 0, 
         :math:`I_{NDVI,min}`
         [-]
     nd_max : float
-        NDVI value where vegetation cover is 1
+        NDVI value where vegetation cover is 1, 
         :math:`I_{NDVI,max}`
         [-]
     vc_pow : float
-        Exponential power used in vegetation cover function
+        Exponential power used in vegetation cover function, 
         :math:`a`
         [-]
 
     Returns
     -------
     vc : float
-        vegetation cover
+        vegetation cover, 
         :math:`c_{veg}`
         [-]
 
     Examples
     --------
     >>> from ETLook import leaf
     >>> leaf.vegetation_cover(0.1, nd_min=0.2)
@@ -76,58 +77,60 @@
             # fill in array
             res[ndvi <= nd_min] = 0
             res[np.logical_and(ndvi > nd_min, ndvi < nd_max)] = 1 - (
                         (nd_max - ndvi[np.logical_and(ndvi > nd_min, ndvi < nd_max)]) / (nd_max - nd_min)) ** vc_pow
             res[ndvi >= nd_max] = 1
         else:
             res = 1 - ((nd_max - ndvi) / (nd_max - nd_min)) ** vc_pow
-            res = res.clip(0.0, 1.0)
+            res = xr.where(ndvi <= nd_min, 0, res)
+            res = xr.where(ndvi >= nd_max, 1, res)
 
     return res
 
 
 def leaf_area_index(vc, vc_min=0.0, vc_max=vegetation_cover(0.795), lai_pow=-0.45):
     r"""
     Computes leaf area index based on vegetation cover. It is based on the
     Kustas formulation of LAI vs NDVI.
 
     .. math ::
+
         I_{lai} =
         \begin{cases}
         \begin{array}{cc}
         0 & c_{veg}\leq c_{veg,min}\\
         \frac{\ln\left(-\left(c_{veg}-1\right)\right)}{b} &
         c_{veg,min}<c_{veg}\leq c_{veg,max}\\
         \frac{\ln\left(-\left(c_{veg,max}-1\right)\right)}{b} &
         c_{veg}>c_{veg,max}
         \end{array}\end{cases}
 
     Parameters
     ----------
     vc : float
-        vegetation cover
+        vegetation cover, 
         :math:`c_{veg}`
         [-]
     vc_min : float
-        vegetation cover where LAI is 0
+        vegetation cover where LAI is 0, 
         :math:`c_{veg,min}`
         [-]
     vc_max : float
-        vegetation cover at maximum LAI
+        vegetation cover at maximum LAI, 
         :math:`c_{veg,max}`
         [-]
     lai_pow : float
-        exponential factor used in LAI function
+        exponential factor used in LAI function, 
         :math:`b`
         [-]
 
     Returns
     -------
     lai : float
-        leaf area index
+        leaf area index, 
         :math:`I_{lai}`
         [-]
 
     Examples
     --------
     >>> from ETLook import leaf
     >>> leaf.leaf_area_index(0.0)
@@ -171,95 +174,35 @@
     Computes effective leaf area index, this describes the leaf area which
     actively participates in transpiration. It is based on the actual leaf
     area index and an extinction function. So with a higher leaf area index the
     effective leaf area index is a smaller percentage of the total leaf area
     index.
 
     .. math ::
-        I_{lai,eff}=\frac{I_{lai}}{0.3I_{lai}+1.2}
+
+        I_{lai,eff}=\frac{I_{lai}}{0.3 \cdot I_{lai}+1.2}
 
     Parameters
     ----------
     lai : float
-        Leaf area index
+        Leaf area index, 
         :math:`I_{lai}`
         [-]
 
     Returns
     -------
     lai_eff : float
-        effective leaf area index
+        effective leaf area index, 
         :math:`I_{lai,eff}`
         [-]
 
     Examples
     --------
     >>> from ETLook import leaf
     >>> leaf.effective_leaf_area_index(3.0)
     1.4285714285714288
     >>> leaf.effective_leaf_area_index(5.0)
     1.8518518518518516
 
     """
     lai_eff = lai / ((0.3 * lai) + 1.2)
     return lai_eff
-
-def fpar(vc, ndvi):
-    r"""
-    Computes the fpar
-
-    Parameters
-    ----------
-    vc : float
-        vegetation cover
-        :math:`c_{veg}`
-        [-]
-    ndvi : float
-        Normalized Difference Vegetation Index
-        :math:`I_{NDVI}`
-        [-]
-        
-    Returns
-    -------
-    fpar : float
-        fpar
-        :math:`I_{vc,ndvi}`
-        [-]
-
-    """
-    # fpar = 0.925 * vc
-    fpar = 0.8624 * ndvi - 0.0814
-    if isinstance(fpar, xr.DataArray):
-        fpar = xr.where(ndvi < 0.1, 0.0, fpar)
-    else:
-        fpar[ndvi < 0.1] = 0.0
-
-    return fpar
-
-def apar(ra_24, fpar):    
-    r"""
-    Computes the Aborbed Photosynthetical Active Radiation
-
-    Parameters
-    ----------
-    ra_24 : float
-        daily solar radiation
-        :math:`S^{\downarrow}`
-        [Wm-2]
-    fpar : float
-        fpar
-        :math:`I_{vc,ndvi}`
-        [-]
-        
-    Returns
-    -------
-    apar : float
-        apar
-        :math:`I_{ra_24,fpar}`
-        [MJ/m2]
-
-    """
-    par = 0.48 * ra_24 * 0.0864
-    apar = par * fpar
-    
-    return apar     
-
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/meteo.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/meteo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,174 +1,173 @@
 """
     The meteo module contains all functions related to meteorological
     variables. All meteorological functions can be calculated on a daily
     or instantaneous basis. Base functions are available also. The daily
     functions have a 'daily' extension, instantaneous functions have a 'inst'
-    extension
+    extension.
 
 """
-from pywapor.et_look_dev import constants as c
+from pywapor.et_look_v2_v3 import constants as c
 import numpy as np
 import xarray as xr
 
-def air_temperature_celcius(t_air_k):
+def mean_temperature_kelvin_daytime(t_air_k_min, t_air_k_max):
     r"""
-    Converts air temperature from Kelvin to Celcius, where 0 degrees Celcius
-    is equal to 273.15 degrees Kelvin
+    Computes the mean temperature over the daily sunshine period.
 
     Parameters
     ----------
-    t_air_k : float
-        air temperature
-        :math:`T_a`
+    t_air_k_min : float
+        maximum air temperature
+        :math:`T_{a,min}`
+        [K]
+    t_air_k_max : float
+        maximum air temperature
+        :math:`T_{a,max}`
         [K]
 
     Returns
     -------
-    t_air_c : float
-        air temperature
-        :math:`T_a`
-        [C]
+    t_air_k_12 : float
+        daytime air temperature
+        :math:`T_{a,12}`
+        [K]
 
-    Examples
-    --------
-    >>> from ETLook import meteo
-    >>> meteo.air_temperature_celcius(12.5)
-    285.65
     """
-    return t_air_k - c.zero_celcius
+    return 0.25 * t_air_k_min + 0.75 * t_air_k_max
 
 
 def air_temperature_kelvin(t_air):
     r"""
     Converts air temperature from Celcius to Kelvin, where 0 degrees Celcius
-    is equal to 273.15 degrees Kelvin
+    is equal to 273.15 degrees Kelvin.
 
     Parameters
     ----------
     t_air : float
-        air temperature
+        air temperature, 
         :math:`T_a`
         [C]
 
     Returns
     -------
     t_air_k : float
-        air temperature
+        air temperature, 
         :math:`T_a`
         [K]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> meteo.air_temperature_kelvin(12.5)
     285.65
     """
     return t_air + c.zero_celcius
 
 
 def air_temperature_kelvin_daily(t_air_24):
-    """Like :func:`air_temperature_kelvin` but as a daily average
+    """Like :func:`air_temperature_kelvin` but as a daily average.
 
     Parameters
     ----------
     t_air_24 : float
-        daily air temperature
+        daily air temperature, 
         :math:`T_{a,24}`
         [C]
 
     Returns
     -------
     t_air_k_24 : float
-        daily air temperature
+        daily air temperature, 
         :math:`T_{a,24}`
         [K]
     """
     return air_temperature_kelvin(t_air_24)
 
 
 def air_temperature_kelvin_inst(t_air_i):
-    """Like :func:`air_temperature_kelvin` but as an instantaneous value
+    """Like :func:`air_temperature_kelvin` but as an instantaneous value.
 
     Parameters
     ----------
     t_air_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a,i}`
         [C]
 
     Returns
     -------
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a,i}`
         [K]
     """
     return air_temperature_kelvin(t_air_i)
 
 
 def wet_bulb_temperature_kelvin_inst(t_wet_i):
     """
     Converts wet bulb temperature from Celcius to Kelvin, where 0
-    degrees Celcius is equal to 273.15 degrees Kelvin
+    degrees Celcius is equal to 273.15 degrees Kelvin.
 
     Parameters
     ----------
     t_wet_i : float
-        instantaneous wet bulb temperature
+        instantaneous wet bulb temperature, 
         :math:`T_{w,i}`
         [C]
 
     Returns
     -------
     t_wet_k_i : float
-        instantaneous wet bulb temperature
+        instantaneous wet bulb temperature, 
         :math:`T_{w,i}`
         [K]
     """
     return air_temperature_kelvin(t_wet_i)
 
 
 def disaggregate_air_temperature(t_air_coarse, z, z_coarse, lapse=-0.006):
     r"""
     Disaggregates GEOS or MERRA or another coarse scale air temperature using
     two digital elevation models. One DEM for the target resolution, another
     DEM smoothed from the original air temperature resolution to the target
     resolution.
 
     .. math ::
-        T_{a}=T_{a,c}+(z-z_{c})L_{T}-T_{K,0}
+
+        T_{a}=T_{a,c}+(z-z_{c}) \cdot L_{T}-T_{K,0}
 
     where the following constant is used
 
     * :math:`T_{K,0}` = 273.15 K is equal to 0 degrees Celsius
 
     Parameters
     ----------
     t_air_coarse : float
-        air temperature at coarse resolution
+        air temperature at coarse resolution, 
         :math:`T_{a,c}`
         [K]
     z : float
-        elevation
+        elevation, 
         :math:`z`
         [m]
     z_coarse : float
-        elevation at coarse resolution
+        elevation at coarse resolution, 
         :math:`z_{c}`
         [m]
     lapse : float
-        lapse rate
+        lapse rate, 
         :math:`L_{T}`
         [K m-1]
 
     Returns
     -------
     t_air : float
-        air temperature
+        air temperature, 
         :math:`T_{a}`
         [C]
 
     Notes
     -----
     The input air temperature is specified in Kelvin. The output air
     temperature is specified in C.
@@ -179,378 +178,503 @@
     >>> meteo.disaggregate_air_temperature(24.5+273.15, 10, 5)
     24.47
     """
     return t_air_coarse + ((z - z_coarse) * lapse) - c.zero_celcius
 
 
 def disaggregate_air_temperature_daily(t_air_24_coarse, z, z_coarse, lapse=-0.006):
-    r"""Like :func:`disaggregate_air_temperature` but as a daily average
+    r"""Like :func:`disaggregate_air_temperature` but as a daily average.
 
     Parameters
     ----------
     t_air_24_coarse : float
-        daily air temperature at coarse resolution
+        daily air temperature at coarse resolution, 
         :math:`T_{a,24,c}`
         [K]
     z : float
-        elevation
+        elevation, 
         :math:`z`
         [m]
     z_coarse : float
-        elevation at coarse resolution
+        elevation at coarse resolution, 
         :math:`z_{c}`
         [m]
     lapse : float
-        lapse rate
+        lapse rate, 
         :math:`L`
         [K m-1]
 
     Returns
     -------
     t_air_24 : float
-        daily air temperature
+        daily air temperature, 
         :math:`T_{a,24}`
         [C]
 
     Notes
     -----
     The input air temperature is specified in Kelvin. The output air
     temperature is specified in C.
     """
     return disaggregate_air_temperature(t_air_24_coarse, z, z_coarse, lapse)
 
 
 def disaggregate_air_temperature_inst(t_air_i_coarse, z, z_coarse, lapse=-0.006):
-    r"""Like :func:`disaggregate_air_temperature` but as a instantaneous value
+    r"""Like :func:`disaggregate_air_temperature` but as a instantaneous value.
 
     Parameters
     ----------
     t_air_i_coarse : float
-        instantaneous air temperature at coarse resolution
+        instantaneous air temperature at coarse resolution, 
         :math:`T_{a,i,c}`
         [K]
     z : float
-        elevation
+        elevation, 
         :math:`z`
         [m]
     z_coarse : float
-        elevation at coarse resolution
+        elevation at coarse resolution, 
         :math:`z_{c}`
         [m]
     lapse : float
-        lapse rate
+        lapse rate, 
         :math:`L`
         [K m-1]
 
     Returns
     -------
     t_air_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a,i}`
         [C]
 
     Notes
     -----
     The input air temperature is specified in Kelvin. The output air
     temperature is specified in C.
     """
     return disaggregate_air_temperature(t_air_i_coarse, z, z_coarse, lapse)
 
 
 def disaggregate_dew_point_temperature_inst(t_dew_coarse_i, z, z_coarse, lapse_dew=-0.002):
     r"""
     Disaggregates geos dew point temperature using lapse rate and difference between
-    smoothed coarse scale DEM and fine scale DEM
+    smoothed coarse scale DEM and fine scale DEM.
 
     Parameters
     ----------
     t_dew_coarse_i : float
-        coarse instantaneous dew point temperature
+        coarse instantaneous dew point temperature, 
         :math:`T_{dew,coarse}`
         [C]
     z : float
-        elevation
+        elevation, 
         :math:`z`
         [m]
     z_coarse : float
-        smoothed elevation at coarse resolution
+        smoothed elevation at coarse resolution, 
         :math:`z`
         [m]
     lapse_dew : float
-        lapse rate
+        lapse rate, 
         :math:`L`
         [K m-1]
 
     Returns
     -------
     t_dew_i : float
-        instantaneous dew point temperature
+        instantaneous dew point temperature, 
         :math:`T_{dew,i}`
         [C]
     """
     return t_dew_coarse_i + ((z - z_coarse) * lapse_dew)
 
 
 def vapour_pressure_from_specific_humidity(qv, p_air):
     r"""
     Computes the vapour pressure :math:`e_a` in [mbar] using specific humidity
-    and surface pressure
+    and surface pressure.
 
     .. math ::
-        e_{a}=\frac{q_{v}P}{\varepsilon}
+
+        e_{a}=\frac{q_{v} \cdot P}{\varepsilon}
 
     where the following constant is used
 
     * :math:`\varepsilon` = ratio of molecular weight of water to
       dry air = 0.622 [-]
 
 
     Parameters
     ----------
     qv : float
-        specific humidity
+        specific humidity, 
         :math:`q_{v}`
         [kg/kg]
     p_air : float
-        air pressure
+        air pressure, 
         :math:`P`
         [mbar]
 
     Returns
     -------
     vp : float
-        vapour pressure
+        vapour pressure, 
         :math:`e_{a}`
         [mbar]
     """
     return (qv * p_air) / c.r_mw
 
+def specific_humidity_from_vapour_pressure(vp, p_air):
+    r"""
+    Computes specific humidity using te vapour pressure :math:`e_a` in [mbar]
+    and surface pressure.
+
+    .. math ::
+
+        e_{a}=\frac{q_{v} \cdot P}{\varepsilon}
+
+    where the following constant is used
+
+    * :math:`\varepsilon` = ratio of molecular weight of water to
+      dry air = 0.622 [-]
+
+
+    Parameters
+    ----------
+    vp : float
+        vapour pressure, 
+        :math:`e_{a}`
+        [mbar]
+    p_air : float
+        air pressure, 
+        :math:`P`
+        [mbar]
+
+    Returns
+    -------
+    qv : float
+        specific humidity, 
+        :math:`q_{v}`
+        [kg/kg]
+    """
+    return (vp * c.r_mw) / p_air
 
 def vapour_pressure_from_specific_humidity_daily(qv_24, p_air_24):
-    """Like :func:`vapour_pressure_from_specific_humidity` but as a daily average
+    """Like :func:`vapour_pressure_from_specific_humidity` but as a daily average.
 
     Parameters
     ----------
     qv_24 : float
-        daily specific humidity
+        daily specific humidity, 
         :math:`q_{v,24}`
         [kg/kg]
     p_air_24 : float
-        daily air pressure
+        daily air pressure, 
         :math:`P_{24}`
         [mbar]
 
     Returns
     -------
     vp_24 : float
-        daily vapour pressure
+        daily vapour pressure, 
         :math:`e_{a,24}`
         [mbar]
     """
     return vapour_pressure_from_specific_humidity(qv_24, p_air_24)
 
 
+def vapour_pressure_from_dewpoint(t_dew):
+    r"""
+    .. math ::
+        e_{a}=6.108\exp\left[\frac{17.27T_{d}}{T_{d}+237.3}\right]
+
+    Parameters
+    ----------
+    t_dew : float
+        dewpoint temperature, 
+        :math:`T_d`
+        [°C]
+
+    Returns
+    -------
+    vp : float
+        vapour pressure, 
+        :math:`e_a`
+        [mbar]
+
+    Examples
+    --------
+    >>> from ETLook import meteo
+    >>> meteo.vapour_pressure_from_dewpoint(20)
+    23.382812709274457
+    """
+
+    return saturated_vapour_pressure(t_dew)
+
+
+def vapour_pressure_from_dewpoint_daily(t_dew_24):
+    r"""
+    .. math ::
+        e_{a}=6.108\exp\left[\frac{17.27T_{d,24}}{T_{d,24}+237.3}\right]
+
+    Parameters
+    ----------
+    t_dew_24 : float
+        dewpoint temperature, 
+        :math:`T_d`
+        [°C]
+
+    Returns
+    -------
+    vp_24 : float
+        vapour pressure, 
+        :math:`e_{a,24}`
+        [mbar]
+
+    Examples
+    --------
+    >>> from ETLook import meteo
+    >>> meteo.vapour_pressure_from_dewpoint_daily(20)
+    23.382812709274457
+    """
+
+    return saturated_vapour_pressure(t_dew_24)
+
+
+def vapour_pressure_from_dewpoint_inst(t_dew_i):
+    r"""
+    .. math ::
+        e_{a,i}=6.108\exp\left[\frac{17.27T_{d,i}}{T_{d,i}+237.3}\right]
+
+    Parameters
+    ----------
+    t_dew_i : float
+        instantaneous dew point temperature, 
+        :math:`T_{dew,i}`
+        [°C]
+
+    Returns
+    -------
+    vp_i : float
+        vapour pressure, 
+        :math:`e_{a,i}`
+        [mbar]
+
+    Examples
+    --------
+    >>> from ETLook import meteo
+    >>> meteo.vapour_pressure_from_dewpoint_inst(20)
+    23.382812709274457
+    """
+
+    return saturated_vapour_pressure(t_dew_i)
+
+
 def saturated_vapour_pressure_minimum(t_air_min_coarse):
     """Like :func:`saturated_vapour_pressure` but based on daily minimum air temperature. This
-    is only relevant for reference ET calculations
+    is only relevant for reference ET calculations.
 
     Parameters
     ----------
     t_air_min_coarse : float
-        daily minimum air temperature
+        daily minimum air temperature, 
         :math:`T_{a,min}`
         [C]
 
     Returns
     -------
     svp_24_min : float
-        daily saturated vapour pressure based on minimum air temperature
+        daily saturated vapour pressure based on minimum air temperature, 
         :math:`e_{s,min}`
         [mbar]
 
     """
     return saturated_vapour_pressure(t_air_min_coarse)
 
 
 def saturated_vapour_pressure_maximum(t_air_max_coarse):
     """Like :func:`saturated_vapour_pressure` but based on daily maximum air temperature. This
-    is only relevant for reference ET calculations
+    is only relevant for reference ET calculations.
 
     Parameters
     ----------
     t_air_max_coarse : float
-        daily maximum air temperature
+        daily maximum air temperature, 
         :math:`T_{a,max}`
         [C]
 
     Returns
     -------
     svp_24_max : float
-        daily saturated vapour pressure based on maximum air temperature
+        daily saturated vapour pressure based on maximum air temperature, 
         :math:`e_{s,max}`
         [mbar]
 
     """
     return saturated_vapour_pressure(t_air_max_coarse)
 
 
 def saturated_vapour_pressure_average(svp_24_max, svp_24_min):
-    """
+    r"""
     Average saturated vapour pressure based on two saturated vapour pressure values
     calculated using minimum and maximum air temperature respectively. This is preferable
     to calculating saturated vapour pressure using the average air temperature, because
     of the strong non-linear relationship between saturated vapour pressure and air
-    temperature
+    temperature.
 
     .. math ::
-        e_{s}=\frac{e^{0}\left(T_{max}\right)+e^{0}\left(T_{mon}\right)}{2}
+
+        e_{s}=\frac{e^{0}\left(T_{max}\right)+e^{0}\left(T_{min}\right)}{2}
 
     Parameters
     ----------
     svp_24_max : float
-        daily saturated vapour pressure based on maximum air temperature
+        daily saturated vapour pressure based on maximum air temperature, 
         :math:`e_{s,max}`
         [mbar]
     svp_24_min : float
-        daily saturated vapour pressure based on minimum air temperature
+        daily saturated vapour pressure based on minimum air temperature, 
         :math:`e_{s,min}`
         [mbar]
 
     Returns
     -------
     svp_24 : float
-        daily saturated vapour pressure
+        daily saturated vapour pressure, 
         :math:`e_{s,24}`
         [mbar]
 
     """
     return (svp_24_max + svp_24_min)/2
 
 
 def vapour_pressure_from_specific_humidity_inst(qv_i, p_air_i):
-    """Like :func:`vapour_pressure_from_specific_humidity` but as an instantaneous value
+    """Like :func:`vapour_pressure_from_specific_humidity` but as an instantaneous value.
 
     Parameters
     ----------
     qv_i : float
-        instantaneous specific humidity
+        instantaneous specific humidity, 
         :math:`q_{v,i}`
         [kg/kg]
     p_air_i : float
-        instantaneous air pressure
+        instantaneous air pressure, 
         :math:`P_{i}`
         [mbar]
 
     Returns
     -------
     vp_i : float
-        instantaneous vapour pressure
+        instantaneous vapour pressure, 
         :math:`e_{a,i}`
         [mbar]
     """
     return vapour_pressure_from_specific_humidity(qv_i, p_air_i)
 
 
 def saturated_vapour_pressure(t_air):
     r"""
-    Computes saturated vapour pressure :math:`e_s` [mbar], it provides 
-    the vapour pressure when the air is fully saturated with water. It is 
-    related to air temperature :math:`T_a` [C]:
+    Computes saturated vapour pressure :math:`e_s` [mbar], it provides
+    the vapour pressure when the air is fully saturated with water. It is
+    related to air temperature :math:`T_a` [C] as:
 
     .. math ::
-        e_{s}=6.108\exp\left[\frac{17.27T_{a}}{T_{a}+237.3}\right]
+
+        e_{s}=6.108 \cdot \exp\left[\frac{17.27 \cdot T_{a}}{T_{a}+237.3}\right]
 
     Parameters
     ----------
     t_air : float
-        air temperature
+        air temperature, 
         :math:`T_a`
         [C]
 
     Returns
     -------
     svp : float
-        saturated vapour pressure
+        saturated vapour pressure, 
         :math:`e_s`
         [mbar]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> meteo.saturated_vapour_pressure(20)
     23.382812709274457
 
     """
     return 6.108 * np.exp(((17.27 * t_air) / (237.3 + t_air)))
 
 
 def saturated_vapour_pressure_daily(t_air_24):
-    """Like :func:`saturated_vapour_pressure` but as a daily average
+    """Like :func:`saturated_vapour_pressure` but as a daily average.
 
     Parameters
     ----------
     t_air_24 : float
-        daily air temperature
+        daily air temperature, 
         :math:`T_{a,24}`
         [C]
 
     Returns
     -------
     svp_24 : float
-        daily saturated vapour pressure
+        daily saturated vapour pressure, 
         :math:`e_{s,24}`
         [mbar]
 
     """
     return saturated_vapour_pressure(t_air_24)
 
 
 def saturated_vapour_pressure_inst(t_air_i):
-    """Like :func:`saturated_vapour_pressure` but as an instantaneous value
+    """Like :func:`saturated_vapour_pressure` but as an instantaneous value.
 
     Parameters
     ----------
     t_air_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a,i}`
         [C]
 
     Returns
     -------
     svp_i : float
-        instantaneous saturated vapour pressure
+        instantaneous saturated vapour pressure, 
         :math:`e_{s,i}`
         [mbar]
 
     """
     return saturated_vapour_pressure(t_air_i)
 
 
 def vapour_pressure(svp, rh):
     r"""
-    Computes the vapour pressure :math:`e_a` in [mbar]
+    Computes the vapour pressure :math:`e_a` in [mbar].
 
     .. math ::
-        e_{a}=\frac{\phi}{100}e_{s}
+
+        e_{a}=\frac{\phi}{100} \cdot e_{s}
 
     Parameters
     ----------
     svp : float
-        saturated vapour pressure
+        saturated vapour pressure, 
         :math:`e_s`
         [mbar]
     rh : float
-        relative humidity
+        relative humidity, 
         :math:`\phi`
         [%]
 
     Returns
     -------
     vp : float
-        vapour pressure
+        vapour pressure, 
         :math:`e_{a}`
         [mbar]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> meteo.vapour_pressure(rh=75, svp=meteo.saturated_vapour_pressure(20))
@@ -564,15 +688,16 @@
     r"""
     Computes the rate of change of vapour pressure :math:`\Delta` in [mbar K-1]
     for a given air temperature :math:`T_a`. It is a function of the air
     temperature :math:`T_a` and the saturated vapour pressure :math:`e_s`
     [mbar] which in itself is a function of :math:`T_a`.
 
     .. math ::
-        \Delta=\frac{4098e_{s}}{\left(237.3+T_{a}\right)^{2}}
+
+        \Delta=\frac{4098 \cdot e_{s}}{\left(237.3+T_{a}\right)^{2}}
 
     for :math:`e_s` see :func:`saturated_vapour_pressure`
 
     Parameters
     ----------
     t_air : float
        air temperature
@@ -594,15 +719,15 @@
 
     """
     svp = saturated_vapour_pressure(t_air)
     return (4098 * svp) / (237.3 + t_air) ** 2
 
 
 def slope_saturated_vapour_pressure_daily(t_air_24):
-    """Like :func:`slope_saturated_vapour_pressure` but as a daily average
+    """Like :func:`slope_saturated_vapour_pressure` but as a daily average.
 
     Parameters
     ----------
     t_air_24 : float
        daily air temperature
        :math:`T_{a,24}`
        [C]
@@ -616,49 +741,50 @@
 
 
     """
     return slope_saturated_vapour_pressure(t_air_24)
 
 
 def slope_saturated_vapour_pressure_inst(t_air_i):
-    """Like :func:`slope_saturated_vapour_pressure` but as an instantaneous
+    """Like :func:`slope_saturated_vapour_pressure` but as an instantaneous.
     value
 
     Parameters
     ----------
     t_air_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a,i}`
         [C]
 
     Returns
     -------
     ssvp_i : float
-        instantaneous slope of saturated vapour pressure curve
+        instantaneous slope of saturated vapour pressure curve, 
         :math:`e_{s,i}`
         [mbar]
     """
     return slope_saturated_vapour_pressure(t_air_i)
 
 
 def vapour_pressure_deficit(svp, vp):
     r"""
-    Computes the vapour pressure deficit :math:`\Delta_e` in [mbar]
+    Computes the vapour pressure deficit :math:`\Delta_e` in [mbar].
 
     .. math ::
+
         \Delta_e=e_s-e_a
 
     Parameters
     ----------
     svp : float
-        saturated vapour pressure
+        saturated vapour pressure, 
         :math:`e_s`
         [mbar]
     vp : float
-        actual vapour pressure
+        actual vapour pressure, 
         :math:`e_a`
         [mbar]
 
     Returns
     -------
     vpd : float
        vapour pressure deficit
@@ -680,24 +806,24 @@
     else:
         vpd[vpd < 0] = 0
 
     return vpd
 
 
 def vapour_pressure_deficit_daily(svp_24, vp_24):
-    """Like :func:`vapour_pressure_deficit` but as a daily average
+    """Like :func:`vapour_pressure_deficit` but as a daily average.
 
     Parameters
     ----------
     svp_24 : float
-        daily saturated vapour pressure
+        daily saturated vapour pressure, 
         :math:`e_{s,24}`
         [mbar]
     vp_24 : float
-        daily actual vapour pressure
+        daily actual vapour pressure, 
         :math:`e_{a,24}`
         [mbar]
 
     Returns
     -------
     vpd_24 : float
        daily vapour pressure deficit
@@ -710,109 +836,111 @@
 def air_pressure(z, p_air_0=1013.25):
     r"""
     Computes air pressure :math:`P` at a certain elevation derived from the
     air pressure at sea level :math:`P_0`. Air pressure decreases with
     increasing elevation.
 
     .. math ::
-        P=P_{0}\left(\frac{T_{ref,0,K}-\alpha_{1}\left(z-z_{0}\right)}
-        {T_{ref,0,K}}\right)^{\frac{g}{\alpha{}_{1^{R}}}}
+
+        P=P_{0} \cdot \left(\frac{T_{ref,0,K}-\alpha_{1} \cdot \left(z-z_{0}\right)}
+        {T_{ref,0,K}}\right)^{\frac{g}{-\alpha_{1}\cdot R }}
 
     where the following constants are used
 
     * :math:`P_0` = air pressure [mbar] at sea level :math:`z_0` = 1013.25 mbar
     * :math:`T_{ref,0,K}` = reference temperature [K] at sea level
       :math:`z_0` = 293.15 K
     * :math:`g` = gravitational acceleration = 9.807 [m/s2]
     * :math:`R` = specific gas constant = 287.0 [J kg-1 K-1]
-    * :math:`\alpha_1` = constant lapse rate for moist air = 0.0065 [K m-1]
+    * :math:`\alpha_{1}` = constant lapse rate for moist air = 0.0065 [K m-1]
 
     Parameters
     ----------
     z : float
-        elevation
+        elevation, 
         :math:`z`
         [m]
     p_air_0 : float
-        air pressure at sea level
+        air pressure at sea level, 
         :math:`P_0`
         [mbar]
 
     Returns
     -------
     p_air : float
-        air pressure
+        air pressure, 
         :math:`P`
         [mbar]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> meteo.air_pressure(z=1000)
     900.5832172948869
 
     """
     return p_air_0 * ((c.t_ref + c.lapse * (z - c.z_ref)) / c.t_ref) ** c.power
 
 
 def air_pressure_daily(z, p_air_0_24=1013.25):
-    r"""Like :func:`air_pressure` but as a daily average
+    r"""Like :func:`air_pressure` but as a daily average.
 
     Parameters
     ----------
     z : float
-        elevation
+        elevation, 
         :math:`z`
         [m]
     p_air_0_24 : float
-        daily air pressure at sea level
+        daily air pressure at sea level, 
         :math:`P_{0,24}`
         [mbar]
 
     Returns
     -------
     p_air_24 : float
-        daily air pressure
+        daily air pressure, 
         :math:`P_{24}`
         [mbar]
 
     """
     return air_pressure(z, p_air_0_24)
 
 
 def dry_air_density(p_air, vp, t_air_k):
     r"""
-    Computes dry air density :math:`\rho_{d}` in [kg m-3]
+    Computes dry air density :math:`\rho_{d}` in [kg m-3].
 
     .. math ::
-        \rho_{d}=\frac{P-e_{a}}{\Re T_{a,K}}
+
+        \rho_{d}=\frac{P-e_{a}}{\Re \cdot T_{a,K}}
 
     where the following constants are used
 
     * :math:`\Re` = gas constant for dry air = 2.87 mbar K-1 m3 kg-1
 
     Parameters
     ----------
     p_air : float
-        air pressure
+        air pressure, 
         :math:`P`
         [mbar]
     vp : float
-        vapour pressure
+        vapour pressure, 
         :math:`e_{a}`
         [mbar]
     t_air_k : float
-        daily air temperature
+        daily air temperature, 
         :math:`T_{a}`
         [K]
 
     Returns
     -------
     ad_dry : float
-        dry air density
+        dry air density, 
         :math:`\rho_{d}`
         [kg m-3]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> meteo.dry_air_density(p_air=900, vp=17.5, t_air_k=293.15)
@@ -820,96 +948,97 @@
 
     """
     return (p_air - vp) / (t_air_k * c.gc_dry)
 
 
 def dry_air_density_daily(p_air_24, vp_24, t_air_k_24):
     r"""
-    Like :func:`dry_air_density` but as a daily average
+    Like :func:`dry_air_density` but as a daily average.
 
     Parameters
     ----------
     p_air_24 : float
-        daily air pressure
+        daily air pressure, 
         :math:`P_{24}`
         [mbar]
     vp_24 : float
-        daily vapour pressure
+        daily vapour pressure, 
         :math:`e_{a,24}`
         [mbar]
     t_air_k_24 : float
-        daily air temperature
+        daily air temperature, 
         :math:`T_{a,24}`
         [K]
 
     Returns
     -------
     ad_dry_24 : float
-        daily dry air density
+        daily dry air density, 
         :math:`\rho_{d,24}`
         [kg m-3]
     """
     return dry_air_density(p_air_24, vp_24, t_air_k_24)
 
 
 def dry_air_density_inst(p_air_i, vp_i, t_air_k_i):
     r"""
-    Like :func:`dry_air_density` but as an instantaneous value
+    Like :func:`dry_air_density` but as an instantaneous value.
 
     Parameters
     ----------
     p_air_i : float
-        instantaneous air pressure
+        instantaneous air pressure, 
         :math:`P_{i}`
         [mbar]
     vp_i : float
-        instantaneous vapour pressure
+        instantaneous vapour pressure, 
         :math:`e_{a,i}`
         [mbar]
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a,i}`
         [K]
 
     Returns
     -------
     ad_dry_i : float
-        instantaneous dry air density
+        instantaneous dry air density, 
         :math:`\rho_{d,i}`
         [kg m-3]
     """
     return dry_air_density(p_air_i, vp_i, t_air_k_i)
 
 
 def moist_air_density(vp, t_air_k):
     r"""
-    Computes moist air density :math:`\rho_{s}` in [kg m-3]
+    Computes moist air density :math:`\rho_{s}` in [kg m-3].
 
     .. math ::
-        \rho_{s}=\frac{e_{a}}{R_{v}T_{a,K}}
 
-    where the following constants are used
+        \rho_{s}=\frac{e_{a}}{R_{v} \cdot T_{a,K}}
+
+    where:
 
     * :math:`R_v` = gas constant for moist air = 4.61 mbar K-1 m3 kg-1
 
     Parameters
     ----------
     vp : float
-        vapour pressure
+        vapour pressure, 
         :math:`e_{a}`
         [mbar]
     t_air_k : float
-        air temperature
+        air temperature, 
         :math:`T_{a,K}`
         [K]
 
     Returns
     -------
     ad_moist : float
-        moist air density
+        moist air density, 
         :math:`\rho_{s}`
         [kg m-3]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> meteo.moist_air_density(vp=17.5, t_air_k = 293.15)
@@ -917,86 +1046,87 @@
 
     """
     return vp / (t_air_k * c.gc_moist)
 
 
 def moist_air_density_daily(vp_24, t_air_k_24):
     r"""
-    Like :func:`moist_air_density` but as a daily average
+    Like :func:`moist_air_density` but as a daily average.
 
     Parameters
     ----------
     vp_24 : float
-        daily vapour pressure
+        daily vapour pressure, 
         :math:`e_{a,24}`
         [mbar]
     t_air_k_24 : float
-        daily air temperature
+        daily air temperature, 
         :math:`T_{a,K,24}`
         [K]
 
     Returns
     -------
     ad_moist_24 : float
-        daily moist air density
+        daily moist air density, 
         :math:`\rho_{s,24}`
         [kg m-3]
 
     """
     return moist_air_density(vp_24, t_air_k_24)
 
 
 def moist_air_density_inst(vp_i, t_air_k_i):
     r"""
-    Like :func:`moist_air_density` but as an instantaneous value
+    Like :func:`moist_air_density` but as an instantaneous value.
 
     Parameters
     ----------
     vp_i : float
-        instantaneous vapour pressure
+        instantaneous vapour pressure, 
         :math:`e_{a,i}`
         [mbar]
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a,K,i}`
         [K]
 
     Returns
     -------
     ad_moist_i : float
-        instantaneous moist air density
+        instantaneous moist air density, 
         :math:`\rho_{s,i}`
         [kg m-3]
 
     """
     return moist_air_density(vp_i, t_air_k_i)
 
 
 def air_density(ad_dry, ad_moist):
     r"""
-    Computes air density :math:`\rho` in [kg m-3]
+    Computes air density :math:`\rho` in [kg m-3].
 
     .. math ::
+
         \rho=\rho_{s}+\rho_{d}
 
     Parameters
     ----------
     ad_dry : float
-        dry air density
+        dry air density, 
         :math:`\rho_{d}`
         [kg m-3]
     ad_moist : float
-        moist air density
+        moist air density, 
         :math:`\rho_{s}`
         [kg m-3]
 
     Returns
     -------
     ad : float
-        air density
+        air density, 
         :math:`\rho`
         [kg m-3]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> ad_moist = meteo.moist_air_density(vp=17.5, t_air_k = 293.15)
@@ -1007,57 +1137,57 @@
     """
     return ad_dry + ad_moist
 
 
 def air_density_daily(ad_dry_24, ad_moist_24):
     r"""
 
-    Like :func:`air_density` but as a daily average
+    Like :func:`air_density` but as a daily average.
 
     Parameters
     ----------
     ad_dry_24 : float
-        daily dry air density
+        daily dry air density, 
         :math:`\rho_{d,24}`
         [kg m-3]
     ad_moist_24 : float
-        daily moist air density
+        daily moist air density, 
         :math:`\rho_{s,24}`
         [kg m-3]
 
     Returns
     -------
     ad_24 : float
-        daily air density
+        daily air density, 
         :math:`\rho_{24}`
         [kg m-3]
 
     """
     return air_density(ad_dry_24, ad_moist_24)
 
 
 def air_density_inst(ad_dry_i, ad_moist_i):
     r"""
-    Like :func:`air_density` but as a instantaneous value
+    Like :func:`air_density` but as a instantaneous value.
 
     Parameters
     ----------
     ad_dry_i : float
-        instantaneous dry air density
+        instantaneous dry air density, 
         :math:`\rho_{d,i}`
         [kg m-3]
     ad_moist_i : float
-        instantaneous moist air density
+        instantaneous moist air density, 
         :math:`\rho_{s,i}`
         [kg m-3]
 
     Returns
     -------
     ad_i : float
-        instantaneous air density
+        instantaneous air density, 
         :math:`\rho_{i}`
         [kg m-3]
 
     """
     return air_density(ad_dry_i, ad_moist_i)
 
 
@@ -1066,214 +1196,210 @@
     Computes latent heat of evaporation :math:`\lambda` [J kg-1], describing
     the amount of energy needed to evaporate one kg of water at constant
     pressure and temperature. At higher temperatures less energy will be
     required than at lower temperatures.
 
     .. math ::
 
-        \lambda=(\lambda_0 + \Delta_\lambda T_{a})
+        \lambda=\lambda_0 + \Delta_\lambda \cdot T_{a}
 
     where the following constants are used
 
     * :math:`\lambda_0` = latent heat of evaporation at 0 C = 2501000 [J kg-1]
     * :math:`\Delta_\lambda` = rate of change of latent heat with respect to temperature = -2361 [J Kg-1 C-1]
 
     Parameters
     ----------
     t_air : float
-        air temperature
+        air temperature, 
         :math:`T_a`
         [C]
 
     Returns
     -------
     lh : float
-        latent heat of evaporation
+        latent heat of evaporation, 
         :math:`\lambda`
         [J/kg]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> meteo.latent_heat(20)
     2453780.0
 
- 
     """
     return c.lh_0 + c.lh_rate * t_air
 
 
 def latent_heat_daily(t_air_24):
-    """Like :func:`latent_heat` but as a daily average
+    """Like :func:`latent_heat` but as a daily average.
 
     Parameters
     ----------
     t_air_24 : float
-        daily air temperature
+        daily air temperature, 
         :math:`T_{a,24}`
         [C]
 
     Returns
     -------
     lh_24 : float
-        daily latent heat of evaporation
+        daily latent heat of evaporation, 
         :math:`\lambda_{24}`
         [J/kg]
 
     """
     return latent_heat(t_air_24)
 
 
 def psychrometric_constant(p_air, lh):
     r"""
     Computes the psychrometric constant :math:`\gamma` [mbar K-1] which
-    relates the partial pressure of water in air to the air temperature
+    relates the partial pressure of water in air to the air temperature.
 
     .. math ::
 
-        \gamma=\frac{Pc_{p}}{\varepsilon\lambda}
+        \gamma=\frac{P \cdot c_{p}}{\varepsilon \cdot \lambda}
 
     where the following constants are used
 
     * :math:`c_{p}` = specific heat for dry air = 1004 [J Kg-1 K-1]
     * :math:`\varepsilon` = ratio of molecular weight of water to
       dry air = 0.622 [-]
 
     Parameters
     ----------
     p_air : float
-        air pressure
+        air pressure, 
         :math:`P`
         [mbar]
     lh : float
-        latent heat of evaporation
+        latent heat of evaporation, 
         :math:`\lambda`
         [J/kg]
 
     Returns
     -------
     psy : float
-        psychrometric constant
+        psychrometric constant, 
         :math:`\gamma`
         [mbar K-1]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> meteo.psychrometric_constant(p_air = 1003.0, lh = 2500000.0)
     0.6475961414790997
     >>> meteo.psychrometric_constant(1003.0, 2500000.0)
     0.6475961414790997
 
- 
-
     """
     return (c.sh * p_air) / (c.r_mw * lh)
 
 
 def psychrometric_constant_daily(p_air_24, lh_24):
-    """Like :func:`psychrometric_constant` but as a daily average
+    """Like :func:`psychrometric_constant` but as a daily average.
 
     Parameters
     ----------
     p_air_24 : float
-        daily air pressure
+        daily air pressure, 
         :math:`P_{24}`
         [mbar]
     lh_24 : float
-        daily latent heat of evaporation
+        daily latent heat of evaporation, 
         :math:`\lambda_{24}`
         [J/kg]
 
     Returns
     -------
     psy_24 : float
-        daily psychrometric constant
+        daily psychrometric constant, 
         :math:`\gamma_{24}`
         [mbar K-1]
 
     """
     return psychrometric_constant(p_air_24, lh_24)
 
 
 def wind_speed_blending_height(u, z_obs=2, z_b=100):
     r"""
     Computes the wind speed at blending height :math:`u_{b}` [m/s] using the
-    logarithmic wind profile
+    logarithmic wind profile.
 
     .. math ::
-        u_{b}=\frac{u_{obs}\ln\left(\frac{z_{b}}{z_{0,m}}\right)}
+
+        u_{b}=\frac{u_{obs} \cdot \ln\left(\frac{z_{b}}{z_{0,m}}\right)}
         {\ln\left(\frac{z_{obs}}{z_{0,m}}\right)}
 
     Parameters
     ----------
     u : float
-        wind speed at observation height
+        wind speed at observation height, 
         :math:`u_{obs}`
         [m/s]
     z_obs : float
-        observation height of wind speed
+        observation height of wind speed, 
         :math:`z_{obs}`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
 
     Returns
     -------
     u_b : float
-        wind speed at blending height
+        wind speed at blending height, 
         :math:`u_{b}`
         [m/s]
 
     Examples
     --------
     >>> from ETLook import meteo
     >>> meteo.wind_speed_blending_height(u=3.0, z_obs=2, z_b=100)
     5.4646162953650572
 
- 
-
     """
 
     z0m = 0.0171
 
     ws = (c.k * u) / np.log(z_obs / z0m) * np.log(z_b / z0m) / c.k
-    
+
     if isinstance(ws, xr.DataArray):
         ws = ws.clip(1, 150)
     else:
-        ws = np.clip(ws, 1, 150)  
+        ws = np.clip(ws, 1, 150)    
 
     return ws
 
 
 def wind_speed_blending_height_daily(u_24, z_obs=2, z_b=100):
-    """Like :func:`wind_speed_blending_height` but as a daily average
+    """Like :func:`wind_speed_blending_height` but as a daily average.
 
     Parameters
     ----------
     u_24 : float
-        daily wind speed at observation height
+        daily wind speed at observation height, 
         :math:`u_{obs,24}`
         [m/s]
     z_obs : float
-        observation height of wind speed
+        observation height of wind speed, 
         :math:`z_{obs}`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
 
     Returns
     -------
     u_b_24 : float
-        daily wind speed at blending height
+        daily wind speed at blending height, 
         :math:`u_{b, 24}`
         [m/s]
 
     """
     return wind_speed_blending_height(u_24, z_obs, z_b)
 
 
@@ -1292,24 +1418,24 @@
     u_24
         Wind speed.
     """
     return np.sqrt(v**2 + u**2)
 
 
 def air_pressure_kpa2mbar(p_air_kpa):
-    """Like :func:`p_air`
+    """Like :func:`p_air`.
 
     Parameters
     ----------
     p_air_kpa : float
-        air pressure
+        air pressure, 
         :math:`Pair_{a}`
         [kpa]
 
     Returns
     -------
     p_air_mbar : float
-        air pressure
+        air pressure, 
         :math:`Pair_{a}`
         [mbar]
     """
     return p_air_kpa * 10
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/neutral.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/neutral.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from pywapor.et_look_dev import constants as c
+from pywapor.et_look_v2_v3 import constants as c
 from numpy import log
 
 
 def initial_soil_aerodynamic_resistance(u_24, z_obs=2):
     r"""
     Computes the aerodynamic resistance for soil without stability corrections
     :math:`r_{a,soil}^{0}`.
 
     .. math ::
 
         r_{a,soil}^{0}=\frac{\ln\left(\frac{z_{obs}}{z_{0,soil}}\right)
-                       \ln\left(\frac{z_{obs}}{0.1z_{0,soil}}\right)}
-                       {k^{2}u_{obs}}
+                       \cdot \ln\left(\frac{z_{obs}}{0.1z_{0,soil}}\right)}
+                       {k^{2} \cdot u_{obs}}
 
 
     where the following constants are used
 
     * :math:`z_{0,soil}` soil roughness = 0.001 [m]
     * :math:`k` = karman constant = 0.41 [-]
 
     The factor 0.1 is the ratio between the surface roughness for momentum and
     heat.
 
     Parameters
     ----------
     u_24 : float
-        daily wind speed at observation height
-        :math:`u_obs`
+        daily wind speed at observation height,
+        :math:`u_{obs}`
         [m/s]
 
     z_obs : float
-        observation height
+        observation height,
         :math:`z_{obs}`
         [m]
 
     Returns
     -------
     ra_soil_init : float
-        aerodynamic resistance without stability corrections
+        aerodynamic resistance without stability corrections, 
         :math:`r_{a,soil}^{0}`
         [s/m]
 
     """
     return (log(z_obs / c.z0_soil) * log(z_obs / (0.1 * c.z0_soil))) / (c.k**2 * u_24)
 
 
@@ -61,50 +61,50 @@
 
     * :math:`c_{p}` specific heat for dry air = 1004 [J kg-1 K-1]
     * :math:`k` = karman constant = 0.41 [-]
 
     Parameters
     ----------
     rn_24_soil : float
-        daily net radiation for soil
+        daily net radiation for soil, 
         :math:`Q_{soil}^{*}`
         [W m-2]
     g0_24 : float
-        daily soil heat flux
+        daily soil heat flux, 
         :math:`G`
         [W m-2]
     ssvp_24 : float
        daily slope of saturated vapour pressure curve
        :math:`\Delta`
        [mbar K-1]
     ad_24 : float
-        daily air density
+        daily air density, 
         :math:`\rho`
         [kg m-3]
     vpd_24 : float
-        daily vapour pressure deficit
+        daily vapour pressure deficit, 
         :math:`\Delta_{e}`
         [mbar]
     psy_24 : float
-        daily psychrometric constant
+        daily psychrometric constant, 
         :math:`\gamma`
         [mbar K-1]
     r_soil : float
-        soil resistance
+        soil resistance, 
         :math:`r_{soil}`
         [m s-1]
     ra_soil_init : float
-        initial soil aerodynamic resistance
+        initial soil aerodynamic resistance, 
         :math:`r_{a,soil}`
         [m s-1]
 
     Returns
     -------
     e_24_init : float
-        initial estimate radiation equivalent daily evaporation
+        initial estimate radiation equivalent daily evaporation, 
         :math:`E^{0}`
         [W m-2]
 
     """
     numerator = (ssvp_24 * (rn_24_soil - g0_24) +
                  ad_24 * c.sh * (vpd_24 / ra_soil_init))
     denominator = (ssvp_24 + psy_24 * (1 + r_soil / ra_soil_init))
@@ -114,77 +114,77 @@
 def initial_daily_evaporation_mm(e_24_init, lh_24):
     r"""
     Computes the soil evaporation based on the Penman Monteith equation
     adapted for soil.
 
     .. math ::
 
-        E^{0}=E^{0}d_{sec}\lambda_{24}
+        E^{0}=E^{0} \cdot d_{sec} \cdot \lambda_{24}
 
     where the following constants are used
 
     * :math:`d_{sec}` seconds in the day = 86400 [s]
 
     Parameters
     ----------
     e_24_init : float
-        initial estimate daily evaporation
+        initial estimate daily evaporation, 
         :math:`E^{0}`
         [W m-2]
     lh_24 : float
-        daily latent heat of evaporation
+        daily latent heat of evaporation, 
         :math:`\lambda_{24}`
         [J/kg]
 
     Returns
     -------
     e_24_init_mm : float
-        initial estimate daily evaporation in mm
+        initial estimate daily evaporation in mm, 
         :math:`E^{0}`
         [mm d-1]
     """
     return e_24_init * c.day_sec / lh_24
 
 
 def initial_canopy_aerodynamic_resistance(u_24, z0m, z_obs=2):
     r"""
     Computes the aerodynamic resistance for a canopy soil without stability
     corrections :math:`r_{a,}^{0}`.
 
     .. math ::
 
-        r_{a,canopy}^{0}=\frac{\ln\left(\frac{z_{obs}}{z_{0,m}}\right)\ln
-        \left(\frac{z_{obs}}{0.1z_{0,m}}\right)}{k^{2}u_{obs}}
+        r_{a,canopy}^{0}=\frac{\ln\left(\frac{z_{obs}}{z_{0,m}}\right) \cdot \ln
+        \left(\frac{z_{obs}}{0.1z_{0,m}}\right)}{k^{2} \cdot u_{obs}}
 
     where the following constants are used
 
     * :math:`k` = karman constant = 0.41 [-]
 
     The factor 0.1 is the ratio between the surface roughness for momentum and
     heat.
 
     Parameters
     ----------
     u_24 : float
-        daily wind speed at observation height
-        :math:`u_obs`
+        daily wind speed at observation height, 
+        :math:`u_{obs}`
         [m/s]
     z0m : float
-        roughness length
+        roughness length, 
         :math:`z_{0,m}`
         [m]
     z_obs : float
-        observation height
+        observation height, 
         :math:`z_{obs}`
         [m]
 
     Returns
     -------
     ra_canopy_init : float
-        canopy resistance without stability corrections
+        canopy resistance without stability corrections, 
         :math:`r_{a,canopy}^{0}`
         [s/m]
     """
     return (log(z_obs / z0m) * log(z_obs / (0.1 * z0m))) / (c.k**2 * u_24)
 
 
 def initial_daily_transpiration(rn_24_canopy, ssvp_24, ad_24, vpd_24,
@@ -204,46 +204,46 @@
 
     * :math:`c_{p}` specific heat for dry air = 1004 [J kg-1 K-1]
     * :math:`k` = karman constant = 0.41 [-]
 
     Parameters
     ----------
     rn_24_canopy : float
-        daily net radiation for the canopy
+        daily net radiation for the canopy, 
         :math:`Q_{soil}^{*}`
         [W m-2]
     ssvp_24 : float
        daily slope of saturated vapour pressure curve
        :math:`\Delta`
        [mbar K-1]
     ad_24 : float
-        daily air density
+        daily air density, 
         :math:`\rho`
         [kg m-3]
     vpd_24 : float
-        daily vapour pressure deficit
+        daily vapour pressure deficit, 
         :math:`\Delta_{e}`
         [mbar]
     psy_24 : float
-        daily psychrometric constant
+        daily psychrometric constant, 
         :math:`\gamma`
         [mbar K-1]
     r_canopy : float
-        canopy resistance
+        canopy resistance, 
         :math:`r_{canopy}`
         [m s-1]
     ra_canopy_init : float
-        initial canopy aerodynamic resistance
+        initial canopy aerodynamic resistance, 
         :math:`r_{a,canopy}`
         [m s-1]
 
     Returns
     -------
     t_24_init : float
-        initial estimate radiation equivalent daily transpiration
+        initial estimate radiation equivalent daily transpiration, 
         :math:`T^{0}`
         [W m-2]
     """
     numerator = (ssvp_24 * rn_24_canopy + ad_24 *
                  c.sh * (vpd_24 / ra_canopy_init))
     denominator = (ssvp_24 + psy_24 * (1 + r_canopy / ra_canopy_init))
     return numerator / denominator
@@ -252,32 +252,32 @@
 def initial_daily_transpiration_mm(t_24_init, lh_24):
     r"""
     Computes the canopy transpiration based on the Penman Monteith equation
     adapted for canopy.
 
     .. math ::
 
-        T^{0}=T^{0}d_{sec}\lambda_{24}
+        T^{0}=T^{0} \cdot d_{sec} \cdot \lambda_{24}
 
     where the following constants are used
 
     * :math:`d_{sec}` seconds in the day = 86400 [s]
 
     Parameters
     ----------
     t_24_init : float
-        initial estimate daily transpiration
+        initial estimate daily transpiration, 
         :math:`E^{0}`
         [W m-2]
     lh_24 : float
-        daily latent heat of evaporation
+        daily latent heat of evaporation, 
         :math:`\lambda_{24}`
         [J/kg]
 
     Returns
     -------
     t_24_init_mm : float
-        initial estimate daily transpiration in mm
+        initial estimate daily transpiration in mm, 
         :math:`T^{0}`
         [mm d-1]
     """
     return t_24_init * c.day_sec / lh_24
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/radiation.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/radiation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import numpy as np
-from pywapor.et_look_dev import constants as c
+from pywapor.et_look_v2_v3 import constants as c
 import xarray as xr
 
 def interception_wm2(int_mm, lh_24):
     r"""
     Computes the energy equivalent for the interception in Wm-2 if it
     is provide in mm/day
 
     .. math ::
-        I = \frac{\lambda I^*}{86400}
+
+        I = \frac{\lambda \cdot I^*}{86400}
 
     Parameters
     ----------
     int_mm : float
-        interception
+        interception, 
         :math:`I^*`
         [mm day-1]
 
     lh_24 : float
-        daily latent heat for evaporation
+        daily latent heat for evaporation, 
         :math:`\lambda`
         [J kg-1]
 
     Returns
     -------
     int_wm2 : float
-        interception
+        interception, 
         :math:`I`
         [W m-2]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> import ETLook.meteo as meteo
@@ -44,27 +45,28 @@
 def soil_fraction(lai):
     r"""
     Computes the effect of the vegetation has in separating the net radiation
     into a soil and canopy component. If the canopy has a full cover almost
     no radiation reaches the soil.
 
     .. math ::
-        s_f = \exp\left(-0.6*I_{lai}\right)
+
+        s_f = \exp^{-0.6 \cdot I_{lai}}
 
     Parameters
     ----------
     lai : float
-        leaf area index
+        leaf area index, 
         :math:`I_{lai}`
         [-]
 
     Returns
     -------
     sf_soil : float
-        soil fraction
+        soil fraction, 
         :math:`s_f`
         [-]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.soil_fraction(3.0)
@@ -76,41 +78,42 @@
 def longwave_radiation_fao_etref(t_air_k_24, vp_24, trans_24):
     r"""
     Computes the net longwave radiation according to the FAO 56 manual. For the
     reference ET calculation the values for vp_slope, vp_offset, lw_slope and
     lw_offset are being provided as defaults
 
     .. math ::
-        L^{*}=\sigma\left(T_{a,K}\right)^{4}
-        \left(vp_off-vp_slp\sqrt{0.1e_{a}}
-        \right)\left(lw_slp\frac{\tau}{0.75}+lw_off\right)
+
+        L^{*}=\sigma\left(T_{a,K}\right)^{4} \cdot
+        \left(vp_{off}-vp_{slope}\sqrt{0.1e_{a}} \cdot 
+        \right)\left(lw_{slope}\frac{\tau}{0.75}+lw_{off}\right)
 
     where the following constant is used
 
     * :math:`\sigma` = Stefan Boltzmann constant = 5.67 e-8 J s-1 m-2 K-4
 
     Parameters
     ----------
     t_air_k_24 : float
-        daily air temperature in Kelvin
+        daily air temperature in Kelvin, 
         :math:`T_{a,K}`
         [-]
     vp_24 : float
-        daily vapour pressure
+        daily vapour pressure, 
         :math:`e_{a}`
         [mbar]
     trans_24 : float
-        daily atmospheric transmissivity
+        daily atmospheric transmissivity, 
         :math:`\tau`
         [-]
 
     Returns
     -------
     l_net : float
-        daily net longwave radiation
+        daily net longwave radiation, 
         :math:`L^{*}`
         [Wm-2]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.longwave_radiation_fao_etref(t_air_k=302.5, vp=10.3, trans_24=0.6)
@@ -126,57 +129,58 @@
 
 def longwave_radiation_fao(t_air_k_24, vp_24, trans_24, vp_slope=0.14, vp_offset=0.34,
                            lw_slope=1.35, lw_offset=-0.35):
     r"""
     Computes the net longwave radiation according to the FAO 56 manual.
 
     .. math ::
+
         L^{*}=\sigma\left(T_{a,K}\right)^{4}
         \left(vp_{off}-vp_{slope}\sqrt{0.1e_{a}}
         \right)\left(lw_{slope}\frac{\tau}{0.75}+lw_{off}\right)
 
     where the following constant is used
 
     * :math:`\sigma` = Stefan Boltzmann constant = 5.67 e-8 J s-1 m-2 K-4
 
     Parameters
     ----------
     t_air_k_24 : float
-        daily air temperature in Kelvin
+        daily air temperature in Kelvin, 
         :math:`T_{a,K}`
         [-]
     vp_24 : float
-        daily vapour pressure
+        daily vapour pressure, 
         :math:`e_{a}`
         [mbar]
     trans_24 : float
-        daily atmospheric transmissivity
+        daily atmospheric transmissivity, 
         :math:`\tau`
         [-]
     vp_slope : float
-        slope of the vp-term in the FAO-56 longwave radiation relationship
+        slope of the vp-term in the FAO-56 longwave radiation relationship, 
         :math:`vp_{slope}`
         [-]
     vp_offset : float
-        offset of the vp-term in the FAO-56 longwave radiation relationship
+        offset of the vp-term in the FAO-56 longwave radiation relationship, 
         :math:`vp_{off}`
         [-]
     lw_slope : float
-        slope of the tau-term in the FAO-56 longwave radiation relationship
+        slope of the tau-term in the FAO-56 longwave radiation relationship, 
         :math:`lw_{slope}`
         [-]
     lw_offset : float
-        offset of the tau-term in the FAO-56 longwave radiation relationship
+        offset of the tau-term in the FAO-56 longwave radiation relationship, 
         :math:`lw_{off}`
         [-]
 
     Returns
     -------
     l_net : float
-        daily net longwave radiation
+        daily net longwave radiation, 
         :math:`L^{*}`
         [Wm-2]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.longwave_radiation_fao(t_air_k=302.5, vp=10.3, trans_24=0.6)
@@ -187,75 +191,75 @@
 
 
 def net_radiation(r0, ra_24, l_net, int_wm2):
     r"""
     Computes the net radiation
 
     .. math ::
+
         Q^{*} = \left[\left(1-\alpha_{0}\right)S^{\downarrow}-L^{*}-I\right]
 
     Parameters
     ----------
     r0 : float
-        albedo
+        albedo, 
         :math:`\alpha_{0}`
         [-]
     ra_24 : float
-        daily solar radiation
+        daily solar radiation, 
         :math:`S^{\downarrow}`
         [Wm-2]
     l_net : float
-        daily net longwave radiation
+        daily net longwave radiation, 
         :math:`L^{*}`
         [wm-2]
     int_wm2 : float
-        interception
+        interception, 
         :math:`I`
         [Wm-2]
 
     Returns
     -------
     rn_24 : float
-        daily net radiation
+        daily net radiation, 
         :math:`Q^{*}`
         [Wm-2]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.net_radiation(r0=0.10, ra_24=123., l_net=24., int_wm2=0)
     86.7
     """
-    rn_24 = (1-r0)*ra_24-l_net-int_wm2
-    rn_24 = rn_24.clip(20, 2000)
-    return rn_24
+    return (1-r0)*ra_24-l_net-int_wm2
 
 
 def net_radiation_canopy(rn_24, sf_soil):
     r"""
     Computes the net radiation for the canopy
 
     .. math ::
+
         Q^{*}_{canopy} = \left(1-s_f\right) Q^{*}
 
     Parameters
     ----------
     rn_24 : float
-        net radiation
+        net radiation, 
         :math:`Q^{*}`
         [Wm-2]
     sf_soil : float
-        soil fraction
+        soil fraction, 
         :math:`s_f`
         [-]
 
     Returns
     -------
     rn_24_canopy : float
-        net radiation for the canopy
+        net radiation for the canopy, 
         :math:`Q^{*}_{canopy}`
         [Wm-2]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.net_radiation_canopy(rn_24=200, sf_soil=0.4)
@@ -266,31 +270,32 @@
 
 
 def net_radiation_soil(rn_24, sf_soil):
     """
     Computes the net radiation for the soil
 
     .. math ::
-        Q^{*}_{soil} = s_f Q^{*}
+
+        Q^{*}_{soil} = s_f \cdot Q^{*}
 
     Parameters
     ----------
     rn_24 : float
-        net radiation
+        net radiation, 
         :math:`Q^{*}`
         [Wm-2]
     sf_soil : float
-        soil fraction
+        soil fraction, 
         :math:`s_f`
         [-]
 
     Returns
     -------
     rn_24_soil : float
-        net radiation for the soil
+        net radiation for the soil, 
         :math:`Q^{*}_{soil}`
         [Wm-2]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.net_radiation_soil(rn_24=200, sf_soil=0.4)
@@ -300,35 +305,36 @@
 
 
 def net_radiation_grass(ra_24, l_net, r0_grass=0.23):
     r"""
     Computes the net radiation for reference grass
 
     .. math ::
+
         Q^{*} = \left[\left(1-\alpha_{0, grass}\right)S^{\downarrow}-L^{*}-I\right]
 
     Parameters
     ----------
     ra_24 : float
-        daily solar radiation
+        daily solar radiation, 
         :math:`S^{\downarrow}`
         [Wm-2]
     l_net : float
-        daily net longwave radiation
+        daily net longwave radiation, 
         :math:`L^{*}`
         [wm-2]
     r0_grass : float
-        albedo for reference grass
+        albedo for reference grass, 
         :math:`\alpha_{0, grass}`
         [-]
 
     Returns
     -------
     rn_24_grass : float
-        daily net radiation for reference grass
+        daily net radiation for reference grass, 
         :math:`Q^{*}`
         [Wm-2]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.net_radiation_grass(ra_24=123., l_net=24.)
@@ -338,32 +344,33 @@
 
 
 def volumetric_heat_capacity(se_top=1.0, porosity=0.4):
     r"""
     Computes the volumetric heat capacity of the soil
 
     .. math ::
-        \rho c_{p}=10e^{6}\left[\left(1-\phi\right)^{2}+
-        2.5\phi+4.2\phi S_{e,top}\right]
+
+        \rho c_{p}=10^{6} \cdot \left[\left(1-\phi\right)^{2}+
+        2.5 \cdot \phi+4.2 \cdot \phi \cdot S_{e,top}\right]
 
     Parameters
     ----------
     se_top : float
-        effective saturation of the topsoil
+        effective saturation of the topsoil, 
         :math:`S_{e,top}`
         [-]
     porosity : float
-        porosity of the soil
+        porosity of the soil, 
         :math:`\phi`
         [-]
 
     Returns
     -------
     vhc : float
-        volumetric heat capacity
+        volumetric heat capacity, 
         :math:`\rho c_{p}`
         [J m-3 K-1]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.volumetric_heat_capacity(se_top=0.4, porosity = 0.5)
@@ -373,27 +380,28 @@
 
 
 def soil_thermal_conductivity(se_top):
     r"""
     Computes the soil thermal conductivity
 
     .. math ::
-        k=0.15+18.5S_{e,top}
+
+        k=0.15+18.5 \cdot S_{e,top}
 
     Parameters
     ----------
     se_top : float
-        effective saturation of the topsoil
+        effective saturation of the topsoil, 
         :math:`S_{e,top}`
         [-]
 
     Returns
     -------
     stc : float
-        soil thermal conductivity
+        soil thermal conductivity, 
         :math:`k`
         [W m-1 K-1]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.soil_thermal_conductivity(se_top=0.4)
@@ -403,35 +411,36 @@
 
 
 def damping_depth(stc, vhc):
     r"""
     Computes the damping depth
 
     .. math ::
+
         z_{d}=\sqrt{\frac{2kP}{2\pi\rho c_{p}}}
 
     with the following constant
 
     * :math:`P` period (seconds within a year)
 
     Parameters
     ----------
     stc : float
-        soil thermal conductivity
+        soil thermal conductivity, 
         :math:`k`
         [W m-1 K-1]
     vhc : float
-        volumetric heat capacity
+        volumetric heat capacity, 
         :math:`\rho c_{p}`
         [J m-3 K-1]
 
     Returns
     -------
     dd : float
-        damping depth
+        damping depth, 
         :math:`z_{d}`
         [m]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.damping_depth(stc=0.9, vhc=volumetric_heat_capacity())
@@ -442,51 +451,52 @@
 
 #TODO north-south transition with regard to latitude
 def bare_soil_heat_flux(doy, dd, stc, t_amp_year, lat):
     r"""
     Computes the bare soil heat flux
 
     .. math ::
-        G_{0}=\frac{\sqrt{2}A_{t,year}k\sin\left(\frac{2\pi J}{P}-
+
+        G_{0}=\frac{\sqrt{2} \cdot A_{t,year} \cdot k \cdot \sin\left(\frac{2\pi \cdot J}{P}-
               \frac{\pi}{4}\right)}{z_{d}}
 
     where the following constant is used
 
     * :math:`P` period (seconds within a year)
 
     The term :math:`-\frac{\pi}{4}` is a phase shift for northern latitudes.
     For southern latitudes the phase shift will be :math:`-\frac{\pi}{4}+\pi`
 
     Parameters
     ----------
     stc : float
-        soil thermal conductivity
+        soil thermal conductivity, 
         :math:`k`
         [W m-1 K-1]
     dd : float
-        damping depth
+        damping depth, 
         :math:`z_{d}`
         [m]
     t_amp_year : float
-        yearly air temperature amplitude
+        yearly air temperature amplitude, 
         :math:`A_{t,year}`
         [m]
     doy : float
-        julian day of the year
+        julian day of the year, 
         :math:`J`
         [-]
     lat : float
-        latitude
+        latitude, 
         :math:`\lambda`
         [rad]
 
     Returns
     -------
     g0_bs : float
-        bare soil heat flux
+        bare soil heat flux, 
         :math:`G_{0}`
         [m]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> stc = rad.soil_thermal_conductivity(se_top=1.0)
@@ -507,59 +517,60 @@
 
 
 def soil_heat_flux(g0_bs, sf_soil, land_mask, rn_24_soil, trans_24, ra_24, l_net, rn_slope=0.92, rn_offset=-61.0):
     r"""
     Computes the soil heat flux
 
     .. math ::
-        G=s_f G_{0}
+
+        G=s_f \cdot G_{0}
 
     Parameters
     ----------
     g0_bs : float
-        bare soil heat flux
+        bare soil heat flux, 
         :math:`G_{0}`
         [W m-2]
     sf_soil : float
-        soil fraction
+        soil fraction, 
         :math:`s_f`
         [-]
     land_mask : int
-        land use classification
+        land use classification, 
         :math:`l`
         [-]
     rn_24_soil : float
-        net radiation for the soil
+        net radiation for the soil, 
         :math:`Q^{*}_{soil}`
         [Wm-2]
     trans_24 : float
-        daily atmospheric transmissivity
+        daily atmospheric transmissivity, 
         :math:`\tau`
         [-]
     rn_slope : float
-        slope rn/g0 relation water
+        slope rn/g0 relation water, 
         :math:`lws`
         [-]
     rn_offset : float
-        offset rn/g0 relation water
+        offset rn/g0 relation water, 
         :math:`lwo`
         [-]
     ra_24 : float
-        daily solar radiation
+        daily solar radiation, 
         :math:`S^{\downarrow}`
         [Wm-2]
     l_net : float
-        daily net longwave radiation
+        daily net longwave radiation, 
         :math:`L^{*}`
         [wm-2]
 
     Returns
     -------
     g0_24 : float
-        daily soil heat flux
+        daily soil heat flux, 
         :math:`G`
         [W m-2]
 
     Examples
     --------
     >>> import ETLook.radiation as rad
     >>> rad.soil_heat_flux(g0_bs=12.4, sf_soil=0.4)
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/resistance.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/resistance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 import numpy as np
 import xarray as xr
 
 def atmospheric_canopy_resistance(lai_eff, stress_rad, stress_vpd,
                                   stress_temp, rs_min=70, rcan_max=1000000.):
     r"""
-    Computes canopy resistance excluding soil moisture stress
+    Computes canopy resistance excluding soil moisture stress.
 
     .. math ::
-        r_{canopy,0}=\left(\frac{r_{s,min}}{I_{lai,eff}}\right)
-        \left(\frac{1}{S_{T}S_{V}S_{r}}\right)
+
+        r_{canopy,0}=\left(\frac{r_{s,min}}{I_{lai, eff}}\right)\cdot
+        \left(\frac{1}{S_{T} \cdot S_{V} \cdot S_{r}}\right)
 
     Parameters
     ----------
     lai_eff : float
-        effective leaf area index
+        effective leaf area index, 
         :math:`I_{lai,eff}`
         [-]
     stress_temp : float
-        stress factor for air temperature
+        stress factor for air temperature, 
         :math:`S_{t}`
         [-]
     stress_vpd : float
-        stress factor for vapour pressure deficit
+        stress factor for vapour pressure deficit, 
         :math:`S_{v}`
         [-]
     stress_rad : float
-        stress factor for radiation
+        stress factor for radiation, 
         :math:`S_{r}`
         [-]
     rs_min : float
-        Minimal stomatal resistance
+        Minimal stomatal resistance, 
         :math:`r_{s_min}`
         [sm-1]
     rcan_max : float
-        Maximum stomatal resistance
+        Maximum stomatal resistance, 
         :math:`r_{can_max}`
         [sm-1]
 
     Returns
     -------
     r_canopy_0 : float
-        atmospheric canopy resistance
+        atmospheric canopy resistance, 
         :math:`r_{canopy,0}`
         [sm-1]
 
     Examples
     --------
     >>> import ETLook.resistance as res
     >>> res.atmospheric_canopy_resistance(0.9, 0.4, 0.9, 0.94)
@@ -61,38 +62,39 @@
         r_canopy_0[max_mask] = rcan_max
 
     return r_canopy_0
 
 
 def canopy_resistance(r_canopy_0, stress_moist, rcan_max=1000000.):
     r"""
-    Computes canopy resistance
+    Computes canopy resistance.
 
     .. math ::
+
         r_{canopy}=\frac{r_{canopy,0}}{S_{m}}
 
     Parameters
     ----------
     r_canopy_0 : float
-        Atmospheric canopy resistance
+        Atmospheric canopy resistance, 
         :math:`r_{canopy_0}`
         [sm-1]
     stress_moist : float
-        stress factor for root zone soil moisture
+        stress factor for root zone soil moisture, 
         :math:`S_{m}`
         [-]
     rcan_max : float
-        Maximum stomatal resistance
+        Maximum stomatal resistance, 
         :math:`r_{can_max}`
         [sm-1]
 
     Returns
     -------
     r_canopy : float
-        canopy resistance
+        canopy resistance, 
         :math:`r_{canopy}`
         [sm-1]
 
     Examples
     --------
     >>> import ETLook.resistance as res
     >>> res.canopy_resistance(218, 0.8)
@@ -103,78 +105,54 @@
         r_canopy = xr.where(stress_moist == 0, rcan_max, r_canopy_0/stress_moist)
     else:
         r_canopy = np.where(stress_moist == 0, rcan_max, r_canopy_0/stress_moist)
 
     return r_canopy
 
 
-def unstressed_canopy_resistance(r_canopy, stress_moist):
-    """Adjust the canopy resistance for a theoretical absence of 
-    moisture stress.
-
-    Parameters
-    ----------
-    r_canopy : float
-        canopy resistance
-        :math:`r_{canopy}`
-        [sm-1]
-    stress_moist : float
-        stress factor for root zone soil moisture
-        :math:`S_{m}`
-        [-]
-
-    Returns
-    -------
-    r_canopy_unstressed : float
-        adjusted canopy resistance
-        :math:`r_{canopy}`
-        [sm-1]
-    """
-    return r_canopy * stress_moist
-
 def soil_resistance(se_top, land_mask=1, r_soil_pow=-2.1, r_soil_min=800):
     r"""
-    Computes soil resistance
+    Computes soil resistance.
 
     .. math ::
-        r_{soil}=r_{soil,min}\left(S_{e,top}\right)^{a}
+
+        r_{soil}=r_{soil, min}\cdot \left(S_{e,top}\right)^{a}
 
     Parameters
     ----------
     r_soil_min : float
-        Minimum soil resistance
+        Minimum soil resistance, 
         :math:`r_{soil,min}`
         [sm-1]
     se_top : float
-        Top soil effective saturation
+        Top soil effective saturation, 
         :math:`S_{e,top}`
         [-]
     r_soil_pow : float
-        Power soil resistance function
+        Power soil resistance function, 
         :math:`a`
         [-]
     land_mask : int
-        land use classification
+        land use classification, 
         :math:`l`
         [-]
 
     Returns
     -------
     r_soil : float
-        soil resistance
+        soil resistance, 
         :math:`r_{soil}`
         [sm-1]
 
     Examples
     --------
     >>> import ETLook.resistance as res
     >>> res.soil_resistance(se_top=0.9)
     998.1153098304111
     """
-    se_top = np.minimum(0.5, se_top)
     if isinstance(land_mask, xr.DataArray):
         res = xr.ones_like(land_mask) * r_soil_min * se_top ** r_soil_pow
         res = xr.where(land_mask == 2, 0, res)
     else:
         res = np.ones(land_mask.shape) * r_soil_min * se_top ** r_soil_pow
         res[land_mask == 2] = 0
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/roughness.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/roughness.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,31 @@
 """
-    The roughness module contains all functions related to surface roughness
+    The roughness module contains all functions related to surface roughness.
 
 """
 import numpy as np
 import xarray as xr
+from pywapor.general.processing_functions import calc_dlat_dlon
+from pywapor.enhancers.dem import calc_slope
 
-def orographic_roughness(slope, dem_resolution=250.0):
-    r"""
-    Computes the orographic roughness, which is a function of the slope of the
-    terrain. Steeper slopes will increase the orographic roughness
-
-    .. math ::
-        z_{oro}=0.002\left(\frac{\left(x_{res}\frac{\Delta}{100}\right)}
-        {x_{res}}^{2}\right)
-
-    Parameters
-    ----------
-    slope : float
-        slope
-        :math:`\Delta`
-        [rad]
-    dem_resolution : float
-        resolution of dem
-        :math:`x_{res}`
-        [m]
-
-    Returns
-    -------
-    z_oro : float
-        orographic roughness
-        :math:`z_{oro}`
-        [m]
+def orographic_roughness(z, x, y):
 
-    """
+    dlat, dlon = calc_dlat_dlon(None, None, None, (y.values, x.values))            
+    dem_resolution = np.nanmedian(np.nanmean([dlat, dlon], axis = 0))
+    slope_per = np.tan(calc_slope(z.to_dataset(), "slope")["slope"])
+    z_oro = 0.002 * (((dem_resolution * slope_per)**2) / dem_resolution)
 
-    slope_per = np.tan(slope)
-    return 0.002*(((dem_resolution*slope_per)**2)/dem_resolution)
+    return z_oro
 
 def roughness_length(lai, z_oro, z_obst, z_obst_max, land_mask=1):
     r"""
     Computes the surface roughness length. The roughness length is related to
     the roughness characteristics. For the logarithmic wind-profile the
     surface roughness length is the height at which the wind speed is zero.
-    The roughness length is calculated differently for different types of land use
+    The roughness length is calculated differently for different types of land use.
 
     Land use is classified as follows:
 
     0. no data
     1. land
     2. water
     3. urban
@@ -54,64 +33,64 @@
     .. math ::
 
         z_{0,m}=\begin{cases}
         \begin{array}{cc}
         0 & l=0\\
         z_{0,m} & l=1\\
         0.0001 & l=2\\
-        \frac{1}{7}z_{obst,max}+z_{oro} & l=3
+        \frac{1}{7} \cdot z_{obst,max}+z_{oro} & l=3
         \end{array}\end{cases}
 
 
     Parameters
     ----------
     lai : float
-        leaf area index
+        leaf area index, 
         :math:`I_{lai}`
         [-]
     z_oro : float
-        orographic roughness
+        orographic roughness, 
         :math:`z_{oro}`
         [m]
     z_obst : float
-        obstacle height
+        obstacle height, 
         :math:`z_{obst}`
         [m]
     z_obst_max : float
-        maximum obstacle height
+        maximum obstacle height, 
         :math:`z_{obst,max}`
         [m]
     land_mask : int
-        land use classification
+        land use classification, 
         :math:`l`
         [-]
 
     Returns
     -------
     z0m : float
-        roughness length
+        roughness length, 
         :math:`z_{0,m}`
         [m]
 
     Examples
     --------
     >>> import ETLook.roughness as roughness
     >>> roughness.roughness_length(0.4)
     0.34179999999999999
 
     """
 
-    def veg_roughness(zo, d, zo_max, l, oro):
+    def veg_roughness(z_obst, disp, z_obst_max, lai, z_oro):
         veg = 0.193
-        z_dif = zo-d
+        z_dif = z_obst-disp
 
-        term1 = np.minimum(0.41**2/((np.log(z_dif/(0.002*zo_max))+veg)**2), 1.0) + 0.35*l/2
+        term1 = np.minimum(0.41**2/((np.log(z_dif/(0.002*z_obst_max))+veg)**2), 1.0) + 0.35*lai/2
         term2 = np.exp(0.41/np.minimum(np.sqrt(term1), 0.3)-veg)
 
-        return z_dif/term2+oro
+        return z_dif/term2+z_oro
 
     # roughness length specific displacement height
     disp = z_obst * (1 - (1 - np.exp(-np.sqrt(12 * lai))) / (np.sqrt(12 * lai)))
     if isinstance(disp, xr.DataArray):
         disp = xr.where(lai == 0, 0.0, disp)
     else:
         disp[lai == 0] = 0
@@ -148,38 +127,38 @@
         I_{ndvi}>I_{ndvi,obs,min}\&I_{ndvi}<I_{ndvi,obs,max}\\
         z_{obst,max} & I_{ndvi}\geq I_{ndvi,obs,max}
         \end{array}\end{cases}
 
     Parameters
     ----------
     ndvi : float
-        normalized difference vegetation index
+        normalized difference vegetation index, 
         :math:`I_{ndvi}`
         [-]
     ndvi_obs_min : float
-        normalized difference vegetation index @ min obstacle height
+        normalized difference vegetation index @ min obstacle height, 
         :math:`I_{ndvi,obs,min}`
         [-]
     ndvi_obs_max : float
-        normalized difference vegetation index @ max obstacle height
+        normalized difference vegetation index @ max obstacle height, 
         :math:`I_{ndvi,obs,max}`
         [-]
     obs_fr : float
-        ratio of minimum and maximum obstacle height
+        ratio of minimum and maximum obstacle height, 
         :math:`f_{obs}`
         [-]
     z_obst_max : float
         maximum obstacle height
         :math`z_{obst,max}`
         [m]
 
     Returns
     -------
     z_obst : float
-        obstacle height
+        obstacle height, 
         :math:`z_{obst}`
         [m]
 
     Examples
     --------
     >>> import ETLook.roughness as roughness
     >>> roughness.obstacle_height(0.4, 2.0)
@@ -216,55 +195,55 @@
     3. urban
 
     .. math ::
 
         z_{disp}=\begin{cases}
         \begin{array}{cc}
         0 & l=0\\
-        z_{obst}\left(1-\frac{1-\exp\left(-\sqrt{c_{1}I_{lai}}\right)}
-        {\sqrt{c_{1}I_{lai}}}\right) & l=1\\
+        z_{obst}\left(1-\frac{1-\exp\left(-\sqrt{c_{1} \cdot I_{lai}}\right)}
+        {\sqrt{c_{1} \cdot I_{lai}}}\right) & l=1\\
         0 & l=2\\
-        \frac{2}{3}z_{obst} & l=3
+        \frac{2}{3} \cdot z_{obst} & l=3
         \end{array}\end{cases}
 
     Parameters
     ----------
     lai : float
-        leaf area index
+        leaf area index, 
         :math:`I_{lai}`
         [-]
     z_obst : float
-        obstacle height
+        obstacle height, 
         :math:`z_{obst}`
         [m]
     land_mask : int
-        land use classification
+        land use classification, 
         :math:`l`
         [-]
     c1 : float
-        exponential growth rate displacement height function
+        exponential growth rate displacement height function, 
         :math:`c_1`
         [-]
 
 
     Returns
     -------
     disp : float
-        displacement height
+        displacement height, 
         :math:`{disp}`
         [m]
 
     Examples
     --------
     >>> import ETLook.roughness as roughness
     >>> roughness.displacement_height(0.4, 2.0)
     0.51779495
 
     """
-    lai = np.clip(lai, 0.001, np.inf)
+
     def disp_func(l):
         return z_obst * (1-(1-np.exp(-np.sqrt(c1*l)))/np.sqrt(c1*l))
 
     if isinstance(land_mask, xr.DataArray):
         disp = xr.zeros_like(land_mask)
         disp = xr.where(land_mask == 1, disp_func(lai), disp)
         disp = xr.where(land_mask == 2, 0, disp)
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/soil_moisture.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/soil_moisture.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,117 +1,94 @@
 """
-    The soil_moisture module contains all functions related to soil moisture data components.
+    The soil_moisture module contains all functions related to soil moisture data components,
+    as outlined by :footcite:t:`yang2015estimation`.
 
 """
-from pywapor.et_look_dev import constants as c
-from pywapor.et_look_dev import unstable
+from pywapor.et_look_v2_v3 import constants as c
+from pywapor.et_look_v2_v3 import unstable
 import numpy as np
 import xarray as xr
 
 
-def wet_bulb_temperature_inst(t_air_i, t_dew_i, p_air_i):
+def wet_bulb_temperature_inst(t_air_i, t_dew_i):
     r"""
     Computes the instantaneous wet bulb temperature.
 
     Parameters
     ----------
     t_air_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a}`
         [C]
     t_dew_i : float
-        instantaneous dew point temperature
+        instantaneous dew point temperature, 
         :math:`Td_{a}`
         [C]
 
     Returns
     -------
     t_wet_i : float
-        instantaneous wet bulb temperature
+        instantaneous wet bulb temperature, 
         :math:`Tw_{a}`
         [C]
     """
-    tw = wetbulb_temperature_iter(t_air_i, t_dew_i, p_air_i)
+    tw = wetbulb_temperature_iter(t_air_i, t_dew_i)
 
     return tw
 
 def wet_bulb_temperature_inst_new(t_air_i, qv_i, p_air_i):
     r"""
-    Computes the instantaneous wet bulb temperature.
+    Computes the instantaneous wet bulb temperature based on Stull, Roland. "Wet-bulb temperature from relative 
+    humidity and air temperature." Journal of applied meteorology and climatology 50.11 (2011): 2267-2269.
 
     Parameters
     ----------
     t_air_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a}`
         [C]
     qv_i : float
-        instantaneous specific humidity
+        instantaneous specific humidity, 
         :math:`q_{v,i}`
         [kg/kg]
     p_air_i : float
-        instantaneous air pressure
+        instantaneous air pressure, 
         :math:`P_{i}`
         [mbar]
 
     Returns
     -------
     t_wet_i : float
-        instantaneous wet bulb temperature
+        instantaneous wet bulb temperature, 
         :math:`Tw_{a}`
         [C]
     """
     es_i = 0.6108*np.exp((17.27*t_air_i)/(t_air_i+237.3))
     rh_i = np.minimum((1.6077717*qv_i/10*p_air_i/es_i),1)*100
     rh_i = rh_i.clip(0,100)
     
     tw = t_air_i * np.arctan(0.152 * (rh_i + 8.3136)**(1/2)) + np.arctan(t_air_i + rh_i) - np.arctan(rh_i - 1.6763) + 0.00391838 *(rh_i)**(3/2) * np.arctan(0.0231 * rh_i) - 4.686
 
     return tw
 
-def wet_bulb_temperature_inst_new2(t_air_i):
-    r"""
-    Computes the instantaneous wet bulb temperature.
-
-    Parameters
-    ----------
-    t_air_i : float
-        instantaneous air temperature
-        :math:`T_{a}`
-        [C]
-
-    Returns
-    -------
-    t_wet_i : float
-        instantaneous wet bulb temperature
-        :math:`Tw_{a}`
-        [C]
-    """
-    
-    temp_tw = (17.27*t_air_i)/(237.3+t_air_i)
-    tw = 1.0919*temp_tw**2 + 13.306*temp_tw + 0.1304
-
-    return tw
-
-
 def dew_point_temperature_inst(vp_i):
     r"""
     Computes the instantaneous dew point temperature.
 
     Parameters
     ----------
     vp_i : float
-        instantaneous vapour pressure
+        instantaneous vapour pressure, 
         :math:`e_{a}`
         [mbar]
 
     Returns
     -------
     t_dew_i : float
-        instantaneous dew point temperature
+        instantaneous dew point temperature, 
         :math:`Td_{a}`
         [K]
     """
     t_dew_i = (237.3 * np.log(vp_i / 6.108)) / (17.27 - np.log(vp_i / 6.108))
 
     return t_dew_i
 
@@ -119,22 +96,22 @@
 def dew_point_temperature_coarse_inst(vp_i):
     r"""
     Computes the instantaneous dew point temperature.
 
     Parameters
     ----------
     vp_i : float
-        instantaneous vapour pressure
+        instantaneous vapour pressure, 
         :math:`e_{a}`
         [mbar]
 
     Returns
     -------
     t_dew_coarse_i : float
-        instantaneous dew point temperature
+        instantaneous dew point temperature, 
         :math:`Td_{a}`
         [K]
     """
     t_dew_i = (237.3 * np.log(vp_i / 6.108)) / (17.27 - np.log(vp_i / 6.108))
 
     return t_dew_i
 
@@ -165,19 +142,18 @@
 
     vp = 6.108 * np.exp((17.27 * t) / (237.3 + t))
 
     return vp
 
 
 # only used internally
-def wetbulb_temperature_iter(ta, td, pressure):
-    
+def wetbulb_temperature_iter(ta, td):
     maxiter = 1000
     tol = 1e-7
-    #pressure = 1013.25
+    pressure = 1013.25
 
     lv = latent_heat_iter(ta)
     psy = psychometric_constant_iter(lv, p=pressure)
 
     tw = td + ((ta - td) / 3)
     ea_ta = vapor_pressure_iter(td)
 
@@ -203,59 +179,57 @@
 
     return tw
 
 
 # some internal functions for the stability correction based on Brutsaert
 def psi_m(y):
     r"""
-    Computes the stability correction for momentum based on
-    Brutsaert (1999) [2]_.
+    Computes the stability correction for momentum based on :footcite:t:`brutsaert1999aspects`.
 
     .. math ::
-        \Psi_{M}(y)=\ln(a+y)-3by^{\frac{1}{3}}+ \\
-        \frac{ba^{\frac{1}{3}}}{2}\ln[\frac{(1+x)^{2}}{(1-x+x^{2})}]+\\
-        \sqrt{3}ba^{\frac{1}{3}}\arctan[\frac{(2x-1)}{\sqrt{3}}]+\Psi_{0}
+
+        \Psi_{M}(y) = & \ln(a+y)-3by^{\frac{1}{3}} + \\
+        & \frac{ba^{\frac{1}{3}}}{2}\ln[\frac{(1+x)^{2}}{(1-x+x^{2})}] + \\
+        & \sqrt{3}ba^{\frac{1}{3}}\arctan[\frac{(2x-1)}{\sqrt{3}}]+\Psi_{0}
 
     where the following constants are used
 
     * :math:`a` = 0.33
     * :math:`b` = 0.41
 
-    in which
+    in which:
 
     .. math ::
+
         x = (\frac{y}{a})^{\frac{1}{3}}
 
-    and
+    and:
 
     .. math ::
+
         y = \frac{-(z-d)}{L}
 
     where :math:`L` is the monin obukhov length defined by
     :func:`ETLook.unstable.monin_obukhov_length`,
     :math:`z` and :math:`d` are the
     measurement height and displacement height respectively. All aforementioned
     parameters are different for the bare soil and full canopy solutions.
 
     The symbol :math:`\Psi_{0}` denotes a constant of integration, given by
 
     .. math ::
-       \Psi_{0}=-\ln{a}+\sqrt{3}ba^{\frac{1}{3}}\frac{\pi}{6}
+
+        \Psi_{0}=-\ln({a}) + \sqrt{3} \cdot b \cdot a^{\frac{1}{3}} \cdot \frac{\pi}{6}
 
     Notes
     -----
     This function should not be used as an input function for a ETLook tool.
     This function is used internally by :func:`aerodynamical_resistance_bare`
     and :func:`aerodynamical_resistance_full` and :func:`wind_speed_soil`.
 
-    References
-    ----------
-    .. [2] Brutsaert, W., Aspect of bulk atmospheric boundary layer similarity
-        under free-convective conditions,
-        Reviews of Geophysics, 1999, 37(4), 439-451.
     """
     a = 0.33
     b = 0.41
     x = (y / a) ** (1. / 3.)
     phi_0 = -np.log(a) + np.sqrt(3) * b * a ** (1. / 3.) * np.pi / 6.
     res = (
         np.log(a + y)
@@ -266,317 +240,319 @@
     )
     return res
 
 
 def psi_h(y):
     r"""
     Computes the stability correction for momentum based on
-    Brutsaert (1999) [2]_.
+    :footcite:t:`brutsaert1999aspects`.
 
     .. math ::
+
         \Psi_{H}(y)=[\frac{(1-d)}{n}]\ln{\frac{(c+y^n)}{c}}
 
     where the following constants are used
 
     * :math:`c` = 1.00
     * :math:`d` = 0.057
     * :math:`n` = 0.78
 
     in which
 
     .. math ::
+
         y = \frac{-(z-d)}{L}
 
     where :math:`L` is the monin obukhov length defined by
     :func:`ETLook.unstable.monin_obukhov_length`,
     :math:`z` and :math:`d` are the
     measurement height and displacement height respectively. All aforementioned
     parameters are different for the bare soil and full canopy solutions.
 
     Notes
     -----
     This function should not be used as an input function for a tool.
     This function is used internally by :func:`aerodynamical_resistance_bare`
     and :func:`aerodynamical_resistance_full` and :func:`wind_speed_soil`.
 
-    References
-    ----------
-    .. [2] Brutsaert, W., Aspect of bulk atmospheric boundary layer similarity
-        under free-convective conditions,
-        Reviews of Geophysics, 1999, 37(4), 439-451.
     """
     c = 0.33
     d = 0.057
     n = 0.78
     return ((1 - d) / n) * np.log((c + y ** n) / c)
 
 
 def initial_friction_velocity_inst(u_b_i, z0m, disp, z_b=100):
     r"""
     Computes the initial instantaneous friction velocity without stability
     corrections.
 
     .. math ::
-        u_{*}=\frac{ku_{b}}{\ln\left(\frac{z_{b}-d}{z_{0,m}}\right)}
+
+        u_{*}=\frac{k \cdot u_{b}}{\ln\left(\frac{z_{b}-d}{z_{0,m}}\right)}
 
     Parameters
     ----------
     u_b_i : float
-        instantaneous wind speed at blending height
+        instantaneous wind speed at blending height, 
         :math:`u_{b}`
         [m s-1]
     z0m : float
-        surface roughness
+        surface roughness, 
         :math:`z_{0,m}`
         [m]
     disp : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
 
 
     Returns
     -------
     u_star_i_init : float
-        initial estimate of the instantaneous friction velocity
+        initial estimate of the instantaneous friction velocity, 
         :math:`u_{*,i}`
         [m s-1]
     """
     return (c.k * u_b_i) / (np.log((z_b - disp) / z0m))
 
 
 def atmospheric_emissivity_inst(vp_i, t_air_k_i):
     r"""
-    Computes the atmospheric emissivity according to Brutsaert [1]_.
+    Computes the atmospheric emissivity according to :footcite:t:`brutsaert1975derivable`.
 
     .. math ::
+
         \varepsilon_{a}=a\left(\frac{e_{a}}{T_{a}}\right)^{b}
 
     where the following constants are used
 
     * :math:`a` = 1.24
     * :math:`b` = 1/7
 
     Parameters
     ----------
     vp_i : float
-        instantaneous vapour pressure
+        instantaneous vapour pressure, 
         :math:`e_{a}`
         [mbar]
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a}`
         [K]
 
     Returns
     -------
     emiss_atm_i : float
-        instantaneous atmospheric emissivity
+        instantaneous atmospheric emissivity, 
         :math:`\varepsilon_{a}`
         [-]
 
-    References
-    ----------
-    .. [1] Brutsaert, W., On a derivable formula for long-wave radiation
-        from clear skies, Water Resour. Res, 1975, 11, 742-744.
     """
     return 1.24 * (vp_i / t_air_k_i) ** (1. / 7.)
 
 
 def net_radiation_bare(ra_hor_clear_i, emiss_atm_i, t_air_k_i, lst, r0_bare=0.38):
     r"""
-    Computes the net radiation for the bare soil with zero evaporation
+    Computes the net radiation for the bare soil with zero evaporation.
 
     .. math ::
 
-        Q_{bare}^{*}=\left(1-\alpha_{0,bare}\right)S_{d}+\varepsilon_{s}\varepsilon_{a}\sigma T_{a}^{4}-\varepsilon_{s}\sigma T_{s}^{4}
+        Q_{bare}^{*}=\left(1-\alpha_{0,bare}\right)S_{d}+\varepsilon_{s} \cdot \varepsilon_{a} \cdot \sigma \cdot T_{a}^{4}-\varepsilon_{s} \cdot \sigma \cdot T_{s}^{4}
 
     Parameters
     ----------
     ra_hor_clear_i : float
-        Total clear-sky irradiance on a horizontal surface
+        Total clear-sky irradiance on a horizontal surface, 
         :math:`S_{d}`
         [W/m2]
     emiss_atm_i : float
-        instantaneous atmospheric emissivity
+        instantaneous atmospheric emissivity, 
         :math:`\varepsilon_{a}`
         [-]
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a}`
         [K]
     lst : float
-        surface temperature
+        surface temperature, 
         :math:`T_{0}`
         [K]
     r0_bare : float
-        dry bare soil surface albedo
+        dry bare soil surface albedo, 
         :math:`\alpha_{0, bare}`
         [-]
 
 
     Returns
     -------
     rn_bare : float
-        net radiation bare soil
+        net radiation bare soil, 
         :math:`Q^*_{bare}`
         [Wm-2]
     """
     emiss_bare = 0.95
     rn_bare = (
         (1 - r0_bare) * ra_hor_clear_i
         + emiss_atm_i * emiss_bare * c.sb * (t_air_k_i) ** 4
         - emiss_bare * c.sb * (lst) ** 4
     )
 
+    if isinstance(rn_bare, xr.DataArray):
+        rn_bare = rn_bare.transpose("time", "y", "x").chunk("auto")
+
     return rn_bare
 
 
 def net_radiation_full(ra_hor_clear_i, emiss_atm_i, t_air_k_i, lst, r0_full=0.18):
     r"""
-    Computes the net radiation at full canopy with zero evaporation
+    Computes the net radiation at full canopy with zero evaporation.
 
     .. math ::
 
-        Q_{full}^{*}=\left(1-\alpha_{0,full}\right)S_{d}+\varepsilon_{c}\varepsilon_{a}\sigma T_{a}^{4}-\varepsilon_{c}\sigma T_{s}^{4}
+        Q_{full}^{*}=\left(1-\alpha_{0,full}\right) \cdot S_{d}+\varepsilon_{c} \cdot \varepsilon_{a} \cdot \sigma \cdot T_{a}^{4}-\varepsilon_{c} \cdot \sigma \cdot T_{s}^{4}
 
     Parameters
     ----------
     ra_hor_clear_i : float
-        Total clear-sky irradiance on a horizontal surface
+        Total clear-sky irradiance on a horizontal surface, 
         :math:`ra_hor_clear_i`
         [W/m2]
     emiss_atm_i : float
-        instantaneous atmospheric emissivity
+        instantaneous atmospheric emissivity, 
         :math:`P`
         [-]
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a}`
         [K]
     lst : float
-        surface temperature
+        surface temperature, 
         :math:`T_{0}`
         [K]
     r0_full : float
-        surface albedo full vegetation
+        surface albedo full vegetation, 
         :math:`\alpha_{0, full}`
         [-]
 
     Returns
     -------
     rn_full : float
-        net radiation full vegetation
+        net radiation full vegetation, 
         :math:`Q^*_{full}`
         [Wm-2]
     """
     emiss_full = 0.99
     rn_full = (
         (1 - r0_full) * ra_hor_clear_i
         + emiss_atm_i * emiss_full * c.sb * (t_air_k_i) ** 4
         - emiss_full * c.sb * (lst) ** 4
     )
 
+    if isinstance(rn_full, xr.DataArray):
+        rn_full = rn_full.transpose("time", "y", "x").chunk("auto")
+
     return rn_full
 
 
 def sensible_heat_flux_bare(rn_bare, fraction_h_bare=0.65):
     r"""
-    Computes the bare soil sensible heat flux
+    Computes the bare soil sensible heat flux.
 
     .. math ::
 
-        H_{bare} = H_{f, bare}Q^*_{bare}
+        H_{bare} = H_{f, bare} \cdot Q^*_{bare}
 
     Parameters
     ----------
     rn_bare : float
-        net radiation bare soil
+        net radiation bare soil, 
         :math:`Q^*_{bare}`
         [Wm-2]
     fraction_h_bare : float
-        fraction of H of net radiation bare soil
+        fraction of H of net radiation bare soil, 
         :math:`H_{f, bare}`
         [-]
 
     Returns
     -------
     h_bare : float
-        sensible heat flux bare soil
+        sensible heat flux bare soil, 
         :math:`H_{bare}`
         [Wm-2]
      """
     return rn_bare * fraction_h_bare
 
 
 def sensible_heat_flux_full(rn_full, fraction_h_full=0.95):
     r"""
-    Computes the full canopy sensible heat flux
+    Computes the full canopy sensible heat flux.
 
     .. math ::
 
-        H_{full} = H_{f, full}Q^*_{full}
+        H_{full} = H_{f, full} \cdot Q^*_{full}
 
     Parameters
     ----------
     rn_full : float
-        net radiation full vegetation
+        net radiation full vegetation, 
         :math:`Q^*_{full}`
         [Wm-2]
     fraction_h_full : float
-        fraction of H of net radiation full vegetation
+        fraction of H of net radiation full vegetation, 
         :math:`H_{f, full}`
         [-]
 
     Returns
     -------
     h_full : float
-        sensible heat flux full vegetation
+        sensible heat flux full vegetation, 
         :math:`H_{full}`
         [Wm-2]
      """
     return rn_full * fraction_h_full
 
 
 def wind_speed_blending_height_bare(u_i, z0m_bare=0.001, z_obs=10, z_b=100):
     r"""
     Computes the wind speed at blending height :math:`u_{b}` [m/s] using the
-    logarithmic wind profile
+    logarithmic wind profile.
 
     .. math ::
-        u_{b}=\frac{u_{obs}\ln\left(\frac{z_{b}}{z_{0,m}}\right)}
+
+        u_{b}=\frac{u_{obs} \cdot \ln\left(\frac{z_{b}}{z_{0,m}}\right)}
         {\ln\left(\frac{z_{obs}}{z_{0,m}}\right)}
 
     Parameters
     ----------
     u_i : float
-        instantaneous wind speed at observation height
+        instantaneous wind speed at observation height, 
         :math:`u_{obs}`
         [m/s]
     z_obs : float
-        observation height of wind speed
+        observation height of wind speed, 
         :math:`z_{obs}`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
     z0m_bare : float
-        surface roughness bare soil
+        surface roughness bare soil, 
         :math:`z_{0,m}`
         m
 
     Returns
     -------
     u_b_i_bare : float
-        instantaneous wind speed at blending height for bare soil
+        instantaneous wind speed at blending height for bare soil, 
         :math:`u_{b,i,bare}`
         [m/s]
     """
     ws = (c.k * u_i) / np.log(z_obs / z0m_bare) * np.log(z_b / z0m_bare) / c.k
 
     if isinstance(ws, xr.DataArray):
         ws = ws.clip(1, 150)
@@ -585,43 +561,44 @@
 
     return ws
 
 
 def wind_speed_blending_height_full_inst(u_i, z0m_full=0.1, z_obs=10, z_b=100):
     r"""
     Computes the wind speed at blending height :math:`u_{b}` [m/s] using the
-    logarithmic wind profile
+    logarithmic wind profile.
 
     .. math ::
-        u_{b}=\frac{u_{obs}\ln\left(\frac{z_{b}}{z_{0,m}}\right)}
+
+        u_{b}=\frac{u_{obs} \cdot \ln\left(\frac{z_{b}}{z_{0,m}}\right)}
         {\ln\left(\frac{z_{obs}}{z_{0,m}}\right)}
 
     Parameters
     ----------
     u_i : float
-        instantaneous wind speed at observation height
+        instantaneous wind speed at observation height, 
         :math:`u_{obs}`
         [m/s]
     z_obs : float
-        observation height of wind speed
+        observation height of wind speed, 
         :math:`z_{obs}`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
     z0m_full : float
-        surface roughness vegetation
+        surface roughness vegetation, 
         :math:`z_{0,m}`
         [m]
 
     Returns
     -------
     u_b_i_full : float
-        instantaneous wind speed at blending height for full vegetation
+        instantaneous wind speed at blending height for full vegetation, 
         :math:`u_{b,i,full}`
         [m s-1]
     """
     ws = (c.k * u_i) / np.log(z_obs / z0m_full) * np.log(z_b / z0m_full) / c.k
 
     if isinstance(ws, xr.DataArray):
         ws = ws.clip(1, 150)
@@ -629,699 +606,720 @@
         ws = np.clip(ws, 1, 150)
 
     return ws
 
 
 def friction_velocity_full_inst(u_b_i_full, z0m_full=0.1, disp_full=0.667, z_b=100):
     r"""
-    Like :func:`initial_friction_velocity_inst` but with full vegetation parameters
+    Like :func:`initial_friction_velocity_inst` but with full vegetation parameters.
 
     Parameters
     ----------
     u_b_i_full : float
-        instantaneous wind speed blending height for full vegetation
+        instantaneous wind speed blending height for full vegetation, 
         :math:`u_{b,d}`
         [m s-1]
     z0m_full : float
-        surface roughness vegetation
+        surface roughness vegetation, 
         :math:`z_{0,m,b}`
         [m]
     disp_full : float
-        displacement height vegetation
+        displacement height vegetation, 
         :math:`d^{b}`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_b`
         [m]
 
     Returns
     -------
     u_star_i_full : float
-        instantaneous friction velocity vegetation
+        instantaneous friction velocity vegetation, 
         :math:`u_{f}^{*}`
         [m s-1]
 
     """
     return initial_friction_velocity_inst(u_b_i_full, z0m_full, disp_full, z_b=100)
 
 
 def friction_velocity_bare_inst(u_b_i_bare, z0m_bare=0.001, disp_bare=0.0, z_b=100):
     r"""
-    Like :func:`initial_friction_velocity_inst` but with bare soil parameters
+    Like :func:`initial_friction_velocity_inst` but with bare soil parameters.
 
     Parameters
     ----------
     u_b_i_bare : float
-        instantaneous wind speed blending height bare soil
+        instantaneous wind speed blending height bare soil, 
         :math:`u_{b,d}`
         [W m-2]
     z0m_bare : float
-        surface roughness bare soil
+        surface roughness bare soil, 
         :math:`z_{0,m,b}`
         [m]
     disp_bare : float
-        displacement height bare soil
+        displacement height bare soil, 
         :math:`d^{b}`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_b`
         [m]
 
     Returns
     -------
     u_star_i_bare : float
-        instantaneous friction velocity bare soil
+        instantaneous friction velocity bare soil, 
         :math:`u_{b}^{*}`
         [m s-1]
 
     """
     return initial_friction_velocity_inst(u_b_i_bare, z0m_bare, disp_bare, z_b=100)
 
 
 def monin_obukhov_length_bare(h_bare, ad_i, u_star_i_bare, t_air_k_i):
     r"""
-    Like :func:`unstable.monin_obukhov_length` but with bare soil parameters
+    Like :func:`unstable.monin_obukhov_length` but with bare soil parameters.
 
     Parameters
     ----------
     h_bare : float
-        sensible heat flux for dry bare soil
+        sensible heat flux for dry bare soil, 
         :math:`H_{b,d}`
         [W m-2]
     ad_i : float
-        instantaneous air density
+        instantaneous air density, 
         :math:`\rho`
         [k g m-3]
     u_star_i_bare : float
-        instantaneous friction velocity bare soil
+        instantaneous friction velocity bare soil, 
         :math:`u^{*}_{b}`
         [m s-1]
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a}`
         [K]
 
     Returns
     -------
     L_bare : float
-        monin obukhov length dry vegetation
+        monin obukhov length dry vegetation, 
         :math:`L_{b,d}`
         [m]
 
     """
     return unstable.monin_obukhov_length(h_bare, ad_i, u_star_i_bare, t_air_k_i)
 
 
 def monin_obukhov_length_full(h_full, ad_i, u_star_i_full, t_air_k_i):
     r"""
-    Like :func:`unstable.monin_obukhov_length` but with full canopy parameters
+    Like :func:`unstable.monin_obukhov_length` but with full canopy parameters.
 
     Parameters
     ----------
     h_full : float
-        sensible heat flux for dry full vegetation
+        sensible heat flux for dry full vegetation, 
         :math:`H_{f,d}`
         [W m-2]
     ad_i : float
-        instantaneous air density
+        instantaneous air density, 
         :math:`\rho`
         [k g m-3]
     u_star_i_full : float
-        instantaneous friction velocity vegetation
+        instantaneous friction velocity vegetation, 
         :math:`u^{*}_{b}`
         [m s-1]
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a}`
         [K]
 
     Returns
     -------
     L_full : float
-        monin obukhov length dry vegetation
+        monin obukhov length dry vegetation, 
         :math:`L_{f,d}`
         [m]
 
     """
     return unstable.monin_obukhov_length(h_full, ad_i, u_star_i_full, t_air_k_i)
 
 
 def aerodynamical_resistance_forced_convection_full(u_i, L_full, z0m_full=0.1, disp_full=0.667, z_obs=10):
     r"""
-    Computes the aerodynamical resistance for a full canopy.
+    Computes the aerodynamical resistance for a full canopy, Eq A1 from Sanchez.
 
     .. math ::
-        z_{1} = \frac{z_{obs}-d}{z_{0,m}}
-
-        z_{2} = \frac{z_{obs}-d}{L}
-
-        z_{3} = \frac{z_{0,m}}{L}
-
-        z_{4} = \frac{z_{obs}-d}{\frac{z_{0,m}}{7}}
-
-        z_{5} = \frac{\frac{z_{0,m}}{7}}{L}
 
-        r_{a,c}=\frac{(\ln(z_{1})-\phi_{m}(-z_{2})+\phi_{m}(-z_{3}))(\ln(z_{4})-\phi_{h}(-z_{2})+\phi_{h}(-z_{5}))}{k^{2}u}
+        z_{1} &= \frac{z_{obs}-d}{z_{0,m}} \\
+        z_{2} &= \frac{z_{obs}-d}{L} \\
+        z_{3} &= \frac{z_{0,m}}{L} \\
+        z_{4} &= \frac{z_{obs}-d}{\frac{z_{0,m}}{7}} \\
+        z_{5} &= \frac{\frac{z_{0,m}}{7}}{L} \\
+        r_{a,c} &= \frac{(\ln(z_{1})-\phi_{m}(-z_{2})+\phi_{m}(-z_{3})) \cdot (\ln(z_{4})-\phi_{h}(-z_{2})+\phi_{h}(-z_{5}))}{k^{2} \cdot u}
 
     Parameters
     ----------
     u_i : float
-        instantaneous wind speed at observation height
+        instantaneous wind speed at observation height, 
         :math:`u_{obs}`
         [m/s]
     z_obs : float
-        observation height of wind speed
+        observation height of wind speed, 
         :math:`z_{obs}`
         [m]
     disp_full : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     z0m_full : float
-        surface roughness
+        surface roughness, 
         :math:`z_{0,m}`
         [m]
     L_full : float
-        monin obukhov length
+        monin obukhov length, 
         :math:`L`
         [m]
 
     Returns
     -------
     rac : float
-        aerodynamical resistance canopy
+        aerodynamical resistance canopy, 
         :math:`r_{a,c}`
         [sm-1]
 
     """
     z1 = (z_obs - disp_full) / z0m_full
     z2 = (z_obs - disp_full) / L_full
     z3 = z0m_full / L_full
     z4 = (z_obs - disp_full) / (z0m_full / 7)
     z5 = (z0m_full / 7) / L_full
-        
-    res_stable = (np.log(z_obs/z0m_full) - -5 * z_obs / L_full  +  -5 * z0m_full / L_full ) / (c.k * u_i) 
-    res_unstable =((np.log(z1) - psi_m(-z2) + psi_m(-z3)) * (np.log(z4) - psi_h(-z2) + psi_h(-z5))) / (c.k ** 2 * u_i)
-    
-    if isinstance(res_unstable, xr.DataArray):
-        res = xr.where(L_full>0,  np.nan, res_unstable)
-    else:
-        res = np.where(L_full>0,  np.nan, res_unstable)    
-    res = res.clip(5, 400)
-    
+    res = (
+        (np.log(z1) - psi_m(-z2) + psi_m(-z3)) * (np.log(z4) - psi_h(-z2) + psi_h(-z5))
+    ) / (c.k ** 2 * u_i)
+
     return res
 
 
 def aerodynamical_resistance_forced_convection_bare(u_i, L_bare, z0m_bare=0.001, disp_bare=0.0, z_obs=10):
     r"""
     Computes the aerodynamical resistance for a dry bare soil.
 
     .. math ::
-        z_{1} = \frac{z_{obs}-d}{z_{0,b,m}}
-
-        z_{2} = \frac{z_{obs}-d}{L_{b}}
 
-        r_{a,a}=\frac{(\ln(z_{1})-\phi_{m}(-z_{2}))(\ln(z_{1})-\phi_{h}(-z_{2}))}{k^{2}u}
+        z_{1} &= \frac{z_{obs}-d}{z_{0,b,m}} \\
+        z_{2} &= \frac{z_{obs}-d}{L_{b}} \\
+        r_{a,a} &= \frac{(\ln(z_{1})-\phi_{m}(-z_{2})) \cdot (\ln(z_{1})-\phi_{h}(-z_{2}))}{k^{2} \cdot u} \\
 
     Parameters
     ----------
     u_i : float
-        instantaneous wind speed at observation height
+        instantaneous wind speed at observation height, 
         :math:`u_{obs}`
         [m/s]
     z_obs : float
-        observation height of wind speed
+        observation height of wind speed, 
         :math:`z_{obs}`
         [m]
     disp_bare : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     z0m_bare : float
-        surface roughness
+        surface roughness, 
         :math:`z_{0,b,m}`
         [m]
     L_bare : float
-        monin obukhov length
+        monin obukhov length, 
         :math:`L_{b}`
         [m]
 
     Returns
     -------
     raa : float
-        aerodynamical resistance dry surface
+        aerodynamical resistance dry surface, 
         :math:`r_{a,a}`
         [sm-1]
 
     """
 
     z1 = (z_obs - disp_bare) / z0m_bare
     z2 = (z_obs - disp_bare) / L_bare
-      
-    res_stable = (np.log(z_obs/z0m_bare) - -5 * z_obs / L_bare  +  -5 * z0m_bare / L_bare ) / (c.k * u_i) 
-    res_unstable = ((np.log(z1) - psi_m(-z2)) * (np.log(z1) - psi_h(-z2))) / (c.k ** 2 * u_i)
-    
-    if isinstance(res_unstable, xr.DataArray):
-        res = xr.where(L_bare>0,  np.nan, res_unstable)
-    else:
-        res = np.where(L_bare>0,  np.nan, res_unstable)
-    res = res.clip(5, 400)
-    
+    res = ((np.log(z1) - psi_m(-z2)) * (np.log(z1) - psi_h(-z2))) / (c.k ** 2 * u_i)
+
     return res
 
 
 def wind_speed_soil_inst(u_i, L_bare, z_obs=10):
     r"""
-    Computes the instantaneous wind speed at soil surface
+    Computes the instantaneous wind speed at soil surface.
 
     .. math ::
 
-        u_{i,s}=u_{obs}\frac{\ln\left(\frac{z_{obs}}{z_{0}}\right)}
+        u_{i,s}=u_{obs} \cdot \frac{\ln\left(\frac{z_{obs}}{z_{0}}\right)}
               {\ln\left(\frac{z_{obs}}{z_{0,s}}\right)-\psi_{m}\left(\frac{-z_{0}}{L}\right)}
 
     Parameters
     ----------
     u_i : float
-        wind speed at observation height
+        wind speed at observation height, 
         :math:`u_{obs}`
         [m/s]
     z_obs : float
-        observation height of wind speed
+        observation height of wind speed, 
         :math:`z_{obs}`
         [m]
     L_bare : float
-        monin obukhov length
+        monin obukhov length, 
         :math:`L`
         [m]
 
     Returns
     -------
     u_i_soil : float
-        instantaneous wind speed just above soil surface
+        instantaneous wind speed just above soil surface, 
         :math:`u_{i,s}`
         [ms-1]
 
     """
     z0_soil = 0.01
     z0_free = 0.1
-
-    # TODO check why res_stable is unused
-    res_stable = (np.log(z_obs/z0_free) - -5 * z_obs / L_bare  +  -5 * z0_free / L_bare ) / (c.k * u_i) 
-    res_unstable = u_i * ((np.log(z0_free / z0_soil)) / (np.log(z_obs / z0_soil) - psi_m(-z0_free / L_bare)))
-    
-    if isinstance(res_unstable, xr.DataArray):
-        res = xr.where(L_bare>0, np.nan, res_unstable)
-    else:
-        res = np.where(L_bare>0, np.nan, res_unstable)
-    res = res.clip(5, 400)
-    
-    return(res)
-
-
-def aerodynamical_resistance_forced_convection_soil(u_i_soil):
-    r"""
-    Computes the aerodynamical resistance of the soil
-
-    .. math ::
-        r_{a,s}=\frac{1}{\left(0.0025T_{dif}^{\frac{1}{3}}+0.012u_{i,s}\right)}
-
-    Parameters
-    ----------
-    u_i_soil : float
-        instantaneous wind speed just above soil surface
-        :math:`u_{i,s}`
-        [m s-1]
-
-    Returns
-    -------
-    ras : float
-        aerodynamical resistance
-        :math:`r_{a,s}`
-        [sm-1]
-
-    """
-    Tdif = 10.0
-    return 1. / (0.0025 * (Tdif) ** (1. / 3.) + 0.012 * u_i_soil)
+    return u_i * (
+        (np.log(z0_free / z0_soil))
+        / (np.log(z_obs / z0_soil) - psi_m(-z0_free / L_bare))
+    )
 
 
 def maximum_temperature_full(
     ra_hor_clear_i, emiss_atm_i, t_air_k_i, ad_i, rac, r0_full=0.18
 ):
     r"""
-    Computes the maximum temperature under fully vegetated conditions
+    Computes the maximum temperature under fully vegetated conditions.
 
     .. math ::
 
-        T_{c,max}=\frac{\left(1-\alpha_{c}\right)S_{d}+\varepsilon_{c}\varepsilon_{a}\sigma
+        T_{c,max}=\frac{\left(1-\alpha_{c}\right) S_{d}+\varepsilon_{c}\varepsilon_{a}\sigma
                   T_{a}^{4}-\varepsilon_{c}\sigma T_{a}^{4}}{4\varepsilon_{s}\sigma
                   T_{a}^{3}+\rho C_{p}/r_{a,c}}+T_{a}
 
     Parameters
     ----------
     ra_hor_clear_i : float
-        Total clear-sky irradiance on a horizontal surface
+        Total clear-sky irradiance on a horizontal surface, 
         :math:`ra_hor_clear_i`
         [W/m2]
     emiss_atm_i : float
-        instantaneous atmospheric emissivity
+        instantaneous atmospheric emissivity, 
         :math:`P`
         [-]
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a}`
         [K]
     rac : float
-        aerodynamic resistance canopy
+        aerodynamic resistance canopy, 
         :math:`r_{a,c}`
         [sm-1]
     ad_i : float
-        instantaneous air density
+        instantaneous air density, 
         :math:`\rho`
         [kg m-3]
     r0_full : float
-        surface albedo full vegetation cover
+        surface albedo full vegetation cover, 
         :math:`\alpha_{0, full}`
         [-]
 
     Returns
     -------
     t_max_full : float
-        maximum temperature at full vegetation cover
+        maximum temperature at full vegetation cover, 
         :math:`T_{c,max}`
         [K]
 
     """
     emiss_full = 0.99
 
     tc_max_num = (
         (1 - r0_full) * ra_hor_clear_i
         + emiss_full * emiss_atm_i * c.sb * (t_air_k_i) ** 4
         - emiss_full * c.sb * (t_air_k_i) ** 4
     )
     tc_max_denom = 4 * emiss_full * c.sb * (t_air_k_i) ** 3 + (ad_i * c.sh) / rac
     tc_max = tc_max_num / tc_max_denom + t_air_k_i
 
+    if isinstance(tc_max, xr.DataArray):
+        tc_max = tc_max.transpose("time", "y", "x").chunk("auto")
+
     return tc_max
 
 
 def maximum_temperature_bare(
     ra_hor_clear_i, emiss_atm_i, t_air_k_i, ad_i, raa, ras, r0_bare=0.38
 ):
     r"""
-    Computes the maximum temperature under dry bare soil conditions
+    Computes the maximum temperature under dry bare soil conditions.
 
     .. math ::
 
         T_{s,max}=\frac{\left(1-\alpha_{s}\right)S_{d}+\varepsilon_{s}\varepsilon_{a}\sigma
         T_{a}^{4}-\varepsilon_{s}\sigma T_{a}^{4}}{4\varepsilon_{s}\sigma T_{a}^{3}+
         \rho C_{p}/\left[\left(r_{a,a}+r_{a,s}\right)\left(1-G/R_{n,s}\right)\right]}+T_{a}
 
     Parameters
     ----------
     ra_hor_clear_i : float
-        Total clear-sky irradiance on a horizontal surface
+        Total clear-sky irradiance on a horizontal surface, 
         :math:`ra_hor_clear_i`
         [W/m2]
     emiss_atm_i : float
-        instantaneous atmospheric emissivity
+        instantaneous atmospheric emissivity, 
         :math:`P`
         [-]
     t_air_k_i : float
-        instantaneous air temperature
+        instantaneous air temperature, 
         :math:`T_{a}`
         [K]
     ad_i : float
-        instantaneous air density
+        instantaneous air density, 
         :math:`\rho`
         [kg m-3]
     raa : float
-        aerodynamical resistance
+        aerodynamical resistance, 
         :math:`r_{a,a}`
         [sm-1]
     ras : float
-        aerodynamical resistance
+        aerodynamical resistance, 
         :math:`r_{a,s}`
         [sm-1]
     r0_bare : float
-        dry bare soil surface albedo
+        dry bare soil surface albedo, 
         :math:`\alpha_{0, bare}`
         [-]
 
     Returns
     -------
     t_max_bare : float
-        maximum temperature at bare soil
+        maximum temperature at bare soil, 
         :math:`T_{c,max}`
         [K]
 
     """
     emiss_bare = 0.95
     ts_max_num = (
         (1 - r0_bare) * ra_hor_clear_i
         + emiss_bare * emiss_atm_i * c.sb * (t_air_k_i) ** 4
         - emiss_bare * c.sb * (t_air_k_i) ** 4
     )
     ts_max_denom = 4 * emiss_bare * c.sb * (t_air_k_i) ** 3 + (ad_i * c.sh) / (
         (raa + ras) * (1 - 0.35)
     )
-    return ts_max_num / ts_max_denom + t_air_k_i
-
-def minimum_temperature_full(
-        ra_hor_clear_i, emiss_atm_i, t_air_k_i, ad_i, rac, lst_zone_mean, r0_full=0.18
-):
-    r"""
-    Computes the minimum temperature under fully vegetated conditions
-
-    .. math ::
-
-
-    Parameters
-    ----------
-    ra_hor_clear_i : float
-        Total clear-sky irradiance on a horizontal surface
-        :math:`ra_hor_clear_i`
-        [W/m2]
-    emiss_atm_i : float
-        instantaneous atmospheric emissivity
-        :math:`P`
-        [-]
-    t_air_k_i : float
-        instantaneous air temperature
-        :math:`T_{a}`
-        [K]
-    ad_i : float
-        instantaneous air density
-        :math:`\rho`
-        [kg m-3]
-    rac : float
-        aerodynamical resistance
-        :math:`r_{a,a}`
-        [sm-1]
-    lst_zone_mean : float
-        land surface temperature zone mean
-        [K]
-    r0_full : float
-        surface albedo full vegetation cover
-        :math:`\alpha_{0, full}`
-        [-]
-
-    Returns
-    -------
-    t_min_full : float
-        minimum temperature at full vegetation cover
-        :math:`T_{c,max}`
-        [K]
-
-    """
-
-    emiss_full = 0.99
-    g_rn_ratio = 0.0
-    LE_Rn_ratio = 1
-    
-    x_full = 1-g_rn_ratio-LE_Rn_ratio
-    c1 = x_full*emiss_full*c.sb*lst_zone_mean**3+(ad_i*c.sh)/rac
-    
-    ts_min_full = (x_full*(1-r0_full)*ra_hor_clear_i+x_full*emiss_atm_i*c.sb*t_air_k_i**4+(ad_i*c.sh*t_air_k_i)/rac)/c1
-
-    return ts_min_full
-
-
-
-def minimum_temperature_bare(
-        ra_hor_clear_i, emiss_atm_i, t_air_k_i, ad_i, raa, ras, lst_zone_mean, r0_bare_wet=0.15
-):
-    r"""
-    Computes the minimum temperature under dry bare soil conditions
-
-    .. math ::
-
-
-    Parameters
-    ----------
-    ra_hor_clear_i : float
-        Total clear-sky irradiance on a horizontal surface
-        :math:`ra_hor_clear_i`
-        [W/m2]
-    emiss_atm_i : float
-        instantaneous atmospheric emissivity
-        :math:`P`
-        [-]
-    t_air_k_i : float
-        instantaneous air temperature
-        :math:`T_{a}`
-        [K]
-    ad_i : float
-        instantaneous air density
-        :math:`\rho`
-        [kg m-3]
-    raa : float
-        aerodynamical resistance
-        :math:`r_{a,a}`
-        [sm-1]
-    ras : float
-        aerodynamical resistance
-        :math:`r_{a,a}`
-        [sm-1]
-    lst_zone_mean : float
-        land surface temperature zone mean
-        [K]
-    r0_bare_wet : float
-        wet bare soil surface albedo
-        :math:`\alpha_{0, bare}`
-        [-]
 
-    Returns
-    -------
-    t_min_bare : float
-        maximum temperature at bare soil
-        :math:`T_{c,max}`
-        [K]
-
-    """
-       
-    emiss_bare = 0.95
-    g_rn_ratio = 0.15
-    LE_Rn_ratio = 1
-    
-    x_bare = 1-g_rn_ratio-LE_Rn_ratio
-    c1 = x_bare*emiss_bare*c.sb*lst_zone_mean**3+(ad_i*c.sh)/(raa + ras)
-    
-    ts_min_bare = (x_bare*(1-r0_bare_wet)*ra_hor_clear_i+x_bare*emiss_atm_i*c.sb*t_air_k_i**4+(ad_i*c.sh*t_air_k_i)/(raa + ras))/c1
+    out = ts_max_num / ts_max_denom + t_air_k_i
 
-    return ts_min_bare
+    if isinstance(out, xr.DataArray):
+        out = out.transpose("time", "y", "x").chunk("auto")
 
+    return out
 
 
 def maximum_temperature(t_max_bare, t_max_full, vc):
     r"""
-    Computes the maximum temperature at dry conditions
+    Computes the maximum temperature at dry conditions.
 
     .. math ::
 
-        T_{0,max} = c_{veg}(T_{c,max}-T_{s,max})+T_{s,max}
+        T_{0,max} = c_{veg} \cdot (T_{c,max}-T_{s,max})+T_{s,max}
 
 
     Parameters
     ----------
     t_max_bare : float
-        maximum temperature at bare soil
+        maximum temperature at bare soil, 
         :math:`T_{s,max}`
         [K]
     t_max_full : float
-        maximum temperature at full dry vegetation
+        maximum temperature at full dry vegetation, 
         :math:`T_{c,max}`
         [K]
     vc : float
-        vegetation cover
+        vegetation cover, 
         :math:`c_{veg}`
         [-]
 
 
     Returns
     -------
     lst_max : float
-        maximum temperature at dry conditions
+        maximum temperature at dry conditions, 
         :math:`T_{0,max}`
         [K]
 
     """
-    return vc * (t_max_full - t_max_bare) + t_max_bare
+    out = vc * (t_max_full - t_max_bare) + t_max_bare
+
+    if isinstance(out, xr.DataArray):
+        out = out.transpose("time", "y", "x").chunk("auto")
+
+    return out
 
 
 def minimum_temperature(t_wet_k_i, t_air_k_i, vc):
     r"""
-    Computes the maximum temperature at dry conditions
+    Computes the maximum temperature at dry conditions.
 
     .. math ::
 
-        T_{0,min} = c_{veg}(T_{a,i}-T_{w})+T_{w}
+        T_{0,min} = c_{veg} \cdot (T_{a,i}-T_{w})+T_{w}
 
 
     Parameters
     ----------
     t_wet_k_i : float
-        minimum temperature at bare soil
+        minimum temperature at bare soil, 
         :math:`T_{s,max}`
         [K]
     t_air_k_i : float
-        minimum temperature at full vegetation
+        minimum temperature at full vegetation, 
         :math:`T_{c,max}`
         [K]
     vc : float
-        vegetation cover
+        vegetation cover, 
         :math:`c_{veg}`
         [-]
 
 
     Returns
     -------
     lst_min : float
-        minimum temperature at wet conditions
+        minimum temperature at wet conditions, 
         :math:`T_{0,min}`
         [K]
 
     """
-    return vc * (t_air_k_i - t_wet_k_i) + t_wet_k_i
+    out = vc * (t_air_k_i - t_wet_k_i) + t_wet_k_i
 
+    if isinstance(out, xr.DataArray):
+        out = out.transpose("time", "y", "x").chunk("auto")
+
+    return out
 
 def soil_moisture_from_maximum_temperature(lst_max, lst, lst_min):
     r"""
     Computes the relative root zone soil moisture based on estimates of
     maximum temperature and wet bulb temperature and measured land
-    surface temperature
+    surface temperature.
 
     .. math ::
 
         \Theta = \frac{T_{0}-T_{0,min}}{T_{0,max}-T_{0,min}}
 
     Parameters
     ----------
     lst : float
-        land surface temperature
+        land surface temperature, 
         :math:`T_{0}`
         [K]
     lst_max : float
-        maximum temperature at dry conditions
+        maximum temperature at dry conditions, 
         :math:`T_{0,max}`
         [K]
     lst_min : float
-        minimum temperature at wet conditions
+        minimum temperature at wet conditions, 
         :math:`T_{0, min}`
         [K]
 
 
     Returns
     -------
     se_root : float
-        soil moisture root zone soil moisture (based on LST)
+        relative root zone soil moisture (based on LST), 
         :math:`\Theta`
-        [cm3/cm3]
+        [%]
 
     """
     ratio = (lst - lst_min) / (lst_max - lst_min)
-    ratio = np.clip(ratio, 0, 1)
-    ratio = 1 - ratio
-    se_root = np.exp((ratio-1.0)/0.421)
-    
-    return se_root
+
+    if isinstance(ratio, xr.DataArray):
+        ratio = ratio.clip(0, 1)
+    else:
+        ratio = np.clip(ratio, 0, 1)
+
+    return 1 - ratio
+
+def aerodynamical_resistance_forced_convection_soil(u_i_soil):
+    r"""
+    Computes the aerodynamical resistance of the soil
+
+    Eq A7 from Sanchez.
+
+    .. math ::
+        r_{a,s}=\frac{1}{\left(0.0025T_{dif}^{\frac{1}{3}}+0.012u_{i,s}\right)}
+
+    Parameters
+    ----------
+    u_i_soil : float
+        instantaneous wind speed just above soil surface
+        :math:`u_{i,s}`
+        [m s-1]
+
+    Returns
+    -------
+    ras_forced : float
+        forced aerodynamical resistance
+        :math:`r_{a,s}`
+        [sm-1]
+
+    """
+    Tdif = 10.0
+    return 1. / (0.0025 * (Tdif) ** (1. / 3.) + 0.012 * u_i_soil)
+
+
+def aerodynamical_resistance_free_convection_bare(h_bare, t_air_k_i, ad_i, z0m_bare=0.001):
+    r"""
+    Calculates the aerodynamic resistance in the case of free convection for bare soil.
+
+    Based on equation 15 from:
+    https://journals.ametsoc.org/view/journals/apme/31/9/1520-0450_1992_031_1096_emlst_2_0_co_2.xml
+
+    Parameters
+    ----------
+    h_bare : float
+        sensible heat flux bare soil
+        :math:`H_{bare}`
+        [Wm-2]
+    t_air_k_i : float
+        instantaneous air temperature
+        :math:`T_{a}`
+        [K]
+    ad_i : float
+        instantaneous air density
+        :math:`\rho`
+        [k g m-3]
+    z0m_bare : float
+        surface roughness bare soil
+        :math:`z_{0,m}`
+        [m]
+
+    Returns
+    -------
+    rah_bare_free : float
+        aerodynamic resistance soil
+        :math:`r_{a,a}`
+        [sm-1]
+    """
+
+    # approximation: tpot = tact
+    θ = t_air_k_i
+    z0h_bare = z0m_bare / 7.
+
+    rah_bare_free = 1.00434 / (np.cbrt(z0h_bare/θ) * np.cbrt(h_bare/(ad_i*c.sh)))
+
+    return rah_bare_free
+
+
+def aerodynamical_resistance_free_convection_full(h_full, t_air_k_i, ad_i, z0m_full=0.1):
+    r"""
+    Calculates the aerodynamic resistance in the case of free convection for the canopy.
+
+    Based on equation 15 from:
+    https://journals.ametsoc.org/view/journals/apme/31/9/1520-0450_1992_031_1096_emlst_2_0_co_2.xml
+
+    Parameters
+    ----------
+    h_full : float
+        sensible heat flux full canopy
+        :math:`H_{full}`
+        [Wm-2]
+    t_air_k_i : float
+        instantaneous air temperature
+        :math:`T_{a}`
+        [K]
+    ad_i : float
+        instantaneous air density
+        :math:`\rho`
+        [k g m-3]
+    z0m_full : float
+        surface roughness full canopy
+        :math:`z_{0,m}`
+        [m]
+
+    Returns
+    -------
+    rah_full_free : float
+        aerodynamic resistance canopy
+        :math:`r_{a,c}`
+        [sm-1]
+    """
+
+    # approximation: tpot = tact
+    θ = t_air_k_i
+    z0h_full = z0m_full / 7.
+
+    rah_full_free = 1.00434 / (np.cbrt(z0h_full/θ) * np.cbrt(h_full/(ad_i*c.sh)))
+
+    return rah_full_free
+
+
+def aerodynamical_resistance_bare(raa_forced, ras_forced, rah_bare_free=np.inf):
+    r"""
+    Computes the aerodynamical resistance for a dry bare soil.
+
+    This function takes the minimum of forced and free convection
+
+    Parameters
+    ----------
+    raa_forced : float
+        forced aerodynamical resistance dry surface
+        :math:`r_{a,a}`
+        [sm-1]
+    ras_forced : float
+        forced aerodynamical resistance
+        :math:`r_{a,s}`
+        [sm-1]
+    rah_bare_free : float
+        aerodynamic resistance soil
+        :math:`r_{a,a}`
+        [sm-1]
+
+    Returns
+    -------
+    rah_bare : float
+        aerodynamical resistance bare soil
+        :math:`r_{a,h} bare`
+        [sm-1]
+    """
+
+    # soil forced resistance in series
+    rah_bare = np.minimum(raa_forced + ras_forced, rah_bare_free)
+
+    return rah_bare
+
+
+def aerodynamical_resistance_full(rac_forced, rah_full_free=np.inf):
+    r"""
+    Computes the aerodynamical resistance for a full canopy.
+
+    This function takes the minimum of forced and free convection
+
+    Parameters
+    ----------
+    rac_forced : float
+        forced aerodynamical resistance canopy
+        :math:`r_{a,c}`
+        [sm-1]
+    rah_full_free : float
+        aerodynamic resistance soil
+        :math:`r_{a,a}`
+        [sm-1]
+
+    Returns
+    -------
+    rah_full : float
+        aerodynamical resistance canopy
+        :math:`r_{a,h} canopy`
+        [sm-1]
+
+    """
+
+    rah_full = np.minimum(rac_forced, rah_full_free)
+
+    return rah_full
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/stress.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/stress.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,30 @@
 import numpy as np
 import xarray as xr
 
-def epsilon_soil_moisture(ef_24):
-    r"""
-    Computes the epsilon soil moisture
-
-    .. math ::
-        I = \frac{\lambda I^*}{86400}
-
-    Parameters
-    ----------
-    ef_24 : float
-        evaporative fraction
-        :math:`EF_{ref}`
-        [-]
-
-    Returns
-    -------
-    eps_w : float
-        epsilon soil moisture
-        :math:`I`
-        [-]
-    """
-    eps_w = 0.5 + 0.5 * ef_24
-     
-    return eps_w
-
-def epsilon_autotrophic_respiration():   
-    r"""
-    Computes the epsilon autotrophic respiration
-
-    Returns
-    -------
-    eps_a : float
-        epsilon autotrophic respiration
-        :math:`I`
-        [-]
-    """    
-    
-    # eps_a = 1-0.23 # 23% of GPP
-    eps_a = 1-0.5
-    
-    return eps_a
-
 def stress_radiation(ra_24):
     r"""
-    Computes the stress for plants when there is not sufficient radiation
+    Computes the stress for plants when there is not sufficient radiation.
 
     .. math ::
-        S_{r}=\frac{S^{\downarrow}}{\left(S^{\downarrow}+60.\right)}
+
+        S_{r}=\frac{S^{\downarrow}}{\left(S^{\downarrow}+60\right)}
         \left(1+\frac{60}{500}\right)
 
     Parameters
     ----------
     ra_24 : float
-        daily solar radiation
+        daily solar radiation, 
         :math:`S^{\downarrow}`
         [Wm-2]
 
     Returns
     -------
     stress_rad : float
-        stress factor for radiation
+        stress factor for radiation, 
         :math:`S_{r}`
         [-]
 
 
     Examples
     --------
     >>> import ETLook.stress as stress
@@ -87,18 +46,19 @@
 
     return stress
 
 
 def stress_moisture(se_root, tenacity=1.5):
     r"""
     Computes the stress for plants when there is not sufficient soil
-    moisture in the root zone
+    moisture in the root zone.
 
     .. math ::
-        S_{m}=K_{sf}S_{e,root}-\frac{\sin\left(2\pi S_{e,root}\right)}{2\pi}
+
+        S_{m}=K_{sf} \cdot S_{e,root}-\frac{\sin\left(2\pi \cdot S_{e,root}\right)}{2\pi}
 
     The tenacity factor :math:`K_{sf}` ranges from 1 for sensitive plants to
     1.5 for moderately sensitive plants to 3 for insensitive
     (tenacious plants).
 
     Parameters
     ----------
@@ -110,15 +70,15 @@
         tenacity factor
         `K_{sf}`
         [-]
 
     Returns
     -------
     stress_moist : float
-        stress factor for root zone moisture
+        stress factor for root zone moisture, 
         :math:`S_{m}`
         [-]
 
     Examples
     --------
     >>> import ETLook.stress as stress
     >>> stress.stress_moisture(0.5)
@@ -139,43 +99,45 @@
 
 
 def stress_temperature(t_air_24, t_opt=25.0, t_min=0.0, t_max=50.0):
     r"""
     Computes the stress for plants when it is too cold or hot
 
     .. math ::
+
         f=\frac{T_{max}-T_{opt}}{T_{opt}-T_{min}}
 
     .. math ::
-        s_{T}=\frac{\left(T_{a}-T_{min}\right)\left(T_{max}-T_{a}\right)^{f}}
-            {\left(T_{opt}-T_{min}\right)\left(T_{max}-T_{opt}\right)^{f}}
+
+        s_{T}=\frac{\left(T_{a}-T_{min}\right)\cdot\left(T_{max}-T_{a}\right)^{f}}
+            {\left(T_{opt}-T_{min}\right)\cdot\left(T_{max}-T_{opt}\right)^{f}}
 
     Parameters
     ----------
     t_air_24 : float
-        daily air temperature
+        daily air temperature, 
         :math:`T_{a}`
         [C]
     t_opt : float
-        optimum air temperature for plant growth
+        optimum air temperature for plant growth, 
         :math:`T_{opt}`
         [C]
     t_min : float
-        minimum air temperature for plant growth
+        minimum air temperature for plant growth, 
         :math:`T_{min}`
         [C]
     t_max : float
-        maximum air temperature for plant growth
+        maximum air temperature for plant growth, 
         :math:`T_{max}`
         [C]
 
     Returns
     -------
     stress_temp : float
-        stress factor for air temperature
+        stress factor for air temperature, 
         :math:`S_{T}`
         [-]
 
     Examples
     --------
     >>> import ETLook.stress as stress
     >>> stress.stress_temperature(15)
@@ -195,42 +157,43 @@
 
     stress = x/y
 
     if isinstance(stress, xr.DataArray):
         stress = stress.clip(0, 1)
     else:
         stress = np.clip(stress, 0, 1)
-        
+
     return stress
 
 
 def stress_vpd(vpd_24, vpd_slope=-0.3):
     r"""
     Computes the stress for plants if the vpd increases too much. With
     lower slopes the stress increases faster. The slope of the curve
-    is between -0.3 and -0.7
+    is between -0.3 and -0.7.
 
     .. math ::
-        S_{v}=m\ln(0.1\Delta_{e}+\frac{1}{2})+1
+
+        S_{v}=m \cdot \ln(0.1 \cdot \Delta_{e}+\frac{1}{2})+1
 
     Parameters
     ----------
     vpd_24 : float
-        daily vapour pressure deficit
+        daily vapour pressure deficit, 
         :math:`\Delta_{e}`
         [mbar]
     vpd_slope : float
-        vapour pressure stress curve slope
+        vapour pressure stress curve slope, 
         :math:`m`
         [mbar-1]
 
     Returns
     -------
     stress_vpd : float
-        stress factor for vapour pressure deficit
+        stress factor for vapour pressure deficit, 
         :math:`S_{v}`
         [-]
 
     Examples
     --------
     >>> import ETLook.stress as stress
     >>> stress.stress_vpd(15)
@@ -238,15 +201,14 @@
     >>> stress.stress_vpd(15, vpd_slope=-0.7)
     0.51479697360803833
     >>> stress.stress_vpd(15, vpd_slope=-0.3)
     0.79205584583201638
 
     """
     stress = vpd_slope * np.log(vpd_24/10. + 0.5) + 1
-
+    
     if isinstance(stress, xr.DataArray):
         stress = stress.clip(0, 1)
     else:
         stress = np.clip(stress, 0, 1)
 
-
     return stress
```

### Comparing `pywapor-3.3.4/pywapor/et_look_dev/unstable.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/unstable.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import numpy as np
-from pywapor.et_look_dev import constants as c
-
+from pywapor.et_look_v2_v3 import constants as c
+import xarray as xr
+import warnings
 
 def initial_sensible_heat_flux_canopy_daily(rn_24_canopy, t_24_init):
     r"""
     Computes the initial sensible heat flux before the iteration which solves
     the stability corrections. The first estimation of transpiration is used
     to estimate the initial sensible heat flux.
 
     .. math ::
 
         H_{canopy}=Q_{canopy}^{*}-T
 
     Parameters
     ----------
     rn_24_canopy : float
-        daily net radiation for the canopy
+        daily net radiation for the canopy, 
         :math:`Q_{canopy}^{*}`
         [W m-2]
     t_24_init : float
-        initial estimate of daily transpiration
+        initial estimate of daily transpiration, 
         :math:`T`
         [W m-2]
 
     Returns
     -------
     h_canopy_24_init : float
-        initial estimate of the sensible heat flux
+        initial estimate of the sensible heat flux, 
         :math:`H^{canopy}`
         [W m-2]
     """
 
     return rn_24_canopy - t_24_init
 
 
@@ -43,102 +44,102 @@
     .. math ::
 
         H_{soil}=Q_{soil}^{*}-G_{0}-E
 
     Parameters
     ----------
     rn_24_soil : float
-        daily net radiation for the soil
+        daily net radiation for the soil, 
         :math:`Q_{canopy}^{*}`
         [W m-2]
     g0_24 : float
-        daily soil heat flux
+        daily soil heat flux, 
         :math:`G_{0}`
         [W m-2]
     e_24_init : float
-        initial estimate of daily evaporation
+        initial estimate of daily evaporation, 
         :math:`E`
         [W m-2]
 
     Returns
     -------
     h_soil_24_init : float
-        initial estimate of the sensible heat flux
+        initial estimate of the sensible heat flux, 
         :math:`H_{canopy}`
         [W m-2]
     """
     return rn_24_soil - g0_24 - e_24_init
 
 
 def initial_friction_velocity_daily(u_b_24, z0m, disp, z_b=100):
     r"""
     Computes the initial friction velocity without using stability corrections.
 
     .. math ::
 
-        u_{*}=\frac{ku_{b}}{ln\left(\frac{z_{b}-d}{z_{0,m}}\right)}
+        u_{*}=\frac{k \cdot u_{b}}{ln\left(\frac{z_{b}-d}{z_{0,m}}\right)}
 
     Parameters
     ----------
     u_b_24 : float
-        daily wind speed at blending heigt
+        daily wind speed at blending heigt, 
         :math:`u_{b}`
         [m s-1]
     z0m : float
-        surface roughness
+        surface roughness, 
         :math:`z_{0,m}`
         [m]
     disp : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
 
 
     Returns
     -------
     u_star_24_init : float
-        initial estimate of the daily friction velocity
+        initial estimate of the daily friction velocity, 
         :math:`u_{*}`
         [m s-1]
     """
     return (c.k * u_b_24) / (np.log((z_b - disp) / z0m))
 
 
 def initial_friction_velocity_soil_daily(u_b_24, disp, z_b=100):
     r"""
     Computes the initial firction velocity without using stability corrections.
 
     .. math ::
 
-        u_{*}=\frac{ku_{b}}{ln\left(\frac{z_{b}-d}{z_{0,m}}\right)}
+        u_{*}=\frac{k \cdot u_{b}}{ln\left(\frac{z_{b}-d}{z_{0,m}}\right)}
 
     Parameters
     ----------
     u_b_24 : float
-        daily wind speed at blending heigt
+        daily wind speed at blending heigt, 
         :math:`u_{b}`
         [m s-1]
     disp : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
 
 
     Returns
     -------
     u_star_24_soil_init : float
-        initial estimate of the daily friction velocity for soil
+        initial estimate of the daily friction velocity for soil, 
         :math:`u_{*}`
         [m s-1]
     """
     return (c.k * u_b_24) / (np.log((z_b - disp) / c.z0_soil))
 
 
 def monin_obukhov_length(h_flux, ad, u_star, t_air_k):
@@ -150,34 +151,34 @@
     .. math ::
 
         L=\frac{-\rho c_{p}u_{*}^{3}T_{a}}{kgH_{canopy}}
 
     Parameters
     ----------
     h_flux : float
-        sensible heat flux
+        sensible heat flux, 
         :math:`H`
         [W m-2]
     ad : float
-        air density
+        air density, 
         :math:`\rho`
         [kg m-3]
     u_star : float
-        Monin Obukhov length
+        Monin Obukhov length, 
         :math:`L`
         [m]
     t_air_k : float
-        air tempererature in kelvin
+        air tempererature in kelvin, 
         :math:`T_{a}`
         [K]
 
     Returns
     -------
     monin : float
-        monin obukhov length
+        monin obukhov length, 
         :math:`L`
         [m]
     """
     return (-ad * c.sh * u_star ** 3 * t_air_k) / (c.k * c.g * h_flux)
 
 
 def stability_parameter(monin, disp, z_b=100):
@@ -189,57 +190,57 @@
     .. math ::
 
         x_{b}=1-16\left(\frac{z_{b}-d}{L}\right)^{0.25}
 
     Parameters
     ----------
     monin : float
-        monin obukhov length
+        monin obukhov length, 
         :math:`L`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
     disp : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
 
     Returns
     -------
     x_b : float
-        stability parameter used in stability correction
+        stability parameter used in stability correction, 
         :math:`x_{b}`
         [-]
     """
     return (1 - 16 * ((z_b - disp) / monin)) ** 0.25
 
 
 def stability_factor(x_b):
     r"""
     Computes the stability correction for heat at blending height.
 
     .. math ::
 
-        \psi_{h,b}=2\ln\left(\frac{1+x_{b}}{2}\right)+
+        \psi_{h,b}=2 \cdot \ln\left(\frac{1+x_{b}}{2}\right)+
         \ln\left(\frac{1+x_{b}^{2}}{2}\right)-
-        2\arctan\left(x_{b}\right)+0.5\pi
+        2 \cdot \arctan\left(x_{b}\right)+0.5 \cdot \pi
 
     Parameters
     ----------
     x_b : float
-        stability parameter used in stability correction
+        stability parameter used in stability correction, 
         :math:`x_{b}`
         [-]
 
     Returns
     -------
     sf : float
-        stability correction for heat
+        stability correction for heat, 
         :math:`\psi_{h,b}`
         [-]
     """
     return (
         2 * np.log((1 + x_b) / 2)
         + np.log((1 + x_b ** 2) / 2)
         - 2 * np.arctan(x_b)
@@ -256,92 +257,92 @@
     .. math ::
 
         x_{obs}=1-16\left(\frac{z_{obs}}{L}\right)^{0.25}
 
     Parameters
     ----------
     monin : float
-        monin obukhov length
+        monin obukhov length, 
         :math:`L`
         [m]
     z_obs : float
-        observation height
+        observation height, 
         :math:`z_{obs}`
         [m]
 
     Returns
     -------
     x_b_obs : float
-        stability parameter used in stability correction for observation height
+        stability parameter used in stability correction for observation height, 
         :math:`x_{obs}`
         [-]
     """
     return (1 - 16 * (z_obs / monin)) ** 0.25
 
 
 def stability_correction_heat_obs(x_b_obs):
     r"""
     Computes the stability correction for heat at observation height.
 
     .. math ::
 
-        \psi_{h,obs}=2\ln\left(\frac{1+x_{obs}^{2}}{2}\right)
+        \psi_{h,obs}=2 \cdot \ln\left(\frac{1+x_{obs}^{2}}{2}\right)
 
     Parameters
     ----------
     x_b_obs : float
-        stability parameter used in stability correction for observation height
+        stability parameter used in stability correction for observation height, 
         :math:`x_{obs}`
         [-]
 
     Returns
     -------
     sf_obs : float
-        stability correction for heat for observation height
+        stability correction for heat for observation height, 
         :math:`\psi_{h,obs}`
         [-]
     """
     return 2 * np.log((1 + x_b_obs ** 2) / 2)
 
 
 def friction_velocity(u_b, z_b, z0m, disp, sf):
     r"""
-    Computes the friction velocity
+    Computes the friction velocity.
 
     .. math ::
 
-        u_{*}=\frac{ku_{b}}{ln\left(\frac{z_{b}-d}{z_{0,m}}\right)-\psi_{h,b}}
+        u_{*}=\frac{k \cdot u_{b}}{ln\left(\frac{z_{b}-d}{z_{0,m}}\right)-\psi_{h,b}}
 
     Parameters
     ----------
     u_b : float
-        windspeed at blending height
+        windspeed at blending height, 
         :math:`u_{b}`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
     z0m : float
-        roughness length
+        roughness length, 
         :math:`z_{0,m}`
         [m]
     disp : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     sf : float
-        stability factor at blending height
+        stability factor at blending height, 
         :math:`\psi_{h,b}`
         [m]
 
     Returns
     -------
     u_star : float
-        friction velocity
+        friction velocity, 
         :math:`u_{*}`
         [m s-1]
     """
     return (c.k * u_b) / (np.log((z_b - disp) / z0m) - sf)
 
 
 def ra_canopy(
@@ -350,107 +351,114 @@
     r"""
     Computes the aerodynamical resistance for canopy using an iterative
     approach. The iteration is needed to compute the frication velocity at
     blending height Iteration stops either after five iterations or
     if the difference between two subsequent estimations is less than 0.01.
 
     .. math ::
-
-        \begin{cases}
-        \begin{array}{c}
-        L=\frac{-\rho c_{p}u_{*}^{3}T_{a}}{kgH_{canopy}}\\
-        x_{b}=1-16\left(\frac{z_{b}-d}{L}\right)^{0.25}\\
-        \psi_{h,b}=2\ln\left(\frac{1+z_{b}}{2}\right)+
+    
+        L &= \frac{-\rho c_{p}u_{*}^{3}T_{a}}{kgH_{canopy}}\\
+        x_{b} &= 1-16\left(\frac{z_{b}-d}{L}\right)^{0.25}\\
+        \psi_{h,b} &= 2 \ln\left(\frac{1+z_{b}}{2}\right)+
         \ln\left(\frac{1+z_{b}^{2}}{2}\right)-
         2\arctan\left(x_{b}\right)+0.5\pi\\
-        u_{*}=\frac{ku_{b}}{ln\left(\frac{z_{b}-d}{z_{0,m}}\right)-\psi_{h,b}}
-        \end{array}\end{cases}
+        u_{*} &= \frac{ku_{b}}{ln\left(\frac{z_{b}-d}{z_{0,m}}\right)-\psi_{h,b}}
+
 
     The friction velocity is independent of height. So this value can be used
     to calculate together with the stability correction for heat on observation
     heigth the aerodynamical resistance.
 
     .. math ::
 
-        x_{obs}=1-16\left(\frac{z_{obs}}{L}\right)^{0.25}
-
-        \psi_{h,obs}=2\ln\left(\frac{1+x_{obs}^{2}}{2}\right)
-
-        r_{a,canopy}=\frac{\ln\left(\frac{z_{obs}-d}
-        {0.1z_{0,m}}\right)-\psi_{h,obs}}{ku_{*}}
+        x_{obs}&=1-16 \cdot \left(\frac{z_{obs}}{L}\right)^{0.25} \\
+        \psi_{h,obs}&=2 \cdot \ln\left(\frac{1+x_{obs}^{2}}{2}\right) \\
+        r_{a,canopy}&=\frac{\ln\left(\frac{z_{obs}-d}
+        {0.1 \cdot z_{0,m}}\right)-\psi_{h,obs}}{k \cdot u_{*}}
 
     Parameters
     ----------
     h_canopy_init : float
-        initial estimate of the sensible heat flux
+        initial estimate of the sensible heat flux, 
         :math:`H^{canopy}`
         [W m-2]
     t_air_k : float
-        air tempererature in kelvin
+        air tempererature in kelvin, 
         :math:`T_{a}`
         [K]
     u_star_init : float
-        initial estimate of the daily friction velocity
+        initial estimate of the daily friction velocity, 
         :math:`u_{*}`
         [m s-1]
     ad : float
-        air density
+        air density, 
         :math:`\rho`
         [kg m-3]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
     z_obs : float
-        observation height
+        observation height, 
         :math:`z_{obs}`
         [m]
     z0m : float
-        roughness length
+        roughness length, 
         :math:`z_{0,m}`
         [m]
     disp : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     u_b : float
-        windspeed at blending height
+        windspeed at blending height, 
         :math:`u_{b}`
         [m/s]
     iter_ra : integer
-        number of iterations for aerodynamical resistance
+        number of iterations for aerodynamical resistance, 
         :math:`n_{ra}`
         [-]
 
     Returns
     -------
     ra_canopy : float
-        aerodynamical resistance for canopy
+        aerodynamical resistance for canopy, 
         :math:`r_{a,canopy}`
         [s m-1]
     """
     h_flux = h_canopy_init
     u_star_start = u_star_init
     iteration = 0
     epsilon = 10.0
     while (iteration < iter_ra) and (np.nanmax(epsilon) > 0.01):
         iteration += 1
         monin = monin_obukhov_length(h_flux, ad, u_star_start, t_air_k)
-        x_b = np.where(monin > 0, 1, stability_parameter(monin, disp, z_b))
+        if isinstance(monin, xr.DataArray):
+            x_b = xr.where(monin > 0, 1, stability_parameter(monin, disp, z_b))
+        else:
+            x_b = np.where(monin > 0, 1, stability_parameter(monin, disp, z_b))
         sf = stability_factor(x_b)
         u_star = friction_velocity(u_b, z_b, z0m, disp, sf)
         epsilon = abs(u_star - u_star_start)
         u_star_start = u_star
 
-    x_b_obs = np.where(monin <= 0, stability_parameter_obs(monin, z_obs), 1)
-    sf_obs = np.where(monin <= 0, stability_correction_heat_obs(x_b_obs), 0)
+    if isinstance(monin, xr.DataArray):
+        x_b_obs = xr.where(monin <= 0, stability_parameter_obs(monin, z_obs), 1)
+        sf_obs = xr.where(monin <= 0, stability_correction_heat_obs(x_b_obs), 0)
+    else:
+        x_b_obs = np.where(monin <= 0, stability_parameter_obs(monin, z_obs), 1)
+        sf_obs = np.where(monin <= 0, stability_correction_heat_obs(x_b_obs), 0)
 
     disp = np.minimum(disp, 1.5)
     ra = (np.log((z_obs - disp) / (0.1 * z0m)) - sf_obs) / (c.k * u_star)
-    ra = np.clip(ra, 25, 500)
+    
+    if isinstance(monin, xr.DataArray):
+        ra = ra.clip(25, 500)
+    else:
+        ra = np.clip(ra, 25, 500)
 
     return ra
 
 
 def transpiration(
     rn_24_canopy,
     ssvp_24,
@@ -481,96 +489,107 @@
         T=\frac{\Delta\left(Q_{canopy}^{*}\right)+\rho c_{p}\
            frac{\Delta_{e}}{r_{a,canopy}}}{\Delta+
            \gamma\left(1+\frac{r_{canopy}}{r_{a,canopy}}\right)}
 
     Parameters
     ----------
     rn_24_canopy : float
-        net radiation for the canopy
+        net radiation for the canopy, 
         :math:`Q^{*}_{canopy}`
         [Wm-2]
     ssvp_24 : float
        daily slope of saturated vapour pressure curve
        :math:`\Delta_{24}`
        [mbar K-1]
     ad_24 : float
-        daily air density
+        daily air density, 
         :math:`\rho_{24}`
         [kg m-3]
     vpd_24 : float
        daily vapour pressure deficit
        :math:`\Delta_{e,24}`
        [mbar]
     psy_24 : float
-        daily psychrometric constant
+        daily psychrometric constant, 
         :math:`\gamma_{24}`
         [mbar K-1]
     r_canopy : float
-        canopy resistance
+        canopy resistance, 
         :math:`r_{canopy}`
         [sm-1]
     h_canopy_24_init : float
-        initial estimate of the sensible heat flux
+        initial estimate of the sensible heat flux, 
         :math:`H^{canopy}`
         [W m-2]
     t_air_k_24 : float
-        daily air tempererature in kelvin
+        daily air tempererature in kelvin, 
         :math:`T_{a}`
         [K]
     u_star_24_init : float
-        initial estimate of the daily friction velocity
+        initial estimate of the daily friction velocity, 
         :math:`u_{*}`
         [m s-1]
     z0m : float
-        roughness length
+        roughness length, 
         :math:`z_{0,m}`
         [m]
     disp : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     u_b_24 : float
-        daily windspeed at blending height
+        daily windspeed at blending height, 
         :math:`u_{b}`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
     z_obs : float
-        observation height
+        observation height, 
         :math:`z_{obs}`
         [m]
     iter_h : integer
-        number of iterations for sensible heat flux
+        number of iterations for sensible heat flux, 
         :math:`n_h`
         [-]
 
     Returns
     -------
     t_24 : float
-        daily transpiration energy equivalent
+        daily transpiration energy equivalent, 
         :math:`T_{24}`
         [W m-2]
     """
     iteration = 0
     epsilon = 10.0
     h_start = h_canopy_24_init
 
-    while (iteration < iter_h) and (np.nanmax(epsilon) > 0.01):
-        iteration += 1
-        ra_canopy_start = ra_canopy(
-            h_start, t_air_k_24, u_star_24_init, ad_24, z0m, disp, u_b_24, z_obs, z_b
-        )
-        t = (ssvp_24 * rn_24_canopy + ad_24 * c.sh * (vpd_24 / ra_canopy_start)) / (
-            ssvp_24 + psy_24 * (1 + r_canopy / ra_canopy_start)
-        )
-        h = rn_24_canopy - t
-        epsilon = abs(h - h_start)
-        h_start = h
+    with warnings.catch_warnings():
+
+        warnings.filterwarnings("ignore", message="invalid value encountered in power")
+        warnings.filterwarnings("ignore", message="invalid value encountered in true_divide")
+        warnings.filterwarnings("ignore", message="invalid value encountered in divide")
+        warnings.filterwarnings("ignore", message="divide by zero encountered in log")
+        warnings.filterwarnings("ignore", message="divide by zero encountered in true_divide")
+        warnings.filterwarnings("ignore", message="divide by zero encountered in divide")
+
+        while (iteration < iter_h) and (np.nanmax(epsilon) > 0.01):
+            iteration += 1
+            
+            ra_canopy_start = ra_canopy(
+                h_start, t_air_k_24, u_star_24_init, ad_24, z0m, disp, u_b_24, z_obs, z_b
+            )
+
+            t = (ssvp_24 * rn_24_canopy + ad_24 * c.sh * (vpd_24 / ra_canopy_start)) / (
+                ssvp_24 + psy_24 * (1 + r_canopy / ra_canopy_start)
+            )
+            h = rn_24_canopy - t
+            epsilon = abs(h - h_start)
+            h_start = h
 
     return t
 
 
 def ra_soil(
     h_soil_24_init, t_air_k, u_star_24_init, ad, disp, u_b, z_obs=2, z_b=100, iter_ra=3
 ):
@@ -578,99 +597,102 @@
     Computes the aerodynamical resistance for canopy using an iterative
     approach. The iteration is needed to compute the friction velocity at
     blending height Iteration stops either after five iterations or
     if the difference between two subsequent estimations is less than 0.01.
 
     .. math ::
 
-        \begin{cases}
-        \begin{array}{c}
-        L=\frac{-\rho c_{p}u_{*}^{3}T_{a}}{kgH_{soil}}\\
-        x_{b}=1-16\left(\frac{z_{b}-d}{L}\right)^{0.25}\\
-        \psi_{h,b}=2\ln\left(\frac{1+z_{b}}{2}\right)+
+        L &= \frac{-\rho c_{p}u_{*}^{3}T_{a}}{kgH_{soil}}\\
+        x_{b} &= 1-16\left(\frac{z_{b}-d}{L}\right)^{0.25}\\
+        \psi_{h,b} &= 2\ln\left(\frac{1+z_{b}}{2}\right)+
         \ln\left(\frac{1+z_{b}^{2}}{2}\right)-
         2\arctan\left(x_{b}\right)+0.5\pi\\
-        u_{*}=\frac{ku_{b}}{ln\left(\frac{z_{b}-d}{z_{0,soil}}\right)
+        u_{*} &= \frac{ku_{b}}{ln\left(\frac{z_{b}-d}{z_{0,soil}}\right)
         -\psi_{h,b}}
-        \end{array}\end{cases}
+
 
     The friction velocity is independent of height. So this value can be used
     to calculate together with the stability correction for heat on observation
     heigth the aerodynamical resistance.
 
     .. math ::
 
-        x_{obs}=1-16\left(\frac{z_{obs}}{L}\right)^{0.25}
-
-        \psi_{h,obs}=2\ln\left(\frac{1+x_{obs}^{2}}{2}\right)
-
-        r_{a,soil}=\frac{\ln\left(\frac{z_{obs}-d}
+        x_{obs} &= 1-16\left(\frac{z_{obs}}{L}\right)^{0.25} \\
+        \psi_{h,obs} &= 2\ln\left(\frac{1+x_{obs}^{2}}{2}\right) \\
+        r_{a,soil} &= \frac{\ln\left(\frac{z_{obs}-d}
         {0.1z_{0,soil}}\right)-\psi_{h,obs}}{ku_{*}}
 
     Parameters
     ----------
     h_soil_24_init : float
-        initial estimate of the sensible heat flux for soil
+        initial estimate of the sensible heat flux for soil, 
         :math:`H^{soil}`
         [W m-2]
     t_air_k : float
-        air tempererature in kelvin
+        air tempererature in kelvin, 
         :math:`T_{a}`
         [K]
     u_star_24_init : float
-        initial estimate of the daily friction velocity
+        initial estimate of the daily friction velocity, 
         :math:`u_{*}`
         [m s-1]
     ad : float
-        air density
+        air density, 
         :math:`\rho`
         [kg m-3]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
     z_obs : float
-        observation height
+        observation height, 
         :math:`z_{obs}`
         [m]
     disp : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     u_b : float
-        windspeed at blending height
+        windspeed at blending height, 
         :math:`u_{b}`
         [m]
     iter_ra : integer
-        number of iterations for aerodynamical resistance
+        number of iterations for aerodynamical resistance, 
         :math:`n_{ra}`
         [-]
 
     Returns
     -------
     ra_soil : float
-        aerodynamical resistance for soil
+        aerodynamical resistance for soil, 
         :math:`r_{a,soil}`
         [s m-1]
     """
     h_flux = h_soil_24_init
     u_star_start = u_star_24_init
     iteration = 0
     epsilon = 10
     while (iteration < iter_ra) and (np.nanmax(epsilon) > 0.01):
         iteration += 1
         monin = monin_obukhov_length(h_flux, ad, u_star_start, t_air_k)
-        x_b = np.where(monin > 0, 0, stability_parameter(monin, disp, z_b))
+        if isinstance(monin, xr.DataArray):
+            x_b = xr.where(monin > 0, 0, stability_parameter(monin, disp, z_b))
+        else:
+            x_b = np.where(monin > 0, 0, stability_parameter(monin, disp, z_b))
         sf = stability_factor(x_b)
         u_star = friction_velocity(u_b, z_b, c.z0_soil, disp, sf)
         epsilon = abs(u_star - u_star_start)
         u_star_start = u_star
 
-    x_b_obs = np.where(monin <= 0, stability_parameter_obs(monin, z_obs), 1)
-    sf_obs = np.where(monin <= 0, stability_correction_heat_obs(x_b_obs), 0)
+    if isinstance(monin, xr.DataArray):
+        x_b_obs = xr.where(monin <= 0, stability_parameter_obs(monin, z_obs), 1)
+        sf_obs = xr.where(monin <= 0, stability_correction_heat_obs(x_b_obs), 0)
+    else:
+        x_b_obs = np.where(monin <= 0, stability_parameter_obs(monin, z_obs), 1)
+        sf_obs = np.where(monin <= 0, stability_correction_heat_obs(x_b_obs), 0)
 
     # 1.5 limit is from ETLook IDL
     disp = np.minimum(disp, 1.5)
     ra = (np.log((z_obs - disp) / (0.1 * c.z0_soil)) - sf_obs) / (c.k * u_star)
     ra = np.maximum(ra, 25)
 
     return ra
@@ -706,161 +728,169 @@
         E=\frac{\Delta\left(Q_{soil}^{*}-G\right)+
           \rho c_{p}\frac{\Delta_{e}}{r_{a,soil}}}
           {\Delta+\gamma\left(1+\frac{r_{soil}}{r_{a,soil}}\right)}
 
     Parameters
     ----------
     rn_24_soil : float
-        net radiation for the soil
+        net radiation for the soil, 
         :math:`Q^{*}_{canopy}`
         [Wm-2]
     g0_24 : float
-        daily soil heat flux
+        daily soil heat flux, 
         :math:`G`
         [Wm-2]
     ssvp_24 : float
        daily slope of saturated vapour pressure curve
        :math:`\Delta_{24}`
        [mbar K-1]
     ad_24 : float
-        daily air density
+        daily air density, 
         :math:`\rho_{24}`
         [kg m-3]
     vpd_24 : float
        daily vapour pressure deficit
        :math:`\Delta_{e,24}`
        [mbar]
     psy_24 : float
-        daily psychrometric constant
+        daily psychrometric constant, 
         :math:`\gamma_{24}`
         [mbar K-1]
     r_soil : float
-        soil resistance
+        soil resistance, 
         :math:`r_{soil}`
         [sm-1]
     h_soil_24_init : float
-        initial estimate of the sensible heat flux for soil
+        initial estimate of the sensible heat flux for soil, 
         :math:`H^{soil}`
         [W m-2]
     t_air_k_24 : float
-        daily air temperature in kelvin
+        daily air temperature in kelvin, 
         :math:`T_{a}`
         [K]
     u_star_24_soil_init : float
-        initial estimate of the daily friction velocity for soil
+        initial estimate of the daily friction velocity for soil, 
         :math:`u_{*}`
         [m s-1]
     disp : float
-        displacement height
+        displacement height, 
         :math:`d`
         [m]
     u_b_24 : float
-        daily wind speed at blending height
+        daily wind speed at blending height, 
         :math:`u_{b}`
         [m]
     z_b : float
-        blending height
+        blending height, 
         :math:`z_{b}`
         [m]
     z_obs : float
-        observation height
+        observation height, 
         :math:`z_{obs}`
         [m]
     iter_h : integer
-        number of iterations for sensible heat flux
+        number of iterations for sensible heat flux, 
         :math:`n_h`
         [-]
 
     Returns
     -------
     e_24 : float
-        daily evaporation energy equivalent
+        daily evaporation energy equivalent, 
         :math:`E_{24}`
         [W m-2]
     """
     iteration = 0
     epsilon = 10
     h_start = h_soil_24_init
-    while (iteration < iter_h) and (np.nanmax(epsilon) > 0.1):
-        iteration += 1
-        ra_soil_start = ra_soil(
-            h_start, t_air_k_24, u_star_24_soil_init, ad_24, disp, u_b_24, z_obs, z_b
-        )
-        e = (
-            ssvp_24 * (rn_24_soil - g0_24) + ad_24 * c.sh * (vpd_24 / ra_soil_start)
-        ) / (ssvp_24 + psy_24 * (1 + r_soil / ra_soil_start))
-        h = rn_24_soil - g0_24 - e
-        epsilon = abs(h - h_start)
-        h_start = h
- 
-    e = e.clip(0, 100)
+
+    with warnings.catch_warnings():
+
+        warnings.filterwarnings("ignore", message="invalid value encountered in power")
+        warnings.filterwarnings("ignore", message="invalid value encountered in divide")
+        warnings.filterwarnings("ignore", message="invalid value encountered in true_divide")
+        warnings.filterwarnings("ignore", message="divide by zero encountered in log")
+        warnings.filterwarnings("ignore", message="divide by zero encountered in power")
+        warnings.filterwarnings("ignore", message="divide by zero encountered in divide")
+        
+        while (iteration < iter_h) and (np.nanmax(epsilon) > 0.1):
+            iteration += 1
+            ra_soil_start = ra_soil(
+                h_start, t_air_k_24, u_star_24_soil_init, ad_24, disp, u_b_24, z_obs, z_b
+            )
+            e = (
+                ssvp_24 * (rn_24_soil - g0_24) + ad_24 * c.sh * (vpd_24 / ra_soil_start)
+            ) / (ssvp_24 + psy_24 * (1 + r_soil / ra_soil_start))
+            h = rn_24_soil - g0_24 - e
+            epsilon = abs(h - h_start)
+            h_start = h
 
     return e
 
 
 def transpiration_mm(t_24, lh_24):
     r"""
     Computes the canopy transpiration based on the Penman Monteith equation
     adapted for canopy.
 
     .. math ::
 
-        T=Td_{sec}\lambda_{24}
+        T=T \cdot \frac{d_{sec}}{\lambda_{24}}
 
     where the following constants are used
 
     * :math:`d_{sec}` seconds in the day = 86400 [s]
 
     Parameters
     ----------
     t_24 : float
-        daily transpiration energy equivalent
+        daily transpiration energy equivalent, 
         :math:`E^{0}`
         [W m-2]
     lh_24 : float
-        daily latent heat of evaporation
+        daily latent heat of evaporation, 
         :math:`\lambda_{24}`
         [J/kg]
 
     Returns
     -------
     t_24_mm : float
-        daily transpiration in mm
+        daily transpiration in mm, 
         :math:`T`
         [mm d-1]
     """
     return t_24 * c.day_sec / lh_24
 
 
 def evaporation_mm(e_24, lh_24):
     r"""
     Computes the soil evaporation based on the Penman Monteith equation
     adapted for soils.
 
     .. math ::
 
-        E=Ed_{sec}\lambda_{24}
+        E=E \cdot \frac{d_{sec}}{\lambda_{24}}
 
     where the following constants are used
 
     * :math:`d_{sec}` seconds in the day = 86400 [s]
 
     Parameters
     ----------
     e_24 : float
-        daily evaporation energy equivalent
+        daily evaporation energy equivalent, 
         :math:`E^{0}`
         [W m-2]
     lh_24 : float
-        daily latent heat of evaporation
+        daily latent heat of evaporation, 
         :math:`\lambda_{24}`
         [J/kg]
 
     Returns
     -------
     e_24_mm : float
-        daily evaporation in mm
+        daily evaporation in mm, 
         :math:`E`
         [mm d-1]
     """
     return e_24 * c.day_sec / lh_24
```

### Comparing `pywapor-3.3.4/pywapor/et_look_v2_v3/biomass.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/biomass.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/et_look_v2_v3/clear_sky_radiation.py` & `pywapor-3.3.5/pywapor/et_look_v2_v3/solar_radiation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,588 +1,692 @@
-"""
-    The `clear_sky_radiation` module contains all functions related to the
-    calculation of (instantaneous) clear sky radation. Most of these
-    functions are based upon :footcite:t:`vsuri2004new`.
-
-"""
 import numpy as np
+from pywapor.et_look_v2_v3 import constants as con
 import xarray as xr
+import warnings
 
-def extraterrestrial_irradiance_normal(I0, ied):
+def longitude_rad(lon_deg):
     r"""
-    Computes the extraterrestrial irradiance normal to the solar beam.
-
-    .. math ::
-
-        G_{0} = I_{0} \cdot \varepsilon
+    Converts longitude from degrees to radians.
 
     Parameters
     ----------
-    I0 : float
-        solar constant, 
-        :math:`I_{0}`
-        [W m\ :sup:`-2`\]
-    ied : float
-        inverse earth sun distance, 
-        :math:`\varepsilon`
-        [AU\ :sup:`-1`\]
+    lon_deg : float
+        longitude in degrees, 
+        :math:`\phi`
+        [deg]
 
     Returns
     -------
-    G0 : float
-        ext rad normal to solar bea, 
-        :math:`G_{0}`
-        [W m\ :sup:`-2`\]
+    lon : float
+        longitude, 
+        :math:`\phi`
+        [rad]
 
     """
-    return I0*ied
+    return lon_deg * np.pi/180.0
 
 
-def inverse_earth_sun_distance(day_angle):
+def latitude_rad(lat_deg):
     r"""
-    Computes the inverse earth sun distance
-
-    .. math ::
-
-        \varepsilon = 1 + 0.03344 \cdot \cos(j^{\prime} - 0.048869)
+    Converts latitude from degrees to radians.
 
     Parameters
     ----------
-    day_angle : float
-        day angle, 
-        :math:`j^{\prime}`
-        [-]
+    lat_deg : float
+        latitude in degrees, 
+        :math:`\lambda`
+        [deg]
 
     Returns
     -------
-    ied : float
-        inverse earth sun distance, 
-        :math:`\varepsilon`
-        [AU]
+    lat : float
+        latitude, 
+        :math:`\lambda`
+        [rad]
 
     """
-    return 1 + 0.03344 * np.cos(day_angle - 0.048869)
+    return lat_deg * np.pi/180.0
 
 
-def day_angle(doy):
+def slope_rad(slope_deg):
     r"""
-
-    Computes the day angle. 0 is january 1\ :sup:`st`\,
-    2\ :math:`\pi` is december 31\ :sup:`st`\.
-
-    .. math ::
-
-        j^{\prime} = \frac{2 \cdot \pi \cdot j} {365.25}
+    Converts slope from degrees to radians.
 
     Parameters
     ----------
-    doy : float
-        day of year, 
-        :math:`j`
-        [-]
+    slope_deg : float
+        slope in degrees, 
+        :math:`s`
+        [deg]
 
     Returns
     -------
-    day_angle : float
-        day angle, 
-        :math:`j^{\prime}`
+    slope : float
+        slope, 
+        :math:`\Delta`
         [rad]
 
     """
-    return 2 * np.pi * doy / 365.25
+    return slope_deg * np.pi/180.0
 
 
-def solar_constant():
+def aspect_rad(aspect_deg):
     r"""
-    Returns the solar constant. The solar constant is defined as the
-    flux density of solar radiation at the mean distance from Sun
-    to Earth. The solar constant is estimated to be 1367 W m\ :sup:`-2`\.
+    Converts aspect from degrees to radians.
 
     Parameters
     ----------
+    aspect_deg : float
+        aspect in degrees, 
+        :math:`s`
+        [deg]
 
     Returns
     -------
-    I0 : float
-        solar constant, 
-        :math:`I_{0}`
-        [W m\ :sup:`-2`\]
+    aspect : float
+        aspect (0 is north; pi is south), 
+        :math:`\alpha`
+        [rad]
     """
-    return 1367.
+    return aspect_deg * np.pi/180.0
 
 
-def declination(day_angle):
+def declination(doy):
     r"""
-    Computes the solar declination. The solar declination is computed according to 
-    :footcite:t:`gruter1984radiation`.
+    Computes the solar declination which is the angular height of the sun
+    above the astronomical equatorial plane in radians.
 
     .. math ::
 
-        \delta = \arcsin\left(0.3978 \cdot \sin\left(j^{\prime} - 1.4 + 0.0355 \cdot \sin
-              \left(j^{\prime} - 0.0489\right)\right)\right)
+        \delta=0.409 \cdot \sin\left(\frac{2\pi \cdot J}{365}-1.39\right)
 
     Parameters
     ----------
-    day_angle : float
-        day angle, 
-        :math:`j^{\prime}`
-        [rad]
+    doy : float
+        julian day of the year, 
+        :math:`J`
+        [-]
 
     Returns
     -------
     decl : float
         declination, 
         :math:`\delta`
         [rad]
 
+    Examples
+    --------
+    >>> import ETLook.solar_radiation as solrad
+    >>> solrad.declination(180)
+    0.40512512455439242
     """
-    return np.arcsin(0.3978 * np.sin(day_angle - 1.4 + 0.0355 * np.sin(day_angle - 0.0489)))
+    return 0.409 * np.sin(2 * np.pi / 365 * doy - 1.39)
 
 
-def relative_optical_airmass(p_air_i, p_air_0_i, h0ref):
+def earth_sun_distance(doy):
     r"""
-    Computes the relative optical air mass. It is calculated according to :footcite:t:`kasten1989revised`.
+    Computes the earth sun distance in Angstrom Unit where 1 AU is 1.496e8 km.
 
     .. math ::
 
-        m = \frac{\frac{p}{p_{0}}}{\sin h_{0}^{ref}+0.50572
-         \left(h_{0}^{ref}+6.07995\right)^{-1.6364}}
+        d_{r}=1+0.033 \cdot \cos\left(\frac{2\pi \cdot J}{365}\right)
 
     Parameters
     ----------
-    p_air_i : float
-        actual instantaneous air pressure, 
-        :math:`p`
-        [hPa]
-    p_air_0_i : float
-        air pressure at sea level, 
-        :math:`p_{0}`
+    doy : float
+        julian day of the year, 
+        :math:`J`
         [-]
-    h0ref : float
-        solar elevation angle corrected for refraction, 
-        :math:`h_{0}^{ref}`
-        [degrees]
 
     Returns
     -------
-    m : float
-        relative optical airmass, 
-        :math:`m`
-        [-]
+    ed : float
+        earth sun distance, 
+        :math:`d_{r}`
+        [AU]
 
+    Examples
+    --------
+    >>> import ETLook.solar_radiation as solrad
+    >>> solrad.earth_sun_distance(180)
+    0.96703055420162642
     """
-    h0ref_rad = h0ref * np.pi/180.
 
-    m = (p_air_i/p_air_0_i)/(np.sin(h0ref_rad) + 0.50572 * (h0ref + 6.07995)**-1.6364)
-    
-    if isinstance(m, np.ndarray):
-        m[h0ref_rad <= 0] = 64
-    else:
-        m = m.where(h0ref_rad > 0, 64)
+    warnings.warn(('Using "ed" for the inverse earth-sun distance is deprecated, '
+                   'use "iesd" (solar_radiation.inverse_earth_sun_distance) instead'),
+                  DeprecationWarning, stacklevel=2)
 
-    return m
+    return 1 + 0.033 * np.cos(doy * 2 * np.pi / 365.0)
 
 
-def solar_elevation_angle_refracted(h0):
+def inverse_earth_sun_distance(doy):
     r"""
-    Computes the solar elevation angle corrected for refraction.
-
-    .. math ::
-
-        h_{0}^{ref} = h_{0} + \Delta h_{0}^{ref}
-
-    where:
+    Computes the inverse earth sun distance (iesd) in Angstrom Unit where 1 AU is 1.496e8 km.
 
     .. math ::
 
-        \Delta h_{0}^{ref}=0.61359 \cdot \frac{0.1594 + 1.123 \cdot h_{0} +
-        0.065656 \cdot h_{0}^{2}}{
-        1+28.9344 \cdot h_{0} + 277.3971 \cdot h_{0}^{2}}
+        d_{r}=1+0.033 \cdot \cos\left(\frac{2\pi \cdot J}{365}\right)
 
     Parameters
     ----------
-    h0 : float
-        solar elevation angle, 
-        :math:`h_{0}`
-        [degrees]
+    doy : float
+        julian day of the year, 
+        :math:`J`
+        [-]
 
     Returns
     -------
-    h0ref : float
-        solar elevation angle corrected for refrection, 
-        :math:`h_{0}^{ref}`
-        [degrees]
+    iesd : float
+        inverse earth sun distance, 
+        :math:`d_{r}`
+        [AU]
+
+    Examples
+    --------
+    >>> import ETLook.solar_radiation as solrad
+    >>> solrad.inverse_earth_sun_distance(180)
+    0.96703055420162642
     """
-    delta_h0ref = 0.061359 * (0.1594 + 1.123*h0 + 0.065656*h0**2)/(1 + 28.9344*h0 + 277.3971*h0**2)
-    h0ref = h0 + delta_h0ref
 
-    return h0ref
+    return 1 + 0.033 * np.cos(doy * 2 * np.pi / 365.0)
 
 
-def hour_angle(solar_time):
+def actual_earth_sun_distance(iesd):
     r"""
-    Computes the solar hour angle.
+    Computes the earth sun distance (esd) in Angstrom Unit where 1 AU is 1.496e8 km.
 
     .. math ::
 
-        T = \frac{\pi}{12}\left(t-12\right)
+        d_{r}=1+0.033 \cdot \cos\left(\frac{2\pi \cdot J}{365}\right)
 
     Parameters
     ----------
-    solar_time : float
-        solar_time, 
-        :math:`t`
-        [hours]
+    iesd : float
+        inverse earth sun distance, 
+        :math:`J`
+        [AU]
 
     Returns
     -------
-    ha : float
-        solar hour angle, 
-        :math:`T`
-        [rad]
+    esd : float
+        earth sun distance, 
+        :math:`d_{r}`
+        [AU]
 
+    Examples
+    --------
+    >>> import ETLook.solar_radiation as solrad
+    >>> solrad.actual_earth_sun_distance(180)
+    1.034093489244084
     """
-    ha = np.pi / 12 * (solar_time - 12)
 
-    return ha
+    return 1 / iesd
 
 
-def solar_elevation_angle(lat, decl, ha):
+def seasonal_correction(doy):
     r"""
-    Computes the solar elevation angle.
+    Computes the seasonal correction for solar time  in hours.
 
     .. math ::
 
-        h_{0}=\arcsin\left(C_{31} \cdot \cos(T) + C_{33}\right)
-
-    where:
+        b=\frac{2\pi\left(J-81\right)}{365}
 
     .. math ::
 
-        C_{31} &= \cos(\varphi) \cdot \cos(\delta) \\
-        C_{33} &= \sin(\varphi) \cdot \sin(\delta)
+        s_{c}= 0.1645 \cdot sin \left( 2b \right) - 0.1255 \cdot cos \left(b \right) - 0.025 \left(b\right)
 
     Parameters
     ----------
-    lat : float
-        latitude, 
-        :math:`\varphi`
-        [rad]
-    decl : float
-        declination, 
-        :math:`\delta`
-        [rad]
-    ha : float
-        solar hour angle, 
-        :math:`T`
-        [rad]
+    doy : float
+        julian day of the year, 
+        :math:`J`
+        [-]
 
     Returns
     -------
-    h0 : float
-        solar elevation angle, 
-        :math:`h_0`
-        [degrees]
+    sc : float
+        seasonal correction, 
+        :math:`s_{c}`
+        [hours]
 
+    Examples
+    --------
+    >>> import ETLook.solar_radiation as solrad
+    >>> solrad.seasonal_correction(180)
+    -0.052343379605521212
     """
-    C31 = np.cos(lat) * np.cos(decl)
-    C33 = np.sin(lat) * np.sin(decl)
-
-    sin_h0 = C31 * np.cos(ha) + C33
-
-    h0_rad = np.arcsin(sin_h0)
+    b = 2 * np.pi * (doy - 81) / 365.0
+    return 0.1645 * np.sin(2 * b) - 0.1255 * np.cos(b) - 0.025 * np.sin(b)
 
-    h0 = h0_rad * 180 / np.pi
 
-    if isinstance(h0, xr.DataArray):
-        h0 = h0.transpose("time", "y", "x").chunk("auto")
+def sunset_hour_angle(lat, decl):
+    r"""
+    Computes the sunset hour angle.
 
-    return h0
+    .. math ::
 
+        w_{s}=\arccos(-\tan(\lambda)\cdot \tan(\delta))
 
-def rayleigh_optical_thickness(m):
-    r"""
-    Computes the Rayleigh optical thickness at airmass :math:`m`. It is calculated according
-    to the improved formula by :footcite:t:`kasten1996linke`.
+    Parameters
+    ----------
+    decl : float
+        solar declination, 
+        :math:`\delta`
+        [rad]
+    lat : float
+        latitude, 
+        :math:`\lambda`
+        [rad]
 
-    if :math:`m` > 20:
+    Returns
+    -------
+    ws : float
+        sunset hour angle, 
+        :math:`w_{s}`
+        [rad]
 
-    .. math ::
+    """
+    return np.arccos(-(np.tan(lat) * np.tan(decl)))
 
-        \delta_{R}(m) = \left(6.6296 + 1.7513 \cdot  m - 0.1202 \cdot m^{2} + 0.0065 \cdot m^{3} - 0.00013 \cdot m^{4}\right)^{-1}
 
-    if :math:`m` < 20:
+def hour_angle(sc, dtime, lon = 0):
+    r"""
+    Computes the hour angle which is zero at noon and -pi at 0:00 am and
+    pi at 12:00 pm
 
     .. math ::
 
-        \delta_{R}(m) = \left(10.4+0.718 \cdot m\right)^{-1}
+        \omega=\left(\frac{\pi}{12}\right)\cdot \left(t+s_{c}-12\right)
 
     Parameters
     ----------
-    m : float
-        relative optical airmass, 
-        :math:`m`
-        [-]
+    sc : float
+        seasonal correction, 
+        :math:`s_{c}`
+        [hours]
+    dtime : float
+        decimal time, 
+        :math:`t`
+        [hours]
+    lon : float
+        longitude, 
+        :math:`\phi`
+        [rad]
 
     Returns
     -------
-    rotm : float
-        Rayleigh optical thickness at airmass m, 
-        :math:`\delta_{R}`
-        [-]
+    ha : float
+        hour_angle, 
+        :math:`\omega`
+        [rad]
 
+    Examples
+    --------
+    >>> import ETLook.solar_radiation as solrad
+    >>> solrad.hour_angle(sc=solrad.seasonal_correction(75), dtime=11.4)
+    -0.19793970172084141
     """
-
-    rotm = 1 / (10.4 + 0.718 * m)
-    if isinstance(rotm, np.ndarray):
-        rotm = np.where(m <= 20, 1/(6.6296 + 1.7513*m - 0.1202*m**2 + 0.0065*m**3 - 0.00013*m**4), rotm)
-    else:
-        rotm_star = 1/(6.6296 + 1.7513*m - 0.1202*m**2 + 0.0065*m**3 - 0.00013*m**4)
-        rotm = rotm_star.where(m <= 20, rotm)
-
-    return rotm
+    dtime = dtime + (lon / (15*np.pi/180.0))
+    return (np.pi / 12.0) * (dtime + sc - 12.0)
 
 
-def beam_irradiance_normal_clear(G0, Tl2, m, rotm, h0):
+def inst_solar_radiation_toa(csza, iesd):
     r"""
-    Computes the clear sky beam irradiance normal to the solar beam.
+    Computes the instantaneous solar radiation at the top of
+    the atmosphere [Wm-2].
 
     .. math ::
 
-        B_{0c}=G_{0} \cdot \exp\left(-0.8662 \cdot T_{LK} \cdot m \cdot \delta_{R}\right)
+        S_{toa}^{i} = S_{sun} \cdot d_{r} \cdot \phi
 
     Parameters
     ----------
-    G0 : float
-        ext rad normal to solar beam, 
-        :math:`G_0`
-        [W/m2]
-    Tl2 : float
-        airmass  2 Linke atmospheric turbidity factor, 
-        :math:`T_{LK}`
+    csza : float
+        cosine solar zenith angle, 
+        :math:`\phi`
         [-]
-    m : float
-        relative optical airmass, 
-        :math:`m`
-        [-]
-    rotm : float
-        Rayleigh optical thickness at airmass m, 
-        :math:`\delta_{R}`
-        [-]
-    h0 : float
-        solar elevation angle, 
-        :math:`h_0`
-        [degrees]
+    iesd : float
+        inverse earth sun distance, 
+        :math:`d_{r}`
+        [AU]
 
     Returns
     -------
-    B0c : float
-        beam irradiance normal to the solar beam, 
-        :math:`B_{0c}`
-        [W/m2]
+    ra_i_toa : float
+        instantaneous solar radiation at top of atmosphere, 
+        :math:`S_{toa}^{i}`
+        [Wm-2]
 
+    Examples
+    --------
+    >>> import ETLook.solar_radiation as solrad
+    >>> doy = 1
+    >>> sc = solrad.seasonal_correction(doy)
+    >>> ha = solrad.hour_angle(sc, dtime=12)
+    >>> decl = solrad.declination(doy)
+    >>> csza = solrad.cosine_solar_zenith_angle(ha, decl, 0)
+    >>> iesd = solrad.inverse_earth_sun_distance(doy)
+    >>> solrad.inst_solar_radiation_toa(csza, iesd)
+    1299.9181944414036
     """
-    B0c = G0 * np.exp(-0.8662 * Tl2 * m * rotm)
-    if isinstance(B0c, np.ndarray):
-        B0c[h0 < 0] = 0
-    else:
-        B0c = B0c.where(h0 >= 0, 0)
-
-    return B0c
+    return csza * con.sol * iesd
 
 
-def beam_irradiance_horizontal_clear(B0c, h0):
+def daily_solar_radiation_toa(sc, decl, iesd, lat, slope=0, aspect=0):
     r"""
-    Computes the clear sky beam irradiance on a horizontal surface.
+    Computes the daily solar radiation at the top of the atmosphere.
 
     .. math ::
 
-        B_{hc} = B_{0c} \cdot \sin\left(h_{0}\right)
+        S_{toa}=S_{sun} \cdot d_{r}\int_{i=-\pi}^{i=\pi}S_{toa}^{i}
 
     Parameters
     ----------
-    B0c : float
-        beam irradiance normal to the solar beam, 
-        :math:`B_{0c}`
-        [W/m2]
-    h0 : float
-        solar elevation angle, 
-        :math:`h_0`
-        [degrees]
+    iesd : float
+        inverse earth sun distance, 
+        :math:`d_{r}`
+        [AU]
+    decl : float
+        solar declination, 
+        :math:`\delta`
+        [rad]
+    sc : float
+        seasonal correction, 
+        :math:`s_{c}`
+        [hours]
+    lat : float
+        latitude, 
+        :math:`\lambda`
+        [rad]
+    slope : float
+        slope, 
+        :math:`\Delta`
+        [rad]
+    aspect : float
+        aspect (0 is north; pi is south), 
+        :math:`\alpha`
+        [rad]
 
     Returns
     -------
-    Bhc : float
-        beam irradiance at a horizontal surface, 
-        :math:`B_{hc}`
-        [W/m2]
+    ra_24_toa : float
+        daily solar radiation at the top of atmosphere, 
+        :math:`S_{toa}`
+        [Wm-2]
 
+    Examples
+    --------
+    >>> import ETLook.solar_radiation as solrad
+    >>> from math import pi
+    >>> doy = 1
+    >>> sc = solrad.seasonal_correction(doy)
+    >>> decl = solrad.declination(doy)
+    >>> iesd = solrad.inverse_earth_sun_distance(doy)
+    >>> solrad.daily_solar_radiation_toa(sc, decl, iesd, lat=25*pi/180.0)
+    265.74072308978026
     """
-    Bhc = B0c * np.sin(h0 * np.pi / 180)
-    if isinstance(Bhc, np.ndarray):
-        Bhc[h0 < 0] = 0
-    else:
-        Bhc = Bhc.where(h0 >= 0, 0)
 
-    return Bhc
+    # hour angle for the whole day in half-hourly intervals (0:15-23:45)
+    t_start = 0.25
+    t_end = 24.00
+    interval = 0.5
+    times = [t_start+i*interval for i in range(0, 48)]
+    hours = [hour_angle(sc, t) for t in times]
+
+    ra24 = 0
+
+    for t in hours:
+        csza = cosine_solar_zenith_angle(t, decl, lat, slope, aspect)
+        ra24 += inst_solar_radiation_toa(csza, iesd) / len(hours)
 
+    # return the average daily radiation
+    return ra24
 
-def linke_turbidity(wv_i, aod550_i, p_air_i, p_air_0_i):
+
+def cosine_solar_zenith_angle(ha, decl, lat, slope=0, aspect=0):
     r"""
-    Computes the air mass 2 Linke atmospheric turbidity factor.
+    computes the cosine of the solar zenith angle [-].
 
     .. math ::
 
-        p_{rel} &= \frac{p}{p_{0}} \\
-        T_{LK} &= 3.91 \cdot \tau_{550} \cdot e^{0.689p_{rel}}+0.376 \cdot \ln\left(TCWV\right)+\left(2+0.54 \cdot p_{rel}-0.34 \cdot p_{rel}^{2}\right)
+        \phi = & \sin\left(\delta\right) \cdot \sin\left(\lambda\right) \cdot  \cos\left(\Delta\right) - \\
+        & \sin\left(\delta\right) \cdot \cos\left(\lambda\right) \cdot \sin\left(\Delta\right) + \\
+        & \cos\left(\delta\right) \cdot \cos\left(\lambda\right) \cdot \cos\left(\Delta\right) \cdot \cos\left(\omega\right)+\\
+        & \cos\left(\delta\right) \cdot \sin\left(\lambda\right) \cdot \sin\left(\Delta\right) \cdot \sin\left(\alpha\right) \cdot \cos\left(\omega\right)+\\
+        & \cos\left(\delta\right) \cdot \sin\left(\Delta\right) \cdot  \sin\left(\alpha\right) \cdot \sin\left(\omega\right)
 
     Parameters
     ----------
-    wv_i : float
-        total column atmospheric water vapor, 
-        :math:`TCWV`
-        [kg m-2]
-    aod550_i : float
-        Aerosol optical depth at 550nm, 
-        :math:`aod550`
-        [-]
-    p_air_i : float
-        actual instantaneous air pressure, 
-        :math:`p`
-        [hPa]
-    p_air_0_i : float
-        air pressure at sea level, 
-        :math:`p_0`
-        [-]
+    ha : float
+        hour angle, 
+        :math:`\omega`
+        [rad]
+    decl : float
+        declination, 
+        :math:`\delta`
+        [rad]
+    lat : float
+        latitude, 
+        :math:`\lambda`
+        [rad]
+    slope : float
+        slope, 
+        :math:`\Delta`
+        [rad]
+    aspect : float
+        aspect (0 is north; pi is south), 
+        :math:`\alpha`
+        [rad]
 
     Returns
     -------
-    Tl2 : float
-        Airmass 2 Linke atmospheric turbidity factor, 
-        :math:`T_{LK}`
+    csza : float
+        cosine solar zenith angle, 
+        :math:`\phi`
         [-]
 
     Examples
     --------
-    """
-    # prel = p0 / p # Papers mixes p/p0 and p0/p????
-    prel = p_air_i / p_air_0_i
+    >>> import ETLook.solar_radiation as solrad
+    >>> sc = solrad.seasonal_correction(1)
+    >>> ha = solrad.hour_angle(sc, dtime=12)
+    >>> solrad.cosine_solar_zenith_angle(ha, decl=solrad.declination(1), lat=0)
+    0.92055394167363314
+    """
+    t1 = np.sin(decl) * np.sin(lat) * np.cos(slope)
+    t2 = np.sin(decl) * np.cos(lat) * np.sin(slope) * np.cos(aspect - np.pi)
+    t3 = np.cos(decl) * np.cos(lat) * np.cos(slope)
+    t4 = np.cos(decl) * np.sin(lat) * np.sin(slope) * np.cos(aspect - np.pi)
+    t5 = np.cos(decl) * np.sin(slope) * np.sin(aspect - np.pi)
+    csza = t1 - t2 + t3 * np.cos(ha) + t4 * np.cos(ha) + t5 * np.sin(ha)
+
+    # check if the sun is above the horizon
+    check = np.sin(decl) * np.sin(lat) + np.cos(decl) * \
+        np.cos(lat) * np.cos(ha)
+
+    if isinstance(csza, xr.DataArray):
+        res = xr.where((csza > 0) & (check >= 0), csza, 0)
+        res = xr.where(csza.notnull() | check.notnull(), res, np.nan)
+    else:
+        nans = np.logical_or(np.isnan(csza), np.isnan(check))
+        res = np.where(np.logical_and(csza > 0, check >= 0), csza, 0)
+        res[nans] = np.nan
+
+    return res
+
 
-    term1 = 3.91 * np.exp(0.689 * prel) * aod550_i
-    term2 = 0.376 * np.log(wv_i)
+def transmissivity(ra, ra_flat):
+    """Computes the transmissivity.
 
-    Tl2 = term1 + term2 + (2 + 0.54 * prel - 0.5 * prel**2 + 0.16 * prel**2)
+    Parameters
+    ----------
+    ra_24 : float
+        daily solar radiation for a flat surface, 
+        :math:`S^{\downarrow}`
+        [Wm-2]
+    ra_24_toa_flat : float
+        daily solar radiation at the top of atmosphere for a flat surface, 
+        :math:`S_{toa,f}`
+        [Wm-2]
 
-    return Tl2
+    Returns
+    -------
+    trans_24 : float
+        daily atmospheric transmissivity, 
+        :math:`\tau`
+        [-]
+    """
+    return ra / ra_flat
 
 
-def diffuse_irradiance_horizontal_clear(G0, Tl2, h0):
+def daily_solar_radiation_toa_flat(decl, iesd, lat, ws):
     r"""
-    Computes the clear sky beam irradiance on a horizontal surface.
+    Computes the daily solar radiation at the top of the atmosphere for a flat
+    surface.
 
     .. math ::
 
-        D_{hc}=G_{0} \cdot Tn\left(T_{LK}\right) \cdot F_{d}\left(h_{0}\right)
+        S_{toa,f}=\frac{S_{sun}}{\pi} \cdot d_{inv,r} \cdot (w_{s} \cdot \sin(\lambda) \cdot \sin(\delta) +
+                  \cos(\lambda)\cdot\cos(\delta)\cdot\sin(w_{s}))
 
-    For the estimation of the transmission function :math:`Tn\left(T_{LK}\right)`
-    the following function is used:
-
-    .. math ::
+    Parameters
+    ----------
+    decl : float
+        solar declination, 
+        :math:`\delta`
+        [rad]
+    iesd : float
+        inverse earth sun distance, 
+        :math:`d_{inv,r}`
+        [AU]
+    lat : float
+        latitude, 
+        :math:`\lambda`
+        [rad]
+    ws : float
+        sunset hour angle, 
+        :math:`w_{s}`
+        [rad]
 
-        Tn\left(T_{LK}\right)=-0.015843+0.030543 \cdot T_{LK}+0.0003797 \cdot T_{LK}^{2}
+    Returns
+    -------
+    ra_24_toa_flat : float
+        daily solar radiation at the top of atmosphere for a flat surface, 
+        :math:`S_{toa,f}`
+        [Wm-2]
 
-    The solar altitude function :math:`F_{d}\left(h_{0}\right)` is evaluated using the expression:
+    """
+    ra_flat = (con.sol / np.pi) * iesd * (ws * np.sin(lat) * np.sin(decl) +
+                                        np.cos(lat) * np.cos(decl) * np.sin(ws))
 
-    .. math ::
+    return ra_flat
 
-        F_{d}\left(h_{0}\right)=A_{1}+A_{2} \cdot \sin (h_{0})+A_{3} \cdot sin^{2}(h_{0})
 
-    with:
+def daily_solar_radiation_flat(ra_24_toa_flat, trans_24):
+    r"""
+    Computes the daily solar radiation at the earth's surface.
 
     .. math ::
 
-        A_{1}^{\prime} &= 0.26463-0.061581 \cdot T_{LK}+0.0031408 \cdot T_{LK}^{2} \\
-        A_{1} &= \frac{0.0022}{Tn\left(T_{LK}\right)} \: \text{if} \: A_{1}^{\prime} \cdot Tn\left(T_{LK}\right)<0.0022 \\
-        A_{1} &= A_{1}^{\prime} \: \text{if} \: A_{1}^{\prime} \cdot Tn\left(T_{LK}\right)\geq0.0022 \\
-        A_{2} &= 2.04020+0.018945 \cdot T_{LK}-0.011161 \cdot T_{LK}^{2} \\
-        A_{3} &= -1.3025+0.039231 \cdot T_{LK}+0.0085079 \cdot T_{LK}^{2}
+        S^{\downarrow} = \tau \cdot S_{toa}
 
     Parameters
     ----------
-    G0 : float
-        ext rad normal to solar beam, 
-        :math:`G_0`
-        [W/m2]
-    Tl2 : float
-        Airmass 2 Linke atmospheric turbidity factor, 
-        :math:`T_{LK}`
+    ra_24_toa_flat : float
+        daily solar radiation at the top of atmosphere for a flat surface, 
+        :math:`S_{toa}`
+        [Wm-2]
+    trans_24 : float
+        daily atmospheric transmissivity, 
+        :math:`\tau`
         [-]
-    h0 : float
-        solar elevation angle, 
-        :math:`h_0`
-        [degrees]
 
     Returns
     -------
-    Dhc : float
-        Diffuse irradiance at a horizontal surface, 
-        :math:`D_{hc}`
-        [W/m2]
+    ra_24 : float
+        daily solar radiation for a flat surface, 
+        :math:`S^{\downarrow}`
+        [Wm-2]
 
-    Examples
-    --------
     """
-    h0_rad = h0 * np.pi / 180.
-    TnTl2 = -0.015843 + 0.030543 * Tl2 + 0.0003797 * Tl2**2
+    return ra_24_toa_flat * trans_24
 
-    A1 = 0.26463 - 0.061581 * Tl2 + 0.0031408 * Tl2**2
-    if isinstance(A1, xr.DataArray):
-        A1 = xr.where((A1 * TnTl2) < 0.0022, 0.0022 / TnTl2, A1)
-    else:
-        A1 = np.where((A1 * TnTl2) < 0.0022, 0.0022 / TnTl2, A1)
-    A2 = 2.04020 + 0.018945 * Tl2 - 0.011161 * Tl2**2
-    A3 = -1.3025 + 0.039231 * Tl2 + 0.0085079 * Tl2**2
 
-    FdH0 = A1 + A2 * np.sin(h0_rad) + A3 * np.sin(h0_rad)**2
+def diffusion_index(trans_24, diffusion_slope=-1.33, diffusion_intercept=1.15):
+    r"""
+    Computes the diffusion index, the ratio between diffuse and direct
+    solar radiation. The results are clipped between 0 and 1.
 
-    Dhc = G0 * TnTl2 * FdH0
+    .. math ::
 
-    if isinstance(Dhc, np.ndarray):
-        Dhc[Dhc < 0] = 0
-    else:
-        Dhc = Dhc.where(Dhc >= 0, 0)
-    
-    return Dhc
+        I_{diff} = a_{diff}+b_{diff} \cdot \tau
+
+    Parameters
+    ----------
+    trans_24 : float
+        daily atmospheric transmissivity, 
+        :math:`\tau`
+        [-]
+    diffusion_slope : float
+        slope of diffusion index vs transmissivity relationship, 
+        :math:`b_{diff}`
+        [-]
+    diffusion_intercept : float
+        intercept of diffusion index vs transmissivity relationship, 
+        :math:`a_{diff}`
+        [-]
+
+    Returns
+    -------
+    diffusion_index : float
+        diffusion_index, 
+        :math:`I_{diff}`
+        [-]
+
+    """
+    res = diffusion_intercept + trans_24 * diffusion_slope
 
+    res = np.clip(res, 0, 1)
 
-def ra_clear_horizontal(Bhc, Dhc):
-    r"""    
-    Computes the clear sky beam irradiance on a horizontal surface.
+    return res
+
+
+def daily_total_solar_radiation(ra_24_toa, ra_24_toa_flat, diffusion_index, trans_24):
+    r"""
+    Computes the daily solar radiation at the earth's surface taken
+    diffuse and direct solar radiation into account.
 
     .. math ::
 
-        G_{hc}=B_{hc}+D_{hc}
+        S^{\downarrow} = I_{diff} \cdot \tau \cdot S_{toa,f} +(1-I_{diff}) \cdot \tau \cdot S_{toa}
 
     Parameters
     ----------
-    Bhc : float
-        beam irradiance at a horizontal surface, 
-        :math:`B_{hc}`
-        [W/m2]
-    Dhc : float
-        Diffuse irradiance at a horizontal surface, 
-        :math:`D_{hc}`
-        [W/m2]
-        
+    ra_24_toa : float
+        daily solar radiation at the top of atmosphere, 
+        :math:`S_{toa}`
+        [Wm-2]
+    ra_24_toa_flat : float
+        daily solar radiation at the top of atmosphere for a flat surface, 
+        :math:`S_{toa,f}`
+        [Wm-2]
+    diffusion_index : float
+        diffusion_index, 
+        :math:`I_{diff}`
+        [-]
+    trans_24 : float
+        daily atmospheric transmissivity, 
+        :math:`\tau`
+        [-]
+
     Returns
     -------
-    ra_hor_clear_i : float
-        Total clear-sky irradiance on a horizontal surface, 
-        :math:`G_{hc}`
-        [W/m2]
+    ra_24 : float
+        daily solar radiation, 
+        :math:`S^{\downarrow}`
+        [Wm-2]
 
-    Examples
-    --------
     """
-    ra_clear_hor = Bhc + Dhc
-    
-    return ra_clear_hor
+    diffuse = trans_24 * ra_24_toa_flat * diffusion_index
+    direct = trans_24 * ra_24_toa * (1 - diffusion_index)
+    return diffuse + direct
+
```

### Comparing `pywapor-3.3.4/pywapor/general/aligner.py` & `pywapor-3.3.5/pywapor/general/aligner.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,20 @@
 
     # Apply variable specific enhancers
     variables = levels.find_setting(sources, "variable_enhancers")
     for var in variables:
         for func in sources[var]["variable_enhancers"]:
             dss2 = func(dss2, var, folder)
 
+    # TODO this info needs to be moved to `sources`.
+    vars_for_sharpening = ['nmdi', 'bsi', 'mndwi', 'cos_solar_zangle', 'vari_red_edge', 'psri', 'nir', 'green']
+    for x in vars_for_sharpening:
+        if x in dss2.keys():
+            _ = dss2.pop(x)
+
     # Align all the variables together.
     example_source = levels.find_setting(sources, "is_example", min_length = 1)
     if len(example_source) == 1:
         example_ds = dss[example_source[0]]
         log_example_ds(example_ds)
     elif len(example_source) == 0:
         example_ds = None
```

### Comparing `pywapor-3.3.4/pywapor/general/bitmasks.py` & `pywapor-3.3.5/pywapor/general/bitmasks.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/compositer.py` & `pywapor-3.3.5/pywapor/general/compositer.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/curvilinear.py` & `pywapor-3.3.5/pywapor/general/curvilinear.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/lazifier.py` & `pywapor-3.3.5/pywapor/general/lazifier.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/levels.py` & `pywapor-3.3.5/pywapor/general/levels.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 example_sources.append(var)
     if len(example_sources) > max_length:
             log.warning(f"--> Found more than {max_length} products for `{setting_str}`.")
     if len(example_sources) > max_length or len(example_sources) < min_length:
         log.warning(f"--> Didn't find any products for `{setting_str}`.")
     return example_sources
 
-def pre_et_look_levels(level = "level_1", bin_length = "DEKAD"):
+def pre_et_look_levels(level = "level_1", bin_length = 1):
     """Create a default `pre_et_look` `sources` dictionary.
 
     Parameters
     ----------
     level : "level_1" | "level_2" | "level_3" | "level_2_v3"
         For which level to create the `sources`, by default "level_1".
     bin_length : str, optional
@@ -474,16 +474,23 @@
             "products": [
                 {
                     "source": se_root_dler,
                     "product_name": "v3",
                     "enhancers": "default",
                 },
             ],
-            "composite_type": "max",
-            "temporal_interp": None,
+            "composite_type": "mean",
+            "temporal_interp":  {
+                                "method": "whittaker",
+                                # "plot_folder": r"",
+                                # "a": 0.65,
+                                "valid_drange": [0.0, 1.0],
+                                "max_dist": np.timedelta64(15, "D"),
+                                "lambdas": 100.,
+                    },
             "spatial_interp": "bilinear",
         }
 
     level_2_v3["p"] = {
         "products": [
             {
                 "source": "CHIRPS",
@@ -570,24 +577,69 @@
                     'product_name': "WaPOR3",
                     'enhancers': 'default'
                 },
             ],
         'composite_type': None,
         'temporal_interp': None,
         'spatial_interp': 'bilinear'}
-    
 
+    level_3_v3 = copy.deepcopy(level_2_v3)
+
+    SRs = [
+                {
+                    "source": "SENTINEL2",
+                    "product_name": "S2MSI2A_R20m",
+                    "enhancers": "default",
+                    "is_example": True
+                },
+                {
+                    "source": "LANDSAT",
+                    "product_name": "LT05_SR",
+                    "enhancers": "default",
+                },
+                {
+                    "source": "LANDSAT",
+                    "product_name": "LE07_SR",
+                    "enhancers": "default",
+                },
+                {
+                    "source": "LANDSAT",
+                    "product_name": "LC08_SR",
+                    "enhancers": "default",
+                },
+                {
+                    "source": "LANDSAT",
+                    "product_name": "LC09_SR",
+                    "enhancers": "default",
+                },
+            ]
+    
+    level_3_v3["ndvi"]["products"] = SRs
+    level_3_v3["r0"]["products"] = SRs
+    level_3_v3["z"] = {
+        "products": [
+            {
+                "source": "COPERNICUS",
+                "product_name": "GLO30",
+                "enhancers": "default",
+            },
+        ],
+        "composite_type": None,
+        "temporal_interp": None,
+        "spatial_interp": "bilinear",
+        }
 
 
     levels = {
             "level_1": level_1,
             "level_2": level_2,
             "level_3": level_3,
 
-            "level_2_v3": level_2_v3
+            "level_2_v3": level_2_v3,
+            "level_3_v3": level_3_v3,
                 }
 
     return levels[level]
 
 def pre_se_root_levels(level = "level_1"):
     """Create a default `pre_se_root` `sources` dictionary.
 
@@ -850,21 +902,15 @@
             {
                 "source": "SENTINEL2",
                 "product_name": "S2MSI2A_R60m",
                 "enhancers": "default",
                 "is_example": True
             },
         ],
-        "temporal_interp":  {
-                    "method": "whittaker",
-                    # "plot_folder": r"",
-                    "valid_drange": [-1.0, 1.0],
-                    "max_dist": np.timedelta64(15, "D"),
-                    "lambdas": 100.,
-        },
+        "temporal_interp": "linear",
         "spatial_interp": "nearest"}
 
     for var in ["mndwi", "psri", "vari_red_edge", "bsi", "nmdi", "green", "nir"]:
         level_2_v3[var] = {
             'products': [{
                 'source': 'SENTINEL2',
                 'product_name': 'S2MSI2A_R60m',
@@ -878,22 +924,27 @@
             {
                 'source': 'VIIRSL1',
                 'product_name': 'VNP02IMG',
                 'enhancers': 'default'
             },
         ],
         'variable_enhancers': [sharpen],
-        "temporal_interp":  {
-                    "method": "whittaker",
-                    # "plot_folder": r"",
-                    "a": 0.95,
-                    # "valid_drange": [-1.0, 1.0],
-                    "max_dist": np.timedelta64(15, "D"),
-                    "lambdas": 100.,
-        },
+        "temporal_interp": None,
+        'spatial_interp': 'nearest'}
+
+    level_2_v3["lst"] = {
+        'products': [
+            {
+                'source': 'SENTINEL3',
+                'product_name': 'SL_2_LST___',
+                'enhancers': 'default'
+            },
+        ],
+        'variable_enhancers': [sharpen],
+        "temporal_interp": None,
         'spatial_interp': 'nearest'}
 
     for var in ["u", "t_dew", "p_air_0", "p_air", "t_air", "wv"]:
         level_2_v3[var] = {
             'products': [
                 {
                     'source': 'ERA5',
@@ -924,29 +975,97 @@
                     'product_name': "WaPOR2",
                     'enhancers': 'default'
                 },
             ],
         'temporal_interp': "linear",
         'spatial_interp': 'bilinear'}
 
+    level_3_v3 = copy.deepcopy(level_2_v3)
+
+    SRs = [
+                {
+                    "source": "SENTINEL2",
+                    "product_name": "S2MSI2A_R20m",
+                    "enhancers": "default",
+                    "is_example": True
+                },
+                # {
+                #     "source": "LANDSAT",
+                #     "product_name": "LT05_SR",
+                #     "enhancers": "default",
+                # },
+                # {
+                #     "source": "LANDSAT",
+                #     "product_name": "LE07_SR",
+                #     "enhancers": "default",
+                # },
+                # {
+                #     "source": "LANDSAT",
+                #     "product_name": "LC08_SR",
+                #     "enhancers": "default",
+                # },
+                # {
+                #     "source": "LANDSAT",
+                #     "product_name": "LC09_SR",
+                #     "enhancers": "default",
+                # },
+            ]
+
+    for var in ["ndvi", "mndwi", "psri", "vari_red_edge", "bsi", "nmdi", "green", "nir"]:
+        level_3_v3[var]["products"] = SRs
+
+    level_3_v3["lst"] = {
+        'products': [
+                {
+                    "source": "LANDSAT",
+                    "product_name": "LT05_ST",
+                    "enhancers": "default",
+                },
+                {
+                    "source": "LANDSAT",
+                    "product_name": "LE07_ST",
+                    "enhancers": "default",
+                },
+                {
+                    "source": "LANDSAT",
+                    "product_name": "LC08_ST",
+                    "enhancers": "default",
+                },
+                {
+                    "source": "LANDSAT",
+                    "product_name": "LC09_ST",
+                    "enhancers": "default",
+                },
+        ],
+        'variable_enhancers': [sharpen],
+        "temporal_interp": None,
+        'spatial_interp': 'nearest'}
+
     levels = {
                 "level_1": level_1,
                 "level_2": level_2,
                 "level_3": level_3,
+                "level_1_v2": level_1,
+                "level_2_v2": level_2,
+                "level_3_v2": level_3,
+
                 "level_2_v3": level_2_v3,
+                "level_3_v3": level_3_v3,
                 }
 
     return levels[level]
 
 if __name__ == "__main__":
 
-    et_look_sources_lvl1 = pre_et_look_levels(level = "level_1", bin_length = "DEKAD")
-    et_look_sources_lvl2 = pre_et_look_levels(level = "level_2", bin_length = "DEKAD")
-    et_look_sources_lvl3 = pre_et_look_levels(level = "level_3", bin_length = "DEKAD")
-    et_look_sources_lvl2_v3 = pre_et_look_levels(level = "level_2_v3", bin_length = "DEKAD")
+    et_look_sources_lvl1 = pre_et_look_levels(level = "level_1")
+    et_look_sources_lvl2 = pre_et_look_levels(level = "level_2")
+    et_look_sources_lvl3 = pre_et_look_levels(level = "level_3")
+    et_look_sources_lvl2_v3 = pre_et_look_levels(level = "level_2_v3")
+    et_look_sources_lvl3_v3 = pre_et_look_levels(level = "level_3_v3")
 
     se_root_sources_lvl1 = pre_se_root_levels(level = "level_1")
     se_root_sources_lvl2 = pre_se_root_levels(level = "level_2")
     se_root_sources_lvl3 = pre_se_root_levels(level = "level_3")
     se_root_sources_lvl2_v3 = pre_se_root_levels(level = "level_2_v3")
+    se_root_sources_lvl3_v3 = pre_se_root_levels(level = "level_3_v3")
```

### Comparing `pywapor-3.3.4/pywapor/general/logger.py` & `pywapor-3.3.5/pywapor/general/logger.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/network.py` & `pywapor-3.3.5/pywapor/general/network.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/performance.py` & `pywapor-3.3.5/pywapor/general/performance.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/pre_defaults.py` & `pywapor-3.3.5/pywapor/general/pre_defaults.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/processing_functions.py` & `pywapor-3.3.5/pywapor/general/processing_functions.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/reproject.py` & `pywapor-3.3.5/pywapor/general/reproject.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/units.py` & `pywapor-3.3.5/pywapor/general/units.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/general/variables.py` & `pywapor-3.3.5/pywapor/general/variables.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/post_et_look.py` & `pywapor-3.3.5/pywapor/post_et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.4/pywapor/pre_et_look.py` & `pywapor-3.3.5/pywapor/pre_et_look.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 def add_constants_new(ds, *args): # TODO make sure this only adds constants for et_look, not for se_root.
     c = defaults.constants_defaults()
     for var, value in c.items():
         if var not in ds.data_vars:
             ds[var] = value
     return ds
 
-def main(folder, latlim, lonlim, timelim, sources = "level_1", bin_length = "DEKAD", enhancers = [lapse_rate]):
+def main(folder, latlim, lonlim, timelim, sources = "level_1", bin_length = 1, enhancers = [lapse_rate]):
     """Prepare input data for `et_look`.
 
     Parameters
     ----------
     folder : str
         Path to folder in which to store (intermediate) data.
     latlim : list
```

### Comparing `pywapor-3.3.4/pywapor/pre_se_root.py` & `pywapor-3.3.5/pywapor/pre_se_root.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 def add_constants_new(ds, *args): # TODO make sure this only adds constants for et_look, not for se_root.
     c = defaults.constants_defaults()
     for var, value in c.items():
         if var not in ds.data_vars:
             ds[var] = value
     return ds
 
-def main(folder, latlim, lonlim, timelim, sources = "level_1", bin_length = "DEKAD", enhancers = [], buffer_timelim = True, **kwargs):
+def main(folder, latlim, lonlim, timelim, sources = "level_1", bin_length = 1, enhancers = [], buffer_timelim = True, **kwargs):
     """Prepare input data for `se_root`.
 
     Parameters
     ----------
     folder : str
         Path to folder in which to store (intermediate) data.
     latlim : list
```

### Comparing `pywapor-3.3.4/pywapor/se_root.py` & `pywapor-3.3.5/pywapor/se_root.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import xarray as xr
 import os
 import numpy as np
 import warnings
 import pandas as pd
 import datetime
 import pywapor.general as g
-import pywapor.general.processing_functions as PF
-import pywapor.et_look_dev as ETLook_dev
 import pywapor.et_look_v2_v3 as ETLook_v2_v3
 from pywapor.general.logger import log, adjust_logger
 from pywapor.enhancers.other import drop_empty_times
 from pywapor.general.processing_functions import save_ds, open_ds
 import copy
 import pywapor.pre_se_root as pre_se_root
 from pywapor.general import levels
@@ -59,15 +57,15 @@
 def main(input_data, se_root_version = "v2", export_vars = "default", chunks = {"time": 1, "x": 1000, "y": 1000}):
     """Run the `se_root` model.
 
     Parameters
     ----------
     input_data : str | xr.Dataset
         (Path to) dataset generated by `pywapor.pre_se_root`.
-    se_root_version : "v2" | "v3" | "dev", optional
+    se_root_version : "v2" | "v3", optional
         Which version of the SERoot model to use, by default "v2".
     export_vars : "default" | "all" | list, optional
         Specify which variables to save inside the output file. `"Default"` only 
         stores `se_root`. `"all"` stores all calculated variables. Use a
         list to specify a custom output set, by default "default".
     chunks : dict, optional
         Specify how the calculations are split up. Increase chunk sizes to speed up calculation, 
@@ -88,47 +86,37 @@
 
     _ = adjust_logger(True, os.path.split(input_data)[0], "INFO")
 
     t1 = datetime.datetime.now()
     log.info("> SE_ROOT").add()
 
     # Version
-    if se_root_version == "v2" or se_root_version == "v3":
-        ETLook = ETLook_v2_v3
-    elif se_root_version == "dev":
-        ETLook = ETLook_dev
+    ETLook = ETLook_v2_v3
 
     log.info(f"--> Running `se_root` ({se_root_version}).")
 
     # Allow skipping of et_look-functions if not all of its required inputs are
     # available.
     g.lazifier.decorate_submods(ETLook, g.lazifier.etlook_decorator)
 
     ds = g.variables.initiate_ds(ds)
 
     fp, fn = os.path.split(input_data)
 
-    if se_root_version == "dev":
-        ds["z0m_full"] = 0.04 + 0.01 * (ds.pixel_size - 30)/(250-30)
-        ds["lst_zone_mean"] = lst_zone_mean(ds)
-
     if not ds["v2m_i"].dtype == object and not ds["u2m_i"].dtype == object:
         ds["u_i"] = np.sqrt(ds["v2m_i"]**2 + ds["u2m_i"]**2)
 
     doy = [int(pd.Timestamp(x).strftime("%j")) for x in ds["time"].values]
     ds["doy"] = xr.DataArray(doy, coords = ds["time"].coords).chunk("auto")
     dtime = [pd.Timestamp(x).hour + (pd.Timestamp(x).minute / 60) for x in ds["time"].values]
     ds["dtime"] = xr.DataArray(dtime, coords = ds["time"].coords).chunk("auto")
     ds["sc"] = ETLook.solar_radiation.seasonal_correction(ds["doy"])
     ds["decl"] = ETLook.solar_radiation.declination(ds["doy"])
     ds["day_angle"] = ETLook.clear_sky_radiation.day_angle(ds["doy"])
 
-    if se_root_version == "dev":
-        ds["t_air_i"] = xr.where(ds["t_air_i"] < -270, np.nan, ds["t_air_i"])
-
     ds["p_air_i"] = ETLook.meteo.air_pressure_kpa2mbar(ds["p_air_i"])
     ds["p_air_0_i"] = ETLook.meteo.air_pressure_kpa2mbar(ds["p_air_0_i"])
 
     ds["vc"] = ETLook.leaf.vegetation_cover(ds["ndvi"], nd_min = ds["nd_min"], nd_max = ds["nd_max"], vc_pow = ds["vc_pow"])
 
     ds["t_air_k_i"] = ETLook.meteo.air_temperature_kelvin_inst(ds["t_air_i"])
 
@@ -188,21 +176,16 @@
 
     ds["t_max_bare"] = ETLook.soil_moisture.maximum_temperature_bare(ds["ra_hor_clear_i"], ds["emiss_atm_i"], ds["t_air_k_i"], ds["ad_i"], ds["raa"], ds["ras"], ds["r0_bare"])
     ds["t_max_full"] = ETLook.soil_moisture.maximum_temperature_full(ds["ra_hor_clear_i"], ds["emiss_atm_i"], ds["t_air_k_i"], ds["ad_i"], ds["rac"], ds["r0_full"])
 
     ds["t_wet_i"] = ETLook.soil_moisture.wet_bulb_temperature_inst_new(ds["t_air_i"], ds["qv_i"], ds["p_air_i"])
     ds["lst_max"] = ETLook.soil_moisture.maximum_temperature(ds["t_max_bare"], ds["t_max_full"], ds["vc"])
 
-    if se_root_version == "v2" or se_root_version == "v3":
-        ds["t_wet_k_i"] = ETLook.meteo.wet_bulb_temperature_kelvin_inst(ds["t_wet_i"])
-        ds["lst_min"] = ETLook.soil_moisture.minimum_temperature(ds["t_wet_k_i"], ds["t_air_k_i"], ds["vc"])
-    elif se_root_version == "dev":
-        ds["t_min_bare"] = ETLook.soil_moisture.minimum_temperature_bare(ds["ra_hor_clear_i"], ds["emiss_atm_i"], ds["t_air_k_i"], ds["ad_i"], ds["raa"], ds["ras"], ds["lst_zone_mean"], r0_bare_wet = ds["r0_bare_wet"])
-        ds["t_min_full"] = ETLook.soil_moisture.minimum_temperature_full(ds["ra_hor_clear_i"], ds["emiss_atm_i"], ds["t_air_k_i"], ds["ad_i"], ds["rac"], ds["lst_zone_mean"], ds["r0_full"])  
-        ds["lst_min"] = ETLook.soil_moisture.maximum_temperature(ds["t_min_bare"], ds["t_min_full"], ds["vc"])
+    ds["t_wet_k_i"] = ETLook.meteo.wet_bulb_temperature_kelvin_inst(ds["t_wet_i"])
+    ds["lst_min"] = ETLook.soil_moisture.minimum_temperature(ds["t_wet_k_i"], ds["t_air_k_i"], ds["vc"])
 
     ds["se_root"] = ETLook.soil_moisture.soil_moisture_from_maximum_temperature(ds["lst_max"], ds["lst"], ds["lst_min"])
 
     if export_vars == "all":
         keep_vars = [var for var in ds.data_vars if "x" in ds[var].dims and "y" in ds[var].dims]
         ds = ds[keep_vars]
     elif export_vars == "default":
@@ -233,57 +216,14 @@
             ds = save_ds(ds, fp_out, encoding = "initiate", chunks = chunks, label = f"Saving output to `{fn}`.")
 
     t2 = datetime.datetime.now()
     log.sub().info(f"< SE_ROOT ({str(t2 - t1)})")
 
     return ds
 
-def lst_zone_mean(ds):
-    # TODO This function needs to be replaced by something like pywapor.enhancers.temperature.local_mean
-
-    geo_ex = ds.geotransform
-    proj_ex = ds.projection
-
-    size_y, size_x = ds["ndvi"].isel(time = 0).shape
-    size_y_zone = int(np.ceil(size_y/200))
-    size_x_zone = int(np.ceil(size_x/200)) 
-    array_fake = np.ones([size_y_zone, size_x_zone])
-    geo_new = tuple([geo_ex[0], geo_ex[1] * 200, geo_ex[2], geo_ex[3], geo_ex[4], geo_ex[5]*200])
-    MEM_file = PF.Save_as_MEM(array_fake, geo_new, proj_ex)
-
-    lst_zone_mean_full = np.ones_like(ds["ndvi"] * np.nan)
-
-    for i, t in enumerate(ds.time):
-
-        lst = ds["lst"].sel(time = t).values
-        lst_filename = PF.Save_as_MEM(lst, geo_new, proj_ex)
-        
-        dest_lst_zone_large = PF.reproject_dataset_example(lst_filename, MEM_file, 4)
-        lst_zone_mean_large = dest_lst_zone_large.GetRasterBand(1).ReadAsArray()
-        lst_zone_mean_large[lst_zone_mean_large==0] = -9999
-        lst_zone_mean_large[np.isnan(lst_zone_mean_large)] = -9999
-
-        if np.nanmax(lst_zone_mean_large) == -9999:
-            for x in range(0, size_x_zone):
-                for y in range(0, size_y_zone):
-                    lst_zone_mean_large[y, x] = np.nanmean(lst[y*200:np.minimum((y+1)*200, size_y-1), x*200:np.minimum((x+1)*200, size_x-1)])
-            lst_zone_mean_large[np.isnan(lst_zone_mean_large)] = -9999
-
-        lst_zone_mean_large = PF.gap_filling(lst_zone_mean_large, -9999, 1)
-        dest_lst_zone_large = PF.Save_as_MEM(lst_zone_mean_large, geo_new, proj_ex)
-        
-        dest_lst_zone = PF.reproject_dataset_example(dest_lst_zone_large, lst_filename, 6)
-        lst_zone_mean = dest_lst_zone.GetRasterBand(1).ReadAsArray()
-
-        lst_zone_mean_full[i, ...] = lst_zone_mean
-        
-    lst_zone_mean_da = xr.DataArray(lst_zone_mean_full, coords = ds.ndvi.coords)
-
-    return lst_zone_mean_da
-
 def test_ds(ds, var):
     from dask.diagnostics import Profiler, ResourceProfiler, CacheProfiler, ProgressBar
     from dask.diagnostics import visualize
 
     with Profiler() as prof, ResourceProfiler(dt=0.25) as rprof, CacheProfiler() as cprof, ProgressBar():
         out = ds[var].compute()
```

### Comparing `pywapor-3.3.4/pywapor.egg-info/SOURCES.txt` & `pywapor-3.3.5/pywapor.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -58,29 +58,14 @@
 pywapor/enhancers/dms/pyDMS_utils.py
 pywapor/enhancers/dms/thermal_sharpener.py
 pywapor/enhancers/smooth/__init__.py
 pywapor/enhancers/smooth/archive.py
 pywapor/enhancers/smooth/core.py
 pywapor/enhancers/smooth/plotters.py
 pywapor/enhancers/smooth/whittaker.py
-pywapor/et_look_dev/__init__.py
-pywapor/et_look_dev/biomass.py
-pywapor/et_look_dev/clear_sky_radiation.py
-pywapor/et_look_dev/constants.py
-pywapor/et_look_dev/evapotranspiration.py
-pywapor/et_look_dev/leaf.py
-pywapor/et_look_dev/meteo.py
-pywapor/et_look_dev/neutral.py
-pywapor/et_look_dev/radiation.py
-pywapor/et_look_dev/resistance.py
-pywapor/et_look_dev/roughness.py
-pywapor/et_look_dev/soil_moisture.py
-pywapor/et_look_dev/solar_radiation.py
-pywapor/et_look_dev/stress.py
-pywapor/et_look_dev/unstable.py
 pywapor/et_look_v2_v3/__init__.py
 pywapor/et_look_v2_v3/biomass.py
 pywapor/et_look_v2_v3/clear_sky_radiation.py
 pywapor/et_look_v2_v3/constants.py
 pywapor/et_look_v2_v3/evapotranspiration.py
 pywapor/et_look_v2_v3/leaf.py
 pywapor/et_look_v2_v3/meteo.py
```

### Comparing `pywapor-3.3.4/setup.py` & `pywapor-3.3.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pywapor',
-    version = '3.3.4',
+    version = '3.3.5',
     url = 'https://www.fao.org/aquastat/py-wapor/',
     author = "FAO",
     author_email = "bert.coerver@fao.org",
     license = "Apache",
     packages = find_packages(include = ['pywapor', 'pywapor.*']),
     include_package_data=True,
     python_requires='>=3.7',
     install_requires = [
         'gdal',
         'xarray>=0.20',
         'numpy',
         'pydap',
-        'pandas',
+# - NOTE in pandas == 2.0.0, the buffering of timelim (e.g. in collect.product.MODIS.download) doesnt work correctly.
+# So fo now sticking to 1.5.3 and waiting for 2.x.x to become more stable.
+        'pandas<2.0.0',
         'requests',
         'matplotlib',
 # - NOTE otherwise opendap gives problem in colab, in conda env netcdf=1.6.0 
 # works fine -> https://github.com/Unidata/netcdf4-python/issues/1179
 # - (fixed) NOTE also, cant install netcdf4 with conda, because the conda-forge distribution cant open
 # the PROBAV HDF files. See issues https://github.com/Unidata/netcdf4-python/issues/1182 and
 # https://github.com/conda-forge/netcdf4-feedstock/issues/136
```

