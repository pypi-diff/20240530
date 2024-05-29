# Comparing `tmp/osbot_aws-2.7.0.tar.gz` & `tmp/osbot_aws-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osbot_aws-2.7.0.tar", max compression
+gzip compressed data, was "osbot_aws-2.9.0.tar", max compression
```

## Comparing `osbot_aws-2.7.0.tar` & `osbot_aws-2.9.0.tar`

### file list

```diff
@@ -1,221 +1,222 @@
--rw-r--r--   0        0        0    11357 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/LICENSE
--rw-r--r--   0        0        0      636 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/README.md
--rw-r--r--   0        0        0     4308 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/AWS_Config.py
--rw-r--r--   0        0        0       92 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/Config.py
--rw-r--r--   0        0        0     3424 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/Dependencies.py
--rw-r--r--   0        0        0     2596 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/OSBot_Setup.py
--rw-r--r--   0        0        0       16 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/__init__.py
--rw-r--r--   0        0        0     1137 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/apis/ACM.py
--rw-r--r--   0        0        0    18486 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/apis/API_Gateway.py
--rw-r--r--   0        0        0     2400 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/apis/Athena.py
--rw-r--r--   0        0        0      370 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/apis/Boto_Helpers.py
--rw-r--r--   0        0        0     6902 2024-05-29 12:02:03.510356 osbot_aws-2.7.0/osbot_aws/apis/Cloud_Trail.py
--rw-r--r--   0        0        0    14907 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Cloud_Watch.py
--rw-r--r--   0        0        0     8632 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Cloud_Watch_Logs.py
--rw-r--r--   0        0        0     3459 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/CodeBuild.py
--rw-r--r--   0        0        0     6297 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Cognito_IDP.py
--rw-r--r--   0        0        0    25047 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/EC2.py
--rw-r--r--   0        0        0     2904 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/ECR.py
--rw-r--r--   0        0        0     5170 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Events.py
--rw-r--r--   0        0        0     4033 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Firehose.py
--rw-r--r--   0        0        0      341 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Kinesis.py
--rw-r--r--   0        0        0    22500 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Lambda.py
--rw-r--r--   0        0        0      730 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Lambda_Docker.py
--rw-r--r--   0        0        0    10392 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Lambda_Http.py
--rw-r--r--   0        0        0     7751 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Lambda_Layer.py
--rw-r--r--   0        0        0     8402 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Logs.py
--rw-r--r--   0        0        0    16253 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/S3.py
--rw-r--r--   0        0        0     8568 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/SQS.py
--rw-r--r--   0        0        0     1161 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/SSM.py
--rw-r--r--   0        0        0     2785 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Secrets.py
--rw-r--r--   0        0        0     8807 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/Session.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/__init__.py
--rw-r--r--   0        0        0     2795 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/shell/Lambda_Shell.py
--rw-r--r--   0        0        0     3904 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/shell/Shell_Client.py
--rw-r--r--   0        0        0     2062 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/shell/Shell_Server.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/shell/__init__.py
--rw-r--r--   0        0        0     1087 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py
--rw-r--r--   0        0        0      623 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_EC2_Instance.py
--rw-r--r--   0        0        0      559 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Event_Rule.py
--rw-r--r--   0        0        0      984 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Event_Rule_To_SQS_Queue.py
--rw-r--r--   0        0        0     1433 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Folder_With_Lambda_File.py
--rw-r--r--   0        0        0      492 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_IAM_Role.py
--rw-r--r--   0        0        0      404 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_IAM_User.py
--rw-r--r--   0        0        0     3131 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Lambda.py
--rw-r--r--   0        0        0     2956 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_S3_Zip_With_Lambda_File.py
--rw-r--r--   0        0        0      868 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_SQS_Queue.py
--rw-r--r--   0        0        0     2349 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_VPC.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/apis/test_helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/__init__.py
--rw-r--r--   0        0        0     1005 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/API_Gateway_Management_API.py
--rw-r--r--   0        0        0      919 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/API_Gateway_V2.py
--rw-r--r--   0        0        0     1521 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/API_Gateway_V2__with_temp_role.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/__init__.py
--rw-r--r--   0        0        0      945 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Connection.py
--rw-r--r--   0        0        0     5209 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/apigw_dydb/WS__DyDB.py
--rw-r--r--   0        0        0     1219 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Events.py
--rw-r--r--   0        0        0     1454 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Lambda.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/apigw_dydb/__init__.py
--rw-r--r--   0        0        0      481 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/lambdas/Deploy__lambda_web_sockets.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/lambdas/__init__.py
--rw-r--r--   0        0        0      209 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/apigateway/lambdas/lambda_web_sockets.py
--rw-r--r--   0        0        0     3698 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/Bedrock.py
--rw-r--r--   0        0        0     2026 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/Bedrock__with_temp_role.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/__init__.py
--rw-r--r--   0        0        0     4050 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/Bedrock__Cache.py
--rw-r--r--   0        0        0      608 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/Sqlite__Bedrock__Row.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/__init__.py
--rw-r--r--   0        0        0     2547 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html.py
--rw-r--r--   0        0        0     8447 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_Table.py
--rw-r--r--   0        0        0     6263 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_With_Images.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/html/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/__init__.py
--rw-r--r--   0        0        0      774 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2.py
--rw-r--r--   0        0        0      181 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Mid.py
--rw-r--r--   0        0        0      185 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Ultra.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/ai21/__init__.py
--rw-r--r--   0        0        0     1116 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Instant_V1.py
--rw-r--r--   0        0        0     1020 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Messages_API.py
--rw-r--r--   0        0        0      205 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_0.py
--rw-r--r--   0        0        0      207 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_1.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/claude/__init__.py
--rw-r--r--   0        0        0     1318 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/command/Cohere_Command.py
--rw-r--r--   0        0        0      186 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Light_Text_V14.py
--rw-r--r--   0        0        0      174 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Text_V14.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/command/__init__.py
--rw-r--r--   0        0        0      798 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion.py
--rw-r--r--   0        0        0      676 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V0.py
--rw-r--r--   0        0        0     2293 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1.py
--rw-r--r--   0        0        0     1396 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Image_To_Image.py
--rw-r--r--   0        0        0      738 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Text_To_Image.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/__init__.py
--rw-r--r--   0        0        0      518 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2.py
--rw-r--r--   0        0        0      164 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_13b_chat_v1.py
--rw-r--r--   0        0        0      164 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_70b_chat_v1.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/llama2/__init__.py
--rw-r--r--   0        0        0      714 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI.py
--rw-r--r--   0        0        0      175 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_7b_Instruct_v0_2.py
--rw-r--r--   0        0        0      179 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_8x7b_Instruct_v0_1.py
--rw-r--r--   0        0        0      173 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_Large_2402_v1_0.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/mistral/__init__.py
--rw-r--r--   0        0        0     3739 2024-05-29 12:02:03.514356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Image_Generator_V1.py
--rw-r--r--   0        0        0      348 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Express_V1.py
--rw-r--r--   0        0        0      342 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Lite_V1.py
--rw-r--r--   0        0        0      318 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Tg1_Large.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/titan/__init__.py
--rw-r--r--   0        0        0     1011 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/titan/base_classes/Amazon_Titan__Text.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/titan/base_classes/__init__.py
--rw-r--r--   0        0        0     1734 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/boto3/Cache_Boto3_Requests.py
--rw-r--r--   0        0        0     2844 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/boto3/Capture_Boto3_Error.py
--rw-r--r--   0        0        0     5978 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/boto3/View_Boto3_Rest_Calls.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/boto3/__init__.py
--rw-r--r--   0        0        0      481 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/cloud_front/Cloud_Front.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/cloud_front/__init__.py
--rw-r--r--   0        0        0     5202 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/code_artifact/Code_Artifact.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/code_artifact/__init__.py
--rw-r--r--   0        0        0    13036 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_DB.py
--rw-r--r--   0        0        0     1412 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Record.py
--rw-r--r--   0        0        0      280 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Streams.py
--rw-r--r--   0        0        0     6960 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Table.py
--rw-r--r--   0        0        0     1294 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_DB__with_temp_role.py
--rw-r--r--   0        0        0     4040 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/__init__.py
--rw-r--r--   0        0        0     7015 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table.py
--rw-r--r--   0        0        0     2217 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_GSI.py
--rw-r--r--   0        0        0     4556 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_Timestamp.py
--rw-r--r--   0        0        0     1084 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table__Resources.py
--rw-r--r--   0        0        0     5693 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Timeseries.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/__init__.py
--rw-r--r--   0        0        0     7645 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/models/DyDB__Document.py
--rw-r--r--   0        0        0     9656 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/models/DyDB__Query__Builder.py
--rw-r--r--   0        0        0      313 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/models/DyDB__Resource.py
--rw-r--r--   0        0        0      303 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/models/Resource__Config.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/models/__init__.py
--rw-r--r--   0        0        0    21575 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/ecs/ECS.py
--rw-r--r--   0        0        0      733 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/ecs/ECS_Actions.py
--rw-r--r--   0        0        0      270 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/ecs/ECS_Cluster.py
--rw-r--r--   0        0        0     7074 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/ecs/ECS_Fargate_Task.py
--rw-r--r--   0        0        0      631 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/ecs/Temp_ECS_Fargate_Task.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/ecs/__init__.py
--rw-r--r--   0        0        0     2398 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/iam/Capture_IAM_Exception.py
--rw-r--r--   0        0        0    21766 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/iam/IAM.py
--rw-r--r--   0        0        0     9963 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Assume_Role.py
--rw-r--r--   0        0        0     1831 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Policy.py
--rw-r--r--   0        0        0     4700 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Role.py
--rw-r--r--   0        0        0     1328 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Role_With_Policy.py
--rw-r--r--   0        0        0     3041 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_User.py
--rw-r--r--   0        0        0      964 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Utils.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/iam/__init__.py
--rw-r--r--   0        0        0     2029 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/lambda_/Lambda__with_temp_role.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/lambda_/__init__.py
--rw-r--r--   0        0        0      557 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/organizations/Organizations.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/organizations/__init__.py
--rw-r--r--   0        0        0     5975 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/route_53/Route_53.py
--rw-r--r--   0        0        0     2226 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/route_53/Route_53__Hosted_Zone.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/route_53/__init__.py
--rw-r--r--   0        0        0     1458 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/s3/S3__with_temp_role.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/s3/__init__.py
--rw-r--r--   0        0        0     4849 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/sts/STS.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/aws/sts/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/decorators/__init__.py
--rw-r--r--   0        0        0      808 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/decorators/aws_inject.py
--rw-r--r--   0        0        0      942 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/decorators/aws_retry.py
--rw-r--r--   0        0        0     2913 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/decorators/enforce_type_safety.py
--rw-r--r--   0        0        0      686 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/decorators/lambda_save_event.py
--rw-r--r--   0        0        0     4865 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/deploy/Deploy_Lambda.py
--rw-r--r--   0        0        0     1367 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/deploy/TestCase__Lambda__Deploy.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/deploy/__init__.py
--rw-r--r--   0        0        0      948 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/exceptions/Session_Bad_Credentials.py
--rw-r--r--   0        0        0      330 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/exceptions/Session_Client_Creation_Fail.py
--rw-r--r--   0        0        0      610 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/exceptions/Session_No_Credentials.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/exceptions/__init__.py
--rw-r--r--   0        0        0      959 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/AMI.py
--rw-r--r--   0        0        0     2595 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Aws_Cli.py
--rw-r--r--   0        0        0    11778 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Create_Code_Build.py
--rw-r--r--   0        0        0     2920 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Create_Image_ECR.py
--rw-r--r--   0        0        0     2038 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/EC_Instance.py
--rw-r--r--   0        0        0     2544 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Event_Rule.py
--rw-r--r--   0        0        0       61 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Lambda_From_S3.py
--rw-r--r--   0        0        0     1771 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Helpers.py
--rw-r--r--   0        0        0     6311 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Layer_Create.py
--rw-r--r--   0        0        0      494 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Layers_Local.py
--rw-r--r--   0        0        0     2845 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Layers_OSBot.py
--rw-r--r--   0        0        0     8284 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Package.py
--rw-r--r--   0        0        0     2001 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Lambda_SSH.py
--rw-r--r--   0        0        0     1247 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Lambda_SSH_Kubectl.py
--rw-r--r--   0        0        0     1338 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Upload_Package.py
--rw-r--r--   0        0        0     2154 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Parameter.py
--rw-r--r--   0        0        0     4127 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/Rest_API.py
--rw-r--r--   0        0        0     1497 2024-05-29 12:02:03.518356 osbot_aws-2.7.0/osbot_aws/helpers/S3_Zip_From_Files.py
--rw-r--r--   0        0        0     5565 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/helpers/SQS_Queue.py
--rw-r--r--   0        0        0     1562 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/helpers/Test_Helper.py
--rw-r--r--   0        0        0     2181 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/helpers/VPC.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/dev/__init__.py
--rw-r--r--   0        0        0      127 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/dev/check_aws_api.py
--rw-r--r--   0        0        0      139 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/dev/check_python_utils.py
--rw-r--r--   0        0        0       87 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/dev/hello_world.py
--rw-r--r--   0        0        0      137 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/dev/lambda_layer.py
--rw-r--r--   0        0        0      326 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/dev/write_cloud_watch_log.py
--rw-r--r--   0        0        0      221 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/dev/write_queue.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/pocs/__init__.py
--rw-r--r--   0        0        0      353 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/pocs/confirm_process_stay_alive.py
--rw-r--r--   0        0        0      648 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py
--rw-r--r--   0        0        0      230 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/pocs/send_event_data_to_queue.py
--rw-r--r--   0        0        0     1916 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/server_ssh.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/shell/__init__.py
--rw-r--r--   0        0        0      138 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/shell/lambda_shell.py
--rw-r--r--   0        0        0      129 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/lambdas/shell/shell_server.py
--rw-r--r--   0        0        0      575 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/testing/TestCase__API_Gateway_V2.py
--rw-r--r--   0        0        0      973 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/testing/TestCase__Bedrock.py
--rw-r--r--   0        0        0      431 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/testing/TestCase__Boto3_Cache.py
--rw-r--r--   0        0        0      525 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/testing/TestCase__Dynamo_DB.py
--rw-r--r--   0        0        0     1707 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/testing/TestCase__Lambda.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/testing/__init__.py
--rw-r--r--   0        0        0       91 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/utils/Execution_Env.py
--rw-r--r--   0        0        0      458 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/utils/Version.py
--rw-r--r--   0        0        0        0 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/utils/__init__.py
--rw-r--r--   0        0        0        7 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/osbot_aws/version
--rw-r--r--   0        0        0      677 2024-05-29 12:02:03.522356 osbot_aws-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     1277 1970-01-01 00:00:00.000000 osbot_aws-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 14:34:11.545262 osbot_aws-2.9.0/LICENSE
+-rw-r--r--   0        0        0      636 2024-05-29 14:34:11.545262 osbot_aws-2.9.0/README.md
+-rw-r--r--   0        0        0     4308 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/AWS_Config.py
+-rw-r--r--   0        0        0       92 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/Config.py
+-rw-r--r--   0        0        0     3424 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/Dependencies.py
+-rw-r--r--   0        0        0     2596 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/OSBot_Setup.py
+-rw-r--r--   0        0        0       16 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/__init__.py
+-rw-r--r--   0        0        0     1137 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/ACM.py
+-rw-r--r--   0        0        0    18486 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/API_Gateway.py
+-rw-r--r--   0        0        0     2400 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Athena.py
+-rw-r--r--   0        0        0      370 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Boto_Helpers.py
+-rw-r--r--   0        0        0     6902 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Cloud_Trail.py
+-rw-r--r--   0        0        0    14907 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Cloud_Watch.py
+-rw-r--r--   0        0        0     8632 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Cloud_Watch_Logs.py
+-rw-r--r--   0        0        0     3459 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/CodeBuild.py
+-rw-r--r--   0        0        0     6297 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Cognito_IDP.py
+-rw-r--r--   0        0        0    25047 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/EC2.py
+-rw-r--r--   0        0        0     2904 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/ECR.py
+-rw-r--r--   0        0        0     5170 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Events.py
+-rw-r--r--   0        0        0     4033 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Firehose.py
+-rw-r--r--   0        0        0      341 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Kinesis.py
+-rw-r--r--   0        0        0    22500 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Lambda.py
+-rw-r--r--   0        0        0      730 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Lambda_Docker.py
+-rw-r--r--   0        0        0    10392 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Lambda_Http.py
+-rw-r--r--   0        0        0     7751 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Lambda_Layer.py
+-rw-r--r--   0        0        0     8402 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Logs.py
+-rw-r--r--   0        0        0    16253 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/S3.py
+-rw-r--r--   0        0        0     8568 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/SQS.py
+-rw-r--r--   0        0        0     1161 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/SSM.py
+-rw-r--r--   0        0        0     2785 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Secrets.py
+-rw-r--r--   0        0        0     8807 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/Session.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/__init__.py
+-rw-r--r--   0        0        0     2795 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/shell/Lambda_Shell.py
+-rw-r--r--   0        0        0     3994 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/shell/Shell_Client.py
+-rw-r--r--   0        0        0      726 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/shell/Shell_Client__Local_Docker.py
+-rw-r--r--   0        0        0     2062 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/shell/Shell_Server.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/shell/__init__.py
+-rw-r--r--   0        0        0     1087 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py
+-rw-r--r--   0        0        0      623 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_EC2_Instance.py
+-rw-r--r--   0        0        0      559 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Event_Rule.py
+-rw-r--r--   0        0        0      984 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Event_Rule_To_SQS_Queue.py
+-rw-r--r--   0        0        0     1433 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Folder_With_Lambda_File.py
+-rw-r--r--   0        0        0      492 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_IAM_Role.py
+-rw-r--r--   0        0        0      404 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_IAM_User.py
+-rw-r--r--   0        0        0     3131 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Lambda.py
+-rw-r--r--   0        0        0     2956 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_S3_Zip_With_Lambda_File.py
+-rw-r--r--   0        0        0      868 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_SQS_Queue.py
+-rw-r--r--   0        0        0     2349 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_VPC.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/apis/test_helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/API_Gateway_Management_API.py
+-rw-r--r--   0        0        0      919 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/API_Gateway_V2.py
+-rw-r--r--   0        0        0     1521 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/API_Gateway_V2__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/__init__.py
+-rw-r--r--   0        0        0      945 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Connection.py
+-rw-r--r--   0        0        0     5209 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/apigw_dydb/WS__DyDB.py
+-rw-r--r--   0        0        0     1219 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Events.py
+-rw-r--r--   0        0        0     1454 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Lambda.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/apigw_dydb/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/lambdas/Deploy__lambda_web_sockets.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/lambdas/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/apigateway/lambdas/lambda_web_sockets.py
+-rw-r--r--   0        0        0     3698 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/Bedrock.py
+-rw-r--r--   0        0        0     2026 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/Bedrock__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/__init__.py
+-rw-r--r--   0        0        0     4050 2024-05-29 14:34:11.549263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/Bedrock__Cache.py
+-rw-r--r--   0        0        0      608 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/Sqlite__Bedrock__Row.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/__init__.py
+-rw-r--r--   0        0        0     2547 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html.py
+-rw-r--r--   0        0        0     8447 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_Table.py
+-rw-r--r--   0        0        0     6263 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_With_Images.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/html/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2.py
+-rw-r--r--   0        0        0      181 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Mid.py
+-rw-r--r--   0        0        0      185 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Ultra.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/ai21/__init__.py
+-rw-r--r--   0        0        0     1116 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Instant_V1.py
+-rw-r--r--   0        0        0     1020 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Messages_API.py
+-rw-r--r--   0        0        0      205 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_0.py
+-rw-r--r--   0        0        0      207 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_1.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/claude/__init__.py
+-rw-r--r--   0        0        0     1318 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/command/Cohere_Command.py
+-rw-r--r--   0        0        0      186 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Light_Text_V14.py
+-rw-r--r--   0        0        0      174 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Text_V14.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/command/__init__.py
+-rw-r--r--   0        0        0      798 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion.py
+-rw-r--r--   0        0        0      676 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V0.py
+-rw-r--r--   0        0        0     2293 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1.py
+-rw-r--r--   0        0        0     1396 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Image_To_Image.py
+-rw-r--r--   0        0        0      738 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Text_To_Image.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/__init__.py
+-rw-r--r--   0        0        0      518 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2.py
+-rw-r--r--   0        0        0      164 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_13b_chat_v1.py
+-rw-r--r--   0        0        0      164 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_70b_chat_v1.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/llama2/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI.py
+-rw-r--r--   0        0        0      175 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_7b_Instruct_v0_2.py
+-rw-r--r--   0        0        0      179 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_8x7b_Instruct_v0_1.py
+-rw-r--r--   0        0        0      173 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_Large_2402_v1_0.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/mistral/__init__.py
+-rw-r--r--   0        0        0     3739 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Image_Generator_V1.py
+-rw-r--r--   0        0        0      348 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Express_V1.py
+-rw-r--r--   0        0        0      342 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Lite_V1.py
+-rw-r--r--   0        0        0      318 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Tg1_Large.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/titan/__init__.py
+-rw-r--r--   0        0        0     1011 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/titan/base_classes/Amazon_Titan__Text.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/titan/base_classes/__init__.py
+-rw-r--r--   0        0        0     1734 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/boto3/Cache_Boto3_Requests.py
+-rw-r--r--   0        0        0     2844 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/boto3/Capture_Boto3_Error.py
+-rw-r--r--   0        0        0     5978 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/boto3/View_Boto3_Rest_Calls.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/boto3/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/cloud_front/Cloud_Front.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/cloud_front/__init__.py
+-rw-r--r--   0        0        0     5202 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/code_artifact/Code_Artifact.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/code_artifact/__init__.py
+-rw-r--r--   0        0        0    13036 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_DB.py
+-rw-r--r--   0        0        0     1412 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Record.py
+-rw-r--r--   0        0        0      280 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Streams.py
+-rw-r--r--   0        0        0     6960 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Table.py
+-rw-r--r--   0        0        0     1294 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_DB__with_temp_role.py
+-rw-r--r--   0        0        0     4040 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/__init__.py
+-rw-r--r--   0        0        0     7015 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table.py
+-rw-r--r--   0        0        0     2217 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_GSI.py
+-rw-r--r--   0        0        0     4556 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_Timestamp.py
+-rw-r--r--   0        0        0     1084 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table__Resources.py
+-rw-r--r--   0        0        0     5693 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Timeseries.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/__init__.py
+-rw-r--r--   0        0        0     7645 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/models/DyDB__Document.py
+-rw-r--r--   0        0        0     9656 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/models/DyDB__Query__Builder.py
+-rw-r--r--   0        0        0      313 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/models/DyDB__Resource.py
+-rw-r--r--   0        0        0      303 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/models/Resource__Config.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/models/__init__.py
+-rw-r--r--   0        0        0    21575 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/ecs/ECS.py
+-rw-r--r--   0        0        0      733 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/ecs/ECS_Actions.py
+-rw-r--r--   0        0        0      270 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/ecs/ECS_Cluster.py
+-rw-r--r--   0        0        0     7074 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/ecs/ECS_Fargate_Task.py
+-rw-r--r--   0        0        0      631 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/ecs/Temp_ECS_Fargate_Task.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/ecs/__init__.py
+-rw-r--r--   0        0        0     2398 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/iam/Capture_IAM_Exception.py
+-rw-r--r--   0        0        0    21766 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/iam/IAM.py
+-rw-r--r--   0        0        0     9963 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Assume_Role.py
+-rw-r--r--   0        0        0     1831 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Policy.py
+-rw-r--r--   0        0        0     4700 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Role.py
+-rw-r--r--   0        0        0     1328 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Role_With_Policy.py
+-rw-r--r--   0        0        0     3041 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_User.py
+-rw-r--r--   0        0        0      964 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Utils.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/iam/__init__.py
+-rw-r--r--   0        0        0     2029 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/lambda_/Lambda__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/lambda_/__init__.py
+-rw-r--r--   0        0        0      557 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/organizations/Organizations.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/organizations/__init__.py
+-rw-r--r--   0        0        0     5975 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/route_53/Route_53.py
+-rw-r--r--   0        0        0     2226 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/route_53/Route_53__Hosted_Zone.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.553263 osbot_aws-2.9.0/osbot_aws/aws/route_53/__init__.py
+-rw-r--r--   0        0        0     1458 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/aws/s3/S3__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/aws/s3/__init__.py
+-rw-r--r--   0        0        0     4849 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/aws/sts/STS.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/aws/sts/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      808 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/decorators/aws_inject.py
+-rw-r--r--   0        0        0      942 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/decorators/aws_retry.py
+-rw-r--r--   0        0        0     2913 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/decorators/enforce_type_safety.py
+-rw-r--r--   0        0        0      686 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/decorators/lambda_save_event.py
+-rw-r--r--   0        0        0     4865 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/deploy/Deploy_Lambda.py
+-rw-r--r--   0        0        0     1367 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/deploy/TestCase__Lambda__Deploy.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/deploy/__init__.py
+-rw-r--r--   0        0        0      948 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/exceptions/Session_Bad_Credentials.py
+-rw-r--r--   0        0        0      330 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/exceptions/Session_Client_Creation_Fail.py
+-rw-r--r--   0        0        0      610 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/exceptions/Session_No_Credentials.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/exceptions/__init__.py
+-rw-r--r--   0        0        0      959 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/AMI.py
+-rw-r--r--   0        0        0     2595 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Aws_Cli.py
+-rw-r--r--   0        0        0    11778 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Create_Code_Build.py
+-rw-r--r--   0        0        0     2920 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Create_Image_ECR.py
+-rw-r--r--   0        0        0     2038 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/EC_Instance.py
+-rw-r--r--   0        0        0     2544 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Event_Rule.py
+-rw-r--r--   0        0        0       61 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Lambda_From_S3.py
+-rw-r--r--   0        0        0     1771 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Helpers.py
+-rw-r--r--   0        0        0     6311 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Layer_Create.py
+-rw-r--r--   0        0        0      494 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Layers_Local.py
+-rw-r--r--   0        0        0     2845 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Layers_OSBot.py
+-rw-r--r--   0        0        0     8284 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Package.py
+-rw-r--r--   0        0        0     2001 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Lambda_SSH.py
+-rw-r--r--   0        0        0     1247 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Lambda_SSH_Kubectl.py
+-rw-r--r--   0        0        0     1338 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Upload_Package.py
+-rw-r--r--   0        0        0     2154 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Parameter.py
+-rw-r--r--   0        0        0     4127 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Rest_API.py
+-rw-r--r--   0        0        0     1497 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/S3_Zip_From_Files.py
+-rw-r--r--   0        0        0     5565 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/SQS_Queue.py
+-rw-r--r--   0        0        0     1562 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/Test_Helper.py
+-rw-r--r--   0        0        0     2181 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/VPC.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/dev/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/dev/check_aws_api.py
+-rw-r--r--   0        0        0      139 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/dev/check_python_utils.py
+-rw-r--r--   0        0        0       87 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/dev/hello_world.py
+-rw-r--r--   0        0        0      137 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/dev/lambda_layer.py
+-rw-r--r--   0        0        0      326 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/dev/write_cloud_watch_log.py
+-rw-r--r--   0        0        0      221 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/dev/write_queue.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/pocs/__init__.py
+-rw-r--r--   0        0        0      353 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/pocs/confirm_process_stay_alive.py
+-rw-r--r--   0        0        0      648 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py
+-rw-r--r--   0        0        0      230 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/pocs/send_event_data_to_queue.py
+-rw-r--r--   0        0        0     1916 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/server_ssh.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/shell/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/shell/lambda_shell.py
+-rw-r--r--   0        0        0      129 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/lambdas/shell/shell_server.py
+-rw-r--r--   0        0        0      575 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/testing/TestCase__API_Gateway_V2.py
+-rw-r--r--   0        0        0      973 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/testing/TestCase__Bedrock.py
+-rw-r--r--   0        0        0      431 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/testing/TestCase__Boto3_Cache.py
+-rw-r--r--   0        0        0      525 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/testing/TestCase__Dynamo_DB.py
+-rw-r--r--   0        0        0     1707 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/testing/TestCase__Lambda.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/testing/__init__.py
+-rw-r--r--   0        0        0       91 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/utils/Execution_Env.py
+-rw-r--r--   0        0        0      458 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/utils/Version.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/utils/__init__.py
+-rw-r--r--   0        0        0        7 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/osbot_aws/version
+-rw-r--r--   0        0        0      677 2024-05-29 14:34:11.557263 osbot_aws-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1277 1970-01-01 00:00:00.000000 osbot_aws-2.9.0/PKG-INFO
```

### Comparing `osbot_aws-2.7.0/LICENSE` & `osbot_aws-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/README.md` & `osbot_aws-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # OSBot-AWS
 
