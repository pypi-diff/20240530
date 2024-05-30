# Comparing `tmp/gapipy-2.9.1.tar.gz` & `tmp/gapipy-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gapipy-2.9.1.tar", last modified: Thu Nov 23 04:59:25 2017, max compression
+gzip compressed data, was "dist/gapipy-2.9.3.tar", last modified: Thu Nov 23 17:04:49 2017, max compression
```

## Comparing `gapipy-2.9.1.tar` & `gapipy-2.9.3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/docs/
--rwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     8931 2016-06-06 20:24:51.000000 gapipy-2.9.1/docs/conf.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       27 2016-06-06 20:24:51.000000 gapipy-2.9.1/docs/history.rst
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      472 2016-06-06 20:24:51.000000 gapipy-2.9.1/docs/index.rst
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     6466 2016-06-06 20:24:51.000000 gapipy-2.9.1/docs/make.bat
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     6777 2016-06-06 20:24:51.000000 gapipy-2.9.1/docs/Makefile
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       26 2016-06-06 20:24:51.000000 gapipy-2.9.1/docs/readme.rst
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      108 2016-06-06 20:24:51.000000 gapipy-2.9.1/docs/usage.rst
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      105 2017-11-23 04:56:02.000000 gapipy-2.9.1/gapipy/__init__.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     4509 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/cache.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     5688 2017-02-15 18:40:58.000000 gapipy-2.9.1/gapipy/client.py
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy/models/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      862 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/__init__.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1126 2017-09-25 16:53:26.000000 gapipy-2.9.1/gapipy/models/addon.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      422 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/address.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      467 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/advertised_departure.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      144 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/models/agency_document.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      329 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/arrival_flight_detail.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      231 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/associated_service.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     8869 2017-11-07 22:53:49.000000 gapipy-2.9.1/gapipy/models/base.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      335 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/departure_flight_detail.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      271 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/departure_service_room.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      278 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/document_info.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      225 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/dossier_feature.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      302 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/incomplete_requirement.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      268 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/international_ticket_number.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1319 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/models/price_band.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      945 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/models/price_promotion.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1701 2017-11-07 22:53:49.000000 gapipy-2.9.1/gapipy/models/room.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      251 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/models/traveller_height.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     6200 2017-11-22 21:14:54.000000 gapipy-2.9.1/gapipy/query.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     6368 2017-11-22 21:14:54.000000 gapipy-2.9.1/gapipy/request.py
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy/resources/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2354 2017-09-07 16:31:20.000000 gapipy-2.9.1/gapipy/resources/__init__.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     3315 2017-11-22 21:14:54.000000 gapipy-2.9.1/gapipy/resources/base.py
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy/resources/booking/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      604 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/booking/__init__.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1156 2017-10-25 19:01:57.000000 gapipy-2.9.1/gapipy/resources/booking/agency.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      385 2017-10-25 19:01:57.000000 gapipy-2.9.1/gapipy/resources/booking/agency_chain.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      363 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/resources/booking/agent.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1162 2017-10-02 21:13:55.000000 gapipy-2.9.1/gapipy/resources/booking/booking.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      902 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/booking/customer.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      184 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/resources/booking/declined_reason.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      632 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/booking/document.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      359 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/booking/nationality.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      701 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/booking/override.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      397 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/booking/override_reason.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     8562 2017-10-23 14:55:35.000000 gapipy-2.9.1/gapipy/resources/booking/service.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      557 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/booking/transaction.py
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy/resources/checkin/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       29 2016-09-20 20:56:28.000000 gapipy-2.9.1/gapipy/resources/checkin/__init__.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      712 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/checkin/checkin.py
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy/resources/dossier/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      453 2016-08-25 15:44:24.000000 gapipy-2.9.1/gapipy/resources/dossier/__init__.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      904 2017-09-20 16:50:08.000000 gapipy-2.9.1/gapipy/resources/dossier/accommodation_dossier.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2622 2017-09-20 16:50:08.000000 gapipy-2.9.1/gapipy/resources/dossier/activity_dossier.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      619 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/dossier/country_dossier.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1405 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/dossier/details.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      387 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/resources/dossier/dossier_features.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      445 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/dossier/dossier_segment.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      596 2017-09-20 16:50:08.000000 gapipy-2.9.1/gapipy/resources/dossier/place_dossier.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      291 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/dossier/service_level.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      860 2017-09-20 16:50:08.000000 gapipy-2.9.1/gapipy/resources/dossier/transport_dossier.py
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy/resources/geo/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      262 2016-06-06 20:24:51.000000 gapipy-2.9.1/gapipy/resources/geo/__init__.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      414 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/geo/airport.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      358 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/geo/continent.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      301 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/geo/country.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      419 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/geo/feature.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      305 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/geo/feature_category.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1514 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/geo/place.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      437 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/geo/state.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      302 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/geo/timezone.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      376 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/language.py
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy/resources/tour/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      535 2016-10-25 13:58:35.000000 gapipy-2.9.1/gapipy/resources/tour/__init__.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      919 2017-09-25 16:24:43.000000 gapipy-2.9.1/gapipy/resources/tour/accommodation.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      710 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/tour/activity.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1220 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/tour/departure.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1001 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/tour/departure_component.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      702 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/tour/image.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     5046 2017-09-20 16:50:08.000000 gapipy-2.9.1/gapipy/resources/tour/itinerary.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2440 2017-11-14 19:57:59.000000 gapipy-2.9.1/gapipy/resources/tour/promotion.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      552 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/tour/single_supplement.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1354 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/tour/tour.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      472 2017-09-20 16:50:08.000000 gapipy-2.9.1/gapipy/resources/tour/tour_category.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2600 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/tour/tour_dossier.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      553 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/resources/tour/transport.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      332 2017-09-20 16:50:08.000000 gapipy-2.9.1/gapipy/resources/tour/video.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     4738 2017-09-07 14:58:15.000000 gapipy-2.9.1/gapipy/utils.py
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy.egg-info/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        1 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy.egg-info/dependency_links.txt
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        1 2017-01-11 18:51:23.000000 gapipy-2.9.1/gapipy.egg-info/not-zip-safe
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    33409 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy.egg-info/PKG-INFO
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       16 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy.egg-info/requires.txt
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     3106 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy.egg-info/SOURCES.txt
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       13 2017-11-23 04:59:25.000000 gapipy-2.9.1/gapipy.egg-info/top_level.txt
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    17283 2017-11-23 04:55:58.000000 gapipy-2.9.1/HISTORY.rst
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1079 2016-06-06 20:24:51.000000 gapipy-2.9.1/LICENSE
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      199 2016-06-06 20:24:51.000000 gapipy-2.9.1/MANIFEST.in
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    33409 2017-11-23 04:59:25.000000 gapipy-2.9.1/PKG-INFO
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     8318 2017-11-22 21:14:54.000000 gapipy-2.9.1/README.rst
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       85 2017-11-23 04:59:25.000000 gapipy-2.9.1/setup.cfg
--rwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1287 2017-11-23 04:49:36.000000 gapipy-2.9.1/setup.py
-drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 04:59:25.000000 gapipy-2.9.1/tests/
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2016-06-06 20:24:51.000000 gapipy-2.9.1/tests/__init__.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    19222 2016-06-06 20:24:51.000000 gapipy-2.9.1/tests/fixtures.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1828 2017-09-07 14:58:15.000000 gapipy-2.9.1/tests/test_cache.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2422 2017-09-07 14:58:15.000000 gapipy-2.9.1/tests/test_client.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     4225 2017-09-07 14:58:15.000000 gapipy-2.9.1/tests/test_live_api.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    15076 2017-10-23 14:55:35.000000 gapipy-2.9.1/tests/test_query.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2509 2017-09-07 14:58:15.000000 gapipy-2.9.1/tests/test_request.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     7717 2017-09-25 16:28:59.000000 gapipy-2.9.1/tests/test_resources.py
--rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2557 2017-09-07 14:58:15.000000 gapipy-2.9.1/tests/test_utils.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/docs/
+-rwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     8931 2017-11-23 16:44:32.000000 gapipy-2.9.3/docs/conf.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       27 2017-11-23 16:44:32.000000 gapipy-2.9.3/docs/history.rst
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      472 2017-11-23 16:44:32.000000 gapipy-2.9.3/docs/index.rst
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     6466 2017-11-23 16:44:32.000000 gapipy-2.9.3/docs/make.bat
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     6777 2017-11-23 16:44:32.000000 gapipy-2.9.3/docs/Makefile
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       26 2017-11-23 16:44:32.000000 gapipy-2.9.3/docs/readme.rst
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      108 2017-11-23 16:44:32.000000 gapipy-2.9.3/docs/usage.rst
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      105 2017-11-23 16:44:50.000000 gapipy-2.9.3/gapipy/__init__.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     4509 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/cache.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     5688 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/client.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy/models/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      862 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/__init__.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1126 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/addon.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      422 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/address.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      467 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/advertised_departure.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      144 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/agency_document.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      329 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/arrival_flight_detail.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      231 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/associated_service.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     8869 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/base.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      335 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/departure_flight_detail.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      271 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/departure_service_room.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      278 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/document_info.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      225 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/dossier_feature.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      321 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/incomplete_requirement.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      268 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/international_ticket_number.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1319 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/price_band.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      945 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/price_promotion.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1701 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/room.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      251 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/models/traveller_height.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     6200 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/query.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     6368 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/request.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy/resources/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2354 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/__init__.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     3315 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/base.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy/resources/booking/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      604 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/__init__.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1156 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/agency.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      385 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/agency_chain.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      363 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/agent.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1162 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/booking.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      902 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/customer.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      184 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/declined_reason.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      632 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/document.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      359 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/nationality.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      701 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/override.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      397 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/override_reason.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     8562 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/service.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      557 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/booking/transaction.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy/resources/checkin/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       29 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/checkin/__init__.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      712 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/checkin/checkin.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy/resources/dossier/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      453 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/__init__.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      904 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/accommodation_dossier.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2622 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/activity_dossier.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      619 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/country_dossier.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1405 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/details.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      387 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/dossier_features.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      445 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/dossier_segment.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      596 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/place_dossier.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      291 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/service_level.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      860 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/dossier/transport_dossier.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy/resources/geo/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      262 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/geo/__init__.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      414 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/geo/airport.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      358 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/geo/continent.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      301 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/geo/country.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      419 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/geo/feature.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      305 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/geo/feature_category.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1514 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/geo/place.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      437 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/geo/state.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      302 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/geo/timezone.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      376 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/language.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy/resources/tour/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      535 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/__init__.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      919 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/accommodation.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      710 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/activity.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1220 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/departure.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1001 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/departure_component.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      702 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/image.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     5046 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/itinerary.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2440 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/promotion.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      552 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/single_supplement.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1354 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/tour.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      472 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/tour_category.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2600 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/tour_dossier.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      553 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/transport.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      332 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/resources/tour/video.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     4738 2017-11-23 16:44:32.000000 gapipy-2.9.3/gapipy/utils.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy.egg-info/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        1 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy.egg-info/dependency_links.txt
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        1 2017-11-23 17:02:43.000000 gapipy-2.9.3/gapipy.egg-info/not-zip-safe
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    33638 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy.egg-info/PKG-INFO
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       16 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy.egg-info/requires.txt
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     3106 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy.egg-info/SOURCES.txt
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       13 2017-11-23 17:04:49.000000 gapipy-2.9.3/gapipy.egg-info/top_level.txt
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    17464 2017-11-23 16:45:32.000000 gapipy-2.9.3/HISTORY.rst
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1079 2017-11-23 16:44:32.000000 gapipy-2.9.3/LICENSE
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)      199 2017-11-23 16:44:32.000000 gapipy-2.9.3/MANIFEST.in
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    33638 2017-11-23 17:04:49.000000 gapipy-2.9.3/PKG-INFO
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     8318 2017-11-23 16:44:32.000000 gapipy-2.9.3/README.rst
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)       85 2017-11-23 17:04:49.000000 gapipy-2.9.3/setup.cfg
+-rwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1287 2017-11-23 16:44:32.000000 gapipy-2.9.3/setup.py
+drwxr-xr-x   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 17:04:49.000000 gapipy-2.9.3/tests/
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)        0 2017-11-23 16:44:32.000000 gapipy-2.9.3/tests/__init__.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    19222 2017-11-23 16:44:32.000000 gapipy-2.9.3/tests/fixtures.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     1828 2017-11-23 16:44:32.000000 gapipy-2.9.3/tests/test_cache.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2422 2017-11-23 16:44:32.000000 gapipy-2.9.3/tests/test_client.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     4225 2017-11-23 16:44:32.000000 gapipy-2.9.3/tests/test_live_api.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)    15076 2017-11-23 16:44:32.000000 gapipy-2.9.3/tests/test_query.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2509 2017-11-23 16:44:32.000000 gapipy-2.9.3/tests/test_request.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     7717 2017-11-23 16:44:32.000000 gapipy-2.9.3/tests/test_resources.py
+-rw-r--r--   0 aesmailjee (1274461873) GADVENTURES\Domain Users (545545006)     2557 2017-11-23 16:44:32.000000 gapipy-2.9.3/tests/test_utils.py
```

### Comparing `gapipy-2.9.1/docs/conf.py` & `gapipy-2.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/docs/make.bat` & `gapipy-2.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/docs/Makefile` & `gapipy-2.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/cache.py` & `gapipy-2.9.3/gapipy/cache.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/client.py` & `gapipy-2.9.3/gapipy/client.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/models/__init__.py` & `gapipy-2.9.3/gapipy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/models/addon.py` & `gapipy-2.9.3/gapipy/models/addon.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/models/base.py` & `gapipy-2.9.3/gapipy/models/base.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/models/price_band.py` & `gapipy-2.9.3/gapipy/models/price_band.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/models/price_promotion.py` & `gapipy-2.9.3/gapipy/models/price_promotion.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/models/room.py` & `gapipy-2.9.3/gapipy/models/room.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/query.py` & `gapipy-2.9.3/gapipy/query.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/request.py` & `gapipy-2.9.3/gapipy/request.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/__init__.py` & `gapipy-2.9.3/gapipy/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/base.py` & `gapipy-2.9.3/gapipy/resources/base.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/booking/__init__.py` & `gapipy-2.9.3/gapipy/resources/booking/__init__.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/booking/agency.py` & `gapipy-2.9.3/gapipy/resources/booking/agency.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/booking/booking.py` & `gapipy-2.9.3/gapipy/resources/booking/booking.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/booking/customer.py` & `gapipy-2.9.3/gapipy/resources/booking/customer.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/booking/document.py` & `gapipy-2.9.3/gapipy/resources/booking/document.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/booking/override.py` & `gapipy-2.9.3/gapipy/resources/booking/override.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/booking/service.py` & `gapipy-2.9.3/gapipy/resources/booking/service.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/booking/transaction.py` & `gapipy-2.9.3/gapipy/resources/booking/transaction.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/checkin/checkin.py` & `gapipy-2.9.3/gapipy/resources/checkin/checkin.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/dossier/accommodation_dossier.py` & `gapipy-2.9.3/gapipy/resources/dossier/accommodation_dossier.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/dossier/activity_dossier.py` & `gapipy-2.9.3/gapipy/resources/dossier/activity_dossier.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/dossier/country_dossier.py` & `gapipy-2.9.3/gapipy/resources/dossier/country_dossier.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/dossier/details.py` & `gapipy-2.9.3/gapipy/resources/dossier/details.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/dossier/place_dossier.py` & `gapipy-2.9.3/gapipy/resources/dossier/place_dossier.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/dossier/transport_dossier.py` & `gapipy-2.9.3/gapipy/resources/dossier/transport_dossier.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/geo/place.py` & `gapipy-2.9.3/gapipy/resources/geo/place.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/__init__.py` & `gapipy-2.9.3/gapipy/resources/tour/__init__.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/accommodation.py` & `gapipy-2.9.3/gapipy/resources/tour/accommodation.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/activity.py` & `gapipy-2.9.3/gapipy/resources/tour/activity.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/departure.py` & `gapipy-2.9.3/gapipy/resources/tour/departure.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/departure_component.py` & `gapipy-2.9.3/gapipy/resources/tour/departure_component.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/image.py` & `gapipy-2.9.3/gapipy/resources/tour/image.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/itinerary.py` & `gapipy-2.9.3/gapipy/resources/tour/itinerary.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/promotion.py` & `gapipy-2.9.3/gapipy/resources/tour/promotion.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/single_supplement.py` & `gapipy-2.9.3/gapipy/resources/tour/single_supplement.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/tour.py` & `gapipy-2.9.3/gapipy/resources/tour/tour.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/tour_dossier.py` & `gapipy-2.9.3/gapipy/resources/tour/tour_dossier.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/resources/tour/transport.py` & `gapipy-2.9.3/gapipy/resources/tour/transport.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy/utils.py` & `gapipy-2.9.3/gapipy/utils.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/gapipy.egg-info/PKG-INFO` & `gapipy-2.9.3/gapipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gapipy
-Version: 2.9.1
+Version: 2.9.3
 Summary: Python client for the G Adventures REST API
 Home-page: https://github.com/gadventures/gapipy
 Author: G Adventures
 Author-email: software@gadventures.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: ===============================
