# Comparing `tmp/Leonardo-Ai-SDK-5.4.4.tar.gz` & `tmp/Leonardo-Ai-SDK-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-5.4.4.tar", last modified: Mon May 27 01:06:53 2024, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-5.5.0.tar", last modified: Thu May 30 01:48:09 2024, max compression
```

## Comparing `Leonardo-Ai-SDK-5.4.4.tar` & `Leonardo-Ai-SDK-5.5.0.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.809497 Leonardo-Ai-SDK-5.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-27 01:06:53.809497 Leonardo-Ai-SDK-5.4.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    10345 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 01:06:53.809497 Leonardo-Ai-SDK-5.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.793497 Leonardo-Ai-SDK-5.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.797497 Leonardo-Ai-SDK-5.4.4/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-27 01:06:53.000000 Leonardo-Ai-SDK-5.4.4/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-27 01:06:53.000000 Leonardo-Ai-SDK-5.4.4/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 01:06:53.000000 Leonardo-Ai-SDK-5.4.4/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-27 01:06:53.000000 Leonardo-Ai-SDK-5.4.4/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 01:06:53.000000 Leonardo-Ai-SDK-5.4.4/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.797497 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.797497 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/init_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.797497 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.797497 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.805497 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/creategeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createlcmgeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createtexturegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createvariationnobg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createvariationunzoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createvariationupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/get3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getuserself.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getvariationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/listelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/listplatformmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/performinpaintinglcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/performinstantrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13322 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/pricingcalculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/promptimprove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/promptrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/uploadinitimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/uploadmodelasset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.809497 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/controlnet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/custom_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/lcm_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/model_asset_texture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/pricingcalculatorservices.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/sd_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/sd_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/universal_upscaler_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/variation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/pricing_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/realtime_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    15328 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/texture.py
--rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/threed_model_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:06:53.809497 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-05-27 01:06:42.000000 Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.925593 Leonardo-Ai-SDK-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-30 01:48:09.925593 Leonardo-Ai-SDK-5.5.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10345 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:48:09.925593 Leonardo-Ai-SDK-5.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.909593 Leonardo-Ai-SDK-5.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.909593 Leonardo-Ai-SDK-5.5.0/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-30 01:48:09.000000 Leonardo-Ai-SDK-5.5.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-30 01:48:09.000000 Leonardo-Ai-SDK-5.5.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:48:09.000000 Leonardo-Ai-SDK-5.5.0/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-30 01:48:09.000000 Leonardo-Ai-SDK-5.5.0/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 01:48:09.000000 Leonardo-Ai-SDK-5.5.0/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.913593 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.913593 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/init_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.913593 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.913593 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.921593 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15844 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/creategeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createlcmgeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createtexturegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createvariationnobg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createvariationunzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/get3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getuserself.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/listelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/listplatformmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/performinpaintinglcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/performinstantrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13322 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/pricingcalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/promptimprove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/promptrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/uploadinitimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/uploadmodelasset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.925593 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/controlnet_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/controlnet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/custom_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/lcm_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/model_asset_texture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/pricingcalculatorservices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/sd_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/universal_upscaler_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/variation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/pricing_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/realtime_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15328 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/threed_model_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:48:09.925593 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-05-30 01:47:59.000000 Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-5.4.4/LICENSE.md` & `Leonardo-Ai-SDK-5.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/PKG-INFO` & `Leonardo-Ai-SDK-5.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.4.4
+Version: 5.5.0
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.4 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.5.0 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) res = s.dataset.create_dataset
 (request=operations.CreateDatasetRequestBody( name='', )) if res.object is not
```

### Comparing `Leonardo-Ai-SDK-5.4.4/README.md` & `Leonardo-Ai-SDK-5.5.0/README.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/setup.py` & `Leonardo-Ai-SDK-5.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='Leonardo-Ai-SDK',
-    version='5.4.4',
+    version='5.5.0',
     author='Leonardo-Ai',
     description='Leonardo AI Python Client SDK',
     url='https://github.com/Leonardo-Interactive/leonardo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `Leonardo-Ai-SDK-5.4.4/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-5.5.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.4.4
+Version: 5.5.0
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.4 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.5.0 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) res = s.dataset.create_dataset
 (request=operations.CreateDatasetRequestBody( name='', )) if res.object is not
```

### Comparing `Leonardo-Ai-SDK-5.4.4/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-5.5.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 src/leonardoaisdk/models/operations/promptimprove.py
 src/leonardoaisdk/models/operations/promptrandom.py
 src/leonardoaisdk/models/operations/uploaddatasetimage.py
 src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
 src/leonardoaisdk/models/operations/uploadinitimage.py
 src/leonardoaisdk/models/operations/uploadmodelasset.py
 src/leonardoaisdk/models/shared/__init__.py
+src/leonardoaisdk/models/shared/controlnet_input.py
 src/leonardoaisdk/models/shared/controlnet_type.py
 src/leonardoaisdk/models/shared/custom_model_type.py
 src/leonardoaisdk/models/shared/element_input.py
 src/leonardoaisdk/models/shared/job_status.py
 src/leonardoaisdk/models/shared/lcm_generation_style.py
 src/leonardoaisdk/models/shared/model_asset_texture_types.py
 src/leonardoaisdk/models/shared/pricingcalculatorservices.py
