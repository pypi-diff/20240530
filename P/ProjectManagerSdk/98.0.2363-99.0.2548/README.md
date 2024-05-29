# Comparing `tmp/projectmanagersdk-98.0.2363.tar.gz` & `tmp/projectmanagersdk-99.0.2548.tar.gz`

## Comparing `projectmanagersdk-98.0.2363.tar` & `projectmanagersdk-99.0.2548.tar`

### file list

```diff
@@ -1,144 +1,146 @@
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/.github/workflows/publish.yml
--rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/__init__.py
--rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/projectmanagerclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/__init__.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/apikeyclient.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/changesetclient.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/dashboardclient.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/discussionclient.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/fileclient.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/homefileclient.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/integrationcategoryclient.py
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/integrationclient.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/integrationproviderclient.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/licenseclient.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/meclient.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectchargecodeclient.py
--rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectclient.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectcustomerclient.py
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectfieldclient.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectfileclient.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectfolderclient.py
--rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectmembersclient.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectpriorityclient.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectstatusclient.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projecttemplateclient.py
--rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/resourceclient.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/resourceskillclient.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/resourceteamclient.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/tagclient.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskassigneeclient.py
--rw-r--r--   0        0        0    13427 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskclient.py
--rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskfieldclient.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskfileclient.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskstatusclient.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/tasktagclient.py
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/timesheetclient.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/userroleclient.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/workspaceclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/__init__.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/apikeycreatedto.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/apikeydto.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/assigneeupsertdto.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/astroerror.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/astroresult.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/authenticationdto.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/authenticationstatusdto.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/changesetgetresponsedto.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/changesetstatusdto.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/connectionschemadto.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createprojectfielddto.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createprojectfieldresponsedto.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createresourceskilldto.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createresourceteamdto.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createtaskfieldrequestdto.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/dashboardsettingcreatedto.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/dashboardsettingdto.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/deleteprojectfielddto.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/directlinkdto.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/discussioncreatedto.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/discussioncreateresponsedto.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/discussiondto.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/discussionemoji.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/filedto.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/getprojectfieldsresponsedto.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/gettaskfieldsresponsedto.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/iddto.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationauthsetupdto.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationcategorydto.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationdto.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationinstancedto.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationproviderdto.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/licensedto.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/namedto.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odataentitysetinfo.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odatafunctionimportinfo.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odataservicedocument.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odatasingletoninfo.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odatatypeannotation.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/permissionoptionsdto.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectchargecodedto.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectcreateaccessdto.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectcreateaccessmemberdto.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectcreatedto.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectcustomerdto.py
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectdto.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectfieldsvalueresponsedto.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectfolderdto.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectmanagerdto.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectmemberdto.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectmemberroledto.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectprioritydto.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectstatusdto.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projecttemplatecategorydto.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projecttemplatedto.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectupdatedto.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/reactgridlayoutdto.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/reactgridlayoutitemdto.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourceapproverdto.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourcecreatedto.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourcedto.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourceskilldto.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourceteamdto.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourceupdatedto.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tagcreatedto.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tagdto.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tagupdatedto.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskassigneedto.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskcreatedto.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskdetailsdto.py
--rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskdto.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskfielddto.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskfieldsvalueresponsedto.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskprioritydto.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskprojectdto.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskstatuscreatedto.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskstatusdto.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskstatusupdatedto.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tasktagdto.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tasktododto.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskupdatedto.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetadmintypedto.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetcreaterequestdto.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetdto.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetprojectdto.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetresourcedto.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetresponsedto.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheettaskdto.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetupdaterequestdto.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updateprojectfieldvaluedto.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updaterequestdto.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updateresourceskilldto.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updateresourceteamdto.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updatetaskfieldvaluedto.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/userroledto.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/workspacedto.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/workspacejoindto.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/workspacelinksdto.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/workspaceuserinfodto.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/tests/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/LICENSE
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/README.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/pyproject.toml
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 projectmanagersdk-98.0.2363/PKG-INFO
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/.github/workflows/publish.yml
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/__init__.py
+-rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/projectmanagerclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/__init__.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/apikeyclient.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/changesetclient.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/dashboardclient.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/discussionclient.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/fileclient.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/homefileclient.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/integrationcategoryclient.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/integrationclient.py
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/integrationproviderclient.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/licenseclient.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/meclient.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectchargecodeclient.py
+-rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectclient.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectcustomerclient.py
+-rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectfieldclient.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectfileclient.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectfolderclient.py
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectmembersclient.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectpriorityclient.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectstatusclient.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projecttemplateclient.py
+-rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/resourceclient.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/resourceskillclient.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/resourceteamclient.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/tagclient.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskassigneeclient.py
+-rw-r--r--   0        0        0    13332 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskclient.py
+-rw-r--r--   0        0        0    13196 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskfieldclient.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskfileclient.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskstatusclient.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/tasktagclient.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/teamsclient.py
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/timesheetclient.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/userroleclient.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/workspaceclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/__init__.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/apikeycreatedto.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/apikeydto.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/assigneeupsertdto.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/astroerror.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/astroresult.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/authenticationdto.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/authenticationstatusdto.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/changesetgetresponsedto.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/changesetstatusdto.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/connectionschemadto.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createprojectfielddto.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createprojectfieldresponsedto.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createresourceskilldto.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createresourceteamdto.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createtaskfielddto.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/dashboardsettingcreatedto.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/dashboardsettingdto.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/directlinkdto.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/discussioncreatedto.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/discussioncreateresponsedto.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/discussiondto.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/discussionemoji.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/filedto.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/getprojectfieldsresponsedto.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/iddto.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationauthsetupdto.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationcategorydto.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationconnectionschemeobjectdto.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationdto.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationinstancedto.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationproviderdto.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/licensedto.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/masterconnectionschemedto.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/namedto.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odataentitysetinfo.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odatafunctionimportinfo.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odataservicedocument.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odatasingletoninfo.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odatatypeannotation.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/permissionoptionsdto.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectchargecodedto.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectcreateaccessdto.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectcreateaccessmemberdto.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectcreatedto.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectcustomerdto.py
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectdto.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectfieldsvalueresponsedto.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectfolderdto.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectmanagerdto.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectmemberdto.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectmemberroledto.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectprioritydto.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectstatusdto.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projecttemplatecategorydto.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projecttemplatedto.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectupdatedto.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/reactgridlayoutdto.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/reactgridlayoutitemdto.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourceapproverdto.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourcecreatedto.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourcedto.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourceskilldto.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourceteamdto.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourceupdatedto.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tagcreatedto.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tagdto.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tagupdatedto.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskassigneedto.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskcreatedto.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskdto.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskfielddto.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskfieldprojectdto.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskfieldvaluedto.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskfieldvaluetaskdto.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskprioritydto.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskprojectdto.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskstatuscreatedto.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskstatusdto.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskstatusupdatedto.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tasktagdto.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tasktododto.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskupdatedto.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetadmintypedto.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetcreaterequestdto.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetdto.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetprojectdto.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetresourcedto.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetresponsedto.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheettaskdto.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetupdaterequestdto.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updateprojectfieldvaluedto.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updaterequestdto.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updateresourceskilldto.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updateresourceteamdto.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updatetaskfieldvaluedto.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/userroledto.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/workspacedto.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/workspacejoindto.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/workspacelinksdto.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/workspaceuserinfodto.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/tests/test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/LICENSE
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/README.md
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/pyproject.toml
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 projectmanagersdk-99.0.2548/PKG-INFO
```

### Comparing `projectmanagersdk-98.0.2363/.github/workflows/publish.yml` & `projectmanagersdk-99.0.2548/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/__init__.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from ProjectManagerSdk.clients.tagclient import TagClient
 from ProjectManagerSdk.clients.taskclient import TaskClient
 from ProjectManagerSdk.clients.taskassigneeclient import TaskAssigneeClient
 from ProjectManagerSdk.clients.taskfieldclient import TaskFieldClient
 from ProjectManagerSdk.clients.taskfileclient import TaskFileClient
 from ProjectManagerSdk.clients.taskstatusclient import TaskStatusClient
 from ProjectManagerSdk.clients.tasktagclient import TaskTagClient
+from ProjectManagerSdk.clients.teamsclient import TeamsClient
 from ProjectManagerSdk.clients.timesheetclient import TimesheetClient
 from ProjectManagerSdk.clients.userroleclient import UserRoleClient
 from ProjectManagerSdk.clients.workspaceclient import WorkSpaceClient
 # Data models
 from ProjectManagerSdk.models.apikeycreatedto import ApiKeyCreateDto
 from ProjectManagerSdk.models.apikeydto import ApiKeyDto
 from ProjectManagerSdk.models.assigneeupsertdto import AssigneeUpsertDto
@@ -46,33 +47,33 @@
 from ProjectManagerSdk.models.changesetgetresponsedto import ChangesetGetResponseDto
 from ProjectManagerSdk.models.changesetstatusdto import ChangeSetStatusDto
 from ProjectManagerSdk.models.connectionschemadto import ConnectionSchemaDto
 from ProjectManagerSdk.models.createprojectfielddto import CreateProjectFieldDto
 from ProjectManagerSdk.models.createprojectfieldresponsedto import CreateProjectFieldResponseDto
 from ProjectManagerSdk.models.createresourceskilldto import CreateResourceSkillDto
 from ProjectManagerSdk.models.createresourceteamdto import CreateResourceTeamDto
