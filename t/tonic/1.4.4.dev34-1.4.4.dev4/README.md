# Comparing `tmp/tonic-1.4.4.dev34.tar.gz` & `tmp/tonic-1.4.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic-1.4.4.dev34.tar", last modified: Thu May 30 16:51:50 2024, max compression
+gzip compressed data, was "tonic-1.4.4.dev4.tar", last modified: Fri Dec 15 18:13:25 2023, max compression
```

## Comparing `tonic-1.4.4.dev34.tar` & `tonic-1.4.4.dev4.tar`

### file list

```diff
@@ -1,203 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.517836 tonic-1.4.4.dev34/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.485836 tonic-1.4.4.dev34/.binder/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/.binder/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.481836 tonic-1.4.4.dev34/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.485836 tonic-1.4.4.dev34/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-30 16:51:50.000000 tonic-1.4.4.dev34/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    45450 2024-05-30 16:51:50.000000 tonic-1.4.4.dev34/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-30 16:51:50.517836 tonic-1.4.4.dev34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.489836 tonic-1.4.4.dev34/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.489836 tonic-1.4.4.dev34/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.489836 tonic-1.4.4.dev34/docs/_static/event-cameras/
--rw-r--r--   0 runner    (1001) docker     (127)   460683 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/event-cameras/eventstream.png
--rw-r--r--   0 runner    (1001) docker     (127)   209036 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/event-cameras/framestream.png
--rw-r--r--   0 runner    (1001) docker     (127)    28336 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/event-cameras/receptive-fields.png
--rw-r--r--   0 runner    (1001) docker     (127)    18392 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/event-cameras/sampling-theorems.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.493836 tonic-1.4.4.dev34/docs/_static/snn/
--rw-r--r--   0 runner    (1001) docker     (127)   119778 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/snn/neuron-models.png
--rw-r--r--   0 runner    (1001) docker     (127)    62505 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/snn/surrogates.png
--rw-r--r--   0 runner    (1001) docker     (127)   188640 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/tonic-logo-black-bg.png
--rw-r--r--   0 runner    (1001) docker     (127)   196968 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/tonic-logo-black.png
--rw-r--r--   0 runner    (1001) docker     (127)   193807 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/tonic-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_static/tonic_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.493836 tonic-1.4.4.dev34/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_templates/class_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/_templates/class_transform.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.493836 tonic-1.4.4.dev34/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/about/info.rst
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/about/prototype.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/about/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.493836 tonic-1.4.4.dev34/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.493836 tonic-1.4.4.dev34/docs/gallery/representations/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/representations/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/representations/plot_tobinarep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/representations/plot_toframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/representations/plot_toimage.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/representations/plot_totimesurface.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/representations/plot_tovoxelgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.497836 tonic-1.4.4.dev34/docs/gallery/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_centercrop.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_crop_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_decimation.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_denoise.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_drop_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_drop_event_by_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_drop_event_by_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_event_downsampling.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_merge_polarities.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_random_flip_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_random_flip_ud.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_random_time_reversal.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/gallery/transformations/plot_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.497836 tonic-1.4.4.dev34/docs/getting_involved/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/getting_involved/communication_channels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/getting_involved/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/getting_involved/getting_involved.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.497836 tonic-1.4.4.dev34/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/getting_started/nmnist.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.497836 tonic-1.4.4.dev34/docs/how-tos/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/how-tos/how-tos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/how-tos/loading-raw-events.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/how-tos/visualizing-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/how-tos/wrapping_own_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.497836 tonic-1.4.4.dev34/docs/reading_material/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/reading_material/design_choices.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/reading_material/intro-event-cameras.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/reading_material/intro-snns.rst
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/reading_material/reading_material.rst
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/reading_material/training-snns.rst
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/transformations.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.501836 tonic-1.4.4.dev34/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/tutorials/Aug_DiskCachDataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1908452 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/tutorials/audio_transforms_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/tutorials/batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/tutorials/davis_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/tutorials/fast_dataloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12518 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/tutorials/large_datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/tutorials/slicing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-30 16:51:50.517836 tonic-1.4.4.dev34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.505836 tonic-1.4.4.dev34/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/prototype_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_audio_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_aug_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_chained_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.509836 tonic-1.4.4.dev34/test/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)   949253 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_data/sample.aedat4
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_data/sample_aedat_header.aedat
--rw-r--r--   0 runner    (1001) docker     (127)    16165 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_data/sample_ncars.dat
--rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_data/sample_nmnist.bin
--rw-r--r--   0 runner    (1001) docker     (127)    38132 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_data/sample_stmnist.mat
--rw-r--r--   0 runner    (1001) docker     (127)     9409 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_dsec.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_prototype_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_slicers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_tonic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23854 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/torch_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.509836 tonic-1.4.4.dev34/tonic/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/audio_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/collation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.513836 tonic-1.4.4.dev34/tonic/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/asl_dvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/cifar10dvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/davisdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/dsec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/dvs_lips.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/dvsgesture.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/ebssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/hsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/mvsec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/ncaltech101.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/pokerdvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/s_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/threeET_eyetracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/tum_vie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/datasets/visual_place_recognition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.517836 tonic-1.4.4.dev34/tonic/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/crop.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/decimate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/denoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/drop_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/event_downsampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/time_skew.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/to_averaged_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/to_bina_rep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/to_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/to_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/to_voxel_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/functional/uniform_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.517836 tonic-1.4.4.dev34/tonic/prototype/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.517836 tonic-1.4.4.dev34/tonic/prototype/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/datasets/ncars.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/datasets/prophesee.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/datasets/stmnist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.517836 tonic-1.4.4.dev34/tonic/prototype/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/datasets/utils/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/datasets/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/prototype/slicers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/slicers.py
--rw-r--r--   0 runner    (1001) docker     (127)    42237 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   212526 2024-05-30 16:51:38.000000 tonic-1.4.4.dev34/tonic-logo-padded.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:51:50.513836 tonic-1.4.4.dev34/tonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-30 16:51:50.000000 tonic-1.4.4.dev34/tonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-30 16:51:50.000000 tonic-1.4.4.dev34/tonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:51:50.000000 tonic-1.4.4.dev34/tonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:51:50.000000 tonic-1.4.4.dev34/tonic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 16:51:50.000000 tonic-1.4.4.dev34/tonic.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-30 16:51:50.000000 tonic-1.4.4.dev34/tonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 16:51:50.000000 tonic-1.4.4.dev34/tonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.112257 tonic-1.4.4.dev4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.084257 tonic-1.4.4.dev4/.binder/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/.binder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.080257 tonic-1.4.4.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.084257 tonic-1.4.4.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2023-12-15 18:13:24.000000 tonic-1.4.4.dev4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    42810 2023-12-15 18:13:24.000000 tonic-1.4.4.dev4/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2023-12-15 18:13:25.112257 tonic-1.4.4.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.084257 tonic-1.4.4.dev4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.084257 tonic-1.4.4.dev4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.088257 tonic-1.4.4.dev4/docs/_static/event-cameras/
+-rw-r--r--   0 runner    (1001) docker     (127)   460683 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/event-cameras/eventstream.png
+-rw-r--r--   0 runner    (1001) docker     (127)   209036 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/event-cameras/framestream.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28336 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/event-cameras/receptive-fields.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18392 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/event-cameras/sampling-theorems.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.088257 tonic-1.4.4.dev4/docs/_static/snn/
+-rw-r--r--   0 runner    (1001) docker     (127)   119778 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/snn/neuron-models.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62505 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/snn/surrogates.png
+-rw-r--r--   0 runner    (1001) docker     (127)   188640 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/tonic-logo-black-bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)   196968 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/tonic-logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)   193807 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/tonic-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_static/tonic_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.088257 tonic-1.4.4.dev4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_templates/class_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/_templates/class_transform.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.088257 tonic-1.4.4.dev4/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/about/info.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/about/prototype.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/about/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.088257 tonic-1.4.4.dev4/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.088257 tonic-1.4.4.dev4/docs/gallery/representations/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/representations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/representations/plot_tobinarep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/representations/plot_toframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/representations/plot_toimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/representations/plot_totimesurface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/representations/plot_tovoxelgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.092257 tonic-1.4.4.dev4/docs/gallery/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_centercrop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_crop_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_decimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_drop_event_by_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_drop_event_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_event_downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_merge_polarities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_random_flip_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_random_flip_ud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_random_time_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/gallery/transformations/plot_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.092257 tonic-1.4.4.dev4/docs/getting_involved/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/getting_involved/communication_channels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/getting_involved/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/getting_involved/getting_involved.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.092257 tonic-1.4.4.dev4/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/getting_started/nmnist.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.096257 tonic-1.4.4.dev4/docs/how-tos/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/how-tos/how-tos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/how-tos/loading-raw-events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/how-tos/visualizing-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/how-tos/wrapping_own_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.096257 tonic-1.4.4.dev4/docs/reading_material/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/reading_material/design_choices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11178 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/reading_material/intro-event-cameras.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/reading_material/intro-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/reading_material/reading_material.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/reading_material/training-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/transformations.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.096257 tonic-1.4.4.dev4/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/tutorials/batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/tutorials/davis_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/tutorials/fast_dataloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12518 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/tutorials/large_datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/tutorials/slicing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-15 18:13:25.112257 tonic-1.4.4.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.100257 tonic-1.4.4.dev4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/prototype_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_chained_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.100257 tonic-1.4.4.dev4/test/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   949253 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_data/sample.aedat4
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_data/sample_aedat_header.aedat
+-rw-r--r--   0 runner    (1001) docker     (127)    16165 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_data/sample_ncars.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    21625 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_data/sample_nmnist.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    38132 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_data/sample_stmnist.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_dsec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_prototype_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_slicers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_tonic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23854 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.104257 tonic-1.4.4.dev4/tonic/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/collation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.104257 tonic-1.4.4.dev4/tonic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/asl_dvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/cifar10dvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/davisdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/dsec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/dvs_lips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/dvsgesture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/ebssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/hsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7708 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/mvsec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/ncaltech101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/pokerdvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/s_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/tum_vie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7894 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/datasets/visual_place_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.108257 tonic-1.4.4.dev4/tonic/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/event_downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/time_skew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/to_averaged_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/to_bina_rep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/to_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/to_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/to_voxel_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/functional/uniform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.108257 tonic-1.4.4.dev4/tonic/prototype/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.108257 tonic-1.4.4.dev4/tonic/prototype/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/datasets/ncars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11417 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/datasets/prophesee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/datasets/stmnist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.108257 tonic-1.4.4.dev4/tonic/prototype/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/datasets/utils/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/datasets/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/prototype/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42237 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   212526 2023-12-15 18:13:13.000000 tonic-1.4.4.dev4/tonic-logo-padded.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 18:13:25.104257 tonic-1.4.4.dev4/tonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2023-12-15 18:13:24.000000 tonic-1.4.4.dev4/tonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2023-12-15 18:13:25.000000 tonic-1.4.4.dev4/tonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 18:13:24.000000 tonic-1.4.4.dev4/tonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 18:13:24.000000 tonic-1.4.4.dev4/tonic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-15 18:13:24.000000 tonic-1.4.4.dev4/tonic.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-15 18:13:24.000000 tonic-1.4.4.dev4/tonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-15 18:13:24.000000 tonic-1.4.4.dev4/tonic.egg-info/top_level.txt
```

### Comparing `tonic-1.4.4.dev34/.github/workflows/ci-pipeline.yml` & `tonic-1.4.4.dev4/.github/workflows/ci-pipeline.yml`

 * *Files 21% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 jobs:
   multitest:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-2022]
-        python-version: ["3.8", "3.10", "3.11"]
+        python-version: ["3.7", "3.9", "3.11"]
     steps:
       - uses: actions/checkout@v3
       - if: matrix.os == 'ubuntu-latest'
         name: install audio library libsndfile
         run: sudo apt-get -y update && sudo apt-get install -y libsndfile1
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install requirements
         run: |
+          pip install torch torchvision --index-url https://download.pytorch.org/whl/cpu
           pip install -r test/requirements.txt
-          pip install -r test/torch_requirements.txt
           pip install .
       - name: Test with pytest
         run: pytest test
         env:
             CI: true
 
   coverage:
@@ -38,16 +38,16 @@
         run: sudo apt-get -y update && sudo apt-get install -y libsndfile1
       - name: Setup Python 3.9
         uses: actions/setup-python@v3
         with:
           python-version: 3.9
       - name: Generate coverage report
         run: |
+          pip install torch torchvision --index-url https://download.pytorch.org/whl/cpu
           pip install -r test/requirements.txt
-          pip install -r test/torch_requirements.txt
           pip install .
           coverage run -m pytest test
           coverage xml
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v3
 
   documentation:
@@ -59,16 +59,16 @@
         run: sudo apt-get -y update && sudo apt-get install -y libsndfile1
       - name: Setup Python 3.9
         uses: actions/setup-python@v3
         with:
           python-version: 3.9
       - name: Install dependencies
         run: |
+          pip install torch torchvision --index-url https://download.pytorch.org/whl/cpu
           pip install -r docs/requirements.txt
-          pip install -r test/torch_requirements.txt
           pip install .
       - name: Build documentation
         run: cd docs && make clean && make html # Use SPHINXOPTS="-W" to fail on warning.
 
   build-and-publish:
     needs: documentation
     if: github.event_name == 'push'
```

