# Comparing `tmp/aws_ecs_deploy-0.1.0.tar.gz` & `tmp/aws_ecs_deploy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ecs_deploy-0.1.0.tar", max compression
+gzip compressed data, was "aws_ecs_deploy-0.1.1.tar", max compression
```

## Comparing `aws_ecs_deploy-0.1.0.tar` & `aws_ecs_deploy-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0    35149 2023-04-26 11:14:40.998333 aws_ecs_deploy-0.1.0/LICENSE
--rw-r--r--   0        0        0      891 2023-04-26 11:15:39.928601 aws_ecs_deploy-0.1.0/README.md
--rw-r--r--   0        0        0       12 2023-04-26 11:15:39.934964 aws_ecs_deploy-0.1.0/aws_deploy/.gitignore
--rw-r--r--   0        0        0        0 2023-04-26 11:15:39.935496 aws_ecs_deploy-0.1.0/aws_deploy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 11:15:39.955066 aws_ecs_deploy-0.1.0/aws_deploy/adminer/__init__.py
--rw-r--r--   0        0        0      373 2023-05-03 16:39:39.040206 aws_ecs_deploy-0.1.0/aws_deploy/adminer/base.py
--rw-r--r--   0        0        0      517 2023-04-30 08:34:17.380785 aws_ecs_deploy-0.1.0/aws_deploy/adminer/commands.py
--rw-r--r--   0        0        0     2367 2023-05-03 16:39:39.040182 aws_ecs_deploy-0.1.0/aws_deploy/adminer/login.py
--rw-r--r--   0        0        0     1516 2023-05-03 16:39:39.040196 aws_ecs_deploy-0.1.0/aws_deploy/adminer/qrcode_generator.py
--rw-r--r--   0        0        0      986 2023-05-03 08:42:11.513390 aws_ecs_deploy-0.1.0/aws_deploy/alb.py
--rw-r--r--   0        0        0      560 2023-05-02 12:08:46.490074 aws_ecs_deploy-0.1.0/aws_deploy/aws_lambda/commands.py
--rw-r--r--   0        0        0     3545 2023-05-05 11:42:34.465814 aws_ecs_deploy-0.1.0/aws_deploy/aws_lambda/create_function.py
--rw-r--r--   0        0        0     1001 2023-05-05 07:48:39.286712 aws_ecs_deploy-0.1.0/aws_deploy/aws_lambda/env_resolver.py
--rw-r--r--   0        0        0      227 2023-04-30 08:35:10.061434 aws_ecs_deploy-0.1.0/aws_deploy/aws_lambda/params.py
--rw-r--r--   0        0        0     2361 2023-05-05 09:27:11.743659 aws_ecs_deploy-0.1.0/aws_deploy/aws_lambda/source_builder.py
--rw-r--r--   0        0        0      957 2023-04-30 10:14:08.091726 aws_ecs_deploy-0.1.0/aws_deploy/cli_common.py
--rw-r--r--   0        0        0     3338 2023-05-05 09:38:10.282494 aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/param_resolver.py
--rw-r--r--   0        0        0     2344 2023-05-05 11:15:10.666131 aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/stack.py
--rw-r--r--   0        0        0     6046 2023-05-05 11:15:24.454596 aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/stack_creator.py
--rw-r--r--   0        0        0     7335 2023-05-03 16:39:39.052122 aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/stack_deleter.py
--rw-r--r--   0        0        0     2517 2023-04-30 08:37:16.771144 aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/stack_operation.py
--rw-r--r--   0        0        0     1417 2023-05-03 12:14:15.144613 aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/template.py
--rw-r--r--   0        0        0       20 2023-05-02 09:23:42.825376 aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/template_factory.py
--rw-r--r--   0        0        0      995 2023-04-30 00:18:33.744614 aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/template_parser.py
--rw-r--r--   0        0        0     1532 2023-05-03 16:39:39.040218 aws_ecs_deploy-0.1.0/aws_deploy/codepipeline/invoker.py
--rw-r--r--   0        0        0     3702 2023-05-05 09:36:04.296771 aws_ecs_deploy-0.1.0/aws_deploy/config.py
--rw-r--r--   0        0        0     4678 2023-04-30 08:37:50.074373 aws_ecs_deploy-0.1.0/aws_deploy/ec2_op.py
--rw-r--r--   0        0        0     3583 2023-05-05 11:00:16.927420 aws_ecs_deploy-0.1.0/aws_deploy/main.py
--rw-r--r--   0        0        0     3193 2023-05-03 16:34:23.132669 aws_ecs_deploy-0.1.0/aws_deploy/params/db_password.py
--rw-r--r--   0        0        0     5615 2023-04-30 10:08:13.141603 aws_ecs_deploy-0.1.0/aws_deploy/params/general.py
--rw-r--r--   0        0        0     4781 2023-05-03 16:58:53.451201 aws_ecs_deploy-0.1.0/aws_deploy/params/ssm_stored.py
--rw-r--r--   0        0        0      803 2023-05-05 08:10:18.453802 aws_ecs_deploy-0.1.0/aws_deploy/service.py
--rw-r--r--   0        0        0      761 2023-05-03 16:39:48.269948 aws_ecs_deploy-0.1.0/aws_deploy/utils.py
--rw-r--r--   0        0        0     1049 2023-05-08 14:30:39.913466 aws_ecs_deploy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 aws_ecs_deploy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 11:14:40.998333 aws_ecs_deploy-0.1.1/LICENSE
+-rw-r--r--   0        0        0      891 2023-04-26 11:15:39.928601 aws_ecs_deploy-0.1.1/README.md
+-rw-r--r--   0        0        0       12 2023-04-26 11:15:39.934964 aws_ecs_deploy-0.1.1/aws_deploy/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-26 11:15:39.935496 aws_ecs_deploy-0.1.1/aws_deploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:15:39.955066 aws_ecs_deploy-0.1.1/aws_deploy/adminer/__init__.py
+-rw-r--r--   0        0        0      517 2023-04-30 08:34:17.380785 aws_ecs_deploy-0.1.1/aws_deploy/adminer/commands.py
+-rw-r--r--   0        0        0     2792 2023-05-10 08:30:58.171012 aws_ecs_deploy-0.1.1/aws_deploy/adminer/login.py
+-rw-r--r--   0        0        0     1594 2023-05-10 08:30:58.171180 aws_ecs_deploy-0.1.1/aws_deploy/adminer/qrcode_generator.py
+-rw-r--r--   0        0        0     1092 2023-05-10 08:30:58.171437 aws_ecs_deploy-0.1.1/aws_deploy/alb.py
+-rw-r--r--   0        0        0      560 2023-05-02 12:08:46.490074 aws_ecs_deploy-0.1.1/aws_deploy/aws_lambda/commands.py
+-rw-r--r--   0        0        0     3406 2023-05-10 08:30:58.171809 aws_ecs_deploy-0.1.1/aws_deploy/aws_lambda/create_function.py
+-rw-r--r--   0        0        0     1001 2023-05-05 07:48:39.286712 aws_ecs_deploy-0.1.1/aws_deploy/aws_lambda/env_resolver.py
+-rw-r--r--   0        0        0     2361 2023-05-05 09:27:11.743659 aws_ecs_deploy-0.1.1/aws_deploy/aws_lambda/source_builder.py
+-rw-r--r--   0        0        0      957 2023-05-10 08:30:10.275971 aws_ecs_deploy-0.1.1/aws_deploy/cli_common.py
+-rw-r--r--   0        0        0       49 2023-05-10 08:30:58.171948 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/exceptions.py
+-rw-r--r--   0        0        0      503 2023-05-10 08:30:58.172108 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter/base.py
+-rw-r--r--   0        0        0     3183 2023-05-10 08:30:58.172241 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter/db_password.py
+-rw-r--r--   0        0        0        0 2023-05-10 08:30:58.172271 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter/exceptions.py
+-rw-r--r--   0        0        0     4145 2023-05-10 08:30:58.172707 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter/general.py
+-rw-r--r--   0        0        0     1862 2023-05-10 08:30:58.172826 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter/resolver.py
+-rw-r--r--   0        0        0     4652 2023-05-10 08:30:58.172941 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter/ssm_stored.py
+-rw-r--r--   0        0        0      855 2023-05-10 08:30:58.173046 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter_manager.py
+-rw-r--r--   0        0        0     2040 2023-05-10 08:30:58.173149 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/resource_remover.py
+-rw-r--r--   0        0        0     2386 2023-05-08 16:32:11.720012 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/stack.py
+-rw-r--r--   0        0        0     5966 2023-05-10 08:30:58.173522 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/stack_creator.py
+-rw-r--r--   0        0        0     7496 2023-05-08 14:45:45.069833 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/stack_deleter.py
+-rw-r--r--   0        0        0     1516 2023-05-10 08:30:58.173698 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/template.py
+-rw-r--r--   0        0        0       20 2023-05-02 09:23:42.825376 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/template_factory.py
+-rw-r--r--   0        0        0      995 2023-04-30 00:18:33.744614 aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/template_parser.py
+-rw-r--r--   0        0        0     1437 2023-05-10 08:30:58.173848 aws_ecs_deploy-0.1.1/aws_deploy/codepipeline/invoker.py
+-rw-r--r--   0        0        0     3861 2023-05-10 08:30:58.173992 aws_ecs_deploy-0.1.1/aws_deploy/config.py
+-rw-r--r--   0        0        0     4570 2023-05-10 08:30:58.174444 aws_ecs_deploy-0.1.1/aws_deploy/ec2_op.py
+-rw-r--r--   0        0        0     3497 2023-05-10 08:30:58.174648 aws_ecs_deploy-0.1.1/aws_deploy/main.py
+-rw-r--r--   0        0        0      803 2023-05-05 08:10:18.453802 aws_ecs_deploy-0.1.1/aws_deploy/service.py
+-rw-r--r--   0        0        0      638 2023-05-08 16:37:51.054091 aws_ecs_deploy-0.1.1/aws_deploy/utils.py
+-rw-r--r--   0        0        0     1077 2023-05-10 08:30:58.175743 aws_ecs_deploy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 aws_ecs_deploy-0.1.1/PKG-INFO
```

### Comparing `aws_ecs_deploy-0.1.0/LICENSE` & `aws_ecs_deploy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_ecs_deploy-0.1.0/README.md` & `aws_ecs_deploy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/adminer/commands.py` & `aws_ecs_deploy-0.1.1/aws_deploy/adminer/commands.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/adminer/login.py` & `aws_ecs_deploy-0.1.1/aws_deploy/adminer/login.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,50 @@
-import os
+
 
 import pyotp
