# Comparing `tmp/aws-arn-0.0.8.tar.gz` & `tmp/aws-arn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-arn-0.0.8.tar", last modified: Tue May  9 22:10:14 2023, max compression
+gzip compressed data, was "aws-arn-0.0.9.tar", last modified: Wed May 17 07:35:26 2023, max compression
```

## Comparing `aws-arn-0.0.8.tar` & `aws-arn-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-05-09 22:10:14.925357 aws-arn-0.0.8/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-05-09 22:10:14.925223 aws-arn-0.0.8/PKG-INFO
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)   100906 2023-05-09 22:09:25.000000 aws-arn-0.0.8/README.md
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-05-09 22:10:14.924231 aws-arn-0.0.8/aws_arn/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)     5781 2023-05-09 22:10:03.000000 aws-arn-0.0.8/aws_arn/__init__.py
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)   178790 2023-05-09 22:08:51.000000 aws-arn-0.0.8/aws_arn/data.py
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)     4230 2023-05-09 16:42:56.000000 aws-arn-0.0.8/aws_arn/get_parser.py
--rwxr-xr-x   0 gabrielsoltz   (501) staff       (20)     1796 2023-05-09 22:10:03.000000 aws-arn-0.0.8/aws_arn/main.py
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-05-09 22:10:14.925052 aws-arn-0.0.8/aws_arn.egg-info/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-05-09 22:10:14.000000 aws-arn-0.0.8/aws_arn.egg-info/PKG-INFO
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      250 2023-05-09 22:10:14.000000 aws-arn-0.0.8/aws_arn.egg-info/SOURCES.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)        1 2023-05-09 22:10:14.000000 aws-arn-0.0.8/aws_arn.egg-info/dependency_links.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)       41 2023-05-09 22:10:14.000000 aws-arn-0.0.8/aws_arn.egg-info/entry_points.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)        8 2023-05-09 22:10:14.000000 aws-arn-0.0.8/aws_arn.egg-info/top_level.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)       38 2023-05-09 22:10:14.925400 aws-arn-0.0.8/setup.cfg
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      731 2023-05-09 22:10:03.000000 aws-arn-0.0.8/setup.py
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-05-17 07:35:26.739904 aws-arn-0.0.9/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-05-17 07:35:26.739766 aws-arn-0.0.9/PKG-INFO
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)   101618 2023-05-17 07:34:58.000000 aws-arn-0.0.9/README.md
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-05-17 07:35:26.738911 aws-arn-0.0.9/aws_arn/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)     5781 2023-05-09 22:18:19.000000 aws-arn-0.0.9/aws_arn/__init__.py
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)   178790 2023-05-14 02:01:38.000000 aws-arn-0.0.9/aws_arn/data.py
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)     4230 2023-05-09 16:42:56.000000 aws-arn-0.0.9/aws_arn/get_parser.py
+-rwxr-xr-x   0 gabrielsoltz   (501) staff       (20)     1796 2023-05-09 22:10:03.000000 aws-arn-0.0.9/aws_arn/main.py
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-05-17 07:35:26.739593 aws-arn-0.0.9/aws_arn.egg-info/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-05-17 07:35:26.000000 aws-arn-0.0.9/aws_arn.egg-info/PKG-INFO
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      250 2023-05-17 07:35:26.000000 aws-arn-0.0.9/aws_arn.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)        1 2023-05-17 07:35:26.000000 aws-arn-0.0.9/aws_arn.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)       41 2023-05-17 07:35:26.000000 aws-arn-0.0.9/aws_arn.egg-info/entry_points.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)        8 2023-05-17 07:35:26.000000 aws-arn-0.0.9/aws_arn.egg-info/top_level.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)       38 2023-05-17 07:35:26.739941 aws-arn-0.0.9/setup.cfg
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      767 2023-05-17 07:35:18.000000 aws-arn-0.0.9/setup.py
```

### Comparing `aws-arn-0.0.8/README.md` & `aws-arn-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 # aws-arn
-A complete list of all AWS ARNs
+A complete list of all AWS ARNs with their respective Cloudformation, Terraform and ASFF resource names.
 
-Isn't anyoning trying to guess the ARN for a specific AWS resource? This is a complete list of all AWS ARNs. The list is sorted alphabetically by service and resource.  This is the only complete list of AWS ARNs available anywhere.
+This is a complete list of all AWS ARNs. The list is sorted alphabetically by service and resource. This is the only complete list of AWS ARNs available anywhere.
 
