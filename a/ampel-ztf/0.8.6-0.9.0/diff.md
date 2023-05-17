# Comparing `tmp/ampel_ztf-0.8.6.tar.gz` & `tmp/ampel_ztf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_ztf-0.8.6.tar", max compression
+gzip compressed data, was "ampel_ztf-0.9.0.tar", max compression
```

## Comparing `ampel_ztf-0.8.6.tar` & `ampel_ztf-0.9.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1512 2023-05-17 13:59:24.493061 ampel_ztf-0.8.6/LICENSE
--rw-r--r--   0        0        0      391 2023-05-17 13:59:24.493061 ampel_ztf-0.8.6/README.md
--rw-r--r--   0        0        0        0 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/py.typed
--rwxr-xr-x   0        0        0     3644 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/template/ZTFLegacyChannelTemplate.py
--rwxr-xr-x   0        0        0      739 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/template/ZTFPeriodicSummaryT3.py
--rwxr-xr-x   0        0        0     2640 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/template/ZTFProcessLocalAlerts.py
--rwxr-xr-x   0        0        0    11970 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/util/Observatory.py
--rw-r--r--   0        0        0     3810 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/HealpixPathSupplier.py
--rwxr-xr-x   0        0        0     9168 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/PhotoAlertPlotter.py
--rw-r--r--   0        0        0    24540 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/ZTFFPbotForcedPhotometryAlertSupplier.py
--rwxr-xr-x   0        0        0     3649 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/ZTFForcedPhotometryAlertSupplier.py
--rwxr-xr-x   0        0        0     3582 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/ZTFGeneralActiveAlertRegister.py
--rwxr-xr-x   0        0        0     2132 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/ZTFGeneralAlertRegister.py
--rw-r--r--   0        0        0     5534 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/ZTFIPACForcedPhotometryAlertSupplier.py
--rwxr-xr-x   0        0        0     2375 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/ZiAlertSupplier.py
--rw-r--r--   0        0        0     2007 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/ZiHealpixAlertSupplier.py
--rwxr-xr-x   0        0        0     2119 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/ZiTaggedAlertSupplier.py
--rw-r--r--   0        0        0     5405 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/alert/load/ZTFHealpixAlertLoader.py
--rw-r--r--   0        0        0     1286 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/base/ArchiveUnit.py
--rwxr-xr-x   0        0        0     3612 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/base/CatalogMatchFilter.py
--rwxr-xr-x   0        0        0     5609 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/base/CatalogMatchUnit.py
--rwxr-xr-x   0        0        0     4803 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/dev/DevAlertConsumer.py
--rwxr-xr-x   0        0        0     6975 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/dev/DevSkyPortalClient.py
--rwxr-xr-x   0        0        0     3550 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/dev/ZTFAlert.py
--rw-r--r--   0        0        0     6187 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/ingest/ZiArchiveMuxer.py
--rw-r--r--   0        0        0      760 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/ingest/ZiCompilerOptions.py
--rwxr-xr-x   0        0        0     3580 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/ingest/ZiDataPointShaper.py
--rwxr-xr-x   0        0        0    10260 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/ingest/ZiMongoMuxer.py
--rwxr-xr-x   0        0        0     1062 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/ingest/tags.py
--rwxr-xr-x   0        0        0     2298 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/legacy_utils.py
--rwxr-xr-x   0        0        0    14357 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/DecentFilter.py
--rw-r--r--   0        0        0    17003 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/T0HealpixPathProcessor.py
--rw-r--r--   0        0        0    13501 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/T0HealpixProcessor.py
--rwxr-xr-x   0        0        0     7702 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/ZTFAlertStreamController.py
--rwxr-xr-x   0        0        0     7598 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/load/AllConsumingConsumer.py
--rwxr-xr-x   0        0        0     2947 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/load/UWAlertLoader.py
--rw-r--r--   0        0        0     2369 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/load/ZTFAlertArchiver.py
--rw-r--r--   0        0        0     3265 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/load/ZTFAlertArchiverV3.py
--rw-r--r--   0        0        0     4764 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py
--rw-r--r--   0        0        0     1346 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/load/avroutils.py
--rwxr-xr-x   0        0        0     2976 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t0/load/fetcherutils.py
--rwxr-xr-x   0        0        0     1198 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t1/ZiT1Combiner.py
--rwxr-xr-x   0        0        0     1048 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t1/ZiT1RetroCombiner.py
--rwxr-xr-x   0        0        0     5674 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t2/T2CatalogMatch.py
--rw-r--r--   0        0        0     2240 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t2/T2LightCurveFeatures.py
--rwxr-xr-x   0        0        0     2757 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t2/T2LightCurveSummary.py
--rwxr-xr-x   0        0        0     1339 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t3/T3LegacyExtJournalAppender.py
--rwxr-xr-x   0        0        0     2891 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t3/complement/FritzReport.py
--rwxr-xr-x   0        0        0     2481 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t3/complement/GROWTHMarshalReport.py
--rwxr-xr-x   0        0        0     3890 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t3/complement/TNSNames.py
--rwxr-xr-x   0        0        0      517 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t3/complement/TNSReports.py
--rwxr-xr-x   0        0        0     3031 2023-05-17 13:59:24.513061 ampel_ztf-0.8.6/ampel/ztf/t3/complement/ZTFCutoutImages.py
--rw-r--r--   0        0        0     3171 2023-05-17 13:59:24.517061 ampel_ztf-0.8.6/ampel/ztf/t3/resource/T3ZTFArchiveTokenGenerator.py
--rwxr-xr-x   0        0        0     1248 2023-05-17 13:59:24.517061 ampel_ztf-0.8.6/ampel/ztf/t3/select/T3AdHocStockSelector.py
--rwxr-xr-x   0        0        0    30107 2023-05-17 13:59:24.517061 ampel_ztf-0.8.6/ampel/ztf/t3/skyportal/SkyPortalClient.py
--rwxr-xr-x   0        0        0     3876 2023-05-17 13:59:24.517061 ampel_ztf-0.8.6/ampel/ztf/t3/skyportal/SkyPortalPublisher.py
--rwxr-xr-x   0        0        0     4337 2023-05-17 13:59:24.517061 ampel_ztf-0.8.6/ampel/ztf/util/ZTFIdMapper.py
--rw-r--r--   0        0        0     2781 2023-05-17 13:59:24.517061 ampel_ztf-0.8.6/ampel/ztf/util/ZTFNoisifiedIdMapper.py
--rw-r--r--   0        0        0     3832 2023-05-17 13:59:24.517061 ampel_ztf-0.8.6/ampel/ztf/view/ZTFT2Tabulator.py
--rw-r--r--   0        0        0     2302 2023-05-17 13:59:24.517061 ampel_ztf-0.8.6/conf/ampel-ztf/ampel.yml
--rw-r--r--   0        0        0     2689 2023-05-17 13:59:24.517061 ampel_ztf-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 ampel_ztf-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-04-07 13:56:59.167697 ampel_ztf-0.9.0/LICENSE
+-rw-r--r--   0        0        0      391 2023-04-07 13:56:59.167697 ampel_ztf-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/py.typed
+-rwxr-xr-x   0        0        0     3644 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/template/ZTFLegacyChannelTemplate.py
+-rwxr-xr-x   0        0        0      739 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/template/ZTFPeriodicSummaryT3.py
+-rwxr-xr-x   0        0        0     2819 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/template/ZTFProcessLocalAlerts.py
+-rwxr-xr-x   0        0        0    11970 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/util/Observatory.py
+-rw-r--r--   0        0        0     3810 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/HealpixPathSupplier.py
+-rwxr-xr-x   0        0        0     9168 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/PhotoAlertPlotter.py
+-rw-r--r--   0        0        0    24540 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFFPbotForcedPhotometryAlertSupplier.py
+-rwxr-xr-x   0        0        0     3649 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFForcedPhotometryAlertSupplier.py
+-rwxr-xr-x   0        0        0     3582 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFGeneralActiveAlertRegister.py
+-rwxr-xr-x   0        0        0     2132 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFGeneralAlertRegister.py
+-rw-r--r--   0        0        0     5534 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFIPACForcedPhotometryAlertSupplier.py
+-rwxr-xr-x   0        0        0     2375 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZiAlertSupplier.py
+-rw-r--r--   0        0        0     2007 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZiHealpixAlertSupplier.py
+-rwxr-xr-x   0        0        0     2119 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZiTaggedAlertSupplier.py
+-rw-r--r--   0        0        0     5405 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/load/ZTFHealpixAlertLoader.py
+-rw-r--r--   0        0        0     1286 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/base/ArchiveUnit.py
+-rwxr-xr-x   0        0        0     3612 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/base/CatalogMatchFilter.py
+-rwxr-xr-x   0        0        0     5609 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/base/CatalogMatchUnit.py
+-rwxr-xr-x   0        0        0     4803 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/dev/DevAlertConsumer.py
+-rwxr-xr-x   0        0        0     6975 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/dev/DevSkyPortalClient.py
+-rwxr-xr-x   0        0        0     3550 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/dev/ZTFAlert.py
+-rw-r--r--   0        0        0     6187 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/ZiArchiveMuxer.py
+-rw-r--r--   0        0        0      760 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/ZiCompilerOptions.py
+-rwxr-xr-x   0        0        0     3580 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/ZiDataPointShaper.py
+-rwxr-xr-x   0        0        0    10260 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/ZiMongoMuxer.py
+-rwxr-xr-x   0        0        0     1062 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/tags.py
+-rwxr-xr-x   0        0        0     2298 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/legacy_utils.py
+-rwxr-xr-x   0        0        0    14327 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/DecentFilter.py
+-rw-r--r--   0        0        0    17003 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/T0HealpixPathProcessor.py
+-rw-r--r--   0        0        0    13501 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/T0HealpixProcessor.py
+-rwxr-xr-x   0        0        0     7702 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/ZTFAlertStreamController.py
+-rwxr-xr-x   0        0        0     7598 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/AllConsumingConsumer.py
+-rwxr-xr-x   0        0        0     2947 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/UWAlertLoader.py
+-rw-r--r--   0        0        0     2369 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFAlertArchiver.py
+-rw-r--r--   0        0        0     3265 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFAlertArchiverV3.py
+-rw-r--r--   0        0        0     3994 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py
+-rw-r--r--   0        0        0     1346 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/avroutils.py
+-rwxr-xr-x   0        0        0     2976 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/fetcherutils.py
+-rwxr-xr-x   0        0        0     1198 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t1/ZiT1Combiner.py
+-rwxr-xr-x   0        0        0     1048 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t1/ZiT1RetroCombiner.py
+-rwxr-xr-x   0        0        0     5674 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t2/T2CatalogMatch.py
+-rw-r--r--   0        0        0     2240 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t2/T2LightCurveFeatures.py
+-rwxr-xr-x   0        0        0     2757 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t2/T2LightCurveSummary.py
+-rwxr-xr-x   0        0        0     1339 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/T3LegacyExtJournalAppender.py
+-rwxr-xr-x   0        0        0     2891 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/FritzReport.py
+-rwxr-xr-x   0        0        0     2481 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/GROWTHMarshalReport.py
+-rwxr-xr-x   0        0        0     3890 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/TNSNames.py
+-rwxr-xr-x   0        0        0      517 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/TNSReports.py
+-rwxr-xr-x   0        0        0     3031 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/ZTFCutoutImages.py
+-rwxr-xr-x   0        0        0     1248 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/select/T3AdHocStockSelector.py
+-rwxr-xr-x   0        0        0    30107 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/skyportal/SkyPortalClient.py
+-rwxr-xr-x   0        0        0     3876 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/skyportal/SkyPortalPublisher.py
+-rw-r--r--   0        0        0     2986 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t4/T4ZTFArchiveTokenGenerator.py
+-rwxr-xr-x   0        0        0     4337 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/util/ZTFIdMapper.py
+-rw-r--r--   0        0        0     2781 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/util/ZTFNoisifiedIdMapper.py
+-rw-r--r--   0        0        0     3832 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/view/ZTFT2Tabulator.py
+-rw-r--r--   0        0        0     2293 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/conf/ampel-ztf/ampel.yml
+-rw-r--r--   0        0        0     2689 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 ampel_ztf-0.9.0/PKG-INFO
```

### Comparing `ampel_ztf-0.8.6/LICENSE` & `ampel_ztf-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/template/ZTFLegacyChannelTemplate.py` & `ampel_ztf-0.9.0/ampel/template/ZTFLegacyChannelTemplate.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/template/ZTFPeriodicSummaryT3.py` & `ampel_ztf-0.9.0/ampel/template/ZTFPeriodicSummaryT3.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/template/ZTFProcessLocalAlerts.py` & `ampel_ztf-0.9.0/ampel/template/ZTFProcessLocalAlerts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # File:                Ampel-ZTF/ampel/template/ZTFProcessLocalAlerts.py
 # License:             BSD-3-Clause
 # Author:              valery brinnel <firstname.lastname@gmail.com>
 # Date:                16.07.2021
