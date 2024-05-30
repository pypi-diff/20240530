# Comparing `tmp/kojen-1.2.30.tar.gz` & `tmp/kojen-1.3.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kojen-1.2.30.tar", last modified: Sun Apr  9 13:23:09 2023, max compression
+gzip compressed data, was "kojen-1.3.31.tar", last modified: Thu May 30 12:41:28 2024, max compression
```

## Comparing `kojen-1.2.30.tar` & `kojen-1.3.31.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.068413 kojen-1.2.30/
--rw-rw-rw-   0        0        0    20890 2023-04-09 13:23:09.068413 kojen-1.2.30/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.028377 kojen-1.2.30/kojen/
--rw-rw-rw-   0        0        0     6200 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/Generate.py
--rw-rw-rw-   0        0        0    14933 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/Language.py
--rw-rw-rw-   0        0        0    44063 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/LanguageCPP.py
--rw-rw-rw-   0        0        0    45191 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/LanguageCsharp.py
--rw-rw-rw-   0        0        0    10159 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/LanguagePython.py
--rw-rw-rw-   0        0        0      357 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/__init__.py
--rw-rw-rw-   0        0        0       26 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/__main__.py
--rw-rw-rw-   0        0        0    27220 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/cgen.py
--rw-rw-rw-   0        0        0    10071 2023-03-25 18:25:48.000000 kojen-1.2.30/kojen/coggen.py
--rw-rw-rw-   0        0        0    17170 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/kojentypes.py
--rw-rw-rw-   0        0        0     3169 2023-03-25 18:25:48.000000 kojen-1.2.30/kojen/plant.py
--rw-rw-rw-   0        0        0     9902 2022-08-08 16:04:22.000000 kojen-1.2.30/kojen/preservative.py
--rw-rw-rw-   0        0        0     7048 2023-03-25 18:25:48.000000 kojen-1.2.30/kojen/protogen.py
--rw-rw-rw-   0        0        0    48690 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/smgen.py
--rw-rw-rw-   0        0        0     4127 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/smvppxml.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.067413 kojen-1.2.30/kojen/test/
--rw-rw-rw-   0        0        0        0 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/test/__init__.py
--rw-rw-rw-   0        0        0    12569 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/test/cgen_test.py
--rw-rw-rw-   0        0        0    10621 2022-08-08 16:04:22.000000 kojen-1.2.30/kojen/test/preservative_test.py
--rw-rw-rw-   0        0        0    18069 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/test/smgen_test.py
--rw-rw-rw-   0        0        0    15390 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/test/vppclassdiagram_test.py
--rw-rw-rw-   0        0        0     3782 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/test/vppfs_test.py
--rw-rw-rw-   0        0        0    24276 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/umlgen.py
--rw-rw-rw-   0        0        0    49539 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/vppclassdiagram.py
--rw-rw-rw-   0        0        0    35625 2022-12-09 07:45:22.000000 kojen-1.2.30/kojen/vppfs.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.050386 kojen-1.2.30/kojen.egg-info/
--rw-rw-rw-   0        0        0    20890 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 13:23:09.069413 kojen-1.2.30/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-04-09 13:22:41.000000 kojen-1.2.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:41:28.927122 kojen-1.3.31/
+-rw-rw-rw-   0        0        0     1121 2022-03-14 15:32:21.000000 kojen-1.3.31/LICENSE
+-rw-rw-rw-   0        0        0    18384 2024-05-30 12:41:28.925120 kojen-1.3.31/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 12:41:28.852181 kojen-1.3.31/kojen/
+-rw-rw-rw-   0        0        0     7734 2024-05-30 12:38:08.000000 kojen-1.3.31/kojen/Generate.py
+-rw-rw-rw-   0        0        0     3025 2024-05-30 12:38:08.000000 kojen-1.3.31/kojen/Install.py
+-rw-rw-rw-   0        0        0    14933 2023-03-27 09:38:27.000000 kojen-1.3.31/kojen/Language.py
+-rw-rw-rw-   0        0        0    44063 2023-03-27 09:38:27.000000 kojen-1.3.31/kojen/LanguageCPP.py
+-rw-rw-rw-   0        0        0    45191 2023-03-27 09:38:27.000000 kojen-1.3.31/kojen/LanguageCsharp.py
+-rw-rw-rw-   0        0        0    10159 2023-03-27 09:38:27.000000 kojen-1.3.31/kojen/LanguagePython.py
+-rw-rw-rw-   0        0        0      357 2022-07-18 07:44:30.000000 kojen-1.3.31/kojen/__init__.py
+-rw-rw-rw-   0        0        0       26 2022-07-18 07:44:30.000000 kojen-1.3.31/kojen/__main__.py
+-rw-rw-rw-   0        0        0    27204 2024-05-30 12:38:08.000000 kojen-1.3.31/kojen/cgen.py
+-rw-rw-rw-   0        0        0    10071 2023-03-27 09:38:27.000000 kojen-1.3.31/kojen/coggen.py
+-rw-rw-rw-   0        0        0    17170 2023-08-08 08:25:38.000000 kojen-1.3.31/kojen/kojentypes.py
+-rw-rw-rw-   0        0        0     3169 2023-03-07 07:39:45.000000 kojen-1.3.31/kojen/plant.py
+-rw-rw-rw-   0        0        0     9902 2022-08-08 17:08:26.000000 kojen-1.3.31/kojen/preservative.py
+-rw-rw-rw-   0        0        0     7048 2023-03-27 09:38:27.000000 kojen-1.3.31/kojen/protogen.py
+-rw-rw-rw-   0        0        0    48690 2023-08-08 08:25:38.000000 kojen-1.3.31/kojen/smgen.py
+-rw-rw-rw-   0        0        0     4127 2022-07-18 07:44:30.000000 kojen-1.3.31/kojen/smvppxml.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:41:28.920603 kojen-1.3.31/kojen/test/
+-rw-rw-rw-   0        0        0        0 2022-07-18 07:44:30.000000 kojen-1.3.31/kojen/test/__init__.py
+-rw-rw-rw-   0        0        0    12569 2023-08-08 08:25:38.000000 kojen-1.3.31/kojen/test/cgen_test.py
+-rw-rw-rw-   0        0        0     2897 2024-05-30 12:38:08.000000 kojen-1.3.31/kojen/test/install_test.py
+-rw-rw-rw-   0        0        0    10621 2022-08-08 17:08:26.000000 kojen-1.3.31/kojen/test/preservative_test.py
+-rw-rw-rw-   0        0        0    18069 2023-08-08 08:25:38.000000 kojen-1.3.31/kojen/test/smgen_test.py
+-rw-rw-rw-   0        0        0    15390 2022-07-18 07:44:30.000000 kojen-1.3.31/kojen/test/vppclassdiagram_test.py
+-rw-rw-rw-   0        0        0     3782 2022-07-18 07:44:30.000000 kojen-1.3.31/kojen/test/vppfs_test.py
+-rw-rw-rw-   0        0        0    24276 2023-03-07 07:39:45.000000 kojen-1.3.31/kojen/umlgen.py
+-rw-rw-rw-   0        0        0    49539 2022-07-18 07:44:30.000000 kojen-1.3.31/kojen/vppclassdiagram.py
+-rw-rw-rw-   0        0        0    35625 2022-10-12 16:33:02.000000 kojen-1.3.31/kojen/vppfs.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:41:28.877359 kojen-1.3.31/kojen.egg-info/
+-rw-rw-rw-   0        0        0    18384 2024-05-30 12:41:28.000000 kojen-1.3.31/kojen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2024-05-30 12:41:28.000000 kojen-1.3.31/kojen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:41:28.000000 kojen-1.3.31/kojen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 12:41:28.000000 kojen-1.3.31/kojen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 12:41:28.000000 kojen-1.3.31/kojen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:41:28.928125 kojen-1.3.31/setup.cfg
+-rw-rw-rw-   0        0        0     1589 2024-05-30 12:38:08.000000 kojen-1.3.31/setup.py
```

### Comparing `kojen-1.2.30/PKG-INFO` & `kojen-1.3.31/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,330 +1,333 @@
 Metadata-Version: 2.1
 Name: kojen
-Version: 1.2.30
+Version: 1.3.31
 Summary: Code generation tools.
 Home-page: https://github.com/kohjaen/kojen
 Author: kohjaen
 Author-email: koh.jaen@yahoo.de
 License: UNKNOWN
