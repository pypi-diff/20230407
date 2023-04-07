# Comparing `tmp/expose_localhost-0.4.5-py3-none-any.whl.zip` & `tmp/expose_localhost-0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 19232 bytes, number of entries: 15
--rw-r--r--  2.0 unx      112 b- defN 23-Mar-20 00:15 expose/__init__.py
--rw-r--r--  2.0 unx    26279 b- defN 23-Mar-20 00:15 expose/main.py
--rw-r--r--  2.0 unx      160 b- defN 23-Mar-20 00:15 expose/requirements.txt
--rw-r--r--  2.0 unx     1029 b- defN 23-Mar-20 00:15 expose/helpers/auxiliary.py
--rw-r--r--  2.0 unx     4812 b- defN 23-Mar-20 00:15 expose/helpers/cert.py
--rw-r--r--  2.0 unx     1582 b- defN 23-Mar-20 00:15 expose/helpers/config.py
--rw-r--r--  2.0 unx      374 b- defN 23-Mar-20 00:15 expose/helpers/defaults.py
--rw-r--r--  2.0 unx      452 b- defN 23-Mar-20 00:15 expose/helpers/logger.py
--rw-r--r--  2.0 unx     3347 b- defN 23-Mar-20 00:15 expose/helpers/route_53.py
--rw-r--r--  2.0 unx     6332 b- defN 23-Mar-20 00:15 expose/helpers/server.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Mar-20 00:16 expose_localhost-0.4.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     7900 b- defN 23-Mar-20 00:16 expose_localhost-0.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-20 00:16 expose_localhost-0.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-20 00:16 expose_localhost-0.4.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1225 b- defN 23-Mar-20 00:16 expose_localhost-0.4.5.dist-info/RECORD
-15 files, 54782 bytes uncompressed, 17206 bytes compressed:  68.6%
+Zip file size: 19729 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      584 b- defN 23-Apr-07 17:53 expose/__init__.py
+-rw-r--r--  2.0 unx    26287 b- defN 23-Apr-07 17:53 expose/main.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Apr-07 17:53 expose/requirements.txt
+-rw-r--r--  2.0 unx     1029 b- defN 23-Apr-07 17:53 expose/helpers/auxiliary.py
+-rw-r--r--  2.0 unx     4812 b- defN 23-Apr-07 17:53 expose/helpers/cert.py
+-rw-r--r--  2.0 unx     1660 b- defN 23-Apr-07 17:53 expose/helpers/config.py
+-rw-r--r--  2.0 unx      545 b- defN 23-Apr-07 17:53 expose/helpers/defaults.py
+-rw-r--r--  2.0 unx      452 b- defN 23-Apr-07 17:53 expose/helpers/logger.py
+-rw-r--r--  2.0 unx     3273 b- defN 23-Apr-07 17:53 expose/helpers/route_53.py
+-rw-r--r--  2.0 unx     6816 b- defN 23-Apr-07 17:53 expose/helpers/server.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Apr-07 17:53 expose_localhost-0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7797 b- defN 23-Apr-07 17:53 expose_localhost-0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 17:53 expose_localhost-0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-07 17:53 expose_localhost-0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1215 b- defN 23-Apr-07 17:53 expose_localhost-0.5.dist-info/RECORD
+15 files, 55808 bytes uncompressed, 17723 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: expose/helpers/route_53.py
 Comment: 
 
 Filename: expose/helpers/server.py
 Comment: 
 
-Filename: expose_localhost-0.4.5.dist-info/LICENSE
+Filename: expose_localhost-0.5.dist-info/LICENSE
 Comment: 
 
-Filename: expose_localhost-0.4.5.dist-info/METADATA
+Filename: expose_localhost-0.5.dist-info/METADATA
 Comment: 
 
-Filename: expose_localhost-0.4.5.dist-info/WHEEL
+Filename: expose_localhost-0.5.dist-info/WHEEL
 Comment: 
 
-Filename: expose_localhost-0.4.5.dist-info/top_level.txt
+Filename: expose_localhost-0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: expose_localhost-0.4.5.dist-info/RECORD
+Filename: expose_localhost-0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## expose/__init__.py

