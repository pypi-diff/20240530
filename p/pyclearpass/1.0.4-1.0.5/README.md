# Comparing `tmp/pyclearpass-1.0.4.tar.gz` & `tmp/pyclearpass-1.0.5.tar.gz`

## Comparing `pyclearpass-1.0.4.tar` & `pyclearpass-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/CONTRIBUTING.md
--rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/PKG-INFO.txt
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/RELEASE-NOTES.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/setup.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/__init__.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_apioperations.py
--rw-r--r--   0        0        0    26936 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_certificateauthority.py
--rw-r--r--   0        0        0   122925 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_endpointvisibility.py
--rw-r--r--   0        0        0   248363 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_enforcementprofile.py
--rw-r--r--   0        0        0   148850 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_globalserverconfiguration.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_guestactions.py
--rw-r--r--   0        0        0   112446 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_guestconfiguration.py
--rw-r--r--   0        0        0   110091 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_identities.py
--rw-r--r--   0        0        0    43353 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_insight.py
--rw-r--r--   0        0        0   108433 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_integrations.py
--rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_localserverconfiguration.py
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_logs.py
--rw-r--r--   0        0        0    31234 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_platformcertificates.py
--rw-r--r--   0        0        0   210162 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_policyelements.py
--rw-r--r--   0        0        0    20203 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_sessioncontrol.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/api_toolsandutilities.py
--rw-r--r--   0        0        0     6566 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyclearpass/common.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/LICENSE.md
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/README.md
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    13831 2020-02-02 00:00:00.000000 pyclearpass-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0    17704 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/PKG-INFO.txt
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/RELEASE-NOTES.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/setup.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/__init__.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_apioperations.py
+-rw-r--r--   0        0        0    26938 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_certificateauthority.py
+-rw-r--r--   0        0        0   123035 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_endpointvisibility.py
+-rw-r--r--   0        0        0   248365 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_enforcementprofile.py
+-rw-r--r--   0        0        0   149308 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_globalserverconfiguration.py
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_guestactions.py
+-rw-r--r--   0        0        0   112448 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_guestconfiguration.py
+-rw-r--r--   0        0        0   113217 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_identities.py
+-rw-r--r--   0        0        0    43710 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_insight.py
+-rw-r--r--   0        0        0   108435 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_integrations.py
+-rw-r--r--   0        0        0    23980 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_localserverconfiguration.py
+-rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_logs.py
+-rw-r--r--   0        0        0    31236 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_platformcertificates.py
+-rw-r--r--   0        0        0   210171 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_policyelements.py
+-rw-r--r--   0        0        0    20205 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_sessioncontrol.py
+-rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/api_toolsandutilities.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyclearpass/common.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/LICENSE.md
+-rw-r--r--   0        0        0    16857 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/README.md
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    17919 2020-02-02 00:00:00.000000 pyclearpass-1.0.5/PKG-INFO
```

### Comparing `pyclearpass-1.0.4/CONTRIBUTING.md` & `pyclearpass-1.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyclearpass-1.0.4/PKG-INFO.txt` & `pyclearpass-1.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,17 @@
-Metadata-Version: 2.1
-Name: pyclearpass
-Version: 1.0.4
-Summary: This package contains all of the API functions to work with the ClearPass API. This package been built based on Aruba ClearPass v6.11.x but is always generated on the latest version available to download.  
-Project-URL: Homepage, https://github.com/aruba/pyclearpass
-Author-email: Aruba Automation <aruba-automation@hpe.com>
-License-File: LICENSE
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: System :: Networking
-Requires-Python: >=3.9
-Requires-Dist: requests>=2.24
-Requires-Dist: urllib3>=1.25.10
-Description-Content-Type: text/markdown
-
 # pyclearpass
-## Aruba ClearPass V6.11 SDK
-Aruba ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the Aruba ClearPass REST API environment. Each available REST API command is available for use in this module. All responses from the ClearPass API are in JSON format and any interactions with the API are logged within the Audit Viewer.
+## HPE Aruba Networking ClearPass V6.12 SDK
+Aruba ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the HPE Aruba Networking ClearPass REST API environment. Each available REST API command is available for use in this module. All responses from HPE Aruba Networking ClearPass API are in JSON format (converted into a Python dictionary object) and any interactions with the API are logged within the Audit Viewer.
+
+This package has been uploaded to https://pypi.org/ and is also available to install via https://github.com/aruba/pyclearpass. 
+These instructions are also available at https://developer.arubanetworks.com/aruba-cppm/docs/getting-started-with-pyclearpass.
+Installation instructions and usage instructions are also provided below. 
 
-This package has been uploaded to https://pypi.org/ and is also available to install via https://github.com/aruba/pyclearpass. Installation instructions are provided below. 
 ## Available API Categories  
-The following describes the available top level functionality of the ClearPass API available within this Python Package. 
+The following describes the available top level functionality of the HPE Aruba Networking ClearPass API available within this Python Package. 
 - Operations
 - Certificate Authority
 - Endpoint Visibility 
 - Enforcement Profile
 - Global Server Configuration
 - Guest Actions
 - Guest Configuration
@@ -38,31 +23,32 @@
 - Platform Certificates
 - Policy Elements
 - Session Controls
 - Tools and Utilities
 
 _This package comes without any warranties and should be used at your own risk._
 
-## ClearPass Server Readiness
-These steps list what is required on the ClearPass server:
-1. Make sure you have the API Service enabled within Services. You may use the template to help you do this. 
-2. Create a new API Client within the ClearPass Guest Portal 
+## HPE Aruba Networking ClearPass Server Readiness
+These steps list what is required on the HPE Aruba Networking ClearPass server:
+1. Create a new API Client within the HPE Aruba Networking ClearPass Guest Portal 
     - client id = demo, 
-    - enabled, Operating Mode = Rest API, 
-    - Operator Profile = Pick one with apporpiate permission level or make a new one,  
+    - enabled, Operating Mode = Rest API
+    - Operator Profile = Pick one with apporpiate permission level or make a new one 
     - Grant Type = client credentials
     - Access Token Lifetime = 8 Hours
-3. Optional but preferred, a valid SSL cerfificate
+2. Optional but preferred: valid SSL cerfificate
+3. Optional: API Service enabled within Services. You may use the template to help you do this. Only required when using 'Grant Type' of Password. 
 
-If you need information, refer to the ClearPass configuration documentation for the API account -
-https://developer.arubanetworks.com/aruba-cppm/docs/clearpass-configuration  
+If you need information, refer to the HPE Aruba Networking ClearPass configuration documentation for the API account -
+https://developer.arubanetworks.com/aruba-cppm/docs/clearpass-configuration
 
 # Python Requirements  
 Ensure Python v3.9 or greater is installed on your operating system
-# Package Installation  
+# Package Installation
+
 #### Method 1 - Installing Package from PyPi
 Run the following in a command line terminal to install the pip package - ```pip3 install pyclearpass``` or ```pip install pyclearpass```. This may vary between Operating Systems. 
 
 #### Method 2 - Installing Package from Github (not using Git.exe)
 1. Click into the Aruba Github Repository where the latest version of pyclearpass is located 
 2. Click Code (in green) and Download to Zip
 3. Extract the zip file into a directory
@@ -70,153 +56,269 @@
 5. In your command line terminal type ```python3 -m build``` or ```python -m build```. This will create a folder called dist with a file containing a .gz extension. 
 6. Run the following in a command line terminal to install the pip package - ```pip3 install pathtozip.gz``` or ```pip install pathtozip.gz```. This may vary between Operating Systems.
 
 #### Method 3 - Installing Package from Github (using Git.exe)
 1. Install Git for your Operating System from https://git-scm.com/download
 2. Run the following in a command line terminal to install the pip package - ```pip3 install git+https://github.com/aruba/pyclearpass``` or ```pip install git+https://github.com/aruba/pyclearpass```. This may vary between Operating Systems. 
 
-# Inital Usage Instructions
-Within your Python favourite IDE environment, create an import reference
-```
+# Initial Usage Instructions
+
+Within your favourite Python IDE environment, create an import reference
+
+```python
 from pyclearpass import *
 ```
-Create a object to login into ClearPass. The login object needs to be passed to use any function within the ClearPass API.
+
+Create a object to login into ClearPass. The login object needs to be passed to use any function within the ClearPass API.  
 Two examples below shows how to create the login object (either one can be used, but not both).
-1. Using client_credentials
-```
+
+1. Using client credentials
+
+```python
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",granttype="client_credentials",
 clientsecret="myclientsecretexample", clientid="myclientidexample", verify_ssl=False)
 ```
->The login object will contain the APIToken once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
-2. Using an explicitly defined api_token
-```
+
+> 📘 
+> 
+> The login object will contain the APIToken once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
+
+2. Using an explicitly defined api_token. You can generate an API token by clicking on the API client and then clicking 'Generate Access Token'.
+
+```python
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",api_token="yoursecretapitoken", verify_ssl=False)
 ```
 
+Find an API you want to use, by prefixing  `Api`  in your IDE and Intellisense will show the available APIs available. Each of the top level API category names are available as a module. Once you have chosen a specific API module to use, for example ApiPolicyElements, it will show you the available methods if you suffix a . to the command - `ApiPolicyElements.`
 
-Find an API you want to use, by prefixing  ```Api```  in your IDE and intellisense will show the available APIs available. Each of the top level API category names are available as a module. Once you have chosen a specifc API to use, for example ApiPolicyElements, it will show you the available methods if you suffix a . to the command - ```ApiPolicyElements.```
+The example below prints a single the roles available within the ClearPass server.
 
-The example below prints the roles available within the clearpass server.
-```	
+```python
 print(ApiPolicyElements.get_role(login)) 
 ```