+from rich.prompt import Prompt
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from webdriver_manager.chrome import ChromeDriverManager
 
-from aws_deploy.adminer.base import AdminerBase
 from aws_deploy.adminer.qrcode_generator import OtpQrCodeGenerator
+from aws_deploy.cloudformation.parameter.db_password import DBPassword
+from aws_deploy.cloudformation.template import CloudformationTemplate
+from aws_deploy.config import (Config, ServiceTemplateNotFound, ServiceType,
+                               console)
 from aws_deploy.utils import db_host
-from aws_deploy.config import Config, console
-from aws_deploy.params.db_password import DBPassword
 
 
-class LoginAdminer(AdminerBase):
-    def __init__(self, service_name: str) -> None:
+class LoginAdminer:
+    def __init__(self, short_name: str) -> None:
         self.driver = self._driver()
-        self.service_name = service_name
+        self.template = CloudformationTemplate.from_short_name(short_name)
+        self.config = Config()
 
     def _driver(self) -> webdriver.Chrome:
-
-        driver_path = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), 'chromedriver')
         return webdriver.Chrome(ChromeDriverManager().install())
 
     def fill_host(self):
         db_host_ele = self.driver.find_element(By.NAME, 'auth[server]')
         db_host_ele.clear()
         db_host_ele.send_keys(db_host())
 
     def fill_username(self):
