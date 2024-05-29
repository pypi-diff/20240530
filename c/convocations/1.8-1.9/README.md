# Comparing `tmp/convocations-1.8.tar.gz` & `tmp/convocations-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convocations-1.8.tar", last modified: Mon Oct 16 22:30:31 2023, max compression
+gzip compressed data, was "convocations-1.9.tar", last modified: Sat Dec  2 06:42:50 2023, max compression
```

## Comparing `convocations-1.8.tar` & `convocations-1.9.tar`

### file list

```diff
@@ -1,200 +1,202 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.243326 convocations-1.8/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      436 2023-10-12 05:30:45.000000 convocations-1.8/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5502 2023-10-16 22:30:31.243326 convocations-1.8/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4082 2023-10-16 22:26:41.000000 convocations-1.8/README.md
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       14 2023-02-22 06:26:46.000000 convocations-1.8/airflow.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       50 2023-02-22 06:26:46.000000 convocations-1.8/aws.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       58 2023-10-16 22:24:37.000000 convocations-1.8/azure.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2023-02-22 06:26:46.000000 convocations-1.8/certs.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       92 2023-02-22 06:26:46.000000 convocations-1.8/checkpoint.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.203326 convocations-1.8/convocations/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.8/convocations/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.203326 convocations-1.8/convocations/airflow/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     8238 2023-06-24 15:59:13.000000 convocations-1.8/convocations/airflow/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.203326 convocations-1.8/convocations/aws/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2058 2023-08-30 21:27:16.000000 convocations-1.8/convocations/aws/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     8555 2023-09-03 03:07:12.000000 convocations-1.8/convocations/aws/ami_helpers.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    20449 2023-03-19 19:56:34.000000 convocations-1.8/convocations/aws/base.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/cfn/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/cfn/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5507 2023-03-13 15:35:55.000000 convocations-1.8/convocations/aws/cfn/import_code_pipeline.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     9133 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/cfn/import_ecs_service.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3476 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/cfn/import_instance.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4209 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/cfn/import_resource_to_cfn.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1666 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/cfn/import_route_table.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4473 2023-06-28 04:50:20.000000 convocations-1.8/convocations/aws/cfn/import_security_group.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4011 2023-07-25 17:58:11.000000 convocations-1.8/convocations/aws/cfn/import_subnet.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2519 2023-03-13 15:35:55.000000 convocations-1.8/convocations/aws/cfn/import_vpc.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    24439 2023-07-29 00:11:12.000000 convocations-1.8/convocations/aws/cfn/stack_commands.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/cloudwatch/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      788 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/cloudwatch/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/codeartifact/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3471 2023-08-16 05:00:44.000000 convocations-1.8/convocations/aws/codeartifact/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/codebuild/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      615 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/codebuild/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    13433 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/codebuild/build.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      168 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/codebuild/detect.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/codedeploy/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3332 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/codedeploy/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/ec2/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    14029 2023-09-02 19:40:54.000000 convocations-1.8/convocations/aws/ec2/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      327 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/ec2/detect.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3546 2023-09-30 22:13:35.000000 convocations-1.8/convocations/aws/ec2/networking.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1673 2023-03-13 15:35:55.000000 convocations-1.8/convocations/aws/ec2/routing.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5784 2023-06-27 04:14:01.000000 convocations-1.8/convocations/aws/ec2/ssh.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/ecs/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2091 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/ecs/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/efs/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1573 2023-08-19 18:59:46.000000 convocations-1.8/convocations/aws/efs/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/elb/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     8604 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/elb/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/health/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      432 2023-05-12 14:51:21.000000 convocations-1.8/convocations/aws/health/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/iam/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2005 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/iam/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      798 2023-03-19 19:56:34.000000 convocations-1.8/convocations/aws/ip_ranges.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4487 2023-03-13 15:35:55.000000 convocations-1.8/convocations/aws/keypairs.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/mgn/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       40 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/mgn/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2138 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/mgn/launch.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/open_id/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      657 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/open_id/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/organizations/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     8604 2023-03-13 15:35:55.000000 convocations-1.8/convocations/aws/organizations/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/ram/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1311 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/ram/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/rds/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     7131 2023-08-16 05:01:33.000000 convocations-1.8/convocations/aws/rds/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/reservations/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    13764 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/reservations/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/route53/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      949 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/route53/__init__.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3704 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/route53/zone_parser.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/s3/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1978 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/s3/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/ssm/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/ssm/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3217 2023-08-20 00:24:56.000000 convocations-1.8/convocations/aws/ssm/runners.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/transit_gateway/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5828 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/transit_gateway/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.213326 convocations-1.8/convocations/aws/vpc_peering/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      615 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/vpc_peering/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      560 2023-02-22 06:26:46.000000 convocations-1.8/convocations/aws/wait_helpers.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.223326 convocations-1.8/convocations/azure/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      520 2023-10-16 20:21:41.000000 convocations-1.8/convocations/azure/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2153 2023-10-16 22:28:56.000000 convocations-1.8/convocations/azure/application_tasks.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1582 2023-10-16 22:27:31.000000 convocations-1.8/convocations/azure/base.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3813 2023-10-16 22:27:49.000000 convocations-1.8/convocations/azure/group_tasks.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2868 2023-10-12 05:32:02.000000 convocations-1.8/convocations/azure/ldap_tasks.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2364 2023-10-12 02:29:24.000000 convocations-1.8/convocations/azure/resource_group_tasks.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      626 2023-10-12 01:44:40.000000 convocations-1.8/convocations/azure/subscription_tasks.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.223326 convocations-1.8/convocations/base/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.8/convocations/base/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1739 2023-02-22 06:26:46.000000 convocations-1.8/convocations/base/projects.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     6956 2023-10-16 16:18:28.000000 convocations-1.8/convocations/base/utils.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.223326 convocations-1.8/convocations/certs/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      191 2023-09-18 20:49:36.000000 convocations-1.8/convocations/certs/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2253 2023-10-12 05:31:53.000000 convocations-1.8/convocations/certs/ed25519.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2678 2023-02-22 06:26:46.000000 convocations-1.8/convocations/certs/validator.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.223326 convocations-1.8/convocations/checkpoint/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      310 2023-02-22 06:26:46.000000 convocations-1.8/convocations/checkpoint/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1082 2023-02-22 06:26:46.000000 convocations-1.8/convocations/checkpoint/base.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      507 2023-02-22 06:26:46.000000 convocations-1.8/convocations/checkpoint/layers.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      648 2023-02-22 06:26:46.000000 convocations-1.8/convocations/checkpoint/objects.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2859 2023-02-22 06:26:46.000000 convocations-1.8/convocations/checkpoint/services.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      433 2023-02-22 06:26:46.000000 convocations-1.8/convocations/checkpoint/versions.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.223326 convocations-1.8/convocations/docker/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      139 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1021 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/template.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.243326 convocations-1.8/convocations/docker/templates/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      188 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/.bumpversion.cfg
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/.dockerignore
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       22 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/.gitignore
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       52 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/Dockerfile
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      364 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/Makefile
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      146 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/README.md
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      696 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/buildspec.yml
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       17 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/requirements.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.223326 convocations-1.8/convocations/docker/templates/tasks/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      134 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/tasks/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2245 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/tasks/build.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2023-02-22 06:26:46.000000 convocations-1.8/convocations/docker/templates/version.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.223326 convocations-1.8/convocations/o365/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.8/convocations/o365/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1032 2023-02-22 06:26:46.000000 convocations-1.8/convocations/o365/imap.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.223326 convocations-1.8/convocations/onelogin/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      124 2023-02-22 06:26:46.000000 convocations-1.8/convocations/onelogin/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      718 2023-02-22 06:26:46.000000 convocations-1.8/convocations/onelogin/base.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1094 2023-02-22 06:26:46.000000 convocations-1.8/convocations/onelogin/users.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.223326 convocations-1.8/convocations/palo_alto/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      380 2023-03-13 15:35:55.000000 convocations-1.8/convocations/palo_alto/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     6079 2023-03-13 15:35:55.000000 convocations-1.8/convocations/palo_alto/base.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4721 2023-03-13 15:35:55.000000 convocations-1.8/convocations/palo_alto/certificates.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1918 2023-03-13 15:35:55.000000 convocations-1.8/convocations/palo_alto/save_config.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3055 2023-03-13 15:35:55.000000 convocations-1.8/convocations/palo_alto/upgrade.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1546 2023-03-13 15:35:55.000000 convocations-1.8/convocations/palo_alto/weird.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/pypi/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1744 2023-03-19 20:21:23.000000 convocations-1.8/convocations/pypi/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      182 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/program.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.243326 convocations-1.8/convocations/pypi/templates/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      198 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/.bumpversion.cfg
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       22 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/.coveragerc
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       66 2023-03-19 20:21:36.000000 convocations-1.8/convocations/pypi/templates/.flake8
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1176 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/.gitignore
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    21589 2023-03-19 20:22:17.000000 convocations-1.8/convocations/pypi/templates/.pylintrc
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       86 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      896 2023-03-19 20:20:39.000000 convocations-1.8/convocations/pypi/templates/Makefile
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      582 2023-03-19 20:16:59.000000 convocations-1.8/convocations/pypi/templates/README.md
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/pypi/templates/conf/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        4 2023-03-19 20:05:33.000000 convocations-1.8/convocations/pypi/templates/conf/convocations.yml
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       87 2023-03-19 20:19:36.000000 convocations-1.8/convocations/pypi/templates/dev.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       66 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/pytest.ini
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       11 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/requirements.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/pypi/templates/sesame_meow_cat/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/sesame_meow_cat/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/sesame_meow_cat/version.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2390 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/setup.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/pypi/templates/tasks/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      297 2023-03-19 20:05:33.000000 convocations-1.8/convocations/pypi/templates/tasks/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/pypi/templates/test/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/test/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       16 2023-02-22 06:26:46.000000 convocations-1.8/convocations/pypi/templates/test/conftest.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/python/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      195 2023-02-22 06:26:46.000000 convocations-1.8/convocations/python/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1529 2023-02-22 06:26:46.000000 convocations-1.8/convocations/python/pytest.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2562 2023-02-22 06:26:46.000000 convocations-1.8/convocations/python/setup.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/sharepoint/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      319 2023-02-22 06:26:46.000000 convocations-1.8/convocations/sharepoint/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1413 2023-02-22 06:26:46.000000 convocations-1.8/convocations/sharepoint/files.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4138 2023-02-22 06:26:46.000000 convocations-1.8/convocations/sharepoint/permissions.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/snobby/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1978 2023-03-13 15:36:01.000000 convocations-1.8/convocations/snobby/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/tundra/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      495 2023-03-19 19:56:34.000000 convocations-1.8/convocations/tundra/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5404 2023-03-19 19:56:34.000000 convocations-1.8/convocations/tundra/codebuild.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3439 2023-03-13 15:35:55.000000 convocations-1.8/convocations/tundra/deploy.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1952 2023-02-22 06:26:46.000000 convocations-1.8/convocations/tundra/docker.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1792 2023-02-22 06:26:46.000000 convocations-1.8/convocations/tundra/ecs.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      640 2023-02-22 06:26:46.000000 convocations-1.8/convocations/tundra/frontend.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1014 2023-02-22 06:26:46.000000 convocations-1.8/convocations/tundra/template.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations/tundra/templates/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      316 2023-02-22 06:26:46.000000 convocations-1.8/convocations/tundra/templates/Makefile
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       79 2023-02-22 06:26:46.000000 convocations-1.8/convocations/tundra/templates/README.md
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4930 2023-02-22 06:26:46.000000 convocations-1.8/convocations/tundra/utils.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1673 2023-02-22 06:26:46.000000 convocations-1.8/convocations/tundra/waiters.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       16 2023-10-16 22:30:19.000000 convocations-1.8/convocations/version.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-10-16 22:30:31.233326 convocations-1.8/convocations.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5502 2023-10-16 22:30:30.000000 convocations-1.8/convocations.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     6315 2023-10-16 22:30:30.000000 convocations-1.8/convocations.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-10-16 22:30:30.000000 convocations-1.8/convocations.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      120 2023-10-16 22:30:30.000000 convocations-1.8/convocations.egg-info/entry_points.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1116 2023-10-16 22:30:30.000000 convocations-1.8/convocations.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2023-10-16 22:30:30.000000 convocations-1.8/convocations.egg-info/top_level.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      239 2023-02-22 06:26:46.000000 convocations-1.8/dev.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        9 2023-02-22 06:26:46.000000 convocations-1.8/onelogin.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       48 2023-02-22 06:26:46.000000 convocations-1.8/palo_alto.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      125 2023-06-24 15:56:02.000000 convocations-1.8/requirements.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2023-10-16 22:30:31.243326 convocations-1.8/setup.cfg
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3254 2023-10-16 22:30:19.000000 convocations-1.8/setup.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       39 2023-02-22 06:26:46.000000 convocations-1.8/sharepoint.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2023-02-22 06:26:46.000000 convocations-1.8/tundra.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.613583 convocations-1.9/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      436 2023-10-12 05:30:45.000000 convocations-1.9/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5502 2023-12-02 06:42:50.613583 convocations-1.9/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4082 2023-10-16 22:26:41.000000 convocations-1.9/README.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       14 2023-02-22 06:26:46.000000 convocations-1.9/airflow.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       50 2023-02-22 06:26:46.000000 convocations-1.9/aws.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       70 2023-10-19 00:41:57.000000 convocations-1.9/azure.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2023-02-22 06:26:46.000000 convocations-1.9/certs.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       92 2023-02-22 06:26:46.000000 convocations-1.9/checkpoint.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.573583 convocations-1.9/convocations/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.9/convocations/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.573583 convocations-1.9/convocations/airflow/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     8238 2023-06-24 15:59:13.000000 convocations-1.9/convocations/airflow/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.573583 convocations-1.9/convocations/aws/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2058 2023-08-30 21:27:16.000000 convocations-1.9/convocations/aws/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     8555 2023-09-03 03:07:12.000000 convocations-1.9/convocations/aws/ami_helpers.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    20449 2023-03-19 19:56:34.000000 convocations-1.9/convocations/aws/base.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.573583 convocations-1.9/convocations/aws/cfn/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/cfn/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5507 2023-03-13 15:35:55.000000 convocations-1.9/convocations/aws/cfn/import_code_pipeline.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     9133 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/cfn/import_ecs_service.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3476 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/cfn/import_instance.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4209 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/cfn/import_resource_to_cfn.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1666 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/cfn/import_route_table.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4473 2023-06-28 04:50:20.000000 convocations-1.9/convocations/aws/cfn/import_security_group.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4011 2023-07-25 17:58:11.000000 convocations-1.9/convocations/aws/cfn/import_subnet.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2519 2023-03-13 15:35:55.000000 convocations-1.9/convocations/aws/cfn/import_vpc.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    24439 2023-07-29 00:11:12.000000 convocations-1.9/convocations/aws/cfn/stack_commands.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.573583 convocations-1.9/convocations/aws/cloudwatch/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      788 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/cloudwatch/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.573583 convocations-1.9/convocations/aws/codeartifact/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3471 2023-08-16 05:00:44.000000 convocations-1.9/convocations/aws/codeartifact/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/codebuild/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      615 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/codebuild/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    13433 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/codebuild/build.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      168 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/codebuild/detect.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/codedeploy/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3332 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/codedeploy/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/ec2/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    14029 2023-09-02 19:40:54.000000 convocations-1.9/convocations/aws/ec2/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      327 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/ec2/detect.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3546 2023-09-30 22:13:35.000000 convocations-1.9/convocations/aws/ec2/networking.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1673 2023-03-13 15:35:55.000000 convocations-1.9/convocations/aws/ec2/routing.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5784 2023-06-27 04:14:01.000000 convocations-1.9/convocations/aws/ec2/ssh.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/ecs/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2091 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/ecs/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/efs/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1573 2023-08-19 18:59:46.000000 convocations-1.9/convocations/aws/efs/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/elb/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     8604 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/elb/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/health/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      432 2023-05-12 14:51:21.000000 convocations-1.9/convocations/aws/health/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/iam/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2005 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/iam/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      798 2023-03-19 19:56:34.000000 convocations-1.9/convocations/aws/ip_ranges.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4487 2023-03-13 15:35:55.000000 convocations-1.9/convocations/aws/keypairs.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/mgn/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       40 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/mgn/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2138 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/mgn/launch.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/open_id/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      657 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/open_id/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/organizations/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     8604 2023-03-13 15:35:55.000000 convocations-1.9/convocations/aws/organizations/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/ram/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1311 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/ram/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/rds/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     7131 2023-08-16 05:01:33.000000 convocations-1.9/convocations/aws/rds/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/reservations/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    13764 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/reservations/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/route53/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      949 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/route53/__init__.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3704 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/route53/zone_parser.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/s3/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1978 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/s3/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/ssm/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/ssm/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3217 2023-08-20 00:24:56.000000 convocations-1.9/convocations/aws/ssm/runners.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/transit_gateway/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5828 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/transit_gateway/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/aws/vpc_peering/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      615 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/vpc_peering/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      560 2023-02-22 06:26:46.000000 convocations-1.9/convocations/aws/wait_helpers.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.583583 convocations-1.9/convocations/azure/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      520 2023-10-16 20:21:41.000000 convocations-1.9/convocations/azure/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2153 2023-10-16 22:28:56.000000 convocations-1.9/convocations/azure/application_tasks.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1699 2023-10-27 03:11:09.000000 convocations-1.9/convocations/azure/base.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3813 2023-10-16 22:27:49.000000 convocations-1.9/convocations/azure/group_tasks.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2868 2023-10-12 05:32:02.000000 convocations-1.9/convocations/azure/ldap_tasks.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2364 2023-10-12 02:29:24.000000 convocations-1.9/convocations/azure/resource_group_tasks.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      626 2023-10-12 01:44:40.000000 convocations-1.9/convocations/azure/subscription_tasks.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.593583 convocations-1.9/convocations/base/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.9/convocations/base/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1739 2023-02-22 06:26:46.000000 convocations-1.9/convocations/base/projects.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     8655 2023-12-02 06:39:22.000000 convocations-1.9/convocations/base/utils.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.593583 convocations-1.9/convocations/certs/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      296 2023-10-19 05:48:37.000000 convocations-1.9/convocations/certs/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2232 2023-10-19 20:57:53.000000 convocations-1.9/convocations/certs/ecdsa.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2253 2023-10-12 05:31:53.000000 convocations-1.9/convocations/certs/ed25519.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2678 2023-02-22 06:26:46.000000 convocations-1.9/convocations/certs/validator.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.593583 convocations-1.9/convocations/checkpoint/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      310 2023-02-22 06:26:46.000000 convocations-1.9/convocations/checkpoint/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1082 2023-02-22 06:26:46.000000 convocations-1.9/convocations/checkpoint/base.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      507 2023-02-22 06:26:46.000000 convocations-1.9/convocations/checkpoint/layers.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      648 2023-02-22 06:26:46.000000 convocations-1.9/convocations/checkpoint/objects.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2859 2023-02-22 06:26:46.000000 convocations-1.9/convocations/checkpoint/services.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      433 2023-02-22 06:26:46.000000 convocations-1.9/convocations/checkpoint/versions.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.593583 convocations-1.9/convocations/docker/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      139 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1021 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/template.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.613583 convocations-1.9/convocations/docker/templates/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      188 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/.bumpversion.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/.dockerignore
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       22 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/.gitignore
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       52 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/Dockerfile
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      364 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/Makefile
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      146 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/README.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      696 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/buildspec.yml
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       17 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/requirements.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.593583 convocations-1.9/convocations/docker/templates/tasks/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      134 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/tasks/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2245 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/tasks/build.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2023-02-22 06:26:46.000000 convocations-1.9/convocations/docker/templates/version.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.593583 convocations-1.9/convocations/o365/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.9/convocations/o365/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1032 2023-02-22 06:26:46.000000 convocations-1.9/convocations/o365/imap.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.593583 convocations-1.9/convocations/onelogin/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      124 2023-02-22 06:26:46.000000 convocations-1.9/convocations/onelogin/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      718 2023-02-22 06:26:46.000000 convocations-1.9/convocations/onelogin/base.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1094 2023-02-22 06:26:46.000000 convocations-1.9/convocations/onelogin/users.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.593583 convocations-1.9/convocations/palo_alto/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      380 2023-03-13 15:35:55.000000 convocations-1.9/convocations/palo_alto/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     6079 2023-03-13 15:35:55.000000 convocations-1.9/convocations/palo_alto/base.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5267 2023-12-02 06:28:46.000000 convocations-1.9/convocations/palo_alto/certificates.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1918 2023-03-13 15:35:55.000000 convocations-1.9/convocations/palo_alto/save_config.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3055 2023-03-13 15:35:55.000000 convocations-1.9/convocations/palo_alto/upgrade.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1546 2023-03-13 15:35:55.000000 convocations-1.9/convocations/palo_alto/weird.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.593583 convocations-1.9/convocations/pypi/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1744 2023-03-19 20:21:23.000000 convocations-1.9/convocations/pypi/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      182 2023-02-22 06:26:46.000000 convocations-1.9/convocations/pypi/program.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.613583 convocations-1.9/convocations/pypi/templates/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      230 2023-10-27 01:44:29.000000 convocations-1.9/convocations/pypi/templates/.bumpversion.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       22 2023-02-22 06:26:46.000000 convocations-1.9/convocations/pypi/templates/.coveragerc
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       66 2023-03-19 20:21:36.000000 convocations-1.9/convocations/pypi/templates/.flake8
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1176 2023-02-22 06:26:46.000000 convocations-1.9/convocations/pypi/templates/.gitignore
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    21589 2023-03-19 20:22:17.000000 convocations-1.9/convocations/pypi/templates/.pylintrc
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      582 2023-03-19 20:16:59.000000 convocations-1.9/convocations/pypi/templates/CONTRIBUTING.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       86 2023-02-22 06:26:46.000000 convocations-1.9/convocations/pypi/templates/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1476 2023-11-01 14:11:18.000000 convocations-1.9/convocations/pypi/templates/Makefile
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       67 2023-10-22 17:43:10.000000 convocations-1.9/convocations/pypi/templates/README.md
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.603583 convocations-1.9/convocations/pypi/templates/conf/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        4 2023-03-19 20:05:33.000000 convocations-1.9/convocations/pypi/templates/conf/convocations.yml
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       98 2023-10-22 17:41:31.000000 convocations-1.9/convocations/pypi/templates/dev.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       66 2023-02-22 06:26:46.000000 convocations-1.9/convocations/pypi/templates/pytest.ini
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       11 2023-02-22 06:26:46.000000 convocations-1.9/convocations/pypi/templates/requirements.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.603583 convocations-1.9/convocations/pypi/templates/sesame_meow_cat/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.9/convocations/pypi/templates/sesame_meow_cat/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       17 2023-10-27 01:44:56.000000 convocations-1.9/convocations/pypi/templates/sesame_meow_cat/version_info.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2323 2023-10-27 01:44:14.000000 convocations-1.9/convocations/pypi/templates/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.603583 convocations-1.9/convocations/pypi/templates/tasks/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      297 2023-03-19 20:05:33.000000 convocations-1.9/convocations/pypi/templates/tasks/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.603583 convocations-1.9/convocations/pypi/templates/test/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 convocations-1.9/convocations/pypi/templates/test/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       16 2023-02-22 06:26:46.000000 convocations-1.9/convocations/pypi/templates/test/conftest.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.603583 convocations-1.9/convocations/python/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      195 2023-02-22 06:26:46.000000 convocations-1.9/convocations/python/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1529 2023-02-22 06:26:46.000000 convocations-1.9/convocations/python/pytest.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2562 2023-02-22 06:26:46.000000 convocations-1.9/convocations/python/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.603583 convocations-1.9/convocations/sharepoint/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      319 2023-02-22 06:26:46.000000 convocations-1.9/convocations/sharepoint/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1413 2023-02-22 06:26:46.000000 convocations-1.9/convocations/sharepoint/files.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4138 2023-02-22 06:26:46.000000 convocations-1.9/convocations/sharepoint/permissions.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.603583 convocations-1.9/convocations/snobby/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1978 2023-03-13 15:36:01.000000 convocations-1.9/convocations/snobby/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.603583 convocations-1.9/convocations/tundra/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      495 2023-03-19 19:56:34.000000 convocations-1.9/convocations/tundra/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5404 2023-03-19 19:56:34.000000 convocations-1.9/convocations/tundra/codebuild.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3439 2023-03-13 15:35:55.000000 convocations-1.9/convocations/tundra/deploy.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1952 2023-02-22 06:26:46.000000 convocations-1.9/convocations/tundra/docker.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1792 2023-02-22 06:26:46.000000 convocations-1.9/convocations/tundra/ecs.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      640 2023-02-22 06:26:46.000000 convocations-1.9/convocations/tundra/frontend.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1014 2023-02-22 06:26:46.000000 convocations-1.9/convocations/tundra/template.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.603583 convocations-1.9/convocations/tundra/templates/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      316 2023-02-22 06:26:46.000000 convocations-1.9/convocations/tundra/templates/Makefile
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       79 2023-02-22 06:26:46.000000 convocations-1.9/convocations/tundra/templates/README.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4930 2023-02-22 06:26:46.000000 convocations-1.9/convocations/tundra/utils.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1673 2023-02-22 06:26:46.000000 convocations-1.9/convocations/tundra/waiters.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       16 2023-12-02 06:42:38.000000 convocations-1.9/convocations/version.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-12-02 06:42:50.613583 convocations-1.9/convocations.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5502 2023-12-02 06:42:50.000000 convocations-1.9/convocations.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     6443 2023-12-02 06:42:50.000000 convocations-1.9/convocations.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-12-02 06:42:50.000000 convocations-1.9/convocations.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      120 2023-12-02 06:42:50.000000 convocations-1.9/convocations.egg-info/entry_points.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1133 2023-12-02 06:42:50.000000 convocations-1.9/convocations.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2023-12-02 06:42:50.000000 convocations-1.9/convocations.egg-info/top_level.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      239 2023-02-22 06:26:46.000000 convocations-1.9/dev.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        9 2023-02-22 06:26:46.000000 convocations-1.9/onelogin.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       51 2023-12-02 06:28:40.000000 convocations-1.9/palo_alto.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      125 2023-06-24 15:56:02.000000 convocations-1.9/requirements.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2023-12-02 06:42:50.613583 convocations-1.9/setup.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3254 2023-12-02 06:42:38.000000 convocations-1.9/setup.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       39 2023-02-22 06:26:46.000000 convocations-1.9/sharepoint.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2023-02-22 06:26:46.000000 convocations-1.9/tundra.txt
```

### Comparing `convocations-1.8/PKG-INFO` & `convocations-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convocations
-Version: 1.8
+Version: 1.9
 Summary: convocations
 Home-page: https://github.com/crazy-penguins/convocations
 Author: 2ps
 Author-email: pshingavi@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `convocations-1.8/README.md` & `convocations-1.9/README.md`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/airflow/__init__.py` & `convocations-1.9/convocations/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/__init__.py` & `convocations-1.9/convocations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/ami_helpers.py` & `convocations-1.9/convocations/aws/ami_helpers.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/base.py` & `convocations-1.9/convocations/aws/base.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cfn/import_code_pipeline.py` & `convocations-1.9/convocations/aws/cfn/import_code_pipeline.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cfn/import_ecs_service.py` & `convocations-1.9/convocations/aws/cfn/import_ecs_service.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cfn/import_instance.py` & `convocations-1.9/convocations/aws/cfn/import_instance.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cfn/import_resource_to_cfn.py` & `convocations-1.9/convocations/aws/cfn/import_resource_to_cfn.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cfn/import_route_table.py` & `convocations-1.9/convocations/aws/cfn/import_route_table.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cfn/import_security_group.py` & `convocations-1.9/convocations/aws/cfn/import_security_group.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cfn/import_subnet.py` & `convocations-1.9/convocations/aws/cfn/import_subnet.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cfn/import_vpc.py` & `convocations-1.9/convocations/aws/cfn/import_vpc.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cfn/stack_commands.py` & `convocations-1.9/convocations/aws/cfn/stack_commands.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/cloudwatch/__init__.py` & `convocations-1.9/convocations/aws/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/codeartifact/__init__.py` & `convocations-1.9/convocations/aws/codeartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/codebuild/__init__.py` & `convocations-1.9/convocations/aws/codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/codebuild/build.py` & `convocations-1.9/convocations/aws/codebuild/build.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/codedeploy/__init__.py` & `convocations-1.9/convocations/aws/codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/ec2/__init__.py` & `convocations-1.9/convocations/aws/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/ec2/networking.py` & `convocations-1.9/convocations/aws/ec2/networking.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/ec2/routing.py` & `convocations-1.9/convocations/aws/ec2/routing.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/ec2/ssh.py` & `convocations-1.9/convocations/aws/ec2/ssh.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/ecs/__init__.py` & `convocations-1.9/convocations/aws/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/efs/__init__.py` & `convocations-1.9/convocations/aws/efs/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/elb/__init__.py` & `convocations-1.9/convocations/aws/elb/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/iam/__init__.py` & `convocations-1.9/convocations/aws/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/ip_ranges.py` & `convocations-1.9/convocations/aws/ip_ranges.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/keypairs.py` & `convocations-1.9/convocations/aws/keypairs.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/mgn/launch.py` & `convocations-1.9/convocations/aws/mgn/launch.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/open_id/__init__.py` & `convocations-1.9/convocations/aws/open_id/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/organizations/__init__.py` & `convocations-1.9/convocations/aws/organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/ram/__init__.py` & `convocations-1.9/convocations/aws/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/rds/__init__.py` & `convocations-1.9/convocations/aws/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/reservations/__init__.py` & `convocations-1.9/convocations/aws/reservations/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/route53/__init__.py` & `convocations-1.9/convocations/aws/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/route53/zone_parser.py` & `convocations-1.9/convocations/aws/route53/zone_parser.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/s3/__init__.py` & `convocations-1.9/convocations/aws/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/ssm/runners.py` & `convocations-1.9/convocations/aws/ssm/runners.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/transit_gateway/__init__.py` & `convocations-1.9/convocations/aws/transit_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/vpc_peering/__init__.py` & `convocations-1.9/convocations/aws/vpc_peering/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/aws/wait_helpers.py` & `convocations-1.9/convocations/aws/wait_helpers.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/azure/__init__.py` & `convocations-1.9/convocations/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/azure/application_tasks.py` & `convocations-1.9/convocations/azure/application_tasks.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/azure/base.py` & `convocations-1.9/convocations/azure/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from time import time
 from raft.tasks import Task
 from raft.context import Context