-By default, the example above to return the roles available within the clearpass server will only show the first 25 roles. If you want to view more, you have to adjust the limit. Placing your cursor over the .getRole will usually show you help about the method. 
-```
+
+By default, the example above returns the first 25 roles. To view more, the limit needs to be adjusted. Placing your cursor over the .getRole will usually show you help about the method. 
+
+```python
 print(ApiPolicyElements.get_role(login, limit=100))
 ```
-# Help 
-Once you have written a specific API  ```ApiName.FunctionName(```, placing your cursor over the command will show you help for the function and what the required parameters are (example is Visual Studio Code). The first parameter is always login. 
-You may also read the help for the function by calling ```help(ApiName.FunctionName)```. Each function contains a help section on how to use it. 
+
+# Help
+
+Once you have written a specific API  `ApiName.FunctionName(`, placing your cursor over the command will show you help for the function and what the required parameters are (example is Visual Studio Code). The first parameter is always login.  
+You may also read the help for the function by calling `help(ApiName.function_name)`.  
+Each function contains a help section on how to use it. 
+
 # Python Package Upgrade Instructions
-Once an update is available on the Python PyPi repository, you may upgrade your release by completing the following in a command line terminal - ```pip3 install pyclearpass --upgrade```
+
+Once an update is available on the Python PyPi repository, you may upgrade your release by completing the following in a command line terminal - 
+
+`pip3 install pyclearpass --upgrade`  
+or  
+`pip install pyclearpass --upgrade`
+
+To install a specific version, execute the following command with x.x.x being the specific version number you want to install. 
+
+`pip3 install pyclearpass==x.x.x`  
+or  
+ `pip install pyclearpass==x.x.x`
+ 
 # Uninstall Package Package
-To remove the Python pyclearpass package, type the following command into a command line terminal - ```pip3 uninstall pyclearpass ``` or ```pip uninstall pyclearpass ```
 
-# Release Notes
-Release notes for this version are availble in the [RELEASE-NOTES.md](RELEASE-NOTES.md) file.
+To remove the Python pyclearpass package, type the following command into a command line terminal -  
+`pip3 uninstall pyclearpass `  
+or  
+ `pip uninstall pyclearpass `
 
 # Further Usage Examples
-The examples below all exclude importing the module and creating the login variable. This is described directly below.
 
-## New Login Session
+The examples below all exclude importing the module and creating the login variable. This is described directly below. Note, these are just a full examples, there are hundreds of API commands available within the SDK.
+
+## New Login Session (Mandatory)
+
 The login variable only needs to be defined once in the script. Two examples are shown below to achieve this;
 
 1. Using client_credentials
-```
+
+```python
 from pyclearpass import *
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",granttype="client_credentials",
 clientsecret="myclientsecretexample", clientid="myclientidexample", verify_ssl=False)
 ```
->As mentioned earlier, the login object will contain the API Token once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
 
-2. Using an explicitly defined api_token
-```
+> 📘 
+> 
+> As mentioned earlier, the login object will contain the API Token once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
+
+2. Using an explicitly defined api_token. You can generate an API token by clicking on the API client and then clicking 'Generate Access Token'.
+
+```python
 from pyclearpass import *
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",api_token="yoursecretapitoken", verify_ssl=False)
 ```
 
-## Get Local Server Configuration 
-```
+## Get Local Server Configuration
+
+```python
+import json
 LSCGCS = ApiLocalServerConfiguration.get_cluster_server(login)
 print(json.dumps(LSCGCS['_embedded']['items'],indent=1))
 ```
 
-## Get Total End Point Count 
-```
+## Get Total End Point Count
+
+```python
 IGEP = ApiIdentities.get_endpoint(login, calculate_count='true')
 print("Total MACs in Table: "+str(IGEP['count']))
 ```
 
 ## Get Insight Device Details
-```
+
+```python
 print(ApiLogs.get_insight_endpoint_ip_by_ip(login,ip="192.168.0.99"))
 ```
 
 ## Get list of Admin Users
-```
+
+```python
 AU = ApiGlobalServerConfiguration.get_admin_user(login)
 for users in AU['_embedded']['items']:
   print(users)
 ```
 
-## Get Network Access Device
+## Add New Endpoint
+
+```python
+newEndPoint = {
+  "mac_address": "11:22:33:44:55:66",
+  "description": "Demo EndPoint 1",
+  "status": "Known"
+}
+print(ApiIdentities.new_endpoint(login,body=newEndPoint))
 ```
+
+## Add New Role
+
+```python
+role={"name": "Test1","description": "Test role made using the API Package in Python"}
+print(ApiPolicyElements.new_role(login,body=role))
+```
+
+## Delete Role
+
+```python
+print(ApiPolicyElements.delete_role_name_by_name(login,name='Demo'))
+```
+
+## Get Network Access Device
+
+```python
 devices = ApiPolicyElements.get_network_device(login)
 for device in devices["_embedded"]["items"]:
     print(device)
 ```
 
 ## Get Network Access Device by Name
-```
+
+```python
 print(ApiPolicyElements.get_network_device_name_by_name(login, "Lab-AP-IAP-VC"))
 ```
 
 ## Add New Network Access Device
-```
+
+```python
 newNAD = {
     "description": "LAB AP IAP VC",
     "name": "Lab-AP-IAP-VC",
     "ip_address": "192.168.0.100",
     "radius_secret": "example_radius_secret",
     "tacacs_secret": "example_tacacs_secret",
     "vendor_name": "Aruba",
     "coa_capable": True,
     "coa_port": 3799,
     "attributes": {"Device Type": "IAP"},
 }
 ApiPolicyElements.new_network_device(login, body=newNAD)
 ```
 
-## Add New Endpoint
-```
-newEndPoint = {
-  "mac_address": "11:22:33:44:55:66",
-  "description": "Demo EndPoint 1",
-  "status": "Known"
-}
-print(ApiIdentities.new_endpoint(login,body=newEndPoint))
-```
+## Add New Network Access Device via CSV
+
+This example adds new Network Access Devices based on the CSV (comma delimited values) named "network access devices.csv" with headings and content filled rows. 
+
+| name  | description    | ip_address    | location |
+| :---- | :------------- | :------------ | :------- |
+| demo1 | example demo 1 | 192.168.100.1 | UK       |
+| demo2 | example demo 2 | 192.168.100.2 | US       |
+
+```python
+import pandas as pd
+df = pd.read_csv("network access devices.csv")
+
+for index, items in df.iterrows():
+    newnad = {
+        "description": items["description"],  # Description of the network device. Object Type: string
+        "name": items["name"],  # Name of the network device. Object Type: string
+        "ip_address": items["ip_address"],  # IP or Subnet Address of the network device. Object Type: string
+        "tacacs_secret": "testing123",  # TACACS+ Shared Secret of the network device. Object Type: string
+        "vendor_name": "Aruba",  # Vendor Name of the network device. Object Type: string
+        "attributes": {"Location": items["location"]},
+    }
+    print(ApiPolicyElements.new_network_device(login, body=newnad))
+    print(items["name"], items["ip_address"])
 
-## Add New Role
-```
-role={"name": "Test1","description": "Test role made using the API Package in Python"}
-print(ApiPolicyElements.new_role(login,body=role))
 ```
 
-## Delete Role
+## Update Network Access Device via CSV
+
+This example updates Network Access Devices attributes based on the CSV (comma delimited values) named "network access devices updates.csv" with headings and content filled rows. 
+
+| name  | description    | location |
+| :---- | :------------- | :------- |
+| demo1 | updated demo 1 | US       |
+| demo2 | updated demo 2 | UK       |
+
+```python
+import pandas as pd
+df = pd.read_csv("network access devices updates.csv")
+for index, items in df.iterrows():
+    nadupdate = {                
+        "tacacs_secret": "updatedpassword123",  # TACACS+ Shared Secret of the network device. Object Type: string
+        "description": items["description"],  # Description of the network device. Object Type: string
+        "attributes": {"Location": items["location"]},
+    }
+    print(ApiPolicyElements.update_network_device_name_by_name(login,name=items["name"],body=nadupdate))
+
 ```
-print(ApiPolicyElements.delete_role_name_by_name(login,name='Demo'))
+
+## Update Network Device Group
+
+This example updates an Network Device Group with additional IP Addresses 192.168.0.100 and 192.168.0.99.  
+These Network Access Devices must of been added before they can be appended to the group.  
+
+```python
+getcurrentnads = ApiPolicyElements.get_network_device_group_name_by_name(login,name="Example")
+newnads={"value" : "192.168.0.100, 192.168.0.98"}
+newnads["value"]=getcurrentnads['value']+", "+newnads["value"]
+print(ApiPolicyElements.update_network_device_group_name_by_name(login,name="Example",body=newnads))
+
 ```
 
-## Add New Guest Device 
+> 🚧 Ensure completion of validation checks
+> 
+> Validate the Network Access Device exists and is not already part of the Network Device Group before attempting to append to the group.
+
+## Add New Guest Device
+
 This example adds a Guest Device including 
+
 1. An expiry date within 24 hours in seconds 
 2. Associated to the role ID of 3 (Guest in test environment)
 3. Statically assigned MPSK password
-```
+
+```python
 import time
 new_guest_device = {
   "enabled": True,
   "expire_time": int(time.time()) + 86400,
   "mac": "11:22:22:33:33:11",
   "notes": "Created by API Test Script",
   "role_id": 3,
@@ -226,28 +328,31 @@
   "mpsk_enable":"1"
 }
 new_device= ApiIdentities.new_device(login,body=new_guest_device)
 print(new_device)
 ```
 
 ## Get Guest Device by MAC
-```
+
+```python
 import json
 get_mac_address = "11-22-33-33-22-11"
 view_guest_device = ApiIdentities.get_device_mac_by_macaddr(login,get_mac_address)
 print(json.dumps(view_guest_device,indent=2))
 ```
 
 ## Delete an Enforcement Policy
-```
+
+```python
 print(ApiPolicyElements.delete_enforcement_policy_by_enforcement_policy_id(login,enforcement_policy_id='3058'))
 ```
 
-## Create a new Enforcement Policy with staged initial rules and then a loop to create additional rules. 
-```
+## Create a new Enforcement Policy with staged initial rules and then a loop to create additional rules.
+
+```python
 newEnforcementPolicy= {
   "name": "MPSK Demo",
   "description": "MPSK Enforcement",
   "enforcement_type": "RADIUS",
   "default_enforcement_profile": "Deny Device",
   "rule_eval_algo": "first-applicable",
   "rules": ''}
@@ -288,18 +393,23 @@
     
     newEnforcementPolicyRules["rules"].append(epf) 
  
 newEnforcementPolicy["rules"] = newEnforcementPolicyRules["rules"]
 print(ApiPolicyElements.new_enforcement_policy(login,body=newEnforcementPolicy))
 ```
 
->Note - you may find it easier to initially pull a working Enforcement Policy with minimal rules before trying to create a new one from scratch. For example, the rule evaluation in the GUI shows as 'First applicable', however in the backend it is shown as 'first-applicable'. This example is a working policy. It is demonstrated with a loop which could read an entry in a CSV file if adapted. 
+> 📘 
+> 
+> You may find it easier to initially pull a working Enforcement Policy with minimal rules before trying to create a new one from scratch. 
+> 
+> For example, the rule evaluation in the GUI shows as 'First applicable', however in the back-end it is shown as 'first-applicable'. This example is a working policy. It is demonstrated with a loop which could read an entry in a CSV file if adapted.
 
-## Update an existing Enforcement Policy, retaining the original items and using a loop to add additional items 
-```
+## Update an existing Enforcement Policy, retaining the original items and using a loop to add additional items
+
+```python
 epol = ApiPolicyElements.get_enforcement_policy_name_by_name(login, name="MPSK Enforcement")
 OriginalRules = epol["rules"]
 CombinedRules =({"rules":[]})
 for item in range(len(OriginalRules)):
     CombinedRules["rules"].append(OriginalRules[item])
 
 for no in range(9,11):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyclearpass-1.0.4/RELEASE-NOTES.md` & `pyclearpass-1.0.5/RELEASE-NOTES.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 # Release Notes
-This document contains high level documented changes to the pyclearpass module releases
-## Version 1.0.0
-Initial Release
-## Version 1.0.1
+This document contains high level documented changes to the pyclearpass package.
+
+## Version 1.0.0 (Not listed) 
+1. Initial Release
+
+## Version 1.0.1 (04/07/2023)
 1. Code updated to PEP8 standards (formatting of code along with renaming of variables, packages, classes and modules)
 2. Additional examples provided
-## Version 1.0.2
+
+## Version 1.0.2 (12/09/2023)
 1. Fixed an issue with the parameter name as not injected correctly into dictionary (page-name)
 2. Added descriptions to body parameters across all methods 
 3. Used new method to generate modules file 
 4. Python package generated  based on latest API available within ClearPass v6.11.4
 5. Newly created code updated to PEP8 standards
 6. Updated ClearPassAPILogin class init method to include 'api_token' to allow an api token to be used rather than client_credentials
 7. Updated ClearPassAPILogin class method name from _get_api_key to _new_api_token and updated local references
 8. Updated ClearPassAPILogin class method _send_request to include a except for KeyError
 9. All file names updated
 10. Updated __init__.py to reflect new filenames
 11. Updated README.md
-## Version 1.0.3
+
+## Version 1.0.3 (12/09/2023)
 1. Missing '_new_api_token' rename from ClearPassAPILogin (common.py)
-## Version 1.0.4
+
+## Version 1.0.4 (06/11/2023)
 1. Fixed incorrect positioning of characters in 'body dictionary object' across all api files (to allow copy and paste of body for easy use of script).
 2. Fixed missed # 'body dictionary object' across all api files for 'object' type.  
-3. API code includes new, modified or deleted API that is implemented in Aruba ClearPass v6.11.5. 
+3. API code includes new, modified or deleted API that is implemented in Aruba ClearPass v6.11.5.
+
+## Version 1.0.5 (30/05/2024)
+1. Updated references of 'Aruba ClearPass' to 'HPE Aruba Networking ClearPass'
+2. API code includes new, modified or deleted API that is implemented in HPE Aruba Networking ClearPass v6.12.2. To use older version built on v6.11.5, execute 'pip install pyclearpass==1.0.4'
+3. Updated README.md
+4. Updated year in license.md
```

### Comparing `pyclearpass-1.0.4/setup.py` & `pyclearpass-1.0.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,24 +4,23 @@
     # Needed to silence warnings (and to be a worthwhile package)
     name='pyclearpass',
     url='https://github.com/aruba/pyclearpass',
     author='Aruba Automation',
     author_email='aruba-automation@hpe.com',
     packages=['pyclearpass'],
     install_requires=['requests >=2.24','urllib3 >=1.25.10'],
-    version='1.0.4',
+    version='1.0.5',
     license='MIT',
-    description='Aruba ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the Aruba ClearPass REST API environment. Each available REST API command is available for use in this module.',
+    description='HPE Aruba Networking ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the HPE Aruba Networking ClearPass REST API environment. Each available REST API command is available for use in this package.',
     long_description=open('README.md').read(),
     classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 	"Intended Audience :: System Administrators",
 	"Intended Audience :: Automation Experts",
 	"Intended Audience :: Deployment Engineers",
     "Topic :: System :: Networking",
     "Natural Language :: English",],
-    project_urls={"Source": "https://github.com/aruba/pyclearpass/"},
-    keywords="Aruba, Aruba ClearPass, Aruba CPPM, CPPM, pyclearpass"
-
+    project_urls={"repository":"https://github.com/aruba/pyclearpass/","changelog":"https://github.com/aruba/pyclearpass/blob/main/RELEASE-NOTES.md","homepage":"https://developer.arubanetworks.com/aruba-cppm/docs/getting-started-with-pyclearpass"},
+    keywords="Aruba, Aruba ClearPass, Aruba CPPM, CPPM, pyclearpass, HPE Aruba Networking ClearPass"
 )
```

### Comparing `pyclearpass-1.0.4/pyclearpass/__init__.py` & `pyclearpass-1.0.5/pyclearpass/__init__.py`

 * *Files identical despite different names*

### Comparing `pyclearpass-1.0.4/pyclearpass/api_apioperations.py` & `pyclearpass-1.0.5/pyclearpass/api_apioperations.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: ApiOperations
 # FileName: api_apioperations.py
 
 
 class ApiApiOperations(ClearPassAPILogin):
+
     # API Service: Obtain an OAuth2 access token for making API calls
     def new_oauth(self, body=({})):
         """
         Operation: Obtain an OAuth2 access token for making API calls
         HTTP Response Codes: 200 OK, 400 Bad Request, 406 Not Acceptable, 415 Unsupported Media Type
         Required Body Parameters:['grant_type', 'client_id']
         Parameter Type: body, Name: body
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_certificateauthority.py` & `pyclearpass-1.0.5/pyclearpass/api_certificateauthority.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: CertificateAuthority
 # FileName: api_certificateauthority.py
 
 
 class ApiCertificateAuthority(ClearPassAPILogin):
+
     # API Service: Manage Onboard certificates
     def get_certificate(
         self, filter="", sort="", offset="", limit="", calculate_count=""
     ):
         """
         Operation: Get a list of certificates
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_endpointvisibility.py` & `pyclearpass-1.0.5/pyclearpass/api_endpointvisibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: EndpointVisibility
 # FileName: api_endpointvisibility.py
 
 
 class ApiEndpointVisibility(ClearPassAPILogin):