-        username = 'root' if 'rds' in self.service_name else f'{self.service_name}user'
+        if self.template.service.Type == ServiceType.CORE:
+            username = 'root'
+        else:
+            username = f'{self.template.service.Name}user'
+
         self.driver.find_element(By.ID, 'username').send_keys(username)
 
     def fill_password(self):
-        param = DBPasswordParameter(f'{self.service_name}-pipeline', '')
-        fetched_param = param.get_parameter(param.ssm_param_name())
+        param = DBPassword(self.template)
+        ssm_param_name = param.ssm_param_name()
+
+        fetched_param = param.ssm_stored.get_parameter(ssm_param_name)
         self.driver.find_element(By.NAME, 'auth[password]').send_keys(
             fetched_param['Value'])  # type: ignore
 
     def fill_otp(self):
         totp = pyotp.TOTP(OtpQrCodeGenerator().base32secret())
         self.driver.find_element(By.NAME, 'auth[otp]').send_keys(totp.now())
 
@@ -48,20 +54,27 @@
 
     def login(self):
         # import subprocess
         # list_files = subprocess.run(["ssh", "ashraful@192.241.250.137",
         #                              "-p", "5151"], shell=True)
 
         # exit()
+        try:
+            service = self.config.find_service('adminer')
+        except ServiceTemplateNotFound:
+            console.log(
+                "[red]Add adminer service in config/{}.yml[/red]".format(self.config.ENV))  # noqa: E501
+            exit(1)
         self.driver.get(
-            "https://{}".format(config.services['adminer-pipeline'].ServiceUrl))  # type: ignore
+            "https://{}".format(service.ServiceUrl))  # type: ignore
         self.fill_host()
         self.fill_username()
         self.fill_password()
         self.fill_otp()
         self.submit_form()
 
         while True:
-            console.log('Type "done" and press Enter to exit...')
-            if input() == "done":
-                return
+            user_input = Prompt.ask('Type "done" and press Enter to exit...')
+            if user_input.strip() == "done":
+                break
+
         # driver.close()
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/adminer/qrcode_generator.py` & `aws_ecs_deploy-0.1.1/aws_deploy/adminer/qrcode_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import base64
 
 import qrcode
 
-from aws_deploy.adminer.base import AdminerBase
-from aws_deploy.utils import db_host
+from aws_deploy.cloudformation.parameter.ssm_stored import GeneratedSecret
+from aws_deploy.cloudformation.template import CloudformationTemplate
 from aws_deploy.config import Config
-from aws_deploy.params.ssm_stored import GeneratedSecret
 
 
-class OtpQrCodeGenerator(AdminerBase):
+class OtpQrCodeGenerator:
 
     def base32secret(self):
         """Return base32 encoded otp secret
 -
-        Fetches base64 encoded otp secret string. 
-        Coverts it to base32 and returns converted 
+        Fetches base64 encoded otp secret string.
+        Coverts it to base32 and returns converted
         base32 in ascii string format
 
         Returns:
-            str: base32 encoded otp secret 
+            str: base32 encoded otp secret
         """
-        ssm_param_name = GeneratedSecret(
-            'adminer-pipeline', 'OtpSecretStore').ssm_param_name()
-        ssm_param = self.get_parameter(ssm_param_name)
+        template = CloudformationTemplate.from_short_name('adminer')
+        param = GeneratedSecret(
+            template)
+        ssm_param_name = param.ssm_param_name('OtpSecretStore')
+        ssm_param = param.ssm_stored.get_parameter(ssm_param_name)
         # 'P2kib4vBUpZf5A=='
         base64_bytes: str = ssm_param['Value']  # type: ignore
         secret_bytes = base64.b64decode(base64_bytes, validate=True)
         base32_bytes = base64.b32encode(secret_bytes)
         return base32_bytes.decode('ascii')
 
     def qr_data(self, otp_secret: str) -> str:
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/alb.py` & `aws_ecs_deploy-0.1.1/aws_deploy/alb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import boto3
 
 from aws_deploy.cli_common import common_params
 from aws_deploy.config import Config, console
 
 
+@common_params
 def priority_list():
     client = boto3.client('elbv2')
     lbs = client.describe_load_balancers()
     lb_arn = ''
     for lb in lbs['LoadBalancers']:
-        if lb['LoadBalancerName'] == f"{config.ENV}-ALB":
+        if lb['LoadBalancerName'] == f"{Config().ENV}-ALB":
             lb_arn = lb['LoadBalancerArn']
             break
     listeners = client.describe_listeners(
         LoadBalancerArn=lb_arn)
     listener_arn = None
     for listener in listeners['Listeners']:
         if listener['Port'] == 443:
             listener_arn = listener['ListenerArn']
             break
     if listener_arn:
         rules = client.describe_rules(
             ListenerArn=listener_arn)
         for rule in rules['Rules']:
-            if len(rule['Conditions']) > 0 and rule['Conditions'][0].get('HostHeaderConfig'):
+            if len(rule['Conditions']) > 0 and \
+                    rule['Conditions'][0].get('HostHeaderConfig'):
                 console.log(
-                    f"{rule['Priority']} --> {rule['Conditions'][0]['HostHeaderConfig']['Values']}")
+                    "{} --> {}".format(rule['Priority'], rule['Conditions']
+                                       [0]['HostHeaderConfig']['Values'])
+                )
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/aws_lambda/commands.py` & `aws_ecs_deploy-0.1.1/aws_deploy/aws_lambda/commands.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/aws_lambda/create_function.py` & `aws_ecs_deploy-0.1.1/aws_deploy/aws_lambda/create_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 from mypy_boto3_lambda import LambdaClient
 
 from aws_deploy.aws_lambda.env_resolver import LambdaEnvVarResolver
 # from aws_deploy.aws_lambda.params import LambdaRoleNameParameter
 from aws_deploy.aws_lambda.source_builder import SourceBuilder
 from aws_deploy.cloudformation.stack_creator import StackCreator
 from aws_deploy.config import Config, console
