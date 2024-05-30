# Comparing `tmp/pmdsky_debug_py-9.0.8-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-9.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 1106339 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 24-Jan-02 04:25 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 24-Jan-02 04:25 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   937244 b- defN 24-Jan-02 04:25 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   889624 b- defN 24-Jan-02 04:25 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   921986 b- defN 24-Jan-02 04:25 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   889614 b- defN 24-Jan-02 04:25 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   938456 b- defN 24-Jan-02 04:25 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   889644 b- defN 24-Jan-02 04:25 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   306661 b- defN 24-Jan-02 04:25 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-02 04:25 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1372 b- defN 24-Jan-02 04:25 pmdsky_debug_py-9.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-02 04:25 pmdsky_debug_py-9.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Jan-02 04:25 pmdsky_debug_py-9.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 24-Jan-02 04:25 pmdsky_debug_py-9.0.8.dist-info/RECORD
-14 files, 5777725 bytes uncompressed, 1104441 bytes compressed:  80.9%
+Zip file size: 1106384 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 24-Jan-04 04:25 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 24-Jan-04 04:25 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   937268 b- defN 24-Jan-04 04:25 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   889648 b- defN 24-Jan-04 04:25 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   922010 b- defN 24-Jan-04 04:25 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   889638 b- defN 24-Jan-04 04:25 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   938480 b- defN 24-Jan-04 04:25 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   889668 b- defN 24-Jan-04 04:25 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   306685 b- defN 24-Jan-04 04:25 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-04 04:25 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1372 b- defN 24-Jan-04 04:26 pmdsky_debug_py-9.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jan-04 04:26 pmdsky_debug_py-9.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Jan-04 04:26 pmdsky_debug_py-9.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 24-Jan-04 04:26 pmdsky_debug_py-9.0.9.dist-info/RECORD
+14 files, 5777893 bytes uncompressed, 1104486 bytes compressed:  80.9%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-9.0.8.dist-info/METADATA
+Filename: pmdsky_debug_py-9.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-9.0.8.dist-info/WHEEL
+Filename: pmdsky_debug_py-9.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-9.0.8.dist-info/top_level.txt
+Filename: pmdsky_debug_py-9.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-9.0.8.dist-info/RECORD
+Filename: pmdsky_debug_py-9.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.9.0+d59bb9ac22"
+RELEASE = "v0.9.0+7a1a2ed617"
```

## pmdsky_debug_py/eu.py

```diff
@@ -9954,15 +9954,15 @@
     length = 0x4000
     functions = EuItcmFunctions
     data = EuItcmData
 
 
 class EuLibsFunctions:
 