### Comparing `tonic-1.4.4.dev34/AUTHORS` & `tonic-1.4.4.dev4/AUTHORS`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Anindya Ghosh <anindya128@yahoo.com>
 Antoine Grimaldi <antoine.grimaldi@univ-amu.fr>
 AntoineGrimaldi <antoine.grimaldi@univ-amu.fr>
 Carsten Nielsen <carstenlau.nielsen@uzh.ch>
-Elias Martinsson <131291250+e-martinsson@users.noreply.github.com>
 Fabrizio Ottati <45739782+fabhertz95@users.noreply.github.com>
 Fabrizio Ottati <fabriziottati@gmail.com>
 Felix Bauer <felix.bauer@aictx.ai>
 Gokul B. Nair <14059534+gokulbnr@users.noreply.github.com>
 Gokul B. Nair <gokulbnr@gmail.com>
 Gregor Lenz <gregor.lenz@synsense.ai>
-Gregor Lenz <gregor@neurobus.space>
 Gregor Lenz <mail@lenzgregor.com>
 Guido Zarrella <jzarrella@mitre.org>
 James Knight <jk421@inf900374.inf.susx.ac.uk>
 Jan <jan.finkbeiner@t-online.de>
 Jan Finkbeiner <j.finkbeiner@fz-juelich.de>
 Jens Egholm <jensegholm@protonmail.com>
 Jonah P. Sengupta <jsengup1@jhu.edu>
 Kenneth Chaney <chaneyk@seas.upenn.edu>
 Laurent Perrinet <laurent.perrinet@univ-amu.fr>
 Marco Rasetto <marcorax93@gmail.com>