@@ -260,21 +260,27 @@
         
         
         
         
         History
         =======
         
+        2.9.3 (2017-11-23)
+        ------------------
+        * Expose `requirement_set` for `departure_services` and `activity_services`.
+        * *NOTE*: We have skipped `2.9.2` due to pypi upload issues.
+        
+        
         2.9.1 (2017-11-22)
         ------------------
         
         * Adds the `options` method on the Resource Query object.
           A more detailed description of the issue can be found at:
           * https://github.com/gadventures/gapipy/releases/2.9.1
-        * *NOTE*: We have skip `2.9.0` due to pypi upload issues
+        * *NOTE*: We have skipped `2.9.0` due to pypi upload issues
         
         
         2.8.2 (2017-11-14)
         ------------------
         
         * Adds fields `sale_start_datetime` and `sale_finish_datetime` to the
           Promotion resource. The fields mark the start/finish date-time values
```

### Comparing `gapipy-2.9.1/gapipy.egg-info/SOURCES.txt` & `gapipy-2.9.3/gapipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/HISTORY.rst` & `gapipy-2.9.3/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 .. :changelog:
 
 History
 =======
 
+2.9.3 (2017-11-23)
+------------------
+* Expose `requirement_set` for `departure_services` and `activity_services`.
+* *NOTE*: We have skipped `2.9.2` due to pypi upload issues.
+
+
 2.9.1 (2017-11-22)
 ------------------
 
 * Adds the `options` method on the Resource Query object.
   A more detailed description of the issue can be found at:
   * https://github.com/gadventures/gapipy/releases/2.9.1