```diff
@@ -1,4 +1,23 @@
-from expose.helpers import config  # noqa: F401
-from expose.main import Tunnel  # noqa: F401
+import os
+from typing import NoReturn, Union
 
-version = "0.4.5"
+import dotenv
+
+from .helpers import config  # noqa: F401
+from .main import Tunnel  # noqa: F401
+
+version = "0.5"
+
+
+def load_env(filename: Union[str, os.PathLike] = ".env", scan: bool = False) -> NoReturn:
+    """Load .env files."""
+    if scan:
+        for file in os.listdir():
+            if os.path.isfile(file) and file.endswith(".env"):
+                dotenv.load_dotenv(dotenv_path=file, verbose=False)
+    else:
+        if os.path.isfile(filename):
+            dotenv.load_dotenv(dotenv_path=filename, verbose=False)
+
+
+load_env()
```

## expose/main.py

```diff
@@ -4,72 +4,73 @@
 import time
 
 import boto3
 import requests
 import urllib3.exceptions
 from botocore.exceptions import ClientError
 
-from expose.helpers.auxiliary import IP_INFO
-from expose.helpers.cert import generate_cert
-from expose.helpers.config import env, fileio, wait
-from expose.helpers.defaults import AWSDefaults
-from expose.helpers.logger import LOGGER
-from expose.helpers.route_53 import change_record_set
-from expose.helpers.server import Server
+from .helpers.auxiliary import IP_INFO
+from .helpers.cert import generate_cert
+from .helpers.config import EnvConfig, fileio, wait
+from .helpers.defaults import AWSDefaults
+from .helpers.logger import LOGGER
+from .helpers.route_53 import change_record_set
+from .helpers.server import Server
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)  # Disable warnings for self-signed certificates
 
 CONFIGURATION_LOCATION = 'https://raw.githubusercontent.com/thevickypedia/expose/main/configuration/'
 
 
 class Tunnel:
     """Initiates ``Tunnel`` object to spin up an EC2 instance with a pre-configured AMI which acts as a tunnel.
 
     >>> Tunnel
 
     """
 
-    def __init__(self, port: int = env.port, image_id: str = env.image_id, domain_name: str = env.domain_name,
-                 subdomain: str = env.subdomain, aws_access_key: str = env.aws_access_key,
-                 aws_secret_key: str = env.aws_secret_key, aws_region_name: str = env.aws_region_name,
-                 email_address: str = env.email_address, organization: str = env.organization,
-                 logger: logging.Logger = LOGGER):
+    def __init__(self, port: int = None, image_id: str = None, domain: str = None,
+                 subdomain: str = None, aws_access_key: str = None, aws_secret_key: str = None,
+                 aws_region_name: str = None, email_address: str = None, organization: str = None,
+                 logger: logging.Logger = None):
         """Assigns a name to the PEM file, initiates the logger, client and resource for EC2 using ``boto3`` module.
 
         Args:
             port: Port number where the application/API is running in localhost.
             image_id: Takes image ID as an argument. Defaults to ``ami_id`` in environment variable.
-            domain_name: Name of the hosted zone in which an ``A`` record has to be added. [``example.com``]
+            domain: Name of the hosted zone in which an ``A`` record has to be added. [``example.com``]
             subdomain: Subdomain using which the localhost has to be accessed. [``tunnel`` or ``tunnel.example.com``]
             aws_access_key: Access token for AWS account.
             aws_secret_key: Secret ID for AWS account.
             aws_region_name: Region where the instance should live. Defaults to ``us-west-2``
 
         See Also:
             - If no values (for aws authentication) are passed during object initialization, script checks for env vars.
             - If the environment variables are ``null``, gets the default credentials from ``~/.aws/credentials``.
         """
+        env = EnvConfig()
+
         # AWS client and resource setup
-        session = boto3.Session(region_name=aws_region_name,
-                                aws_access_key_id=aws_access_key,
-                                aws_secret_access_key=aws_secret_key)
-        self.region = aws_region_name.lower()
+        self.region = (aws_region_name or env.aws_region_name).lower()
+        session = boto3.Session(region_name=aws_region_name or env.aws_region_name,
+                                aws_access_key_id=aws_access_key or aws_access_key,
+                                aws_secret_access_key=aws_secret_key or aws_secret_key)
         self.ec2_client = session.client(service_name='ec2')
         self.ec2_resource = session.resource(service_name='ec2')
         self.route53_client = session.client(service_name='route53')
 
         # Tunnelling requirements setup
-        self.image_id = image_id
-        self.port = port
-        self.domain_name = domain_name
-        self.subdomain = subdomain
-        self.email_address = email_address
-        self.organization = organization
+        self.image_id = image_id or env.image_id
+        self.port = port or env.port
+        self.domain_name = domain or env.domain
+        self.subdomain = subdomain or env.subdomain
+        self.email_address = email_address or env.email_address
+        self.organization = organization or env.organization
 
-        self.logger = logger
+        self.logger = logger or LOGGER
 
     def _get_image_id(self) -> None:
         """Fetches AMI ID from public images."""
         if self.region.startswith('us'):
             self.image_id = AWSDefaults.IMAGE_MAP[self.region]
             return
 
@@ -387,17 +388,17 @@
             self.logger.warning('Received request to start VM, but looks like a session is up and running already.')
             self.logger.warning('Initiating re-configuration.')
             with open('server_info.json') as file:
                 data = json.load(file)
             self._configure_vm(public_dns=data.get('public_dns'), public_ip=data.get('public_ip'))
             return
 
-        if not all([self.domain_name, self.subdomain]):
+        if not all((self.domain_name, self.subdomain)):
             self.logger.warning("DOMAIN and SUBDOMAIN gives a customized access to the tunnel.")
-        if not all([self.email_address, self.organization]):
+        if not all((self.email_address, self.organization)):
             self.logger.warning("EMAIL_ADDRESS and ORGANIZATION can be used to create a customized certificate.")
 
         if not self.image_id:
             self._get_image_id()
             self.logger.info("AMI ID was not set. Using the default AMI ID '%s' for the region '%s'",
                              self.image_id, self.region)
 
@@ -511,22 +512,21 @@
             download_and_copy["nginx.conf"] = _download_config_file(filename="nginx-non-ssl.conf")
 
         self.logger.info('Copying configuration files to %s', public_dns)
         nginx_server.server_write(data=download_and_copy)
 
         self.logger.info('Configuring nginx server.')
         nginx_status = nginx_server.run_interactive_ssh(
-            commands=[
+            commands=(
                 "sudo apt-get update -y",
-                "sudo apt-get upgrade -y",
                 "echo Y | sudo -S apt-get install nginx -y",
                 "sudo mv /home/ubuntu/server.conf /etc/nginx/conf.d/server.conf",
                 "sudo mv /home/ubuntu/nginx.conf /etc/nginx/nginx.conf",
                 "sudo systemctl restart nginx"
-            ]
+            )
         )
         if not nginx_status:
             self.logger.error('Nginx server was not configured. Cleaning up AWS resources acquired.')
             self.stop()
             return
 
         self.logger.info('Nginx server was configured successfully.')
```