-Mina Khoei <mina.khoei@synsense.ai>
 MrPeterJin <Cheng.Jin@std.uestc.edu.cn>
 Omar Oubari <omaroubari@gmail.com>
 Sadique Sheik <sadique.sheik@aictx.ai>
 Sadique Sheik <sadique.sheik@synsense.ai>
 Sadique Sheik <sheiksadique@gmail.com>
 Sami Barchid <sami.barchid@univ-lille.fr>
 Simon Narduzzi <simon.narduzzi@gmail.com>
 Thomas Nowotny <t.nowotny@sussex.ac.uk>
 Tobias Fischer <info@tobiasfischer.info>
 Yalun_Hu <yalun.hu@synsense.ai>
-ZuowenWang0000 <wangzu@ethz.ch>
 anindyaghosh <anindya128@yahoo.com>
 bamsumit <bam_sumit@hotmail.com>
 fabrizio.ottati <fabrizio.ottati@studenti.polito.it>
 guidoz <guidoz@users.noreply.github.com>
 k-chaney <chaneyk@seas.upenn.edu>
 kai.wang <kai.wang@synsense.ai>
 neworderofjamie <J.C.Knight@sussex.ac.uk>
```

### Comparing `tonic-1.4.4.dev34/ChangeLog` & `tonic-1.4.4.dev4/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,90 +1,24 @@
 CHANGES
 =======
 
-* DataSet class import was removed, the mini dataset does not inherent from that
-* moving torchvision import to inside function
-* moving typing-extensions to the root requirement
-* moving torch import to inside function, where it is used
-* pin torchvision version to something compatible with torch 2.1
-* add torch requirements to documentation github action
-* shorten GH actions pipeline to three Python versions
-* specified unit
-* build lists of users indices and lighting  in DVS gesture
-* Update ebssa.py
-* fix typo
-* fix path format on windows for test case for ThreeET\_Eyetracking
-* Revert "fix path format on windows for test case for ThreeET\_Eyetracking"
-* fix path format on windows for test case for ThreeET\_Eyetracking
-* add test case for ThreeET\_Eyetracking
-* notebook added to elaborate teh function of AugDiskCachedDataset
-* test added for aug\_diskcached
-* including Aug\_DiskCachedDataset in init imports
-* bug fixed in Aug\_DiskCach
-* add ThreeET\_Eyetracking to the documentation
 * fix: check for empty array in DropPixel transform
 * added: tests for empty frames
 * exclude AUTHORS and ChangeLog files
 
 v1.4.3
 ------
 
 * Update communication\_channels.rst
 * Update Discord badge in docs
 * Update Discord badge
 * Update Discord invite link
-* change .h5 file loader to h5py
-* add 3ET eye tracking dataset
-* add threeET\_eyetracking(3et) dataset
-* tutorial added for audio transforms/augmentations
-* bug fixed in test
-* sample\_length was removed from some transforms (when not needed)
 * Fix: silent frames is now supported in uniform noise
 * Fix: silent frame support
-* importing TypedDict from typing\_extensions for python 3.7
-* adding typing-extensions to requirments
-* small fixes and cleanup
-* noise related augmentations removed
 * Fix: wrong range of histogram in drop\_pixel