-from aws_deploy.params.general import ParameterResolver
-
-
-class RdsMasterPasswordSSMNameParameter(ParameterResolver):
-    # FIXME
-    pass
 
 
 class CreateLambdaStack(StackCreator):
     def __init__(self, short_name: str) -> None:
         super().__init__(short_name)
 
     def template_f_path(self):
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/aws_lambda/env_resolver.py` & `aws_ecs_deploy-0.1.1/aws_deploy/aws_lambda/env_resolver.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/aws_lambda/source_builder.py` & `aws_ecs_deploy-0.1.1/aws_deploy/aws_lambda/source_builder.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/cli_common.py` & `aws_ecs_deploy-0.1.1/aws_deploy/cli_common.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/stack.py` & `aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/stack.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,35 +13,36 @@
 ]
 
 
 @dataclass
 class OutputData:
     OutputKey: str
     OutputValue: str
-    Description: str
-    ExportName: Optional[str]
+    Description: Optional[str] = None
+    ExportName: Optional[str] = None
 
 
 @dataclass
 class CloudformationStack:
     StackId: str
     StackName: str
-    Description: str
+
     Parameters: List[Dict[str, Optional[Union[str, bool]]]]
     CreationTime: datetime
     RollbackConfiguration: Dict[str, Union[List[Dict[str, str]], int]]
     StackStatus: str
     DisableRollback: bool
     NotificationARNs: List[str]
     Capabilities: List[str]
     Outputs: Optional[List[OutputData]]
     Tags: List[Dict[str, str]]
     EnableTerminationProtection: bool
     DriftInformation: Dict[str, Union[str, datetime]]
 
+    Description: Optional[str] = None
     ChangeSetId: Optional[str] = None
     DeletionTime: Optional[datetime] = None
     LastUpdatedTime: Optional[datetime] = None
     StackStatusReason: Optional[str] = None
     TimeoutInMinutes: Optional[int] = None
     RoleARN: Optional[str] = None
     ParentId: Optional[str] = None
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/stack_creator.py` & `aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/stack_creator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import boto3
 from botocore import exceptions
 from mypy_boto3_cloudformation import CloudFormationClient
 
-from aws_deploy.cloudformation.param_resolver import ParameterManager
+from aws_deploy.cloudformation.parameter_manager import ParameterManager
 from aws_deploy.cloudformation.stack import (STACK_FAILED_STATUS_LIST,
                                              CloudformationStack)
 # from aws_deploy.cloudformation.stack_deleter import StackDeleter
 from aws_deploy.cloudformation.template import CloudformationTemplate
 from aws_deploy.config import Config, console
-from aws_deploy.utils import full_stack_name
 
 # def permitted_on(env: str):
 
 #     def gate_decorator(func: Callable):
 #         if config.ENV != env:
 #             console.log(
 #                 f'{func.__name__} is not permitted in {config.ENV}
@@ -30,17 +29,15 @@
     #     self.waiter_status = None
     #     super().__init__(short_name)
     def __init__(self, short_name: str) -> None:
         self.config = Config()
         self.cf: CloudFormationClient = boto3.client(
             'cloudformation', region_name=self.config.REGION)
         self.template = CloudformationTemplate.from_short_name(short_name)
-        self.stack_name = full_stack_name(
-            self.template.service.Type,
-            self.template.service.Name)
+        self.stack_name = self.template.stack_name()
 
     # @permitted_on('dev')
 
     def delete_stack(self, stack_name: str):
         # FIXME
         pass
         # if self.config.ENV == "prod":
@@ -120,15 +117,15 @@
         try:
             resp = self.cf.describe_stacks(StackName=self.stack_name)
 
             # type: ignore
 
             return CloudformationStack.from_dict(  # type : ignore
                 resp['Stacks'][0])  # type : ignore
-        except Exception as e:
+        except self.cf.exceptions.StackNotFoundException as e:
             console.log(e)
             return None
 
     def _stack_failed(self, stack):
         return stack['Stacks'][0]['StackStatus'] in STACK_FAILED_STATUS_LIST
 
     def create(self):
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/stack_deleter.py` & `aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/stack_deleter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Type
 
 import boto3
 from mypy_boto3_cloudformation import CloudFormationClient
 from mypy_boto3_ecr import ECRClient
 
-from aws_deploy.utils import full_stack_name
+from aws_deploy.cloudformation.template import CloudformationTemplate
 from aws_deploy.config import Config, console
 
 deletable_stack_statuses = [
     'CREATE_FAILED',
     'CREATE_COMPLETE',
     'ROLLBACK_COMPLETE',
     'DELETE_FAILED',
@@ -103,15 +103,15 @@
 }
 
 
 class StackDeleter:
     def __init__(self, short_name: str) -> None:
         self.cf: CloudFormationClient = boto3.client('cloudformation')
         self.config = Config()
-        self.name = full_stack_name
+        self.template = CloudformationTemplate.from_short_name(short_name)
 
     def list_stacks(self):
         return self.cf.list_stacks(
             StackStatusFilter=deletable_stack_statuses)['StackSummaries']  # type: ignore # noqa: E501
 
     @staticmethod
     def get_all_resources(env):
@@ -160,19 +160,21 @@
             # print(resource)
             # if resource['LogicalResourceId'] in stack['Stacks'][0]['StackStatusReason']: # noqa: E501
             # this resource is the reason of delete being failed
             deleter_cls = delete_resource_map.get(resource['ResourceType'])
             if deleter_cls:
                 deleter_cls(resource).delete()  # type: ignore
 