+
     # API Service: Manage Agentless OnGuard settings
     def get_agentless_onguard_settings(self):
         """
         Operation: Get a list of Agentless OnGuard Settings
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type
         """
         url_path = "/agentless-onguard/settings"
@@ -1346,14 +1347,15 @@
         "agentLibraryVersion" : "", #Version of the OnGuard Agent Library. This is read-only field. Object Type: string
         "installer_modified_time" : "", #Time when Agent Installers was last updated. This is read only field. Object Type: string
         "installer_modified_time_formatted" : "", #Formatted Time when Agent Installers was last updated. This is read only field. Object Type: string
         "agent_installers" : {}, #Details about Agent installers. This is read-only field. Object Type: object
         "agent_web_installers" : {}, #Details about Native Dissolvable Agent installers. This is read only field. Object Type: object
         "ip_version_onguard" : "", #IP Version for Server Communication (OnGuard). Object Type: string
         "ip_version_native" : "", #IP Version for Server Communication (Native). Object Type: string
+        "ip_version_agentless" : "", #IP Version for Server Communication (Agentless). Object Type: string
         "custom_remediation" : {}, #Customize webpage details for Agent Remediation UI. Input should be in JSON format.. Object Type: object
 
         }
         """
         url_path = "/onguard/settings"
         body = _remove_empty_keys(keys=body)
         return ClearPassAPILogin._send_request(
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_enforcementprofile.py` & `pyclearpass-1.0.5/pyclearpass/api_enforcementprofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: EnforcementProfile
 # FileName: api_enforcementprofile.py
 
 
 class ApiEnforcementProfile(ClearPassAPILogin):
+
     # API Service: Manage Captive Portal Profile
     def get_enforcement_profile_dur_captive_portal_profile_by_product_name(
         self, product_name=""
     ):
         """
         Operation: GET a list of Captive Portal Profiles
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_globalserverconfiguration.py` & `pyclearpass-1.0.5/pyclearpass/api_globalserverconfiguration.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: GlobalServerConfiguration
 # FileName: api_globalserverconfiguration.py
 
 
 class ApiGlobalServerConfiguration(ClearPassAPILogin):
+
     # API Service: Manage admin privileges
     def get_admin_privilege(
         self, filter="", sort="", offset="", limit="", calculate_count=""
     ):
         """
         Operation: Get a list of admin privileges
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
@@ -907,38 +908,40 @@
         "AdminUserLoginTertiaryRemoteTacacsServerSecret" : "", #No Desc. Object Type: string
         "AlertNotificationTimeout" : "", #Alert Notification Timeout in hours. Object Type: string
         "AuditRecordsCleanupInterval" : 0, #Old Audit Records cleanup interval in days. Object Type: integer
         "AutoBackupConfigOptions" : "", #Auto backup configuration options. Object Type: string
         "CLISessionIdleTimeout" : 0, #CLI Session Idle Timeout in minutes. Object Type: integer
         "CSRCleanupInterval" : 0, #Cleanup interval for CSRs and private keys. Object Type: integer
         "ClearPassZoneCache" : "", #ClearPass Zone Cache Durability. Object Type: string
+        "CloseIdleRadSecTunnelFromNAD" : 0, #No Desc. Object Type: integer
         "ClusterCommunicationMode" : "", #Mode of communication between cluster nodes. Object Type: string
         "CommonCriteriaMode" : "", #Enable Common Criteria mode for the cluster. Object Type: string
         "ConsoleSessionIdleTimeout" : 0, #Console Session Idle Timeout in minutes. Object Type: integer
         "ContentSecurityPolicy" : "", #Enable Content Security Policy (CSP). Object Type: string
         "ContextServerPollInterval" : 0, #Endpoint Context Servers polling interval in minutes. Object Type: integer
         "ContextServerPollStartTime" : "", #[00:00:00-23:59:59] Endpoint Context Servers polling start time. Object Type: string
         "DbAppexternalUserPassword" : "", #Database user "appexternal" password. Object Type: string
         "DesignatedStandbyPublisher" : "", #Designated Standby Publisher. Object Type: string
-        "DisableTLS1.0" : "", #Disable TLSv1.0 support. Object Type: string
-        "DisableTLS1.1" : "", #Disable TLSv1.1 support. Object Type: string
+        "DisableTLS1.0" : "", #Disable TLSv1.0 support, this field cannot be modified in FIPS mode. Object Type: string
+        "DisableTLS1.1" : "", #Disable TLSv1.1 support, this field cannot be modified in FIPS mode. Object Type: string
         "DisableTLS1.3" : "", #No Desc. Object Type: string
         "EnableNTLMV1ForWmi" : "", #Enable NTLMV1 for WMI scans. Object Type: string
         "EnablePublisherFailover" : "", #Enable Publisher Failover. Object Type: string
         "EnableTelemetry" : "", #Enable sharing information about the cluster to Telemetry server. Object Type: string
         "EnableUserAcknowledgement" : "", #Force Enable User Acknowledgement. Object Type: string
         "ExpiredGuestAccountsCleanupInterval" : 0, #Expired guest accounts cleanup interval in days. Object Type: integer
         "ExtensionsAutoUpgradesFlag" : "", #No Desc. Object Type: string
         "FreeDiskSpaceThreshold" : 0, #Free disk space threshold value in %. Object Type: integer
         "FreeMemoryThreshold" : 0, #Free memory threshold value in %. Object Type: integer
         "ICMPv6Filters" : "", #Enable ICMPv6 Filters. Object Type: string
         "IgnoreConflictNetworkBootAgents" : "", #Enable Ignore Conflict (Network Boot Agents). Object Type: string
         "InformationStoredCleanupInterval" : 0, #Cleanup interval for information stored on the disk in days. Object Type: integer
         "KnownEndpointsCleanupInterval" : 0, #Known endpoints cleanup interval in days. Object Type: integer
         "LoginBannerText" : "", #Login Banner Text. Object Type: string
+        "MACAddressFormat" : "", #No Desc. Object Type: string
         "NetflowReprofileInterval" : 0, #Netflow reprofile interval in days. Object Type: integer
         "NotificationEmailAddress" : "", #Alert Notification - Email Address. Object Type: string
         "NotificationSmsAddress" : "", #Alert Notification - SMS Address. Object Type: string
         "OnGuardAutoUpdatesFlag" : "", #Automatically check for available OnGuard Signature Updates. Object Type: string
         "PasswordPrompt" : "", #TACACS+ Password Prompt Text. Object Type: string
         "PolicyResultCacheTimeout" : 0, #Policy result cache timeout in minutes. Object Type: integer
         "PostAuthUnsubscribeEndpoints" : "", #No Desc. Object Type: string
@@ -1002,38 +1005,40 @@
         "AdminUserLoginTertiaryRemoteTacacsServerSecret" : "", #No Desc. Object Type: string
         "AlertNotificationTimeout" : "", #Alert Notification Timeout in hours. Object Type: string
         "AuditRecordsCleanupInterval" : 0, #Old Audit Records cleanup interval in days. Object Type: integer
         "AutoBackupConfigOptions" : "", #Auto backup configuration options. Object Type: string
         "CLISessionIdleTimeout" : 0, #CLI Session Idle Timeout in minutes. Object Type: integer
         "CSRCleanupInterval" : 0, #Cleanup interval for CSRs and private keys. Object Type: integer
         "ClearPassZoneCache" : "", #ClearPass Zone Cache Durability. Object Type: string
+        "CloseIdleRadSecTunnelFromNAD" : 0, #No Desc. Object Type: integer
         "ClusterCommunicationMode" : "", #Mode of communication between cluster nodes. Object Type: string
         "CommonCriteriaMode" : "", #Enable Common Criteria mode for the cluster. Object Type: string
         "ConsoleSessionIdleTimeout" : 0, #Console Session Idle Timeout in minutes. Object Type: integer
         "ContentSecurityPolicy" : "", #Enable Content Security Policy (CSP). Object Type: string
         "ContextServerPollInterval" : 0, #Endpoint Context Servers polling interval in minutes. Object Type: integer
         "ContextServerPollStartTime" : "", #[00:00:00-23:59:59] Endpoint Context Servers polling start time. Object Type: string
         "DbAppexternalUserPassword" : "", #Database user "appexternal" password. Object Type: string
         "DesignatedStandbyPublisher" : "", #Designated Standby Publisher. Object Type: string
-        "DisableTLS1.0" : "", #Disable TLSv1.0 support. Object Type: string
-        "DisableTLS1.1" : "", #Disable TLSv1.1 support. Object Type: string
+        "DisableTLS1.0" : "", #Disable TLSv1.0 support, this field cannot be modified in FIPS mode. Object Type: string
+        "DisableTLS1.1" : "", #Disable TLSv1.1 support, this field cannot be modified in FIPS mode. Object Type: string
         "DisableTLS1.3" : "", #No Desc. Object Type: string
         "EnableNTLMV1ForWmi" : "", #Enable NTLMV1 for WMI scans. Object Type: string
         "EnablePublisherFailover" : "", #Enable Publisher Failover. Object Type: string
         "EnableTelemetry" : "", #Enable sharing information about the cluster to Telemetry server. Object Type: string
         "EnableUserAcknowledgement" : "", #Force Enable User Acknowledgement. Object Type: string
         "ExpiredGuestAccountsCleanupInterval" : 0, #Expired guest accounts cleanup interval in days. Object Type: integer
         "ExtensionsAutoUpgradesFlag" : "", #No Desc. Object Type: string
         "FreeDiskSpaceThreshold" : 0, #Free disk space threshold value in %. Object Type: integer
         "FreeMemoryThreshold" : 0, #Free memory threshold value in %. Object Type: integer
         "ICMPv6Filters" : "", #Enable ICMPv6 Filters. Object Type: string
         "IgnoreConflictNetworkBootAgents" : "", #Enable Ignore Conflict (Network Boot Agents). Object Type: string
         "InformationStoredCleanupInterval" : 0, #Cleanup interval for information stored on the disk in days. Object Type: integer
         "KnownEndpointsCleanupInterval" : 0, #Known endpoints cleanup interval in days. Object Type: integer
         "LoginBannerText" : "", #Login Banner Text. Object Type: string
+        "MACAddressFormat" : "", #No Desc. Object Type: string
         "NetflowReprofileInterval" : 0, #Netflow reprofile interval in days. Object Type: integer
         "NotificationEmailAddress" : "", #Alert Notification - Email Address. Object Type: string
         "NotificationSmsAddress" : "", #Alert Notification - SMS Address. Object Type: string
         "OnGuardAutoUpdatesFlag" : "", #Automatically check for available OnGuard Signature Updates. Object Type: string
         "PasswordPrompt" : "", #TACACS+ Password Prompt Text. Object Type: string
         "PolicyResultCacheTimeout" : 0, #Policy result cache timeout in minutes. Object Type: integer
         "PostAuthUnsubscribeEndpoints" : "", #No Desc. Object Type: string
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_guestactions.py` & `pyclearpass-1.0.5/pyclearpass/api_guestactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: GuestActions
 # FileName: api_guestactions.py
 
 
 class ApiGuestActions(ClearPassAPILogin):
+
     # API Service: Operations for GenerateGuestDigitalPass
     def get_guest_by_guest_id_pass_id(self, guest_id="", id=""):
         """
         Operation: Generate digital pass for guest account based on template specified by ID
         HTTP Response Codes: 200 OK, 400 Bad Request, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Parameter Type: path, Name: guest_id, Description: Numeric ID of the guest account
         Parameter Type: path, Name: id, Description: Numeric ID of the digital pass template
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_guestconfiguration.py` & `pyclearpass-1.0.5/pyclearpass/api_guestconfiguration.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: GuestConfiguration
 # FileName: api_guestconfiguration.py
 
 
 class ApiGuestConfiguration(ClearPassAPILogin):
+
     # API Service: Manage pass templates
     def get_template_pass(
         self, filter="", sort="", offset="", limit="", calculate_count=""
     ):
         """
         Operation: Get a list of pass templates
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_identities.py` & `pyclearpass-1.0.5/pyclearpass/api_identities.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: Identities
 # FileName: api_identities.py
 
 
 class ApiIdentities(ClearPassAPILogin):
+
     # API Service: Manage API clients at Administration -> API Services -> API Clients
     def get_api_client(
         self, filter="", sort="", offset="", limit="", calculate_count=""
     ):
         """
         Operation: Get a list of API clients
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
@@ -547,31 +548,41 @@
         url_path = _generate_parameterised_url(parameters=dict_query, url=url_path)
         dict_path = {"macaddr": macaddr}
         for item in dict_path:
             url_path = url_path.replace("{" + item + "}", dict_path[item])
         return ClearPassAPILogin._send_request(self, url=url_path, method="delete")
 
     # API Service: Manage endpoints