-* Testing with python>=3.8 and python<=3.11
-* Update ci-pipeline.yml
-* Update torch\_requirements.txt
-* Update ci-pipeline.yml
-* Update torch\_requirements.txt
-* Update ci-pipeline.yml
-* Update torch\_requirements.txt
-* Update requirements.txt
-* Create torch\_requirements.txt
-* Update requirements.txt
-* Update requirements.txt
-* merge
-* Trying to make torchaudio work
-* cpu version is spesified for torchaudio
-* adding torchaudio
-* removing conflicting requirements
-* updated the required version of torch
-* dict keys updated to more generic
-* RIR test updated
-* removing hard coded room impulse audio from RIR transform
-* requirments updated with torch and torchaudio versions
-* removing torchaudio dependency temporarily to run the tests
-* torchaudio added to requirements
-* AugDiskCachedDataset added
-* tests\_passed
-* tests for audio augmentations
-* tests for added transforms
-* fixes in docstrings
-* typos fixed in docstrings
-* Noise augmentations added
-* AmplitudeScale and RobustAmplitudeScale transforms added
-* RIR transform (room impulse response) added
-* RandomAmplitudeScale is added
-* RandomPitchShift transfrom added
-* audio\_augmentation module is added: with RandomTimeStretch
-* new transform added: SwapAxes
 * fix EBSSA test sample file path
 * Prophesee prototype docstring updates
 * update documentation config
 * exclude sphinx gallery READMEs
 * update incoherent docstrings
 * Update .readthedocs.yml
 * unskip some DSEC tests
```

### Comparing `tonic-1.4.4.dev34/LICENSE.txt` & `tonic-1.4.4.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/PKG-INFO` & `tonic-1.4.4.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.4.4.dev34
+Version: 1.4.4.dev4
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.4.4.dev34/README.md` & `tonic-1.4.4.dev4/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/Makefile` & `tonic-1.4.4.dev4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/event-cameras/eventstream.png` & `tonic-1.4.4.dev4/docs/_static/event-cameras/eventstream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/event-cameras/framestream.png` & `tonic-1.4.4.dev4/docs/_static/event-cameras/framestream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/event-cameras/receptive-fields.png` & `tonic-1.4.4.dev4/docs/_static/event-cameras/receptive-fields.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/event-cameras/sampling-theorems.png` & `tonic-1.4.4.dev4/docs/_static/event-cameras/sampling-theorems.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/snn/neuron-models.png` & `tonic-1.4.4.dev4/docs/_static/snn/neuron-models.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/snn/surrogates.png` & `tonic-1.4.4.dev4/docs/_static/snn/surrogates.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/tonic-logo-black-bg.png` & `tonic-1.4.4.dev4/docs/_static/tonic-logo-black-bg.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/tonic-logo-black.png` & `tonic-1.4.4.dev4/docs/_static/tonic-logo-black.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/tonic-logo-white.png` & `tonic-1.4.4.dev4/docs/_static/tonic-logo-white.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/_static/tonic_favicon.png` & `tonic-1.4.4.dev4/docs/_static/tonic_favicon.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/about/info.rst` & `tonic-1.4.4.dev4/docs/about/info.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/about/prototype.rst` & `tonic-1.4.4.dev4/docs/about/prototype.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/about/release_notes.rst` & `tonic-1.4.4.dev4/docs/about/release_notes.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/conf.py` & `tonic-1.4.4.dev4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/datasets.rst` & `tonic-1.4.4.dev4/docs/datasets.rst`

 * *Files 10% similar despite different names*

```diff
@@ -49,28 +49,20 @@
 -------------------
 .. autosummary::
     :toctree: generated/
     :template: class_dataset.rst
 
     EBSSA
 
-Eye tracking
--------------------
-.. autosummary::
-    :toctree: generated/
-    :template: class_dataset.rst
-
-    ThreeET_Eyetracking
-
 .. currentmodule:: tonic.prototype.datasets
 
 Prototype iterable datasets
 ---------------------------
 .. autosummary::
     :toctree: generated/
     :template: class_dataset.rst
 
     NMNIST
     NCARS
     STMNIST
     Gen1AutomotiveDetection
-    Gen4AutomotiveDetectionMini
+    Gen4AutomotiveDetectionMini
```

### Comparing `tonic-1.4.4.dev34/docs/gallery/representations/plot_tobinarep.py` & `tonic-1.4.4.dev4/docs/gallery/representations/plot_tobinarep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/representations/plot_toframe.py` & `tonic-1.4.4.dev4/docs/gallery/representations/plot_toframe.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/representations/plot_toimage.py` & `tonic-1.4.4.dev4/docs/gallery/representations/plot_toimage.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_centercrop.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_centercrop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_crop_time.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_crop_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_decimation.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_decimation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_denoise.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_downsample.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_downsample.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_drop_event.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_drop_event_by_area.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_drop_event_by_area.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_drop_event_by_time.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_drop_event_by_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_drop_pixel.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_event_downsampling.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_event_downsampling.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_merge_polarities.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_merge_polarities.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_random_crop.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_random_crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_random_flip_lr.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_random_flip_lr.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_random_flip_ud.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_random_flip_ud.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_random_time_reversal.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_random_time_reversal.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_refractory_period.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_spatial_jitter.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_time_jitter.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/gallery/transformations/plot_uniform_noise.py` & `tonic-1.4.4.dev4/docs/gallery/transformations/plot_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/getting_involved/communication_channels.rst` & `tonic-1.4.4.dev4/docs/getting_involved/communication_channels.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/getting_involved/contribute.rst` & `tonic-1.4.4.dev4/docs/getting_involved/contribute.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/getting_started/install.rst` & `tonic-1.4.4.dev4/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/getting_started/nmnist.ipynb` & `tonic-1.4.4.dev4/docs/getting_started/nmnist.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/how-tos/loading-raw-events.ipynb` & `tonic-1.4.4.dev4/docs/how-tos/loading-raw-events.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/how-tos/visualizing-data.ipynb` & `tonic-1.4.4.dev4/docs/how-tos/visualizing-data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/how-tos/wrapping_own_data.ipynb` & `tonic-1.4.4.dev4/docs/how-tos/wrapping_own_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/index.md` & `tonic-1.4.4.dev4/docs/index.md`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/make.bat` & `tonic-1.4.4.dev4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/reading_material/design_choices.rst` & `tonic-1.4.4.dev4/docs/reading_material/design_choices.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/reading_material/intro-event-cameras.rst` & `tonic-1.4.4.dev4/docs/reading_material/intro-event-cameras.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/reading_material/intro-snns.rst` & `tonic-1.4.4.dev4/docs/reading_material/intro-snns.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 Figure 1 shows the principal difference
 between a neuron unit in an ANN and in an SNN. Whereas the input for an
 ANN is typically a
 tensor with high data precision, but low temporal resolution, the input
 for an SNN are
 binary flags of spikes with comparatively high temporal precision in the
-order of µs. The unit in the SNN integrates all of the incoming spikes,
+order of s. The unit in the SNN integrates all of the incoming spikes,
 which affect the internal parameters such as membrane potential. The
 unit in the ANN
 merely computes the linear combination for inputs on all synapses and
 outputs that. Although there are ANN units with memory characteristics and
 internal states such as recurrent or long short-term memory
 units, they typically
 operate on much wider time frames such as a few words in a sentence or a
```