+import requests
+from requests.adapters import HTTPAdapter
+from urllib3.util.retry import Retry
 
 
 class AzureTask(Task):
     def __call__(self, *args, **kwargs):
         from azure.identity import ClientSecretCredential
         from azure.identity import InteractiveBrowserCredential
         from azure.identity import TokenCachePersistenceOptions
```

### Comparing `convocations-1.8/convocations/azure/group_tasks.py` & `convocations-1.9/convocations/azure/group_tasks.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/azure/ldap_tasks.py` & `convocations-1.9/convocations/azure/ldap_tasks.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/azure/resource_group_tasks.py` & `convocations-1.9/convocations/azure/resource_group_tasks.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/azure/subscription_tasks.py` & `convocations-1.9/convocations/azure/subscription_tasks.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/base/projects.py` & `convocations-1.9/convocations/base/projects.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/base/utils.py` & `convocations-1.9/convocations/base/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -94,64 +94,105 @@
         cprint(st, color, **kwargs)
     elif st is False:
         flush_print('\N{wilted flower}')
     else:
         flush_print('\N{cherry blossom}')
 
 
-def to_string(value: Any) -> str:
+def to_string(value: Any, format_floats=True) -> str:
     """
     used by the `print_table` function, this function converts
     a value to a string making sure to format decimal.Decimal and float values
     to 2 decimal places
     :param Any value: the message that will be provided to the user
+    :param bool format_floats: if specified as True, values will be formatted
+                               nicely with commas and 2 decimal places
     :return: the string representation of value
     :rtype: str
     """