-* *NOTE*: We have skip `2.9.0` due to pypi upload issues
+* *NOTE*: We have skipped `2.9.0` due to pypi upload issues
 
 
 2.8.2 (2017-11-14)
 ------------------
 
 * Adds fields `sale_start_datetime` and `sale_finish_datetime` to the
   Promotion resource. The fields mark the start/finish date-time values
```

### Comparing `gapipy-2.9.1/LICENSE` & `gapipy-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/PKG-INFO` & `gapipy-2.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gapipy
-Version: 2.9.1
+Version: 2.9.3
 Summary: Python client for the G Adventures REST API
 Home-page: https://github.com/gadventures/gapipy
 Author: G Adventures
 Author-email: software@gadventures.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: ===============================
@@ -260,21 +260,27 @@
         
         
         
         
         History
         =======
         
+        2.9.3 (2017-11-23)
+        ------------------
+        * Expose `requirement_set` for `departure_services` and `activity_services`.
+        * *NOTE*: We have skipped `2.9.2` due to pypi upload issues.
+        
+        
         2.9.1 (2017-11-22)
         ------------------
         
         * Adds the `options` method on the Resource Query object.
           A more detailed description of the issue can be found at:
           * https://github.com/gadventures/gapipy/releases/2.9.1
-        * *NOTE*: We have skip `2.9.0` due to pypi upload issues
+        * *NOTE*: We have skipped `2.9.0` due to pypi upload issues
         
         
         2.8.2 (2017-11-14)
         ------------------
         
         * Adds fields `sale_start_datetime` and `sale_finish_datetime` to the
           Promotion resource. The fields mark the start/finish date-time values
```

### Comparing `gapipy-2.9.1/README.rst` & `gapipy-2.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/setup.py` & `gapipy-2.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/tests/fixtures.py` & `gapipy-2.9.3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/tests/test_cache.py` & `gapipy-2.9.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/tests/test_client.py` & `gapipy-2.9.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/tests/test_live_api.py` & `gapipy-2.9.3/tests/test_live_api.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/tests/test_query.py` & `gapipy-2.9.3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/tests/test_request.py` & `gapipy-2.9.3/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/tests/test_resources.py` & `gapipy-2.9.3/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `gapipy-2.9.1/tests/test_utils.py` & `gapipy-2.9.3/tests/test_utils.py`

 * *Files identical despite different names*