### Comparing `tonic-1.4.4.dev34/docs/reading_material/training-snns.rst` & `tonic-1.4.4.dev4/docs/reading_material/training-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/transformations.rst` & `tonic-1.4.4.dev4/docs/transformations.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/tutorials/batching.ipynb` & `tonic-1.4.4.dev4/docs/tutorials/batching.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/tutorials/davis_data.ipynb` & `tonic-1.4.4.dev4/docs/tutorials/davis_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/tutorials/fast_dataloading.ipynb` & `tonic-1.4.4.dev4/docs/tutorials/fast_dataloading.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/tutorials/large_datasets.ipynb` & `tonic-1.4.4.dev4/docs/tutorials/large_datasets.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/docs/tutorials/slicing.ipynb` & `tonic-1.4.4.dev4/docs/tutorials/slicing.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/setup.cfg` & `tonic-1.4.4.dev4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/dataset_utils.py` & `tonic-1.4.4.dev4/test/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/prototype_dataset_utils.py` & `tonic-1.4.4.dev4/test/prototype_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_caching.py` & `tonic-1.4.4.dev4/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_chained_transforms.py` & `tonic-1.4.4.dev4/test/test_chained_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_data/sample.aedat4` & `tonic-1.4.4.dev4/test/test_data/sample.aedat4`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_data/sample_aedat_header.aedat` & `tonic-1.4.4.dev4/test/test_data/sample_aedat_header.aedat`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_data/sample_ncars.dat` & `tonic-1.4.4.dev4/test/test_data/sample_ncars.dat`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_data/sample_nmnist.bin` & `tonic-1.4.4.dev4/test/test_data/sample_nmnist.bin`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_data/sample_stmnist.mat` & `tonic-1.4.4.dev4/test/test_data/sample_stmnist.mat`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_datasets.py` & `tonic-1.4.4.dev4/test/test_datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -101,45 +101,14 @@
         filename = "Jpw3Adae5kReMrN/download/labelled_ebssa.h5"
         download_url(
             url=base_url + filename, root=testfolder, filename="labelled_ebssa.h5"
         )
         return {"n_samples": 1}
 
 
-class ThreeET_EyetrackingTestCase(dataset_utils.DatasetTestCase):
-    DATASET_CLASS = datasets.ThreeET_Eyetracking
-    FEATURE_TYPES = (datasets.ThreeET_Eyetracking.dtype,)
-    TARGET_TYPES = (np.ndarray,)
-    KWARGS = {"split": "train"}
-
-    def inject_fake_data(self, tmpdir):
-        testfolder = os.path.join(tmpdir, "ThreeET_Eyetracking")
-        os.makedirs(testfolder, exist_ok=True)
-        os.makedirs(os.path.join(testfolder, "data"), exist_ok=True)
-        os.makedirs(os.path.join(testfolder, "labels"), exist_ok=True)
-        # write one line of file name into train_files.txt under testfolder
-        os.system("echo testcase > " + os.path.join(testfolder, "train_files.txt"))
-        filename = "testcase"
-
-        # download test h5 file
-        download_url(
-            url=base_url + "4aiA4BAqz5km4Gc/download/" + filename + ".h5",
-            root=os.path.join(testfolder, "data"),
-            filename=filename + ".h5",
-        )
-        # # download test labels
-        download_url(
-            url=base_url + "G6ejNmXNnB2sKyc/download/" + filename + ".txt",
-            root=os.path.join(testfolder, "labels"),
-            filename=filename + ".txt",
-        )
-
-        return {"n_samples": 1}
-
-
 class NCaltech101TestCase(dataset_utils.DatasetTestCase):
     DATASET_CLASS = datasets.NCALTECH101
     FEATURE_TYPES = (datasets.NCALTECH101.dtype,)
     TARGET_TYPES = (int,)
     KWARGS = {}
 
     def inject_fake_data(self, tmpdir):
```

### Comparing `tonic-1.4.4.dev34/test/test_dsec.py` & `tonic-1.4.4.dev4/test/test_dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_io.py` & `tonic-1.4.4.dev4/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_prototype_datasets.py` & `tonic-1.4.4.dev4/test/test_prototype_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_representations.py` & `tonic-1.4.4.dev4/test/test_representations.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_sliced_dataset.py` & `tonic-1.4.4.dev4/test/test_sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_slicers.py` & `tonic-1.4.4.dev4/test/test_slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_tonic_utils.py` & `tonic-1.4.4.dev4/test/test_tonic_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/test_transforms.py` & `tonic-1.4.4.dev4/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/test/utils.py` & `tonic-1.4.4.dev4/test/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/audio_transforms.py` & `tonic-1.4.4.dev4/tonic/audio_transforms.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,90 +53,14 @@
         n_splits = int(data_len / (self.orig_freq / self.new_freq))
         splits = np.array_split(data, n_splits, axis=self.axis)
         data = [np.sum(split, axis=self.axis, keepdims=True) for split in splits]
         return np.concatenate(data, self.axis)
 
 
 @dataclass