-    def delete(self, stack_name: str):
+    def delete(self, stack_name: str | None = None):
         console.log(
             f"[red]Deleting stack: [deep_sky_blue3]{stack_name}[/deep_sky_blue3][/red]")  # noqa: E501
         # console.log(
         #     f"[green]Stack last status: [deep_sky_blue3]{stack_name}[/deep_sky_blue3] [/green] ") # noqa: E501
+        if stack_name is None:
+            stack_name = self.template.stack_name()
         self.delete_stack_resources(stack_name)
         self.cf.delete_stack(StackName=stack_name)
         if not self.config.NO_WAIT:
             waiter = self.cf.get_waiter('stack_delete_complete')
             waiter.wait(StackName=stack_name,
                         WaiterConfig=self.config.waiter_config)  # type: ignore
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/template.py` & `aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     @classmethod
     def from_short_name(cls, short_name: str,
                         service_dir: Optional[str] = None):
         config = Config()
         service = config.find_service(short_name)
         if service_dir is None:
             template_path = os.path.join(
-                service.Type.value, f"{service.Name}.yml")
+                str(service.Type), f"{service.Name}.yml")
         else:
             template_path = os.path.join(service_dir, f"{service.Name}.yml")
         with open(template_path) as f:
             template_body = f.read()
         _content: dict = load_yaml(template_body)
         # TODO: handle keyerror
 
@@ -47,9 +47,12 @@
             _content,
             service,
         )
 
     def add_resource(self, name: str, definition: dict):
         self.content[name] = definition
 
+    def stack_name(self):
+        return f"{Config().ENV}-{self.service.Type}-{self.service.Name}"
+
     def __str__(self) -> str:
         return dump_yaml(self.content)
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/cloudformation/template_parser.py` & `aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/template_parser.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/codepipeline/invoker.py` & `aws_ecs_deploy-0.1.1/aws_deploy/codepipeline/invoker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Literal
-from aws_deploy.utils import full_stack_name
 
 import boto3
 
 
 class CodePipelineInvoker:
     def __init__(self, stack_name: str):
 
@@ -36,11 +35,10 @@
             name: Literal['codepipeline'] = 'codepipeline'
             client = boto3.client(name)
             response = client.start_pipeline_execution(
                 name=pipeline_details['pipelineName'])
             return response
         else:
             return None
-    
+
     def run(self, short_name: str):
-        full_stack_name(
-           'service', short_name)
+        pass
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/config.py` & `aws_ecs_deploy-0.1.1/aws_deploy/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,20 +19,26 @@
 
 # the order of the template core_templates_map is very important.
 # As each core template depends on the previous resource.
 class DeploymentEnv(enum.Enum):
     DEV = 'dev'
     PROD = 'prod'
 
+    def __str__(self):
+        return self.name.lower()
+
 
 class ServiceType(enum.Enum):
     CORE = 'core'
     SERVICE = 'service'
     LAMBDA = 'lambda'
 
+    def __str__(self):
+        return self.name.lower()
+
 
 @dataclass
 class ServiceConfig:
     Name: str
     ShortName: str
     Type: ServiceType
     DesiredCount: Optional[int] = 2
@@ -65,17 +71,17 @@
     CodestarConnectionArn: str = ''
     DBInstanceClass: str = ''
     services: list[ServiceConfig] = field(default_factory=list)
     Ec2DesiredCapacity: int = 1
     Ec2InstanceType: str = 't3.small'
     ContainerEfsMountpoint: str = '/home/ec2-user/efsdata'
 
-    _instance = None
+    # _instance = None
 
-    ENV = DEPLOY_ENV
+    ENV: DeploymentEnv = DeploymentEnv.DEV
     TAG_ENV = TAG_ENV
     REGION = 'us-east-1'
     NO_WAIT: bool = False
     CONFIG_DIR = 'config'
     lambda_python_version = "python:3.9"
     LambdaPythonRuntime = lambda_python_version.replace(":", '')
     waiter_config = {
@@ -106,30 +112,31 @@
         raise ServiceTemplateNotFound
 
     @classmethod
     def from_env(cls, env: DeploymentEnv):
 
         # open(os.path.join(pathlib.Path(__file__).parent.resolve()
         # current directory should have config folder
-        config_path = os.path.join(cls.CONFIG_DIR, f"{env.value}.yml")
+        config_path = os.path.join(cls.CONFIG_DIR, f"{env}.yml")
         yml_config = cls.yml_config(config_path)
         body_keys = [
             'CodestarConnectionArn',
             'DBInstanceClass',
             'Ec2DesiredCapacity',
             'Ec2InstanceType',
             'ContainerEfsMountpoint'
 
         ]
+
         _attrs = {key: val for key, val in yml_config.items()
                   if key in body_keys}
-
+        _attrs['ENV'] = env
         _attrs['services'] = []
         for service_type in ServiceType:
-            for name, service in yml_config[service_type.value].items():
+            for name, service in yml_config[str(service_type)].items():
                 if not service:
                     service = {}
                 if not service.get('ShortName'):
                     service['ShortName'] = name.split("-")[0]
                 service['Type'] = service_type
                 service['Name'] = name
                 _attrs['services'].append(ServiceConfig(**service))
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/ec2_op.py` & `aws_ecs_deploy-0.1.1/aws_deploy/ec2_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 import boto3
 from mypy_boto3_ec2 import EC2Client
 
+from aws_deploy.cloudformation.parameter.general import AllowedIpParameter
 from aws_deploy.config import Config, console
-from aws_deploy.params.general import AllowedIpParameter, ServiceParameter
 
 
 class EcsEc2:
     def __init__(self) -> None:
         self._instances = None
         self.client: EC2Client = boto3.client('ec2')
+        self.config = Config()
 
     @property
     def instances(self):
         if not self._instances:
-            resp = self.client.describe_instances(Filters=[{'Name': 'tag:deployment',
-                                                            'Values': [config.ENV]},
-                                                           {
-                'Name': 'instance-state-name',
-                'Values': ['running']
-            }])
+            resp = self.client.describe_instances(
+                Filters=[{'Name': 'tag:deployment',
+                          'Values': [str(self.config.ENV)]},
+                         {
+                    'Name': 'instance-state-name',
+                    'Values': ['running']
+                }])
             # type:ignore
             self._instances = []
             for group in resp['Reservations']:
-                self._instances.extend(group['Instances'])
+                self._instances.extend(group['Instances'])  # type: ignore
         return self._instances
 
     def ec2_ips(self):
         for ec2 in self.instances:
             console.log(ec2['PublicIpAddress'])  # type: ignore
 
     def ec2_ip(self, service_name: str | None = None) -> str:  # type: ignore
         if not service_name:
             return self.instances[0]['PublicIpAddress']
-        cluster = f'{config.ENV}-ec2'
+        cluster = f'{self.config.ENV}-ec2'
         client = boto3.client('ecs')
         task_arn = client.list_tasks(
             cluster=cluster,
             serviceName=service_name+"-pipeline",
 
         )['taskArns'][0]
         tasks = client.describe_tasks(
             cluster=cluster, tasks=[task_arn])['tasks']
         container_instance_arn = tasks[0]['containerInstanceArn']
-        con_instance = client.describe_container_instances(cluster=cluster,
+        con_instance = client.describe_container_instances(
+            cluster=cluster,
 
-                                                           containerInstances=[
-                                                               container_instance_arn]
-                                                           )['containerInstances'][0]
+            containerInstances=[
+                container_instance_arn]
+        )['containerInstances'][0]
         ec2_instance_id = con_instance['ec2InstanceId']
         for ec2 in self.instances:
             if ec2['InstanceId'] == ec2_instance_id:
                 return ec2['PublicIpAddress']
 
     def ssh_login(self, service_name: str | None = None):
 
@@ -84,36 +87,37 @@
             #     'string',
             # ],
             DryRun=False,
             # NextToken='string',
             MaxResults=123
         )
         return [sg_rule for sg_rule in response['SecurityGroupRules']
-                if sg_rule['IsEgress'] == False]  # type: ignore
+                if sg_rule['IsEgress'] is False]  # type: ignore
 
     def verify_sg_ingress(self, sg_id: str, inbound_rules: list):