-> :warning: **Work in progress**: This is a work in progress.  Not all services and resources are included yet.  Please open an issue or pull request if you find any errors or omissions.
+This is also a python module and CLI to generate ARNs for any AWS resource by passing in the resource ID, region and partition.
+
+You can use this repository as documentation, or you can use it as a module or CLI to generate ARNs for any AWS resource.
+
+> :warning: **Work in progress**: This is a work in progress. Not all services and resources are included yet. Please open an issue or pull request if you find any errors or omissions.
 
 - Total number of services:  153
 - Total number of resources:  468
 
 See the full list of ARNs [here](#full-list-of-arns).
 
 # Features
 
 - Generate ARNs for any AWS resource by passing in the resource ID, region and partition
-    - Using service and resoruce name
-    - Using Terraform resource name
-    - Using Cloudformation resource name
-- Get the ASFF Resource Name for any AWS resource (e.g. `AwsCertificateManagerCertificate`)
-- Get the Cloudformation Resource Name for any AWS resource (e.g. `AWS::CertificateManager::Certificate`)
-- Get the Terraform Resource Name for any AWS resource (e.g. `aws_acm_certificate`)
+    - Using service and resoruce name (e.g. `acm` and `certificate`)
+    - Using Terraform resource name (e.g. `aws_acm_certificate`)
+    - Using Cloudformation resource name (e.g. `AWS::CertificateManager::Certificate`)
+- Get the ASFF Resource Name for any AWS resource
+- Get the Cloudformation Resource Name for any AWS resource
+- Get the Terraform Resource Name for any AWS resource
+
+# To do
+
+- [ ] Code quality
+- [ ] From an ARN: get the service, resource name, terraform resource name, cloudformation resource name and ASFF resource name
+- [ ] From an ASFF resource name: get the service, resource name, terraform resource name, cloudformation resource name and ARN
+- [ ] Provide a block of terraform or cloudformation block and generate the ARN for it
+
 
 # Contributing to this list
 
 ARNs are defined under [aws_arn/data.py](aws_arn/data.py). 
 
 Format:
 
@@ -37,14 +49,16 @@
             "terraform": "aws_acm_certificate",  --> The Terraform Resource Name
         }
     },
 ```
 
 # Use it as a module
 
+`pip3 install aws-arn`
+
 ## Generate ARN using service and resource name
 
 ```
 import aws_arn
 
 arn = aws_arn.generate_arn('i-1234568901', 'ec2', 'instance', 'us-east-1', '012345789012', 'aws')
 