-    def get_endpoint(self, filter="", sort="", offset="", limit="", calculate_count=""):
+    def get_endpoint(
+        self,
+        filter="",
+        sort="",
+        offset="",
+        limit="",
+        calculate_count="",
+        profile_details="",
+    ):
         """
-        Operation: Get a list of endpoints
+        Operation: Get a list of endpoints along with its profiling information
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Parameter Type (Optional): query, Name: filter, Description: JSON filter expression specifying the items to return
         Parameter Type (Optional): query, Name: sort, Description: Sort ordering for returned items (default +id)
         Parameter Type (Optional): query, Name: offset, Description: Zero based offset to start from
         Parameter Type (Optional): query, Name: limit, Description: Maximum number of items to return (1 – 1000)
         Parameter Type (Optional): query, Name: calculate_count, Description: Whether to calculate the total item count
+        Parameter Type (Optional): query, Name: profile_details, Description: <b>true:</b> Fetch the endpoint profile details as well<br/><b>false:</b> Fetch only endpoint details(default)
         """
         url_path = "/endpoint"
         dict_query = {
             "filter": filter,
             "sort": sort,
             "offset": offset,
             "limit": limit,
             "calculate_count": calculate_count,
+            "profile_details": profile_details,
         }
         url_path = _generate_parameterised_url(parameters=dict_query, url=url_path)
         return ClearPassAPILogin._send_request(self, url=url_path, method="get")
 
     def new_endpoint(self, body=({})):
         """
         Operation: Create a new endpoint
@@ -580,79 +591,87 @@
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "mac_address" : "", #MAC Address of the endpoint. Object Type: string
         "description" : "", #Description of the endpoint. Object Type: string
         "status" : "", #Status of the endpoint. Object Type: string
+        "randomized_mac" : False, #Is MAC address randomized?. Object Type: boolean
         "device_insight_tags" : "", #List of Device Insight Tags. Object Type: string
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the endpoint. Object Type: object
 
         }
         """
         url_path = "/endpoint"
         body = _remove_empty_keys(keys=body)
         return ClearPassAPILogin._send_request(
             self, url=url_path, method="post", query=body
         )
 
-    def get_endpoint_by_endpoint_id(self, endpoint_id=""):
+    def get_endpoint_by_endpoint_id(self, profile_details="", endpoint_id=""):
         """
-        Operation: Get an endpoint
+        Operation: Get an endpoint along with its profiling information
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type
+        Parameter Type (Optional): query, Name: profile_details, Description: <b>true:</b> Fetch the endpoint profile details as well<br/><b>false:</b> Fetch only endpoint details(default)
         Parameter Type: path, Name: endpoint_id, Description: Numeric ID of the endpoint
         """
         url_path = "/endpoint/{endpoint_id}"
+        dict_query = {"profile_details": profile_details}
+        url_path = _generate_parameterised_url(parameters=dict_query, url=url_path)
         dict_path = {"endpoint_id": endpoint_id}
         for item in dict_path:
             url_path = url_path.replace("{" + item + "}", dict_path[item])
         return ClearPassAPILogin._send_request(self, url=url_path, method="get")
 
     def update_endpoint_by_endpoint_id(self, endpoint_id="", body=({})):
         """
-        Operation: Update some fields of an endpoint
+        Operation: Update some fields of an endpoint. Only Device Category/OS Family/Name can be updated as a part of profile details
         HTTP Response Codes: 200 OK, 204 No Content, 304 Not Modified, 401 Unauthorized, 403 Forbidden, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Parameter Type: path, Name: endpoint_id, Description: Numeric ID of the endpoint
         Required Body Parameters: None listed
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "mac_address" : "", #MAC Address of the endpoint. Object Type: string
         "description" : "", #Description of the endpoint. Object Type: string
         "status" : "", #Status of the endpoint. Object Type: string
+        "randomized_mac" : False, #Is MAC address randomized?. Object Type: boolean
         "device_insight_tags" : "", #List of Device Insight Tags. Object Type: string
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the endpoint. Object Type: object
+        "profile" : {}, #Endpoint Profile. Object Type: ProfileUpdate
 
         }
         """
         url_path = "/endpoint/{endpoint_id}"
         dict_path = {"endpoint_id": endpoint_id}
         for item in dict_path:
             url_path = url_path.replace("{" + item + "}", dict_path[item])
         body = _remove_empty_keys(keys=body)
         return ClearPassAPILogin._send_request(
             self, url=url_path, method="patch", query=body
         )
 
     def replace_endpoint_by_endpoint_id(self, endpoint_id="", body=({})):
         """
-        Operation: Replace an endpoint
+        Operation: Replace an endpoint. Only Device Category/OS Family/Name can be modified as a part of profile details
         HTTP Response Codes: 200 OK, 204 No Content, 304 Not Modified, 401 Unauthorized, 403 Forbidden, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Parameter Type: path, Name: endpoint_id, Description: Numeric ID of the endpoint
-        Required Body Parameters:['mac_address', 'status']
+        Required Body Parameters:['mac_address', 'status', 'profile']
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "mac_address" : "", #MAC Address of the endpoint. Object Type: string
         "description" : "", #Description of the endpoint. Object Type: string
         "status" : "", #Status of the endpoint. Object Type: string
+        "randomized_mac" : False, #Is MAC address randomized?. Object Type: boolean
         "device_insight_tags" : "", #List of Device Insight Tags. Object Type: string
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the endpoint. Object Type: object
+        "profile" : {}, #Endpoint Profile. Object Type: ProfileReplace
 
         }
         """
         url_path = "/endpoint/{endpoint_id}"
         dict_path = {"endpoint_id": endpoint_id}
         for item in dict_path:
             url_path = url_path.replace("{" + item + "}", dict_path[item])
@@ -669,68 +688,77 @@
         """
         url_path = "/endpoint/{endpoint_id}"
         dict_path = {"endpoint_id": endpoint_id}
         for item in dict_path:
             url_path = url_path.replace("{" + item + "}", dict_path[item])
         return ClearPassAPILogin._send_request(self, url=url_path, method="delete")
 
-    def get_endpoint_mac_address_by_mac_address(self, mac_address=""):
+    def get_endpoint_mac_address_by_mac_address(
+        self, profile_details="", mac_address=""
+    ):
         """
-        Operation: Get an endpoint by mac_address
+        Operation: Get an endpoint along with its profiling information by mac_address
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type
+        Parameter Type (Optional): query, Name: profile_details, Description: <b>true:</b> Fetch the endpoint profile details as well<br/><b>false:</b> Fetch only endpoint details(default)
         Parameter Type: path, Name: mac_address, Description: Unique mac_address of the endpoint
         """
         url_path = "/endpoint/mac-address/{mac_address}"
+        dict_query = {"profile_details": profile_details}
+        url_path = _generate_parameterised_url(parameters=dict_query, url=url_path)
         dict_path = {"mac_address": mac_address}
         for item in dict_path:
             url_path = url_path.replace("{" + item + "}", dict_path[item])
         return ClearPassAPILogin._send_request(self, url=url_path, method="get")
 
     def update_endpoint_mac_address_by_mac_address(self, mac_address="", body=({})):
         """
-        Operation: Update some fields of an endpoint by mac_address
+        Operation: Update some fields of an endpoint. Only Device Category/OS Family/Name can be updated as a part of profile details by mac_address
         HTTP Response Codes: 200 OK, 204 No Content, 304 Not Modified, 401 Unauthorized, 403 Forbidden, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Parameter Type: path, Name: mac_address, Description: Unique mac_address of the endpoint
         Required Body Parameters: None listed
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "mac_address" : "", #MAC Address of the endpoint. Object Type: string
         "description" : "", #Description of the endpoint. Object Type: string
         "status" : "", #Status of the endpoint. Object Type: string
+        "randomized_mac" : False, #Is MAC address randomized?. Object Type: boolean
         "device_insight_tags" : "", #List of Device Insight Tags. Object Type: string
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the endpoint. Object Type: object
+        "profile" : {}, #Endpoint Profile. Object Type: ProfileUpdate
 
         }
         """
         url_path = "/endpoint/mac-address/{mac_address}"
         dict_path = {"mac_address": mac_address}
         for item in dict_path:
             url_path = url_path.replace("{" + item + "}", dict_path[item])
         body = _remove_empty_keys(keys=body)
         return ClearPassAPILogin._send_request(
             self, url=url_path, method="patch", query=body
         )
 
     def replace_endpoint_mac_address_by_mac_address(self, mac_address="", body=({})):
         """
-        Operation: Replace an endpoint by mac_address
+        Operation: Replace an endpoint. Only Device Category/OS Family/Name can be modified as a part of profile details by mac_address
         HTTP Response Codes: 200 OK, 204 No Content, 304 Not Modified, 401 Unauthorized, 403 Forbidden, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Parameter Type: path, Name: mac_address, Description: Unique mac_address of the endpoint
-        Required Body Parameters:['mac_address', 'status']
+        Required Body Parameters:['mac_address', 'status', 'profile']
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "mac_address" : "", #MAC Address of the endpoint. Object Type: string
         "description" : "", #Description of the endpoint. Object Type: string
         "status" : "", #Status of the endpoint. Object Type: string
+        "randomized_mac" : False, #Is MAC address randomized?. Object Type: boolean
         "device_insight_tags" : "", #List of Device Insight Tags. Object Type: string
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the endpoint. Object Type: object
+        "profile" : {}, #Endpoint Profile. Object Type: ProfileReplace
 
         }
         """
         url_path = "/endpoint/mac-address/{mac_address}"
         dict_path = {"mac_address": mac_address}
         for item in dict_path:
             url_path = url_path.replace("{" + item + "}", dict_path[item])
@@ -1339,16 +1367,18 @@
         HTTP Response Codes: 201 Created, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Required Body Parameters:['user_id', 'password', 'username', 'role_name']
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "user_id" : "", #Unique user id of the local user. Object Type: string
-        "password" : "", #Password of the local user. Object Type: string
         "username" : "", #User name of the local user. Object Type: string
+        "password" : "", #Password of the local user. Object Type: string
+        "password_hash" : "", #Password Hash of the local user. Object Type: string
+        "password_ntlm_hash" : "", #Password NTLM Hash of the local user. Object Type: string
         "role_name" : "", #Role name of the local user. Object Type: string
         "enabled" : False, #Flag indicating if the account is enabled. Object Type: boolean
         "change_pwd_next_login" : False, #Flag indicating if the password change is required in next login. Object Type: boolean
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the local user account. Object Type: object
 
         }
         """
@@ -1377,16 +1407,18 @@
         Parameter Type: path, Name: local_user_id, Description: Numeric ID of the local user
         Required Body Parameters: None listed
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "user_id" : "", #Unique user id of the local user. Object Type: string
-        "password" : "", #Password of the local user. Object Type: string
         "username" : "", #User name of the local user. Object Type: string
+        "password" : "", #Password of the local user. Object Type: string
+        "password_hash" : "", #Password Hash of the local user. Object Type: string
+        "password_ntlm_hash" : "", #Password NTLM Hash of the local user. Object Type: string
         "role_name" : "", #Role name of the local user. Object Type: string
         "enabled" : False, #Flag indicating if the account is enabled. Object Type: boolean
         "change_pwd_next_login" : False, #Flag indicating if the password change is required in next login. Object Type: boolean
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the local user account. Object Type: object
 
         }
         """
@@ -1406,16 +1438,18 @@
         Parameter Type: path, Name: local_user_id, Description: Numeric ID of the local user
         Required Body Parameters:['user_id', 'password', 'username', 'role_name']
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "user_id" : "", #Unique user id of the local user. Object Type: string
-        "password" : "", #Password of the local user. Object Type: string
         "username" : "", #User name of the local user. Object Type: string
+        "password" : "", #Password of the local user. Object Type: string
+        "password_hash" : "", #Password Hash of the local user. Object Type: string
+        "password_ntlm_hash" : "", #Password NTLM Hash of the local user. Object Type: string
         "role_name" : "", #Role name of the local user. Object Type: string
         "enabled" : False, #Flag indicating if the account is enabled. Object Type: boolean
         "change_pwd_next_login" : False, #Flag indicating if the password change is required in next login. Object Type: boolean
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the local user account. Object Type: object
 
         }
         """
@@ -1459,16 +1493,18 @@
         Parameter Type: path, Name: user_id, Description: Unique user_id of the local user
         Required Body Parameters: None listed
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "user_id" : "", #Unique user id of the local user. Object Type: string
-        "password" : "", #Password of the local user. Object Type: string
         "username" : "", #User name of the local user. Object Type: string
+        "password" : "", #Password of the local user. Object Type: string
+        "password_hash" : "", #Password Hash of the local user. Object Type: string
+        "password_ntlm_hash" : "", #Password NTLM Hash of the local user. Object Type: string
         "role_name" : "", #Role name of the local user. Object Type: string
         "enabled" : False, #Flag indicating if the account is enabled. Object Type: boolean
         "change_pwd_next_login" : False, #Flag indicating if the password change is required in next login. Object Type: boolean
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the local user account. Object Type: object
 
         }
         """
@@ -1488,16 +1524,18 @@
         Parameter Type: path, Name: user_id, Description: Unique user_id of the local user
         Required Body Parameters:['user_id', 'password', 'username', 'role_name']
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "user_id" : "", #Unique user id of the local user. Object Type: string
-        "password" : "", #Password of the local user. Object Type: string
         "username" : "", #User name of the local user. Object Type: string
+        "password" : "", #Password of the local user. Object Type: string
+        "password_hash" : "", #Password Hash of the local user. Object Type: string
+        "password_ntlm_hash" : "", #Password NTLM Hash of the local user. Object Type: string
         "role_name" : "", #Role name of the local user. Object Type: string
         "enabled" : False, #Flag indicating if the account is enabled. Object Type: boolean
         "change_pwd_next_login" : False, #Flag indicating if the password change is required in next login. Object Type: boolean
         "attributes" : {}, #Additional attributes(key/value pairs) may be stored with the local user account. Object Type: object
 
         }
         """
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_insight.py` & `pyclearpass-1.0.5/pyclearpass/api_insight.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: Insight
 # FileName: api_insight.py
 
 
 class ApiInsight(ClearPassAPILogin):