-class SwapAxes:
-    """Interchange two axes of an array.
-
-    Args:
-        ax1 (int): First axis
-        ax2 (int): Second axis
-
-    Returns:
-        np.ndarray : array with interchanged axes
-    """
-
-    ax1: int = 0
-    ax2: int = 1
-
-    def __call__(self, data: np.ndarray) -> np.ndarray:
-        return np.swapaxes(data, self.ax1, self.ax2)
-
-
-@dataclass
-class AmplitudeScale:
-    """Normalize the maximum amplitude of the input signal to a desired value, for instance the
-    value can corespond to the mVolt equivalent of be the maximum loudness of the audio.
-
-    Args:
-        data (np.ndarray): input single- or multi-channel signal.
-
-    Returns:
-        np.ndarray: scaled version of the signal.
-    """
-
-    max_amplitude: float = 158e-3
-
-    def __call__(self, data: np.ndarray) -> np.ndarray:
-        max_data_amplitude = np.max(np.abs(data.ravel()))
-
-        if max_data_amplitude == 0:
-            max_data_amplitude = 1.0
-
-        return data / max_data_amplitude * self.max_amplitude
-
-
-@dataclass
-class RobustAmplitudeScale:
-    """Normalize the maximum amplitude of the input signal while eliminating the outliers, to
-    ensure that some very large outlier samples do not attenuate the majority of the samples.
-
-    Paremeters:
-        max_robust_amplitude (float): maximum amplitude of non-outlier samples of the signal after robust scaling.
-        outlier_percent (float, optional): percentage of the outlier in the data. Defaults to 0.01.
-    Args:
-        data (np.ndarray): input single- or multi-channel signal.
-
-    Returns:
-        np.ndarray: scaled version of the signal.
-    """
-
-    max_robust_amplitude: float = 158e-3
-    outlier_percent: float = 0.01
-
-    def __call__(self, data: np.ndarray) -> np.ndarray:
-        sorted_amplitudes = np.sort(np.abs(data.ravel()))
-
-        robsut_amplitude_index = int(
-            len(sorted_amplitudes) * (1 - self.outlier_percent)
-        )
-        robust_amplitude = sorted_amplitudes[robsut_amplitude_index]
-
-        if robust_amplitude == 0:
-            # input signal consists of just outlier section
-            # then: try to limit the amplitude of the outlier
-            return data / np.max(np.abs(data.ravel())) * self.max_robust_amplitude
-
-        return data / robust_amplitude * self.max_robust_amplitude
-
-
-@dataclass
 class SOSFilter:
     """SOS filter.
 
     Parameters
     ----------
 
     coeffs:
```

### Comparing `tonic-1.4.4.dev34/tonic/cached_dataset.py` & `tonic-1.4.4.dev4/tonic/cached_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 import logging
 import os
-import sys
-
-if sys.version_info >= (3, 8):
-    from typing import Callable, Iterable, Optional, Tuple, TypedDict, Union
-else:
-    from typing import Callable, Iterable, Optional, Tuple, Union
-    from typing_extensions import TypedDict
-
-import random
 import shutil
 from dataclasses import dataclass, field
 from pathlib import Path
+from typing import Callable, Iterable, Optional, Tuple, Union
 from warnings import warn
 
 import h5py
 import numpy as np
 
 
 @dataclass
@@ -231,91 +223,14 @@
     if len(data_list) == 1:
         data_list = data_list[0]
     if len(target_list) == 1:
         target_list = target_list[0]
     return data_list, target_list
 
 
-@dataclass
-class Aug_DiskCachedDataset(DiskCachedDataset):
-    """Aug_DiskCachedDataset is a child class from DiskCachedDataset with further customizations to
-    handle augmented copies of a sample. The goal of this customization is to map the indices of
-    cached files (copy) to augmentation parameters. This is useful in a category of augmentations
-    where the range of parameter is rather disceret and non probabilistic, for instance an audio
-    sample is being augmented with noise and SNR can take only N=5 values. Passing copy_index to
-    augmentation Class as an init argument ensures that each copy will be a a distinct augmented
-    sample with a trackable parameter.
-
-    'generate_all' method generates all augmented vesions of a sample.
-    'generate_copy' method generates the missing variant (augmented version)
-
-
-
-    Therefore all transforms applied to the dataset are categorized by the keys:  "pre_aug", "augmentations"
-     and "post_aug".
-
-     Args:
-         'all_transforms' is a dictionarty passed to this class containing information about all transforms.
-    """
-
-    all_transforms: Optional[TypedDict] = None
-
-    def __post_init__(self):
-        self.pre_aug = self.all_transforms["pre_aug"]
-        self.aug = self.all_transforms["augmentations"]
-        self.post_aug = self.all_transforms["post_aug"]
-
-    def generate_all(self, item):
-        for copy in range(0, self.num_copies):
-            file_path = os.path.join(self.cache_path, f"{item}_{copy}.hdf5")
-            try:
-                data, targets = load_from_disk_cache(file_path)
-            except (FileNotFoundError, OSError) as _:
-                self.generate_copy(item, copy)
-
-    def generate_copy(self, item, copy):
-        from torchvision.transforms import Compose
-
-        file_path = os.path.join(self.cache_path, f"{item}_{copy}.hdf5")
-        # copy index is passed to augmentation (callable)
-        self.aug[0].aug_index = copy
-        augmentation = self.aug
-        self.dataset.transform = Compose(self.pre_aug + augmentation + self.post_aug)
-        data, targets = self.dataset[item]
-        save_to_disk_cache(data, targets, file_path=file_path, compress=self.compress)
-
-    def __getitem__(self, item) -> Tuple[object, object]:
-        if self.dataset is None and item >= self.n_samples:
-            raise IndexError(f"This dataset only has {self.n_samples} items.")
-
-        copy = random.randint(0, self.num_copies - 1)
-        file_path = os.path.join(self.cache_path, f"{item}_{copy}.hdf5")
-        try:
-            data, targets = load_from_disk_cache(file_path)
-
-        except (FileNotFoundError, OSError) as _:
-            logging.info(
-                f"Data {item}: {file_path} not in cache, generating it now",
-                stacklevel=2,
-            )
-            self.generate_copy(item, copy)
-
-            # format might change during save to hdf5, i.e. tensors -> np arrays
-            # We load the sample here again to keep the output format consistent.
-            data, targets = load_from_disk_cache(file_path)
-
-        if self.transform is not None:
-            data = self.transform(data)
-        if self.target_transform is not None:
-            targets = self.target_transform(targets)
-        if self.transforms is not None:
-            data, targets = self.transforms(data, targets)
-        return data, targets
-
-
 class CachedDataset(DiskCachedDataset):
     """Deprecated class that points to DiskCachedDataset for now but will be removed in a future
     release.
 
     Please use MemoryCachedDataset or DiskCachedDataset in the future.
     """
```

### Comparing `tonic-1.4.4.dev34/tonic/collation.py` & `tonic-1.4.4.dev4/tonic/collation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/dataset.py` & `tonic-1.4.4.dev4/tonic/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/__init__.py` & `tonic-1.4.4.dev4/tonic/datasets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from .ebssa import EBSSA
 from .hsd import SHD, SSC
 from .mvsec import MVSEC
 from .ncaltech101 import NCALTECH101
 from .nmnist import NMNIST
 from .pokerdvs import POKERDVS
 from .s_mnist import SMNIST
-from .threeET_eyetracking import ThreeET_Eyetracking
 from .tum_vie import TUMVIE
 from .visual_place_recognition import VPR
 
 __all__ = [
     "ASLDVS",
     "CIFAR10DVS",
     "DAVISDATA",
@@ -25,12 +24,11 @@
     "MVSEC",
     "NCALTECH101",
     "NMNIST",
     "POKERDVS",
     "SHD",
     "SMNIST",
     "SSC",
-    "ThreeET_Eyetracking",
     "TUMVIE",
     "VPR",
     "DVSLip",
 ]
```

### Comparing `tonic-1.4.4.dev34/tonic/datasets/asl_dvs.py` & `tonic-1.4.4.dev4/tonic/datasets/asl_dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/cifar10dvs.py` & `tonic-1.4.4.dev4/tonic/datasets/cifar10dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/davisdataset.py` & `tonic-1.4.4.dev4/tonic/datasets/davisdataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/dsec.py` & `tonic-1.4.4.dev4/tonic/datasets/dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/dvs_lips.py` & `tonic-1.4.4.dev4/tonic/datasets/dvs_lips.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/dvsgesture.py` & `tonic-1.4.4.dev4/tonic/datasets/dvsgesture.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,29 +82,21 @@
             self.file_md5 = self.test_md5
             self.filename = self.test_filename
             self.folder_name = "ibmGestureTest"
 
         if not self._check_exists():
             self.download()
 
-        self.users = []
-        self.lighting = []
         file_path = os.path.join(self.location_on_system, self.folder_name)
         for path, dirs, files in os.walk(file_path):
-            rel_path = os.path.relpath(path, file_path)
-            if rel_path != ".":
-                user, lighting = rel_path.split("_", 1)
-                user = int(user[4:])
-                dirs.sort()
-                for file in files:
-                    if file.endswith("npy"):
-                        self.data.append(os.path.join(path, file))
-                        self.targets.append(int(file[:-4]))
-                        self.users.append(user)
-                        self.lighting.append(lighting)
+            dirs.sort()
+            for file in files:
+                if file.endswith("npy"):
+                    self.data.append(path + "/" + file)
+                    self.targets.append(int(file[:-4]))
 
     def __getitem__(self, index):
         """
         Returns:
             a tuple of (events, target) where target is the index of the target class.
         """
         events = np.load(self.data[index])
```

### Comparing `tonic-1.4.4.dev34/tonic/datasets/ebssa.py` & `tonic-1.4.4.dev4/tonic/datasets/ebssa.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 from tonic.dataset import Dataset
 from tonic.io import events_struct, make_structured_array
 
 
 class EBSSA(Dataset):
     """`EBSSA <https://www.westernsydney.edu.au/icns/resources/reproducible_research3/publication_support_materials2/space_imaging>`_
 