-        # pyright: reportTypedDictNotRequiredAccess=false
 
         updatable_rule = None
         for sg_rule in inbound_rules:
             if sg_rule['FromPort'] == 22 and sg_rule['ToPort']:
                 updatable_rule = sg_rule
                 break
-        current_ip = AllowedIpParameter.value()
+        current_ip = AllowedIpParameter.public_ip()+"/32"
         if updatable_rule and updatable_rule['CidrIpv4'] != current_ip:
             allowed_params = ['IpProtocol', 'FromPort', 'ToPort',
-                              'CidrIpv4', 'CidrIpv6', 'PrefixListId', 'ReferencedGroupId']
+                              'CidrIpv4', 'CidrIpv6', 'PrefixListId',
+                              'ReferencedGroupId']
             rule_id = updatable_rule['SecurityGroupRuleId']
 
             updatable_rule = {_key: _val for _key,
-                              _val in updatable_rule.items() if _key in allowed_params}
+                              _val in updatable_rule.items()
+                              if _key in allowed_params}
 
             updatable_rule['CidrIpv4'] = current_ip  # type: ignore
             # updatable_rule['ReferencedGroupId'] = self.sg_id
             sg_rules_list = [{'SecurityGroupRuleId': rule_id,
                               'SecurityGroupRule': updatable_rule
                               }
                              ]