```

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/_hooks/sdkhooks.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/_hooks/types.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/elements.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/elements.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/image.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/image.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/init_images.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/init_images.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/errors/sdkerror.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ...models.shared import controlnet_input as shared_controlnet_input
 from ...models.shared import controlnet_type as shared_controlnet_type
 from ...models.shared import element_input as shared_element_input
 from ...models.shared import sd_generation_schedulers as shared_sd_generation_schedulers
 from ...models.shared import sd_generation_style as shared_sd_generation_style
 from ...models.shared import sd_versions as shared_sd_versions
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
@@ -26,17 +27,24 @@
     r"""Query parameters to be provided in the request body as a JSON object"""
     UNSET='__SPEAKEASY_UNSET__'
     alchemy: Optional[bool] = dataclasses.field(default=True, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alchemy'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use Alchemy. Note: The appropriate Alchemy version is selected for the specified model. For example, XL models will use Alchemy V2."""
     contrast_ratio: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contrastRatio'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Contrast Ratio to use with Alchemy. Must be a float between 0 and 1 inclusive."""
     control_net: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('controlNet'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
-    r"""Enable to use ControlNet. Requires an init image to be provided. Requires a model based on SD v1.5"""
+    r"""This parameter will be deprecated in September 2024. Please use the controlnets array instead.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     control_net_type: Optional[shared_controlnet_type.ControlnetType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('controlNetType'), 'exclude': lambda f: f is None }})
-    r"""The type of ControlNet to use."""
+    r"""This parameter will be deprecated in September 2024. Please use the controlnets array instead.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
+    controlnets: Optional[List[shared_controlnet_input.ControlnetInput]] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('controlnets'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     elements: Optional[List[shared_element_input.ElementInput]] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('elements'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     expanded_domain: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expandedDomain'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use the Expanded Domain feature of Alchemy."""
     fantasy_avatar: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fantasyAvatar'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use the Fantasy Avatar feature."""
     guidance_scale: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guidance_scale'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How strongly the generation should reflect the prompt. 7 is recommended. Must be between 1 and 20."""
@@ -92,15 +100,18 @@
     unzoom: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unzoom'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Whether the generated images should be unzoomed (requires unzoomAmount and init_image_id to be set)."""
     unzoom_amount: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unzoomAmount'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How much the image should be unzoomed (requires an init_image_id and unzoom to be set to true)."""
     upscale_ratio: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('upscaleRatio'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How much the image should be upscaled. (Enterprise Only)"""
     weighting: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weighting'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
-    r"""How much weighting to use for ControlNet. This parameter works with controlNet and controlNetType."""
+    r"""This parameter will be deprecated in September 2024. Please use the controlnets array instead.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     width: Optional[int] = dataclasses.field(default=1024, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The input width of the images. Must be between 32 and 1024 and be a multiple of 8. Note: Input resolution is not always the same as output resolution due to upscaling from other features."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createlcmgeneration.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createlcmgeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createtexturegeneration.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createtexturegeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createvariationnobg.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createvariationnobg.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createvariationunzoom.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createvariationunzoom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/delete3dmodelbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/delete3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/get3dmodelbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/get3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/listelements.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/listelements.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/listplatformmodels.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/listplatformmodels.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/performinpaintinglcm.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/performinpaintinglcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/performinstantrefine.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/performinstantrefine.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/pricingcalculator.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/pricingcalculator.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/promptimprove.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/promptimprove.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/promptrandom.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/promptrandom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/operations/uploadmodelasset.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/operations/uploadmodelasset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/__init__.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
+from .controlnet_input import *
 from .controlnet_type import *
 from .custom_model_type import *
 from .element_input import *
 from .job_status import *
 from .lcm_generation_style import *
 from .model_asset_texture_types import *
 from .pricingcalculatorservices import *
@@ -11,8 +12,8 @@
 from .sd_generation_style import *
 from .sd_versions import *
 from .security import *
 from .strength import *
 from .universal_upscaler_style import *
 from .variation_type import *
 
-__all__ = ["ControlnetType","CustomModelType","ElementInput","JobStatus","LcmGenerationStyle","ModelAssetTextureTypes","PricingCalculatorServices","SdGenerationSchedulers","SdGenerationStyle","SdVersions","Security","Strength","UniversalUpscalerStyle","VariationType"]
+__all__ = ["ControlnetInput","ControlnetType","CustomModelType","ElementInput","InitImageType","JobStatus","LcmGenerationStyle","ModelAssetTextureTypes","PricingCalculatorServices","SdGenerationSchedulers","SdGenerationStyle","SdVersions","Security","Strength","StrengthType","UniversalUpscalerStyle","VariationType"]
```

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/element_input.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/element_input.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/lcm_generation_style.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/lcm_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/pricingcalculatorservices.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/pricingcalculatorservices.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/sd_generation_style.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/sd_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models/shared/sd_versions.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models/shared/sd_versions.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/models_.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/models_.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/motion.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/motion.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/pricing_calculator.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/pricing_calculator.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/prompt.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/prompt.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/realtime_canvas.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/realtime_canvas.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/sdk.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '5.4.4'
-    gen_version: str = '2.335.5'
-    user_agent: str = 'speakeasy-sdk/python 5.4.4 2.335.5 v1.0.0 Leonardo-Ai-SDK'
+    sdk_version: str = '5.5.0'
+    gen_version: str = '2.338.1'
+    user_agent: str = 'speakeasy-sdk/python 5.5.0 2.338.1 v1.0.0 Leonardo-Ai-SDK'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/texture.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/texture.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/threed_model_assets.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/threed_model_assets.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.4/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-5.5.0/src/leonardoaisdk/variation.py`

 * *Files identical despite different names*