## expose/helpers/config.py

```diff
@@ -1,33 +1,28 @@
 import os
 
-import dotenv
 
-dotenv.load_dotenv(dotenv_path='.env')
-
-
-class EnvConfig(dict):
+class EnvConfig:
     """Wrapper to load env variables.
 
     >>> EnvConfig
 
     """
 
-    port: int = os.environ.get('PORT') or os.environ.get('port')
-    image_id: str = os.environ.get('AMI_ID') or os.environ.get('ami_id')
-    domain_name: str = os.environ.get('DOMAIN') or os.environ.get('domain')
-    subdomain: str = os.environ.get('SUBDOMAIN') or os.environ.get('subdomain')
-    aws_access_key: str = os.environ.get('ACCESS_KEY') or os.environ.get('access_key')
-    aws_secret_key: str = os.environ.get('SECRET_KEY') or os.environ.get('secret_key')
-    aws_region_name: str = os.environ.get('REGION_NAME') or os.environ.get('region_name') or 'us-west-2'
-    email_address: str = os.environ.get('EMAIL_ADDRESS') or os.environ.get('email_address')
-    organization: str = os.environ.get('ORGANIZATION') or os.environ.get('organization')
-
-
-env = EnvConfig()
+    def __init__(self):
+        """Load all env vars."""
+        self.port: str = os.environ.get('PORT') or os.environ.get('port')
+        self.image_id: str = os.environ.get('IMAGE_ID') or os.environ.get('image_id')
+        self.domain: str = os.environ.get('DOMAIN') or os.environ.get('domain')
+        self.subdomain: str = os.environ.get('SUBDOMAIN') or os.environ.get('subdomain')
+        self.aws_access_key: str = os.environ.get('AWS_ACCESS_KEY') or os.environ.get('aws_access_key')
+        self.aws_secret_key: str = os.environ.get('AWS_SECRET_KEY') or os.environ.get('aws_secret_key')
+        self.aws_region_name: str = os.environ.get('AWS_REGION_NAME') or os.environ.get('aws_region_name', 'us-west-2')
+        self.email_address: str = os.environ.get('EMAIL_ADDRESS') or os.environ.get('email_address')
+        self.organization: str = os.environ.get('ORGANIZATION') or os.environ.get('organization')
 
 
 class WaitTimes:
     """Wrapper for different wait times.
 
     >>> WaitTimes
```