-from ProjectManagerSdk.models.createtaskfieldrequestdto import CreateTaskFieldRequestDto
+from ProjectManagerSdk.models.createtaskfielddto import CreateTaskFieldDto
 from ProjectManagerSdk.models.dashboardsettingcreatedto import DashboardSettingCreateDto
 from ProjectManagerSdk.models.dashboardsettingdto import DashboardSettingDto
-from ProjectManagerSdk.models.deleteprojectfielddto import DeleteProjectFieldDto
 from ProjectManagerSdk.models.directlinkdto import DirectLinkDto
 from ProjectManagerSdk.models.discussioncreatedto import DiscussionCreateDto
 from ProjectManagerSdk.models.discussioncreateresponsedto import DiscussionCreateResponseDto
 from ProjectManagerSdk.models.discussiondto import DiscussionDto
 from ProjectManagerSdk.models.discussionemoji import DiscussionEmoji
 from ProjectManagerSdk.models.filedto import FileDto
 from ProjectManagerSdk.models.getprojectfieldsresponsedto import GetProjectFieldsResponseDto
-from ProjectManagerSdk.models.gettaskfieldsresponsedto import GetTaskFieldsResponseDto
 from ProjectManagerSdk.models.iddto import IdDto
 from ProjectManagerSdk.models.integrationauthsetupdto import IntegrationAuthSetupDto
 from ProjectManagerSdk.models.integrationcategorydto import IntegrationCategoryDto
+from ProjectManagerSdk.models.integrationconnectionschemeobjectdto import IntegrationConnectionSchemeObjectDto
 from ProjectManagerSdk.models.integrationdto import IntegrationDto
 from ProjectManagerSdk.models.integrationinstancedto import IntegrationInstanceDto
 from ProjectManagerSdk.models.integrationproviderdto import IntegrationProviderDto
 from ProjectManagerSdk.models.licensedto import LicenseDto
+from ProjectManagerSdk.models.masterconnectionschemedto import MasterConnectionSchemeDto
 from ProjectManagerSdk.models.namedto import NameDto
 from ProjectManagerSdk.models.odataentitysetinfo import ODataEntitySetInfo
 from ProjectManagerSdk.models.odatafunctionimportinfo import ODataFunctionImportInfo
 from ProjectManagerSdk.models.odataservicedocument import ODataServiceDocument
 from ProjectManagerSdk.models.odatasingletoninfo import ODataSingletonInfo
 from ProjectManagerSdk.models.odatatypeannotation import ODataTypeAnnotation
 from ProjectManagerSdk.models.permissionoptionsdto import PermissionOptionsDto
@@ -101,18 +102,19 @@
 from ProjectManagerSdk.models.resourceteamdto import ResourceTeamDto
 from ProjectManagerSdk.models.resourceupdatedto import ResourceUpdateDto
 from ProjectManagerSdk.models.tagcreatedto import TagCreateDto
 from ProjectManagerSdk.models.tagdto import TagDto
 from ProjectManagerSdk.models.tagupdatedto import TagUpdateDto
 from ProjectManagerSdk.models.taskassigneedto import TaskAssigneeDto
 from ProjectManagerSdk.models.taskcreatedto import TaskCreateDto
-from ProjectManagerSdk.models.taskdetailsdto import TaskDetailsDto
 from ProjectManagerSdk.models.taskdto import TaskDto
 from ProjectManagerSdk.models.taskfielddto import TaskFieldDto
-from ProjectManagerSdk.models.taskfieldsvalueresponsedto import TaskFieldsValueResponseDto
+from ProjectManagerSdk.models.taskfieldprojectdto import TaskFieldProjectDto
+from ProjectManagerSdk.models.taskfieldvaluedto import TaskFieldValueDto
+from ProjectManagerSdk.models.taskfieldvaluetaskdto import TaskFieldValueTaskDto
 from ProjectManagerSdk.models.taskprioritydto import TaskPriorityDto
 from ProjectManagerSdk.models.taskprojectdto import TaskProjectDto
 from ProjectManagerSdk.models.taskstatuscreatedto import TaskStatusCreateDto
 from ProjectManagerSdk.models.taskstatusdto import TaskStatusDto
 from ProjectManagerSdk.models.taskstatusupdatedto import TaskStatusUpdateDto
 from ProjectManagerSdk.models.tasktagdto import TaskTagDto
 from ProjectManagerSdk.models.tasktododto import TaskTodoDto
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/projectmanagerclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/projectmanagerclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # For the full copyright and license information, please view the LICENSE
 # file that was distributed with this source code.
 #
 # @author     ProjectManager.com <support@projectmanager.com>
 #             
 # @copyright  2023-2023 ProjectManager.com, Inc.
-# @version    98.0.2363
+# @version    99.0.2548
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 import platform
 import requests
 import typing
 import urllib.parse
@@ -68,14 +68,15 @@
         from ProjectManagerSdk.clients.tagclient import TagClient
         from ProjectManagerSdk.clients.taskclient import TaskClient
         from ProjectManagerSdk.clients.taskassigneeclient import TaskAssigneeClient
         from ProjectManagerSdk.clients.taskfieldclient import TaskFieldClient
         from ProjectManagerSdk.clients.taskfileclient import TaskFileClient
         from ProjectManagerSdk.clients.taskstatusclient import TaskStatusClient
         from ProjectManagerSdk.clients.tasktagclient import TaskTagClient
+        from ProjectManagerSdk.clients.teamsclient import TeamsClient
         from ProjectManagerSdk.clients.timesheetclient import TimesheetClient
         from ProjectManagerSdk.clients.userroleclient import UserRoleClient
         from ProjectManagerSdk.clients.workspaceclient import WorkSpaceClient
         self.apiKey = ApiKeyClient(self)
         self.changeset = ChangesetClient(self)
         self.dashboard = DashboardClient(self)
         self.discussion = DiscussionClient(self)
@@ -102,22 +103,23 @@
         self.tag = TagClient(self)
         self.task = TaskClient(self)
         self.taskAssignee = TaskAssigneeClient(self)
         self.taskField = TaskFieldClient(self)
         self.taskFile = TaskFileClient(self)
         self.taskStatus = TaskStatusClient(self)
         self.taskTag = TaskTagClient(self)
+        self.teams = TeamsClient(self)
         self.timesheet = TimesheetClient(self)
         self.userRole = UserRoleClient(self)
         self.workSpace = WorkSpaceClient(self)
         self.serverUrl = env
         if env == "production":
             self.serverUrl = "https://api.projectmanager.com"
         self.sdkName = "Python"
-        self.sdkVersion = "98.0.2363"
+        self.sdkVersion = "99.0.2548"
         self.machineName = platform.uname().node
         self.applicationName = appname
         self.bearerToken = None
     
     def with_api_key(self, key: str):
         """Configure this API client to use API Key authentication
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/apikeyclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/apikeyclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/changesetclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/changesetclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/dashboardclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/dashboardclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/discussionclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/discussionclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/fileclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/workspaceclient.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,82 +8,74 @@
 #
 # @author     ProjectManager.com <support@projectmanager.com>
 # @copyright  2023-2023 ProjectManager.com, Inc.
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 from ProjectManagerSdk.models.astroresult import AstroResult
-from ProjectManagerSdk.models.updaterequestdto import UpdateRequestDto
+from ProjectManagerSdk.models.workspacedto import WorkSpaceDto
+from ProjectManagerSdk.models.workspacejoindto import WorkSpaceJoinDto
 import json
 
-class FileClient:
+class WorkSpaceClient:
     """
-    API methods related to File
+    API methods related to WorkSpace
     """
     from ProjectManagerSdk.projectmanagerclient import ProjectManagerClient
 
     def __init__(self, client: ProjectManagerClient):
         self.client = client
 
-    def download_file(self, documentId: str, type: str) -> AstroResult[object]:
+    def retrieve_workspaces(self) -> AstroResult[list[WorkSpaceDto]]:
         """
-        Downloads the contents of a file that was previously uploaded to
-        ProjectManager.com.
+        Retrieve the list of Workspaces to which the currently logged on
+        user has access.
 
-        ProjectManager allows you to store Files connected to other
-        elements of your Workspace such as a Project, a Task, or Home.
-        Files are maintained separately based on the location where the
-        file was stored.
-
-        When you upload a File, please allow a few moments for the File
-        to be processed and verified. ProjectManager may reject File
-        uploads that contain problems such as malware. Once a File has
-        completed the upload the process, you may retrieve it using the
-        DownloadFile API.
+        A single User may have access to multiple Workspaces, although
+        they can only be logged on to one Workspace at a time. This API
+        lists all Workspaces to which the currently logged on user is
+        entitled to access. To determine which Workspace a user is
+        currently logged on use the `/api/data/me` endpoint.
 
         Parameters
         ----------
-        documentId : str
-            The unique identifier of the document to download
-        type : str
-            If you specify a type of `html`, processes the file using
-            text encoding, otherwise binary
         """
-        path = f"/api/data/files/{documentId}/download"
+        path = "/api/data/workspaces"
         queryParams = {}
-        if type:
-            queryParams['type'] = type
         result = self.client.send_request("GET", path, None, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
-            return AstroResult[object](None, True, False, result.status_code, object(**json.loads(result.content)['data']))
+            data = []
+            for dict in json.loads(result.content)['data']:
+                data.append(WorkSpaceDto(**dict))
+            return AstroResult[list[WorkSpaceDto]](None, True, False, result.status_code, data)
         else:
-            return AstroResult[object](result.json(), False, True, result.status_code, None)
+            return AstroResult[list[WorkSpaceDto]](result.json(), False, True, result.status_code, None)
 
-    def update_file(self, fileId: str, body: UpdateRequestDto) -> AstroResult[object]:
+    def invite_to_workspace(self, organizationId: str, body: WorkSpaceJoinDto) -> AstroResult[object]:
         """