+
     # API Service: Operations for Alert
     def get_alert(self, offset="", limit="", calculate_count=""):
         """
         Operation: Get all Insight alert configurations.
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type
         Parameter Type (Optional): query, Name: offset, Description: Starting point to return rows from a result set. i.e Default: 0
         Parameter Type (Optional): query, Name: limit, Description: Limit the number of rows returned from a result set. i.e Default: 25
@@ -373,14 +374,15 @@
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "id" : 0, #Numeric id of the report. Object Type: integer
         "name" : "", #Name of the report. Object Type: string
         "description" : "", #Description of the report. Object Type: string
+        "language" : "", #Language of the report. Object Type: string
         "category" : "", #Category of the report. Object Type: string
         "subcategory" : "", #Sub category is the template name of the report. Object Type: string
         "email_targets" : {}, #Send report to the configured email targets, e.g. "email_targets":["...", "..."]. Object Type: object
         "sms_targets" : {}, #Send report to the configured SMS targets, e.g. "sms_targets":["...", "..."]. Object Type: object
         "copy_remote" : False, #Enable to copy the report to the configured SCP/SFTP server. Object Type: boolean
         "config" : {},      #Setting the report filter configurations & adding CSV columns for the CSV report,     e.g. "config": {     "filter": {     "auth.ap_name": {     "operator": "EQUALS",     "value": ["..."]     },     "cppm_cluster.hostname": {     "operator":"CONTAINS",     "value":["...", "..."]     }     },     csv_cols": ["...", "...", "..."]     #}. Object Type: object
         "schedule" : {},      #Scheduling the report. Options are [noRepeat, daily, weekly, monthly],     e.g. when running the report "now" itself => "schedule": {} - then "begin_dt" & "end_dt" are mandatory,     when scheduling the report at "daily" => "schedule": {"freq": "daily", "hour": 12}     when scheduling the report at "weekly" => "schedule": {"freq": "weekly", "day": 0, "hour": 12}     when scheduling the report at "monthly" => "schedule": {"freq": "monthly", "date": 1, "hour": 12}     #. Object Type: object
@@ -417,14 +419,15 @@
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "id" : 0, #Numeric id of the report. Object Type: integer
         "name" : "", #Name of the report. Object Type: string
         "description" : "", #Description of the report. Object Type: string
+        "language" : "", #Language of the report. Object Type: string
         "category" : "", #Category of the report. Object Type: string
         "subcategory" : "", #Sub category is the template name of the report. Object Type: string
         "email_targets" : {}, #Send report to the configured email targets, e.g. "email_targets":["...", "..."]. Object Type: object
         "sms_targets" : {}, #Send report to the configured SMS targets, e.g. "sms_targets":["...", "..."]. Object Type: object
         "copy_remote" : False, #Enable to copy the report to the configured SCP/SFTP server. Object Type: boolean
         "config" : {},      #Setting the report filter configurations & adding CSV columns for the CSV report,     e.g. "config": {     "filter": {     "auth.ap_name": {     "operator": "EQUALS",     "value": ["..."]     },     "cppm_cluster.hostname": {     "operator":"CONTAINS",     "value":["...", "..."]     }     },     csv_cols": ["...", "...", "..."]     #}. Object Type: object
         "schedule" : {},      #Scheduling the report. Options are [noRepeat, daily, weekly, monthly],     e.g. when running the report "now" itself => "schedule": {} - then "begin_dt" & "end_dt" are mandatory,     when scheduling the report at "daily" => "schedule": {"freq": "daily", "hour": 12}     when scheduling the report at "weekly" => "schedule": {"freq": "weekly", "day": 0, "hour": 12}     when scheduling the report at "monthly" => "schedule": {"freq": "monthly", "date": 1, "hour": 12}     #. Object Type: object
@@ -452,14 +455,15 @@
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "id" : 0, #Numeric id of the report. Object Type: integer
         "name" : "", #Name of the report. Object Type: string
         "description" : "", #Description of the report. Object Type: string
+        "language" : "", #Language of the report. Object Type: string
         "category" : "", #Category of the report. Object Type: string
         "subcategory" : "", #Sub category is the template name of the report. Object Type: string
         "email_targets" : {}, #Send report to the configured email targets, e.g. "email_targets":["...", "..."]. Object Type: object
         "sms_targets" : {}, #Send report to the configured SMS targets, e.g. "sms_targets":["...", "..."]. Object Type: object
         "copy_remote" : False, #Enable to copy the report to the configured SCP/SFTP server. Object Type: boolean
         "config" : {},      #Setting the report filter configurations & adding CSV columns for the CSV report,     e.g. "config": {     "filter": {     "auth.ap_name": {     "operator": "EQUALS",     "value": ["..."]     },     "cppm_cluster.hostname": {     "operator":"CONTAINS",     "value":["...", "..."]     }     },     csv_cols": ["...", "...", "..."]     #}. Object Type: object
         "schedule" : {},      #Scheduling the report. Options are [noRepeat, daily, weekly, monthly],     e.g. when running the report "now" itself => "schedule": {} - then "begin_dt" & "end_dt" are mandatory,     when scheduling the report at "daily" => "schedule": {"freq": "daily", "hour": 12}     when scheduling the report at "weekly" => "schedule": {"freq": "weekly", "day": 0, "hour": 12}     when scheduling the report at "monthly" => "schedule": {"freq": "monthly", "date": 1, "hour": 12}     #. Object Type: object
@@ -511,14 +515,15 @@
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "id" : 0, #Numeric id of the report. Object Type: integer
         "name" : "", #Name of the report. Object Type: string
         "description" : "", #Description of the report. Object Type: string
+        "language" : "", #Language of the report. Object Type: string
         "category" : "", #Category of the report. Object Type: string
         "subcategory" : "", #Sub category is the template name of the report. Object Type: string
         "email_targets" : {}, #Send report to the configured email targets, e.g. "email_targets":["...", "..."]. Object Type: object
         "sms_targets" : {}, #Send report to the configured SMS targets, e.g. "sms_targets":["...", "..."]. Object Type: object
         "copy_remote" : False, #Enable to copy the report to the configured SCP/SFTP server. Object Type: boolean
         "config" : {},      #Setting the report filter configurations & adding CSV columns for the CSV report,     e.g. "config": {     "filter": {     "auth.ap_name": {     "operator": "EQUALS",     "value": ["..."]     },     "cppm_cluster.hostname": {     "operator":"CONTAINS",     "value":["...", "..."]     }     },     csv_cols": ["...", "...", "..."]     #}. Object Type: object
         "schedule" : {},      #Scheduling the report. Options are [noRepeat, daily, weekly, monthly],     e.g. when running the report "now" itself => "schedule": {} - then "begin_dt" & "end_dt" are mandatory,     when scheduling the report at "daily" => "schedule": {"freq": "daily", "hour": 12}     when scheduling the report at "weekly" => "schedule": {"freq": "weekly", "day": 0, "hour": 12}     when scheduling the report at "monthly" => "schedule": {"freq": "monthly", "date": 1, "hour": 12}     #. Object Type: object
@@ -546,14 +551,15 @@
         Parameter Type: body, Name: body
         Body example with descriptions and object types below (type(dict):
 
         body={
         "id" : 0, #Numeric id of the report. Object Type: integer
         "name" : "", #Name of the report. Object Type: string
         "description" : "", #Description of the report. Object Type: string
+        "language" : "", #Language of the report. Object Type: string
         "category" : "", #Category of the report. Object Type: string
         "subcategory" : "", #Sub category is the template name of the report. Object Type: string
         "email_targets" : {}, #Send report to the configured email targets, e.g. "email_targets":["...", "..."]. Object Type: object
         "sms_targets" : {}, #Send report to the configured SMS targets, e.g. "sms_targets":["...", "..."]. Object Type: object
         "copy_remote" : False, #Enable to copy the report to the configured SCP/SFTP server. Object Type: boolean
         "config" : {},      #Setting the report filter configurations & adding CSV columns for the CSV report,     e.g. "config": {     "filter": {     "auth.ap_name": {     "operator": "EQUALS",     "value": ["..."]     },     "cppm_cluster.hostname": {     "operator":"CONTAINS",     "value":["...", "..."]     }     },     csv_cols": ["...", "...", "..."]     #}. Object Type: object
         "schedule" : {},      #Scheduling the report. Options are [noRepeat, daily, weekly, monthly],     e.g. when running the report "now" itself => "schedule": {} - then "begin_dt" & "end_dt" are mandatory,     when scheduling the report at "daily" => "schedule": {"freq": "daily", "hour": 12}     when scheduling the report at "weekly" => "schedule": {"freq": "weekly", "day": 0, "hour": 12}     when scheduling the report at "monthly" => "schedule": {"freq": "monthly", "date": 1, "hour": 12}     #. Object Type: object
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_integrations.py` & `pyclearpass-1.0.5/pyclearpass/api_integrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: Integrations
 # FileName: api_integrations.py
 
 
 class ApiIntegrations(ClearPassAPILogin):
+
     # API Service: Manage Context Server Actions
     def get_context_server_action(
         self, filter="", sort="", offset="", limit="", calculate_count=""
     ):
         """
         Operation: Get a list of Context Server Actions
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_localserverconfiguration.py` & `pyclearpass-1.0.5/pyclearpass/api_localserverconfiguration.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: LocalServerConfiguration
 # FileName: api_localserverconfiguration.py
 
 
 class ApiLocalServerConfiguration(ClearPassAPILogin):
+
     # API Service: Manage Application access controls
     def get_server_access_control_by_server_uuid(self, server_uuid=""):
         """
         Operation: Get all application access controls
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type
         Parameter Type: path, Name: server_uuid, Description: UUID of the server
         """
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_logs.py` & `pyclearpass-1.0.5/pyclearpass/api_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: Logs
 # FileName: api_logs.py
 
 
 class ApiLogs(ClearPassAPILogin):
+
     # API Service: Collection of endpoints
     def get_insight_endpoint_mac_by_mac(self, mac=""):
         """
         Operation: Get a single endpoint by MAC address
         HTTP Response Codes: 200 OK, 404 Not Found, 406 Not Acceptable, 415 Unsupported Media Type
         Parameter Type: path, Name: mac, Description: URL parameter mac
         """
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_platformcertificates.py` & `pyclearpass-1.0.5/pyclearpass/api_platformcertificates.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: PlatformCertificates
 # FileName: api_platformcertificates.py
 
 
 class ApiPlatformCertificates(ClearPassAPILogin):
+
     # API Service: Manage Certificate Signing Requests
     def new_cert_sign_request(self, body=({})):
         """
         Operation: Post a certificate sign request
         HTTP Response Codes: 201 Created, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Required Body Parameters:['subject_CN', 'private_key_password', 'private_key_type', 'digest_algorithm']
         Parameter Type: body, Name: body
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_policyelements.py` & `pyclearpass-1.0.5/pyclearpass/api_policyelements.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: PolicyElements
 # FileName: api_policyelements.py
 
 
 class ApiPolicyElements(ClearPassAPILogin):
+
     # API Service: Manage Application Dictionaries
     def get_application_dictionary(
         self, filter="", sort="", offset="", limit="", calculate_count=""
     ):
         """
         Operation: Get a list of Application Dictionaries
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
@@ -1569,15 +1570,15 @@
     def get_radius_dictionary(
         self, filter="", sort="", offset="", limit="", calculate_count=""
     ):
         """
         Operation: Get a list of RADIUS Dictionaries
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Parameter Type (Optional): query, Name: filter, Description: JSON filter expression specifying the items to return
-        Parameter Type (Optional): query, Name: sort, Description: Sort ordering for returned items (default +id)
+        Parameter Type (Optional): query, Name: sort, Description: Sort ordering for returned items (default +vendor_id)
         Parameter Type (Optional): query, Name: offset, Description: Zero based offset to start from
         Parameter Type (Optional): query, Name: limit, Description: Maximum number of items to return (1 – 1000)
         Parameter Type (Optional): query, Name: calculate_count, Description: Whether to calculate the total item count
         """
         url_path = "/radius-dictionary"
         dict_query = {
             "filter": filter,
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_sessioncontrol.py` & `pyclearpass-1.0.5/pyclearpass/api_sessioncontrol.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: SessionControl
 # FileName: api_sessioncontrol.py
 
 
 class ApiSessionControl(ClearPassAPILogin):
+
     # API Service: Manage active sessions
     def get_session(self, filter="", sort="", offset="", limit="", calculate_count=""):
         """
         Operation: Get a list of active sessions
         HTTP Response Codes: 200 OK, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Parameter Type (Optional): query, Name: filter, Description: JSON filter expression specifying the items to return
         Parameter Type (Optional): query, Name: sort, Description: Sort ordering for returned items (default -id)
```

### Comparing `pyclearpass-1.0.4/pyclearpass/api_toolsandutilities.py` & `pyclearpass-1.0.5/pyclearpass/api_toolsandutilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 
 # API Category Name: ToolsAndUtilities
 # FileName: api_toolsandutilities.py
 
 
 class ApiToolsAndUtilities(ClearPassAPILogin):
+
     # API Service: Operations for Email Send
     def new_email_send(self, body=({})):
         """
         Operation: Send an Email
         HTTP Response Codes: 201 Created, 401 Unauthorized, 403 Forbidden, 406 Not Acceptable, 415 Unsupported Media Type, 422 Unprocessable Entity
         Required Body Parameters:['to', 'message']
         Parameter Type: body, Name: body
```

### Comparing `pyclearpass-1.0.4/pyclearpass/common.py` & `pyclearpass-1.0.5/pyclearpass/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,32 +11,32 @@
         granttype="",
         clientid="",
         clientsecret="",
         username="",
         password="",
         server="",
         api_token="",
-        verify_ssl=False
+        verify_ssl=False,
     ):
         """
         This is the class constructor for the ClearPassModule.
 
         This constructor is required to be created before any modules can be used and must contain the following function arguments:
-        
-        Mandatory Parameters: 
+
+        Mandatory Parameters:
         server (string): Website for ClearPass services example - https://yourserver.network.local:443/api
         verify_ssl (boolean, optional): default value False. Allows use of an invalid SSL certificate.
 
-        Option 1 Parameters - 
+        Option 1 Parameters -
         granttype (string) = ['client_credentials' or 'password' or 'refresh_token']: OAuth2 authentication method,client_id (string): Client ID defined in API Clients,
         clientsecret (string, optional): Client secret, required if the API client is not a public client,
         username (string, optional): Username for authentication, required for grant_type "password",
         password (string, optional): Password for authentication, required for grant_type "password",
-        
-        Option 2 Parameters- 
+
+        Option 2 Parameters-
         api_token = Provide the api_token which is the 'access token'.
 
         }
 
         """
         self.granttype = granttype
         self.clientid = clientid