-    if isinstance(value, (float, Decimal)):
-        return f'{value:,.2f}'
-    return f'{value}'
+    if isinstance(value, (float, Decimal)) and format_floats:
+        st = f'{value:,.2f}'
+    else:
+        st = f'{value}'
+    if '\n' in st:
+        st = st.split('\n')
+    return st
 
 
-def print_table(header, rows, color='cyan'):
+def print_table(
+        header,
+        rows,
+        color='cyan',
+        wrap_newline=False,
+        format_floats=True,
+        **kwargs):
     """
     prints a header and rows in a tabular format in the specified color.
     this function is useful for presenting summary information from aws
     commands in a tabular format
     :param list[str] header: a list of strings for the table header
     :param list[Iterable[Any]] rows: a list of list of values to present
     :param str color: the color in which we will print our table
+    :param bool wrap_newline: if true, values with new lines in them
+                              will be wrapped at '\n'
+    :param bool format_floats: if true, floats and Decimals will be
+                               formatted numerically
     """
     max_lens = [ 0 ] * len(header)
-    rows = [ [ to_string(x) for x in row ] for row in rows ]
+    rows = [ [ to_string(x, format_floats) for x in row ] for row in rows ]
     for row in chain([ header ], rows):
         for i, x in enumerate(row):
-            max_lens[i] = max(max_lens[i], len(x))
+            if isinstance(x, list):
+                local_max = max([ len(lx) for lx in x ])
+                max_lens[i] = max(max_lens[i], local_max)
+            else:
+                max_lens[i] = max(max_lens[i], len(x))
     f_header = []
     for width, x in zip(max_lens, header):
         diff = len(x)
         x = colored(x, color)
         diff = len(x) - diff
         f = f'%-{width + diff}s'
         f = f % (x,)
         f_header.append(f)
     print(' | '.join(f_header))
     print(' | '.join([ colored('-' * width, color) for width in max_lens ]))