-            response = self.client.modify_security_group_rules(
+            self.client.modify_security_group_rules(
                 GroupId=sg_id,
                 SecurityGroupRules=sg_rules_list)  # type: ignore
             # response
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/main.py` & `aws_ecs_deploy-0.1.1/aws_deploy/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-import importlib
 import logging
-import os
 
 import click
 
 from aws_deploy.adminer.commands import adminer
 from aws_deploy.alb import priority_list
 from aws_deploy.aws_lambda.commands import aws_lambda
 from aws_deploy.cli_common import common_params
 from aws_deploy.cloudformation.stack_creator import StackCreator
 from aws_deploy.cloudformation.stack_deleter import StackDeleter
-from aws_deploy.config import Config, DeploymentEnv
+from aws_deploy.config import console
 
 log = logging.getLogger('deploy.cf.create_or_update')
 
 failed_stack_statuses = [
     'CREATE_FAILED',
     'ROLLBACK_COMPLETE',
     'DELETE_FAILED',
     'UPDATE_FAILED',
     'UPDATE_ROLLBACK_FAILED',
     'ROLLBACK_FAILED'
     # 'UPDATE_ROLLBACK_COMPLETE'
 ]
-deploy_module_name = "deploy"
 
 
 class StdCommand(click.core.Command):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.params.insert(0, click.core.Option(
             ('--env',), help='Override env'))
 
 
 def import_deploy():
     try:
-        importlib.import_module(
-            deploy_module_name, package=None)
+        import deploy  # type: ignore # noqa: F401
 
     except (ImportError, AttributeError) as e:
-        click.echo(f"Failed to load or execute deploy module: {e}")
+        console.log(e)
+        console.log("deploy.py not found on current directory.")
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
-@click.option('--prod', is_flag=True, default=False, help="Executes on production")  # noqa: E501
-@click.option('--no-wait', is_flag=True, default=False, help="Wait for status update to complete")  # noqa: E501
+# @click.option('--prod', is_flag=True, default=False, help="Executes on production")  # noqa: E501
+# @click.option('--no-wait', is_flag=True, default=False, help="Wait for status update to complete")  # noqa: E501
 @click.pass_context
-def cli(ctx: click.core.Context, prod: bool, no_wait: bool):
+def cli(ctx: click.core.Context):
     ctx.ensure_object(dict)
     # env = DeploymentEnv.PROD if prod else DeploymentEnv.DEV
 
     # ctx.obj = Config.from_env(env)
 
     import_deploy()
 # @click.group
@@ -68,33 +65,33 @@
 @cli.command()
 @common_params
 @click.option("-s", "--service-name", help="Full template name without .yml extension")  # noqa: E501
 def delete_stack(service_name: str):
     StackDeleter(service_name).delete()
 
 
-@cli.command()
-@common_params
-@click.option("--services", is_flag=True, default=False, help="Deletes all service stacks")  # noqa: E501
-@click.option("--doit", is_flag=True, default=False, help="Delete all stacks in configured env")  # noqa: E501
-def delete_stacks(services, doit):
-
-    if not doit:
-        return
-    if services:
-        DeleteAllServiceStacks().run()
+# @cli.command()
+# @common_params
+# @click.option("--services", is_flag=True, default=False, help="Deletes all service stacks")  # noqa: E501
+# @click.option("--doit", is_flag=True, default=False, help="Delete all stacks in configured env")  # noqa: E501
+# def delete_stacks(services, doit):
+
+#     if not doit:
+#         return
+#     if services:
+#         DeleteAllServiceStacks().run()
 
 
 @cli.command()
 @common_params
 @click.argument("name")
 @click.option("--recreate", is_flag=True,  default=False, help="Deletes old stack and creates new one")  # noqa: E501
 def create(name: str, recreate: bool):
     if recreate:
-        DeleteSingleStack(name).run()
+        StackDeleter(name).delete()
     StackCreator(name).create()
 
 
 # @cli.command(cls=StdCommand)
 # @common_params
 # # @cli.command()
 # @click.option("-c", "--core", is_flag=True, help="For creating core infrastructure")  # noqa: E501
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/params/db_password.py` & `aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter/db_password.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import time
 
 import boto3
 from mypy_boto3_lambda import LambdaClient
 
 from aws_deploy.cloudformation.template import CloudformationTemplate
 from aws_deploy.config import Config, console
-from aws_deploy.params.general import DbName, DBUserName, ParameterResolver
-from aws_deploy.params.ssm_stored import SSMStored
 
+from .base import ParameterFactoryBase
+from .general import DbName, DBUserName
+from .ssm_stored import SSMStored
 
-class DBPassword(ParameterResolver):
+
+class DBPassword(ParameterFactoryBase):
     def __init__(self, template: CloudformationTemplate):
         super().__init__(template)
         self.ssm_stored = SSMStored()
 
     def ssm_param_name(self) -> str:
         return f"{Config().ENV}-rds-{self.unique_name()}-password"
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/params/general.py` & `aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter/general.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,78 @@
 import fnmatch
 import re
-from abc import ABC, abstractmethod
 
 import boto3
 import requests
 
 from aws_deploy.cloudformation.template import CloudformationTemplate
 from aws_deploy.config import Config, console
 
+from .base import ParameterFactoryBase
 
-class ParameterResolver(ABC):
 
-    def __init__(self, template: CloudformationTemplate):
-        """_summary_
-
-        Args:
-            template (CloudformationTemplate): _description_
-        """
-        self.template = template
-
-    @abstractmethod
-    def resolve(self, parameter_name: str):
-        """
-        Resolve the parameter value.
-        """
-        raise NotImplementedError
-
-
-# class Parameter:
-#     """Base class of all template parameter
-#     """
-
-#     def __init__(self, template: CloudformationTemplate, parameter_key: str):
-#         """_summary_
-
-#         Args:
-#             template (CloudformationTemplate): _description_
-#             parameter_key (str): _description_
-#         """
-#         self.template = template
-#         self.p_key = parameter_key
-
-#     def param_dict(self, param_value: str):
-#         return {
-#             'ParameterKey': self.p_key,
-#             'ParameterValue': param_value,
-#             'UsePreviousValue': False,
-#         }
-
-#     def add_job(self, jobs: list):
-#         pass
-
-#     def value(self):
-#         raise NotImplementedError
-
-#     def add(self, params: list):
-#         """Adds formatted parameter dict to supplied params list
-
-#         Args:
-#             params (list): current parameter list
-#         """
-#         params.append(self.param_dict(self.value()))
-
-#     def update_body(self, template):
-#         """Updated template body if needed. Example: cert arn
-
-#         Args:
-#             template (_type_): _description_
-#         """
-#         pass
-
-
-class ServiceNotFound(Exception):
-    pass
-
-
-class GeneralParameter(ParameterResolver):
+class GeneralParameter(ParameterFactoryBase):
 
     def resolve(self, param_name: str):
         return str(getattr(self.template.service, param_name))
 
 
-class AllowedIpParameter(ParameterResolver):
+class AllowedIpParameter(ParameterFactoryBase):
     @staticmethod
     def is_valid_ip(ip: str):
         import ipaddress
         try:
             ipaddress.ip_address(ip)
             return True
         except ValueError:
             return False
 
-    def resolve(self, param_name: str):
-
+    @staticmethod
+    def public_ip():
         response = requests.get("http://checkip.amazonaws.com")
         ip = response.text.strip()
         console.log('Current public ip: {}'.format(ip))
+        return ip
+
+    def resolve(self, param_name: str):
+
+        ip = self.public_ip()
         if self.is_valid_ip(ip):
             return f"{ip}/32"
         raise Exception(
             '''Couldnt Find valid public id address.
             Check your internet connection''')  # type: ignore
 
 
-class ServiceParameter(ParameterResolver):
+class ServiceParameter(ParameterFactoryBase):
     def resolve(self, param_name: str):
         return self.template.service.Name
 
 
 # class CodebuildProjectNameParameter(TemplateParameter):
 #     def value(self):
 #         return f"{config.ENV}-{self.t_name}-codebuild"
 
 
-class EnvironmentName(ParameterResolver):
+class EnvironmentName(ParameterFactoryBase):
     def resolve(self, param_key: str):
         return Config().ENV
 
 
 # class CodeStarConnectionArnParameter(TemplateParameter):
 #     def value(self):
 #         return config.CODESTAR_CONNECTION_ARN
 
 
-class ConfigConstant(ParameterResolver):
+class ConfigConstant(ParameterFactoryBase):
     def resolve(self, param_key: str):
         return getattr(Config(), param_key)
 
 
-class AlbCertArn(ParameterResolver):
+class AlbCertArn(ParameterFactoryBase):
     def __init__(self, template: CloudformationTemplate):
         self.cert_arns = list()
         self.config = Config()
         super().__init__(template)
 
     @staticmethod
     def certs():
@@ -185,16 +125,16 @@
             return
         main_cert_arn = self.cert_arns.pop(0)
         listener_cert = self.listener_extra_cert_resource()
         self.template.add_resource('ALBExtraCerts', listener_cert)
         return main_cert_arn
 
 
-class DbName(ParameterResolver):
+class DbName(ParameterFactoryBase):
     def resolve(self, param_name: str):
-        name = re.sub('[^A-Za-z0-9]+', '', self.template.name.lower())
+        name = re.sub('[^A-Za-z0-9]+', '', self.template.service.Name.lower())
         return name.replace("pipeline", "")
 
 
 class DBUserName(DbName):
     def resolve(self, param_name: str):
         return f"{super().resolve(param_name)}user"
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/params/ssm_stored.py` & `aws_ecs_deploy-0.1.1/aws_deploy/cloudformation/parameter/ssm_stored.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import secrets
 
 import boto3
 from mypy_boto3_ssm import SSMClient
 
 from aws_deploy.cloudformation.template import CloudformationTemplate
 from aws_deploy.config import Config, console
-from aws_deploy.params.general import ParameterResolver
+
+from .base import ParameterFactoryBase
 
 # r5aFR0s6_OsqGdSrwbJjv2ub-sq3xS2KNBF_iA
 
 
 class SSMStored:
     def __init__(self):
         self.client: SSMClient = boto3.client('ssm')
@@ -46,32 +47,29 @@
             Tags=tags,
             Tier='Standard',
             # Policies='string',
             DataType=data_type,
 
         )
 