@@ -69,14 +83,17 @@
 print (arn)
 
 arn:aws:ec2:us-east-1:012345789012:instance/i-1234568901
 ```
 
 # Use it as CLI
 
+`git clone git@github.com:gabrielsoltz/aws-arn.git`
+`./aws-arn --help`
+
 ## Generate ARN using service and resource name
 ```
 ./aws-arn --generate-arn --id test --service ec2 --sub-service instance --region us-east-1 --account 012345789012 --partition aws
 
 arn:aws:ec2:us-east-1:012345789012:instance/test
 ```
 
@@ -127,16 +144,16 @@
 | appstream | directory_config | `arn:{partition}:appstream:{region}:{account}:directoryconfig/{resource_id}` | DirectoryConfigName | `[a-zA-Z0-9-]+` |  | AWS::AppStream::DirectoryConfig | aws_appstream_directory_config |
 | appstream | fleet | `arn:{partition}:appstream:{region}:{account}:fleet/{resource_id}` | FleetName | `[a-zA-Z0-9-]+` |  | AWS::AppStream::Fleet | aws_appstream_fleet |
 | appstream | image | `arn:{partition}:appstream:{region}:{account}:image/{resource_id}` | ImageName | `[a-zA-Z0-9-]+` |  | AWS::AppStream::Image | aws_appstream_image |
 | appstream | image_builder | `arn:{partition}:appstream:{region}:{account}:imagebuilder/{resource_id}` | ImageBuilderName | `[a-zA-Z0-9-]+` |  | AWS::AppStream::ImageBuilder | aws_appstream_image_builder |
 | appstream | stack | `arn:{partition}:appstream:{region}:{account}:stack/{resource_id}` | StackName | `[a-zA-Z0-9-]+` |  | AWS::AppStream::Stack | aws_appstream_stack |
 | athena | workgroup | `arn:{partition}:athena:{region}:{account}:workgroup/{resource_id}` | WorkGroupName | `([a-zA-Z0-9._-]+)` |  | AWS::Athena::WorkGroup | aws_athena_workgroup |
 | augmentedairuntime | human_loop | `arn:{partition}:sagemaker:{region}:{account}:human-loop/{resource_id}` | HumanLoopName | `^[a-zA-Z0-9](-*[a-zA-Z0-9])*` |  | AWS::SageMaker::HumanTaskUi | aws_sagemaker_human_task_ui |
-| autoscaling | auto_scaling_group | `arn:{partition}:autoscaling:{region}:{account}:autoScalingGroup:{resource_id}` | AutoScalingGroupName | `[a-zA-Z0-9-]{1,255}` | AwsAutoScalingAutoScalingGroup | AWS::AutoScaling::AutoScalingGroup | aws_autoscaling_group |
-| autoscaling | launch_configuration | `arn:{partition}:autoscaling:{region}:{account}:launchConfiguration:{resource_id}` | LaunchConfigurationName | `[a-zA-Z0-9-]{1,255}` | AwsAutoScalingLaunchConfiguration | AWS::AutoScaling::LaunchConfiguration | aws_launch_configuration |
+| autoscaling | auto_scaling_group | `arn:{partition}:autoscaling:{region}:{account}:autoScalingGroup/{resource_id}` | AutoScalingGroupName | `[a-zA-Z0-9-]{1,255}` | AwsAutoScalingAutoScalingGroup | AWS::AutoScaling::AutoScalingGroup | aws_autoscaling_group |
+| autoscaling | launch_configuration | `arn:{partition}:autoscaling:{region}:{account}:launchConfiguration/{resource_id}` | LaunchConfigurationName | `[a-zA-Z0-9-]{1,255}` | AwsAutoScalingLaunchConfiguration | AWS::AutoScaling::LaunchConfiguration | aws_launch_configuration |
 | backup | backup_plan | `arn:{partition}:backup:{region}:{account}:backup-plan/{resource_id}` | BackupPlanId | `^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$` | AwsBackupBackupPlan | AWS::Backup::BackupPlan | aws_backup_plan |
 | backup | backup_vault | `arn:{partition}:backup:{region}:{account}:backup-vault/{resource_id}` | BackupVaultName | `^[a-zA-Z0-9_-]{1,50}$` | AwsBackupBackupVault | AWS::Backup::BackupVault | aws_backup_vault |
 | backup | recovery_plan | `arn:{partition}:backup:{region}:{account}:recoveryplan/{resource_id}` | RecoveryPlanName | `^[a-zA-Z0-9\-\_\.]+$` | AwsBackupRecoveryPoint | AWS::Backup::RecoveryPlan | aws_backup_recovery_point |
 | batch | compute_environment | `arn:{partition}:batch:{region}:{account}:compute-environment/{resource_id}` | ComputeEnvironmentName | `[a-zA-Z0-9_-]+` |  | AWS::Batch::ComputeEnvironment | aws_batch_compute_environment |
 | batch | job_definition | `arn:{partition}:batch:{region}:{account}:job-definition/{resource_id}:{version}` | JobDefinitionName | `[a-zA-Z0-9_-]+` |  | AWS::Batch::JobDefinition | aws_batch_job_definition |
 | batch | job_queue | `arn:{partition}:batch:{region}:{account}:job-queue/{resource_id}` | JobQueueName | `[a-zA-Z0-9_-]+` |  | AWS::Batch::JobQueue | aws_batch_job_queue |
 | budgets | budget | `arn:{partition}:budgets:{region}:{account}:budget/{resource_id}` | BudgetName | `([a-zA-Z0-9-_.]+)` |  | AWS::Budgets::Budget | aws_budgets_budget |
```

### Comparing `aws-arn-0.0.8/aws_arn/__init__.py` & `aws-arn-0.0.9/aws_arn/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.8/aws_arn/data.py` & `aws-arn-0.0.9/aws_arn/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,23 +269,23 @@
             "asff_name": "",
             "cloudformation": "AWS::SageMaker::HumanTaskUi",
             "terraform": "aws_sagemaker_human_task_ui",
         }
     },
     "autoscaling": {
         "auto_scaling_group": {
-            "arn_format": "arn:{partition}:autoscaling:{region}:{account}:autoScalingGroup:{resource_id}",
+            "arn_format": "arn:{partition}:autoscaling:{region}:{account}:autoScalingGroup/{resource_id}",
             "id_name": "AutoScalingGroupName",
             "id_regexp": "[a-zA-Z0-9-]{1,255}",
             "asff_name": "AwsAutoScalingAutoScalingGroup",
             "cloudformation": "AWS::AutoScaling::AutoScalingGroup",
             "terraform": "aws_autoscaling_group",
         },
         "launch_configuration": {
-            "arn_format": "arn:{partition}:autoscaling:{region}:{account}:launchConfiguration:{resource_id}",
+            "arn_format": "arn:{partition}:autoscaling:{region}:{account}:launchConfiguration/{resource_id}",
             "id_name": "LaunchConfigurationName",
             "id_regexp": "[a-zA-Z0-9-]{1,255}",
             "asff_name": "AwsAutoScalingLaunchConfiguration",
             "cloudformation": "AWS::AutoScaling::LaunchConfiguration",
             "terraform": "aws_launch_configuration",
         },
     },
```

### Comparing `aws-arn-0.0.8/aws_arn/get_parser.py` & `aws-arn-0.0.9/aws_arn/get_parser.py`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.8/aws_arn/main.py` & `aws-arn-0.0.9/aws_arn/main.py`

 * *Files identical despite different names*