-# Last Modified Date:  24.11.2021
+# Last Modified Date:  07.04.2023
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
 from typing import Any, Literal
 from ampel.types import ChannelId
 from ampel.log.AmpelLogger import AmpelLogger
 from ampel.model.UnitModel import UnitModel
+from ampel.model.job.JobTaskModel import JobTaskModel
 from ampel.model.ingest.T2Compute import T2Compute
-from ampel.abstract.AbsProcessorTemplate import AbsProcessorTemplate
+from ampel.abstract.AbsConfigMorpher import AbsConfigMorpher
 from ampel.template.AbsEasyChannelTemplate import AbsEasyChannelTemplate
 
 
-class ZTFProcessLocalAlerts(AbsProcessorTemplate):
+# Inheritance orders matters in this case
+class ZTFProcessLocalAlerts(JobTaskModel, AbsConfigMorpher): # type: ignore[misc]
 	"""
 	Returns adequate config for an alert consumer configured to process local alerts
 	"""
 
 	channel: ChannelId
 	folder: str
 	extension: Literal['json', 'avro', 'csv'] = "json"
@@ -35,21 +37,21 @@
 	#: units will be added automatically.
 	t2_compute: list[T2Compute] = []
 
 	extra: dict = {}
 
 
 	# Mandatory override