-    # def ssm_param_name(self, param_name: str):
-    #     return f"{Config().ENV}-{self.template.name}-{param_name}"
-
     def get_parameter(self, ssm_param_name: str):
         return self.client.get_parameter(
             Name=ssm_param_name, WithDecryption=True).get('Parameter')
 
     # def resolve(self, param_name: str):
     #     ssm_param_name = self.ssm_param_name(param_name)
     #     try:
     #         fetched_param = self.get_parameter(ssm_param_name)
     #     except self.client.exceptions.ParameterNotFound:
     #         fetched_param = self.put_parameter(ssm_param_name)
     #     self.version = fetched_param.get('Version')
     #     return ssm_param_name
 
 
-class UpdatableSSM(ParameterResolver):
+class UpdatableSSM(ParameterFactoryBase):
     def __init__(self, template: CloudformationTemplate):
         self.ssm_stored = SSMStored()
         self.ssm_stored.secret_token = 'replace-this-with-key'
         super().__init__(template)
 
     @property
     def secret_token(self):
@@ -107,15 +105,15 @@
 
 
 # class GtmContainerConfigStore(UpdatableSSMParameterName):
 #     def ssm_param_name(self, param_name: str) -> str:
 #         return f"{Config().ENV}-{param_name}"
 
 
-class GeneratedSecret(ParameterResolver):
+class GeneratedSecret(ParameterFactoryBase):
     def __init__(self, template: CloudformationTemplate):
         self.ssm_stored = SSMStored()
         self.ssm_stored.secret_token = self.secret_token()
         super().__init__(template)
 
     def secret_token(self):
         """Returns base64 encoded secret.
```

### Comparing `aws_ecs_deploy-0.1.0/aws_deploy/service.py` & `aws_ecs_deploy-0.1.1/aws_deploy/service.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_deploy-0.1.0/pyproject.toml` & `aws_ecs_deploy-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-ecs-deploy"
-version = "0.1.0"
+version = "0.1.1"
 description = "Full lifecyle deployment from github to aws ecs"
 authors = [
     "Ashraful Firoz <ashraf.akon201@gmail.com>",
     "Scotty Rippel <scotty418@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -28,14 +28,15 @@
 docker = "^6.0.1"
 pyotp = "^2.8.0"
 mypy-boto3-cloudformation = "^1.26.108"
 selenium = "^4.9.0"
 mypy-boto3-lambda = "^1.26.122"
 mypy-boto3-ec2 = "^1.26.122"
 mypy-boto3-ecr = "^1.26.0.post1"
+mypy-boto3-s3 = "^1.26.127"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 pytest = "^7.3.1"
 flake8 = "^6.0.0"
```

### Comparing `aws_ecs_deploy-0.1.0/PKG-INFO` & `aws_ecs_deploy-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ecs-deploy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Full lifecyle deployment from github to aws ecs
 License: MIT
 Author: Ashraful Firoz
 Author-email: ashraf.akon201@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: docker (>=6.0.1,<7.0.0)
 Requires-Dist: mypy-boto3-cloudformation (>=1.26.108,<2.0.0)
 Requires-Dist: mypy-boto3-ec2 (>=1.26.122,<2.0.0)
 Requires-Dist: mypy-boto3-ecr (>=1.26.0.post1,<2.0.0)
 Requires-Dist: mypy-boto3-iam (>=1.26.97,<2.0.0)
 Requires-Dist: mypy-boto3-lambda (>=1.26.122,<2.0.0)
+Requires-Dist: mypy-boto3-s3 (>=1.26.127,<2.0.0)
 Requires-Dist: mypy-boto3-ssm (>=1.26.97,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pyotp (>=2.8.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
```