```

### Comparing `pyclearpass-1.0.4/LICENSE.md` & `pyclearpass-1.0.5/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Aruba, a Hewlett Packard Enterprise company
+Copyright (c) 2024 Aruba, a Hewlett Packard Enterprise company
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyclearpass-1.0.4/README.md` & `pyclearpass-1.0.5/PKG-INFO.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,35 @@
+Metadata-Version: 2.1
+Name: pyclearpass
+Version: 1.0.5
+Summary: This package contains all of the API functions to work with the HPE Aruba Networking ClearPass API. This package been built based on version v6.12 but is always generated on the latest version available to download.  
+Project-URL: Homepage, https://github.com/aruba/pyclearpass
+Author-email: Aruba Automation <aruba-automation@hpe.com>
+License-File: LICENSE
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: System :: Networking
+Requires-Python: >=3.9
+Requires-Dist: requests>=2.24
+Requires-Dist: urllib3>=1.25.10
+Description-Content-Type: text/markdown
+
 # pyclearpass
-## Aruba ClearPass V6.11 SDK
-Aruba ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the Aruba ClearPass REST API environment. Each available REST API command is available for use in this module. All responses from the ClearPass API are in JSON format and any interactions with the API are logged within the Audit Viewer.
+## HPE Aruba Networking ClearPass V6.12 SDK
+Aruba ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the HPE Aruba Networking ClearPass REST API environment. Each available REST API command is available for use in this module. All responses from HPE Aruba Networking ClearPass API are in JSON format (converted into a Python dictionary object) and any interactions with the API are logged within the Audit Viewer.
+
+This package has been uploaded to https://pypi.org/ and is also available to install via https://github.com/aruba/pyclearpass. 
+These instructions are also available at https://developer.arubanetworks.com/aruba-cppm/docs/getting-started-with-pyclearpass.
+Installation instructions and usage instructions are also provided below. 
 
-This package has been uploaded to https://pypi.org/ and is also available to install via https://github.com/aruba/pyclearpass. Installation instructions are provided below. 
 ## Available API Categories  
-The following describes the available top level functionality of the ClearPass API available within this Python Package. 
+The following describes the available top level functionality of the HPE Aruba Networking ClearPass API available within this Python Package. 
 - Operations
 - Certificate Authority
 - Endpoint Visibility 
 - Enforcement Profile
 - Global Server Configuration
 - Guest Actions
 - Guest Configuration
@@ -20,31 +41,32 @@
 - Platform Certificates
 - Policy Elements
 - Session Controls
 - Tools and Utilities
 
 _This package comes without any warranties and should be used at your own risk._
 
-## ClearPass Server Readiness
-These steps list what is required on the ClearPass server:
-1. Make sure you have the API Service enabled within Services. You may use the template to help you do this. 
-2. Create a new API Client within the ClearPass Guest Portal 
+## HPE Aruba Networking ClearPass Server Readiness
+These steps list what is required on the HPE Aruba Networking ClearPass server:
+1. Create a new API Client within the HPE Aruba Networking ClearPass Guest Portal 
     - client id = demo, 
-    - enabled, Operating Mode = Rest API, 
-    - Operator Profile = Pick one with apporpiate permission level or make a new one,  
+    - enabled, Operating Mode = Rest API
+    - Operator Profile = Pick one with apporpiate permission level or make a new one 
     - Grant Type = client credentials
     - Access Token Lifetime = 8 Hours
-3. Optional but preferred, a valid SSL cerfificate
+2. Optional but preferred: valid SSL cerfificate
+3. Optional: API Service enabled within Services. You may use the template to help you do this. Only required when using 'Grant Type' of Password. 
 
-If you need information, refer to the ClearPass configuration documentation for the API account -
-https://developer.arubanetworks.com/aruba-cppm/docs/clearpass-configuration  
+If you need information, refer to the HPE Aruba Networking ClearPass configuration documentation for the API account -
+https://developer.arubanetworks.com/aruba-cppm/docs/clearpass-configuration
 
 # Python Requirements  
 Ensure Python v3.9 or greater is installed on your operating system
-# Package Installation  
+# Package Installation
+
 #### Method 1 - Installing Package from PyPi
 Run the following in a command line terminal to install the pip package - ```pip3 install pyclearpass``` or ```pip install pyclearpass```. This may vary between Operating Systems. 
 
 #### Method 2 - Installing Package from Github (not using Git.exe)
 1. Click into the Aruba Github Repository where the latest version of pyclearpass is located 
 2. Click Code (in green) and Download to Zip
 3. Extract the zip file into a directory
@@ -52,153 +74,269 @@
 5. In your command line terminal type ```python3 -m build``` or ```python -m build```. This will create a folder called dist with a file containing a .gz extension. 
 6. Run the following in a command line terminal to install the pip package - ```pip3 install pathtozip.gz``` or ```pip install pathtozip.gz```. This may vary between Operating Systems.
 
 #### Method 3 - Installing Package from Github (using Git.exe)
 1. Install Git for your Operating System from https://git-scm.com/download
 2. Run the following in a command line terminal to install the pip package - ```pip3 install git+https://github.com/aruba/pyclearpass``` or ```pip install git+https://github.com/aruba/pyclearpass```. This may vary between Operating Systems. 
 
-# Inital Usage Instructions
-Within your Python favourite IDE environment, create an import reference
-```
+# Initial Usage Instructions
+
+Within your favourite Python IDE environment, create an import reference
+
+```python
 from pyclearpass import *
 ```
-Create a object to login into ClearPass. The login object needs to be passed to use any function within the ClearPass API.
+
+Create a object to login into ClearPass. The login object needs to be passed to use any function within the ClearPass API.  
 Two examples below shows how to create the login object (either one can be used, but not both).
-1. Using client_credentials
-```
+
+1. Using client credentials
+
+```python
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",granttype="client_credentials",
 clientsecret="myclientsecretexample", clientid="myclientidexample", verify_ssl=False)
 ```
->The login object will contain the APIToken once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
-2. Using an explicitly defined api_token
-```
+
+> 📘 
+> 
+> The login object will contain the APIToken once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
+
+2. Using an explicitly defined api_token. You can generate an API token by clicking on the API client and then clicking 'Generate Access Token'.
+
+```python
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",api_token="yoursecretapitoken", verify_ssl=False)
 ```
 
+Find an API you want to use, by prefixing  `Api`  in your IDE and Intellisense will show the available APIs available. Each of the top level API category names are available as a module. Once you have chosen a specific API module to use, for example ApiPolicyElements, it will show you the available methods if you suffix a . to the command - `ApiPolicyElements.`
 
-Find an API you want to use, by prefixing  ```Api```  in your IDE and intellisense will show the available APIs available. Each of the top level API category names are available as a module. Once you have chosen a specifc API to use, for example ApiPolicyElements, it will show you the available methods if you suffix a . to the command - ```ApiPolicyElements.```
+The example below prints a single the roles available within the ClearPass server.
 
-The example below prints the roles available within the clearpass server.
-```	
+```python
 print(ApiPolicyElements.get_role(login)) 
 ```
