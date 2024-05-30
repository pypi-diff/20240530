# Comparing `tmp/ecuapassdocs-0.80.tar.gz` & `tmp/ecuapassdocs-0.801.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecuapassdocs-0.80.tar", last modified: Wed May 22 18:02:16 2024, max compression
+gzip compressed data, was "ecuapassdocs-0.801.tar", last modified: Thu May 30 14:38:11 2024, max compression
```

## Comparing `ecuapassdocs-0.80.tar` & `ecuapassdocs-0.801.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.749927 ecuapassdocs-0.80/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-22 18:02:16.749927 ecuapassdocs-0.80/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)      144 2024-05-18 12:09:20.000000 ecuapassdocs-0.80/README.md
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.717928 ecuapassdocs-0.80/ecuapassdocs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.725928 ecuapassdocs-0.80/ecuapassdocs/info/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     3416 2024-05-16 12:39:30.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_data.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18205 2024-05-20 18:19:53.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_extractor.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4638 2024-05-18 12:32:53.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_feedback.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9720 2024-05-20 18:17:08.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    19650 2024-05-19 22:14:26.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1521 2024-05-12 16:16:09.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2732 2024-05-04 03:37:00.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_declaracion.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    24020 2024-05-13 19:40:43.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2187 2024-05-10 22:50:32.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2065 2024-05-13 22:36:59.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    13890 2024-05-20 12:55:05.000000 ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.80/ecuapassdocs/info/resourceloader.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.725928 ecuapassdocs-0.80/ecuapassdocs/resources/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.729928 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      623 2024-05-14 16:35:53.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/documentos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/empresa.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/monedas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/out.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/sustancias.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.729928 ecuapassdocs-0.80/ecuapassdocs/resources/data_declaracion/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_declaracion/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.737928 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/sectores.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.741928 ecuapassdocs-0.80/ecuapassdocs/resources/docs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    15818 2024-05-16 12:20:48.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    18780 2024-05-12 00:44:17.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.80/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.749927 ecuapassdocs-0.80/ecuapassdocs/resources/images/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)   218079 2024-05-22 13:19:12.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/cartaporte-DUMMY.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-colombia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-ecuador.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-white-bot.ico
--rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-cartaporte-vacia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-scroll-up.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image-windows-WindowButtons.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    23824 2024-05-22 13:29:05.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/image_DUMMY.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   267971 2024-05-22 13:19:51.000000 ecuapassdocs-0.80/ecuapassdocs/resources/images/manifiesto_DUMMY.png
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-22 18:02:16.721928 ecuapassdocs-0.80/ecuapassdocs.egg-info/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)     5870 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/requires.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-05-22 18:02:16.000000 ecuapassdocs-0.80/ecuapassdocs.egg-info/top_level.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-05-22 18:02:16.749927 ecuapassdocs-0.80/setup.cfg
--rw-rw-r--   0 lg        (1000) lg        (1000)     1700 2024-05-22 18:02:14.000000 ecuapassdocs-0.80/setup.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.148779 ecuapassdocs-0.801/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      349 2024-05-30 14:38:11.148779 ecuapassdocs-0.801/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)      212 2024-05-30 14:37:43.000000 ecuapassdocs-0.801/README.md
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.024784 ecuapassdocs-0.801/ecuapassdocs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.036784 ecuapassdocs-0.801/ecuapassdocs/info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.801/ecuapassdocs/info/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3415 2024-05-30 10:38:07.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_data.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18322 2024-05-30 14:22:48.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_extractor.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4638 2024-05-18 12:32:53.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_feedback.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9554 2024-05-30 14:23:20.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    19651 2024-05-30 10:49:03.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1521 2024-05-12 16:16:09.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2732 2024-05-04 03:37:00.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_declaracion.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    24020 2024-05-13 19:40:43.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2187 2024-05-10 22:50:32.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2065 2024-05-13 22:36:59.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    13890 2024-05-20 12:55:05.000000 ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.801/ecuapassdocs/info/resourceloader.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.036784 ecuapassdocs-0.801/ecuapassdocs/resources/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.056783 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      623 2024-05-14 16:35:53.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/documentos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/empresa.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/monedas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/out.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/sustancias.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.060783 ecuapassdocs-0.801/ecuapassdocs/resources/data_declaracion/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_declaracion/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.088782 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/sectores.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.112780 ecuapassdocs-0.801/ecuapassdocs/resources/docs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    15818 2024-05-16 12:20:48.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18780 2024-05-12 00:44:17.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.801/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.144779 ecuapassdocs-0.801/ecuapassdocs/resources/images/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)   218079 2024-05-22 13:19:12.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/cartaporte-DUMMY.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/icon-colombia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/icon-ecuador.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/icon-white-bot.ico
+-rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-cartaporte-vacia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-scroll-up.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image-windows-WindowButtons.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    23824 2024-05-22 13:29:05.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/image_DUMMY.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   267971 2024-05-22 13:19:51.000000 ecuapassdocs-0.801/ecuapassdocs/resources/images/manifiesto_DUMMY.png
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-30 14:38:11.028784 ecuapassdocs-0.801/ecuapassdocs.egg-info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      349 2024-05-30 14:38:10.000000 ecuapassdocs-0.801/ecuapassdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)     5870 2024-05-30 14:38:10.000000 ecuapassdocs-0.801/ecuapassdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-05-30 14:38:10.000000 ecuapassdocs-0.801/ecuapassdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-05-30 14:38:10.000000 ecuapassdocs-0.801/ecuapassdocs.egg-info/requires.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-05-30 14:38:10.000000 ecuapassdocs-0.801/ecuapassdocs.egg-info/top_level.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-05-30 14:38:11.148779 ecuapassdocs-0.801/setup.cfg
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1731 2024-05-30 14:37:25.000000 ecuapassdocs-0.801/setup.py
```

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_data.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 			"direccion": "Carrera 42 No 75-63 Aut. Sur, Itagui (Antioquia)",
 			"idTipo" : "NIT", 
 			"idNumero" : "890.901.321-5",
 			"modelCartaportes": "Model_Cartaportes_Botero",
 			"modelManifiestos": "Model_Manifiestos_Botero",
 			"modelDeclaraciones": None,
 			"MRN": None,
-			"MSN": None,
+			"MSN": None
 		},
 		"NTA" : { 
 			'id'     : "NTA",
 			"nombre" : "NUEVO TRANSPORTE DE AMERICA COMPAÑIA LIMITADA", 
 			"direccion": "ARGENTINA Y JUAN LEON MERA - TULCAN",
 			"idTipo" : "RUC", 
 			"idNumero" : "1791834461001",
```

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_extractor.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,26 +338,31 @@
 	def getTipoEmbalaje (text, resourcesPath):
 		Utils.printx (f">>> Extrayendo embalaje desde el texto: '{text}'")
 		try:
 			reNumber   = r'\d+(?:[.,]*\d*)+' # RE for extracting a float number 
 			reEmbalaje = rf"{reNumber}\s+(\b(\w+)\b)"    # String after number
 			embalaje   = Extractor.getValueRE (reEmbalaje, text) 
 