## expose/helpers/defaults.py

```diff
@@ -9,7 +9,9 @@
 
     IMAGE_MAP = {
         "us-east-2": "ami-0971e839208a0d58a",
         "us-east-1": "ami-0eaca42ad8ff8647d",
         "us-west-1": "ami-0005fe7be6ce06e3c",
         "us-west-2": "ami-06e20d17437157772"
     }
+    SUPPORTED_RECORDS = ('SOA', 'A', 'TXT', 'NS', 'CNAME', 'MX', 'NAPTR', 'PTR', 'SRV', 'SPF', 'AAAA', 'CAA', 'DS')
+    SUPPORTED_ACTIONS = ('CREATE', 'DELETE', 'UPSERT')
```

## expose/helpers/route_53.py

```diff
@@ -1,13 +1,15 @@
 import logging
 from typing import Dict, Union
 
 import boto3
 from botocore.exceptions import ClientError
 
+from expose.helpers.defaults import AWSDefaults
+
 
 def _get_zone_id(client: boto3.client, logger: logging.Logger, dns: str = None) -> str or None:
     """Gets the zone ID of a DNS name registered in route53.
 
     Args:
         client: Pre instantiated boto3 client.
         logger: Custom logger.
@@ -43,25 +45,23 @@
         logger: Custom logger.
         action: The action to perform.
 
     Returns:
         dict or None:
         ChangeSet response from AWS.
     """
-    supported_records = ['SOA', 'A', 'TXT', 'NS', 'CNAME', 'MX', 'NAPTR', 'PTR', 'SRV', 'SPF', 'AAAA', 'CAA', 'DS']
-    if record_type not in supported_records:
+    if record_type not in AWSDefaults.SUPPORTED_RECORDS:
         logger.error('Unsupported record type passed.')
-        logger.warning(f"Should be one of {', '.join(sorted(supported_records))}")
+        logger.warning(f"Should be one of {', '.join(sorted(AWSDefaults.SUPPORTED_RECORDS))}")
         return
 
     action = action.upper()
-    supported_actions = ['CREATE', 'DELETE', 'UPSERT']
-    if action not in supported_actions:
+    if action not in AWSDefaults.SUPPORTED_ACTIONS:
         logger.error('Unsupported action type passed.')
-        logger.warning(f"Should be one of {', '.join(sorted(supported_actions))}")
+        logger.warning(f"Should be one of {', '.join(sorted(AWSDefaults.SUPPORTED_ACTIONS))}")
         return
 
     if not source.endswith(dns_name):
         source = f'{source}.{dns_name}'
     logger.info("%s `%s` record::%s -> %s", action, record_type, source, destination)
     try:
         response = client.change_resource_record_sets(
```

## expose/helpers/server.py