-	def get_model(self, config: dict[str, Any], logger: AmpelLogger) -> UnitModel:
+	def morph(self, ampel_config: dict[str, Any], logger: AmpelLogger) -> dict[str, Any]:
 
-		return UnitModel(
+		return self.dict(include=JobTaskModel.__fields__.keys()) | dict(
 			unit = 'AlertConsumer',
 			config = self.extra | AbsEasyChannelTemplate.craft_t0_processor_config(
 				channel = self.channel,
-				config = config,
+				alconf = ampel_config,
 				t2_compute = self.t2_compute,
 				supplier = self._get_supplier(),
 				shaper = "ZiDataPointShaper",
 				combiner = "ZiT1Combiner",
 				filter_dict = None,
 				muxer = None,
 				compiler_opts = {
```

### Comparing `ampel_ztf-0.8.6/ampel/util/Observatory.py` & `ampel_ztf-0.9.0/ampel/util/Observatory.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/HealpixPathSupplier.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/HealpixPathSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/PhotoAlertPlotter.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/PhotoAlertPlotter.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/ZTFFPbotForcedPhotometryAlertSupplier.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFFPbotForcedPhotometryAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/ZTFForcedPhotometryAlertSupplier.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFForcedPhotometryAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/ZTFGeneralActiveAlertRegister.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFGeneralActiveAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/ZTFGeneralAlertRegister.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFGeneralAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/ZTFIPACForcedPhotometryAlertSupplier.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFIPACForcedPhotometryAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/ZiAlertSupplier.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/ZiAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/ZiHealpixAlertSupplier.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/ZiHealpixAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/ZiTaggedAlertSupplier.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/ZiTaggedAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/alert/load/ZTFHealpixAlertLoader.py` & `ampel_ztf-0.9.0/ampel/ztf/alert/load/ZTFHealpixAlertLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/base/ArchiveUnit.py` & `ampel_ztf-0.9.0/ampel/ztf/base/ArchiveUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/base/CatalogMatchFilter.py` & `ampel_ztf-0.9.0/ampel/ztf/base/CatalogMatchFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/base/CatalogMatchUnit.py` & `ampel_ztf-0.9.0/ampel/ztf/base/CatalogMatchUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/dev/DevAlertConsumer.py` & `ampel_ztf-0.9.0/ampel/ztf/dev/DevAlertConsumer.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/dev/DevSkyPortalClient.py` & `ampel_ztf-0.9.0/ampel/ztf/dev/DevSkyPortalClient.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/dev/ZTFAlert.py` & `ampel_ztf-0.9.0/ampel/ztf/dev/ZTFAlert.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/ingest/ZiArchiveMuxer.py` & `ampel_ztf-0.9.0/ampel/ztf/ingest/ZiArchiveMuxer.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/ingest/ZiCompilerOptions.py` & `ampel_ztf-0.9.0/ampel/ztf/ingest/ZiCompilerOptions.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/ingest/ZiDataPointShaper.py` & `ampel_ztf-0.9.0/ampel/ztf/ingest/ZiDataPointShaper.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/ingest/ZiMongoMuxer.py` & `ampel_ztf-0.9.0/ampel/ztf/ingest/ZiMongoMuxer.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/ingest/tags.py` & `ampel_ztf-0.9.0/ampel/ztf/ingest/tags.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/legacy_utils.py` & `ampel_ztf-0.9.0/ampel/ztf/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/DecentFilter.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/DecentFilter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # File:                Ampel-ZTF/ampel/ztf/t0/DecentFilter.py
 # License:             BSD-3-Clause
 # Author:              m. giomi <matteo.giomi@desy.de>
 # Date:                06.06.2018
-# Last Modified Date:  17.05.2023
-# Last Modified By:    Simeon Reusch <simeon.reusch@desy.de>
+# Last Modified Date:  10.03.2021
+# Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
+import numpy as np
 from typing import Any
+from astropy.table import Table
+from astropy.coordinates import SkyCoord
 
-import numpy as np
 from ampel.abstract.AbsAlertFilter import AbsAlertFilter
-from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
 from ampel.ztf.base.CatalogMatchUnit import CatalogMatchUnit
-from astropy.coordinates import SkyCoord
-from astropy.table import Table
+from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
 
 
 class DecentFilter(CatalogMatchUnit, AbsAlertFilter):
     """
     General-purpose filter with ~ 0.6% acceptance. It selects alerts based on:
     * numper of previous detections
     * positive subtraction flag
@@ -32,18 +32,16 @@
     on the provided PS1 star-galaxy classification.
     """
 
     # History
     min_ndet: int  # number of previous detections
     min_tspan: float  # minimum duration of alert detection history [days]
     max_tspan: float  # maximum duration of alert detection history [days]
-    min_archive_tspan: float = 0.0  # minimum duration of alert detection history [days]
-    max_archive_tspan: float = (
-        10**5.0
-    )  # maximum duration of alert detection history [days]
+    min_archive_tspan: float = 0. # minimum duration of alert detection history [days]
+    max_archive_tspan: float = 10**5. # maximum duration of alert detection history [days]
 
     # Image quality
     min_drb: float = 0.0  # deep learning real bogus score
     min_rb: float  # real bogus score
     max_fwhm: float  # sexctrator FWHM (assume Gaussian) [pix]
     max_elong: float  # Axis ratio of image: aimage / bimage
     max_magdiff: float  # Difference: magap - magpsf [mag]
@@ -64,17 +62,18 @@
     gaia_pm_signif: float  # significance of proper motion detection of GAIA counterpart [sigma]
     gaia_plx_signif: float  # significance of parallax detection of GAIA counterpart [sigma]
     gaia_veto_gmag_min: float  # min gmag for normalized distance cut of GAIA counterparts [mag]
     gaia_veto_gmag_max: float  # max gmag for normalized distance cut of GAIA counterparts [mag]
     gaia_excessnoise_sig_max: float  # maximum allowed noise (expressed as significance) for Gaia match to be trusted.
 
     def post_init(self):
+
         # feedback
         for k in self.__annotations__:
-            self.logger.debug(f"Using {k}={getattr(self, k)}")
+            self.logger.info(f"Using {k}={getattr(self, k)}")
 
         # To make this tenable we should create this list dynamically depending on what entries are required
         # by the filter. Now deciding not to include drb in this list, eg.
         self.keys_to_check = (
             "fwhm",
             "elong",
             "magdiff",
@@ -94,18 +93,18 @@
 
     def _alert_has_keys(self, photop) -> bool:
         """
         check that given photopoint contains all the keys needed to filter
         """
         for el in self.keys_to_check:
             if el not in photop:
-                self.logger.debug(None, extra={"missing": el})
+                self.logger.info(None, extra={"missing": el})
                 return False
             if photop[el] is None:
-                self.logger.debug(None, extra={"isNone": el})
+                self.logger.info(None, extra={"isNone": el})
                 return False
         return True
 
     def get_galactic_latitude(self, transient):
         """
         compute galactic latitude of the transient
         """
@@ -181,14 +180,15 @@
                         "ExcessNoiseSig",
                     ],
                 }
             ],
         )[0]
 
         if srcs:
+
             gaia_tab = Table(
                 [
                     {k: np.nan if v is None else v for k, v in src["body"].items()}
                     for src in srcs
                 ]
             )
 
@@ -223,15 +223,15 @@
             # select just the sources that are close enough and that are not noisy
             gaia_tab = gaia_tab[gaia_tab["FLAG_PROX"]]
             gaia_tab = gaia_tab[gaia_tab["FLAG_Clean"]]
 
             # among the remaining sources there is anything with
             # significant proper motion or parallax measurement
             if (
-                any(gaia_tab["FLAG_PMRA"] == True)  # noqa
+                any(gaia_tab["FLAG_PMRA"] == True) # noqa
                 or any(gaia_tab["FLAG_PMDec"] == True)
                 or any(gaia_tab["FLAG_Plx"] == True)
             ):
                 return True
 
         return False
 
@@ -247,103 +247,104 @@
 
         # CUT ON THE HISTORY OF THE ALERT
         #################################
 
         pps = [el for el in alert.datapoints if el.get("candid") is not None]
         if len(pps) < self.min_ndet:
             # self.logger.debug("rejected: %d photopoints in alert (minimum required %d)"% (npp, self.min_ndet))
-            self.logger.debug(None, extra={"nDet": len(pps)})
+            self.logger.info(None, extra={"nDet": len(pps)})
             return None
 
         # cut on length of detection history
-        detections_jds = [el["jd"] for el in pps]
+        detections_jds = [el['jd'] for el in pps]
         det_tspan = max(detections_jds) - min(detections_jds)
         if not (self.min_tspan <= det_tspan <= self.max_tspan):
             # self.logger.debug("rejected: detection history is %.3f d long, \
             # requested between %.3f and %.3f d"% (det_tspan, self.min_tspan, self.max_tspan))
-            self.logger.debug(None, extra={"tSpan": det_tspan})
+            self.logger.info(None, extra={"tSpan": det_tspan})
             return None
 
         # IMAGE QUALITY CUTS
         ####################
 
         latest = alert.datapoints[0]
         if not self._alert_has_keys(latest):
             return None
 
         if latest["isdiffpos"] == "f" or latest["isdiffpos"] == "0":
             # self.logger.debug("rejected: 'isdiffpos' is %s", latest['isdiffpos'])
-            self.logger.debug(None, extra={"isdiffpos": latest["isdiffpos"]})
+            self.logger.info(None, extra={"isdiffpos": latest["isdiffpos"]})
             return None
 
         if latest["rb"] < self.min_rb:
             # self.logger.debug("rejected: RB score %.2f below threshod (%.2f)"% (latest['rb'], self.min_rb))
-            self.logger.debug(None, extra={"rb": latest["rb"]})
+            self.logger.info(None, extra={"rb": latest["rb"]})
             return None
 
         if self.min_drb > 0.0 and latest["drb"] < self.min_drb:
             # self.logger.debug("rejected: RB score %.2f below threshod (%.2f)"% (latest['rb'], self.min_rb))
-            self.logger.debug(None, extra={"drb": latest["drb"]})
+            self.logger.info(None, extra={"drb": latest["drb"]})
             return None
 
         if latest["fwhm"] > self.max_fwhm:
             # self.logger.debug("rejected: fwhm %.2f above threshod (%.2f)"% (latest['fwhm'], self.max_fwhm))
-            self.logger.debug(None, extra={"fwhm": latest["fwhm"]})
+            self.logger.info(None, extra={"fwhm": latest["fwhm"]})
             return None
 
         if latest["elong"] > self.max_elong:
             # self.logger.debug("rejected: elongation %.2f above threshod (%.2f)"% (latest['elong'], self.max_elong))
-            self.logger.debug(None, extra={"elong": latest["elong"]})
+            self.logger.info(None, extra={"elong": latest["elong"]})
             return None
 
         if abs(latest["magdiff"]) > self.max_magdiff:
             # self.logger.debug("rejected: magdiff (AP-PSF) %.2f above threshod (%.2f)"% (latest['magdiff'], self.max_magdiff))
-            self.logger.debug(None, extra={"magdiff": latest["magdiff"]})
+            self.logger.info(None, extra={"magdiff": latest["magdiff"]})
             return None
 
         # cut on archive length
-        if "jdendhist" in latest.keys() and "jdstarthist" in latest.keys():
-            archive_tspan = latest["jdendhist"] - latest["jdstarthist"]
+        if 'jdendhist' in latest.keys() and 'jdstarthist' in latest.keys():
+            archive_tspan = latest['jdendhist'] - latest['jdstarthist']
             if not (self.min_archive_tspan < archive_tspan < self.max_archive_tspan):
-                self.logger.debug(None, extra={"archive_tspan": archive_tspan})
+                self.logger.info(None, extra={'archive_tspan': archive_tspan})
                 return None
 
+
         # ASTRONOMY
         ###########
 
         # check for closeby ss objects
         if 0 <= latest["ssdistnr"] < self.min_sso_dist:
             # self.logger.debug("rejected: solar-system object close to transient (max allowed: %d)."% (self.min_sso_dist))
-            self.logger.debug(None, extra={"ssdistnr": latest["ssdistnr"]})
+            self.logger.info(None, extra={"ssdistnr": latest["ssdistnr"]})
             return None
 
         # cut on galactic latitude
         b = self.get_galactic_latitude(latest)
         if abs(b) < self.min_gal_lat:
             # self.logger.debug("rejected: b=%.4f, too close to Galactic plane (max allowed: %f)."% (b, self.min_gal_lat))
-            self.logger.debug(None, extra={"galPlane": abs(b)})
+            self.logger.info(None, extra={"galPlane": abs(b)})
             return None
 
         # check ps1 star-galaxy score
         if self.is_star_in_PS1(latest):
             # self.logger.debug("rejected: closest PS1 source %.2f arcsec away with sgscore of %.2f"% (latest['distpsnr1'], latest['sgscore1']))
-            self.logger.debug(None, extra={"distpsnr1": latest["distpsnr1"]})
+            self.logger.info(None, extra={"distpsnr1": latest["distpsnr1"]})
             return None
 
         if self.is_confused_in_PS1(latest):
             # self.logger.debug("rejected: three confused PS1 sources within %.2f arcsec from alert."% (self.ps1_confusion_rad))
-            self.logger.debug(None, extra={"ps1Confusion": True})
+            self.logger.info(None, extra={"ps1Confusion": True})
             return None
 
         # check with gaia
         if self.gaia_rs > 0 and self.is_star_in_gaia(latest):
             # self.logger.debug("rejected: within %.2f arcsec from a GAIA start (PM of PLX)" % (self.gaia_rs))
-            self.logger.debug(None, extra={"gaiaIsStar": True})
+            self.logger.info(None, extra={"gaiaIsStar": True})
             return None
 
         # self.logger.debug("Alert %s accepted. Latest pp ID: %d"%(alert.tran_id, latest['candid']))
         self.logger.debug("Alert accepted", extra={"latestPpId": latest["candid"]})
 
         # for key in self.keys_to_check:
-        #   self.logger.debug("{}: {}".format(key, latest[key]))
+        # 	self.logger.debug("{}: {}".format(key, latest[key]))
 
         return True
```

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/T0HealpixPathProcessor.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/T0HealpixPathProcessor.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/T0HealpixProcessor.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/T0HealpixProcessor.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/ZTFAlertStreamController.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/ZTFAlertStreamController.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/load/AllConsumingConsumer.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/load/AllConsumingConsumer.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/load/UWAlertLoader.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/load/UWAlertLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/load/ZTFAlertArchiver.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFAlertArchiver.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/load/ZTFAlertArchiverV3.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFAlertArchiverV3.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # File:                Ampel-ZTF/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py
 # License:             BSD-3-Clause
 # Author:              jvs
 # Date:                20.10.2021
-# Last Modified Date:  17.05.2023
-# Last Modified By:    Simeon Reusch <simeon.reusch@desy.de>
+# Last Modified Date:  22.12.2022
+# Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
-import logging
+import logging, backoff, requests
 from typing import Any
-
-import backoff
-import requests
 from ampel.abstract.AbsAlertLoader import AbsAlertLoader
 from ampel.base.AmpelBaseModel import AmpelBaseModel
-from ampel.struct.Resource import Resource
 
 log = logging.getLogger(__name__)
 
 
 class ZTFSource(AmpelBaseModel):
     ztf_name: str
     programid: None | int = None
@@ -38,36 +34,20 @@
     this is acknowledged and a new chunk retrieved.
     """
 
     #: Base URL of archive service
     archive: str = "https://ampel.zeuthen.desy.de/api/ztf/archive/v3"
 
     #: A stream identifier, created via POST /api/ztf/archive/streams/, or a query
-    stream: None | str | ZTFSource
-
-    #: Name of dynamic resource, fetched by a T3 process and forwarded
-    #: to suppliers/loaders by AlertConsumer via their methods add_resource
-    resource_name: str = "ztf_stream_token"
-
-    with_history: bool = True
+    stream: None | str | ZTFSource = '%%ztf_stream_token'
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
         self._it = None
 
-    # override
-    def add_resource(self, name: str, resource: Resource) -> None:
-        if name == self.resource_name:
-            if not isinstance(resource.value, str):
-                raise ValueError(
-                    f"Unexpected {self.resource_name} resource "
-                    f"value type: {type(resource.value)}"
-                )
-            self.stream = resource.value
-
     def __iter__(self):
         return self.get_alerts()
 
     def __next__(self):
         if not self._it:
             self._it = iter(self)
         return next(self._it)
@@ -79,58 +59,52 @@
             while True:
                 chunk = self._get_chunk(session)
                 yield from chunk["alerts"] if isinstance(chunk, dict) else chunk
                 # NB: if generator exits before we get here, chunk is never acknowledged
                 if "chunk" in chunk:
                     self._acknowledge_chunk(session, chunk["chunk"])
                     log.info(
-                        None,
-                        extra={"streamToken": self.stream, "chunk": chunk["chunk"]},
+                        None, extra={"streamToken": self.stream, "chunk": chunk["chunk"]}
                     )
                 if isinstance(self.stream, ZTFSource) or (
                     len(chunk["alerts"]) == 0 and chunk["remaining"]["chunks"] == 0
                 ):
                     break
 
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
-        giveup=lambda e: (
-            not isinstance(e, requests.HTTPError)
-            or e.response.status_code not in {502, 503, 504, 429, 408, 423}
+        giveup = lambda e: (
+            not isinstance(e, requests.HTTPError) or
+            e.response.status_code not in {502, 503, 504, 429, 408}
         ),
-        max_time=600,
+        max_time = 600,
     )
     def _get_chunk(self, session: requests.Session) -> dict[str, Any]:
+
         if isinstance(self.stream, ZTFSource):
             params = {"with_history": self.stream.with_history}
             for k in ("jd_start", "jd_end", "programid"):
                 if (x := getattr(self.stream, k)) is not None:
                     params[k] = x
             response = session.get(
                 f"{self.archive}/object/{self.stream.ztf_name}/alerts",
-                headers={"Authorization": f"bearer {self.stream.archive_token}"},
-                params=params,
+                headers = {"Authorization": f"bearer {self.stream.archive_token}"},
+                params = params
             )
         else:
-            response = session.get(
-                f"{self.archive}/stream/{self.stream}/chunk",
-                params={"with_history": self.with_history},
-            )
-
+            response = session.get(f"{self.archive}/stream/{self.stream}/chunk")
         response.raise_for_status()
         return response.json()
 
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
-        giveup=(
-            lambda e: not isinstance(e, requests.HTTPError)
-            or e.response.status_code not in {502, 503, 504, 429, 408}
+        giveup = (
+            lambda e: not isinstance(e, requests.HTTPError) or
+            e.response.status_code not in {502, 503, 504, 429, 408}
         ),
-        max_time=600,
+        max_time = 600,
     )
     def _acknowledge_chunk(self, session: requests.Session, chunk_id: int) -> None:
-        response = session.post(
-            f"{self.archive}/stream/{self.stream}/chunk/{chunk_id}/acknowledge"
-        )
+        response = session.post(f"{self.archive}/stream/{self.stream}/chunk/{chunk_id}/acknowledge")
         response.raise_for_status()
```

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/load/avroutils.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/load/avroutils.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t0/load/fetcherutils.py` & `ampel_ztf-0.9.0/ampel/ztf/t0/load/fetcherutils.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t1/ZiT1Combiner.py` & `ampel_ztf-0.9.0/ampel/ztf/t1/ZiT1Combiner.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t1/ZiT1RetroCombiner.py` & `ampel_ztf-0.9.0/ampel/ztf/t1/ZiT1RetroCombiner.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t2/T2CatalogMatch.py` & `ampel_ztf-0.9.0/ampel/ztf/t2/T2CatalogMatch.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t2/T2LightCurveFeatures.py` & `ampel_ztf-0.9.0/ampel/ztf/t2/T2LightCurveFeatures.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t2/T2LightCurveSummary.py` & `ampel_ztf-0.9.0/ampel/ztf/t2/T2LightCurveSummary.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/T3LegacyExtJournalAppender.py` & `ampel_ztf-0.9.0/ampel/ztf/t3/T3LegacyExtJournalAppender.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/complement/FritzReport.py` & `ampel_ztf-0.9.0/ampel/ztf/t3/complement/FritzReport.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/complement/GROWTHMarshalReport.py` & `ampel_ztf-0.9.0/ampel/ztf/t3/complement/GROWTHMarshalReport.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/complement/TNSNames.py` & `ampel_ztf-0.9.0/ampel/ztf/t3/complement/TNSNames.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/complement/TNSReports.py` & `ampel_ztf-0.9.0/ampel/ztf/t3/complement/TNSReports.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/complement/ZTFCutoutImages.py` & `ampel_ztf-0.9.0/ampel/ztf/t3/complement/ZTFCutoutImages.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/resource/T3ZTFArchiveTokenGenerator.py` & `ampel_ztf-0.9.0/ampel/ztf/t4/T4ZTFArchiveTokenGenerator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File:                Ampel-ZTF/ampel/ztf/t3/resource/T3ZTFArchiveTokenGenerator.py
+# File:                Ampel-ZTF/ampel/ztf/t4/T4ZTFArchiveTokenGenerator.py
 # License:             BSD-3-Clause
 # Author:              valery brinnel & Simeon Reusch
 # Date:                21.12.2022
-# Last Modified Date:  21.12.2022
+# Last Modified Date:  07.04.2023
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
 import random
 import time
 from typing import Any
-from astropy.time import Time  # type: ignore
+from astropy.time import Time  # type: ignore[import]
 from datetime import datetime
-
-from requests_toolbelt.sessions import BaseUrlSession
+from requests_toolbelt.sessions import BaseUrlSession # type: ignore[import]
 
 from ampel.types import UBson
-from ampel.struct.T3Store import T3Store
-from ampel.struct.Resource import Resource
 from ampel.struct.UnitResult import UnitResult
 from ampel.secret.NamedSecret import NamedSecret
-from ampel.abstract.AbsT3PlainUnit import AbsT3PlainUnit
+from ampel.abstract.AbsT4Unit import AbsT4Unit
 
 
-class T3ZTFArchiveTokenGenerator(AbsT3PlainUnit):
+class T4ZTFArchiveTokenGenerator(AbsT4Unit):
 
 	archive_token: NamedSecret[str] = NamedSecret(label="ztf/archive/token")
 
 	#: Base URL of archive service
 	archive: str = "https://ampel.zeuthen.desy.de/api/ztf/archive/v3/"
-	resource_name: str = 'ztf_stream_token'
+	resource_name: str = '%%ztf_stream_token'
 
 	max_dist_ps1_src: float = 0.5
 	min_detections: int = 3
 
 	date_str: None | str = None
 	date_format: str = "%Y-%m-%d"
 	days_ago: None | int = None
@@ -43,15 +40,15 @@
 
 	#: seconds to wait for query to complete
 	timeout: float = 60
 
 	debug: bool = False
 
 
-	def process(self, t3s: T3Store) -> UBson | UnitResult:
+	def do(self) -> UBson | UnitResult:
 
 		if self.date_str:
 			start_jd = Time(
 				str(datetime.strptime(self.date_str, self.date_format)),
 				format="iso", scale="utc"
 			).jd
 			delta_t = 1
@@ -106,14 +103,8 @@
 			time.sleep(random.uniform(0, delay))
 			delay *= 2
 		else:
 			raise RuntimeError(f"{session.base_url}stream/{token} still locked after {time.time() - t0:.0f} s")
 		response.raise_for_status()
 		self.logger.info("Stream created", extra=response.json())
 
-		r = Resource(name=self.resource_name, value=token)
-		t3s.add_resource(r)
-
-		if self.debug:
-			return r.dict()
-
-		return None
+		return {self.resource_name: token}
```

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/select/T3AdHocStockSelector.py` & `ampel_ztf-0.9.0/ampel/ztf/t3/select/T3AdHocStockSelector.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/skyportal/SkyPortalClient.py` & `ampel_ztf-0.9.0/ampel/ztf/t3/skyportal/SkyPortalClient.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/t3/skyportal/SkyPortalPublisher.py` & `ampel_ztf-0.9.0/ampel/ztf/t3/skyportal/SkyPortalPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/util/ZTFIdMapper.py` & `ampel_ztf-0.9.0/ampel/ztf/util/ZTFIdMapper.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/util/ZTFNoisifiedIdMapper.py` & `ampel_ztf-0.9.0/ampel/ztf/util/ZTFNoisifiedIdMapper.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/ampel/ztf/view/ZTFT2Tabulator.py` & `ampel_ztf-0.9.0/ampel/ztf/view/ZTFT2Tabulator.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.8.6/conf/ampel-ztf/ampel.yml` & `ampel_ztf-0.9.0/conf/ampel-ztf/ampel.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 - ampel.ztf.t0.DecentFilter
 - ampel.ztf.ingest.ZiDataPointShaper
 - ampel.ztf.base.CatalogMatchFilter
 - ampel.ztf.t2.T2LightCurveSummary
 - ampel.ztf.t2.T2CatalogMatch
 - ampel.ztf.t2.T2LightCurveFeatures
 - ampel.ztf.t3.skyportal.SkyPortalPublisher
-- ampel.ztf.t3.resource.T3ZTFArchiveTokenGenerator
+- ampel.ztf.t4.T4ZTFArchiveTokenGenerator
 
 # Ops units
 - ampel.ztf.t0.load.ZTFAlertArchiverV3
 
 # Aux units
 - ampel.ztf.alert.HealpixPathSupplier
 - ampel.ztf.alert.ZiAlertSupplier
```

### Comparing `ampel_ztf-0.8.6/pyproject.toml` & `ampel_ztf-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-ztf"
-version = "0.8.6"
+version = "0.9.0"
 description = "Zwicky Transient Facility support for the Ampel system"
 authors = [
     "Valery Brinnel",
     "Jakob van Santen <jakob.van.santen@desy.de>",
     "Sjoert van Velzen",
     "Jakob Nordin",
 ]
@@ -45,18 +45,18 @@
 fastavro = "~1.6.0"
 requests = "^2.25.1"
 requests-toolbelt = "^0.10.0"
 confluent-kafka = {version = "^2.0.0", optional = true}
 healpy = {version = "^1.15", optional = true}
 light-curve = {version = ">=0.7,<0.8", optional = true}
 ampel-ztf-archive = {version = "^0.8.0-alpha.0", optional = true}
-ampel-interface = "^0.8.7"
-ampel-core = "^0.8.6"
-ampel-photometry = "^0.8.3"
-ampel-alerts = "^0.8.4"
+ampel-interface = "^0.9.0"
+ampel-core = "^0.9.0"
+ampel-photometry = "^0.9.0"
+ampel-alerts = "^0.9.0"
 ampel-plot = {version = "^0.8.3-3", optional = true}
 pandas = {version = "^1.5.2", optional = true}
 scipy = "^1.9.3"
 planobs = {version = "^0.6.1", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
```

### Comparing `ampel_ztf-0.8.6/PKG-INFO` & `ampel_ztf-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampel-ztf
-Version: 0.8.6
+Version: 0.9.0
 Summary: Zwicky Transient Facility support for the Ampel system
 Home-page: https://ampelproject.github.io
 License: BSD-3-Clause
 Author: Valery Brinnel
 Maintainer: Jakob van Santen
 Maintainer-email: jakob.van.santen@desy.de
 Requires-Python: >=3.10,<3.12
@@ -21,18 +21,18 @@
 Provides-Extra: bayes
 Provides-Extra: fp
 Provides-Extra: healpix
 Provides-Extra: kafka
 Provides-Extra: light-curve
 Provides-Extra: plot
 Requires-Dist: aiohttp (>=3.7.3,<4.0.0)
-Requires-Dist: ampel-alerts (>=0.8.4,<0.9.0)
-Requires-Dist: ampel-core (>=0.8.6,<0.9.0)
-Requires-Dist: ampel-interface (>=0.8.7,<0.9.0)
-Requires-Dist: ampel-photometry (>=0.8.3,<0.9.0)
+Requires-Dist: ampel-alerts (>=0.9.0,<0.10.0)
+Requires-Dist: ampel-core (>=0.9.0,<0.10.0)
+Requires-Dist: ampel-interface (>=0.9.0,<0.10.0)
+Requires-Dist: ampel-photometry (>=0.9.0,<0.10.0)
 Requires-Dist: ampel-plot (>=0.8.3-3,<0.9.0) ; extra == "plot" or extra == "bayes"
 Requires-Dist: ampel-ztf-archive (>=0.8.0-alpha.0,<0.9.0) ; extra == "archive"
 Requires-Dist: astropy (>=5.0,<6.0)
 Requires-Dist: backoff (>=2.0.0,<3.0.0)
 Requires-Dist: confluent-kafka (>=2.0.0,<3.0.0) ; extra == "kafka"
 Requires-Dist: fastavro (>=1.6.0,<1.7.0)
 Requires-Dist: healpy (>=1.15,<2.0) ; extra == "healpix"
```