-			if "PALLET" in embalaje or "ESTIBA":
-				return "152" # "[152] PALETAS"
-			elif "SACO" in embalaje.upper ():
-				return "104" # "[104] SACO"
-			elif "CAJA" in embalaje.upper ():
-				return "035" # "[035] CAJA"
-			else:
-				return embalaje.strip () + "||LOW"
+			codeEmbalaje = Extractor.getCodeEmbalaje (embalaje)
+
+			return codeEmbalaje
 		except:
 			Utils.printx (f"Problemas extrayendo embalaje desde texto: '{text}'")
 			return None
 
+	def getCodeEmbalaje (embalaje):
+		if "PALLET" in embalaje or "ESTIBA" in embalaje:
+			return "152" # "[152] PALETAS"
+		elif "SACO" in embalaje.upper ():
+			return "104" # "[104] SACO"
+		elif "CAJA" in embalaje.upper ():
+			return "035" # "[035] CAJA"
+		else:
+			return embalaje.strip () + "||LOW"
+
 	#------------------------------------------------------------------
 	#-- Extract numerical or text date from text ----------------------
 	#------------------------------------------------------------------
 	def getDate (text, resourcesPath):
 		numericalDate = "||LOW"
 		try:
 			# Load months from data file
```

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_feedback.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_feedback.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,23 +45,15 @@
 
 			# Vehiculo
 			if "Tipo_Vehiculo" in key:
 				vehiculos    = {"SEMIRREMOLQUE":"SR", "TRACTOCAMION":"TC", "CAMION":"CA"}
 				ecuapassFields [key] = vehiculos [ecuapassFields[key]]
 
 			# Embalaje
-			if "Embalaje" in key: 
-				embalaje = ecuapassFields [key].upper()
-				if "PALLET" in embalaje:
-					embalaje = "152" # "[152] PALETAS"
-				elif "SACO" in embalaje:
-					embalaje = "104" # "[104] SACO"
-				elif "CAJA" in embalaje:
-					embalaje = "035" # "[035] CAJA"
-				ecuapassFields [key] = embalaje
+			ecuapassFields [key] = Extractor.getCodeEmbalaje (embalaje)
 
 			# Moneda
 			if "Moneda" in key:
 				ecuapassFields [key] = "USD"
 
 			# Remove confidence string ("||LOW")
 			value        = ecuapassFields [key] 
@@ -95,14 +87,18 @@
 	def getDocFields (self):
 		return self.fields
 
 	#-- Get id (short name)
 	def getIdEmpresa (self):
 		return self.empresa ["id"]
 
+	def getIdNumeroEmpresa (self):
+		id = self.empresa ["idNumero"]
+		return id
+
 	#-- Get data and value from document main fields"""
 	def getNombreEmpresa (self):
 		return self.empresa ["nombre"]
 
 	def getDireccionEmpresa (self):
 		return self.empresa ["direccion"]
```

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 			self.ecudoc ["04_MSN"]               = self.getMSN () 
 			self.ecudoc ["05_TipoProcedimiento"] = self.getTipoProcedimiento ()
 
 			#-- Empresa
 			self.ecudoc ["06_EmpresaTransporte"] = self.getNombreEmpresa ()
 			self.ecudoc ["07_DepositoMercancia"] = self.getDepositoMercancia ()
 			self.ecudoc ["08_DirTransportista"]	 = self.getDireccionEmpresa ()