```diff
@@ -1,15 +1,15 @@
 import logging
 import sys
 import time
 from select import select
 from socket import socket
 from threading import Thread
 from time import sleep
-from typing import List, Union
+from typing import List, Tuple, Union
 
 import requests
 from paramiko import AutoAddPolicy, RSAKey, SSHClient
 from paramiko.channel import Channel
 from paramiko.transport import Transport
 
 
@@ -62,15 +62,15 @@
         pem_key = RSAKey.from_private_key_file(filename=pem_file)
         self.ssh_client = SSHClient()
         self.ssh_client.load_system_host_keys()
         self.ssh_client.set_missing_host_key_policy(AutoAddPolicy())
         self.ssh_client.connect(hostname=hostname, username=username, pkey=pem_key)
         self.logger = logger
 
-    def run_interactive_ssh(self, commands: List[str]) -> bool:
+    def run_interactive_ssh(self, commands: Tuple[str, str, str, str, str]) -> bool:
         """Authenticates remote server using a ``*.pem`` file and runs interactive ssh commands using ``paramiko``.
 
         Args:
             commands: List of commands to be executed.
 
         Returns:
             bool:
@@ -150,20 +150,29 @@
                 self.logger.info('Application is running on port: %d', port)
                 break
             except requests.exceptions.RequestException:
                 print_warning(port=port)
         self.logger.info("Awaiting connection...")
         transport: Transport = self.ssh_client.get_transport()
         transport.request_port_forward(address="localhost", port=8080)
+        threads: List[Thread] = []
         try:
             while True:
                 if not (channel := transport.accept(timeout=1000)):
                     continue
-                Thread(target=self._handler, args=[channel, port], daemon=True).start()
+                thread = Thread(target=self._handler, args=(channel, port))
+                thread.daemon = True
+                thread.start()
+                self.logger.debug("Launching daemon service: %s", thread.ident or thread.native_id)
+                threads.append(thread)
         except KeyboardInterrupt:
             self.logger.info("Tunneling interrupted")
         if host_keys := self.ssh_client.get_host_keys().keys():
             self.logger.info("Closing SSH connection on %s", host_keys[0])
         else:
             self.logger.info("Closing SSH connection on %s", join(transport.getpeername()))
         transport.cancel_port_forward(address="localhost", port=8080)
         self.ssh_client.close()
+        self.logger.info("Daemons launched: %d", len(threads))
+        for thread in threads:
+            self.logger.debug("Awaiting daemon service: %s", thread.ident or thread.native_id)
+            thread.join(timeout=0.5)
```

## Comparing `expose_localhost-0.4.5.dist-info/LICENSE` & `expose_localhost-0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `expose_localhost-0.4.5.dist-info/METADATA` & `expose_localhost-0.5.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expose-localhost
-Version: 0.4.5
+Version: 0.5
 Summary: Expose an app/api running on local host to public internet using AWS EC2
 Author-email: Vignesh Sivanandha Rao <svignesh1793@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Vignesh Sivanandha Rao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,34 +57,37 @@
 Provides-Extra: dev
 Requires-Dist: pre-commit ; extra == 'dev'
 
 # Expose localhost using EC2
 Expose an app/api running on local host to public internet using AWS EC2
 
 ### Requirements