-By default, the example above to return the roles available within the clearpass server will only show the first 25 roles. If you want to view more, you have to adjust the limit. Placing your cursor over the .getRole will usually show you help about the method. 
-```
+
+By default, the example above returns the first 25 roles. To view more, the limit needs to be adjusted. Placing your cursor over the .getRole will usually show you help about the method. 
+
+```python
 print(ApiPolicyElements.get_role(login, limit=100))
 ```
-# Help 
-Once you have written a specific API  ```ApiName.FunctionName(```, placing your cursor over the command will show you help for the function and what the required parameters are (example is Visual Studio Code). The first parameter is always login. 
-You may also read the help for the function by calling ```help(ApiName.FunctionName)```. Each function contains a help section on how to use it. 
+
+# Help
+
+Once you have written a specific API  `ApiName.FunctionName(`, placing your cursor over the command will show you help for the function and what the required parameters are (example is Visual Studio Code). The first parameter is always login.  
+You may also read the help for the function by calling `help(ApiName.function_name)`.  
+Each function contains a help section on how to use it. 
+
 # Python Package Upgrade Instructions
-Once an update is available on the Python PyPi repository, you may upgrade your release by completing the following in a command line terminal - ```pip3 install pyclearpass --upgrade```
+
+Once an update is available on the Python PyPi repository, you may upgrade your release by completing the following in a command line terminal - 
+
+`pip3 install pyclearpass --upgrade`  
+or  
+`pip install pyclearpass --upgrade`
+
+To install a specific version, execute the following command with x.x.x being the specific version number you want to install. 
+
+`pip3 install pyclearpass==x.x.x`  
+or  
+ `pip install pyclearpass==x.x.x`
+ 
 # Uninstall Package Package
-To remove the Python pyclearpass package, type the following command into a command line terminal - ```pip3 uninstall pyclearpass ``` or ```pip uninstall pyclearpass ```
 
-# Release Notes
-Release notes for this version are availble in the [RELEASE-NOTES.md](RELEASE-NOTES.md) file.
+To remove the Python pyclearpass package, type the following command into a command line terminal -  
+`pip3 uninstall pyclearpass `  
+or  
+ `pip uninstall pyclearpass `
 
 # Further Usage Examples
-The examples below all exclude importing the module and creating the login variable. This is described directly below.
 
-## New Login Session
+The examples below all exclude importing the module and creating the login variable. This is described directly below. Note, these are just a full examples, there are hundreds of API commands available within the SDK.
+
+## New Login Session (Mandatory)
+
 The login variable only needs to be defined once in the script. Two examples are shown below to achieve this;
 
 1. Using client_credentials
-```
+
+```python
 from pyclearpass import *
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",granttype="client_credentials",
 clientsecret="myclientsecretexample", clientid="myclientidexample", verify_ssl=False)
 ```
->As mentioned earlier, the login object will contain the API Token once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
 
-2. Using an explicitly defined api_token
-```
+> 📘 
+> 
+> As mentioned earlier, the login object will contain the API Token once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
+
+2. Using an explicitly defined api_token. You can generate an API token by clicking on the API client and then clicking 'Generate Access Token'.
+
+```python
 from pyclearpass import *
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",api_token="yoursecretapitoken", verify_ssl=False)
 ```
 
-## Get Local Server Configuration 
-```
+## Get Local Server Configuration
+
+```python
+import json
 LSCGCS = ApiLocalServerConfiguration.get_cluster_server(login)
 print(json.dumps(LSCGCS['_embedded']['items'],indent=1))
 ```
 
-## Get Total End Point Count 
-```
+## Get Total End Point Count
+
+```python
 IGEP = ApiIdentities.get_endpoint(login, calculate_count='true')
 print("Total MACs in Table: "+str(IGEP['count']))
 ```
 
 ## Get Insight Device Details
-```
+
+```python
 print(ApiLogs.get_insight_endpoint_ip_by_ip(login,ip="192.168.0.99"))
 ```
 
 ## Get list of Admin Users
-```
+
+```python
 AU = ApiGlobalServerConfiguration.get_admin_user(login)
 for users in AU['_embedded']['items']:
   print(users)
 ```
 
-## Get Network Access Device
+## Add New Endpoint
+
+```python
+newEndPoint = {
+  "mac_address": "11:22:33:44:55:66",
+  "description": "Demo EndPoint 1",
+  "status": "Known"
+}
+print(ApiIdentities.new_endpoint(login,body=newEndPoint))
 ```
+
+## Add New Role
+
+```python
+role={"name": "Test1","description": "Test role made using the API Package in Python"}
+print(ApiPolicyElements.new_role(login,body=role))
+```
+
+## Delete Role
+
+```python
+print(ApiPolicyElements.delete_role_name_by_name(login,name='Demo'))
+```
+
+## Get Network Access Device
+
+```python
 devices = ApiPolicyElements.get_network_device(login)
 for device in devices["_embedded"]["items"]:
     print(device)
 ```
 
 ## Get Network Access Device by Name
-```
+
+```python
 print(ApiPolicyElements.get_network_device_name_by_name(login, "Lab-AP-IAP-VC"))
 ```
 
 ## Add New Network Access Device
-```
+
+```python
 newNAD = {
     "description": "LAB AP IAP VC",
     "name": "Lab-AP-IAP-VC",
     "ip_address": "192.168.0.100",
     "radius_secret": "example_radius_secret",
     "tacacs_secret": "example_tacacs_secret",
     "vendor_name": "Aruba",
     "coa_capable": True,
     "coa_port": 3799,
     "attributes": {"Device Type": "IAP"},
 }
-print(ApiPolicyElements.new_network_device(login, body=newNAD))
+ApiPolicyElements.new_network_device(login, body=newNAD)
 ```
 
-## Add New Endpoint
-```
-newEndPoint = {
-  "mac_address": "11:22:33:44:55:66",
-  "description": "Demo EndPoint 1",
-  "status": "Known"
-}
-print(ApiIdentities.new_endpoint(login,body=newEndPoint))
-```
+## Add New Network Access Device via CSV
+
+This example adds new Network Access Devices based on the CSV (comma delimited values) named "network access devices.csv" with headings and content filled rows. 
+
+| name  | description    | ip_address    | location |
+| :---- | :------------- | :------------ | :------- |
+| demo1 | example demo 1 | 192.168.100.1 | UK       |
+| demo2 | example demo 2 | 192.168.100.2 | US       |
+
+```python
+import pandas as pd
+df = pd.read_csv("network access devices.csv")
+
+for index, items in df.iterrows():
+    newnad = {
+        "description": items["description"],  # Description of the network device. Object Type: string
+        "name": items["name"],  # Name of the network device. Object Type: string
+        "ip_address": items["ip_address"],  # IP or Subnet Address of the network device. Object Type: string
+        "tacacs_secret": "testing123",  # TACACS+ Shared Secret of the network device. Object Type: string
+        "vendor_name": "Aruba",  # Vendor Name of the network device. Object Type: string
+        "attributes": {"Location": items["location"]},
+    }
+    print(ApiPolicyElements.new_network_device(login, body=newnad))
+    print(items["name"], items["ip_address"])
 
-## Add New Role
-```
-role={"name": "Test1","description": "Test role made using the API Package in Python"}
-print(ApiPolicyElements.new_role(login,body=role))
 ```
 
-## Delete Role
+## Update Network Access Device via CSV
+
+This example updates Network Access Devices attributes based on the CSV (comma delimited values) named "network access devices updates.csv" with headings and content filled rows. 
+
+| name  | description    | location |
+| :---- | :------------- | :------- |
+| demo1 | updated demo 1 | US       |
+| demo2 | updated demo 2 | UK       |
+
+```python
+import pandas as pd
+df = pd.read_csv("network access devices updates.csv")
+for index, items in df.iterrows():
+    nadupdate = {                
+        "tacacs_secret": "updatedpassword123",  # TACACS+ Shared Secret of the network device. Object Type: string
+        "description": items["description"],  # Description of the network device. Object Type: string
+        "attributes": {"Location": items["location"]},
+    }
+    print(ApiPolicyElements.update_network_device_name_by_name(login,name=items["name"],body=nadupdate))
+
 ```
-print(ApiPolicyElements.delete_role_name_by_name(login,name='Demo'))
+
+## Update Network Device Group
+
+This example updates an Network Device Group with additional IP Addresses 192.168.0.100 and 192.168.0.99.  
+These Network Access Devices must of been added before they can be appended to the group.  
+
+```python
+getcurrentnads = ApiPolicyElements.get_network_device_group_name_by_name(login,name="Example")
+newnads={"value" : "192.168.0.100, 192.168.0.98"}
+newnads["value"]=getcurrentnads['value']+", "+newnads["value"]
+print(ApiPolicyElements.update_network_device_group_name_by_name(login,name="Example",body=newnads))
+
 ```
 
-## Add New Guest Device 
+> 🚧 Ensure completion of validation checks
+> 
+> Validate the Network Access Device exists and is not already part of the Network Device Group before attempting to append to the group.
+
+## Add New Guest Device
+
 This example adds a Guest Device including 
+
 1. An expiry date within 24 hours in seconds 
 2. Associated to the role ID of 3 (Guest in test environment)
 3. Statically assigned MPSK password
-```
+
+```python
 import time
 new_guest_device = {
   "enabled": True,
   "expire_time": int(time.time()) + 86400,
   "mac": "11:22:22:33:33:11",
   "notes": "Created by API Test Script",
   "role_id": 3,
@@ -208,28 +346,31 @@
   "mpsk_enable":"1"
 }
 new_device= ApiIdentities.new_device(login,body=new_guest_device)
 print(new_device)
 ```
 
 ## Get Guest Device by MAC
-```
+
+```python
 import json
 get_mac_address = "11-22-33-33-22-11"
 view_guest_device = ApiIdentities.get_device_mac_by_macaddr(login,get_mac_address)
 print(json.dumps(view_guest_device,indent=2))
 ```
 
 ## Delete an Enforcement Policy
-```
+
+```python
 print(ApiPolicyElements.delete_enforcement_policy_by_enforcement_policy_id(login,enforcement_policy_id='3058'))
 ```
 
-## Create a new Enforcement Policy with staged initial rules and then a loop to create additional rules. 
-```
+## Create a new Enforcement Policy with staged initial rules and then a loop to create additional rules.
+
+```python
 newEnforcementPolicy= {
   "name": "MPSK Demo",
   "description": "MPSK Enforcement",
   "enforcement_type": "RADIUS",
   "default_enforcement_profile": "Deny Device",
   "rule_eval_algo": "first-applicable",
   "rules": ''}
@@ -270,18 +411,23 @@
     
     newEnforcementPolicyRules["rules"].append(epf) 
  
 newEnforcementPolicy["rules"] = newEnforcementPolicyRules["rules"]
 print(ApiPolicyElements.new_enforcement_policy(login,body=newEnforcementPolicy))
 ```
 
->Note - you may find it easier to initially pull a working Enforcement Policy with minimal rules before trying to create a new one from scratch. For example, the rule evaluation in the GUI shows as 'First applicable', however in the backend it is shown as 'first-applicable'. This example is a working policy. It is demonstrated with a loop which could read an entry in a CSV file if adapted. 
+> 📘 
+> 
+> You may find it easier to initially pull a working Enforcement Policy with minimal rules before trying to create a new one from scratch. 
+> 
+> For example, the rule evaluation in the GUI shows as 'First applicable', however in the back-end it is shown as 'first-applicable'. This example is a working policy. It is demonstrated with a loop which could read an entry in a CSV file if adapted.
 
-## Update an existing Enforcement Policy, retaining the original items and using a loop to add additional items 
-```
+## Update an existing Enforcement Policy, retaining the original items and using a loop to add additional items
+
+```python
 epol = ApiPolicyElements.get_enforcement_policy_name_by_name(login, name="MPSK Enforcement")
 OriginalRules = epol["rules"]
 CombinedRules =({"rules":[]})
 for item in range(len(OriginalRules)):
     CombinedRules["rules"].append(OriginalRules[item])
 
 for no in range(9,11):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyclearpass-1.0.4/pyproject.toml` & `pyclearpass-1.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "pyclearpass"
-version = "1.0.4"
+version = "1.0.5"
 authors = [{ name="Aruba Automation", email="aruba-automation@hpe.com" }]
 dependencies = ["requests >=2.24","urllib3 >=1.25.10"]
-description = "Aruba ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the Aruba ClearPass REST API environment. Each available REST API command is available for use in this module."
+description = "HPE Aruba Networking ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the HPE Aruba Networking ClearPass REST API environment. Each available REST API command is available for use in this module."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 	"Intended Audience :: System Administrators",
     "Topic :: System :: Networking",
     "Development Status :: 5 - Production/Stable"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/aruba/pyclearpass"
+"homepage" = "https://developer.arubanetworks.com/aruba-cppm/docs/getting-started-with-pyclearpass"
+"repository" = "https://github.com/aruba/pyclearpass"
+"changelog" = "https://github.com/aruba/pyclearpass/blob/main/RELEASE-NOTES.md"
```

### Comparing `pyclearpass-1.0.4/PKG-INFO` & `pyclearpass-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pyclearpass
-Version: 1.0.4
-Summary: Aruba ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the Aruba ClearPass REST API environment. Each available REST API command is available for use in this module.
-Project-URL: Homepage, https://github.com/aruba/pyclearpass
+Version: 1.0.5
+Summary: HPE Aruba Networking ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the HPE Aruba Networking ClearPass REST API environment. Each available REST API command is available for use in this module.
+Project-URL: homepage, https://developer.arubanetworks.com/aruba-cppm/docs/getting-started-with-pyclearpass
+Project-URL: repository, https://github.com/aruba/pyclearpass
+Project-URL: changelog, https://github.com/aruba/pyclearpass/blob/main/RELEASE-NOTES.md
 Author-email: Aruba Automation <aruba-automation@hpe.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.9
 Requires-Dist: requests>=2.24
 Requires-Dist: urllib3>=1.25.10
 Description-Content-Type: text/markdown
 
 # pyclearpass
-## Aruba ClearPass V6.11 SDK
-Aruba ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the Aruba ClearPass REST API environment. Each available REST API command is available for use in this module. All responses from the ClearPass API are in JSON format and any interactions with the API are logged within the Audit Viewer.
+## HPE Aruba Networking ClearPass V6.12 SDK
+Aruba ClearPass SDK has been developed in Python v3.9 to utilise the full functionality of the HPE Aruba Networking ClearPass REST API environment. Each available REST API command is available for use in this module. All responses from HPE Aruba Networking ClearPass API are in JSON format (converted into a Python dictionary object) and any interactions with the API are logged within the Audit Viewer.
+
+This package has been uploaded to https://pypi.org/ and is also available to install via https://github.com/aruba/pyclearpass. 
+These instructions are also available at https://developer.arubanetworks.com/aruba-cppm/docs/getting-started-with-pyclearpass.
+Installation instructions and usage instructions are also provided below. 
 
-This package has been uploaded to https://pypi.org/ and is also available to install via https://github.com/aruba/pyclearpass. Installation instructions are provided below. 
 ## Available API Categories  
-The following describes the available top level functionality of the ClearPass API available within this Python Package. 
+The following describes the available top level functionality of the HPE Aruba Networking ClearPass API available within this Python Package. 
 - Operations
 - Certificate Authority
 - Endpoint Visibility 
 - Enforcement Profile
 - Global Server Configuration
 - Guest Actions
 - Guest Configuration
@@ -38,31 +43,32 @@
 - Platform Certificates
 - Policy Elements
 - Session Controls
 - Tools and Utilities
 
 _This package comes without any warranties and should be used at your own risk._
 
-## ClearPass Server Readiness
-These steps list what is required on the ClearPass server:
-1. Make sure you have the API Service enabled within Services. You may use the template to help you do this. 
-2. Create a new API Client within the ClearPass Guest Portal 
+## HPE Aruba Networking ClearPass Server Readiness
+These steps list what is required on the HPE Aruba Networking ClearPass server:
+1. Create a new API Client within the HPE Aruba Networking ClearPass Guest Portal 
     - client id = demo, 
-    - enabled, Operating Mode = Rest API, 
-    - Operator Profile = Pick one with apporpiate permission level or make a new one,  
+    - enabled, Operating Mode = Rest API
+    - Operator Profile = Pick one with apporpiate permission level or make a new one 
     - Grant Type = client credentials
     - Access Token Lifetime = 8 Hours
-3. Optional but preferred, a valid SSL cerfificate
+2. Optional but preferred: valid SSL cerfificate
+3. Optional: API Service enabled within Services. You may use the template to help you do this. Only required when using 'Grant Type' of Password. 
 
-If you need information, refer to the ClearPass configuration documentation for the API account -
-https://developer.arubanetworks.com/aruba-cppm/docs/clearpass-configuration  
+If you need information, refer to the HPE Aruba Networking ClearPass configuration documentation for the API account -
+https://developer.arubanetworks.com/aruba-cppm/docs/clearpass-configuration
 
 # Python Requirements  
 Ensure Python v3.9 or greater is installed on your operating system
-# Package Installation  
+# Package Installation
+
 #### Method 1 - Installing Package from PyPi
 Run the following in a command line terminal to install the pip package - ```pip3 install pyclearpass``` or ```pip install pyclearpass```. This may vary between Operating Systems. 
 
 #### Method 2 - Installing Package from Github (not using Git.exe)
 1. Click into the Aruba Github Repository where the latest version of pyclearpass is located 
 2. Click Code (in green) and Download to Zip
 3. Extract the zip file into a directory
@@ -70,153 +76,269 @@
 5. In your command line terminal type ```python3 -m build``` or ```python -m build```. This will create a folder called dist with a file containing a .gz extension. 
 6. Run the following in a command line terminal to install the pip package - ```pip3 install pathtozip.gz``` or ```pip install pathtozip.gz```. This may vary between Operating Systems.
 
 #### Method 3 - Installing Package from Github (using Git.exe)
 1. Install Git for your Operating System from https://git-scm.com/download
 2. Run the following in a command line terminal to install the pip package - ```pip3 install git+https://github.com/aruba/pyclearpass``` or ```pip install git+https://github.com/aruba/pyclearpass```. This may vary between Operating Systems. 
 
-# Inital Usage Instructions
-Within your Python favourite IDE environment, create an import reference
-```
+# Initial Usage Instructions
+
+Within your favourite Python IDE environment, create an import reference
+
+```python
 from pyclearpass import *
 ```
-Create a object to login into ClearPass. The login object needs to be passed to use any function within the ClearPass API.
+
+Create a object to login into ClearPass. The login object needs to be passed to use any function within the ClearPass API.  
 Two examples below shows how to create the login object (either one can be used, but not both).
-1. Using client_credentials
-```
+
+1. Using client credentials
+
+```python
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",granttype="client_credentials",
 clientsecret="myclientsecretexample", clientid="myclientidexample", verify_ssl=False)
 ```
->The login object will contain the APIToken once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
-2. Using an explicitly defined api_token
-```
+
+> 📘 
+> 
+> The login object will contain the APIToken once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
+
+2. Using an explicitly defined api_token. You can generate an API token by clicking on the API client and then clicking 'Generate Access Token'.
+
+```python
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",api_token="yoursecretapitoken", verify_ssl=False)
 ```
 
+Find an API you want to use, by prefixing  `Api`  in your IDE and Intellisense will show the available APIs available. Each of the top level API category names are available as a module. Once you have chosen a specific API module to use, for example ApiPolicyElements, it will show you the available methods if you suffix a . to the command - `ApiPolicyElements.`
 
-Find an API you want to use, by prefixing  ```Api```  in your IDE and intellisense will show the available APIs available. Each of the top level API category names are available as a module. Once you have chosen a specifc API to use, for example ApiPolicyElements, it will show you the available methods if you suffix a . to the command - ```ApiPolicyElements.```
+The example below prints a single the roles available within the ClearPass server.
 
-The example below prints the roles available within the clearpass server.
-```	
+```python
 print(ApiPolicyElements.get_role(login)) 
 ```
-By default, the example above to return the roles available within the clearpass server will only show the first 25 roles. If you want to view more, you have to adjust the limit. Placing your cursor over the .getRole will usually show you help about the method. 
-```
+
+By default, the example above returns the first 25 roles. To view more, the limit needs to be adjusted. Placing your cursor over the .getRole will usually show you help about the method. 
+
+```python
 print(ApiPolicyElements.get_role(login, limit=100))
 ```
-# Help 
-Once you have written a specific API  ```ApiName.FunctionName(```, placing your cursor over the command will show you help for the function and what the required parameters are (example is Visual Studio Code). The first parameter is always login. 
-You may also read the help for the function by calling ```help(ApiName.FunctionName)```. Each function contains a help section on how to use it. 
+
+# Help
+
+Once you have written a specific API  `ApiName.FunctionName(`, placing your cursor over the command will show you help for the function and what the required parameters are (example is Visual Studio Code). The first parameter is always login.  
+You may also read the help for the function by calling `help(ApiName.function_name)`.  
+Each function contains a help section on how to use it. 
+
 # Python Package Upgrade Instructions
-Once an update is available on the Python PyPi repository, you may upgrade your release by completing the following in a command line terminal - ```pip3 install pyclearpass --upgrade```
+
+Once an update is available on the Python PyPi repository, you may upgrade your release by completing the following in a command line terminal - 
+
+`pip3 install pyclearpass --upgrade`  
+or  
+`pip install pyclearpass --upgrade`
+
+To install a specific version, execute the following command with x.x.x being the specific version number you want to install. 
+
+`pip3 install pyclearpass==x.x.x`  
+or  
+ `pip install pyclearpass==x.x.x`
+ 
 # Uninstall Package Package
-To remove the Python pyclearpass package, type the following command into a command line terminal - ```pip3 uninstall pyclearpass ``` or ```pip uninstall pyclearpass ```
 
-# Release Notes
-Release notes for this version are availble in the [RELEASE-NOTES.md](RELEASE-NOTES.md) file.
+To remove the Python pyclearpass package, type the following command into a command line terminal -  
+`pip3 uninstall pyclearpass `  
+or  
+ `pip uninstall pyclearpass `
 
 # Further Usage Examples
-The examples below all exclude importing the module and creating the login variable. This is described directly below.
 
-## New Login Session
+The examples below all exclude importing the module and creating the login variable. This is described directly below. Note, these are just a full examples, there are hundreds of API commands available within the SDK.
+
+## New Login Session (Mandatory)
+
 The login variable only needs to be defined once in the script. Two examples are shown below to achieve this;
 
 1. Using client_credentials
-```
+
+```python
 from pyclearpass import *
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",granttype="client_credentials",
 clientsecret="myclientsecretexample", clientid="myclientidexample", verify_ssl=False)
 ```
->As mentioned earlier, the login object will contain the API Token once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
 
-2. Using an explicitly defined api_token
-```
+> 📘 
+> 
+> As mentioned earlier, the login object will contain the API Token once any function has been used. It obtains it once for the session and uses the same token through the execution of the rest of the script. You can extract this token and reuse it for other sessions if required (login.api_token). The token will only be available for reuse until the lifetime expires which was configured when specifying a new API Client within the ClearPass Guest Module.
+
+2. Using an explicitly defined api_token. You can generate an API token by clicking on the API client and then clicking 'Generate Access Token'.
+
+```python
 from pyclearpass import *
 login = ClearPassAPILogin(server="https://yourserver.network.local:443/api",api_token="yoursecretapitoken", verify_ssl=False)
 ```
 
-## Get Local Server Configuration 
-```
+## Get Local Server Configuration
+
+```python
+import json
 LSCGCS = ApiLocalServerConfiguration.get_cluster_server(login)
 print(json.dumps(LSCGCS['_embedded']['items'],indent=1))
 ```
 
-## Get Total End Point Count 
-```
+## Get Total End Point Count
+
+```python
 IGEP = ApiIdentities.get_endpoint(login, calculate_count='true')
 print("Total MACs in Table: "+str(IGEP['count']))
 ```
 
 ## Get Insight Device Details
-```
+
+```python
 print(ApiLogs.get_insight_endpoint_ip_by_ip(login,ip="192.168.0.99"))
 ```
 
 ## Get list of Admin Users
-```
+
+```python
 AU = ApiGlobalServerConfiguration.get_admin_user(login)
 for users in AU['_embedded']['items']:
   print(users)
 ```
 
-## Get Network Access Device
+## Add New Endpoint
+
+```python
+newEndPoint = {
+  "mac_address": "11:22:33:44:55:66",
+  "description": "Demo EndPoint 1",
+  "status": "Known"
+}
+print(ApiIdentities.new_endpoint(login,body=newEndPoint))
+```
+
+## Add New Role
+
+```python
+role={"name": "Test1","description": "Test role made using the API Package in Python"}
+print(ApiPolicyElements.new_role(login,body=role))
+```
+
+## Delete Role
+
+```python
+print(ApiPolicyElements.delete_role_name_by_name(login,name='Demo'))
 ```
+
+## Get Network Access Device
+
+```python
 devices = ApiPolicyElements.get_network_device(login)
 for device in devices["_embedded"]["items"]:
     print(device)
 ```
 
 ## Get Network Access Device by Name
-```
+
+```python
 print(ApiPolicyElements.get_network_device_name_by_name(login, "Lab-AP-IAP-VC"))
 ```
 
 ## Add New Network Access Device
-```
+
+```python
 newNAD = {
     "description": "LAB AP IAP VC",
     "name": "Lab-AP-IAP-VC",
     "ip_address": "192.168.0.100",
     "radius_secret": "example_radius_secret",
     "tacacs_secret": "example_tacacs_secret",
     "vendor_name": "Aruba",
     "coa_capable": True,
     "coa_port": 3799,
     "attributes": {"Device Type": "IAP"},
 }
-print(ApiPolicyElements.new_network_device(login, body=newNAD))
+ApiPolicyElements.new_network_device(login, body=newNAD)
 ```
 
-## Add New Endpoint
-```
-newEndPoint = {
-  "mac_address": "11:22:33:44:55:66",
-  "description": "Demo EndPoint 1",
-  "status": "Known"
-}
-print(ApiIdentities.new_endpoint(login,body=newEndPoint))
-```
+## Add New Network Access Device via CSV
+
+This example adds new Network Access Devices based on the CSV (comma delimited values) named "network access devices.csv" with headings and content filled rows. 
+
+| name  | description    | ip_address    | location |
+| :---- | :------------- | :------------ | :------- |
+| demo1 | example demo 1 | 192.168.100.1 | UK       |
+| demo2 | example demo 2 | 192.168.100.2 | US       |
+
+```python
+import pandas as pd
+df = pd.read_csv("network access devices.csv")
+
+for index, items in df.iterrows():
+    newnad = {
+        "description": items["description"],  # Description of the network device. Object Type: string
+        "name": items["name"],  # Name of the network device. Object Type: string
+        "ip_address": items["ip_address"],  # IP or Subnet Address of the network device. Object Type: string
+        "tacacs_secret": "testing123",  # TACACS+ Shared Secret of the network device. Object Type: string
+        "vendor_name": "Aruba",  # Vendor Name of the network device. Object Type: string
+        "attributes": {"Location": items["location"]},
+    }
+    print(ApiPolicyElements.new_network_device(login, body=newnad))
+    print(items["name"], items["ip_address"])
 
-## Add New Role
-```
-role={"name": "Test1","description": "Test role made using the API Package in Python"}
-print(ApiPolicyElements.new_role(login,body=role))
 ```
 
-## Delete Role
+## Update Network Access Device via CSV
+
+This example updates Network Access Devices attributes based on the CSV (comma delimited values) named "network access devices updates.csv" with headings and content filled rows. 
+
+| name  | description    | location |
+| :---- | :------------- | :------- |
+| demo1 | updated demo 1 | US       |
+| demo2 | updated demo 2 | UK       |
+
+```python
+import pandas as pd
+df = pd.read_csv("network access devices updates.csv")
+for index, items in df.iterrows():
+    nadupdate = {                
+        "tacacs_secret": "updatedpassword123",  # TACACS+ Shared Secret of the network device. Object Type: string
+        "description": items["description"],  # Description of the network device. Object Type: string
+        "attributes": {"Location": items["location"]},
+    }
+    print(ApiPolicyElements.update_network_device_name_by_name(login,name=items["name"],body=nadupdate))
+
 ```
-print(ApiPolicyElements.delete_role_name_by_name(login,name='Demo'))
+
+## Update Network Device Group
+
+This example updates an Network Device Group with additional IP Addresses 192.168.0.100 and 192.168.0.99.  
+These Network Access Devices must of been added before they can be appended to the group.  
+
+```python
+getcurrentnads = ApiPolicyElements.get_network_device_group_name_by_name(login,name="Example")
+newnads={"value" : "192.168.0.100, 192.168.0.98"}
+newnads["value"]=getcurrentnads['value']+", "+newnads["value"]
+print(ApiPolicyElements.update_network_device_group_name_by_name(login,name="Example",body=newnads))
+
 ```
 
-## Add New Guest Device 
+> 🚧 Ensure completion of validation checks
+> 
+> Validate the Network Access Device exists and is not already part of the Network Device Group before attempting to append to the group.
+
+## Add New Guest Device
+
 This example adds a Guest Device including 
+
 1. An expiry date within 24 hours in seconds 
 2. Associated to the role ID of 3 (Guest in test environment)
 3. Statically assigned MPSK password
-```
+
+```python
 import time
 new_guest_device = {
   "enabled": True,
   "expire_time": int(time.time()) + 86400,
   "mac": "11:22:22:33:33:11",
   "notes": "Created by API Test Script",
   "role_id": 3,
@@ -226,28 +348,31 @@
   "mpsk_enable":"1"
 }
 new_device= ApiIdentities.new_device(login,body=new_guest_device)
 print(new_device)
 ```
 
 ## Get Guest Device by MAC
-```
+
+```python
 import json
 get_mac_address = "11-22-33-33-22-11"
 view_guest_device = ApiIdentities.get_device_mac_by_macaddr(login,get_mac_address)
 print(json.dumps(view_guest_device,indent=2))
 ```
 
 ## Delete an Enforcement Policy
-```
+
+```python
 print(ApiPolicyElements.delete_enforcement_policy_by_enforcement_policy_id(login,enforcement_policy_id='3058'))
 ```
 
-## Create a new Enforcement Policy with staged initial rules and then a loop to create additional rules. 
-```
+## Create a new Enforcement Policy with staged initial rules and then a loop to create additional rules.
+
+```python
 newEnforcementPolicy= {
   "name": "MPSK Demo",
   "description": "MPSK Enforcement",
   "enforcement_type": "RADIUS",
   "default_enforcement_profile": "Deny Device",
   "rule_eval_algo": "first-applicable",
   "rules": ''}
@@ -288,18 +413,23 @@
     
     newEnforcementPolicyRules["rules"].append(epf) 
  
 newEnforcementPolicy["rules"] = newEnforcementPolicyRules["rules"]
 print(ApiPolicyElements.new_enforcement_policy(login,body=newEnforcementPolicy))
 ```
 
->Note - you may find it easier to initially pull a working Enforcement Policy with minimal rules before trying to create a new one from scratch. For example, the rule evaluation in the GUI shows as 'First applicable', however in the backend it is shown as 'first-applicable'. This example is a working policy. It is demonstrated with a loop which could read an entry in a CSV file if adapted. 
+> 📘 
+> 
+> You may find it easier to initially pull a working Enforcement Policy with minimal rules before trying to create a new one from scratch. 
+> 
+> For example, the rule evaluation in the GUI shows as 'First applicable', however in the back-end it is shown as 'first-applicable'. This example is a working policy. It is demonstrated with a loop which could read an entry in a CSV file if adapted.
 
-## Update an existing Enforcement Policy, retaining the original items and using a loop to add additional items 
-```
+## Update an existing Enforcement Policy, retaining the original items and using a loop to add additional items
+
+```python
 epol = ApiPolicyElements.get_enforcement_policy_name_by_name(login, name="MPSK Enforcement")
 OriginalRules = epol["rules"]
 CombinedRules =({"rules":[]})
 for item in range(len(OriginalRules)):
     CombinedRules["rules"].append(OriginalRules[item])
 
 for no in range(9,11):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