-        Updates information about a File uploaded to your Workspace.
+        Invite a specific user to join a Workspace to which the current
+        user has administrator rights.
+
+        A single User may have access to multiple Workspaces, although
+        they can only be logged on to one Workspace at a time. This API
+        lists all Workspaces to which the currently logged on user is
+        entitled to access. To determine which Workspace a user is
+        currently logged on use the `/api/data/me` endpoint.
 
-        ProjectManager allows you to store Files connected to other
-        elements of your Workspace such as a Project, a Task, or Home.
-        Files are maintained separately based on the location where the
-        file was stored.
-
-        When you upload a File, please allow a few moments for the File
-        to be processed and verified. ProjectManager may reject File
-        uploads that contain problems such as malware. Once a File has
-        completed the upload the process, you may retrieve it using the
-        DownloadFile API.
+        This API allows you to invite a specific an invitation to join a
+        specific Workspace.
 
         Parameters
         ----------
-        fileId : str
-            The unique identifier of the File to update
-        body : UpdateRequestDto
-            Information to change about the File and its location
+        organizationId : str
+            The unique identifier of the Organization that you are
+            inviting a User to joi
+        body : WorkSpaceJoinDto
+            Information about the user which will receive the invitation
         """
-        path = f"/api/data/files/{fileId}"
+        path = f"/api/data/workspaces/{organizationId}/join"
         queryParams = {}
-        result = self.client.send_request("PUT", path, body, queryParams, None)
+        result = self.client.send_request("POST", path, body, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
             return AstroResult[object](None, True, False, result.status_code, object(**json.loads(result.content)['data']))
         else:
             return AstroResult[object](result.json(), False, True, result.status_code, None)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/homefileclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/homefileclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/integrationcategoryclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/integrationcategoryclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/integrationclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/integrationclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/integrationproviderclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/integrationproviderclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/licenseclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/licenseclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/meclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/meclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectchargecodeclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectchargecodeclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectcustomerclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectcustomerclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,18 @@
     def __init__(self, client: ProjectManagerClient):
         self.client = client
 
     def retrieve_project_customers(self) -> AstroResult[list[ProjectCustomerDto]]:
         """
         Retrieves all ProjectCustomers defined within your Workspace.
 
-        A ProjectCustomer is a code used to identify costs within your
-        Projects. Each ProjectCustomer has a name and a unique
-        identifier. ProjectCustomers are defined per Workspace and are
-        shared among Projects.
+        A ProjectCustomer is a code used to identify customers
+        associated with your Projects. Each ProjectCustomer has a name
+        and a unique identifier. ProjectCustomers are defined per
+        Workspace and are shared among Projects.
 
         Parameters
         ----------
         """
         path = "/api/data/projects/customers"
         queryParams = {}
         result = self.client.send_request("GET", path, None, queryParams, None)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectfieldclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectfieldclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # @copyright  2023-2023 ProjectManager.com, Inc.
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 from ProjectManagerSdk.models.astroresult import AstroResult
 from ProjectManagerSdk.models.createprojectfielddto import CreateProjectFieldDto
 from ProjectManagerSdk.models.createprojectfieldresponsedto import CreateProjectFieldResponseDto
-from ProjectManagerSdk.models.deleteprojectfielddto import DeleteProjectFieldDto
 from ProjectManagerSdk.models.getprojectfieldsresponsedto import GetProjectFieldsResponseDto
 from ProjectManagerSdk.models.projectfieldsvalueresponsedto import ProjectFieldsValueResponseDto
 from ProjectManagerSdk.models.updateprojectfieldvaluedto import UpdateProjectFieldValueDto
 import json
 
 class ProjectFieldClient:
     """