-			self.ecudoc ["09_NroIdentificacion"] = self.getIdEmpresa ()
+			self.ecudoc ["09_NroIdentificacion"] = self.getIdNumeroEmpresa ()
 
 			#--------------------------------------------------------------
 			# print ("\n>>>>>> Datos Generales de la CPIC: Sujetos <<<<<<<<")
 			#--------------------------------------------------------------
 			#-- Remitente 
 			remitente                             = Utils.checkLow (self.getSubjectInfo ("02_Remitente"))
 			self.ecudoc ["10_PaisRemitente"]      = remitente ["pais"]
@@ -199,17 +199,14 @@
 
 	def getNombreEmpresa (self):
 		return self.empresa ["nombre"]
 
 	def getDireccionEmpresa (self):
 		return self.empresa ["direccion"]
 
-	def getIdEmpresa (self):
-		id = self.empresa ["idNumero"]
-		return id
 	#------------------------------------------------------------
 	# Return the code number from the text matching a "deposito"
 	#-- BOTERO-SOTO en casilla 21 o 22, NTA en la 22 ------------
 	#------------------------------------------------------------
 	def getDepositoMercancia (self):
 		for casilla in ["21_Instrucciones", "22_Observaciones"]:
 			text = ""
@@ -242,25 +239,27 @@
 		location = Extractor.extractLocationDate (text, self.resourcesPath, key)
 		return (location)
 
 	#-----------------------------------------------------------
 	# Get "Entrega" location and suggest a date if it is None
 	#-----------------------------------------------------------
 	def getEntregaLocation (self, key):