-![Current Release](https://img.shields.io/badge/release-v2.7.0-blue)
+![Current Release](https://img.shields.io/badge/release-v2.9.0-blue)
 
 Large number of AWS apis and utils from the OWASP Security Bot (OSBot) which make
 the use of AWS's boto3 library easier and more intuitive.
 
 ## Current version is 2.x.x 
 
 This version has a number of breaking changes, mainly on the location of the apis,
```

### Comparing `osbot_aws-2.7.0/osbot_aws/AWS_Config.py` & `osbot_aws-2.9.0/osbot_aws/AWS_Config.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/Dependencies.py` & `osbot_aws-2.9.0/osbot_aws/Dependencies.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/OSBot_Setup.py` & `osbot_aws-2.9.0/osbot_aws/OSBot_Setup.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/ACM.py` & `osbot_aws-2.9.0/osbot_aws/apis/ACM.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/API_Gateway.py` & `osbot_aws-2.9.0/osbot_aws/apis/API_Gateway.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Athena.py` & `osbot_aws-2.9.0/osbot_aws/apis/Athena.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Cloud_Trail.py` & `osbot_aws-2.9.0/osbot_aws/apis/Cloud_Trail.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Cloud_Watch.py` & `osbot_aws-2.9.0/osbot_aws/apis/Cloud_Watch.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Cloud_Watch_Logs.py` & `osbot_aws-2.9.0/osbot_aws/apis/Cloud_Watch_Logs.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/CodeBuild.py` & `osbot_aws-2.9.0/osbot_aws/apis/CodeBuild.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Cognito_IDP.py` & `osbot_aws-2.9.0/osbot_aws/apis/Cognito_IDP.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/EC2.py` & `osbot_aws-2.9.0/osbot_aws/apis/EC2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/ECR.py` & `osbot_aws-2.9.0/osbot_aws/apis/ECR.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Events.py` & `osbot_aws-2.9.0/osbot_aws/apis/Events.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Firehose.py` & `osbot_aws-2.9.0/osbot_aws/apis/Firehose.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Lambda.py` & `osbot_aws-2.9.0/osbot_aws/apis/Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Lambda_Docker.py` & `osbot_aws-2.9.0/osbot_aws/apis/Lambda_Docker.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Lambda_Http.py` & `osbot_aws-2.9.0/osbot_aws/apis/Lambda_Http.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Lambda_Layer.py` & `osbot_aws-2.9.0/osbot_aws/apis/Lambda_Layer.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Logs.py` & `osbot_aws-2.9.0/osbot_aws/apis/Logs.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/S3.py` & `osbot_aws-2.9.0/osbot_aws/apis/S3.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/SQS.py` & `osbot_aws-2.9.0/osbot_aws/apis/SQS.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/SSM.py` & `osbot_aws-2.9.0/osbot_aws/apis/SSM.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Secrets.py` & `osbot_aws-2.9.0/osbot_aws/apis/Secrets.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/Session.py` & `osbot_aws-2.9.0/osbot_aws/apis/Session.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/shell/Lambda_Shell.py` & `osbot_aws-2.9.0/osbot_aws/apis/shell/Lambda_Shell.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/shell/Shell_Client.py` & `osbot_aws-2.9.0/osbot_aws/apis/shell/Shell_Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from osbot_aws.AWS_Config import AWS_Config
 from osbot_aws.apis.shell.Lambda_Shell import Lambda_Shell
 from osbot_aws.apis.shell.Shell_Server import Shell_Server
 from osbot_aws.apis.Lambda import Lambda                    # todo: see how to resolve the circular dependency with the Lambda Function
+from osbot_utils.decorators.methods.cache_on_self import cache_on_self
 from osbot_utils.utils.Functions import function_source_code
 
 
 class Shell_Client:
 
     def __init__(self, aws_lambda: Lambda):
         self.aws_lambda = aws_lambda
 
+    @cache_on_self
     def _lambda_auth_key(self):
         return Lambda_Shell().get_lambda_shell_auth()
 
     def _invoke(self, method_name, method_kwargs=None,return_logs=False):
         event = {'lambda_shell': {'method_name': method_name, 'method_kwargs': method_kwargs}}
         if self.aws_lambda:
             event['lambda_shell']['auth_key'] = self._lambda_auth_key()
```

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/shell/Shell_Server.py` & `osbot_aws-2.9.0/osbot_aws/apis/shell/Shell_Server.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py` & `osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_EC2_Instance.py` & `osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_EC2_Instance.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Event_Rule.py` & `osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Event_Rule.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Event_Rule_To_SQS_Queue.py` & `osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Event_Rule_To_SQS_Queue.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Folder_With_Lambda_File.py` & `osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Folder_With_Lambda_File.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_Lambda.py` & `osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_S3_Zip_With_Lambda_File.py` & `osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_S3_Zip_With_Lambda_File.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_SQS_Queue.py` & `osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_SQS_Queue.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/apis/test_helpers/Temp_VPC.py` & `osbot_aws-2.9.0/osbot_aws/apis/test_helpers/Temp_VPC.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/apigateway/API_Gateway_Management_API.py` & `osbot_aws-2.9.0/osbot_aws/aws/apigateway/API_Gateway_Management_API.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/apigateway/API_Gateway_V2.py` & `osbot_aws-2.9.0/osbot_aws/aws/apigateway/API_Gateway_V2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/apigateway/API_Gateway_V2__with_temp_role.py` & `osbot_aws-2.9.0/osbot_aws/aws/apigateway/API_Gateway_V2__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Connection.py` & `osbot_aws-2.9.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Connection.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/apigateway/apigw_dydb/WS__DyDB.py` & `osbot_aws-2.9.0/osbot_aws/aws/apigateway/apigw_dydb/WS__DyDB.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Events.py` & `osbot_aws-2.9.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Events.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Lambda.py` & `osbot_aws-2.9.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/Bedrock.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/Bedrock.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/Bedrock__with_temp_role.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/Bedrock__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/Bedrock__Cache.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/Bedrock__Cache.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/Sqlite__Bedrock__Row.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/Sqlite__Bedrock__Row.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_Table.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_Table.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_With_Images.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_With_Images.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Instant_V1.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Instant_V1.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Messages_API.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Messages_API.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/command/Cohere_Command.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/command/Cohere_Command.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V0.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V0.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Image_To_Image.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Image_To_Image.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Text_To_Image.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Text_To_Image.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Image_Generator_V1.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Image_Generator_V1.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/bedrock/models/titan/base_classes/Amazon_Titan__Text.py` & `osbot_aws-2.9.0/osbot_aws/aws/bedrock/models/titan/base_classes/Amazon_Titan__Text.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/boto3/Cache_Boto3_Requests.py` & `osbot_aws-2.9.0/osbot_aws/aws/boto3/Cache_Boto3_Requests.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/boto3/Capture_Boto3_Error.py` & `osbot_aws-2.9.0/osbot_aws/aws/boto3/Capture_Boto3_Error.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/boto3/View_Boto3_Rest_Calls.py` & `osbot_aws-2.9.0/osbot_aws/aws/boto3/View_Boto3_Rest_Calls.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/code_artifact/Code_Artifact.py` & `osbot_aws-2.9.0/osbot_aws/aws/code_artifact/Code_Artifact.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_DB.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_DB.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Record.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Record.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Table.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Table.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_DB__with_temp_role.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_DB__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_GSI.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_GSI.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_Timestamp.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_Timestamp.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table__Resources.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table__Resources.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/domains/DyDB__Timeseries.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/domains/DyDB__Timeseries.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/models/DyDB__Document.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/models/DyDB__Document.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/dynamo_db/models/DyDB__Query__Builder.py` & `osbot_aws-2.9.0/osbot_aws/aws/dynamo_db/models/DyDB__Query__Builder.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/ecs/ECS.py` & `osbot_aws-2.9.0/osbot_aws/aws/ecs/ECS.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/ecs/ECS_Actions.py` & `osbot_aws-2.9.0/osbot_aws/aws/ecs/ECS_Actions.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/ecs/ECS_Fargate_Task.py` & `osbot_aws-2.9.0/osbot_aws/aws/ecs/ECS_Fargate_Task.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/ecs/Temp_ECS_Fargate_Task.py` & `osbot_aws-2.9.0/osbot_aws/aws/ecs/Temp_ECS_Fargate_Task.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/iam/Capture_IAM_Exception.py` & `osbot_aws-2.9.0/osbot_aws/aws/iam/Capture_IAM_Exception.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/iam/IAM.py` & `osbot_aws-2.9.0/osbot_aws/aws/iam/IAM.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Assume_Role.py` & `osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Assume_Role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Policy.py` & `osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Policy.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Role.py` & `osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Role_With_Policy.py` & `osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Role_With_Policy.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_User.py` & `osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_User.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/iam/IAM_Utils.py` & `osbot_aws-2.9.0/osbot_aws/aws/iam/IAM_Utils.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/lambda_/Lambda__with_temp_role.py` & `osbot_aws-2.9.0/osbot_aws/aws/lambda_/Lambda__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/organizations/Organizations.py` & `osbot_aws-2.9.0/osbot_aws/aws/organizations/Organizations.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/route_53/Route_53.py` & `osbot_aws-2.9.0/osbot_aws/aws/route_53/Route_53.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/route_53/Route_53__Hosted_Zone.py` & `osbot_aws-2.9.0/osbot_aws/aws/route_53/Route_53__Hosted_Zone.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/s3/S3__with_temp_role.py` & `osbot_aws-2.9.0/osbot_aws/aws/s3/S3__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/aws/sts/STS.py` & `osbot_aws-2.9.0/osbot_aws/aws/sts/STS.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/decorators/aws_inject.py` & `osbot_aws-2.9.0/osbot_aws/decorators/aws_inject.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/decorators/aws_retry.py` & `osbot_aws-2.9.0/osbot_aws/decorators/aws_retry.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/decorators/enforce_type_safety.py` & `osbot_aws-2.9.0/osbot_aws/decorators/enforce_type_safety.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/decorators/lambda_save_event.py` & `osbot_aws-2.9.0/osbot_aws/decorators/lambda_save_event.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/deploy/Deploy_Lambda.py` & `osbot_aws-2.9.0/osbot_aws/deploy/Deploy_Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/deploy/TestCase__Lambda__Deploy.py` & `osbot_aws-2.9.0/osbot_aws/deploy/TestCase__Lambda__Deploy.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/exceptions/Session_Bad_Credentials.py` & `osbot_aws-2.9.0/osbot_aws/exceptions/Session_Bad_Credentials.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/exceptions/Session_No_Credentials.py` & `osbot_aws-2.9.0/osbot_aws/exceptions/Session_No_Credentials.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/AMI.py` & `osbot_aws-2.9.0/osbot_aws/helpers/AMI.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Aws_Cli.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Aws_Cli.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Create_Code_Build.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Create_Code_Build.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Create_Image_ECR.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Create_Image_ECR.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/EC_Instance.py` & `osbot_aws-2.9.0/osbot_aws/helpers/EC_Instance.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Event_Rule.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Event_Rule.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Helpers.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Helpers.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Layer_Create.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Layer_Create.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Layers_OSBot.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Layers_OSBot.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Package.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Package.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Lambda_SSH.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Lambda_SSH.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Lambda_SSH_Kubectl.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Lambda_SSH_Kubectl.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Lambda_Upload_Package.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Lambda_Upload_Package.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Parameter.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Parameter.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Rest_API.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Rest_API.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/S3_Zip_From_Files.py` & `osbot_aws-2.9.0/osbot_aws/helpers/S3_Zip_From_Files.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/SQS_Queue.py` & `osbot_aws-2.9.0/osbot_aws/helpers/SQS_Queue.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/Test_Helper.py` & `osbot_aws-2.9.0/osbot_aws/helpers/Test_Helper.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/helpers/VPC.py` & `osbot_aws-2.9.0/osbot_aws/helpers/VPC.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py` & `osbot_aws-2.9.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/lambdas/server_ssh.py` & `osbot_aws-2.9.0/osbot_aws/lambdas/server_ssh.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/testing/TestCase__API_Gateway_V2.py` & `osbot_aws-2.9.0/osbot_aws/testing/TestCase__API_Gateway_V2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/testing/TestCase__Bedrock.py` & `osbot_aws-2.9.0/osbot_aws/testing/TestCase__Bedrock.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/testing/TestCase__Dynamo_DB.py` & `osbot_aws-2.9.0/osbot_aws/testing/TestCase__Dynamo_DB.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/osbot_aws/testing/TestCase__Lambda.py` & `osbot_aws-2.9.0/osbot_aws/testing/TestCase__Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.7.0/pyproject.toml` & `osbot_aws-2.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name        = "osbot_aws"
-version     = "v2.7.0"
+version     = "v2.9.0"
 description = "OWASP Security Bot - AWS"
 authors     = ["Dinis Cruz <dinis.cruz@owasp.org>"]
 license     = "MIT"
 readme      = "README.md"
 homepage    = "https://github.com/owasp-sbot/OSBot-AWS"
 repository  = "https://github.com/owasp-sbot/OSBot-AWS"
```

### Comparing `osbot_aws-2.7.0/PKG-INFO` & `osbot_aws-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osbot_aws
-Version: 2.7.0
+Version: 2.9.0
 Summary: OWASP Security Bot - AWS
 Home-page: https://github.com/owasp-sbot/OSBot-AWS
 License: MIT
 Author: Dinis Cruz
 Author-email: dinis.cruz@owasp.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Project-URL: Repository, https://github.com/owasp-sbot/OSBot-AWS
 Description-Content-Type: text/markdown
 
 # OSBot-AWS
 
-![Current Release](https://img.shields.io/badge/release-v2.7.0-blue)
+![Current Release](https://img.shields.io/badge/release-v2.9.0-blue)
 
 Large number of AWS apis and utils from the OWASP Security Bot (OSBot) which make
 the use of AWS's boto3 library easier and more intuitive.
 
 ## Current version is 2.x.x 
 
 This version has a number of breaking changes, mainly on the location of the apis,
```