@@ -72,54 +71,55 @@
         queryParams = {}
         result = self.client.send_request("POST", path, body, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
             return AstroResult[CreateProjectFieldResponseDto](None, True, False, result.status_code, CreateProjectFieldResponseDto(**json.loads(result.content)['data']))
         else:
             return AstroResult[CreateProjectFieldResponseDto](result.json(), False, True, result.status_code, None)
 
-    def delete_project_field(self, body: DeleteProjectFieldDto) -> AstroResult[object]:
+    def delete_project_field(self, fieldId: str) -> AstroResult[object]:
         """
         Deletes an existing ProjectField within your Workspace.
 
         A ProjectField is a custom field defined within your Workspace.
         You can define ProjectFields for any integration purpose that is
         important to your business. Each ProjectField has a data type as
         well as options in how it is handled. ProjectFields can be
         edited for each Project within your Workspace.
 
         Parameters
         ----------
-        body : DeleteProjectFieldDto
-            The identity of the ProjectField to delete
+        fieldId : str
+            The unique identifier or short ID of this ProjectField
         """
-        path = "/api/data/projects/fields"
+        path = f"/api/data/projects/fields/{fieldId}"
         queryParams = {}
-        result = self.client.send_request("DELETE", path, body, queryParams, None)
+        result = self.client.send_request("DELETE", path, None, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
             return AstroResult[object](None, True, False, result.status_code, object(**json.loads(result.content)['data']))
         else:
             return AstroResult[object](result.json(), False, True, result.status_code, None)
 
-    def update_project_field(self, projectId: str, fieldId: str, body: UpdateProjectFieldValueDto) -> AstroResult[object]:
+    def update_projectfield_value(self, projectId: str, fieldId: str, body: UpdateProjectFieldValueDto) -> AstroResult[object]:
         """
-        Updates an existing ProjectField with new information.
+        Replaces the current value of a ProjectField for a specific
+        Project within your Workspace.
 
         A ProjectField is a custom field defined within your Workspace.
         You can define ProjectFields for any integration purpose that is
         important to your business. Each ProjectField has a data type as
         well as options in how it is handled. ProjectFields can be
         edited for each Project within your Workspace.
 
         Parameters
         ----------
         projectId : str
             The unique identifier of the Project that contains this
             ProjectField
         fieldId : str
-            The unique identifier of this ProjectField
+            The unique identifier or short ID of this ProjectField
         body : UpdateProjectFieldValueDto
             The new information for this ProjectField
         """
         path = f"/api/data/projects/{projectId}/fields/{fieldId}"
         queryParams = {}
         result = self.client.send_request("PUT", path, body, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
@@ -128,35 +128,47 @@
             return AstroResult[object](result.json(), False, True, result.status_code, None)
 
     def retrieve_projectfield_value(self, projectId: str, fieldId: str) -> AstroResult[ProjectFieldsValueResponseDto]:
         """
         Retrieves the current ProjectField value for a particular
         Project and ProjectField.
 
+        A ProjectField is a custom field defined within your Workspace.
+        You can define ProjectFields for any integration purpose that is
+        important to your business. Each ProjectField has a data type as
+        well as options in how it is handled. ProjectFields can be
+        edited for each Project within your Workspace.
+
         Parameters
         ----------
         projectId : str
             The unique identifier of the Project of the value to
             retrieve
         fieldId : str
-            The unique identifier of the ProjectField of the value to
-            retrieve
+            The unique identifier or short ID of the ProjectField of the
+            value to retrieve
         """
         path = f"/api/data/projects/{projectId}/fields/{fieldId}"
         queryParams = {}
         result = self.client.send_request("GET", path, None, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
             return AstroResult[ProjectFieldsValueResponseDto](None, True, False, result.status_code, ProjectFieldsValueResponseDto(**json.loads(result.content)['data']))
         else:
             return AstroResult[ProjectFieldsValueResponseDto](result.json(), False, True, result.status_code, None)
 
     def retrieve_all_projectfield_values(self, projectId: str) -> AstroResult[list[ProjectFieldsValueResponseDto]]:
         """
         Retrieves all ProjectField values for a particular Project.
 
+        A ProjectField is a custom field defined within your Workspace.
+        You can define ProjectFields for any integration purpose that is
+        important to your business. Each ProjectField has a data type as
+        well as options in how it is handled. ProjectFields can be
+        edited for each Project within your Workspace.
+
         Parameters
         ----------
         projectId : str
             The unique identifier of the Project for which we want
             ProjectField values
         """
         path = f"/api/data/projects/{projectId}/fields"
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectfileclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectfileclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectfolderclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectfolderclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectpriorityclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectpriorityclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projectstatusclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projectstatusclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/projecttemplateclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/projecttemplateclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/resourceclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/resourceclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/resourceskillclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/resourceskillclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/resourceteamclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/resourceteamclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/tagclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/tagclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskassigneeclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskassigneeclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # @copyright  2023-2023 ProjectManager.com, Inc.
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 from ProjectManagerSdk.models.astroresult import AstroResult
 from ProjectManagerSdk.models.changesetstatusdto import ChangeSetStatusDto
 from ProjectManagerSdk.models.taskcreatedto import TaskCreateDto
-from ProjectManagerSdk.models.taskdetailsdto import TaskDetailsDto
 from ProjectManagerSdk.models.taskdto import TaskDto
 from ProjectManagerSdk.models.taskprioritydto import TaskPriorityDto
 from ProjectManagerSdk.models.taskupdatedto import TaskUpdateDto
 import json
 
 class TaskClient:
     """
@@ -74,15 +73,15 @@
             data = []
             for dict in json.loads(result.content)['data']:
                 data.append(TaskDto(**dict))
             return AstroResult[list[TaskDto]](None, True, False, result.status_code, data)
         else:
             return AstroResult[list[TaskDto]](result.json(), False, True, result.status_code, None)
 
-    def retrieve_task(self, taskId: str) -> AstroResult[TaskDetailsDto]:
+    def retrieve_task(self, taskId: str) -> AstroResult[TaskDto]:
         """
         Retrieve a Task by its unique identifier or by its short ID. A
         Task has both a unique identifier, which is a GUID, and a short
         ID, which is a small text label that is unique only within your
         Workspace.
 
         A Task is an individual element of work that must be performed
@@ -95,17 +94,17 @@
         taskId : str
             The unique identifier or short ID of the Task to retrieve
         """
         path = f"/api/data/tasks/{taskId}"
         queryParams = {}
         result = self.client.send_request("GET", path, None, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
-            return AstroResult[TaskDetailsDto](None, True, False, result.status_code, TaskDetailsDto(**json.loads(result.content)['data']))
+            return AstroResult[TaskDto](None, True, False, result.status_code, TaskDto(**json.loads(result.content)['data']))
         else:
-            return AstroResult[TaskDetailsDto](result.json(), False, True, result.status_code, None)
+            return AstroResult[TaskDto](result.json(), False, True, result.status_code, None)
 
     def update_task(self, taskId: str, body: TaskUpdateDto) -> AstroResult[ChangeSetStatusDto]:
         """
         Update an existing Task and replace the values of fields
         specified.
 
         A Task is an individual element of work that must be performed
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskfieldclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskfieldclient.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 # @author     ProjectManager.com <support@projectmanager.com>
 # @copyright  2023-2023 ProjectManager.com, Inc.
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 from ProjectManagerSdk.models.astroresult import AstroResult
 from ProjectManagerSdk.models.changesetstatusdto import ChangeSetStatusDto
-from ProjectManagerSdk.models.createtaskfieldrequestdto import CreateTaskFieldRequestDto
-from ProjectManagerSdk.models.gettaskfieldsresponsedto import GetTaskFieldsResponseDto
-from ProjectManagerSdk.models.taskfieldsvalueresponsedto import TaskFieldsValueResponseDto
+from ProjectManagerSdk.models.createtaskfielddto import CreateTaskFieldDto
+from ProjectManagerSdk.models.taskfielddto import TaskFieldDto
+from ProjectManagerSdk.models.taskfieldvaluedto import TaskFieldValueDto
 from ProjectManagerSdk.models.updatetaskfieldvaluedto import UpdateTaskFieldValueDto
 import json
 
 class TaskFieldClient:
     """
     API methods related to TaskField
     """
     from ProjectManagerSdk.projectmanagerclient import ProjectManagerClient
 
     def __init__(self, client: ProjectManagerClient):
         self.client = client
 
-    def retrieve_task_fields(self, projectId: str) -> AstroResult[list[GetTaskFieldsResponseDto]]:
+    def retrieve_task_fields(self, projectId: str) -> AstroResult[list[TaskFieldDto]]:
         """
         Retrieves all TaskFields defined for a specific Project within
         your Workspace.
 
         A TaskField is a custom field defined within your Workspace for
         a specific Project. You can define TaskFields for any
         integration purpose that is important to your business. Each
@@ -47,47 +47,98 @@
         """
         path = f"/api/data/projects/{projectId}/tasks/fields"
         queryParams = {}
         result = self.client.send_request("GET", path, None, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
             data = []
             for dict in json.loads(result.content)['data']:
-                data.append(GetTaskFieldsResponseDto(**dict))
-            return AstroResult[list[GetTaskFieldsResponseDto]](None, True, False, result.status_code, data)
+                data.append(TaskFieldDto(**dict))
+            return AstroResult[list[TaskFieldDto]](None, True, False, result.status_code, data)
         else:
-            return AstroResult[list[GetTaskFieldsResponseDto]](result.json(), False, True, result.status_code, None)
+            return AstroResult[list[TaskFieldDto]](result.json(), False, True, result.status_code, None)
 
-    def create_task_field(self, projectId: str, body: CreateTaskFieldRequestDto) -> AstroResult[ChangeSetStatusDto]:
+    def create_task_field(self, projectId: str, body: CreateTaskFieldDto) -> AstroResult[ChangeSetStatusDto]:
         """
-        Creates a new TaskFields for a specific Project within your
+        Creates a new TaskField for a specific Project within your
         Workspace.
 
         A TaskField is a custom field defined within your Workspace for
         a specific Project. You can define TaskFields for any
         integration purpose that is important to your business. Each
         TaskField has a data type as well as options in how it is
         handled. TaskFields can be edited for each Task inside this
         Project.
 
         Parameters
         ----------
         projectId : str
             The unique identifier of the Project within which to create
             this TaskField
-        body : CreateTaskFieldRequestDto
+        body : CreateTaskFieldDto
             Information about the TaskField to create
         """
         path = f"/api/data/projects/{projectId}/tasks/fields"
         queryParams = {}
         result = self.client.send_request("POST", path, body, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
             return AstroResult[ChangeSetStatusDto](None, True, False, result.status_code, ChangeSetStatusDto(**json.loads(result.content)['data']))
         else:
             return AstroResult[ChangeSetStatusDto](result.json(), False, True, result.status_code, None)
 
+    def query_task_fields(self, top: int, skip: int, filter: str, select: str, orderby: str, expand: str) -> AstroResult[list[TaskFieldDto]]:
+        """
+        Retrieve a list of TaskFields that match an [OData formatted
+        query](https://www.odata.org/).
+
+        A TaskField is a custom field defined within your Workspace for
+        a specific Project. You can define TaskFields for any
+        integration purpose that is important to your business. Each
+        TaskField has a data type as well as options in how it is
+        handled. TaskFields can be edited for each Task inside a
+        Project.
+
+        Parameters
+        ----------
+        $top : int
+            The number of records to return
+        $skip : int
+            Skips the given number of records and then returns $top
+            records
+        $filter : str
+            Filter the expression according to oData queries
+        $select : str
+            Specify which properties should be returned
+        $orderby : str
+            Order collection by this field.
+        $expand : str
+            Include related data in the response
+        """
+        path = "/api/data/projects/tasks/fields"
+        queryParams = {}
+        if top:
+            queryParams['$top'] = top
+        if skip:
+            queryParams['$skip'] = skip
+        if filter:
+            queryParams['$filter'] = filter
+        if select:
+            queryParams['$select'] = select
+        if orderby:
+            queryParams['$orderby'] = orderby
+        if expand:
+            queryParams['$expand'] = expand
+        result = self.client.send_request("GET", path, None, queryParams, None)
+        if result.status_code >= 200 and result.status_code < 300:
+            data = []
+            for dict in json.loads(result.content)['data']:
+                data.append(TaskFieldDto(**dict))
+            return AstroResult[list[TaskFieldDto]](None, True, False, result.status_code, data)
+        else:
+            return AstroResult[list[TaskFieldDto]](result.json(), False, True, result.status_code, None)
+
     def delete_task_field(self, projectId: str, fieldId: str) -> AstroResult[object]:
         """
         Deletes a TaskField for a specific Project within your
         Workspace.
 
         A TaskField is a custom field defined within your Workspace for
         a specific Project. You can define TaskFields for any
@@ -108,93 +159,144 @@
         queryParams = {}
         result = self.client.send_request("DELETE", path, None, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
             return AstroResult[object](None, True, False, result.status_code, object(**json.loads(result.content)['data']))
         else:
             return AstroResult[object](result.json(), False, True, result.status_code, None)
 
-    def retrieve_taskfield_value(self, taskId: str, fieldId: str) -> AstroResult[TaskFieldsValueResponseDto]:
+    def retrieve_all_taskfield_values(self, taskId: str) -> AstroResult[list[TaskFieldValueDto]]:
         """
-        Retrieves the current TaskField value for a particular Task and
-        TaskField.
+        Retrieves all TaskField values for a particular Task.
 
         A TaskField is a custom field defined within your Workspace for
         a specific Project. You can define TaskFields for any
         integration purpose that is important to your business. Each
         TaskField has a data type as well as options in how it is
         handled. TaskFields can be edited for each Task inside this
         Project.
 
         Parameters
         ----------
         taskId : str
-            The unique identifier of the Task of the value to retrieve
-        fieldId : str
-            The unique identifier of the TaskField of the value to
-            retrieve
+            The unique identifier of the Task for which we want
+            TaskField values
         """
-        path = f"/api/data/tasks/{taskId}/fields/{fieldId}"
+        path = f"/api/data/tasks/{taskId}/fields/values"
         queryParams = {}
         result = self.client.send_request("GET", path, None, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
-            return AstroResult[TaskFieldsValueResponseDto](None, True, False, result.status_code, TaskFieldsValueResponseDto(**json.loads(result.content)['data']))
+            data = []
+            for dict in json.loads(result.content)['data']:
+                data.append(TaskFieldValueDto(**dict))
+            return AstroResult[list[TaskFieldValueDto]](None, True, False, result.status_code, data)
         else:
-            return AstroResult[TaskFieldsValueResponseDto](result.json(), False, True, result.status_code, None)
+            return AstroResult[list[TaskFieldValueDto]](result.json(), False, True, result.status_code, None)
 
-    def update_taskfield_value(self, taskId: str, fieldId: str, body: UpdateTaskFieldValueDto) -> AstroResult[ChangeSetStatusDto]:
+    def query_task_field_values(self, top: int, skip: int, filter: str, select: str, orderby: str, expand: str) -> AstroResult[list[TaskFieldValueDto]]:
         """
-        Replaces the current value of a TaskFields for a specific Task
-        within your Workspace.
+        Retrieve a list of TaskFieldValues that match an [OData
+        formatted query](https://www.odata.org/).
+
+        A TaskField is a custom field defined within your Workspace for
+        a specific Project. You can define TaskFields for any
+        integration purpose that is important to your business. Each
+        TaskField has a data type as well as options in how it is
+        handled. TaskFields can be edited for each Task inside this
+        Project.
+
+        Parameters
+        ----------
+        $top : int
+            The number of records to return
+        $skip : int
+            Skips the given number of records and then returns $top
+            records
+        $filter : str
+            Filter the expression according to oData queries
+        $select : str
+            Specify which properties should be returned
+        $orderby : str
+            Order collection by this field.
+        $expand : str
+            Include related data in the response
+        """
+        path = "/api/data/tasks/fields/values"
+        queryParams = {}
+        if top:
+            queryParams['$top'] = top
+        if skip:
+            queryParams['$skip'] = skip
+        if filter:
+            queryParams['$filter'] = filter
+        if select:
+            queryParams['$select'] = select
+        if orderby:
+            queryParams['$orderby'] = orderby
+        if expand:
+            queryParams['$expand'] = expand
+        result = self.client.send_request("GET", path, None, queryParams, None)
+        if result.status_code >= 200 and result.status_code < 300:
+            data = []
+            for dict in json.loads(result.content)['data']:
+                data.append(TaskFieldValueDto(**dict))
+            return AstroResult[list[TaskFieldValueDto]](None, True, False, result.status_code, data)
+        else:
+            return AstroResult[list[TaskFieldValueDto]](result.json(), False, True, result.status_code, None)
+
+    def retrieve_task_field_value(self, taskId: str, fieldId: str) -> AstroResult[TaskFieldValueDto]:
+        """
+        Retrieves the current TaskField value for a particular Task and
+        TaskField.
 
         A TaskField is a custom field defined within your Workspace for
         a specific Project. You can define TaskFields for any
         integration purpose that is important to your business. Each
         TaskField has a data type as well as options in how it is
         handled. TaskFields can be edited for each Task inside this
         Project.
 
         Parameters
         ----------
         taskId : str
-            The unique identifier of the Task whose value you wish to
-            update
+            The unique identifier of the Task of the value to retrieve
         fieldId : str
-            The unique identifier of the TaskField whose value you wish
-            to update
-        body : UpdateTaskFieldValueDto
-            The new value for this TaskField for this Task
+            The unique identifier of the TaskField of the value to
+            retrieve
         """
-        path = f"/api/data/tasks/{taskId}/fields/{fieldId}"
+        path = f"/api/data/tasks/{taskId}/fields/{fieldId}/values"
         queryParams = {}
-        result = self.client.send_request("PUT", path, body, queryParams, None)
+        result = self.client.send_request("GET", path, None, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
-            return AstroResult[ChangeSetStatusDto](None, True, False, result.status_code, ChangeSetStatusDto(**json.loads(result.content)['data']))
+            return AstroResult[TaskFieldValueDto](None, True, False, result.status_code, TaskFieldValueDto(**json.loads(result.content)['data']))
         else:
-            return AstroResult[ChangeSetStatusDto](result.json(), False, True, result.status_code, None)
+            return AstroResult[TaskFieldValueDto](result.json(), False, True, result.status_code, None)
 
-    def retrieve_all_taskfield_values(self, taskId: str) -> AstroResult[list[TaskFieldsValueResponseDto]]:
+    def update_task_field_value(self, taskId: str, fieldId: str, body: UpdateTaskFieldValueDto) -> AstroResult[ChangeSetStatusDto]:
         """
-        Retrieves all TaskField values for a particular Task.
+        Replaces the current value of a TaskField for a specific Task
+        within your Workspace.
 
         A TaskField is a custom field defined within your Workspace for
         a specific Project. You can define TaskFields for any
         integration purpose that is important to your business. Each
         TaskField has a data type as well as options in how it is
         handled. TaskFields can be edited for each Task inside this
         Project.
 
         Parameters
         ----------
         taskId : str
-            The unique identifier of the Task for which we want
-            TaskField values
+            The unique identifier of the Task whose value you wish to
+            update
+        fieldId : str
+            The unique identifier of the TaskField whose value you wish
+            to update
+        body : UpdateTaskFieldValueDto
+            The new value for this TaskField for this Task
         """
-        path = f"/api/data/tasks/{taskId}/fields"
+        path = f"/api/data/tasks/{taskId}/fields/{fieldId}/values"
         queryParams = {}
-        result = self.client.send_request("GET", path, None, queryParams, None)
+        result = self.client.send_request("PUT", path, body, queryParams, None)
         if result.status_code >= 200 and result.status_code < 300:
-            data = []
-            for dict in json.loads(result.content)['data']:
-                data.append(TaskFieldsValueResponseDto(**dict))
-            return AstroResult[list[TaskFieldsValueResponseDto]](None, True, False, result.status_code, data)
+            return AstroResult[ChangeSetStatusDto](None, True, False, result.status_code, ChangeSetStatusDto(**json.loads(result.content)['data']))
         else:
-            return AstroResult[list[TaskFieldsValueResponseDto]](result.json(), False, True, result.status_code, None)
+            return AstroResult[ChangeSetStatusDto](result.json(), False, True, result.status_code, None)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskfileclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskfileclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/taskstatusclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/taskstatusclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/tasktagclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/tasktagclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/timesheetclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/timesheetclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/clients/userroleclient.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/clients/userroleclient.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/apikeycreatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/apikeycreatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/apikeydto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/apikeydto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/assigneeupsertdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/assigneeupsertdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/astroerror.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/astroerror.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/astroresult.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/astroresult.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/authenticationdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/authenticationdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/authenticationstatusdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/authenticationstatusdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/changesetgetresponsedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/changesetgetresponsedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/changesetstatusdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/changesetstatusdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/connectionschemadto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/connectionschemadto.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 @dataclass
 class ConnectionSchemaDto:
     """
     This class contains the URL or AuthScheme to use to authenticate
     with the Integration Provider.
     """
 
+    connected: bool | None = None
+    """
+    Whether or not the Integration Provider is connected.
+    """
+
     url: str | None = None
     """
     The URL to use to authenticate with the Integration Provider.
     """
 
     authScheme: object | None = None
     """
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createprojectfielddto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createprojectfielddto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createprojectfieldresponsedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createprojectfieldresponsedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createresourceskilldto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createresourceskilldto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createresourceteamdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createresourceteamdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/createtaskfieldrequestdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectfieldsvalueresponsedto.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,35 +11,53 @@
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from dataclasses import dataclass
 
 @dataclass
-class CreateTaskFieldRequestDto:
+class ProjectFieldsValueResponseDto:
     """
-    A TaskField is a custom field defined within your Workspace for a
-    specific Project. You can define TaskFields for any integration
-    purpose that is important to your business. Each TaskField has a
-    data type as well as options in how it is handled. TaskFields can be
-    edited for each Task inside this Project.
+    A ProjectField is a custom field defined within your Workspace for
+    each Project. Each ProjectField has a data type as well as options
+    in how it is handled.
+    """
+
+    id: str | None = None
+    """
+    The unique identifier of this Project Field.
+    """
+
+    value: str | None = None
+    """
+    The value currently set for this Project Field.
     """
 
     name: str | None = None
     """
-    The name of the TaskField
+    The name of this Project Field.
     """
 
     type: str | None = None
     """
-    The type of this TaskField. Valid types are the following: * Text *
-    Number * Date * Checkbox * Currency * Dropdown
+    The type of this Project Field. Valid types are the following: *
+    Text * Number * Date * Checkbox * Currency * Dropdown
     """
 
     shortId: str | None = None
     """
     The short Id of this field - human readable identity
     """
 
+    createdDate: str | None = None
+    """
+    Date and time (in UTC) that this TaskField was created.
+    """
+
+    modifiedDate: str | None = None
+    """
+    Date and time (in UTC) that this TaskField was last modified.
+    """
+
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/dashboardsettingcreatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/dashboardsettingcreatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/dashboardsettingdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/dashboardsettingdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/deleteprojectfielddto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/workspacejoindto.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,29 +11,25 @@
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from dataclasses import dataclass
 
 @dataclass
-class DeleteProjectFieldDto:
+class WorkSpaceJoinDto:
     """
-    A ProjectField is a custom field defined within your Workspace. You
-    can define ProjectFields for any integration purpose that is
-    important to your business. Each ProjectField has a data type as
-    well as options in how it is handled. ProjectFields can be edited
-    for each Project within your Workspace.
+    A Workspace represents a single business subscription to the
+    ProjectManager.com service. You can be a member of multiple
+    Workspaces. Each Workspace is completely separate from all other
+    Workspaces and a user cannot log in to multiple Workspaces at the
+    same time.
     """
 
-    id: str | None = None
+    businessUserId: str | None = None
     """
-    The unique identifier of the ProjectField being deleted
-    """
-
-    name: str | None = None
-    """
-    The name of the ProjectField being deleted
+    The unique identifier of the BusinessUser to invite to this
+    Workspace.
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/directlinkdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/directlinkdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/discussioncreatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/discussioncreatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/discussioncreateresponsedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/discussioncreateresponsedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/discussiondto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/discussiondto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/discussionemoji.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/discussionemoji.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/filedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/filedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/getprojectfieldsresponsedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/getprojectfieldsresponsedto.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,10 +57,15 @@
     """
     A list of options for use of this Field. This is only valid if the
     `Type` value is set to `Dropdown`. When a custom Field of type
     `DropDown` is shown to a user in the application, they will be able
     to choose one of the `Options` in this list.
     """
 
+    shortId: str | None = None
+    """
+    The short Id of this field - human readable identity
+    """
+
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/gettaskfieldsresponsedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskfielddto.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 #
 # @author     ProjectManager.com <support@projectmanager.com>
 # @copyright  2023-2023 ProjectManager.com, Inc.
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
+from ProjectManagerSdk.models.taskfieldprojectdto import TaskFieldProjectDto
 from dataclasses import dataclass
 
 @dataclass
-class GetTaskFieldsResponseDto:
+class TaskFieldDto:
     """
     A TaskField is a custom field defined within your Workspace for a
     specific Project. You can define TaskFields for any integration
     purpose that is important to your business. Each TaskField has a
     data type as well as options in how it is handled. TaskFields can be
     edited for each Task inside this Project.
     """
@@ -47,10 +48,30 @@
     """
     A list of options for use of this TaskField. This is only valid if
     the `Type` value is set to `Dropdown`. When a custom TaskField of
     type `DropDown` is shown to a user in the application, they will be
     able to choose one of the `Options` in this list.
     """
 
+    shortId: str | None = None
+    """
+    The short Id of this TaskField - human readable identity
+    """
+
+    project: TaskFieldProjectDto | None = None
+    """
+    The Project to which this TaskField belongs.
+    """
+
+    createdDate: str | None = None
+    """
+    Date and time (in UTC) that this TaskField was created.
+    """
+
+    modifiedDate: str | None = None
+    """
+    Date and time (in UTC) that this TaskField was last modified.
+    """
+
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/iddto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/iddto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationauthsetupdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationauthsetupdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationcategorydto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationcategorydto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationdto.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,10 +72,15 @@
     """
 
     authenticated: bool | None = None
     """
     True if the user has authenticated
     """
 
+    autoEnabled: bool | None = None
+    """
+    True if the integration is auto-enabled
+    """
+
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationinstancedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationinstancedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/integrationproviderdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/integrationproviderdto.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,10 +75,15 @@
     """
 
     authSetup: IntegrationAuthSetupDto | None = None
     """
     The list of available AuthSetup for this Provider.
     """
 
+    createInWorkato: bool | None = None
+    """
+    Flag whether user/workspace needs to be setup in Workato
+    """
+
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/licensedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/licensedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/namedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/namedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odataentitysetinfo.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odataentitysetinfo.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odatafunctionimportinfo.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odatafunctionimportinfo.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odataservicedocument.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odataservicedocument.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odatasingletoninfo.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odatasingletoninfo.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/odatatypeannotation.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/odatatypeannotation.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/permissionoptionsdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/permissionoptionsdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectchargecodedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectchargecodedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectcreateaccessdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectcreateaccessdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectcreateaccessmemberdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectcreateaccessmemberdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectcreatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectcreatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectcustomerdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectcustomerdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectfieldsvalueresponsedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectstatusdto.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,38 +11,34 @@
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from dataclasses import dataclass
 
 @dataclass
-class ProjectFieldsValueResponseDto:
+class ProjectStatusDto:
     """
-    A Project Field is a custom field defined within your Workspace for
-    each Project. Each Project Field has a data type as well as options
-    in how it is handled.
+    A ProjectStatus is a named condition used by your business to
+    categorize the completion level of Tasks and Projects within your
+    Workspace. You can name your ProjectStatus levels anything you like
+    and you can reorganize the order of the ProjectPriority levels at
+    any time.
     """
 
     id: str | None = None
     """
-    The unique identifier of this Project Field.
-    """
-
-    value: str | None = None
-    """
-    The value currently set for this Project Field.
+    The unique identifier of this ProjectStatus.
     """
 
     name: str | None = None
     """
-    The name of this Project Field.
+    The name of this ProjectStatus.
     """
 
-    type: str | None = None
+    isDeleted: bool | None = None
     """
-    The type of this Project Field. Valid types are the following: *
-    Text * Number * Date * Checkbox * Currency * Dropdown
+    Is this a deleted status
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectfolderdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectfolderdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectmanagerdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectmanagerdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectmemberdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectmemberdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectmemberroledto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectmemberroledto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectprioritydto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectprioritydto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectstatusdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tagdto.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,34 +11,36 @@
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from dataclasses import dataclass
 
 @dataclass
-class ProjectStatusDto:
+class TagDto:
     """
-    A ProjectStatus is a named condition used by your business to
-    categorize the completion level of Tasks and Projects within your
-    Workspace. You can name your ProjectStatus levels anything you like
-    and you can reorganize the order of the ProjectPriority levels at
-    any time.
+    A Tag is a named categorization you can use to distinguish objects
+    from each other. Tags each have a unique identifier, a name, and a
+    color.
     """
 
     id: str | None = None
     """
-    The unique identifier of this ProjectStatus.
+    The unique identifier of this Tag.
     """
 
     name: str | None = None
     """
-    The name of this ProjectStatus.
+    The name of this Tag.
     """
 
-    isDeleted: bool | None = None
+    color: str | None = None
     """
-    Is this a deleted status
+    The color that will be used to represent this Tag visually. This
+    color is automatically chosen by the application when a user creates
+    a Tag. You can choose specify any color that can be represented
+    using HTML RGB syntax such as `#0088FF`, in the format `RRGGBB`. You
+    may not use names for colors.
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projecttemplatecategorydto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projecttemplatecategorydto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projecttemplatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projecttemplatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/projectupdatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/projectupdatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/reactgridlayoutdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/reactgridlayoutdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/reactgridlayoutitemdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/reactgridlayoutitemdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourceapproverdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourceapproverdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourcecreatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourcecreatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourcedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourcedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourceskilldto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourceskilldto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourceteamdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourceteamdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/resourceupdatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/resourceupdatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tagcreatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tagcreatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tagdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tagupdatedto.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,31 +11,21 @@
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from dataclasses import dataclass
 
 @dataclass
-class TagDto:
+class TagUpdateDto:
     """
     A Tag is a named categorization you can use to distinguish objects
     from each other. Tags each have a unique identifier, a name, and a
     color.
     """
 
-    id: str | None = None
-    """
-    The unique identifier of this Tag.
-    """
-
-    name: str | None = None
-    """
-    The name of this Tag.
-    """
-
     color: str | None = None
     """
     The color that will be used to represent this Tag visually. This
     color is automatically chosen by the application when a user creates
     a Tag. You can choose specify any color that can be represented
     using HTML RGB syntax such as `#0088FF`, in the format `RRGGBB`. You
     may not use names for colors.
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tagupdatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskfieldprojectdto.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,26 +11,31 @@
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from dataclasses import dataclass
 
 @dataclass
-class TagUpdateDto:
+class TaskFieldProjectDto:
     """
-    A Tag is a named categorization you can use to distinguish objects
-    from each other. Tags each have a unique identifier, a name, and a
-    color.
+    The TaskFieldProject is a summary of the Project that this TaskField
+    relates to.
     """
 
-    color: str | None = None
+    id: str | None = None
     """
-    The color that will be used to represent this Tag visually. This
-    color is automatically chosen by the application when a user creates
-    a Tag. You can choose specify any color that can be represented
-    using HTML RGB syntax such as `#0088FF`, in the format `RRGGBB`. You
-    may not use names for colors.
+    The unique identifier of this Project.
+    """
+
+    shortId: str | None = None
+    """
+    The ShortId of this Project.
+    """
+
+    name: str | None = None
+    """
+    The common name of this Project.
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskassigneedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskassigneedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskcreatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskcreatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskdetailsdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskupdatedto.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,153 +8,116 @@
 #
 # @author     ProjectManager.com <support@projectmanager.com>
 # @copyright  2023-2023 ProjectManager.com, Inc.
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
-from ProjectManagerSdk.models.taskassigneedto import TaskAssigneeDto
-from ProjectManagerSdk.models.taskprojectdto import TaskProjectDto
-from ProjectManagerSdk.models.taskstatusdto import TaskStatusDto
-from ProjectManagerSdk.models.tasktagdto import TaskTagDto
-from ProjectManagerSdk.models.tasktododto import TaskTodoDto
 from dataclasses import dataclass
 
 @dataclass
-class TaskDetailsDto:
+class TaskUpdateDto:
     """
     A Task is an individual element of work that must be performed to
     complete a Project. A Task can have one or more Resources assigned
     to it. Tasks can be linked to other Tasks to indicate whether they
     have a dependency or a connection.
     """
 
-    id: str | None = None
-    """
-    The unique identifier of this Task.
-    """
-
-    project: TaskProjectDto | None = None
-    """
-    The Project to which this Task belongs.
-    """
-
-    tags: list[TaskTagDto] | None = None
-    """
-    The TaskTags that apply to this Task.
-    """
-
-    assignees: list[TaskAssigneeDto] | None = None
-    """
-    The list of assignees who are to work on this Task, if any.
-    """
-
-    todos: list[TaskTodoDto] | None = None
-    """
-    A list of TaskTodo items, which are sub-tasks within this Task.
-    """
-
-    shortId: str | None = None
-    """
-    A short ID that can be used to refer to this Task. This short ID is
-    guaranteed to be unique within your Workspace.
-    """
-
     name: str | None = None
     """
     The common name of this Task.
     """
 
     description: str | None = None
     """
     A description of the work to be performed in this Task.
     """
 
-    status: TaskStatusDto | None = None
+    percentComplete: int | None = None
+    """
+    The numerical percentage, from 0-100, representing the percentage
+    completion for this Task. Any numbers below zero or above 100 will
+    be clamped to the minimum or maximum value. This value can be edited
+    manually in the Gantt chart view of the application, or can be
+    selected on the Task Detail page within the Kanban board.
+    """
+
+    statusId: str | None = None
     """
     The TaskStatus assigned to this Task.
     """
 
     priorityId: int | None = None
     """
     The unique identifier of the TaskPriority
     """
 
     plannedStartDate: str | None = None
     """
-    The date when work on this Task is planned to begin.
+    The date when work on this Task is planned to begin. This value
+    contains only the date in year-month-day format. For display, this
+    date will always be shown as this same year-month-day regardless of
+    time zone. For reporting purposes, this date is calculated against
+    the official time zone of the Workspace. For example: A Task has a
+    planned completion date of July 5, 2023 in a Workspace that has a
+    time zone of US Pacific Time (GMT-7 or GMT-8, depending on daylight
+    savings time). This project is considered overdue on 12:01 AM July
+    6th 2023 in US Pacific time.
     """
 
     plannedFinishDate: str | None = None
     """
-    The date when work on this Task is expected to complete.
-    """
-
-    actualStartDate: str | None = None
-    """
-    If set, this is the actual date when work began on the Task.
-    """
-
-    actualFinishDate: str | None = None
-    """
-    If set, this is the actual date when work was completed on this
-    Task.
+    The date when work on this Task is expected to complete. This value
+    contains only the date in year-month-day format. For display, this
+    date will always be shown as this same year-month-day regardless of
+    time zone. For reporting purposes, this date is calculated against
+    the official time zone of the Workspace. For example: A Task has a
+    planned completion date of July 5, 2023 in a Workspace that has a
+    time zone of US Pacific Time (GMT-7 or GMT-8, depending on daylight
+    savings time). This project is considered overdue on 12:01 AM July
+    6th 2023 in US Pacific time.
     """
 
-    modifyDate: str | None = None
+    plannedDuration: int | None = None
     """
-    The timestamp in UTC when this Task was most recently modified.
+    The planned duration (in minutes) for this Task. Cannot be negative.
     """
 
-    createDate: str | None = None
+    plannedEffort: int | None = None
     """
-    The timestamp in UTC when this Task was created.
+    The planned effort (in minutes) for this Task. Cannot be negative.
     """
 
-    percentComplete: int | None = None
+    plannedCost: float | None = None
     """
-    The numerical percentage, from 0-100, representing the percentage
-    completion for this Task. Any numbers below zero or above 100 will
-    be clamped to the minimum or maximum value. This value can be edited
-    manually in the Gantt chart view of the application, or can be
-    selected on the Task Detail page within the Kanban board.
+    The planned cost for this Task. Cannot be negative.
     """
 
-    isSummary: bool | None = None
+    actualStartDate: str | None = None
     """
-    True if this Task is the parent of multiple Tasks underneath it. A
-    parent Task is a "rolled-up" view of multiple children that allows
-    you to view a section of work at a glance. You can create a summary
-    Task in the Gantt chart view of the application by adding child
-    tasks underneath a parent Task.
-    """
-
-    wbs: str | None = None
-    """
-    The WBS (Work Breakdown Structure) number for this task within the
-    Gantt chart hierarchy. See [What Is a Work Breakdown Structure
-    (WBS)?](https://www.projectmanager.com/guides/work-breakdown-structure)
-    on Project Manager for more information. The WBS number is an
-    outline number in the form `#.#.#.#` which indicates how tasks are
-    organized and sorted. The WBS value is only available to users at
-    certain edition levels. This value can only be changed if you are a
-    Project Editor.
+    If set, this is the actual date when work began on the Task. This
+    value contains only the date in year-month-day format. For display,
+    this date will always be shown as this same year-month-day
+    regardless of time zone. For reporting purposes, this date is
+    calculated against the official time zone of the Workspace. For
+    example: A Task has a planned completion date of July 5, 2023 in a
+    Workspace that has a time zone of US Pacific Time (GMT-7 or GMT-8,
+    depending on daylight savings time). This project is considered
+    overdue on 12:01 AM July 6th 2023 in US Pacific time.
     """
 
     actualCost: float | None = None
     """
-    The actual cost of this Task to date, if known.
-    """
-
-    plannedCost: float | None = None
-    """
-    The planned cost for this Task. Cannot be negative.
+    If set, this represents the actual tracked cost for this Task.
     """
 
-    fields: object | None = None
+    theme: str | None = None
     """
-    Task fields array with values
+    Color theme definition for this task. eg. Blue, Brown, DarkBlue,
+    DarkGrey, Gold, Green, Grey, LightBrown, LightGreen, LightGrey,
+    LightPurple, LightYellow, Magenta, Mauve, Navy, Orange, Purple, Red.
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskdto.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @author     ProjectManager.com <support@projectmanager.com>
 # @copyright  2023-2023 ProjectManager.com, Inc.
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from ProjectManagerSdk.models.taskassigneedto import TaskAssigneeDto
-from ProjectManagerSdk.models.taskfielddto import TaskFieldDto
+from ProjectManagerSdk.models.taskfieldvaluedto import TaskFieldValueDto
 from ProjectManagerSdk.models.taskprojectdto import TaskProjectDto
 from ProjectManagerSdk.models.taskstatusdto import TaskStatusDto
 from ProjectManagerSdk.models.tasktagdto import TaskTagDto
 from ProjectManagerSdk.models.tasktododto import TaskTodoDto
 from dataclasses import dataclass
 
 @dataclass
@@ -198,15 +198,15 @@
     """
 
     plannedEffort: int | None = None
     """
     The planned effort (in minutes) for this Task.
     """
 
-    fields: list[TaskFieldDto] | None = None
+    fields: list[TaskFieldValueDto] | None = None
     """
     Task fields array with values
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskfielddto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/masterconnectionschemedto.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from dataclasses import dataclass
 
 @dataclass
-class TaskFieldDto:
+class MasterConnectionSchemeDto:
     """
-    A model that contains the value for a TaskField.
+    Master Connection Scheme for Providers
     """
 
-    shortId: str | None = None
+    value: str | None = None
     """
-    The unique Short Id of this TaskField.
+    The value of the property
     """
 
-    value: str | None = None
+    type: str | None = None
+    """
+    The type of the property
+    """
+
+    sendToClient: bool | None = None
     """
-    The value currently set for this TaskField for this Task.
+    Send to the client true/false
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskfieldsvalueresponsedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/createtaskfielddto.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,40 +11,43 @@
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from dataclasses import dataclass
 
 @dataclass
-class TaskFieldsValueResponseDto:
+class CreateTaskFieldDto:
     """
     A TaskField is a custom field defined within your Workspace for a
     specific Project. You can define TaskFields for any integration
     purpose that is important to your business. Each TaskField has a
     data type as well as options in how it is handled. TaskFields can be
     edited for each Task inside this Project.
     """
 
-    id: str | None = None
+    name: str | None = None
     """
-    The unique identifier of this TaskField.
+    The name of the TaskField
     """
 
-    value: str | None = None
+    type: str | None = None
     """
-    The value currently set for this TaskField for this Task.
+    The type of this TaskField. Valid types are the following: * Text *
+    Number * Date * Checkbox * Currency * DropdownSingle * DropdownMulti
     """
 
-    name: str | None = None
+    options: list[str] | None = None
     """
-    The name of this TaskField.
+    A list of options for use of this TaskField. This is only valid if
+    the `Type` value is set to `Dropdown`. When a custom TaskField of
+    type `DropDown` is shown to a user in the application, they will be
+    able to choose one of the `Options` in this list.
     """
 
-    type: str | None = None
+    shortId: str | None = None
     """
-    The type of this TaskField. Valid types are the following: * Text *
-    Number * Date * Checkbox * Currency * Dropdown
+    The short Id of this field - human readable identity
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskprioritydto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskprioritydto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskprojectdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskprojectdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskstatuscreatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskstatuscreatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskstatusdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskstatusdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskstatusupdatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskstatusupdatedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tasktagdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tasktagdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/tasktododto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/tasktododto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/taskupdatedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheettaskdto.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,49 +11,46 @@
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
 from dataclasses import dataclass
 
 @dataclass
-class TaskUpdateDto:
+class TimesheetTaskDto:
     """
     A Task is an individual element of work that must be performed to
     complete a Project. A Task can have one or more Resources assigned
     to it. Tasks can be linked to other Tasks to indicate whether they
     have a dependency or a connection.
     """
 
-    name: str | None = None
+    id: str | None = None
     """
-    The common name of this Task.
+    The unique identifier of this Task.
     """
 
-    description: str | None = None
+    projectId: str | None = None
     """
-    A description of the work to be performed in this Task.
+    The unique identifier of the Project to which this Task belongs.
     """
 
-    percentComplete: int | None = None
+    shortId: str | None = None
     """
-    The numerical percentage, from 0-100, representing the percentage
-    completion for this Task. Any numbers below zero or above 100 will
-    be clamped to the minimum or maximum value. This value can be edited
-    manually in the Gantt chart view of the application, or can be
-    selected on the Task Detail page within the Kanban board.
+    A short ID that can be used to refer to this Task. This short ID is
+    guaranteed to be unique within your Workspace.
     """
 
-    statusId: str | None = None
+    name: str | None = None
     """
-    The TaskStatus assigned to this Task.
+    The common name of this Task.
     """
 
-    priorityId: int | None = None
+    description: str | None = None
     """
-    The unique identifier of the TaskPriority
+    A description of the work to be performed in this Task.
     """
 
     plannedStartDate: str | None = None
     """
     The date when work on this Task is planned to begin. This value
     contains only the date in year-month-day format. For display, this
     date will always be shown as this same year-month-day regardless of
@@ -74,50 +71,96 @@
     the official time zone of the Workspace. For example: A Task has a
     planned completion date of July 5, 2023 in a Workspace that has a
     time zone of US Pacific Time (GMT-7 or GMT-8, depending on daylight
     savings time). This project is considered overdue on 12:01 AM July
     6th 2023 in US Pacific time.
     """
 
-    plannedDuration: int | None = None
-    """
-    The planned duration (in minutes) for this Task. Cannot be negative.
-    """
-
-    plannedEffort: int | None = None
-    """
-    The planned effort (in minutes) for this Task. Cannot be negative.
-    """
-
-    plannedCost: float | None = None
-    """
-    The planned cost for this Task. Cannot be negative.
-    """
-
     actualStartDate: str | None = None
     """
     If set, this is the actual date when work began on the Task. This
     value contains only the date in year-month-day format. For display,
     this date will always be shown as this same year-month-day
     regardless of time zone. For reporting purposes, this date is
     calculated against the official time zone of the Workspace. For
     example: A Task has a planned completion date of July 5, 2023 in a
     Workspace that has a time zone of US Pacific Time (GMT-7 or GMT-8,
     depending on daylight savings time). This project is considered
     overdue on 12:01 AM July 6th 2023 in US Pacific time.
     """
 
+    actualFinishDate: str | None = None
+    """
+    If set, this is the actual date when work was completed on this
+    Task. This value contains only the date in year-month-day format.
+    For display, this date will always be shown as this same
+    year-month-day regardless of time zone. For reporting purposes, this
+    date is calculated against the official time zone of the Workspace.
+    For example: A Task has a planned completion date of July 5, 2023 in
+    a Workspace that has a time zone of US Pacific Time (GMT-7 or GMT-8,
+    depending on daylight savings time). This project is considered
+    overdue on 12:01 AM July 6th 2023 in US Pacific time.
+    """
+
+    modifyDate: str | None = None
+    """
+    The timestamp in UTC when this Task was most recently modified.
+    """
+
+    createDate: str | None = None
+    """
+    The timestamp in UTC when this Task was created.
+    """
+
+    percentComplete: int | None = None
+    """
+    The numerical percentage, from 0-100, representing the percentage
+    completion for this Task. Any numbers below zero or above 100 will
+    be clamped to the minimum or maximum value. This value can be edited
+    manually in the Gantt chart view of the application, or can be
+    selected on the Task Detail page within the Kanban board.
+    """
+
+    isSummary: bool | None = None
+    """
+    True if this Task is the parent of multiple Tasks underneath it. A
+    parent Task is a "rolled-up" view of multiple children that allows
+    you to view a section of work at a glance. You can create a summary
+    Task in the Gantt chart view of the application by adding child
+    tasks underneath a parent Task.
+    """
+
+    priorityId: int | None = None
+    """
+    Return the priority of a task
+    """
+
+    wbs: str | None = None
+    """
+    The WBS (Work Breakdown Structure) number for this task within the
+    Gantt chart hierarchy. See [What Is a Work Breakdown Structure
+    (WBS)?](https://www.projectmanager.com/guides/work-breakdown-structure)
+    on Project Manager for more information. The WBS number is an
+    outline number in the form `#.#.#.#` which indicates how tasks are
+    organized and sorted. The WBS value is only available to users at
+    certain edition levels. This value can only be changed if you are a
+    Project Editor.
+    """
+
+    color: str | None = None
+    """
+    Task Color as set in the Gantt
+    """
+
     actualCost: float | None = None
     """
-    If set, this represents the actual tracked cost for this Task.
+    The actual cost of this Task to date, if known.
     """
 
-    theme: str | None = None
+    plannedCost: float | None = None
     """
-    Color theme definition for this task. eg. Blue, Brown, DarkBlue,
-    DarkGrey, Gold, Green, Grey, LightBrown, LightGreen, LightGrey,
-    LightPurple, LightYellow, Magenta, Mauve, Navy, Orange, Purple, Red.
+    The planned cost for this Task. Cannot be negative.
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetadmintypedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetadmintypedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetcreaterequestdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetcreaterequestdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetdto.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # @author     ProjectManager.com <support@projectmanager.com>
 # @copyright  2023-2023 ProjectManager.com, Inc.
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
+from ProjectManagerSdk.models.timesheetadmintypedto import TimesheetAdminTypeDto
 from ProjectManagerSdk.models.timesheetprojectdto import TimeSheetProjectDto
 from ProjectManagerSdk.models.timesheetresourcedto import TimesheetResourceDto
 from ProjectManagerSdk.models.timesheettaskdto import TimesheetTaskDto
 from dataclasses import dataclass
 
 @dataclass
 class TimesheetDto:
@@ -64,10 +65,15 @@
     """
 
     resource: TimesheetResourceDto | None = None
     """
     The resource associated with this timesheet entry
     """
 
+    adminType: TimesheetAdminTypeDto | None = None
+    """
+    The administration type associated with this timesheet entry
+    """
+
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetprojectdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetprojectdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetresourcedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetresourcedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetresponsedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetresponsedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/timesheetupdaterequestdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/timesheetupdaterequestdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updateprojectfieldvaluedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updateprojectfieldvaluedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updaterequestdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updaterequestdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updateresourceskilldto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updateresourceskilldto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updateresourceteamdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updateresourceteamdto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/updatetaskfieldvaluedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/updatetaskfieldvaluedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/userroledto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/userroledto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/workspacedto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/workspacedto.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/workspacelinksdto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/workspacelinksdto.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 
 from dataclasses import dataclass
 
 @dataclass
 class WorkSpaceLinksDto:
     """
-    TODO - What is this?
+    A shortcut link within the currently logged in Workspace.
     """
 
     project: str | None = None
     """
-    TODO - What is this?
+    The name of the project for this link.
     """
 
     workSpaceApi: str | None = None
     """
-    This is the link to the api for this business, some legacy endpoints
-    may need this.
+    This is the link to the api for this business. Some endpoints may
+    need this value.
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/src/ProjectManagerSdk/models/workspaceuserinfodto.py` & `projectmanagersdk-99.0.2548/src/ProjectManagerSdk/models/taskfieldvaluedto.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,44 +8,49 @@
 #
 # @author     ProjectManager.com <support@projectmanager.com>
 # @copyright  2023-2023 ProjectManager.com, Inc.
 # @link       https://github.com/projectmgr/projectmanager-sdk-python
 #
 
 
-from ProjectManagerSdk.models.workspacelinksdto import WorkSpaceLinksDto
+from ProjectManagerSdk.models.taskfieldvaluetaskdto import TaskFieldValueTaskDto
 from dataclasses import dataclass
 
 @dataclass
-class WorkSpaceUserInfoDto:
+class TaskFieldValueDto:
     """
-    TODO - What is this?
+    A model that contains the value for a TaskField.
     """
 
-    links: WorkSpaceLinksDto | None = None
+    id: str | None = None
     """
-    TODO - What is this?
+    The unique identifier of this TaskField.
     """
 
-    emailAddress: str | None = None
+    shortId: str | None = None
     """
-    TODO - What is this?
+    The unique Short Id of this TaskField.
     """
 
-    id: str | None = None
+    value: str | None = None
+    """
+    The value currently set for this TaskFieldValue.
+    """
+
+    createdDate: str | None = None
     """
-    TODO - What is this?
+    Date and time (in UTC) that this TaskField was created.
     """
 
-    fullName: str | None = None
+    modifiedDate: str | None = None
     """
-    TODO - What is this?
+    Date and time (in UTC) that this TaskField was last modified.
     """
 
-    workSpaceName: str | None = None
+    task: TaskFieldValueTaskDto | None = None
     """
-    TODO - What is this?
+    The Task to which this Value belongs.
     """
 
 
     def to_dict(self) -> dict:
         return dataclass.asdict(self)
```

### Comparing `projectmanagersdk-98.0.2363/tests/test.py` & `projectmanagersdk-99.0.2548/tests/test.py`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/.gitignore` & `projectmanagersdk-99.0.2548/.gitignore`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/LICENSE` & `projectmanagersdk-99.0.2548/LICENSE`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/README.md` & `projectmanagersdk-99.0.2548/README.md`

 * *Files identical despite different names*

### Comparing `projectmanagersdk-98.0.2363/pyproject.toml` & `projectmanagersdk-99.0.2548/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ProjectManagerSdk"
-version = "98.0.2363"
+version = "99.0.2548"
 authors = [
     { name = "ProjectManager.com", email = "support@projectmanager.com" }
 ]
 description = "Software development kit for the ProjectManager.com API for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `projectmanagersdk-98.0.2363/PKG-INFO` & `projectmanagersdk-99.0.2548/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjectManagerSdk
-Version: 98.0.2363
+Version: 99.0.2548
 Summary: Software development kit for the ProjectManager.com API for Python
 Project-URL: Homepage, https://github.com/projectmgr/projectmanager-sdk-python
 Project-URL: Bug Tracker, https://github.com/projectmgr/projectmanager-sdk-python/issues
 Author-email: "ProjectManager.com" <support@projectmanager.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