+		idEmpresa = self.getIdEmpresa ()
 		location = self.getLocationInfo (key)
-		print ("++ location:", location)
 		try:
 			# Add a week to 'entrega' from 'embarque' date
 			if location ["fecha"] == "||LOW" or location ["fecha"] is None:
 				fechaEmbarque      = self.ecudoc ["34_FechaEmbarque"]
 				date_obj           = datetime.strptime (fechaEmbarque, "%d-%m-%Y")
-				new_date_obj       = date_obj  # Fecha actual
+				new_date_obj       = date_obj  # Fecha igual a la de Embarque
 
-				if "BYZA" in self.getNombreEmpresa().upper():
+				if "BYZA" in idEmpresa:
 					new_date_obj       = date_obj + timedelta(weeks=2)   # 15 días
+				elif "NTA" in idEmpresa:
+					new_date_obj       = datetime.today()
 
 				location ["fecha"] = new_date_obj.strftime("%d-%m-%Y") + "||LOW"
 		except:
 			Utils.printException ("Obteniendo información de 'entrega'")
 
 		return location
 	#-----------------------------------------------------------
```

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_declaracion.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_declaracion.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/ecuapass_utils.py` & `ecuapassdocs-0.801/ecuapassdocs/info/ecuapass_utils.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/info/resourceloader.py` & `ecuapassdocs-0.801/ecuapassdocs/info/resourceloader.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/out.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/out.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/paises_todos.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/paises_todos.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/sustancias.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/sustancias.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/cartaporte_input_parameters.json` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/cartaporte_input_parameters.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/manifiesto_input_parameters.json` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/manifiesto_input_parameters.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.801/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/cartaporte-DUMMY.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/cartaporte-DUMMY.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-colombia.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/icon-colombia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-ecuador.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/icon-ecuador.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/icon-white-bot.ico` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/icon-white-bot.ico`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-cartaporte-vacia.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image-cartaporte-vacia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-declaracion-ecuapass.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image-declaracion-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/image_DUMMY.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/image_DUMMY.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs/resources/images/manifiesto_DUMMY.png` & `ecuapassdocs-0.801/ecuapassdocs/resources/images/manifiesto_DUMMY.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/ecuapassdocs.egg-info/SOURCES.txt` & `ecuapassdocs-0.801/ecuapassdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.80/setup.py` & `ecuapassdocs-0.801/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ecuapassdocs',  # Package name
-    version='0.80',  # Package version
+    version='0.801',  # Package version
     url="https://github.com/lgarreta/ecuapassdocs",
     author='Luis Garreta',
     author_email='lgarreta@gmail.com',
     description='Utils for creating PDFs, loading resources and extracting info from fields in ECUAPASS docs: cartaportes, manifiestos, declaraciones',
     packages=find_packages(),  # Automatically finds packages within the directory
 	include_package_data=True, 
 	package_data={"ecuapassdocs": ["resources/images/*", 
@@ -17,15 +17,15 @@
 	# List any dependencies here
     install_requires = [
 		"PyPDF2==3.0.1",
 		"reportlab==4.0.8",
 		"Pillow==10.1.0"
 	], 
 	logs = {
-		"0.80"   : "Improved info:embalaje",
+		"0.801"  : "30-Mayo : Fixed info: 'embalaje' and 'fecha entrega'",
 		"0.79"   : "Search codebin form by NAME. Added settings for NTA",
 		"0.78"   : "Improved infos:depositos, dates, vehiculo",
 		"0.77"   : "Improved update (posprocessing) ECUAPASS file",
 		"0.76"   : "Improved Utils, getCodebinValues",
 		"0.75"   : "Simplified info classes (e.g. removed Gastos table)",
 		"0.74"   : "Changed tipoProc (Byza === NTA)",
 		"0.73"   : "Improved Byza's clean watermarks",
```