-    There are six different splits provided in this dataset. The labelled section of the dataset contains 84 recordings and 84 label files. 
-    The unlabelled section of the dataset contains 153 recordings in folders marked "Unlabelled".
-    If the automatic download from Google Drive fails, please download the file manually from https://drive.google.com/uc?id=1lCh2HWvxEzzaBHT5TlPuyUn6XPM5OVWN
-    and put it in a folder called 'EBSSA'. Then point the path to its parent folder. For example, if you put the data file in 'datasets/EBSSA/labelled_ebssa.h5',
-    create the dataset object with 'dataset = tonic.datasets.EBSSA('datasets', split='labelled')'
+    There are six different splits provided in this dataset. The labelled section of the dataset contains 84 recordings and 84 label files. The unlabelled section of the dataset contains 153 recordings in folders marked "Unlabelled".
 
     ::
 
         @article{afshar2020event,
             title={Event-based object detection and tracking for space situational awareness},
             author={Afshar, Saeed and Nicholson, Andrew Peter and Van Schaik, Andre and Cohen, Gregory},
             journal={IEEE Sensors Journal},
```

### Comparing `tonic-1.4.4.dev34/tonic/datasets/hsd.py` & `tonic-1.4.4.dev4/tonic/datasets/hsd.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/mvsec.py` & `tonic-1.4.4.dev4/tonic/datasets/mvsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/ncaltech101.py` & `tonic-1.4.4.dev4/tonic/datasets/ncaltech101.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/nmnist.py` & `tonic-1.4.4.dev4/tonic/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/pokerdvs.py` & `tonic-1.4.4.dev4/tonic/datasets/pokerdvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/s_mnist.py` & `tonic-1.4.4.dev4/tonic/datasets/s_mnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/tum_vie.py` & `tonic-1.4.4.dev4/tonic/datasets/tum_vie.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/datasets/visual_place_recognition.py` & `tonic-1.4.4.dev4/tonic/datasets/visual_place_recognition.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/download_utils.py` & `tonic-1.4.4.dev4/tonic/download_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/__init__.py` & `tonic-1.4.4.dev4/tonic/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/crop.py` & `tonic-1.4.4.dev4/tonic/functional/crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/decimate.py` & `tonic-1.4.4.dev4/tonic/functional/decimate.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/denoise.py` & `tonic-1.4.4.dev4/tonic/functional/denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/drop_event.py` & `tonic-1.4.4.dev4/tonic/functional/drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/drop_pixel.py` & `tonic-1.4.4.dev4/tonic/functional/drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/event_downsampling.py` & `tonic-1.4.4.dev4/tonic/functional/event_downsampling.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/refractory_period.py` & `tonic-1.4.4.dev4/tonic/functional/refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/spatial_jitter.py` & `tonic-1.4.4.dev4/tonic/functional/spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/time_jitter.py` & `tonic-1.4.4.dev4/tonic/functional/time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/time_skew.py` & `tonic-1.4.4.dev4/tonic/functional/time_skew.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/to_averaged_timesurface.py` & `tonic-1.4.4.dev4/tonic/functional/to_averaged_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/to_bina_rep.py` & `tonic-1.4.4.dev4/tonic/functional/to_bina_rep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/to_frame.py` & `tonic-1.4.4.dev4/tonic/functional/to_frame.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/to_timesurface.py` & `tonic-1.4.4.dev4/tonic/functional/to_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/to_voxel_grid.py` & `tonic-1.4.4.dev4/tonic/functional/to_voxel_grid.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/functional/uniform_noise.py` & `tonic-1.4.4.dev4/tonic/functional/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/io.py` & `tonic-1.4.4.dev4/tonic/io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/prototype/README.md` & `tonic-1.4.4.dev4/tonic/prototype/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/prototype/datasets/ncars.py` & `tonic-1.4.4.dev4/tonic/prototype/datasets/ncars.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/prototype/datasets/nmnist.py` & `tonic-1.4.4.dev4/tonic/prototype/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/prototype/datasets/prophesee.py` & `tonic-1.4.4.dev4/tonic/prototype/datasets/prophesee.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/prototype/datasets/stmnist.py` & `tonic-1.4.4.dev4/tonic/prototype/datasets/stmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/prototype/datasets/utils/_dataset.py` & `tonic-1.4.4.dev4/tonic/prototype/datasets/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/prototype/datasets/utils/_utils.py` & `tonic-1.4.4.dev4/tonic/prototype/datasets/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/prototype/slicers.py` & `tonic-1.4.4.dev4/tonic/prototype/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/sliced_dataset.py` & `tonic-1.4.4.dev4/tonic/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/slicers.py` & `tonic-1.4.4.dev4/tonic/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/transforms.py` & `tonic-1.4.4.dev4/tonic/transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic/utils.py` & `tonic-1.4.4.dev4/tonic/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic-logo-padded.png` & `tonic-1.4.4.dev4/tonic-logo-padded.png`

 * *Files identical despite different names*

### Comparing `tonic-1.4.4.dev34/tonic.egg-info/PKG-INFO` & `tonic-1.4.4.dev4/tonic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.4.4.dev34
+Version: 1.4.4.dev4
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.4.4.dev34/tonic.egg-info/SOURCES.txt` & `tonic-1.4.4.dev4/tonic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -73,48 +73,42 @@
 docs/how-tos/visualizing-data.ipynb
 docs/how-tos/wrapping_own_data.ipynb
 docs/reading_material/design_choices.rst
 docs/reading_material/intro-event-cameras.rst
 docs/reading_material/intro-snns.rst
 docs/reading_material/reading_material.rst
 docs/reading_material/training-snns.rst
-docs/tutorials/Aug_DiskCachDataset.ipynb
-docs/tutorials/audio_transforms_tutorial.ipynb
 docs/tutorials/batching.ipynb
 docs/tutorials/davis_data.ipynb
 docs/tutorials/fast_dataloading.ipynb
 docs/tutorials/large_datasets.ipynb
 docs/tutorials/slicing.ipynb
 docs/tutorials/tutorials.rst
 test/dataset_utils.py
 test/prototype_dataset_utils.py
 test/requirements.txt
-test/test_audio_augmentations.py
 test/test_audio_transforms.py
-test/test_aug_caching.py
 test/test_caching.py
 test/test_chained_transforms.py
 test/test_datasets.py
 test/test_dsec.py
 test/test_io.py
 test/test_prototype_datasets.py
 test/test_representations.py
 test/test_sliced_dataset.py
 test/test_slicers.py
 test/test_tonic_utils.py
 test/test_transforms.py
-test/torch_requirements.txt
 test/utils.py
 test/test_data/sample.aedat4
 test/test_data/sample_aedat_header.aedat
 test/test_data/sample_ncars.dat
 test/test_data/sample_nmnist.bin
 test/test_data/sample_stmnist.mat
 tonic/__init__.py
-tonic/audio_augmentations.py
 tonic/audio_transforms.py
 tonic/cached_dataset.py
 tonic/collation.py
 tonic/dataset.py
 tonic/download_utils.py
 tonic/io.py
 tonic/sliced_dataset.py
@@ -138,15 +132,14 @@
 tonic/datasets/ebssa.py
 tonic/datasets/hsd.py
 tonic/datasets/mvsec.py
 tonic/datasets/ncaltech101.py
 tonic/datasets/nmnist.py
 tonic/datasets/pokerdvs.py
 tonic/datasets/s_mnist.py
-tonic/datasets/threeET_eyetracking.py
 tonic/datasets/tum_vie.py
 tonic/datasets/visual_place_recognition.py
 tonic/functional/__init__.py
 tonic/functional/crop.py
 tonic/functional/decimate.py
 tonic/functional/denoise.py
 tonic/functional/drop_event.py
```