-    SoundUtilGetRandomNumber = Symbol(
+    SoundUtil_GetRandomNumber = Symbol(
         [0x81C], [0x206CC8C], None, "return: random number in the range [0, 32767]"
     )
 
     ReadWaviEntry = Symbol(
         [0x1480],
         [0x206D8F0],
         None,
@@ -10018,34 +10018,34 @@
         [0x83B4],
         [0x2074824],
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/"
         " and Irdkwia's notes.\n\nNo params.",
     )
 
-    SoundEnvelopeReset = Symbol(
+    SoundEnvelope_Reset = Symbol(
         [0x8B98], [0x2075008], None, "r0: Sound envelope pointer"
     )
 
-    SoundEnvelopeParametersReset = Symbol(
+    SoundEnvelopeParameters_Reset = Symbol(
         [0x8BAC], [0x207501C], None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeParametersCheckValidity = Symbol(
+    SoundEnvelopeParameters_CheckValidity = Symbol(
         [0x8BC8], [0x2075038], None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeSetParameters = Symbol(
+    SoundEnvelope_SetParameters = Symbol(
         [0x8C1C],
         [0x207508C],
         None,
         "r0: Sound envelope pointer\nr1: Sound envelope parameters pointer",
     )
 
-    SoundEnvelopeSetSlide = Symbol(
+    SoundEnvelope_SetSlide = Symbol(
         [0x8C80],
         [0x20750F0],
         None,
         "r0: Sound envelope pointer\nr1: Target volume\nr2: Music duration lookup table"
         " index",
     )
 
@@ -10053,90 +10053,90 @@
         [0x8D34],
         [0x20751A4],
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/\n\nr0:"
         " Sound envelope pointer",
     )
 
-    SoundEnvelopeRelease = Symbol(
+    SoundEnvelope_Release = Symbol(
         [0x8E00], [0x2075270], None, "r0: Sound envelope pointer"
     )
 
-    SoundEnvelopeStop = Symbol(
+    SoundEnvelope_Stop = Symbol(
         [0x8E2C], [0x207529C], None, "r0: Sound envelope pointer"
     )
 
-    SoundEnvelopeForceVolume = Symbol(
+    SoundEnvelope_ForceVolume = Symbol(
         [0x8E44], [0x20752B4], None, "r0: Sound envelope pointer\nr1: Volume"
     )
 
-    SoundEnvelopeStop2 = Symbol(
+    SoundEnvelope_Stop2 = Symbol(
         [0x8E64], [0x20752D4], None, "r0: Sound envelope pointer"
     )
 
-    SoundEnvelopeTick = Symbol(
+    SoundEnvelope_Tick = Symbol(
         [0x8E7C],
         [0x20752EC],
         None,
         "r0: Sound envelope pointer\nreturn: Current volume",
     )
 
-    SoundLfoBankReset = Symbol([0x8FC4], [0x2075434], None, "r0: LFO bank pointer")
+    SoundLfoBank_Reset = Symbol([0x8FC4], [0x2075434], None, "r0: LFO bank pointer")
 
-    SoundLfoBankSet = Symbol(
+    SoundLfoBank_Set = Symbol(
         [0x8FDC],
         [0x207544C],
         None,
         "r0: LFO bank pointer\nr1: LFO settings pointer\nr2: Envelope level",
     )
 
-    SoundLfoBankSetConstEnvelopes = Symbol(
+    SoundLfoBank_SetConstEnvelopes = Symbol(
         [0x91D4], [0x2075644], None, "r0: LFO bank pointer\nr1: Level"
     )
 
-    SoundLfoBankTick = Symbol(
+    SoundLfoBank_Tick = Symbol(
         [0x9220],
         [0x2075690],
         None,
         "r0: LFO bank pointer\nreturn: New voice update flags",
     )
 
-    SoundLfoWaveInvalidFunc = Symbol(
+    SoundLfoWave_InvalidFunc = Symbol(
         [0x92D4], [0x2075744], None, "r0: LFO pointer\nreturn: 0"
     )
 
-    SoundLfoWaveHalfSquareFunc = Symbol(
+    SoundLfoWave_HalfSquareFunc = Symbol(
         [0x92E8], [0x2075758], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullSquareFunc = Symbol(
+    SoundLfoWave_FullSquareFunc = Symbol(
         [0x9324], [0x2075794], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfTriangleFunc = Symbol(
+    SoundLfoWave_HalfTriangleFunc = Symbol(
         [0x936C], [0x20757DC], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullTriangleFunc = Symbol(
+    SoundLfoWave_FullTriangleFunc = Symbol(
         [0x93C0], [0x2075830], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveSawFunc = Symbol(
+    SoundLfoWave_SawFunc = Symbol(
         [0x9424], [0x2075894], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveReverseSawFunc = Symbol(
+    SoundLfoWave_ReverseSawFunc = Symbol(
         [0x9460], [0x20758D0], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfNoiseFunc = Symbol(
+    SoundLfoWave_HalfNoiseFunc = Symbol(
         [0x949C], [0x207590C], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullNoiseFunc = Symbol(
+    SoundLfoWave_FullNoiseFunc = Symbol(
         [0x94E0], [0x2075950], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
     Crypto_RC4Init = Symbol([0x9648], [0x2075AB8], None, "")
 
     Mtx_LookAt = Symbol([0x9750], [0x2075BC0], None, "")
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -9723,15 +9723,15 @@
     length = 0x4000
     functions = EuItcmItcmFunctions
     data = EuItcmItcmData
 
 
 class EuItcmLibsFunctions:
 
-    SoundUtilGetRandomNumber = Symbol(
+    SoundUtil_GetRandomNumber = Symbol(
         None, None, None, "return: random number in the range [0, 32767]"
     )
 
     ReadWaviEntry = Symbol(
         None,
         None,
         None,
@@ -9784,32 +9784,32 @@
         None,
         None,
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/"
         " and Irdkwia's notes.\n\nNo params.",
     )
 
-    SoundEnvelopeReset = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Reset = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeParametersReset = Symbol(
+    SoundEnvelopeParameters_Reset = Symbol(
         None, None, None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeParametersCheckValidity = Symbol(
+    SoundEnvelopeParameters_CheckValidity = Symbol(
         None, None, None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeSetParameters = Symbol(
+    SoundEnvelope_SetParameters = Symbol(
         None,
         None,
         None,
         "r0: Sound envelope pointer\nr1: Sound envelope parameters pointer",
     )
 
-    SoundEnvelopeSetSlide = Symbol(
+    SoundEnvelope_SetSlide = Symbol(
         None,
         None,
         None,
         "r0: Sound envelope pointer\nr1: Target volume\nr2: Music duration lookup table"
         " index",
     )
 
@@ -9817,76 +9817,76 @@
         None,
         None,
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/\n\nr0:"
         " Sound envelope pointer",
     )
 
-    SoundEnvelopeRelease = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Release = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeStop = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Stop = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeForceVolume = Symbol(
+    SoundEnvelope_ForceVolume = Symbol(
         None, None, None, "r0: Sound envelope pointer\nr1: Volume"
     )
 
-    SoundEnvelopeStop2 = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Stop2 = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeTick = Symbol(
+    SoundEnvelope_Tick = Symbol(
         None, None, None, "r0: Sound envelope pointer\nreturn: Current volume"
     )
 
-    SoundLfoBankReset = Symbol(None, None, None, "r0: LFO bank pointer")
+    SoundLfoBank_Reset = Symbol(None, None, None, "r0: LFO bank pointer")
 
-    SoundLfoBankSet = Symbol(
+    SoundLfoBank_Set = Symbol(
         None,
         None,
         None,
         "r0: LFO bank pointer\nr1: LFO settings pointer\nr2: Envelope level",
     )
 
-    SoundLfoBankSetConstEnvelopes = Symbol(
+    SoundLfoBank_SetConstEnvelopes = Symbol(
         None, None, None, "r0: LFO bank pointer\nr1: Level"
     )
 
-    SoundLfoBankTick = Symbol(
+    SoundLfoBank_Tick = Symbol(
         None, None, None, "r0: LFO bank pointer\nreturn: New voice update flags"
     )
 
-    SoundLfoWaveInvalidFunc = Symbol(None, None, None, "r0: LFO pointer\nreturn: 0")
+    SoundLfoWave_InvalidFunc = Symbol(None, None, None, "r0: LFO pointer\nreturn: 0")
 
-    SoundLfoWaveHalfSquareFunc = Symbol(
+    SoundLfoWave_HalfSquareFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullSquareFunc = Symbol(
+    SoundLfoWave_FullSquareFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfTriangleFunc = Symbol(
+    SoundLfoWave_HalfTriangleFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullTriangleFunc = Symbol(
+    SoundLfoWave_FullTriangleFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveSawFunc = Symbol(
+    SoundLfoWave_SawFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveReverseSawFunc = Symbol(
+    SoundLfoWave_ReverseSawFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfNoiseFunc = Symbol(
+    SoundLfoWave_HalfNoiseFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullNoiseFunc = Symbol(
+    SoundLfoWave_FullNoiseFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
     Crypto_RC4Init = Symbol(None, None, None, "")
 
     Mtx_LookAt = Symbol(None, None, None, "")
```

## pmdsky_debug_py/jp.py

```diff
@@ -9942,15 +9942,15 @@
     length = 0x4060
     functions = JpItcmFunctions
     data = JpItcmData
 
 
 class JpLibsFunctions:
 
-    SoundUtilGetRandomNumber = Symbol(
+    SoundUtil_GetRandomNumber = Symbol(
         None, None, None, "return: random number in the range [0, 32767]"
     )
 
     ReadWaviEntry = Symbol(
         [0x1480],
         [0x206D840],
         None,
@@ -10006,32 +10006,32 @@
         [0x83B4],
         [0x2074774],
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/"
         " and Irdkwia's notes.\n\nNo params.",
     )
 
-    SoundEnvelopeReset = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Reset = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeParametersReset = Symbol(
+    SoundEnvelopeParameters_Reset = Symbol(
         None, None, None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeParametersCheckValidity = Symbol(
+    SoundEnvelopeParameters_CheckValidity = Symbol(
         None, None, None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeSetParameters = Symbol(
+    SoundEnvelope_SetParameters = Symbol(
         None,
         None,
         None,
         "r0: Sound envelope pointer\nr1: Sound envelope parameters pointer",
     )
 
-    SoundEnvelopeSetSlide = Symbol(
+    SoundEnvelope_SetSlide = Symbol(
         None,
         None,
         None,
         "r0: Sound envelope pointer\nr1: Target volume\nr2: Music duration lookup table"
         " index",
     )
 
@@ -10039,76 +10039,76 @@
         [0x8D34],
         [0x20750F4],
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/\n\nr0:"
         " Sound envelope pointer",
     )
 
-    SoundEnvelopeRelease = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Release = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeStop = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Stop = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeForceVolume = Symbol(
+    SoundEnvelope_ForceVolume = Symbol(
         None, None, None, "r0: Sound envelope pointer\nr1: Volume"
     )
 
-    SoundEnvelopeStop2 = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Stop2 = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeTick = Symbol(
+    SoundEnvelope_Tick = Symbol(
         None, None, None, "r0: Sound envelope pointer\nreturn: Current volume"
     )
 
-    SoundLfoBankReset = Symbol(None, None, None, "r0: LFO bank pointer")
+    SoundLfoBank_Reset = Symbol(None, None, None, "r0: LFO bank pointer")
 
-    SoundLfoBankSet = Symbol(
+    SoundLfoBank_Set = Symbol(
         None,
         None,
         None,
         "r0: LFO bank pointer\nr1: LFO settings pointer\nr2: Envelope level",
     )
 
-    SoundLfoBankSetConstEnvelopes = Symbol(
+    SoundLfoBank_SetConstEnvelopes = Symbol(
         None, None, None, "r0: LFO bank pointer\nr1: Level"
     )
 
-    SoundLfoBankTick = Symbol(
+    SoundLfoBank_Tick = Symbol(
         None, None, None, "r0: LFO bank pointer\nreturn: New voice update flags"
     )
 
-    SoundLfoWaveInvalidFunc = Symbol(None, None, None, "r0: LFO pointer\nreturn: 0")
+    SoundLfoWave_InvalidFunc = Symbol(None, None, None, "r0: LFO pointer\nreturn: 0")
 
-    SoundLfoWaveHalfSquareFunc = Symbol(
+    SoundLfoWave_HalfSquareFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullSquareFunc = Symbol(
+    SoundLfoWave_FullSquareFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfTriangleFunc = Symbol(
+    SoundLfoWave_HalfTriangleFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullTriangleFunc = Symbol(
+    SoundLfoWave_FullTriangleFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveSawFunc = Symbol(
+    SoundLfoWave_SawFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveReverseSawFunc = Symbol(
+    SoundLfoWave_ReverseSawFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfNoiseFunc = Symbol(
+    SoundLfoWave_HalfNoiseFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullNoiseFunc = Symbol(
+    SoundLfoWave_FullNoiseFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
     Crypto_RC4Init = Symbol(None, None, None, "")
 
     Mtx_LookAt = Symbol(None, None, None, "")
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -9723,15 +9723,15 @@
     length = 0x4060
     functions = JpItcmItcmFunctions
     data = JpItcmItcmData
 
 
 class JpItcmLibsFunctions:
 
-    SoundUtilGetRandomNumber = Symbol(
+    SoundUtil_GetRandomNumber = Symbol(
         None, None, None, "return: random number in the range [0, 32767]"
     )
 
     ReadWaviEntry = Symbol(
         None,
         None,
         None,
@@ -9784,32 +9784,32 @@
         None,
         None,
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/"
         " and Irdkwia's notes.\n\nNo params.",
     )
 
-    SoundEnvelopeReset = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Reset = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeParametersReset = Symbol(
+    SoundEnvelopeParameters_Reset = Symbol(
         None, None, None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeParametersCheckValidity = Symbol(
+    SoundEnvelopeParameters_CheckValidity = Symbol(
         None, None, None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeSetParameters = Symbol(
+    SoundEnvelope_SetParameters = Symbol(
         None,
         None,
         None,
         "r0: Sound envelope pointer\nr1: Sound envelope parameters pointer",
     )
 
-    SoundEnvelopeSetSlide = Symbol(
+    SoundEnvelope_SetSlide = Symbol(
         None,
         None,
         None,
         "r0: Sound envelope pointer\nr1: Target volume\nr2: Music duration lookup table"
         " index",
     )
 
@@ -9817,76 +9817,76 @@
         None,
         None,
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/\n\nr0:"
         " Sound envelope pointer",
     )
 
-    SoundEnvelopeRelease = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Release = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeStop = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Stop = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeForceVolume = Symbol(
+    SoundEnvelope_ForceVolume = Symbol(
         None, None, None, "r0: Sound envelope pointer\nr1: Volume"
     )
 
-    SoundEnvelopeStop2 = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Stop2 = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeTick = Symbol(
+    SoundEnvelope_Tick = Symbol(
         None, None, None, "r0: Sound envelope pointer\nreturn: Current volume"
     )
 
-    SoundLfoBankReset = Symbol(None, None, None, "r0: LFO bank pointer")
+    SoundLfoBank_Reset = Symbol(None, None, None, "r0: LFO bank pointer")
 
-    SoundLfoBankSet = Symbol(
+    SoundLfoBank_Set = Symbol(
         None,
         None,
         None,
         "r0: LFO bank pointer\nr1: LFO settings pointer\nr2: Envelope level",
     )
 
-    SoundLfoBankSetConstEnvelopes = Symbol(
+    SoundLfoBank_SetConstEnvelopes = Symbol(
         None, None, None, "r0: LFO bank pointer\nr1: Level"
     )
 
-    SoundLfoBankTick = Symbol(
+    SoundLfoBank_Tick = Symbol(
         None, None, None, "r0: LFO bank pointer\nreturn: New voice update flags"
     )
 
-    SoundLfoWaveInvalidFunc = Symbol(None, None, None, "r0: LFO pointer\nreturn: 0")
+    SoundLfoWave_InvalidFunc = Symbol(None, None, None, "r0: LFO pointer\nreturn: 0")
 
-    SoundLfoWaveHalfSquareFunc = Symbol(
+    SoundLfoWave_HalfSquareFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullSquareFunc = Symbol(
+    SoundLfoWave_FullSquareFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfTriangleFunc = Symbol(
+    SoundLfoWave_HalfTriangleFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullTriangleFunc = Symbol(
+    SoundLfoWave_FullTriangleFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveSawFunc = Symbol(
+    SoundLfoWave_SawFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveReverseSawFunc = Symbol(
+    SoundLfoWave_ReverseSawFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfNoiseFunc = Symbol(
+    SoundLfoWave_HalfNoiseFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullNoiseFunc = Symbol(
+    SoundLfoWave_FullNoiseFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
     Crypto_RC4Init = Symbol(None, None, None, "")
 
     Mtx_LookAt = Symbol(None, None, None, "")
```

## pmdsky_debug_py/na.py

```diff
@@ -9959,15 +9959,15 @@
     length = 0x4000
     functions = NaItcmFunctions
     data = NaItcmData
 
 
 class NaLibsFunctions:
 
-    SoundUtilGetRandomNumber = Symbol(
+    SoundUtil_GetRandomNumber = Symbol(
         [0x81C], [0x206C8F4], None, "return: random number in the range [0, 32767]"
     )
 
     ReadWaviEntry = Symbol(
         [0x1480],
         [0x206D558],
         None,
@@ -10023,34 +10023,34 @@
         [0x83B4],
         [0x207448C],
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/"
         " and Irdkwia's notes.\n\nNo params.",
     )
 
-    SoundEnvelopeReset = Symbol(
+    SoundEnvelope_Reset = Symbol(
         [0x8B98], [0x2074C70], None, "r0: Sound envelope pointer"
     )
 
-    SoundEnvelopeParametersReset = Symbol(
+    SoundEnvelopeParameters_Reset = Symbol(
         [0x8BAC], [0x2074C84], None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeParametersCheckValidity = Symbol(
+    SoundEnvelopeParameters_CheckValidity = Symbol(
         [0x8BC8], [0x2074CA0], None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeSetParameters = Symbol(
+    SoundEnvelope_SetParameters = Symbol(
         [0x8C1C],
         [0x2074CF4],
         None,
         "r0: Sound envelope pointer\nr1: Sound envelope parameters pointer",
     )
 
-    SoundEnvelopeSetSlide = Symbol(
+    SoundEnvelope_SetSlide = Symbol(
         [0x8C80],
         [0x2074D58],
         None,
         "r0: Sound envelope pointer\nr1: Target volume\nr2: Music duration lookup table"
         " index",
     )
 
@@ -10058,90 +10058,90 @@
         [0x8D34],
         [0x2074E0C],
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/\n\nr0:"
         " Sound envelope pointer",
     )
 
-    SoundEnvelopeRelease = Symbol(
+    SoundEnvelope_Release = Symbol(
         [0x8E00], [0x2074ED8], None, "r0: Sound envelope pointer"
     )
 
-    SoundEnvelopeStop = Symbol(
+    SoundEnvelope_Stop = Symbol(
         [0x8E2C], [0x2074F04], None, "r0: Sound envelope pointer"
     )
 
-    SoundEnvelopeForceVolume = Symbol(
+    SoundEnvelope_ForceVolume = Symbol(
         [0x8E44], [0x2074F1C], None, "r0: Sound envelope pointer\nr1: Volume"
     )
 
-    SoundEnvelopeStop2 = Symbol(
+    SoundEnvelope_Stop2 = Symbol(
         [0x8E64], [0x2074F3C], None, "r0: Sound envelope pointer"
     )
 
-    SoundEnvelopeTick = Symbol(
+    SoundEnvelope_Tick = Symbol(
         [0x8E7C],
         [0x2074F54],
         None,
         "r0: Sound envelope pointer\nreturn: Current volume",
     )
 
-    SoundLfoBankReset = Symbol([0x8FC4], [0x207509C], None, "r0: LFO bank pointer")
+    SoundLfoBank_Reset = Symbol([0x8FC4], [0x207509C], None, "r0: LFO bank pointer")
 
-    SoundLfoBankSet = Symbol(
+    SoundLfoBank_Set = Symbol(
         [0x8FDC],
         [0x20750B4],
         None,
         "r0: LFO bank pointer\nr1: LFO settings pointer\nr2: Envelope level",
     )
 
-    SoundLfoBankSetConstEnvelopes = Symbol(
+    SoundLfoBank_SetConstEnvelopes = Symbol(
         [0x91D4], [0x20752AC], None, "r0: LFO bank pointer\nr1: Level"
     )
 
-    SoundLfoBankTick = Symbol(
+    SoundLfoBank_Tick = Symbol(
         [0x9220],
         [0x20752F8],
         None,
         "r0: LFO bank pointer\nreturn: New voice update flags",
     )
 
-    SoundLfoWaveInvalidFunc = Symbol(
+    SoundLfoWave_InvalidFunc = Symbol(
         [0x92D4], [0x20753AC], None, "r0: LFO pointer\nreturn: 0"
     )
 
-    SoundLfoWaveHalfSquareFunc = Symbol(
+    SoundLfoWave_HalfSquareFunc = Symbol(
         [0x92E8], [0x20753C0], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullSquareFunc = Symbol(
+    SoundLfoWave_FullSquareFunc = Symbol(
         [0x9324], [0x20753FC], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfTriangleFunc = Symbol(
+    SoundLfoWave_HalfTriangleFunc = Symbol(
         [0x936C], [0x2075444], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullTriangleFunc = Symbol(
+    SoundLfoWave_FullTriangleFunc = Symbol(
         [0x93C0], [0x2075498], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveSawFunc = Symbol(
+    SoundLfoWave_SawFunc = Symbol(
         [0x9424], [0x20754FC], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveReverseSawFunc = Symbol(
+    SoundLfoWave_ReverseSawFunc = Symbol(
         [0x9460], [0x2075538], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfNoiseFunc = Symbol(
+    SoundLfoWave_HalfNoiseFunc = Symbol(
         [0x949C], [0x2075574], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullNoiseFunc = Symbol(
+    SoundLfoWave_FullNoiseFunc = Symbol(
         [0x94E0], [0x20755B8], None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
     Crypto_RC4Init = Symbol([0x9648], [0x2075720], None, "")
 
     Mtx_LookAt = Symbol([0x9750], [0x2075828], None, "")
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -9723,15 +9723,15 @@
     length = 0x4000
     functions = NaItcmItcmFunctions
     data = NaItcmItcmData
 
 
 class NaItcmLibsFunctions:
 
-    SoundUtilGetRandomNumber = Symbol(
+    SoundUtil_GetRandomNumber = Symbol(
         None, None, None, "return: random number in the range [0, 32767]"
     )
 
     ReadWaviEntry = Symbol(
         None,
         None,
         None,
@@ -9784,32 +9784,32 @@
         None,
         None,
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/"
         " and Irdkwia's notes.\n\nNo params.",
     )
 
-    SoundEnvelopeReset = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Reset = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeParametersReset = Symbol(
+    SoundEnvelopeParameters_Reset = Symbol(
         None, None, None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeParametersCheckValidity = Symbol(
+    SoundEnvelopeParameters_CheckValidity = Symbol(
         None, None, None, "r0: Sound envelope parameters pointer"
     )
 
-    SoundEnvelopeSetParameters = Symbol(
+    SoundEnvelope_SetParameters = Symbol(
         None,
         None,
         None,
         "r0: Sound envelope pointer\nr1: Sound envelope parameters pointer",
     )
 
-    SoundEnvelopeSetSlide = Symbol(
+    SoundEnvelope_SetSlide = Symbol(
         None,
         None,
         None,
         "r0: Sound envelope pointer\nr1: Target volume\nr2: Music duration lookup table"
         " index",
     )
 
@@ -9817,76 +9817,76 @@
         None,
         None,
         None,
         "From https://projectpokemon.org/docs/mystery-dungeon-nds/procyon-studios-digital-sound-elements-r12/\n\nr0:"
         " Sound envelope pointer",
     )
 
-    SoundEnvelopeRelease = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Release = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeStop = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Stop = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeForceVolume = Symbol(
+    SoundEnvelope_ForceVolume = Symbol(
         None, None, None, "r0: Sound envelope pointer\nr1: Volume"
     )
 
-    SoundEnvelopeStop2 = Symbol(None, None, None, "r0: Sound envelope pointer")
+    SoundEnvelope_Stop2 = Symbol(None, None, None, "r0: Sound envelope pointer")
 
-    SoundEnvelopeTick = Symbol(
+    SoundEnvelope_Tick = Symbol(
         None, None, None, "r0: Sound envelope pointer\nreturn: Current volume"
     )
 
-    SoundLfoBankReset = Symbol(None, None, None, "r0: LFO bank pointer")
+    SoundLfoBank_Reset = Symbol(None, None, None, "r0: LFO bank pointer")
 
-    SoundLfoBankSet = Symbol(
+    SoundLfoBank_Set = Symbol(
         None,
         None,
         None,
         "r0: LFO bank pointer\nr1: LFO settings pointer\nr2: Envelope level",
     )
 
-    SoundLfoBankSetConstEnvelopes = Symbol(
+    SoundLfoBank_SetConstEnvelopes = Symbol(
         None, None, None, "r0: LFO bank pointer\nr1: Level"
     )
 
-    SoundLfoBankTick = Symbol(
+    SoundLfoBank_Tick = Symbol(
         None, None, None, "r0: LFO bank pointer\nreturn: New voice update flags"
     )
 
-    SoundLfoWaveInvalidFunc = Symbol(None, None, None, "r0: LFO pointer\nreturn: 0")
+    SoundLfoWave_InvalidFunc = Symbol(None, None, None, "r0: LFO pointer\nreturn: 0")
 
-    SoundLfoWaveHalfSquareFunc = Symbol(
+    SoundLfoWave_HalfSquareFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullSquareFunc = Symbol(
+    SoundLfoWave_FullSquareFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfTriangleFunc = Symbol(
+    SoundLfoWave_HalfTriangleFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullTriangleFunc = Symbol(
+    SoundLfoWave_FullTriangleFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveSawFunc = Symbol(
+    SoundLfoWave_SawFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveReverseSawFunc = Symbol(
+    SoundLfoWave_ReverseSawFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveHalfNoiseFunc = Symbol(
+    SoundLfoWave_HalfNoiseFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
-    SoundLfoWaveFullNoiseFunc = Symbol(
+    SoundLfoWave_FullNoiseFunc = Symbol(
         None, None, None, "r0: LFO pointer\nreturn: LFO current output"
     )
 
     Crypto_RC4Init = Symbol(None, None, None, "")
 
     Mtx_LookAt = Symbol(None, None, None, "")
```

## pmdsky_debug_py/protocol.py

```diff
@@ -6181,15 +6181,15 @@
     ItcmDataProtocol,
     int,
 ]
 
 
 class LibsFunctionsProtocol(Protocol):
 
-    SoundUtilGetRandomNumber: Symbol[
+    SoundUtil_GetRandomNumber: Symbol[
         Optional[list[int]],
         None,
     ]
 
     ReadWaviEntry: Symbol[
         Optional[list[int]],
         None,
@@ -6221,130 +6221,130 @@
     ]
 
     UpdateChannels: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeReset: Symbol[
+    SoundEnvelope_Reset: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeParametersReset: Symbol[
+    SoundEnvelopeParameters_Reset: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeParametersCheckValidity: Symbol[
+    SoundEnvelopeParameters_CheckValidity: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeSetParameters: Symbol[
+    SoundEnvelope_SetParameters: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeSetSlide: Symbol[
+    SoundEnvelope_SetSlide: Symbol[
         Optional[list[int]],
         None,
     ]
 
     UpdateTrackVolumeEnvelopes: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeRelease: Symbol[
+    SoundEnvelope_Release: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeStop: Symbol[
+    SoundEnvelope_Stop: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeForceVolume: Symbol[
+    SoundEnvelope_ForceVolume: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeStop2: Symbol[
+    SoundEnvelope_Stop2: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundEnvelopeTick: Symbol[
+    SoundEnvelope_Tick: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoBankReset: Symbol[
+    SoundLfoBank_Reset: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoBankSet: Symbol[
+    SoundLfoBank_Set: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoBankSetConstEnvelopes: Symbol[
+    SoundLfoBank_SetConstEnvelopes: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoBankTick: Symbol[
+    SoundLfoBank_Tick: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoWaveInvalidFunc: Symbol[
+    SoundLfoWave_InvalidFunc: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoWaveHalfSquareFunc: Symbol[
+    SoundLfoWave_HalfSquareFunc: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoWaveFullSquareFunc: Symbol[
+    SoundLfoWave_FullSquareFunc: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoWaveHalfTriangleFunc: Symbol[
+    SoundLfoWave_HalfTriangleFunc: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoWaveFullTriangleFunc: Symbol[
+    SoundLfoWave_FullTriangleFunc: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoWaveSawFunc: Symbol[
+    SoundLfoWave_SawFunc: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoWaveReverseSawFunc: Symbol[
+    SoundLfoWave_ReverseSawFunc: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoWaveHalfNoiseFunc: Symbol[
+    SoundLfoWave_HalfNoiseFunc: Symbol[
         Optional[list[int]],
         None,
     ]
 
-    SoundLfoWaveFullNoiseFunc: Symbol[
+    SoundLfoWave_FullNoiseFunc: Symbol[
         Optional[list[int]],
         None,
     ]
 
     Crypto_RC4Init: Symbol[
         Optional[list[int]],
         None,
```

## Comparing `pmdsky_debug_py-9.0.8.dist-info/METADATA` & `pmdsky_debug_py-9.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 9.0.8
+Version: 9.0.9
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `pmdsky_debug_py-9.0.8.dist-info/RECORD` & `pmdsky_debug_py-9.0.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pmdsky_debug_py/__init__.py,sha256=xvXjdxEqeoQaaS6ssZYVI9jARzv5M4q6FNwA3Z6fOw4,1831
-pmdsky_debug_py/_release.py,sha256=ZyC-kt6anIaC-P1OECbcC9pci6N8Gv4rzVMBDHYy6aY,30
-pmdsky_debug_py/eu.py,sha256=2XsmCZQJ6o9yqc2owmMtRr3h0PKkWF0scdGtPirj7O0,937244
-pmdsky_debug_py/eu_itcm.py,sha256=Vavlp4V8f_FrZUmeLznmXk0nsI4mwaUtBkRLsZU0C4g,889624
-pmdsky_debug_py/jp.py,sha256=9VdJwKFOQ5025CHq9fp5SJoxmsoWnq2df-y5mlgDn3A,921986
-pmdsky_debug_py/jp_itcm.py,sha256=1IyFSmKU_xSIIVO9Oab-yigethh1JpFVhfquHUGRwRo,889614
-pmdsky_debug_py/na.py,sha256=P8-RkY7_EIPlc74hyglM4Kn7i_CpDsju8hh8zDIarGw,938456
-pmdsky_debug_py/na_itcm.py,sha256=CjPso4VWZEVpNReXDbEuJz2DUDfKqN_I0_1QDdxswSo,889644
-pmdsky_debug_py/protocol.py,sha256=H95ob-nyBstgzFDuM3V1_his5I8kN7JLKm2dxRqmm7E,306661
+pmdsky_debug_py/_release.py,sha256=I9VuCydGIbt1J17l-0HWFKT4sqSnxhLnCC3DUTaNo-c,30
+pmdsky_debug_py/eu.py,sha256=VaCTgvgEUSXlKWHRw07k7HvXS2AL-3yil8G6hIbXdLI,937268
+pmdsky_debug_py/eu_itcm.py,sha256=PxqDymHs25O7Gom8aKOTcvRN-w-Ey6ujZEVISKOhZeE,889648
+pmdsky_debug_py/jp.py,sha256=FtP7-j4ETptuTCUlcDVoLyzLnJoY6Hd_MOysGzLQ5p4,922010
+pmdsky_debug_py/jp_itcm.py,sha256=2gDTGVuvHvXzVzNgBx0KV2ZBDROyFrwnsG9yGPrk4kE,889638
+pmdsky_debug_py/na.py,sha256=pMXltSJwA-xf6pTSQdWNnZfts9egurnFIQ8g3ZQcJDM,938480
+pmdsky_debug_py/na_itcm.py,sha256=Wu1AFVb6tdY96-eZVH10I-P9IQ8HpegQOAbK1h7vEz8,889668
+pmdsky_debug_py/protocol.py,sha256=HWixl6nSHgJsLOrcSzluhYdYV6-ovD_wQAXdkcYBsPc,306685
 pmdsky_debug_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pmdsky_debug_py-9.0.8.dist-info/METADATA,sha256=la_FKqUqb0N_kcQKULkLAfFbG2xkSYLoob0585Y9DrA,1372
-pmdsky_debug_py-9.0.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-pmdsky_debug_py-9.0.8.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
-pmdsky_debug_py-9.0.8.dist-info/RECORD,,
+pmdsky_debug_py-9.0.9.dist-info/METADATA,sha256=tTozoXbHAX1PGom194Tkw7_kLyVNVSu1N8hQTfydp2k,1372
+pmdsky_debug_py-9.0.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+pmdsky_debug_py-9.0.9.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
+pmdsky_debug_py-9.0.9.dist-info/RECORD,,
```