-- Access to an AWS account.
+- Access to an AWS account and [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html#getting-started-install-instructions) configured.
 - A `service/app/api` running on a specific port that has to be exposed to public internet.
 - **[Optional]** A domain `example.com` hosted on `route53`.
 
 ### Setup
 #### Environment Variables:
 Environment variables can be loaded from a `.env` file.
 
 **Mandatory Arg:**
 - `PORT`: Port number that has to be exposed (on which a localhost `service/app/api` is running)
 
 **Optional Args:**
-- `AMI_ID`: ID of any public AMI with an Ubuntu OS. Defaults to a region specific image ID.
-- `ACCESS_KEY`: Access key to access AWS resources. Defaults to `~/.aws/config`
-- `SECRET_KEY`: Secret key to access AWS resources. Defaults to `~/.aws/config`
-- `REGION_NAME`: Region name where the instance should live. Defaults to `US-WEST-2`
-- `DOMAIN`: If the domain name is registered using `route53`. *Example: `mywebsite.com`*
-- `SUBDOMAIN`: Sub-domain that has to be added for the domain name. *Example: `tunnel.mywebsite.com`*
-- `EMAIL`: Email address to create the self-signed SSL and private key. Defaults to `USER@expose-localhost.com`
-- `ORG`: Organization name for the certificate. Defaults to the AWS endpoint.
+- `IMAGE_ID`: ID of any public AMI with an Ubuntu OS. Defaults to a region specific image ID.
+- `AWS_ACCESS_KEY`: Access key to access AWS resources. Defaults to `~/.aws/config`
+- `AWS_SECRET_KEY`: Secret key to access AWS resources. Defaults to `~/.aws/config`
+- `AWS_REGION_NAME`: Region name where the instance should live. Defaults to `US-WEST-2`
+
+*Optionally `.env` files can also be scanned for:*
+```python
+import expose
+
+expose.load_env(scan=True)
+```
 
 <details>
 <summary><strong>Setup a custom endpoint</strong></summary>
 
 The public DNS names for EC2 instances are long and messy. To avoid that, an `A` record can be added to the `route53` hosted zone.
 
 :warning: &nbsp; Requires an active hosted zone on `route53`.
@@ -113,16 +116,16 @@
 
 > `openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout ~/.ssh/key.pem -out ~/.ssh/cert.pem`
 
 [OR]
 
 Simply let `expose` create a self-signed SSL certificate and a private key.
 
-- `EMAIL`: Email address to create the self-signed SSL and private key. Defaults to `USER@expose-localhost.com`
-- `ORG`: Organization name for the certificate. Defaults to the AWS endpoint.
+- `EMAIL_ADDRESS`: Email address to create the self-signed SSL and private key. Defaults to `USER@expose-localhost.com`
+- `ORGANIZATION`: Organization name for the certificate. Defaults to the AWS endpoint.
 
 </details>
 
 ### Usage
 ###### Installation
 ```shell
 python3 -m pip install expose-localhost
```

## Comparing `expose_localhost-0.4.5.dist-info/RECORD` & `expose_localhost-0.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-expose/__init__.py,sha256=O0Z-0t7SlOMYyxMnjbb403Gv8zU6HkZoI-TfJr6NLLI,112
-expose/main.py,sha256=byDhWouoMVznUT5pocuNMUxdH2PhqL3cFpTeDogcByM,26279
+expose/__init__.py,sha256=tcT_hxGwzLtck-dGVtAT4M3v3fYg4p5Xr0CAINDFy3I,584
+expose/main.py,sha256=j2MJGnzpuUDl3JrvZl_yg4QRC2f37vckxC9YAvC5Ing,26287
 expose/requirements.txt,sha256=vcz7x9tP90OVpsBpk3A64tIQr_BYien9R7CtDtLmWBU,160
 expose/helpers/auxiliary.py,sha256=9lFHEq4UbKYa5sC6eoOQqccf7Xa6J7tngl9a6ySnp5w,1029
 expose/helpers/cert.py,sha256=MRDNW-EOhInAyQjTJngjguTFBc44OKRr2jd72Ix1KrA,4812
-expose/helpers/config.py,sha256=xcTiSA5BCSr3mR8O8r8RxoAvPnwmaiEFseJBGn-IW7M,1582
-expose/helpers/defaults.py,sha256=WqJRsiYhyRgA2AaKhy-N6eMSdh6ICPo1WD2ImH8QOqE,374
+expose/helpers/config.py,sha256=fGUMZnaTVS0NOS6pJnG1DVtOaoNrj1zgC54s31FnsL8,1660
+expose/helpers/defaults.py,sha256=1QPXZpuVkubtPMmCQgL1VSEr-HDakwl856VzMgA3aLw,545
 expose/helpers/logger.py,sha256=AfFgm17fqVUhsE36eGigFC6b7HM9zTOLwDswS5eNeoo,452
-expose/helpers/route_53.py,sha256=zHsz5IO1OZGFq2GMTelpVxNEvnpMgyJ7EF69bCqetE4,3347
-expose/helpers/server.py,sha256=GpHJ0AIKuLZaaIyYTsUPIXQr9UBnSFMm-U0jf7te7hg,6332
-expose_localhost-0.4.5.dist-info/LICENSE,sha256=QrtVd9OxjohKWoSGkqro3tPJR_7WGlpAQs_IYq269wg,1079
-expose_localhost-0.4.5.dist-info/METADATA,sha256=GnDCiQRe9TrfORJEJOVFdADqzz8YMNDmAjx_F_VWdpo,7900
-expose_localhost-0.4.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-expose_localhost-0.4.5.dist-info/top_level.txt,sha256=rfEifC7BiiixZTxDPETdLI5WnyGn5AS_KX332sx_xHA,7
-expose_localhost-0.4.5.dist-info/RECORD,,
+expose/helpers/route_53.py,sha256=v4VXY9uJGTAc4tkAmuf4pWHPdgV7Nx_CWKB0LGEhVc8,3273
+expose/helpers/server.py,sha256=qPsrCnheBdGdfXVRfavxPqw5aHgf8vfN9Sd9ovASlk0,6816
+expose_localhost-0.5.dist-info/LICENSE,sha256=QrtVd9OxjohKWoSGkqro3tPJR_7WGlpAQs_IYq269wg,1079
+expose_localhost-0.5.dist-info/METADATA,sha256=ZT0hpUMRhKCitn1VnrBsZ5j8cdftvfxaolJBtVcfSC0,7797
+expose_localhost-0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+expose_localhost-0.5.dist-info/top_level.txt,sha256=rfEifC7BiiixZTxDPETdLI5WnyGn5AS_KX332sx_xHA,7
+expose_localhost-0.5.dist-info/RECORD,,
```