-Description: ![CI](https://github.com/kohjaen/kojen/workflows/CI/badge.svg)
-        
-        # Description
-        
-        Kojen is a protocol (C++), state-machine(C++/C#/Python) and Class (C++/C# from UML) code-generation tool written in Python and existing within the Python Package Index (PyPi). Python >= 3.6.8 is supported. To install run ```python -m pip install kojen```.  
-        
-        The default generated state-machine uses the fast and lightweight single-header-file-only [boost sml](https://boost-ext.github.io/sml/). It is linked to the repository as a git sub-module for an out-the-box solution. This is suitable for both embedded and PC applications using C++14 and higher.
-        
-        For state-machines and software-architecture-from-UML-model : user-code is preserved within special comment tags. Should you change the name of tags that had code within them, on the next generation a new text file prepended with ```.Lostcode``` will be output next to the original source file with all the code that was lost. The main concept is that code-generation is a manually-initiated process and exists within a hand-crafted source-repository. The intention is to be able to manually program in all auto-generated state-machine / Class Diagram output source files, and preserve hand-crafted code within those files when system requirements change. Its not intended to disassociate the programmer from the code (like most CASE tools). Typically after the Design phase code-generation is done first in the initial implementation phase (and maybe a few more times until things are as they should be) and then development is done the usual way. Naturally in time further changes/additions can be done in the model (Updating the 'diagrams' first) and their changes propagated to code by generation : this also allows for updates to the design (from Model -> Code) in a non-intrusive manner. Protocols and their unit tests are the only files which require no hand-coding.
-        
-        Unit testing : Tests for protocols are generated, and tests for state-machines too (but those require some hand-coding, code preservation applies). The included testing framework is extremely light-weight and great for embedded (and PC) applications : [minunit](https://github.com/kohjaen/minunit) is used for this and it is also linked to the repository as a git sub-module. The original fork of minunit is a C-based single header file, but some improvements have been made (not possible with C) so it now consists of a single header and a single cpp file. It contains a test-runner which will run all registered test-suites.
-        
-        It currently supports Windows/Linux/MacOS and FreeRTOS and includes multi-threading components (threads/queues/dispatchers/fixed-block-memory-allocators as well as stl-with-fixed-block-mem-allocator wrappers for no spurious heap usage and much faster STL containers) that works on all platforms by including CMake configuration files in generated outputs.
-        
-        Message Queues use move-semantics and are thus platform independant and adding a new RTOS will only require adding a 'condition variable' like synchronization mechanism for that RTOS (the provided example of how it is done with FreeRTOS can be followed).
-        
-        # Quickstart
-        ## Example folder
-        
-        The git repository has a fully functional example (which is used in the CI), including CMake integration. An executable is generated and that runs all unit tests. Feel free to go straight there. The example is described below.
-        
-        ## Protocol
-        ### Input
-        In a folder where you will execute your project from, create the interface definition file `MyInterface.py`.
-        
-        In your interface definition file `MyInterface.py` create a function `CreateInterface()` that returns a  `kojen.Interface` object. 
-        
-        Here is an example of what is permissible in an interface. For messages, make sure each has a unique message-id (second parameter after the name in the constructor)
-        ```python
-        from kojen.kojentypes import *
-        
-        def CreateInterface():
-            sCustomStruct = Struct('sCustomStruct')
-            sCustomStruct.AddType('m_Member1','uint16')
-            sCustomStruct.AddType('m_Member2','uint16')
-            sCustomStruct.AddType('m_Member3','uint32')
-        
-            MsgSomeCMD = Message('MsgSomeCMD',0x01)
-            MsgSomeCMD.AddType('m_Member1','uint8')
-        
-            MsgSomeCMDRSP = Message('MsgSomeCMDRSP',0x02)
-            MsgSomeCMDRSP.AddStruct('mStructMember1',sCustomStruct)
-            MsgSomeCMDRSP.AddType('m_Member2','uint8')
-            
-            MsgSomeREQ = Message('MsgSomeREQ',0x03)
-            MsgSomeREQ.AddType('m_Member1','uint8')
-        
-            #Array of type : Not supported by ARM due to dynamic memory allocation requirements
-            MsgSomeREQRSP = Message('MsgSomeREQRSP',0x04)
-            MsgSomeREQRSP.AddStruct('mStructMember1',sCustomStruct)
-            MsgSomeREQRSP.AddType('m_Member2','uint8')
-            MsgSomeREQRSP.AddArrayOfType('mArrayMember3','double')
-        
-        
-            MsgSomeUnsolicitedData = Message('MsgSomeUnsolicitedData',0x05)
-            MsgSomeUnsolicitedData.AddArrayOfStruct('mStructArrayMember1',sCustomStruct)
-        
-            #
-            # Includes : Enums and defines ...
-            #
-            Type = Enum("Type")
-            Type.Add("kOne", 0)
-            Type.Add("kTwo", 1)
-        
-            Revision = Enum("Revision")
-            Revision.Add("kVersion1", 0)
-            Revision.Add("kVersion2", 1)
-            Revision.Add("kVersion3", 2)
-        
-            interface = Interface('IMyInterfaceIO')
-        
-            interface.AddEnum(Type)
-            interface.AddEnum(Revision)
-        
-            interface.AddHashDefine("THREE", 3)
-            interface.AddHashDefine("PI", 3.14159265359)
-        
-            interface.AddStruct(sCustomStruct)
-            interface.AddMessage(MsgSomeCMD)
-            interface.AddMessage(MsgSomeCMDRSP)
-            interface.AddMessage(MsgSomeREQ)
-            interface.AddMessage(MsgSomeREQRSP)
-            interface.AddMessage(MsgSomeUnsolicitedData)
-        
-            return interface
-        ```
-        
-        Then, create a file `Generate.py`.
-        
-        
-        ```python
-        import kojen.Generate as Generate
-        import os
-        
-        author = "myname@mydomain.com"
-        group  = "MY_PACKAGE"
-        brief  = "An example demonstrating protocol code-generation abilities."
-        namespacename = "ExampleIO"
-        classname = "CExampleIF"
-        declspec = "" # your define for symbol export/import in C++ e.g. MY_PROJECT_API
-        outputdir = os.path.join(os.path.abspath(os.path.dirname(__file__)), os.path.join("autogen","protocol"))
-        protocolfile = os.path.join(os.path.abspath(os.path.dirname(__file__)), "MyInterface.py")
-        Generate.Protocol(outputdir, protocolfile, namespacename, classname, declspec, author, group, brief)
-        ```
-        
-        Execute `Generate.py` using python. Your C++ code should be in the folder **./autogen/protocol**.
-        
-        > **Please note** : you may include this code in a library, and thus want to export some of the generated features.
-        > Typically somewhere in a common header of your C++ code, you would have declared something like
-        
-        ```cplusplus
-        #ifdef MY_PROJECT_EXPORTS
-        #	define MY_PROJECT_API __declspec(dllexport)
-        #else
-        #	define MY_PROJECT_API __declspec(dllimport)
-        #endif
-        ```
-        
-        > You should thus pass **MY_PROJECT_API** as the *declspec* argument to the generator.
-        
-        ### Output
-        
-        There will be several files in the output folder.
-        
-        * allplatforms *(folder containing required framework files)*
-        * CExampleIF.h *(contains all factories to create messages which automatically and correctly fill in the headers, as well as serialization to/from bytestreams.)
-        * CExampleIF.cpp
-        * CExampleIFDefines.h *(contains all enums and defines)
-        * CExampleIFReceiver.h *(contains a derivable class that received fully constructed messages. Override receive functions to handle them as per need.)
-        * CExampleIFReceiver.cpp
-        * CExampleIFStructs.h *(contains all structs)
-        * CExampleIFTests.cpp *(contains all unit tests)
-        * CExampleIFTransmitter.h *(contains all functions to transmit fully constructed messages. Highly advices to use the autogenerated factories.)
-        * CExampleIFTransmitter.cpp
-        * MsgHeader.h
-        
-        The following class diagram explains roughly where focus should be when implementing for actual integration into the real system.
-        
-        <!---![Image of necessary classes](kojen/docs/images/ProtocolClassDiagram.PNG) ... doesnt work on PyPi!--->
-        ![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/ProtocolClassDiagram.PNG)
-        
-        *IConnection* is the interface to derive from for your actual physical layer for an embedded platform. If you use boost on x86/x64, in the 'allplatforms' directory exist classes for substituting this with a TCPConnection, UDPConnection and SerialPort.
-        Have a good look at the unit tests, this shows roughly how to derive from it and connect everything up, albeit creating a loopback connection, and implementing uncessary routing as the interface for the tests have a special requirement.
-        
-        A summary to link it up:
-        * Create a derived IConnection that knows how to send and receive physical layer data.
-        * Create a generated Transmitter, passing it a pointer to this connection.
-        * Create a generated Receiver
-        * Set the Receiver to the derived IConnection. You will then get messages in the message receiving functions...override the correct ones to handle them.
-        * Use the Transmitter to send.
-        
-        ## State Machine in C++
-        ### Requrements
-        - Don't forget to update your git submodules when checking out.
-        ### Input
-        The following diagram defines (roughly) a state machine for a CD player.
-        
-        <!---![Image of CD Player](kojen/docs/images/StateMachine.PNG)--->
-        
-        ![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/StateMachine.PNG)
-        
-        This state machine can be represented by the following transition table in python (format : 'startstate', 'event', 'nextstate', 'action', 'guard'):
-        
-        ```python
-        #
-        # StartState    Event                     NextState     Action                 Guard
-        #
-         'StateStop',  'EventOpen',              'StateOpen',  'OnOpenDrive',         'None'
-         'StateStop',  'EventPlay',              'StatePlay',  'OnPlayTrack',         'GuardCDInside'
-         'StateOpen',  'EventOpen',              'StateStop',  'OnCloseDrive',        'None'
-         'StatePlay',  'EventPlay',              'StatePause', 'OnPause',             'None'
-         'StatePlay',  'EventEndOfTrack',        'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'
-         'StatePlay',  'EventEndOfTrack',        'StateStop',  'OnStop',              'GuardCDHasNoMoreTracks'
-         'StatePlay',  'EventSkipNextTrack',     'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'
-         'StatePlay',  'EventSkipPreviousTrack', 'None',       'OnPlayPreviousTrack', 'GuardCDHasPreviousTrack'
-         'StatePlay',  'EventStop',              'StateStop',  'OnStop',              'None'
-         'StatePause', 'EventPlay',              'StatePlay',  'OnPlayTrack',         'None'
-         'StatePause', 'EventAfter10Minutes',    'StateStop',  'OnStop',              'None'
-        ```
-        
-        Create a file `Generate.py` (or add your state machine to the one already present in your project) :
-        
-        ```python
-        from kojen import Generate
-        from kojen.kojentypes import *
-        
-        #
-        # Generate Statemachine (from TransitionTable)
-        #
-        
-        # For playing a track the tracknumber should be parameterized.
-        EventPlay = Struct('EventPlay')
-        EventPlay.AddType('m_track_no','uint16_t')
-        
-        eventsinterface = Interface('params')
-        eventsinterface.AddStruct(EventPlay)
-        
-        # Optional features
-        eventsinterface.AddUserTag("StateMachineThread", 1) # 0 = SM runs on caller thread, 1 = SM runs on its own thread. Default is 1.
-        eventsinterface.AddUserTag("Verbose", 1)            # 0 = No printouts, 1 = printouts. Default is 1.
-        
-        # Transition Table.
-        transition_table = []
-        #                         StartState    Event                     NextState     Action                 Guard
-        transition_table.append(['StateStop',  'EventOpen',              'StateOpen',  'OnOpenDrive',         'None'                   ])
-        transition_table.append(['StateStop',  'EventPlay',              'StatePlay',  'OnPlayTrack',         'GuardCDInside'          ]) 
-        transition_table.append(['StateOpen',  'EventOpen',              'StateStop',  'OnCloseDrive',        'None'                   ]) 
-        transition_table.append(['StatePlay',  'EventPlay',              'StatePause', 'OnPause',             'None'                   ])
-        transition_table.append(['StatePlay',  'EventEndOfTrack',        'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'   ])
-        transition_table.append(['StatePlay',  'EventEndOfTrack',        'StateStop',  'OnStop',              'GuardCDHasNoMoreTracks' ])
-        transition_table.append(['StatePlay',  'EventSkipNextTrack',     'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'   ]) 
-        transition_table.append(['StatePlay',  'EventSkipPreviousTrack', 'None',       'OnPlayPreviousTrack', 'GuardCDHasPreviousTrack'])
-        transition_table.append(['StatePlay',  'EventStop',              'StateStop',  'OnStop',              'None'                   ])
-        transition_table.append(['StatePause', 'EventPlay',              'StatePlay',  'OnPlayTrack',         'None'                   ])
-        transition_table.append(['StatePause', 'EventAfter10Minutes',    'StateStop',  'OnStop',              'None'                   ])
-        
-        author = "myname@mydomain.com"
-        group  = "MY_PACKAGE"
-        brief  = "An example demonstrating state-machine code-generation abilities."
-        
-        eventsinterface = None
-        namespacename = "CDPlayerSM"
-        statemachinenameprefix = "CDPlayer"
-        declspec = ""
-        outputdir = "autogen/state_machine"
-        templatedir = "" # defaults are for 'SML'
-        Generate.StateMachine(outputdir, transition_table, eventsinterface, namespacename, statemachinenameprefix, declspec, author, group, brief, templatedir)
-        ```
-        
-        Execute `Generate.py` using python. Your C++ code should be generated to the configured folder **./autogen/state_machine**.
-        
-        > **Please note** : you may may wish to parameterize events in your statemachine. An event is of type `kojen.Struct` in a `kojen.Interface` object. 
-        > Simply follow the quickstart for protocols, creating and returning an interface : your Event structs need to have the exact same name as defined in the transition table.
-        > You should thus pass your interface object  as the *eventsinterface* argument to the generator instead of **None**.
-        
-        ### Output
-        
-        There will be several files in the output folder.
-        
-        * allplatforms *(folder containing framework files for standalone solution)*
-        * CDPlayerStateMachine.h
-        * CDPlayerStateMachineImpl_SML.cpp *(all state machine code generated for boost-sml)*  
-        * ICDPlayerController.h
-        * Test.CDPlayerStateMachine.cpp
-          
-        The following class diagram explains roughly where focus should be when implementing for test-driven development as well as for actual integration into the real system.
-        
-        <!---![Image of necessary classes](kojen/docs/images/StateMachineClassDiagram.PNG)--->
-        ![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/StateMachineClassDiagram.PNG)
-        
-        White classes are auto-generated, and have code-preservation features. Grey is what you have to manually create, and implement for integration into your real system.
-        
-        All required functionality for your system should be implemented in the **Controller** classes, being the base-class *ICDPlayerController*, the derived *C_My_CDPlayerController* and the derived test class *CTestCDPlayerController*.
-        
-        It is critical that as much of the 'business logic' is put into the base class *IPlayerController*, and tested using the *CTestCDPlayerController* in the unit-tests as possible, such that the actual integrated *C_My_CDPlayerController* uses unit-tested business logic, with a good example of how its intended to work in the unit tests...as well as for regression testing and continuous integration.
-        
-        As the state-machine-implementation uses the controller base class, the following construction is valid for unit tests and system integration by substituting the correct controller:
-        
-        ```cplusplus
-          CTestCDPlayerController controller;
-          auto* sm = ICDPlayerStateMachine::Create(controller);
-        ```
-        
-        All state queries and event triggering are done using the ```sm``` instance.
-        
-        Due to the use of move-semantics, parameterized event structs are unique_ptr's (allocated in fixed-blocks for embedded applications) and thus once an event is triggered those pointers are no longer valid in the calling context.
-        
-        ## State Machine in C#
-        
-        Similar to the above example, the only difference is the Generate call to use.
-        
-        ```python
-           ...
-           Generate.StateMachine_CSHARP(...)
-           ...
-        ```
-        
-        ## State Machine in Python
-        
-        Similar to the above example, the only difference is the Generate call to use.
-        
-        ```python
-            ...
-           Generate.StateMachine_PYTHON(...)
-           ...
-        ```
-        
-        <!---
-        ### Deferred Events
-        
-        Deferred events are supported in SML and MSM state machines.
-        
-        In the example CD player statemachine this use-case could be pressing 'play' whilst the tray is closing : the close button will be pressed, and the tray will start closing, however the software trigger for *EventOpen* will only occur on the interrupt signalling that the tray actuator has completed either opening/closing the tray. 
-        This can take up to several seconds. In that time, the 'play' button could be pressed. 
-        
-        The desired behaviour would be that once the tray is closed, the CD starts playing.
-        
-        This can be achieved by manually adding the correct deferred event in the *CDPlayerStateMachineImpl_SML.cpp* in the code preservation tags at the end of the transition table:
-        
-        ```cplusplus
-        /// {{{USER_DEFERRED_EVENTS}}}
-        , StateOpen + event<EventPlay> / defer
-        /// {{{USER_DEFERRED_EVENTS}}}
-        ```
-        
-        For *boost::msm* this can be achieved by manually adding the correct deferred event in code preservation tags in the state struct for *StateOpen* in *CDPlayerStateMachineImpl_SML.cpp* :
-        
-        ```cplusplus
-        /// {{{USER_StateOpen_DEFERRED_EVENTS}}}
-        typedef boost::mpl::vector<EventPlay> deferred_events;
-        /// {{{USER_StateOpen_DEFERRED_EVENTS}}} 
-        ```
-        
-        I believe this will also allow the sequence of 'play' then 'close' to work.
-        --->
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![CI](https://github.com/kohjaen/kojen/workflows/CI/badge.svg)
+
+# Description
+
+Kojen is a protocol (C++), state-machine(C++/C#/Python) and Class (C++/C# from UML) code-generation tool written in Python and existing within the Python Package Index (PyPi). Python >= 3.6.8 is supported. To install run ```python -m pip install kojen```.  
+
+The default generated state-machine uses the fast and lightweight single-header-file-only [boost sml](https://boost-ext.github.io/sml/). It is linked to the repository as a git sub-module for an out-the-box solution. This is suitable for both embedded and PC applications using C++14 and higher.
+
+For state-machines and software-architecture-from-UML-model : user-code is preserved within special comment tags. Should you change the name of tags that had code within them, on the next generation a new text file prepended with ```.Lostcode``` will be output next to the original source file with all the code that was lost. The main concept is that code-generation is a manually-initiated process and exists within a hand-crafted source-repository. The intention is to be able to manually program in all auto-generated state-machine / Class Diagram output source files, and preserve hand-crafted code within those files when system requirements change. Its not intended to disassociate the programmer from the code (like most CASE tools). Typically after the Design phase code-generation is done first in the initial implementation phase (and maybe a few more times until things are as they should be) and then development is done the usual way. Naturally in time further changes/additions can be done in the model (Updating the 'diagrams' first) and their changes propagated to code by generation : this also allows for updates to the design (from Model -> Code) in a non-intrusive manner. Protocols and their unit tests are the only files which require no hand-coding.
+
+Unit testing : Tests for protocols are generated, and tests for state-machines too (but those require some hand-coding, code preservation applies). The included testing framework is extremely light-weight and great for embedded (and PC) applications : [minunit](https://github.com/kohjaen/minunit) is used for this and it is also linked to the repository as a git sub-module. The original fork of minunit is a C-based single header file, but some improvements have been made (not possible with C) so it now consists of a single header and a single cpp file. It contains a test-runner which will run all registered test-suites.
+
+It currently supports Windows/Linux/MacOS and FreeRTOS and includes multi-threading components (threads/queues/dispatchers/fixed-block-memory-allocators as well as stl-with-fixed-block-mem-allocator wrappers for no spurious heap usage and much faster STL containers) that works on all platforms by including CMake configuration files in generated outputs.
+
+Message Queues use move-semantics and are thus platform independant and adding a new RTOS will only require adding a 'condition variable' like synchronization mechanism for that RTOS (the provided example of how it is done with FreeRTOS can be followed).
+
+# Quickstart
+## Example folder
+
+The git repository has a fully functional example (which is used in the CI), including CMake integration. An executable is generated and that runs all unit tests. Feel free to go straight there. The example is described below.
+
+## Protocol
+### Input
+In a folder where you will execute your project from, create the interface definition file `MyInterface.py`.
+
+In your interface definition file `MyInterface.py` create a function `CreateInterface()` that returns a  `kojen.Interface` object. 
+
+Here is an example of what is permissible in an interface. For messages, make sure each has a unique message-id (second parameter after the name in the constructor)
+```python
+from kojen.kojentypes import *
+
+def CreateInterface():
+    sCustomStruct = Struct('sCustomStruct')
+    sCustomStruct.AddType('m_Member1','uint16')
+    sCustomStruct.AddType('m_Member2','uint16')
+    sCustomStruct.AddType('m_Member3','uint32')
+
+    MsgSomeCMD = Message('MsgSomeCMD',0x01)
+    MsgSomeCMD.AddType('m_Member1','uint8')
+
+    MsgSomeCMDRSP = Message('MsgSomeCMDRSP',0x02)
+    MsgSomeCMDRSP.AddStruct('mStructMember1',sCustomStruct)
+    MsgSomeCMDRSP.AddType('m_Member2','uint8')
+    
+    MsgSomeREQ = Message('MsgSomeREQ',0x03)
+    MsgSomeREQ.AddType('m_Member1','uint8')
+
+    #Array of type : Not supported by ARM due to dynamic memory allocation requirements
+    MsgSomeREQRSP = Message('MsgSomeREQRSP',0x04)
+    MsgSomeREQRSP.AddStruct('mStructMember1',sCustomStruct)
+    MsgSomeREQRSP.AddType('m_Member2','uint8')
+    MsgSomeREQRSP.AddArrayOfType('mArrayMember3','double')
+
+
+    MsgSomeUnsolicitedData = Message('MsgSomeUnsolicitedData',0x05)
+    MsgSomeUnsolicitedData.AddArrayOfStruct('mStructArrayMember1',sCustomStruct)
+
+    #
+    # Includes : Enums and defines ...
+    #
+    Type = Enum("Type")
+    Type.Add("kOne", 0)
+    Type.Add("kTwo", 1)
+
+    Revision = Enum("Revision")
+    Revision.Add("kVersion1", 0)
+    Revision.Add("kVersion2", 1)
+    Revision.Add("kVersion3", 2)
+
+    interface = Interface('IMyInterfaceIO')
+
+    interface.AddEnum(Type)
+    interface.AddEnum(Revision)
+
+    interface.AddHashDefine("THREE", 3)
+    interface.AddHashDefine("PI", 3.14159265359)
+
+    interface.AddStruct(sCustomStruct)
+    interface.AddMessage(MsgSomeCMD)
+    interface.AddMessage(MsgSomeCMDRSP)
+    interface.AddMessage(MsgSomeREQ)
+    interface.AddMessage(MsgSomeREQRSP)
+    interface.AddMessage(MsgSomeUnsolicitedData)
+
+    return interface
+```
+
+Then, create a file `Generate.py`.
+
+
+```python
+import kojen.Generate as Generate
+import os
+
+author = "myname@mydomain.com"
+group  = "MY_PACKAGE"
+brief  = "An example demonstrating protocol code-generation abilities."
+namespacename = "ExampleIO"
+classname = "CExampleIF"
+declspec = "" # your define for symbol export/import in C++ e.g. MY_PROJECT_API
+outputdir = os.path.join(os.path.abspath(os.path.dirname(__file__)), os.path.join("autogen","protocol"))
+protocolfile = os.path.join(os.path.abspath(os.path.dirname(__file__)), "MyInterface.py")
+Generate.Protocol(outputdir, protocolfile, namespacename, classname, declspec, author, group, brief)
+```
+
+Execute `Generate.py` using python. Your C++ code should be in the folder **./autogen/protocol**.
+
+> **Please note** : you may include this code in a library, and thus want to export some of the generated features.
+> Typically somewhere in a common header of your C++ code, you would have declared something like
+
+```cplusplus
+#ifdef MY_PROJECT_EXPORTS
+#	define MY_PROJECT_API __declspec(dllexport)
+#else
+#	define MY_PROJECT_API __declspec(dllimport)
+#endif
+```
+
+> You should thus pass **MY_PROJECT_API** as the *declspec* argument to the generator.
+
+### Output
+
+There will be several files in the output folder.
+
+* allplatforms *(folder containing required framework files)*
+* CExampleIF.h *(contains all factories to create messages which automatically and correctly fill in the headers, as well as serialization to/from bytestreams.)
+* CExampleIF.cpp
+* CExampleIFDefines.h *(contains all enums and defines)
+* CExampleIFReceiver.h *(contains a derivable class that received fully constructed messages. Override receive functions to handle them as per need.)
+* CExampleIFReceiver.cpp
+* CExampleIFStructs.h *(contains all structs)
+* CExampleIFTests.cpp *(contains all unit tests)
+* CExampleIFTransmitter.h *(contains all functions to transmit fully constructed messages. Highly advices to use the autogenerated factories.)
+* CExampleIFTransmitter.cpp
+* MsgHeader.h
+
+The following class diagram explains roughly where focus should be when implementing for actual integration into the real system.
+
+<!---![Image of necessary classes](kojen/docs/images/ProtocolClassDiagram.PNG) ... doesnt work on PyPi!--->
+![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/ProtocolClassDiagram.PNG)
+
+*IConnection* is the interface to derive from for your actual physical layer for an embedded platform. If you use boost on x86/x64, in the 'allplatforms' directory exist classes for substituting this with a TCPConnection, UDPConnection and SerialPort.
+Have a good look at the unit tests, this shows roughly how to derive from it and connect everything up, albeit creating a loopback connection, and implementing uncessary routing as the interface for the tests have a special requirement.
+
+A summary to link it up:
+* Create a derived IConnection that knows how to send and receive physical layer data.
+* Create a generated Transmitter, passing it a pointer to this connection.
+* Create a generated Receiver
+* Set the Receiver to the derived IConnection. You will then get messages in the message receiving functions...override the correct ones to handle them.
+* Use the Transmitter to send.
+
+## State Machine in C++
+### Requrements
+- Don't forget to update your git submodules when checking out.
+### Input
+The following diagram defines (roughly) a state machine for a CD player.
+
+<!---![Image of CD Player](kojen/docs/images/StateMachine.PNG)--->
+
+![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/StateMachine.PNG)
+
+This state machine can be represented by the following transition table in python (format : 'startstate', 'event', 'nextstate', 'action', 'guard'):
+
+```python
+#
+# StartState    Event                     NextState     Action                 Guard
+#
+ 'StateStop',  'EventOpen',              'StateOpen',  'OnOpenDrive',         'None'
+ 'StateStop',  'EventPlay',              'StatePlay',  'OnPlayTrack',         'GuardCDInside'
+ 'StateOpen',  'EventOpen',              'StateStop',  'OnCloseDrive',        'None'
+ 'StatePlay',  'EventPlay',              'StatePause', 'OnPause',             'None'
+ 'StatePlay',  'EventEndOfTrack',        'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'
+ 'StatePlay',  'EventEndOfTrack',        'StateStop',  'OnStop',              'GuardCDHasNoMoreTracks'
+ 'StatePlay',  'EventSkipNextTrack',     'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'
+ 'StatePlay',  'EventSkipPreviousTrack', 'None',       'OnPlayPreviousTrack', 'GuardCDHasPreviousTrack'
+ 'StatePlay',  'EventStop',              'StateStop',  'OnStop',              'None'
+ 'StatePause', 'EventPlay',              'StatePlay',  'OnPlayTrack',         'None'
+ 'StatePause', 'EventAfter10Minutes',    'StateStop',  'OnStop',              'None'
+```
+
+Create a file `Generate.py` (or add your state machine to the one already present in your project) :
+
+```python
+from kojen import Generate
+from kojen.kojentypes import *
+
+#
+# Generate Statemachine (from TransitionTable)
+#
+
+# For playing a track the tracknumber should be parameterized.
+EventPlay = Struct('EventPlay')
+EventPlay.AddType('m_track_no','uint16_t')
+
+eventsinterface = Interface('params')
+eventsinterface.AddStruct(EventPlay)
+
+# Optional features
+eventsinterface.AddUserTag("StateMachineThread", 1) # 0 = SM runs on caller thread, 1 = SM runs on its own thread. Default is 1.
+eventsinterface.AddUserTag("Verbose", 1)            # 0 = No printouts, 1 = printouts. Default is 1.
+
+# Transition Table.
+transition_table = []
+#                         StartState    Event                     NextState     Action                 Guard
+transition_table.append(['StateStop',  'EventOpen',              'StateOpen',  'OnOpenDrive',         'None'                   ])
+transition_table.append(['StateStop',  'EventPlay',              'StatePlay',  'OnPlayTrack',         'GuardCDInside'          ]) 
+transition_table.append(['StateOpen',  'EventOpen',              'StateStop',  'OnCloseDrive',        'None'                   ]) 
+transition_table.append(['StatePlay',  'EventPlay',              'StatePause', 'OnPause',             'None'                   ])
+transition_table.append(['StatePlay',  'EventEndOfTrack',        'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'   ])
+transition_table.append(['StatePlay',  'EventEndOfTrack',        'StateStop',  'OnStop',              'GuardCDHasNoMoreTracks' ])
+transition_table.append(['StatePlay',  'EventSkipNextTrack',     'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'   ]) 
+transition_table.append(['StatePlay',  'EventSkipPreviousTrack', 'None',       'OnPlayPreviousTrack', 'GuardCDHasPreviousTrack'])
+transition_table.append(['StatePlay',  'EventStop',              'StateStop',  'OnStop',              'None'                   ])
+transition_table.append(['StatePause', 'EventPlay',              'StatePlay',  'OnPlayTrack',         'None'                   ])
+transition_table.append(['StatePause', 'EventAfter10Minutes',    'StateStop',  'OnStop',              'None'                   ])
+
+author = "myname@mydomain.com"
+group  = "MY_PACKAGE"
+brief  = "An example demonstrating state-machine code-generation abilities."
+
+eventsinterface = None
+namespacename = "CDPlayerSM"
+statemachinenameprefix = "CDPlayer"
+declspec = ""
+outputdir = "autogen/state_machine"
+templatedir = "" # defaults are for 'SML'
+Generate.StateMachine(outputdir, transition_table, eventsinterface, namespacename, statemachinenameprefix, declspec, author, group, brief, templatedir)
+```
+
+Execute `Generate.py` using python. Your C++ code should be generated to the configured folder **./autogen/state_machine**.
+
+> **Please note** : you may may wish to parameterize events in your statemachine. An event is of type `kojen.Struct` in a `kojen.Interface` object. 
+> Simply follow the quickstart for protocols, creating and returning an interface : your Event structs need to have the exact same name as defined in the transition table.
+> You should thus pass your interface object  as the *eventsinterface* argument to the generator instead of **None**.
+
+### Output
+
+There will be several files in the output folder.
+
+* allplatforms *(folder containing framework files for standalone solution)*
+* CDPlayerStateMachine.h
+* CDPlayerStateMachineImpl_SML.cpp *(all state machine code generated for boost-sml)*  
+* ICDPlayerController.h
+* Test.CDPlayerStateMachine.cpp
+  
+The following class diagram explains roughly where focus should be when implementing for test-driven development as well as for actual integration into the real system.
+
+<!---![Image of necessary classes](kojen/docs/images/StateMachineClassDiagram.PNG)--->
+![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/StateMachineClassDiagram.PNG)
+
+White classes are auto-generated, and have code-preservation features. Grey is what you have to manually create, and implement for integration into your real system.
+
+All required functionality for your system should be implemented in the **Controller** classes, being the base-class *ICDPlayerController*, the derived *C_My_CDPlayerController* and the derived test class *CTestCDPlayerController*.
+
+It is critical that as much of the 'business logic' is put into the base class *IPlayerController*, and tested using the *CTestCDPlayerController* in the unit-tests as possible, such that the actual integrated *C_My_CDPlayerController* uses unit-tested business logic, with a good example of how its intended to work in the unit tests...as well as for regression testing and continuous integration.
+
+As the state-machine-implementation uses the controller base class, the following construction is valid for unit tests and system integration by substituting the correct controller:
+
+```cplusplus
+  CTestCDPlayerController controller;
+  auto* sm = ICDPlayerStateMachine::Create(controller);
+```
+
+All state queries and event triggering are done using the ```sm``` instance.
+
+Due to the use of move-semantics, parameterized event structs are unique_ptr's (allocated in fixed-blocks for embedded applications) and thus once an event is triggered those pointers are no longer valid in the calling context.
+
+## State Machine in C#
+
+Similar to the above example, the only difference is the Generate call to use.
+
+```python
+   ...
+   Generate.StateMachine_CSHARP(...)
+   ...
+```
+
+## State Machine in Python
+
+Similar to the above example, the only difference is the Generate call to use.
+
+```python
+    ...
+   Generate.StateMachine_PYTHON(...)
+   ...
+```
+
+<!---
+### Deferred Events
+
+Deferred events are supported in SML and MSM state machines.
+
+In the example CD player statemachine this use-case could be pressing 'play' whilst the tray is closing : the close button will be pressed, and the tray will start closing, however the software trigger for *EventOpen* will only occur on the interrupt signalling that the tray actuator has completed either opening/closing the tray. 
+This can take up to several seconds. In that time, the 'play' button could be pressed. 
+
+The desired behaviour would be that once the tray is closed, the CD starts playing.
+
+This can be achieved by manually adding the correct deferred event in the *CDPlayerStateMachineImpl_SML.cpp* in the code preservation tags at the end of the transition table:
+
+```cplusplus
+/// {{{USER_DEFERRED_EVENTS}}}
+, StateOpen + event<EventPlay> / defer
+/// {{{USER_DEFERRED_EVENTS}}}
+```
+
+For *boost::msm* this can be achieved by manually adding the correct deferred event in code preservation tags in the state struct for *StateOpen* in *CDPlayerStateMachineImpl_SML.cpp* :
+
+```cplusplus
+/// {{{USER_StateOpen_DEFERRED_EVENTS}}}
+typedef boost::mpl::vector<EventPlay> deferred_events;
+/// {{{USER_StateOpen_DEFERRED_EVENTS}}} 
+```
+
+I believe this will also allow the sequence of 'play' then 'close' to work.
+--->
+
+
```

### Comparing `kojen-1.2.30/kojen/Generate.py` & `kojen-1.3.31/kojen/Generate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #!/usr/bin/env python3
 try:
-    from . import protogen, smgen, umlgen, coggen, vppfs, LanguageCPP, LanguageCsharp, LanguagePython, cgen
+    from . import protogen, smgen, umlgen, coggen, vppfs, LanguageCPP, LanguageCsharp, LanguagePython, cgen, Install
 except:
-    import protogen, smgen, umlgen, coggen, vppfs, LanguageCPP, LanguageCsharp, LanguagePython, cgen
+    import protogen, smgen, umlgen, coggen, vppfs, LanguageCPP, LanguageCsharp, LanguagePython, cgen, Install
 
 import os
 
-''' Generate Entry function for Protocols. 
+''' Generate Entry function for Protocols.
 '''
 
 
 #def Protocol(output_dir, pythoninterfacegeneratorfilename, namespacename, classname, declspec="", author = "", group="", brief="", template_dir="") -> list:
 #    return protogen.Generate(output_dir, pythoninterfacegeneratorfilename, namespacename, classname, declspec, author, group, brief, template_dir)
 
 def Protocol(outputdir, eventsinterface, namespacenname, classname, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir) and templatedir.strip():
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
     if not templatedir.strip():
         templatedir = os.path.join(os.path.join(os.path.abspath(os.path.dirname(__file__)), "protocol_templates"), "CPP")
     res =  StateMachine(outputdir, [], eventsinterface, namespacenname, classname, dclspc, author, group, brief, templatedir, __internal, False)
     if __copy_other_files:
         protogen.CopyFrameworkFiles_CPP(outputdir)
     return res
 
@@ -25,74 +29,99 @@
 
 
 ''' Generate Entry function for State Machines
 '''
 
 
 def StateMachine(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir) and templatedir.strip():
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
+
     if not templatedir.strip():
         templatedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "statemachine_templates_embedded_arm")
 
     if not os.path.isdir(templatedir) and not os.path.isfile(templatedir):
-        print("Error : dir '" + templatedir + "' does not exist. Aborting.")
+        print("Error : path '" + templatedir + "' does not exist. Aborting.")
         return
 
     language = LanguageCPP.LanguageCPP()
     smgenerator = smgen.CStateMachineGenerator(templatedir, outputdir, eventsinterface, language, author, group, brief)
     if not __internal:
         smgenerator.vpp_filename = "Transition Table"
     else:
         smgenerator.vpp_filename = __internal
     return smgenerator.Generate(transition_table, namespacenname, statemachinenameprefix, dclspc, __copy_other_files)
 
 
 def StateMachine_CSHARP(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir) and templatedir.strip():
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
+
     if not templatedir.strip():
         templatedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "statemachine_templates_cs_winlinmac")
 
     if not os.path.isdir(templatedir) and not os.path.isfile(templatedir):
-        print("Error : dir '" + templatedir + "' does not exist. Aborting.")
+        print("Error : path '" + templatedir + "' does not exist. Aborting.")
         return []
 
     language = LanguageCsharp.LanguageCsharp()
     smgenerator = smgen.CStateMachineGenerator(templatedir, outputdir, eventsinterface, language, author, group, brief)
     if not __internal:
         smgenerator.vpp_filename = "Transition Table"
     else:
         smgenerator.vpp_filename = __internal
     return smgenerator.Generate(transition_table, namespacenname, statemachinenameprefix, dclspc, __copy_other_files)
 
 
 def StateMachine_PYTHON(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir) and templatedir.strip():
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
+
     if not templatedir.strip():
         templatedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "statemachine_templates_py")
 
     if not os.path.isdir(templatedir) and not os.path.isfile(templatedir):
-        print("Error : dir '" + templatedir + "' does not exist. Aborting.")
+        print("Error : path '" + templatedir + "' does not exist. Aborting.")
         return []
 
     language = LanguagePython.LanguagePython()
     smgenerator = smgen.CStateMachineGenerator(templatedir, outputdir, eventsinterface, language, author, group, brief)
     if not __internal:
         smgenerator.vpp_filename = "Transition Table"
     else:
         smgenerator.vpp_filename = __internal
     return smgenerator.Generate(transition_table, namespacenname, statemachinenameprefix, dclspc, __copy_other_files)
 
 
 def StateMachineFromModel(outputdir, vp_project_path, vp_statemachinename, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir) and templatedir.strip():
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
+
     transition_table = vppfs.ExtractTransitionTable(vp_statemachinename, vp_project_path)
     return StateMachine(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc, author, group, brief, templatedir, os.path.basename(vp_project_path),__copy_other_files)
 
 
 ''' Generate Entry function for Class Diagrams
 '''
 
 
 def UML(outputdir, vp_project_path, vp_classdiagramname, dclspc="", author="", group="", brief="", namespace_to_folders=False, templatefiledir="") -> list:
+    if not os.path.isabs(templatefiledir):
+        # Is it a user template?
+        if Install.ContainsTemplates(templatefiledir):
+            templatefiledir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatefiledir))
+
     language = LanguageCPP.LanguageCPP()
     return umlgen.Generate(vp_project_path, vp_classdiagramname, outputdir, language, author, group, brief, namespace_to_folders, dclspc, templatefiledir)
 
 def UML_CSHARP(outputdir, vp_project_path, vp_classdiagramname, dclspc="", author="", group="", brief="", namespace_to_folders=False, templatefiledir="") -> list:
     language = LanguageCsharp.LanguageCsharp()
     return umlgen.Generate(vp_project_path, vp_classdiagramname, outputdir, language, author, group, brief, namespace_to_folders, dclspc, templatefiledir)
```

### Comparing `kojen-1.2.30/kojen/Language.py` & `kojen-1.3.31/kojen/Language.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/LanguageCPP.py` & `kojen-1.3.31/kojen/LanguageCPP.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/LanguageCsharp.py` & `kojen-1.3.31/kojen/LanguageCsharp.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/LanguagePython.py` & `kojen-1.3.31/kojen/LanguagePython.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/cgen.py` & `kojen-1.3.31/kojen/cgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 '''
 
 ''' This forms the base for some sorts of code generation.
 
     Step 1) Load template files to memory
     Step 2) Search and replace passed-in tags in memory (including filenames).
-    
+
 '''
 
 __TAG_DATETIME__           = '<<<DATETIME>>>'
 __TAG_PLATFORM__           = '<<<PLATFORM>>>'
 __TAG_EXTENDS__            = '<<<EXTENDS>>>'
 __TAG_EXCLUDE__            = '<<<EXCLUDE>>>'
 __TAG_FOR_BEGIN__          = "<<<FOR_BEGIN>>>"
@@ -601,17 +601,17 @@
     """
     try:
         os.makedirs(dir_to, exist_ok=True)
         for filename in list_of_filenames:
             try:
                 shutil.copy(os.path.join(dir_from, filename), os.path.join(dir_to, filename))
             except OSError:
-                warnings.warn("Copy of the file %s failed" % os.path.join(dir_from, filename))
+                warning("Copy of the file %s failed" % os.path.join(dir_from, filename))
     except OSError:
-        warnings.warn("Creation of the directory %s failed" % dir_to)
+        warning("Creation of the directory %s failed" % dir_to)
 
 def FilePreservationSyncUtil(file_from, file_to) -> None:
     """
     Will synchronize code in preservation tags from 'file_from' to 'file_to',
     if these tags exist in 'file_to'.
 
     Tags that exist exclusively in 'file_to' will remain untouched if they do not
```

### Comparing `kojen-1.2.30/kojen/coggen.py` & `kojen-1.3.31/kojen/coggen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/kojentypes.py` & `kojen-1.3.31/kojen/kojentypes.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/plant.py` & `kojen-1.3.31/kojen/plant.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/preservative.py` & `kojen-1.3.31/kojen/preservative.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/protogen.py` & `kojen-1.3.31/kojen/protogen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/smgen.py` & `kojen-1.3.31/kojen/smgen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/smvppxml.py` & `kojen-1.3.31/kojen/smvppxml.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/cgen_test.py` & `kojen-1.3.31/kojen/test/cgen_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/preservative_test.py` & `kojen-1.3.31/kojen/test/preservative_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/smgen_test.py` & `kojen-1.3.31/kojen/test/smgen_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/vppclassdiagram_test.py` & `kojen-1.3.31/kojen/test/vppclassdiagram_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/vppfs_test.py` & `kojen-1.3.31/kojen/test/vppfs_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/umlgen.py` & `kojen-1.3.31/kojen/umlgen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/vppclassdiagram.py` & `kojen-1.3.31/kojen/vppclassdiagram.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/vppfs.py` & `kojen-1.3.31/kojen/vppfs.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen.egg-info/PKG-INFO` & `kojen-1.3.31/kojen.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,330 +1,333 @@
 Metadata-Version: 2.1
 Name: kojen
-Version: 1.2.30
+Version: 1.3.31
 Summary: Code generation tools.
 Home-page: https://github.com/kohjaen/kojen
 Author: kohjaen
 Author-email: koh.jaen@yahoo.de
 License: UNKNOWN
-Description: ![CI](https://github.com/kohjaen/kojen/workflows/CI/badge.svg)
-        
-        # Description
-        
-        Kojen is a protocol (C++), state-machine(C++/C#/Python) and Class (C++/C# from UML) code-generation tool written in Python and existing within the Python Package Index (PyPi). Python >= 3.6.8 is supported. To install run ```python -m pip install kojen```.  
-        
-        The default generated state-machine uses the fast and lightweight single-header-file-only [boost sml](https://boost-ext.github.io/sml/). It is linked to the repository as a git sub-module for an out-the-box solution. This is suitable for both embedded and PC applications using C++14 and higher.
-        
-        For state-machines and software-architecture-from-UML-model : user-code is preserved within special comment tags. Should you change the name of tags that had code within them, on the next generation a new text file prepended with ```.Lostcode``` will be output next to the original source file with all the code that was lost. The main concept is that code-generation is a manually-initiated process and exists within a hand-crafted source-repository. The intention is to be able to manually program in all auto-generated state-machine / Class Diagram output source files, and preserve hand-crafted code within those files when system requirements change. Its not intended to disassociate the programmer from the code (like most CASE tools). Typically after the Design phase code-generation is done first in the initial implementation phase (and maybe a few more times until things are as they should be) and then development is done the usual way. Naturally in time further changes/additions can be done in the model (Updating the 'diagrams' first) and their changes propagated to code by generation : this also allows for updates to the design (from Model -> Code) in a non-intrusive manner. Protocols and their unit tests are the only files which require no hand-coding.
-        
-        Unit testing : Tests for protocols are generated, and tests for state-machines too (but those require some hand-coding, code preservation applies). The included testing framework is extremely light-weight and great for embedded (and PC) applications : [minunit](https://github.com/kohjaen/minunit) is used for this and it is also linked to the repository as a git sub-module. The original fork of minunit is a C-based single header file, but some improvements have been made (not possible with C) so it now consists of a single header and a single cpp file. It contains a test-runner which will run all registered test-suites.
-        
-        It currently supports Windows/Linux/MacOS and FreeRTOS and includes multi-threading components (threads/queues/dispatchers/fixed-block-memory-allocators as well as stl-with-fixed-block-mem-allocator wrappers for no spurious heap usage and much faster STL containers) that works on all platforms by including CMake configuration files in generated outputs.
-        
-        Message Queues use move-semantics and are thus platform independant and adding a new RTOS will only require adding a 'condition variable' like synchronization mechanism for that RTOS (the provided example of how it is done with FreeRTOS can be followed).
-        
-        # Quickstart
-        ## Example folder
-        
-        The git repository has a fully functional example (which is used in the CI), including CMake integration. An executable is generated and that runs all unit tests. Feel free to go straight there. The example is described below.
-        
-        ## Protocol
-        ### Input
-        In a folder where you will execute your project from, create the interface definition file `MyInterface.py`.
-        
-        In your interface definition file `MyInterface.py` create a function `CreateInterface()` that returns a  `kojen.Interface` object. 
-        
-        Here is an example of what is permissible in an interface. For messages, make sure each has a unique message-id (second parameter after the name in the constructor)
-        ```python
-        from kojen.kojentypes import *
-        
-        def CreateInterface():
-            sCustomStruct = Struct('sCustomStruct')
-            sCustomStruct.AddType('m_Member1','uint16')
-            sCustomStruct.AddType('m_Member2','uint16')
-            sCustomStruct.AddType('m_Member3','uint32')
-        
-            MsgSomeCMD = Message('MsgSomeCMD',0x01)
-            MsgSomeCMD.AddType('m_Member1','uint8')
-        
-            MsgSomeCMDRSP = Message('MsgSomeCMDRSP',0x02)
-            MsgSomeCMDRSP.AddStruct('mStructMember1',sCustomStruct)
-            MsgSomeCMDRSP.AddType('m_Member2','uint8')
-            
-            MsgSomeREQ = Message('MsgSomeREQ',0x03)
-            MsgSomeREQ.AddType('m_Member1','uint8')
-        
-            #Array of type : Not supported by ARM due to dynamic memory allocation requirements
-            MsgSomeREQRSP = Message('MsgSomeREQRSP',0x04)
-            MsgSomeREQRSP.AddStruct('mStructMember1',sCustomStruct)
-            MsgSomeREQRSP.AddType('m_Member2','uint8')
-            MsgSomeREQRSP.AddArrayOfType('mArrayMember3','double')
-        
-        
-            MsgSomeUnsolicitedData = Message('MsgSomeUnsolicitedData',0x05)
-            MsgSomeUnsolicitedData.AddArrayOfStruct('mStructArrayMember1',sCustomStruct)
-        
-            #
-            # Includes : Enums and defines ...
-            #
-            Type = Enum("Type")
-            Type.Add("kOne", 0)
-            Type.Add("kTwo", 1)
-        
-            Revision = Enum("Revision")
-            Revision.Add("kVersion1", 0)
-            Revision.Add("kVersion2", 1)
-            Revision.Add("kVersion3", 2)
-        
-            interface = Interface('IMyInterfaceIO')
-        
-            interface.AddEnum(Type)
-            interface.AddEnum(Revision)
-        
-            interface.AddHashDefine("THREE", 3)
-            interface.AddHashDefine("PI", 3.14159265359)
-        
-            interface.AddStruct(sCustomStruct)
-            interface.AddMessage(MsgSomeCMD)
-            interface.AddMessage(MsgSomeCMDRSP)
-            interface.AddMessage(MsgSomeREQ)
-            interface.AddMessage(MsgSomeREQRSP)
-            interface.AddMessage(MsgSomeUnsolicitedData)
-        
-            return interface
-        ```
-        
-        Then, create a file `Generate.py`.
-        
-        
-        ```python
-        import kojen.Generate as Generate
-        import os
-        
-        author = "myname@mydomain.com"
-        group  = "MY_PACKAGE"
-        brief  = "An example demonstrating protocol code-generation abilities."
-        namespacename = "ExampleIO"
-        classname = "CExampleIF"
-        declspec = "" # your define for symbol export/import in C++ e.g. MY_PROJECT_API
-        outputdir = os.path.join(os.path.abspath(os.path.dirname(__file__)), os.path.join("autogen","protocol"))
-        protocolfile = os.path.join(os.path.abspath(os.path.dirname(__file__)), "MyInterface.py")
-        Generate.Protocol(outputdir, protocolfile, namespacename, classname, declspec, author, group, brief)
-        ```
-        
-        Execute `Generate.py` using python. Your C++ code should be in the folder **./autogen/protocol**.
-        
-        > **Please note** : you may include this code in a library, and thus want to export some of the generated features.
-        > Typically somewhere in a common header of your C++ code, you would have declared something like
-        
-        ```cplusplus
-        #ifdef MY_PROJECT_EXPORTS
-        #	define MY_PROJECT_API __declspec(dllexport)
-        #else
-        #	define MY_PROJECT_API __declspec(dllimport)
-        #endif
-        ```
-        
-        > You should thus pass **MY_PROJECT_API** as the *declspec* argument to the generator.
-        
-        ### Output
-        
-        There will be several files in the output folder.
-        
-        * allplatforms *(folder containing required framework files)*
-        * CExampleIF.h *(contains all factories to create messages which automatically and correctly fill in the headers, as well as serialization to/from bytestreams.)
-        * CExampleIF.cpp
-        * CExampleIFDefines.h *(contains all enums and defines)
-        * CExampleIFReceiver.h *(contains a derivable class that received fully constructed messages. Override receive functions to handle them as per need.)
-        * CExampleIFReceiver.cpp
-        * CExampleIFStructs.h *(contains all structs)
-        * CExampleIFTests.cpp *(contains all unit tests)
-        * CExampleIFTransmitter.h *(contains all functions to transmit fully constructed messages. Highly advices to use the autogenerated factories.)
-        * CExampleIFTransmitter.cpp
-        * MsgHeader.h
-        
-        The following class diagram explains roughly where focus should be when implementing for actual integration into the real system.
-        
-        <!---![Image of necessary classes](kojen/docs/images/ProtocolClassDiagram.PNG) ... doesnt work on PyPi!--->
-        ![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/ProtocolClassDiagram.PNG)
-        
-        *IConnection* is the interface to derive from for your actual physical layer for an embedded platform. If you use boost on x86/x64, in the 'allplatforms' directory exist classes for substituting this with a TCPConnection, UDPConnection and SerialPort.
-        Have a good look at the unit tests, this shows roughly how to derive from it and connect everything up, albeit creating a loopback connection, and implementing uncessary routing as the interface for the tests have a special requirement.
-        
-        A summary to link it up:
-        * Create a derived IConnection that knows how to send and receive physical layer data.
-        * Create a generated Transmitter, passing it a pointer to this connection.
-        * Create a generated Receiver
-        * Set the Receiver to the derived IConnection. You will then get messages in the message receiving functions...override the correct ones to handle them.
-        * Use the Transmitter to send.
-        
-        ## State Machine in C++
-        ### Requrements
-        - Don't forget to update your git submodules when checking out.
-        ### Input
-        The following diagram defines (roughly) a state machine for a CD player.
-        
-        <!---![Image of CD Player](kojen/docs/images/StateMachine.PNG)--->
-        
-        ![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/StateMachine.PNG)
-        
-        This state machine can be represented by the following transition table in python (format : 'startstate', 'event', 'nextstate', 'action', 'guard'):
-        
-        ```python
-        #
-        # StartState    Event                     NextState     Action                 Guard
-        #
-         'StateStop',  'EventOpen',              'StateOpen',  'OnOpenDrive',         'None'
-         'StateStop',  'EventPlay',              'StatePlay',  'OnPlayTrack',         'GuardCDInside'
-         'StateOpen',  'EventOpen',              'StateStop',  'OnCloseDrive',        'None'
-         'StatePlay',  'EventPlay',              'StatePause', 'OnPause',             'None'
-         'StatePlay',  'EventEndOfTrack',        'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'
-         'StatePlay',  'EventEndOfTrack',        'StateStop',  'OnStop',              'GuardCDHasNoMoreTracks'
-         'StatePlay',  'EventSkipNextTrack',     'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'
-         'StatePlay',  'EventSkipPreviousTrack', 'None',       'OnPlayPreviousTrack', 'GuardCDHasPreviousTrack'
-         'StatePlay',  'EventStop',              'StateStop',  'OnStop',              'None'
-         'StatePause', 'EventPlay',              'StatePlay',  'OnPlayTrack',         'None'
-         'StatePause', 'EventAfter10Minutes',    'StateStop',  'OnStop',              'None'
-        ```
-        
-        Create a file `Generate.py` (or add your state machine to the one already present in your project) :
-        
-        ```python
-        from kojen import Generate
-        from kojen.kojentypes import *
-        
-        #
-        # Generate Statemachine (from TransitionTable)
-        #
-        
-        # For playing a track the tracknumber should be parameterized.
-        EventPlay = Struct('EventPlay')
-        EventPlay.AddType('m_track_no','uint16_t')
-        
-        eventsinterface = Interface('params')
-        eventsinterface.AddStruct(EventPlay)
-        
-        # Optional features
-        eventsinterface.AddUserTag("StateMachineThread", 1) # 0 = SM runs on caller thread, 1 = SM runs on its own thread. Default is 1.
-        eventsinterface.AddUserTag("Verbose", 1)            # 0 = No printouts, 1 = printouts. Default is 1.
-        
-        # Transition Table.
-        transition_table = []
-        #                         StartState    Event                     NextState     Action                 Guard
-        transition_table.append(['StateStop',  'EventOpen',              'StateOpen',  'OnOpenDrive',         'None'                   ])
-        transition_table.append(['StateStop',  'EventPlay',              'StatePlay',  'OnPlayTrack',         'GuardCDInside'          ]) 
-        transition_table.append(['StateOpen',  'EventOpen',              'StateStop',  'OnCloseDrive',        'None'                   ]) 
-        transition_table.append(['StatePlay',  'EventPlay',              'StatePause', 'OnPause',             'None'                   ])
-        transition_table.append(['StatePlay',  'EventEndOfTrack',        'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'   ])
-        transition_table.append(['StatePlay',  'EventEndOfTrack',        'StateStop',  'OnStop',              'GuardCDHasNoMoreTracks' ])
-        transition_table.append(['StatePlay',  'EventSkipNextTrack',     'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'   ]) 
-        transition_table.append(['StatePlay',  'EventSkipPreviousTrack', 'None',       'OnPlayPreviousTrack', 'GuardCDHasPreviousTrack'])
-        transition_table.append(['StatePlay',  'EventStop',              'StateStop',  'OnStop',              'None'                   ])
-        transition_table.append(['StatePause', 'EventPlay',              'StatePlay',  'OnPlayTrack',         'None'                   ])
-        transition_table.append(['StatePause', 'EventAfter10Minutes',    'StateStop',  'OnStop',              'None'                   ])
-        
-        author = "myname@mydomain.com"
-        group  = "MY_PACKAGE"
-        brief  = "An example demonstrating state-machine code-generation abilities."
-        
-        eventsinterface = None
-        namespacename = "CDPlayerSM"
-        statemachinenameprefix = "CDPlayer"
-        declspec = ""
-        outputdir = "autogen/state_machine"
-        templatedir = "" # defaults are for 'SML'
-        Generate.StateMachine(outputdir, transition_table, eventsinterface, namespacename, statemachinenameprefix, declspec, author, group, brief, templatedir)
-        ```
-        
-        Execute `Generate.py` using python. Your C++ code should be generated to the configured folder **./autogen/state_machine**.
-        
-        > **Please note** : you may may wish to parameterize events in your statemachine. An event is of type `kojen.Struct` in a `kojen.Interface` object. 
-        > Simply follow the quickstart for protocols, creating and returning an interface : your Event structs need to have the exact same name as defined in the transition table.
-        > You should thus pass your interface object  as the *eventsinterface* argument to the generator instead of **None**.
-        
-        ### Output
-        
-        There will be several files in the output folder.
-        
-        * allplatforms *(folder containing framework files for standalone solution)*
-        * CDPlayerStateMachine.h
-        * CDPlayerStateMachineImpl_SML.cpp *(all state machine code generated for boost-sml)*  
-        * ICDPlayerController.h
-        * Test.CDPlayerStateMachine.cpp
-          
-        The following class diagram explains roughly where focus should be when implementing for test-driven development as well as for actual integration into the real system.
-        
-        <!---![Image of necessary classes](kojen/docs/images/StateMachineClassDiagram.PNG)--->
-        ![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/StateMachineClassDiagram.PNG)
-        
-        White classes are auto-generated, and have code-preservation features. Grey is what you have to manually create, and implement for integration into your real system.
-        
-        All required functionality for your system should be implemented in the **Controller** classes, being the base-class *ICDPlayerController*, the derived *C_My_CDPlayerController* and the derived test class *CTestCDPlayerController*.
-        
-        It is critical that as much of the 'business logic' is put into the base class *IPlayerController*, and tested using the *CTestCDPlayerController* in the unit-tests as possible, such that the actual integrated *C_My_CDPlayerController* uses unit-tested business logic, with a good example of how its intended to work in the unit tests...as well as for regression testing and continuous integration.
-        
-        As the state-machine-implementation uses the controller base class, the following construction is valid for unit tests and system integration by substituting the correct controller:
-        
-        ```cplusplus
-          CTestCDPlayerController controller;
-          auto* sm = ICDPlayerStateMachine::Create(controller);
-        ```
-        
-        All state queries and event triggering are done using the ```sm``` instance.
-        
-        Due to the use of move-semantics, parameterized event structs are unique_ptr's (allocated in fixed-blocks for embedded applications) and thus once an event is triggered those pointers are no longer valid in the calling context.
-        
-        ## State Machine in C#
-        
-        Similar to the above example, the only difference is the Generate call to use.
-        
-        ```python
-           ...
-           Generate.StateMachine_CSHARP(...)
-           ...
-        ```
-        
-        ## State Machine in Python
-        
-        Similar to the above example, the only difference is the Generate call to use.
-        
-        ```python
-            ...
-           Generate.StateMachine_PYTHON(...)
-           ...
-        ```
-        
-        <!---
-        ### Deferred Events
-        
-        Deferred events are supported in SML and MSM state machines.
-        
-        In the example CD player statemachine this use-case could be pressing 'play' whilst the tray is closing : the close button will be pressed, and the tray will start closing, however the software trigger for *EventOpen* will only occur on the interrupt signalling that the tray actuator has completed either opening/closing the tray. 
-        This can take up to several seconds. In that time, the 'play' button could be pressed. 
-        
-        The desired behaviour would be that once the tray is closed, the CD starts playing.
-        
-        This can be achieved by manually adding the correct deferred event in the *CDPlayerStateMachineImpl_SML.cpp* in the code preservation tags at the end of the transition table:
-        
-        ```cplusplus
-        /// {{{USER_DEFERRED_EVENTS}}}
-        , StateOpen + event<EventPlay> / defer
-        /// {{{USER_DEFERRED_EVENTS}}}
-        ```
-        
-        For *boost::msm* this can be achieved by manually adding the correct deferred event in code preservation tags in the state struct for *StateOpen* in *CDPlayerStateMachineImpl_SML.cpp* :
-        
-        ```cplusplus
-        /// {{{USER_StateOpen_DEFERRED_EVENTS}}}
-        typedef boost::mpl::vector<EventPlay> deferred_events;
-        /// {{{USER_StateOpen_DEFERRED_EVENTS}}} 
-        ```
-        
-        I believe this will also allow the sequence of 'play' then 'close' to work.
-        --->
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![CI](https://github.com/kohjaen/kojen/workflows/CI/badge.svg)
+
+# Description
+
+Kojen is a protocol (C++), state-machine(C++/C#/Python) and Class (C++/C# from UML) code-generation tool written in Python and existing within the Python Package Index (PyPi). Python >= 3.6.8 is supported. To install run ```python -m pip install kojen```.  
+
+The default generated state-machine uses the fast and lightweight single-header-file-only [boost sml](https://boost-ext.github.io/sml/). It is linked to the repository as a git sub-module for an out-the-box solution. This is suitable for both embedded and PC applications using C++14 and higher.
+
+For state-machines and software-architecture-from-UML-model : user-code is preserved within special comment tags. Should you change the name of tags that had code within them, on the next generation a new text file prepended with ```.Lostcode``` will be output next to the original source file with all the code that was lost. The main concept is that code-generation is a manually-initiated process and exists within a hand-crafted source-repository. The intention is to be able to manually program in all auto-generated state-machine / Class Diagram output source files, and preserve hand-crafted code within those files when system requirements change. Its not intended to disassociate the programmer from the code (like most CASE tools). Typically after the Design phase code-generation is done first in the initial implementation phase (and maybe a few more times until things are as they should be) and then development is done the usual way. Naturally in time further changes/additions can be done in the model (Updating the 'diagrams' first) and their changes propagated to code by generation : this also allows for updates to the design (from Model -> Code) in a non-intrusive manner. Protocols and their unit tests are the only files which require no hand-coding.
+
+Unit testing : Tests for protocols are generated, and tests for state-machines too (but those require some hand-coding, code preservation applies). The included testing framework is extremely light-weight and great for embedded (and PC) applications : [minunit](https://github.com/kohjaen/minunit) is used for this and it is also linked to the repository as a git sub-module. The original fork of minunit is a C-based single header file, but some improvements have been made (not possible with C) so it now consists of a single header and a single cpp file. It contains a test-runner which will run all registered test-suites.
+
+It currently supports Windows/Linux/MacOS and FreeRTOS and includes multi-threading components (threads/queues/dispatchers/fixed-block-memory-allocators as well as stl-with-fixed-block-mem-allocator wrappers for no spurious heap usage and much faster STL containers) that works on all platforms by including CMake configuration files in generated outputs.
+
+Message Queues use move-semantics and are thus platform independant and adding a new RTOS will only require adding a 'condition variable' like synchronization mechanism for that RTOS (the provided example of how it is done with FreeRTOS can be followed).
+
+# Quickstart
+## Example folder
+
+The git repository has a fully functional example (which is used in the CI), including CMake integration. An executable is generated and that runs all unit tests. Feel free to go straight there. The example is described below.
+
+## Protocol
+### Input
+In a folder where you will execute your project from, create the interface definition file `MyInterface.py`.
+
+In your interface definition file `MyInterface.py` create a function `CreateInterface()` that returns a  `kojen.Interface` object. 
+
+Here is an example of what is permissible in an interface. For messages, make sure each has a unique message-id (second parameter after the name in the constructor)
+```python
+from kojen.kojentypes import *
+
+def CreateInterface():
+    sCustomStruct = Struct('sCustomStruct')
+    sCustomStruct.AddType('m_Member1','uint16')
+    sCustomStruct.AddType('m_Member2','uint16')
+    sCustomStruct.AddType('m_Member3','uint32')
+
+    MsgSomeCMD = Message('MsgSomeCMD',0x01)
+    MsgSomeCMD.AddType('m_Member1','uint8')
+
+    MsgSomeCMDRSP = Message('MsgSomeCMDRSP',0x02)
+    MsgSomeCMDRSP.AddStruct('mStructMember1',sCustomStruct)
+    MsgSomeCMDRSP.AddType('m_Member2','uint8')
+    
+    MsgSomeREQ = Message('MsgSomeREQ',0x03)
+    MsgSomeREQ.AddType('m_Member1','uint8')
+
+    #Array of type : Not supported by ARM due to dynamic memory allocation requirements
+    MsgSomeREQRSP = Message('MsgSomeREQRSP',0x04)
+    MsgSomeREQRSP.AddStruct('mStructMember1',sCustomStruct)
+    MsgSomeREQRSP.AddType('m_Member2','uint8')
+    MsgSomeREQRSP.AddArrayOfType('mArrayMember3','double')
+
+
+    MsgSomeUnsolicitedData = Message('MsgSomeUnsolicitedData',0x05)
+    MsgSomeUnsolicitedData.AddArrayOfStruct('mStructArrayMember1',sCustomStruct)
+
+    #
+    # Includes : Enums and defines ...
+    #
+    Type = Enum("Type")
+    Type.Add("kOne", 0)
+    Type.Add("kTwo", 1)
+
+    Revision = Enum("Revision")
+    Revision.Add("kVersion1", 0)
+    Revision.Add("kVersion2", 1)
+    Revision.Add("kVersion3", 2)
+
+    interface = Interface('IMyInterfaceIO')
+
+    interface.AddEnum(Type)
+    interface.AddEnum(Revision)
+
+    interface.AddHashDefine("THREE", 3)
+    interface.AddHashDefine("PI", 3.14159265359)
+
+    interface.AddStruct(sCustomStruct)
+    interface.AddMessage(MsgSomeCMD)
+    interface.AddMessage(MsgSomeCMDRSP)
+    interface.AddMessage(MsgSomeREQ)
+    interface.AddMessage(MsgSomeREQRSP)
+    interface.AddMessage(MsgSomeUnsolicitedData)
+
+    return interface
+```
+
+Then, create a file `Generate.py`.
+
+
+```python
+import kojen.Generate as Generate
+import os
+
+author = "myname@mydomain.com"
+group  = "MY_PACKAGE"
+brief  = "An example demonstrating protocol code-generation abilities."
+namespacename = "ExampleIO"
+classname = "CExampleIF"
+declspec = "" # your define for symbol export/import in C++ e.g. MY_PROJECT_API
+outputdir = os.path.join(os.path.abspath(os.path.dirname(__file__)), os.path.join("autogen","protocol"))
+protocolfile = os.path.join(os.path.abspath(os.path.dirname(__file__)), "MyInterface.py")
+Generate.Protocol(outputdir, protocolfile, namespacename, classname, declspec, author, group, brief)
+```
+
+Execute `Generate.py` using python. Your C++ code should be in the folder **./autogen/protocol**.
+
+> **Please note** : you may include this code in a library, and thus want to export some of the generated features.
+> Typically somewhere in a common header of your C++ code, you would have declared something like
+
+```cplusplus
+#ifdef MY_PROJECT_EXPORTS
+#	define MY_PROJECT_API __declspec(dllexport)
+#else
+#	define MY_PROJECT_API __declspec(dllimport)
+#endif
+```
+
+> You should thus pass **MY_PROJECT_API** as the *declspec* argument to the generator.
+
+### Output
+
+There will be several files in the output folder.
+
+* allplatforms *(folder containing required framework files)*
+* CExampleIF.h *(contains all factories to create messages which automatically and correctly fill in the headers, as well as serialization to/from bytestreams.)
+* CExampleIF.cpp
+* CExampleIFDefines.h *(contains all enums and defines)
+* CExampleIFReceiver.h *(contains a derivable class that received fully constructed messages. Override receive functions to handle them as per need.)
+* CExampleIFReceiver.cpp
+* CExampleIFStructs.h *(contains all structs)
+* CExampleIFTests.cpp *(contains all unit tests)
+* CExampleIFTransmitter.h *(contains all functions to transmit fully constructed messages. Highly advices to use the autogenerated factories.)
+* CExampleIFTransmitter.cpp
+* MsgHeader.h
+
+The following class diagram explains roughly where focus should be when implementing for actual integration into the real system.
+
+<!---![Image of necessary classes](kojen/docs/images/ProtocolClassDiagram.PNG) ... doesnt work on PyPi!--->
+![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/ProtocolClassDiagram.PNG)
+
+*IConnection* is the interface to derive from for your actual physical layer for an embedded platform. If you use boost on x86/x64, in the 'allplatforms' directory exist classes for substituting this with a TCPConnection, UDPConnection and SerialPort.
+Have a good look at the unit tests, this shows roughly how to derive from it and connect everything up, albeit creating a loopback connection, and implementing uncessary routing as the interface for the tests have a special requirement.
+
+A summary to link it up:
+* Create a derived IConnection that knows how to send and receive physical layer data.
+* Create a generated Transmitter, passing it a pointer to this connection.
+* Create a generated Receiver
+* Set the Receiver to the derived IConnection. You will then get messages in the message receiving functions...override the correct ones to handle them.
+* Use the Transmitter to send.
+
+## State Machine in C++
+### Requrements
+- Don't forget to update your git submodules when checking out.
+### Input
+The following diagram defines (roughly) a state machine for a CD player.
+
+<!---![Image of CD Player](kojen/docs/images/StateMachine.PNG)--->
+
+![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/StateMachine.PNG)
+
+This state machine can be represented by the following transition table in python (format : 'startstate', 'event', 'nextstate', 'action', 'guard'):
+
+```python
+#
+# StartState    Event                     NextState     Action                 Guard
+#
+ 'StateStop',  'EventOpen',              'StateOpen',  'OnOpenDrive',         'None'
+ 'StateStop',  'EventPlay',              'StatePlay',  'OnPlayTrack',         'GuardCDInside'
+ 'StateOpen',  'EventOpen',              'StateStop',  'OnCloseDrive',        'None'
+ 'StatePlay',  'EventPlay',              'StatePause', 'OnPause',             'None'
+ 'StatePlay',  'EventEndOfTrack',        'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'
+ 'StatePlay',  'EventEndOfTrack',        'StateStop',  'OnStop',              'GuardCDHasNoMoreTracks'
+ 'StatePlay',  'EventSkipNextTrack',     'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'
+ 'StatePlay',  'EventSkipPreviousTrack', 'None',       'OnPlayPreviousTrack', 'GuardCDHasPreviousTrack'
+ 'StatePlay',  'EventStop',              'StateStop',  'OnStop',              'None'
+ 'StatePause', 'EventPlay',              'StatePlay',  'OnPlayTrack',         'None'
+ 'StatePause', 'EventAfter10Minutes',    'StateStop',  'OnStop',              'None'
+```
+
+Create a file `Generate.py` (or add your state machine to the one already present in your project) :
+
+```python
+from kojen import Generate
+from kojen.kojentypes import *
+
+#
+# Generate Statemachine (from TransitionTable)
+#
+
+# For playing a track the tracknumber should be parameterized.
+EventPlay = Struct('EventPlay')
+EventPlay.AddType('m_track_no','uint16_t')
+
+eventsinterface = Interface('params')
+eventsinterface.AddStruct(EventPlay)
+
+# Optional features
+eventsinterface.AddUserTag("StateMachineThread", 1) # 0 = SM runs on caller thread, 1 = SM runs on its own thread. Default is 1.
+eventsinterface.AddUserTag("Verbose", 1)            # 0 = No printouts, 1 = printouts. Default is 1.
+
+# Transition Table.
+transition_table = []
+#                         StartState    Event                     NextState     Action                 Guard
+transition_table.append(['StateStop',  'EventOpen',              'StateOpen',  'OnOpenDrive',         'None'                   ])
+transition_table.append(['StateStop',  'EventPlay',              'StatePlay',  'OnPlayTrack',         'GuardCDInside'          ]) 
+transition_table.append(['StateOpen',  'EventOpen',              'StateStop',  'OnCloseDrive',        'None'                   ]) 
+transition_table.append(['StatePlay',  'EventPlay',              'StatePause', 'OnPause',             'None'                   ])
+transition_table.append(['StatePlay',  'EventEndOfTrack',        'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'   ])
+transition_table.append(['StatePlay',  'EventEndOfTrack',        'StateStop',  'OnStop',              'GuardCDHasNoMoreTracks' ])
+transition_table.append(['StatePlay',  'EventSkipNextTrack',     'None',       'OnPlayNextTrack',     'GuardCDHasMoreTracks'   ]) 
+transition_table.append(['StatePlay',  'EventSkipPreviousTrack', 'None',       'OnPlayPreviousTrack', 'GuardCDHasPreviousTrack'])
+transition_table.append(['StatePlay',  'EventStop',              'StateStop',  'OnStop',              'None'                   ])
+transition_table.append(['StatePause', 'EventPlay',              'StatePlay',  'OnPlayTrack',         'None'                   ])
+transition_table.append(['StatePause', 'EventAfter10Minutes',    'StateStop',  'OnStop',              'None'                   ])
+
+author = "myname@mydomain.com"
+group  = "MY_PACKAGE"
+brief  = "An example demonstrating state-machine code-generation abilities."
+
+eventsinterface = None
+namespacename = "CDPlayerSM"
+statemachinenameprefix = "CDPlayer"
+declspec = ""
+outputdir = "autogen/state_machine"
+templatedir = "" # defaults are for 'SML'
+Generate.StateMachine(outputdir, transition_table, eventsinterface, namespacename, statemachinenameprefix, declspec, author, group, brief, templatedir)
+```
+
+Execute `Generate.py` using python. Your C++ code should be generated to the configured folder **./autogen/state_machine**.
+
+> **Please note** : you may may wish to parameterize events in your statemachine. An event is of type `kojen.Struct` in a `kojen.Interface` object. 
+> Simply follow the quickstart for protocols, creating and returning an interface : your Event structs need to have the exact same name as defined in the transition table.
+> You should thus pass your interface object  as the *eventsinterface* argument to the generator instead of **None**.
+
+### Output
+
+There will be several files in the output folder.
+
+* allplatforms *(folder containing framework files for standalone solution)*
+* CDPlayerStateMachine.h
+* CDPlayerStateMachineImpl_SML.cpp *(all state machine code generated for boost-sml)*  
+* ICDPlayerController.h
+* Test.CDPlayerStateMachine.cpp
+  
+The following class diagram explains roughly where focus should be when implementing for test-driven development as well as for actual integration into the real system.
+
+<!---![Image of necessary classes](kojen/docs/images/StateMachineClassDiagram.PNG)--->
+![Image of necessary classes](https://raw.githubusercontent.com/kohjaen/kojen/master/kojen/docs/images/StateMachineClassDiagram.PNG)
+
+White classes are auto-generated, and have code-preservation features. Grey is what you have to manually create, and implement for integration into your real system.
+
+All required functionality for your system should be implemented in the **Controller** classes, being the base-class *ICDPlayerController*, the derived *C_My_CDPlayerController* and the derived test class *CTestCDPlayerController*.
+
+It is critical that as much of the 'business logic' is put into the base class *IPlayerController*, and tested using the *CTestCDPlayerController* in the unit-tests as possible, such that the actual integrated *C_My_CDPlayerController* uses unit-tested business logic, with a good example of how its intended to work in the unit tests...as well as for regression testing and continuous integration.
+
+As the state-machine-implementation uses the controller base class, the following construction is valid for unit tests and system integration by substituting the correct controller:
+
+```cplusplus
+  CTestCDPlayerController controller;
+  auto* sm = ICDPlayerStateMachine::Create(controller);
+```
+
+All state queries and event triggering are done using the ```sm``` instance.
+
+Due to the use of move-semantics, parameterized event structs are unique_ptr's (allocated in fixed-blocks for embedded applications) and thus once an event is triggered those pointers are no longer valid in the calling context.
+
+## State Machine in C#
+
+Similar to the above example, the only difference is the Generate call to use.
+
+```python
+   ...
+   Generate.StateMachine_CSHARP(...)
+   ...
+```
+
+## State Machine in Python
+
+Similar to the above example, the only difference is the Generate call to use.
+
+```python
+    ...
+   Generate.StateMachine_PYTHON(...)
+   ...
+```
+
+<!---
+### Deferred Events
+
+Deferred events are supported in SML and MSM state machines.
+
+In the example CD player statemachine this use-case could be pressing 'play' whilst the tray is closing : the close button will be pressed, and the tray will start closing, however the software trigger for *EventOpen* will only occur on the interrupt signalling that the tray actuator has completed either opening/closing the tray. 
+This can take up to several seconds. In that time, the 'play' button could be pressed. 
+
+The desired behaviour would be that once the tray is closed, the CD starts playing.
+
+This can be achieved by manually adding the correct deferred event in the *CDPlayerStateMachineImpl_SML.cpp* in the code preservation tags at the end of the transition table:
+
+```cplusplus
+/// {{{USER_DEFERRED_EVENTS}}}
+, StateOpen + event<EventPlay> / defer
+/// {{{USER_DEFERRED_EVENTS}}}
+```
+
+For *boost::msm* this can be achieved by manually adding the correct deferred event in code preservation tags in the state struct for *StateOpen* in *CDPlayerStateMachineImpl_SML.cpp* :
+
+```cplusplus
+/// {{{USER_StateOpen_DEFERRED_EVENTS}}}
+typedef boost::mpl::vector<EventPlay> deferred_events;
+/// {{{USER_StateOpen_DEFERRED_EVENTS}}} 
+```
+
+I believe this will also allow the sequence of 'play' then 'close' to work.
+--->
+
+
```

### Comparing `kojen-1.2.30/kojen.egg-info/SOURCES.txt` & `kojen-1.3.31/kojen.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENSE
 setup.py
 kojen/Generate.py
+kojen/Install.py
 kojen/Language.py
 kojen/LanguageCPP.py
 kojen/LanguageCsharp.py
 kojen/LanguagePython.py
 kojen/__init__.py
 kojen/__main__.py
 kojen/cgen.py
@@ -20,11 +22,12 @@
 kojen.egg-info/PKG-INFO
 kojen.egg-info/SOURCES.txt
 kojen.egg-info/dependency_links.txt
 kojen.egg-info/requires.txt
 kojen.egg-info/top_level.txt
 kojen/test/__init__.py
 kojen/test/cgen_test.py
+kojen/test/install_test.py
 kojen/test/preservative_test.py
 kojen/test/smgen_test.py
 kojen/test/vppclassdiagram_test.py
 kojen/test/vppfs_test.py
```

### Comparing `kojen-1.2.30/setup.py` & `kojen-1.3.31/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import setuptools
 
 with open("README.MD", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kojen",
-    version="1.2.30",
+    version="1.3.31",
     author="kohjaen",
     author_email="koh.jaen@yahoo.de",
     description="Code generation tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kohjaen/kojen",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6.8',
-	package_data={'': ['allplatforms/CPP/*.*', 
-                       'allplatforms/CPP/sml/include/boost/*.*', 
-                       'allplatforms/CPP/testsuite/*.*', 
-                       'allplatforms/CPP/testsuite/minunit/minunit.h', 
-                       'allplatforms/CPP/testsuite/minunit/minunit.cpp', 
-                       'classdiagram_templates/C#/*.*', 
-                       'classdiagram_templates/CPP/*.*', 
-                       'protocol_templates/CPP/*.*', 
+	package_data={'': ['allplatforms/CPP/*.*',
+                       'allplatforms/CPP/sml/include/boost/*.*',
+                       'allplatforms/CPP/testsuite/*.*',
+                       'allplatforms/CPP/testsuite/minunit/minunit.h',
+                       'allplatforms/CPP/testsuite/minunit/minunit.cpp',
+                       'classdiagram_templates/C#/*.*',
+                       'classdiagram_templates/CPP/*.*',
+                       'protocol_templates/CPP/*.*',
                        'protocol_templates/PY/*.*',
                        'statemachine_templates_cs_winlinmac/*.*',
                        'statemachine_templates_embedded_arm/*.*',
                        'statemachine_templates_py/*.*',
-                       'statemachine_templates_pc_boost/*.*', 
-                       'docs/images/*.*', 
+                       'statemachine_templates_pc_boost/*.*',
+                       'docs/images/*.*',
                        'docs/*.*']},
 	include_package_data=True,
     install_requires=['cogapp>=3.0.0',],
 )
```