-    for row in rows:
-        f_row = []
-        for n, (width, x) in enumerate(zip(max_lens, row)):
-            diff = 0
-            if n == 0:
-                diff = len(x)
-                x = colored(x, color)
-                diff = len(x) - diff
-            f = f'%-{width + diff}s'
-            f = f % (x,)
-            f_row.append(f)
-        print(' | '.join(f_row))
+    if wrap_newline:
+        for row in rows:
+            max_height = max([ len(x) if isinstance(x, list) else 1 for x in row ])
+            for h in range(max_height):
+                f_row = []
+                for n, (width, x) in enumerate(zip(max_lens, row)):
+                    diff = 0
+                    value = ' '
+                    if isinstance(x, list) and h < len(x):
+                        value = x[h]
+                    elif h == 0 and not isinstance(x, list):
+                        value = x
+                    if n == 0:
+                        diff = len(value)
+                        value = colored(value, color)
+                        diff = len(value) - diff
+                    f = f'%-{width + diff}s'
+                    f = f % (value,)
+                    f_row.append(f)
+                print(' | '.join(f_row))
+    else:
+        for row in rows:
+            f_row = []
+            for n, (width, x) in enumerate(zip(max_lens, row)):
+                diff = 0
+                if n == 0:
+                    diff = len(x)
+                    x = colored(x, color)
+                    diff = len(x) - diff
+                f = f'%-{width + diff}s'
+                f = f % (x,)
+                f_row.append(f)
+            print(' | '.join(f_row))
 
 
 def confirm(message: str) -> bool:
     """
     presents the user with a confirmation message to which the user should
     respond with a YES / NO response
     :param message: the confirmation prompt
```

### Comparing `convocations-1.8/convocations/certs/ed25519.py` & `convocations-1.9/convocations/certs/ed25519.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/certs/validator.py` & `convocations-1.9/convocations/certs/validator.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/checkpoint/base.py` & `convocations-1.9/convocations/checkpoint/base.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/checkpoint/objects.py` & `convocations-1.9/convocations/checkpoint/objects.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/checkpoint/services.py` & `convocations-1.9/convocations/checkpoint/services.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/docker/template.py` & `convocations-1.9/convocations/docker/template.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/docker/templates/buildspec.yml` & `convocations-1.9/convocations/docker/templates/buildspec.yml`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/docker/templates/tasks/build.py` & `convocations-1.9/convocations/docker/templates/tasks/build.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/o365/imap.py` & `convocations-1.9/convocations/o365/imap.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/onelogin/base.py` & `convocations-1.9/convocations/onelogin/base.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/onelogin/users.py` & `convocations-1.9/convocations/onelogin/users.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/palo_alto/base.py` & `convocations-1.9/convocations/palo_alto/base.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/palo_alto/certificates.py` & `convocations-1.9/convocations/palo_alto/certificates.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,30 +33,46 @@
 def install_pfx(ctx, pfx, pfx_password=None,
                 host=None, username=None, password=None,
                 profile=None, **kwargs):
     """
     installs a cert to the firewall
     """
     from lxml import etree
-    from OpenSSL.crypto import load_pkcs12
+    from cryptography.hazmat.primitives.serialization.pkcs12 import (
+        load_pkcs12, serialize_key_and_certificates
+    )
+    from cryptography.hazmat.primitives.serialization import (
+        BestAvailableEncryption
+    )
+    from cryptography.hazmat.backends import default_backend
     api = XmlApi(host, username, password, profile=profile, **kwargs)
     session = kwargs['session']
     if pfx.startswith('s3://'):
         p12_data = load_from_s3(session, pfx)
     else:
         p12_data = load_file(pfx)
         if not p12_data:
             return
 
-    p12 = load_pkcs12(p12_data, pfx_password)
+    password_bytes = None
+    if pfx_password:
+        password_bytes = pfx_password.encode('utf8')
+    p12 = load_pkcs12(p12_data, password_bytes, default_backend())
     if not pfx_password:
         pfx_password = uuid4().hex.encode('utf-8')[:30]
-        p12_data = p12.export(pfx_password)
-    name = p12.get_certificate().get_subject()
-    name = name.get_components()[0][-1].decode('utf-8')
+        en = BestAvailableEncryption(pfx_password)
+        p12_data = serialize_key_and_certificates(
+            None,
+            p12.key,
+            p12.cert.certificate,
+            p12.additional_certs,
+            en
+        )
+    name = p12.cert.certificate.subject.rfc4514_string()
+    name = name.split('=', 1)[-1]
     notice(f'importing to {host}')
     response = api.import_pfx(name, p12_data, pfx_password)
     success = response.attrib['status'] == 'success'
     notice_end(success)
     if not success:
         print(etree.tostring(response, pretty_print=True).decode())
     else:
```

### Comparing `convocations-1.8/convocations/palo_alto/save_config.py` & `convocations-1.9/convocations/palo_alto/save_config.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/palo_alto/upgrade.py` & `convocations-1.9/convocations/palo_alto/upgrade.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/palo_alto/weird.py` & `convocations-1.9/convocations/palo_alto/weird.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/pypi/__init__.py` & `convocations-1.9/convocations/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/pypi/templates/.gitignore` & `convocations-1.9/convocations/pypi/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/pypi/templates/.pylintrc` & `convocations-1.9/convocations/pypi/templates/.pylintrc`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/pypi/templates/README.md` & `convocations-1.9/convocations/pypi/templates/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/pypi/templates/setup.py` & `convocations-1.9/convocations/pypi/templates/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # Support setuptools only, distutils has a divergent and more annoying API and
 # few folks will lack setuptools.
 from setuptools import setup
 from importlib.resources import open_text
 # Version info -- read without importing
 _locals = {}
 
-version = open_text('{{ name }}', 'version.txt').read().strip()
-
 # PyYAML ships a split Python 2/3 codebase. Unfortunately, some pip versions
 # attempt to interpret both halves of PyYAML, yielding SyntaxErrors. Thus, we
 # exclude whichever appears inappropriate for the installing interpreter.
 exclude = ["*.yaml2", 'test']
 
 # Frankenstein long_description: version-specific changelog note + README
 with open('README.md') as f:
@@ -32,15 +30,15 @@
     all_extras = list(all_extras)
     all_extras.sort()
     extras['all'] = all_extras
 
 
 setup(
     name='{{ name }}',
-    version=version,
+    version='0.0',
     description='{{ name }}',
     license='BSD',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='dev',
     author_email='developers@directbuy.com',
     url='https://bitbucket.org/dbuy/{{ name }}',
```

### Comparing `convocations-1.8/convocations/python/pytest.py` & `convocations-1.9/convocations/python/pytest.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/python/setup.py` & `convocations-1.9/convocations/python/setup.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/sharepoint/files.py` & `convocations-1.9/convocations/sharepoint/files.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/sharepoint/permissions.py` & `convocations-1.9/convocations/sharepoint/permissions.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/snobby/__init__.py` & `convocations-1.9/convocations/snobby/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/tundra/codebuild.py` & `convocations-1.9/convocations/tundra/codebuild.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/tundra/deploy.py` & `convocations-1.9/convocations/tundra/deploy.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/tundra/docker.py` & `convocations-1.9/convocations/tundra/docker.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/tundra/ecs.py` & `convocations-1.9/convocations/tundra/ecs.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/tundra/frontend.py` & `convocations-1.9/convocations/tundra/frontend.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/tundra/template.py` & `convocations-1.9/convocations/tundra/template.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/tundra/utils.py` & `convocations-1.9/convocations/tundra/utils.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations/tundra/waiters.py` & `convocations-1.9/convocations/tundra/waiters.py`

 * *Files identical despite different names*

### Comparing `convocations-1.8/convocations.egg-info/PKG-INFO` & `convocations-1.9/convocations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convocations
-Version: 1.8
+Version: 1.9
 Summary: convocations
 Home-page: https://github.com/crazy-penguins/convocations
 Author: 2ps
 Author-email: pshingavi@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `convocations-1.8/convocations.egg-info/SOURCES.txt` & `convocations-1.9/convocations.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 ./convocations/azure/ldap_tasks.py
 ./convocations/azure/resource_group_tasks.py
 ./convocations/azure/subscription_tasks.py
 ./convocations/base/__init__.py
 ./convocations/base/projects.py
 ./convocations/base/utils.py
 ./convocations/certs/__init__.py
+./convocations/certs/ecdsa.py
 ./convocations/certs/ed25519.py
 ./convocations/certs/validator.py
 ./convocations/checkpoint/__init__.py
 ./convocations/checkpoint/base.py
 ./convocations/checkpoint/layers.py
 ./convocations/checkpoint/objects.py
 ./convocations/checkpoint/services.py
@@ -99,24 +100,25 @@
 ./convocations/palo_alto/base.py
 ./convocations/palo_alto/certificates.py
 ./convocations/palo_alto/save_config.py
 ./convocations/palo_alto/upgrade.py
 ./convocations/palo_alto/weird.py
 ./convocations/pypi/__init__.py
 ./convocations/pypi/program.py
+./convocations/pypi/templates/CONTRIBUTING.md
 ./convocations/pypi/templates/MANIFEST.in
 ./convocations/pypi/templates/Makefile
 ./convocations/pypi/templates/README.md
 ./convocations/pypi/templates/dev.txt
 ./convocations/pypi/templates/pytest.ini
 ./convocations/pypi/templates/requirements.txt
 ./convocations/pypi/templates/setup.py
 ./convocations/pypi/templates/conf/convocations.yml
 ./convocations/pypi/templates/sesame_meow_cat/__init__.py
-./convocations/pypi/templates/sesame_meow_cat/version.txt
+./convocations/pypi/templates/sesame_meow_cat/version_info.py
 ./convocations/pypi/templates/tasks/__init__.py
 ./convocations/pypi/templates/test/__init__.py
 ./convocations/pypi/templates/test/conftest.py
 ./convocations/python/__init__.py
 ./convocations/python/pytest.py
 ./convocations/python/setup.py
 ./convocations/sharepoint/__init__.py
@@ -152,22 +154,23 @@
 convocations/docker/templates/tasks/__init__.py
 convocations/docker/templates/tasks/build.py
 convocations/pypi/templates/.bumpversion.cfg
 convocations/pypi/templates/.coveragerc
 convocations/pypi/templates/.flake8
 convocations/pypi/templates/.gitignore
 convocations/pypi/templates/.pylintrc
+convocations/pypi/templates/CONTRIBUTING.md
 convocations/pypi/templates/MANIFEST.in
 convocations/pypi/templates/Makefile
 convocations/pypi/templates/README.md
 convocations/pypi/templates/dev.txt
 convocations/pypi/templates/pytest.ini
 convocations/pypi/templates/requirements.txt
 convocations/pypi/templates/setup.py
 convocations/pypi/templates/conf/convocations.yml
 convocations/pypi/templates/sesame_meow_cat/__init__.py
-convocations/pypi/templates/sesame_meow_cat/version.txt
+convocations/pypi/templates/sesame_meow_cat/version_info.py
 convocations/pypi/templates/tasks/__init__.py
 convocations/pypi/templates/test/__init__.py
 convocations/pypi/templates/test/conftest.py
 convocations/tundra/templates/Makefile
 convocations/tundra/templates/README.md
```

### Comparing `convocations-1.8/convocations.egg-info/requires.txt` & `convocations-1.9/convocations.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 azure-mgmt-resource
 boto3
 botocore
 cp-mgmt-api-sdk@ git+https://github.com/CheckPointSW/cp_mgmt_api_python_sdk@v1.5.0
 cryptography
 lxml
 msal
+msgraph-sdk
 office365-rest-python-client
 onelogin
 openpyxl
 pan-os-python
 pan-python
 pandas
 pwinput
 pygobject
-pyopenssl
 redis
 ruamel.yaml
 urllib3
 
 [aws]
 awscli
 botocore
@@ -48,14 +48,15 @@
 openpyxl
 
 [azure]
 azure-mgmt-resource
 azure-identity
 cryptography
 pygobject
+msgraph-sdk
 
 [certs]
 cryptography
 
 [checkpoint]
 pwinput
 cp-mgmt-api-sdk@ git+https://github.com/CheckPointSW/cp_mgmt_api_python_sdk@v1.5.0
@@ -80,15 +81,15 @@
 
 [onelogin]
 onelogin
 
 [palo_alto]
 urllib3
 lxml
-pyopenssl
+cryptography
 pan-os-python
 pan-python
 
 [sharepoint]
 msal
 office365-rest-python-client
 adal
```

### Comparing `convocations-1.8/setup.py` & `convocations-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Support setuptools only, distutils has a divergent and more annoying API and
 # few folks will lack setuptools.
 from setuptools import setup, find_packages
 from importlib.resources import open_text
 # Version info -- read without importing
 _locals = {}
 
-version = '1.8'
+version = '1.9'
 
 # PyYAML ships a split Python 2/3 codebase. Unfortunately, some pip versions
 # attempt to interpret both halves of PyYAML, yielding SyntaxErrors. Thus, we
 # exclude whichever appears inappropriate for the installing interpreter.
 exclude = ["*.yaml2", 'test']
 
 # Frankenstein long_description: version-specific changelog note + README
```

