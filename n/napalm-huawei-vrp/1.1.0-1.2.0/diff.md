# Comparing `tmp/napalm-huawei-vrp-1.1.0.tar.gz` & `tmp/napalm-huawei-vrp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm-huawei-vrp-1.1.0.tar", last modified: Sun Oct 30 18:17:56 2022, max compression
+gzip compressed data, was "napalm-huawei-vrp-1.2.0.tar", last modified: Sat Apr  6 19:19:15 2024, max compression
```

## Comparing `napalm-huawei-vrp-1.1.0.tar` & `napalm-huawei-vrp-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 malvarez  (1000) malvarez  (1000)        0 2022-10-30 18:17:56.103256 napalm-huawei-vrp-1.1.0/
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)      122 2022-06-27 02:08:21.000000 napalm-huawei-vrp-1.1.0/MANIFEST.in
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)     5809 2022-10-30 18:17:56.103256 napalm-huawei-vrp-1.1.0/PKG-INFO
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)     3993 2022-06-27 02:08:21.000000 napalm-huawei-vrp-1.1.0/README.md
-drwxrwxr-x   0 malvarez  (1000) malvarez  (1000)        0 2022-10-30 18:17:56.103256 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp/
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)      733 2022-06-27 02:08:21.000000 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp/__init__.py
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)    83785 2022-10-30 18:11:45.000000 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp/huawei_vrp.py
-drwxrwxr-x   0 malvarez  (1000) malvarez  (1000)        0 2022-10-30 18:17:56.103256 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp/utils/
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)       28 2022-06-27 02:08:21.000000 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp/utils/__init__.py
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)      464 2022-06-27 02:08:21.000000 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp/utils/utils.py
-drwxrwxr-x   0 malvarez  (1000) malvarez  (1000)        0 2022-10-30 18:17:56.103256 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp.egg-info/
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)     5809 2022-10-30 18:17:56.000000 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp.egg-info/PKG-INFO
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)      392 2022-10-30 18:17:56.000000 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp.egg-info/SOURCES.txt
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)        1 2022-10-30 18:17:56.000000 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp.egg-info/dependency_links.txt
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)       14 2022-10-30 18:17:56.000000 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp.egg-info/requires.txt
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)       18 2022-10-30 18:17:56.000000 napalm-huawei-vrp-1.1.0/napalm_huawei_vrp.egg-info/top_level.txt
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)       14 2022-06-27 02:08:21.000000 napalm-huawei-vrp-1.1.0/requirements.txt
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)      503 2022-10-30 18:17:56.103256 napalm-huawei-vrp-1.1.0/setup.cfg
--rw-rw-r--   0 malvarez  (1000) malvarez  (1000)     1788 2022-10-30 18:17:13.000000 napalm-huawei-vrp-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:19:15.236627 napalm-huawei-vrp-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-06 19:19:15.236627 napalm-huawei-vrp-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:19:15.232627 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93764 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp/huawei_vrp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:19:15.236627 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:19:15.236627 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-06 19:19:15.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-06 19:19:15.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:19:15.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-06 19:19:15.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 19:19:15.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 19:19:15.000000 napalm-huawei-vrp-1.2.0/napalm_huawei_vrp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-06 19:19:15.236627 napalm-huawei-vrp-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-06 19:19:11.000000 napalm-huawei-vrp-1.2.0/setup.py
```

### Comparing `napalm-huawei-vrp-1.1.0/README.md` & `napalm-huawei-vrp-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `napalm-huawei-vrp-1.1.0/napalm_huawei_vrp/__init__.py` & `napalm-huawei-vrp-1.2.0/napalm_huawei_vrp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 """napalm-skeleton package."""
 from napalm_huawei_vrp.huawei_vrp import VRPDriver
 
-__all__ = ('VRPDriver',)
+__all__ = ("VRPDriver",)
```

### Comparing `napalm-huawei-vrp-1.1.0/napalm_huawei_vrp/huawei_vrp.py` & `napalm-huawei-vrp-1.2.0/napalm_huawei_vrp/huawei_vrp.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 """
 
 import socket
 import re
 import telnetlib
 import os
 import tempfile
-import paramiko
 import uuid
 import hashlib
-import napalm.base.helpers
-import napalm.base.constants as c
+from napalm.base.helpers import mac
+import napalm.base.constants as C
 
 from datetime import datetime
+from diffplus import IndentedConfig, IncrementalDiff
 from napalm.base import NetworkDriver
 from napalm.base.netmiko_helpers import netmiko_args
 from napalm.base.exceptions import (
     MergeConfigException,
     ReplaceConfigException,
     CommandErrorException,
     CommitError,
 )
-from .utils.utils import pretty_mac
+from .utils.utils import pretty_mac, SafeList
 
 # Easier to store these as constants
 HOUR_SECONDS = 3600
 DAY_SECONDS = 24 * HOUR_SECONDS
 WEEK_SECONDS = 7 * DAY_SECONDS
 YEAR_SECONDS = 365 * DAY_SECONDS
 
@@ -53,24 +53,27 @@
 IPV4_ADDR_REGEX = IP_ADDR_REGEX
 IPV6_ADDR_REGEX_1 = r"::"
 IPV6_ADDR_REGEX_2 = r"[0-9a-fA-F:]{1,39}::[0-9a-fA-F:]{1,39}"
 IPV6_ADDR_REGEX_3 = (
     r"[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:"
     "[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}"
 )
-INTERFACE_REGEX = r"(?:[0-9]*GE[0-9\/\.]+)|(?:LoopBack\d+)|(?:Eth-Trunk[0-9\.]+)|(?:Vlanif[0-9\.]+)"
+INTERFACE_REGEX = (
+    r"(?:[0-9]*GE[0-9\/\.]+)|(?:LoopBack\d+)|(?:Eth-Trunk[0-9\.]+)|(?:Vlanif[0-9\.]+)"
+)
 
 # Should validate IPv6 address using an IP address library after matching with this regex
 IPV6_ADDR_REGEX = "(?:{}|{}|{})".format(
     IPV6_ADDR_REGEX_1, IPV6_ADDR_REGEX_2, IPV6_ADDR_REGEX_3
 )
 
 # Period needed for 32-bit AS Numbers
 ASN_REGEX = r"[\d\.]+"
 
+
 class VRPDriver(NetworkDriver):
     """Napalm driver for Huawei vrp."""
 
     def __init__(self, hostname, username, password, timeout=60, optional_args=None):
         """Constructor.
         :param hostname:
         :param username:
@@ -85,44 +88,43 @@
         self.timeout = timeout
 
         if optional_args is None:
             optional_args = {}
 
         # Netmiko possible arguments
         netmiko_argument_map = {
-            'port': None,
-            'verbose': False,
-            'timeout': self.timeout,
-            'global_delay_factor': 1,
-            'use_keys': False,
-            'key_file': None,
-            'ssh_strict': False,
-            'system_host_keys': False,
-            'alt_host_keys': False,
-            'alt_key_file': '',
-            'ssh_config_file': None,
-            'allow_agent': False,
-            'keepalive': 30
+            "port": None,
+            "verbose": False,
+            "timeout": self.timeout,
+            "global_delay_factor": 1,
+            "use_keys": False,
+            "key_file": None,
+            "ssh_strict": False,
+            "system_host_keys": False,
+            "alt_host_keys": False,
+            "alt_key_file": "",
+            "ssh_config_file": None,
+            "allow_agent": False,
+            "keepalive": 30,
         }
 
         # Build dict of any optional Netmiko args
         self.netmiko_optional_args = {
-            k: optional_args.get(k, v)
-            for k, v in netmiko_argument_map.items()
+            k: optional_args.get(k, v) for k, v in netmiko_argument_map.items()
         }
 
-        self.transport = optional_args.get('transport', 'ssh')
-        self.port = optional_args.get('port', 22)
+        self.transport = optional_args.get("transport", "ssh")
+        self.port = optional_args.get("port", 22)
 
         self.changed = False
         self.loaded = False
-        self.backup_file = ''
+        self.backup_file = ""
         self.replace = False
-        self.merge_candidate = ''
-        self.replace_file = ''
+        self.merge_candidate = ""
+        self.replace_file = ""
         self.profile = ["huawei_vrp"]
 
         # netmiko args
         self.netmiko_optional_args = netmiko_args(optional_args)
 
         # Set the default port if not set
         default_port = {"ssh": 22, "telnet": 23}
@@ -132,18 +134,20 @@
         self.auto_file_prompt = optional_args.get("auto_file_prompt", True)
 
         # Track whether 'file prompt quiet' has been changed by NAPALM.
         self.prompt_quiet_changed = False
         # Track whether 'file prompt quiet' is known to be configured
         self.prompt_quiet_configured = None
 
+        # Contextual diff computation mode
+        self.contextual_diff = optional_args.get("contextual_diff", False)
+
     # verified
     def open(self):
-        """Open a connection to the device.
-        """
+        """Open a connection to the device."""
         device_type = "huawei"
         if self.transport == "telnet":
             device_type = "huawei_telnet"
         self.device = self._netmiko_open(
             device_type, netmiko_optional_args=self.netmiko_optional_args
         )
 
@@ -156,34 +160,32 @@
             self.device.send_config_set(["no file prompt quiet"])
             self.prompt_quiet_changed = False
             self.prompt_quiet_configured = False
         self._netmiko_close()
 
     # verified
     def is_alive(self):
-        """ Returns a flag with the state of the connection."""
+        """Returns a flag with the state of the connection."""
         if self.device is None:
-            return {'is_alive': False}
+            return {"is_alive": False}
         try:
-            if self.transport == 'telnet':
+            if self.transport == "telnet":
                 # Try sending IAC + NOP (IAC is telnet way of sending command
                 # IAC = Interpret as Command (it comes before the NOP)
                 self.device.write_channel(telnetlib.IAC + telnetlib.NOP)
-                return {'is_alive': True}
+                return {"is_alive": True}
             else:
                 # SSH
                 # Try sending ASCII null byte to maintain the connection alive
                 null = chr(0)
                 self.device.write_channel(null)
-                return {
-                    'is_alive': self.device.remote_conn.transport.is_active()
-                }
+                return {"is_alive": self.device.remote_conn.transport.is_active()}
         except (socket.error, EOFError, OSError):
             # If unable to send, we can tell for sure that the connection is unusable
-            return {'is_alive': False}
+            return {"is_alive": False}
 
     # verified
     def cli(self, commands):
         """Execute a list of commands and return the output in a dictionary format using the command
         Example input:
         ['dis version', 'dis cu']
         """
@@ -199,66 +201,76 @@
 
         return cli_output
 
     # verified
     def get_facts(self):
         """Return a set of facts from the devices."""
         # default values.
-        vendor = u'Huawei'
+        vendor = "Huawei"
         uptime = -1
-        serial_number, fqdn, os_version, hostname, model = (u'Unknown', u'Unknown', u'Unknown', u'Unknown', u'Unknown')
+        serial_number, fqdn, os_version, hostname, model = (
+            "Unknown",
+            "Unknown",
+            "Unknown",
+            "Unknown",
+            "Unknown",
+        )
 
         # obtain output from device
-        show_ver = self.device.send_command('display version')
-        show_hostname = self.device.send_command('display current-configuration | inc sysname')
-        show_int_status = self.device.send_command('display interface brief')
-        show_esn = self.device.send_command('display esn')
+        show_ver = self.device.send_command("display version")
+        show_hostname = self.device.send_command(
+            "display current-configuration | inc sysname"
+        )
+        show_int_status = self.device.send_command("display interface brief")
+        show_esn = self.device.send_command("display esn")
 
         # os_version/uptime/model
         for line in show_ver.splitlines():
-            if 'VRP (R) software' in line:
+            if "VRP (R) software" in line:
                 search_result = re.search(r"\(S\S+\s+(?P<os_version>V\S+)\)", line)
                 if search_result is not None:
-                    os_version = search_result.group('os_version')
+                    os_version = search_result.group("os_version")
 
-            if 'HUAWEI' in line and 'uptime is' in line:
+            if "HUAWEI" in line and "uptime is" in line:
                 search_result = re.search(r"S\S+", line)
                 if search_result is not None:
                     model = search_result.group(0)
                 uptime = self._parse_uptime(line)
                 break
 
         # get serial_number,due to the stack have multiple SN, so show it in a list
         # 由于堆叠设备会有多少个SN，所以这里用列表展示
         re_sn = r"ESN\s+of\s+slot\s+\S+\s+(?P<serial_number>\S+)"
         serial_number = re.findall(re_sn, show_esn, flags=re.M)
 
-        if 'sysname ' in show_hostname:
+        if "sysname " in show_hostname:
             _, hostname = show_hostname.split("sysname ")
             hostname = hostname.strip()
 
         # interface_list filter
         interface_list = []
-        if 'Interface' in show_int_status:
+        if "Interface" in show_int_status:
             _, interface_part = show_int_status.split("Interface")
-            re_intf = r"(?P<interface>\S+)\s+(?P<physical_state>down|up|offline|\*down)\s+" \
-                      r"(?P<protocal_state>down|up|\*down)"
+            re_intf = (
+                r"(?P<interface>\S+)\s+(?P<physical_state>down|up|offline|\*down)\s+"
+                r"(?P<protocal_state>down|up|\*down)"
+            )
             search_result = re.findall(re_intf, interface_part, flags=re.M)
             for interface_info in search_result:
                 interface_list.append(interface_info[0])
 
         return {
-            'uptime': int(uptime),
-            'vendor': vendor,
-            'os_version': os_version,
-            'serial_number': serial_number,
-            'model': model,
-            'hostname': hostname,
-            'fqdn': fqdn,  # ? fqdn(fully qualified domain name)
-            'interface_list': interface_list
+            "uptime": int(uptime),
+            "vendor": vendor,
+            "os_version": os_version,
+            "serial_number": serial_number,
+            "model": model,
+            "hostname": hostname,
+            "fqdn": fqdn,  # ? fqdn(fully qualified domain name)
+            "interface_list": interface_list,
         }
 
     # developing
     def get_environment(self):
         """
         Return environment details.
 
@@ -293,269 +305,270 @@
                 }
             }
         }
         """
         # 空包
         environment = {}
         # 定义执行命令
-        fan_cmd = 'display fan'
+        fan_cmd = "display fan"
         """
          Slot  FanID   Online    Status    Speed     Mode     Airflow            
         -------------------------------------------------------------------------
          0     1       Present   Normal    55%       Auto     Side-to-Back
          1     1       Present   Normal    55%       Auto     Side-to-Back
         """
-        power_cmd = 'display power'
+        power_cmd = "display power"
         """
         ------------------------------------------------------------
          Slot    PowerID  Online   Mode   State      Power(W)
         ------------------------------------------------------------
          0       PWR1     Present  AC     Supply     600.00     
          0       PWR2     Present  AC     Supply     600.00     
          1       PWR1     Present  AC     Supply     600.00     
          1       PWR2     Present  AC     Supply     600.00  
         """
-        temp_cmd = 'display temperature all'
+        temp_cmd = "display temperature all"
         """
         -------------------------------------------------------------------------------
          Slot  Card  Sensor Status    Current(C) Lower(C) Lower     Upper(C) Upper
                                                           Resume(C)          Resume(C)
         -------------------------------------------------------------------------------
          0     NA    NA     Normal     37        0        4         63       59
          1     NA    NA     Normal     39        0        4         63       59
          """
-        cpu_cmd = 'display cpu-usage'
+        cpu_cmd = "display cpu-usage"
         """
         CPU Usage Stat. Cycle: 60 (Second)
         CPU Usage            : 28% Max: 87%
         CPU Usage Stat. Time : 2022-01-13  18:57:06 
         CPU utilization for five seconds: 28%: one minute: 28%: five minutes: 20%
         Max CPU Usage Stat. Time : 2021-10-05 17:50:44.
         """
-        mem_cmd = 'display memory-usage'
+        mem_cmd = "display memory-usage"
         """
          Memory utilization statistics at 2022-01-13 18:57:37+08:00
          System Total Memory Is: 1598029824 bytes
          Total Memory Used Is: 188593436 bytes
          Memory Using Percentage Is: 11%
         """
         # 发送命令
         fan_output = self.device.send_command(fan_cmd)
         power_cmd = self.device.send_command(power_cmd)
         temp_cmd = self.device.send_command(temp_cmd)
         cpu_cmd = self.device.send_command(cpu_cmd)
         mem_cmd = self.device.send_command(mem_cmd)
         # 设备风扇情况
-        environment.setdefault('fans', {})
-        for i in fan_output.split('\n'):
+        environment.setdefault("fans", {})
+        for i in fan_output.split("\n"):
             match = re.match(r"\s+(\d+).+(Normal|Abnormal).+", i)
             if match:
                 slot = match.group(1)
                 status = True if match.group(2) == "Normal" else False
-                environment['fans'][slot] = {'status': status}
+                environment["fans"][slot] = {"status": status}
 
         # 设备电源情况
-        environment.setdefault('power', {})
-        for i in power_cmd.split('\n'):
+        environment.setdefault("power", {})
+        for i in power_cmd.split("\n"):
             # match = re.match(r"\s+(\d+).+(Normal|Abnormal).+", i)
             match = re.match(r"\s+(\d+)\s+(\w+\d+)\s+(\w+).+\s+(\w+)\s+(\d+\.\d+)", i)
             if match:
-                environment['power'][f"{match.group(2)}-{match.group(1)}"] = {
+                environment["power"][f"{match.group(2)}-{match.group(1)}"] = {
                     "capacity": float(match.group(5)),
                     "output": None,
-                    "status": True if match.group(4) == 'Supply' else False
-
+                    "status": True if match.group(4) == "Supply" else False,
                 }
         # 设备温度情况
-        environment.setdefault('temperature', {})
-        for i in temp_cmd.split('\n'):
-            match = re.split('\s+', i)
+        environment.setdefault("temperature", {})
+        for i in temp_cmd.split("\n"):
+            match = re.split("\s+", i)
             if len(match) == 10:
-                if 'Upper' not in match:
-                    environment['temperature']['slot' + match[1]] = {
+                if "Upper" not in match:
+                    environment["temperature"]["slot" + match[1]] = {
                         "is_alert": False if match[4] == "Normal" else True,
                         "is_critical": False if match[4] == "Normal" else True,
-                        "temperature": float(match[-1])
+                        "temperature": float(match[-1]),
                     }
 
         # CPU使用率
-        environment.setdefault('cpu', {})
-        cpu_use = re.search(r'CPU utilization for five seconds: \d+%: one minute: \d+%: five minutes: (\d+)%', cpu_cmd)
-        environment['cpu'] = {
-            "0": {
-                "usage": cpu_use.group(1)
-            }
-
-        }
+        environment.setdefault("cpu", {})
+        cpu_use = re.search(
+            r"CPU utilization for five seconds: \d+%: one minute: \d+%: five minutes: (\d+)%",
+            cpu_cmd,
+        )
+        environment["cpu"] = {"0": {"usage": cpu_use.group(1)}}
         # 内存使用情况
-        environment.setdefault('memory', {})
-        memory_use = re.findall(r'(\d+) bytes', mem_cmd)
-        environment['memory'] = {
+        environment.setdefault("memory", {})
+        memory_use = re.findall(r"(\d+) bytes", mem_cmd)
+        environment["memory"] = {
             "available_ram": int(memory_use[0]) - int(memory_use[1]),
-            "used_ram": int(memory_use[1])
+            "used_ram": int(memory_use[1]),
         }
         return environment
 
     # verified
     def get_config(self, retrieve="all", full=False):
         """
         Get config from device.
 
         Returns the running configuration as dictionary.
         The candidate and startup are always empty string for now,
         since CE does not support candidate configuration.
         """
-        config = {
-            'startup': '',
-            'running': '',
-            'candidate': ''
-        }
+        config = {"startup": "", "running": "", "candidate": ""}
 
-        if retrieve.lower() in ('running', 'all'):
-            command = 'display current-configuration'
-            config['running'] = self.device.send_command(command)
-        if retrieve.lower() in ('startup', 'all'):
+        if retrieve.lower() in ("running", "all"):
+            command = "display current-configuration"
+            config["running"] = self.device.send_command(command)
+        if retrieve.lower() in ("startup", "all"):
             # command = 'display saved-configuration last'
             # config['startup'] = py23_compat.text_type(self.device.send_command(command))
             pass
         return config
 
     # ok
     def load_merge_candidate(self, filename=None, config=None):
         """Open the candidate config and merge."""
         if not filename and not config:
-            raise MergeConfigException('filename or config param must be provided.')
+            raise MergeConfigException("filename or config param must be provided.")
 
-        self.merge_candidate += '\n'  # insert one extra line
+        self.merge_candidate += "\n"  # insert one extra line
         if filename is not None:
             with open(filename, "r") as f:
                 self.merge_candidate += f.read()
         else:
             self.merge_candidate += config
 
         self.replace = False
         self.loaded = True
 
     # developing
     def load_replace_candidate(self, filename=None, config=None):
         """Open the candidate config and replace."""
-        if not filename and not config:
-            raise ReplaceConfigException('filename or config param must be provided.')
-
-        self._replace_candidate(filename, config)
-        self.replace = True
-        self.loaded = True
+        pass
 
     # ok
     def commit_config(self, message=""):
         """Commit configuration."""
         if self.loaded:
             try:
-                self.backup_file = 'config_' + datetime.now().strftime("%Y%m%d_%H%M") + '.cfg'
+                self.backup_file = (
+                    "config_" + datetime.now().strftime("%Y%m%d_%H%M") + ".cfg"
+                )
                 if self._check_file_exists(self.backup_file):
                     self._delete_file(self.backup_file)
                 self._save_config(self.backup_file)
                 if self.replace:
-                    self._load_config(self.replace_file.split('/')[-1])
+                    self._load_config(self.replace_file.split("/")[-1])
                 else:
                     self._commit_merge()
-                    self.merge_candidate = ''  # clear the merge buffer
+                    self.merge_candidate = ""  # clear the merge buffer
 
                 self.changed = True
                 self.loaded = False
                 self._save_config()
             except Exception as e:
                 raise CommitError(str(e))
         else:
-            raise CommitError('No config loaded.')
+            raise CommitError("No config loaded.")
 
     # ok
     def compare_config(self):
         """Compare candidate config with running."""
         if self.loaded:
             if not self.replace:
+                if self.contextual_diff:
+                    return self._get_contextual_diff()
                 return self._get_merge_diff()
                 # return self.merge_candidate
-            diff = self._get_diff(self.replace_file.split('/')[-1])
+            diff = self._get_diff(self.replace_file.split("/")[-1])
             return diff
-        return ''
+        return ""
 
     # ok
     def discard_config(self):
         """Discard changes."""
         if self.loaded:
-            self.merge_candidate = ''  # clear the buffer
+            self.merge_candidate = ""  # clear the buffer
         if self.loaded and self.replace:
             self._delete_file(self.replace_file)
         self.loaded = False
 
     # developing
     def rollback(self):
         """Rollback to previous commit."""
         if self.changed:
             self._load_config(self.backup_file)
             self.changed = False
             self._save_config()
 
     # verified
-    def ping(self, destination, source=c.PING_SOURCE, ttl=c.PING_TTL, timeout=c.PING_TIMEOUT, size=c.PING_SIZE,
-             count=c.PING_COUNT, vrf=c.PING_VRF):
+    def ping(
+        self,
+        destination,
+        source=C.PING_SOURCE,
+        ttl=C.PING_TTL,
+        timeout=C.PING_TIMEOUT,
+        size=C.PING_SIZE,
+        count=C.PING_COUNT,
+        vrf=C.PING_VRF,
+    ):
         """Execute ping on the device."""
         ping_dict = {}
-        command = 'ping'
+        command = "ping"
         # Timeout in milliseconds to wait for each reply, the default is 2000
-        command += ' -t {}'.format(timeout * 1000)
+        command += " -t {}".format(timeout * 1000)
         # Specify the number of data bytes to be sent
-        command += ' -s {}'.format(size)
+        command += " -s {}".format(size)
         # Specify the number of echo requests to be sent
-        command += ' -c {}'.format(count)
-        if source != '':
-            command += ' -a {}'.format(source)
-        command += ' {}'.format(destination)
+        command += " -c {}".format(count)
+        if source != "":
+            command += " -a {}".format(source)
+        command += " {}".format(destination)
         output = self.device.send_command(command)
 
-        if 'Error' in output:
-            ping_dict['error'] = output
-        elif 'PING' in output:
-            ping_dict['success'] = {
-                'probes_sent': 0,
-                'packet_loss': 0,
-                'rtt_min': 0.0,
-                'rtt_max': 0.0,
-                'rtt_avg': 0.0,
-                'rtt_stddev': 0.0,
-                'results': []
+        if "Error" in output:
+            ping_dict["error"] = output
+        elif "PING" in output:
+            ping_dict["success"] = {
+                "probes_sent": 0,
+                "packet_loss": 0,
+                "rtt_min": 0.0,
+                "rtt_max": 0.0,
+                "rtt_avg": 0.0,
+                "rtt_stddev": 0.0,
+                "results": [],
             }
 
             match_sent = re.search(r"(\d+).+transmitted", output, re.M)
             match_received = re.search(r"(\d+).+received", output, re.M)
 
             try:
                 probes_sent = int(match_sent.group(1))
                 probes_received = int(match_received.group(1))
-                ping_dict['success']['probes_sent'] = probes_sent
-                ping_dict['success']['packet_loss'] = probes_sent - probes_received
+                ping_dict["success"]["probes_sent"] = probes_sent
+                ping_dict["success"]["packet_loss"] = probes_sent - probes_received
             except Exception:
                 msg = "Unexpected output data:\n{}".format(output)
                 raise ValueError(msg)
 
             match = re.search(r"min/avg/max = (\d+)/(\d+)/(\d+)", output, re.M)
             if match:
-                ping_dict['success'].update({
-                    'rtt_min': float(match.group(1)),
-                    'rtt_avg': float(match.group(2)),
-                    'rtt_max': float(match.group(3)),
-                })
+                ping_dict["success"].update(
+                    {
+                        "rtt_min": float(match.group(1)),
+                        "rtt_avg": float(match.group(2)),
+                        "rtt_max": float(match.group(3)),
+                    }
+                )
 
                 results_array = []
                 match = re.findall(r"Reply from.+time=(\d+)", output, re.M)
                 for i in match:
-                    results_array.append({'ip_address': destination,
-                                          'rtt': float(i)})
-                ping_dict['success'].update({'results': results_array})
+                    results_array.append({"ip_address": destination, "rtt": float(i)})
+                ping_dict["success"].update({"results": results_array})
         return ping_dict
 
     # developing
     def traceroute(self):
         pass
 
     # get information from network device
@@ -581,69 +594,87 @@
                 "is_up": false,
                 "mac_address": "0C:45:BA:7D:83:E4",
                 "speed": -1
             }
         }
         """
         interfaces = {}
-        output = self.device.send_command('display interface')
+        output = self.device.send_command("display interface")
         if not output:
             return {}
 
         separator = r"(^(?!Line protocol).*current state.*$)"
-        re_intf_name_state = r"^(?!Line protocol)(?P<intf_name>\S+).+current state\W+(?P<intf_state>.+)$"
+        re_intf_name_state = (
+            r"^(?!Line protocol)(?P<intf_name>\S+).+current state\W+(?P<intf_state>.+)$"
+        )
         re_protocol = r"Line protocol current state\W+(?P<protocol>.+)$"
         re_mac = r"Hardware address is\W+(?P<mac_address>\S+)"
         re_speed = r"^Speed\W+(?P<speed>\d+|\w+)"
-        re_description = r"^Description\W+(?P<description>.*)$"
+        re_description = r"Description:(?:(?:)|(?P<description>.*))\n"
+        re_mtu = r"Maximum Transmit Unit(?:(?:\(L3\))|(?:)) is (?P<int_mtu>\d+)"
 
         new_interfaces = self._separate_section(separator, output)
         for interface in new_interfaces:
             interface = interface.strip()
             match_intf = re.search(re_intf_name_state, interface, flags=re.M)
             match_proto = re.search(re_protocol, interface, flags=re.M)
 
             if match_intf is None or match_proto is None:
                 msg = "Unexpected interface format: {}".format(interface)
                 raise ValueError(msg)
-            intf_name = match_intf.group('intf_name')
-            intf_state = match_intf.group('intf_state')
-            is_enabled = bool('up' in intf_state.lower())
+            intf_name = match_intf.group("intf_name")
+            intf_state = match_intf.group("intf_state")
+            is_enabled = bool("up" in intf_state.lower())
 
-            protocol = match_proto.group('protocol')
-            is_up = bool('up' in protocol.lower())
+            protocol = match_proto.group("protocol")
+            is_up = bool("up" in protocol.lower())
 
             match_mac = re.search(re_mac, interface, flags=re.M)
             if match_mac:
-                mac_address = match_mac.group('mac_address')
-                mac_address = napalm.base.helpers.mac(mac_address)
+                mac_address = match_mac.group("mac_address")
+                mac_address = mac(mac_address)
             else:
                 mac_address = ""
 
-            speed = -1
+            # interface MTU Matching
+            intf_mtu = -1
+            match = re.search(re_mtu, interface, flags=re.M)
+            if match:
+                intf_mtu = int(match.group("int_mtu"))
+
+            speed = -1.0
             match_speed = re.search(re_speed, interface, flags=re.M)
             if match_speed:
-                speed = match_speed.group('speed')
+                speed = match_speed.group("speed")
                 if speed.isdigit():
-                    speed = int(speed)
+                    speed = float(speed)
 
-            description = ''
-            match = re.search(re_description, interface, flags=re.M)
+            # description matching
+            description = ""
+            match = re.search(re_description, interface)
             if match:
-                description = match.group('description')
+                description = (
+                    match.group("description").strip()
+                    if match.group("description")
+                    else ""
+                )
 
-            interfaces.update({
-                intf_name: {
-                    'description': description,
-                    'is_enabled': is_enabled,
-                    'is_up': is_up,
-                    'last_flapped': -1.0,
-                    'mac_address': mac_address,
-                    'speed': speed}
-            })
+            interfaces.update(
+                {
+                    intf_name: {
+                        "is_up": is_up,
+                        "is_enabled": is_enabled,
+                        "description": description,
+                        "last_flapped": -1.0,
+                        "mtu": intf_mtu,
+                        "speed": speed,
+                        "mac_address": mac_address,
+                    }
+                }
+            )
         return interfaces
 
     # verified
     def get_interfaces_ip(self):
         """
         Get interface IP details. Returns a dictionary of dictionaries.
 
@@ -673,82 +704,77 @@
                         "prefix_length": 64
                     }
                 }
             }
         }
         """
         interfaces_ip = {}
-        output_v4 = self.device.send_command('display ip interface')
-        output_v6 = self.device.send_command('display ipv6 interface')
+        output_v4 = self.device.send_command("display ip interface")
+        output_v6 = self.device.send_command("display ipv6 interface")
 
         v4_interfaces = {}
         separator = r"(^(?!Line protocol).*current state.*$)"
         new_v4_interfaces = self._separate_section(separator, output_v4)
         for interface in new_v4_interfaces:
             re_intf_name_state = r"^(?!Line protocol)(?P<intf_name>\S+).+current state\W+(?P<intf_state>.+)$"
             re_intf_ip = r"Internet Address is\s+(?P<ip_address>\d+.\d+.\d+.\d+)\/(?P<prefix_length>\d+)"
 
             match_intf = re.search(re_intf_name_state, interface, flags=re.M)
             if match_intf is None:
                 msg = "Unexpected interface format: {}".format(interface)
                 raise ValueError(msg)
-            intf_name = match_intf.group('intf_name')
+            intf_name = match_intf.group("intf_name")
             # v4_interfaces[intf_name] = {}
             match_ip = re.findall(re_intf_ip, interface, flags=re.M)
 
             for ip_info in match_ip:
-                val = {'prefix_length': int(ip_info[1])}
+                val = {"prefix_length": int(ip_info[1])}
                 # v4_interfaces[intf_name][ip_info[0]] = val
                 v4_interfaces.setdefault(intf_name, {})[ip_info[0]] = val
 
         v6_interfaces = {}
         separator = r"(^(?!IPv6 protocol).*current state.*$)"
         new_v6_interfaces = self._separate_section(separator, output_v6)
         for interface in new_v6_interfaces:
             re_intf_name_state = r"^(?!IPv6 protocol)(?P<intf_name>\S+).+current state\W+(?P<intf_state>.+)$"
             re_intf_ip = r"(?P<ip_address>\S+), subnet is.+\/(?P<prefix_length>\d+)"
 
             match_intf = re.search(re_intf_name_state, interface, flags=re.M)
             if match_intf is None:
                 msg = "Unexpected interface format: {}".format(interface)
                 raise ValueError(msg)
-            intf_name = match_intf.group('intf_name')
+            intf_name = match_intf.group("intf_name")
             match_ip = re.findall(re_intf_ip, interface, flags=re.M)
 
             for ip_info in match_ip:
-                val = {'prefix_length': int(ip_info[1])}
+                val = {"prefix_length": int(ip_info[1])}
                 v6_interfaces.setdefault(intf_name, {})[ip_info[0]] = val
 
         # Join data from intermediate dictionaries.
         for interface, data in v4_interfaces.items():
-            interfaces_ip.setdefault(interface, {'ipv4': {}})['ipv4'] = data
+            interfaces_ip.setdefault(interface, {"ipv4": {}})["ipv4"] = data
 
         for interface, data in v6_interfaces.items():
-            interfaces_ip.setdefault(interface, {'ipv6': {}})['ipv6'] = data
+            interfaces_ip.setdefault(interface, {"ipv6": {}})["ipv6"] = data
 
         return interfaces_ip
 
-    # verified
     def get_interfaces_counters(self):
         """Return interfaces counters."""
 
-        def process_counts(tup):
-            for item in tup:
-                if item != "":
-                    return int(item)
-            return 0
-
         interfaces = {}
         # command "display interface counters" lacks of some keys
-        output = self.device.send_command('display interface')
+        output = self.device.send_command("display interface")
         if not output:
             return {}
 
         separator = r"(^(?!Line protocol).*current state.*$)"
-        re_intf_name_state = r"^(?!Line protocol)(?P<intf_name>\S+).+current state\W+(?P<intf_state>.+)$"
+        re_intf_name_state = (
+            r"^(?!Line protocol)(?P<intf_name>\S+).+current state\W+(?P<intf_state>.+)$"
+        )
         re_unicast = r"Unicast:\s+(\d+)|(\d+)\s+unicast"
         re_multicast = r"Multicast:\s+(\d+)|(\d+)\s+multicast"
         re_broadcast = r"Broadcast:\s+(\d+)|(\d+)\s+broadcast"
         re_dicards = r"Discard:\s+(\d+)|(\d+)\s+discard"
         re_rx_octets = r"Input.+\s+(\d+)\sbytes|Input:.+,(\d+)\sbytes"
         re_tx_octets = r"Output.+\s+(\d+)\sbytes|Output:.+,(\d+)\sbytes"
         re_errors = r"Total Error:\s+(\d+)|(\d+)\s+errors"
@@ -757,67 +783,39 @@
         for interface in new_interfaces:
             interface = interface.strip()
             match_intf = re.search(re_intf_name_state, interface, flags=re.M)
 
             if match_intf is None:
                 msg = "Unexpected interface format: {}".format(interface)
                 raise ValueError(msg)
-            intf_name = match_intf.group('intf_name')
+
+            intf_name = match_intf.group("intf_name")
+            match_errors = SafeList(re.findall(re_errors, interface, flags=re.M))
+            match_unicast = SafeList(re.findall(re_unicast, interface, flags=re.M))
+            match_multicast = SafeList(re.findall(re_multicast, interface, flags=re.M))
+            match_broadcast = SafeList(re.findall(re_broadcast, interface, flags=re.M))
+            match_discards = SafeList(re.findall(re_dicards, interface, flags=re.M))
+            match_rx_octets = SafeList(re.findall(re_rx_octets, interface, flags=re.M))
+            match_tx_octets = SafeList(re.findall(re_tx_octets, interface, flags=re.M))
             intf_counter = {
-                'tx_errors': 0,
-                'rx_errors': 0,
-                'tx_discards': 0,
-                'rx_discards': 0,
-                'tx_octets': 0,
-                'rx_octets': 0,
-                'tx_unicast_packets': 0,
-                'rx_unicast_packets': 0,
-                'tx_multicast_packets': 0,
-                'rx_multicast_packets': 0,
-                'tx_broadcast_packets': 0,
-                'rx_broadcast_packets': 0
+                "tx_errors": int(match_errors.get_not_none(0, -1)),
+                "rx_errors": int(match_errors.get_not_none(1, -1)),
+                "tx_discards": int(match_discards.get_not_none(0, -1)),
+                "rx_discards": int(match_discards.get_not_none(1, -1)),
+                "tx_octets": int(match_tx_octets.get_not_none(0, -1)),
+                "rx_octets": int(match_rx_octets.get_not_none(0, -1)),
+                "tx_unicast_packets": int(match_unicast.get_not_none(0, -1)),
+                "rx_unicast_packets": int(match_unicast.get_not_none(1, -1)),
+                "tx_multicast_packets": int(match_multicast.get_not_none(0, -1)),
+                "rx_multicast_packets": int(match_multicast.get_not_none(1, -1)),
+                "tx_broadcast_packets": int(match_broadcast.get_not_none(0, -1)),
+                "rx_broadcast_packets": int(match_broadcast.get_not_none(1, -1)),
             }
 
-            match = re.findall(re_errors, interface, flags=re.M)
-            if match:
-                intf_counter['rx_errors'] = process_counts(match[0])
-            if len(match) == 2:
-                intf_counter['tx_errors'] = process_counts(match[1])
-
-            match = re.findall(re_dicards, interface, flags=re.M)
-            if len(match) == 2:
-                intf_counter['rx_discards'] = process_counts(match[0])
-                intf_counter['tx_discards'] = process_counts(match[1])
-
-            match = re.findall(re_unicast, interface, flags=re.M)
-            if len(match) == 2:
-                intf_counter['rx_unicast_packets'] = process_counts(match[0])
-                intf_counter['tx_unicast_packets'] = process_counts(match[1])
-
-            match = re.findall(re_multicast, interface, flags=re.M)
-            if len(match) == 2:
-                intf_counter['rx_multicast_packets'] = process_counts(match[0])
-                intf_counter['tx_multicast_packets'] = process_counts(match[1])
-
-            match = re.findall(re_broadcast, interface, flags=re.M)
-            if len(match) == 2:
-                intf_counter['rx_broadcast_packets'] = process_counts(match[0])
-                intf_counter['tx_broadcast_packets'] = process_counts(match[1])
-
-            match = re.findall(re_rx_octets, interface, flags=re.M)
-            if match:
-                intf_counter['rx_octets'] = process_counts(match[0])
-
-            match = re.findall(re_tx_octets, interface, flags=re.M)
-            if match:
-                intf_counter['tx_octets'] = process_counts(match[0])
-
-            interfaces.update({
-                intf_name: intf_counter
-            })
+            interfaces.update({intf_name: intf_counter})
         return interfaces
 
     # verified
     def get_lldp_neighbors(self):
         """
         Return LLDP neighbors brief info.
 
@@ -845,26 +843,26 @@
                     'hostname': 'Aruba-7210-M',
                     'port': 'GE0/0/2'
                 },
             ]
         }
         """
         results = {}
-        command = 'display lldp neighbor brief'
+        command = "display lldp neighbor brief"
         output = self.device.send_command(command)
         re_lldp = r"(?P<local>\S+)\s+(?P<hostname>\S+)\s+(?P<port>\S+)\s+\d+\s+"
         match = re.findall(re_lldp, output, re.M)
         for neighbor in match:
             local_intf = neighbor[0]
             if local_intf not in results:
                 results[local_intf] = []
 
             neighbor_dict = dict()
-            neighbor_dict['hostname'] = neighbor[1]
-            neighbor_dict['port'] = neighbor[2]
+            neighbor_dict["hostname"] = neighbor[1]
+            neighbor_dict["port"] = neighbor[2]
             results[local_intf].append(neighbor_dict)
         return results
 
     # develop
     def get_lldp_neighbors_detail(self, interface=""):
         pass
         """
@@ -876,55 +874,57 @@
         """
         lldp_neighbors = {}
         return lldp_neighbors
 
     # verified
     def get_arp_table(self, vrf=""):
         """
-                Get arp table information.
+        Get arp table information.
 
-                Return a list of dictionaries having the following set of keys:
-                    * interface (string)
-                    * mac (string)
-                    * ip (string)
-                    * age (float) (not support)
+        Return a list of dictionaries having the following set of keys:
+            * interface (string)
+            * mac (string)
+            * ip (string)
+            * age (float) (not support)
 
-                Sample output:
-                    [
-                        {
-                            'interface' : 'MgmtEth0/RSP0/CPU0/0',
-                            'mac'       : '5c:5e:ab:da:3c:f0',
-                            'ip'        : '172.17.17.1',
-                            'age'       : -1
-                        },
-                        {
-                            'interface': 'MgmtEth0/RSP0/CPU0/0',
-                            'mac'       : '66:0e:94:96:e0:ff',
-                            'ip'        : '172.17.17.2',
-                            'age'       : -1
-                        }
-                    ]
-                """
+        Sample output:
+            [
+                {
+                    'interface' : 'MgmtEth0/RSP0/CPU0/0',
+                    'mac'       : '5c:5e:ab:da:3c:f0',
+                    'ip'        : '172.17.17.1',
+                    'age'       : -1
+                },
+                {
+                    'interface': 'MgmtEth0/RSP0/CPU0/0',
+                    'mac'       : '66:0e:94:96:e0:ff',
+                    'ip'        : '172.17.17.2',
+                    'age'       : -1
+                }
+            ]
+        """
         arp_table = []
-        output = self.device.send_command('display arp')
-        re_arp = r"(?P<ip_address>\d+\.\d+\.\d+\.\d+)\s+(?P<mac>\S+)\s+(?P<exp>\d+|)\s+" \
-                 r"(?P<type>I|D|S|O)\S+\s+(?P<interface>\S+)"
+        output = self.device.send_command("display arp all")
+        re_arp = (
+            r"(?P<ip_address>\d+\.\d+\.\d+\.\d+)\s+(?P<mac>\S+)\s+(?P<exp>\d+|)\s+"
+            r"(?P<type>I|D|S|O)\S+\s+(?P<interface>\S+)"
+        )
         match = re.findall(re_arp, output, flags=re.M)
 
         for arp in match:
             # if arp[2].isdigit():
             #     exp = float(arp[2]) * 60
             # else:
             #     exp = 0
 
             entry = {
-                'interface': arp[4],
-                'mac': pretty_mac(arp[1]),
-                'ip': arp[0],
-                'age': -1.0,
+                "interface": arp[4],
+                "mac": pretty_mac(arp[1]),
+                "ip": arp[0],
+                "age": -1.0,
             }
             arp_table.append(entry)
         return arp_table
 
     # verified
     def get_mac_address_table(self):
         """
@@ -962,34 +962,35 @@
                 mux：        标识MUX MAC表项，当接口使能MUX VLAN功能后，该接口学习到的MAC地址表项会记录到mux类型的MAC地址表项中。
                 snooping：   根据DHCP Snooping绑定表生成的静态MAC表项类型。
                 authen：     已获取到IP地址的NAC认证用户（无法生成MAC地址的三层Portal认证用户和直接转发模式下的无线用户除外）对应的MAC地址表项。
                 pre-authen： 用户使能NAC认证功能后，处于预连接状态且未获取到IP地址的NAC认证用户对应的MAC地址表项。
                 evpn：       标识EVPN网络中存在的MAC地址表项。
         """
         mac_address_table = []
-        command = 'display mac-address'
+        command = "display mac-address"
         output = self.device.send_command(command)
-        re_mac = r"(?P<mac>\S+)\s+(?P<vlan>\d+|-)\S+\s+(?P<interface>\S+)\s+(?P<type>\w+)\s+"
+        re_mac = (
+            r"(?P<mac>\S+)\s+(?P<vlan>\d+|-)\S+\s+(?P<interface>\S+)\s+(?P<type>\w+)\s+"
+        )
         match = re.findall(re_mac, output, re.M)
 
         for mac_info in match:
             mac_dict = {
-                'mac': napalm.base.helpers.mac(mac_info[0]),
-                'interface': mac_info[2],
-                'vlan': int(mac_info[1]),
-                'static': True if mac_info[3] == "static" else False,
-                'active': True if mac_info[3] == "dynamic" else False,
-                'authen': True if mac_info[3] == "authen" else False,
-                'moves': -1,
-                'last_move': -1.0
+                "mac": mac(mac_info[0]),
+                "interface": mac_info[2],
+                "vlan": int(mac_info[1]),
+                "static": True if mac_info[3] == "static" else False,
+                "active": True if mac_info[3] == "dynamic" else False,
+                "authen": True if mac_info[3] == "authen" else False,
+                "moves": -1,
+                "last_move": -1.0,
             }
             mac_address_table.append(mac_dict)
         return mac_address_table
 
-
     # developing
     def get_probes_config(self):
         pass
 
     # developing
     def get_probes_results(self):
         pass
@@ -1016,407 +1017,676 @@
                                 "sent_prefixes": 2
                             }
                         }
                     }
                 }
             }
         }
-        """
+
         bgp_neighbors = {}
 
         command_bgp_peer = "display bgp peer"
-        command_bgp_ipv6 = "display bgp ipv6 peer"
+        # command_bgp_ipv6 = "display bgp ipv6 peer"
         command_bgp_vpnv4 = "display bgp vpnv4 all peer"
         command_bgp_vpnv6 = "display bgp vpnv6 all peer"
         command_bgp_vpntarget = "display bgp vpn-target peer"
 
         output_peer = self.device.send_command(command_bgp_peer)
         output_peer_ipv6 = self.device.send_command(command_bgp_peer)
         output_vpnv4 = self.device.send_command(command_bgp_vpnv4)
         output_vpnv6 = self.device.send_command(command_bgp_vpnv6)
         output_vpntarget = self.device.send_command(command_bgp_vpntarget)
 
-
-        if output_peer == "" and output_vpnv4 == "" and output_vpnv6 == "" and output_peer_ipv6 == "" and \
-            output_vpntarget == "":
+        if (
+            output_peer == ""
+            and output_vpnv4 == ""
+            and output_vpnv6 == ""
+            and output_peer_ipv6 == ""
+            and output_vpntarget == ""
+        ):
             return bgp_neighbors
 
-        #Regular Expressions
+        # Regular Expressions
         re_separator = r"\n\s*(?=VPN-Instance\s+)"
 
         #
         re_global_router_id = r"BGP local router ID :\s+(?P<glob_router_id>\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"
         re_global_local_as = r"Local AS number :\s+(?P<local_as>{})".format(ASN_REGEX)
-        re_vrf_router_id = r"VPN-Instance\s+(?P<vrf>[-_a-zA-Z0-9]+), [rR]outer ID\s+" \
-                              r"(?P<vrf_router_id>\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"
-        re_peers = r"(?P<peer_ip>({})|({}))\s+(?P<bgp_version>\d)\s+" \
-                   r"(?P<as>{})\s+\d+\s+\d+\s+\d+\s+(?P<updown_time>[a-zA-Z0-9:]+)\s+" \
-                   r"(?P<state>[a-zA-Z0-9\(\)]+)\s+(?P<received_prefixes>\d+)".format(
-                            IPV4_ADDR_REGEX, IPV6_ADDR_REGEX, ASN_REGEX)
+        re_vrf_router_id = (
+            r"VPN-Instance\s+(?P<vrf>[-_a-zA-Z0-9]+), [rR]outer ID\s+"
+            r"(?P<vrf_router_id>\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"
+        )
+        re_peers = (
+            r"(?P<peer_ip>({})|({}))\s+(?P<bgp_version>\d)\s+"
+            r"(?P<as>{})\s+\d+\s+\d+\s+\d+\s+(?P<updown_time>[a-zA-Z0-9:]+)\s+"
+            r"(?P<state>[a-zA-Z0-9\(\)]+)\s+(?P<received_prefixes>\d+)".format(
+                IPV4_ADDR_REGEX, IPV6_ADDR_REGEX, ASN_REGEX
+            )
+        )
 
         re_remote_rid = r"Remote router ID\s+(?P<remote_rid>{})".format(IPV4_ADDR_REGEX)
         re_peer_description = r"Peer's description:\s+\"(?P<peer_description>.*)\""
         re_advertised_routes = r"Advertised total routes:\s*(?P<sent_prefixes>\d+)"
 
-
         if output_peer != "":
-
             bgp_global_router_id = ""
             bgp_global_local_as = ""
 
-            match_afi = re.search(re_global_router_id,output_peer, flags=re.M)
-            match_local_as = re.search(re_global_local_as,output_peer, flags=re.M)
+            match_afi = re.search(re_global_router_id, output_peer, flags=re.M)
+            match_local_as = re.search(re_global_local_as, output_peer, flags=re.M)
             if match_afi is not None:
-                bgp_global_router_id = match_afi.group('glob_router_id')
-                bgp_global_local_as = match_local_as.group('local_as')
+                bgp_global_router_id = match_afi.group("glob_router_id")
+                bgp_global_local_as = match_local_as.group("local_as")
 
-            #IPv4 Unicast y IPv6 Unicas Peerings
-            bgp_neighbors.update({"global": {"router_id": bgp_global_router_id, "peers" : {}}})
+            # IPv4 Unicast y IPv6 Unicas Peerings
+            bgp_neighbors.update(
+                {"global": {"router_id": bgp_global_router_id, "peers": {}}}
+            )
 
             for peer in output_peer.splitlines():
-
                 match_peer = re.search(re_peers, peer, flags=re.M)
-                
+
                 if match_peer:
+                    peer_bgp_command = "display bgp peer {} verbose".format(
+                        match_peer.group("peer_ip")
+                    )
 
-                    peer_bgp_command = "display bgp peer {} verbose".format(match_peer.group('peer_ip'))
-                    
-                    #Send Display BGP Peer Vervose
+                    # Send Display BGP Peer Vervose
                     peer_detail = self.device.send_command(peer_bgp_command)
 
                     match_remote_rid = re.search(re_remote_rid, peer_detail, flags=re.M)
-                    match_peer_description = re.search(re_peer_description, peer_detail, flags=re.M)
-                    match_advertised_routes = re.search(re_advertised_routes, peer_detail, flags=re.M)
+                    match_peer_description = re.search(
+                        re_peer_description, peer_detail, flags=re.M
+                    )
+                    match_advertised_routes = re.search(
+                        re_advertised_routes, peer_detail, flags=re.M
+                    )
 
-                    bgp_neighbors["global"]["peers"].update( { 
-                    match_peer.group('peer_ip'): { 
-                    "local_as": int(bgp_global_local_as), 
-                    "remote_as": int(match_peer.group('as')), 
-                    "remote_id": "" if match_remote_rid is None else match_remote_rid.group('remote_rid'), 
-                    "is_up": True if "Established" in match_peer.group('state') else False, 
-                    "is_enabled": False if "Admin" in match_peer.group('state') else True, 
-                    "description": "" if match_peer_description is None else match_peer_description.group('peer_description'), 
-                    "uptime": int(self.bgp_time_conversion(match_peer.group('updown_time'))), 
-                    "address_family": { 
-                            "ipv4 unicast": { 
-                            "is_up": True if "Established" in match_peer.group('state') else False,
-                            "received_prefixes": int(match_peer.group('received_prefixes')), 
-                            "accepted_prefixes": -1, 
-                            "sent_prefixes": int(match_advertised_routes.group('sent_prefixes')) if match_advertised_routes is not None else "Unknown", 
-                                        }
+                    bgp_neighbors["global"]["peers"].update(
+                        {
+                            match_peer.group("peer_ip"): {
+                                "local_as": int(bgp_global_local_as),
+                                "remote_as": int(match_peer.group("as")),
+                                "remote_id": ""
+                                if match_remote_rid is None
+                                else match_remote_rid.group("remote_rid"),
+                                "is_up": True
+                                if "Established" in match_peer.group("state")
+                                else False,
+                                "is_enabled": False
+                                if "Admin" in match_peer.group("state")
+                                else True,
+                                "description": ""
+                                if match_peer_description is None
+                                else match_peer_description.group("peer_description"),
+                                "uptime": int(
+                                    self.bgp_time_conversion(
+                                        match_peer.group("updown_time")
+                                    )
+                                ),
+                                "address_family": {
+                                    "ipv4 unicast": {
+                                        "is_up": True
+                                        if "Established" in match_peer.group("state")
+                                        else False,
+                                        "received_prefixes": int(
+                                            match_peer.group("received_prefixes")
+                                        ),
+                                        "accepted_prefixes": -1,
+                                        "sent_prefixes": int(
+                                            match_advertised_routes.group(
+                                                "sent_prefixes"
+                                            )
+                                        )
+                                        if match_advertised_routes is not None
+                                        else "Unknown",
                                     }
+                                },
                             }
-                        })
+                        }
+                    )
         if output_vpnv4 != "":
-
             if output_peer == "":
                 bgp_global_router_id = ""
                 bgp_global_local_as = ""
 
-                match_afi = re.search(re_global_router_id,output_vpnv4, flags=re.M)
-                match_local_as = re.search(re_global_local_as,output_vpnv4, flags=re.M)
+                match_afi = re.search(re_global_router_id, output_vpnv4, flags=re.M)
+                match_local_as = re.search(re_global_local_as, output_vpnv4, flags=re.M)
                 if match_afi is not None:
-                    bgp_global_router_id = match_afi.group('glob_router_id')
-                    bgp_global_local_as = match_local_as.group('local_as')
+                    bgp_global_router_id = match_afi.group("glob_router_id")
+                    bgp_global_local_as = match_local_as.group("local_as")
 
-                #IPv4 Unicast y IPv6 Unicas Peerings
-                bgp_neighbors.update({"global": {"router_id": bgp_global_router_id, "peers" : {}}})
+                # IPv4 Unicast y IPv6 Unicas Peerings
+                bgp_neighbors.update(
+                    {"global": {"router_id": bgp_global_router_id, "peers": {}}}
+                )
 
-            #Separation of AFIs VPNv4
+            # Separation of AFIs VPNv4
             afi_list = re.split(re_separator, output_vpnv4, flags=re.M)
-            #       
+            #
             for vpn_peers in afi_list:
- 
                 if "VPN-Instance " not in vpn_peers:
                     for peer in vpn_peers.splitlines():
-                        match_peer = re.search(re_peers,peer, flags=re.M)
+                        match_peer = re.search(re_peers, peer, flags=re.M)
                         if match_peer:
-
-                            peer_bgp_command = "display bgp vpnv4 all peer {} verbose".format(match_peer.group('peer_ip'))            
+                            peer_bgp_command = (
+                                "display bgp vpnv4 all peer {} verbose".format(
+                                    match_peer.group("peer_ip")
+                                )
+                            )
                             peer_detail = self.device.send_command(peer_bgp_command)
-                            match_advertised_routes = re.search(re_advertised_routes, peer_detail, flags=re.M)
-
-                            #If the Peer Already Exist, just add the info of the new vpnv4.
-                            if match_peer.group('peer_ip') in bgp_neighbors["global"]["peers"]:
-                                bgp_neighbors["global"]["peers"][match_peer.group('peer_ip')]["address_family"].update(
-                                { 
-                                    "vpnv4 unicast": { 
-                                    "is_up": True if "Established" in match_peer.group('state') else False,
-                                    "received_prefixes": int(match_peer.group('received_prefixes')), 
-                                    "accepted_prefixes": -1, 
-                                    "sent_prefixes": int(match_advertised_routes.group('sent_prefixes')) if match_advertised_routes is not None else "Unknown"
-                                                }
-                                            }
-                                ) 
+                            match_advertised_routes = re.search(
+                                re_advertised_routes, peer_detail, flags=re.M
+                            )
+
+                            # If the Peer Already Exist, just add the info of the new vpnv4.
+                            if (
+                                match_peer.group("peer_ip")
+                                in bgp_neighbors["global"]["peers"]
+                            ):
+                                bgp_neighbors["global"]["peers"][
+                                    match_peer.group("peer_ip")
+                                ]["address_family"].update(
+                                    {
+                                        "vpnv4 unicast": {
+                                            "is_up": True
+                                            if "Established"
+                                            in match_peer.group("state")
+                                            else False,
+                                            "received_prefixes": int(
+                                                match_peer.group("received_prefixes")
+                                            ),
+                                            "accepted_prefixes": -1,
+                                            "sent_prefixes": int(
+                                                match_advertised_routes.group(
+                                                    "sent_prefixes"
+                                                )
+                                            )
+                                            if match_advertised_routes is not None
+                                            else "Unknown",
+                                        }
+                                    }
+                                )
                             else:
-
-                                match_remote_rid = re.search(re_remote_rid, peer_detail, flags=re.M)
-                                match_peer_description = re.search(re_peer_description, peer_detail, flags=re.M)
-                                
-                                bgp_neighbors["global"]["peers"].update( { 
-                                match_peer.group('peer_ip'): { 
-                                "local_as": int(bgp_global_local_as), 
-                                "remote_as": int(match_peer.group('as')), 
-                                "remote_id": "" if match_remote_rid is None else match_remote_rid.group('remote_rid'), 
-                                "is_up": True if "Established" in match_peer.group('state') else False, 
-                                "is_enabled": False if "Admin" in match_peer.group('state') else True, 
-                                "description": "" if match_peer_description is None else match_peer_description.group('peer_description'), 
-                                "uptime": int(self.bgp_time_conversion(match_peer.group('updown_time'))), 
-                                "address_family": { 
-                                    "vpnv4 unicast": { 
-                                        "is_up": True if "Established" in match_peer.group('state') else False,
-                                        "received_prefixes": int(match_peer.group('received_prefixes')), 
-                                        "accepted_prefixes": -1, 
-                                        "sent_prefixes": int(match_advertised_routes.group('sent_prefixes')) if match_advertised_routes is not None else "Unknown"
-                                                    }
+                                match_remote_rid = re.search(
+                                    re_remote_rid, peer_detail, flags=re.M
+                                )
+                                match_peer_description = re.search(
+                                    re_peer_description, peer_detail, flags=re.M
+                                )
+
+                                bgp_neighbors["global"]["peers"].update(
+                                    {
+                                        match_peer.group("peer_ip"): {
+                                            "local_as": int(bgp_global_local_as),
+                                            "remote_as": int(match_peer.group("as")),
+                                            "remote_id": ""
+                                            if match_remote_rid is None
+                                            else match_remote_rid.group("remote_rid"),
+                                            "is_up": True
+                                            if "Established"
+                                            in match_peer.group("state")
+                                            else False,
+                                            "is_enabled": False
+                                            if "Admin" in match_peer.group("state")
+                                            else True,
+                                            "description": ""
+                                            if match_peer_description is None
+                                            else match_peer_description.group(
+                                                "peer_description"
+                                            ),
+                                            "uptime": int(
+                                                self.bgp_time_conversion(
+                                                    match_peer.group("updown_time")
+                                                )
+                                            ),
+                                            "address_family": {
+                                                "vpnv4 unicast": {
+                                                    "is_up": True
+                                                    if "Established"
+                                                    in match_peer.group("state")
+                                                    else False,
+                                                    "received_prefixes": int(
+                                                        match_peer.group(
+                                                            "received_prefixes"
+                                                        )
+                                                    ),
+                                                    "accepted_prefixes": -1,
+                                                    "sent_prefixes": int(
+                                                        match_advertised_routes.group(
+                                                            "sent_prefixes"
+                                                        )
+                                                    )
+                                                    if match_advertised_routes
+                                                    is not None
+                                                    else "Unknown",
                                                 }
+                                            },
                                         }
-                                    })
+                                    }
+                                )
                 else:
-                    match_vrf_router_id = re.search(re_vrf_router_id, vpn_peers, flags=re.M)
+                    match_vrf_router_id = re.search(
+                        re_vrf_router_id, vpn_peers, flags=re.M
+                    )
 
                     if match_vrf_router_id is None:
                         msg = "No Match Found"
                         raise ValueError(msg)
 
-                    peer_vpn_instance = match_vrf_router_id.group('vrf')
-                    peer_router_id = match_vrf_router_id.group('vrf_router_id')
+                    peer_vpn_instance = match_vrf_router_id.group("vrf")
+                    peer_router_id = match_vrf_router_id.group("vrf_router_id")
 
-                    bgp_neighbors.update({peer_vpn_instance: {
-                                    "router_id": peer_router_id, "peers" : {}}})
+                    bgp_neighbors.update(
+                        {peer_vpn_instance: {"router_id": peer_router_id, "peers": {}}}
+                    )
 
                     for peer in vpn_peers.splitlines():
-                                
                         match_peer = re.search(re_peers, peer, flags=re.M)
                         if match_peer:
-
                             peer_bgp_command = ""
                             afi_vrf = ""
-                            peer_bgp_command = "display bgp vpnv4 vpn-instance {} peer {} verbose".format(peer_vpn_instance, match_peer.group('peer_ip'))
+                            peer_bgp_command = "display bgp vpnv4 vpn-instance {} peer {} verbose".format(
+                                peer_vpn_instance, match_peer.group("peer_ip")
+                            )
                             afi_vrf = "ipv4 unicast"
-                            
+
                             peer_detail = self.device.send_command(peer_bgp_command)
 
-                            match_remote_rid = re.search(re_remote_rid, peer_detail, flags=re.M)
-                            match_peer_description = re.search(re_peer_description, peer_detail, flags=re.M)
-                            match_advertised_routes = re.search(re_advertised_routes, peer_detail, flags=re.M)
-
-                            bgp_neighbors[peer_vpn_instance]["peers"].update( { 
-                            match_peer.group('peer_ip'): { 
-                            "local_as": int(bgp_global_local_as), 
-                            "remote_as": int(match_peer.group('as')), 
-                            "remote_id": "" if match_remote_rid is None else match_remote_rid.group('remote_rid'), 
-                            "is_up": True if "Established" in match_peer.group('state') else False, 
-                            "is_enabled": False if "Admin" in match_peer.group('state') else True, 
-                            "description": "" if match_peer_description is None else match_peer_description.group('peer_description'), 
-                            "uptime": int(self.bgp_time_conversion(match_peer.group('updown_time'))),         
-                            "address_family": { 
-                                afi_vrf: { 
-                                    "is_up": True if "Established" in match_peer.group('state') else False,
-                                    "received_prefixes": int(match_peer.group('received_prefixes')), 
-                                    "accepted_prefixes": -1, 
-                                    "sent_prefixes": int(match_advertised_routes.group('sent_prefixes')) if match_advertised_routes is not None else "Unknown"
+                            match_remote_rid = re.search(
+                                re_remote_rid, peer_detail, flags=re.M
+                            )
+                            match_peer_description = re.search(
+                                re_peer_description, peer_detail, flags=re.M
+                            )
+                            match_advertised_routes = re.search(
+                                re_advertised_routes, peer_detail, flags=re.M
+                            )
+
+                            bgp_neighbors[peer_vpn_instance]["peers"].update(
+                                {
+                                    match_peer.group("peer_ip"): {
+                                        "local_as": int(bgp_global_local_as),
+                                        "remote_as": int(match_peer.group("as")),
+                                        "remote_id": ""
+                                        if match_remote_rid is None
+                                        else match_remote_rid.group("remote_rid"),
+                                        "is_up": True
+                                        if "Established" in match_peer.group("state")
+                                        else False,
+                                        "is_enabled": False
+                                        if "Admin" in match_peer.group("state")
+                                        else True,
+                                        "description": ""
+                                        if match_peer_description is None
+                                        else match_peer_description.group(
+                                            "peer_description"
+                                        ),
+                                        "uptime": int(
+                                            self.bgp_time_conversion(
+                                                match_peer.group("updown_time")
+                                            )
+                                        ),
+                                        "address_family": {
+                                            afi_vrf: {
+                                                "is_up": True
+                                                if "Established"
+                                                in match_peer.group("state")
+                                                else False,
+                                                "received_prefixes": int(
+                                                    match_peer.group(
+                                                        "received_prefixes"
+                                                    )
+                                                ),
+                                                "accepted_prefixes": -1,
+                                                "sent_prefixes": int(
+                                                    match_advertised_routes.group(
+                                                        "sent_prefixes"
+                                                    )
+                                                )
+                                                if match_advertised_routes is not None
+                                                else "Unknown",
                                             }
-                                        }
+                                        },
                                     }
-                            })
+                                }
+                            )
 
         if output_vpnv6 != "":
             if output_peer == "" and output_vpnv4 == "":
                 bgp_global_router_id = ""
                 bgp_global_local_as = ""
 
-                match_afi = re.search(re_global_router_id,output_vpnv6, flags=re.M)
-                match_local_as = re.search(re_global_local_as,output_vpnv6, flags=re.M)
+                match_afi = re.search(re_global_router_id, output_vpnv6, flags=re.M)
+                match_local_as = re.search(re_global_local_as, output_vpnv6, flags=re.M)
                 if match_afi is not None:
-                    bgp_global_router_id = match_afi.group('glob_router_id')
-                    bgp_global_local_as = match_local_as.group('local_as')
+                    bgp_global_router_id = match_afi.group("glob_router_id")
+                    bgp_global_local_as = match_local_as.group("local_as")
 
-                #IPv4 Unicast y IPv6 Unicas Peerings
-                bgp_neighbors.update({"global": {"router_id": bgp_global_router_id, "peers" : {}}})
+                # IPv4 Unicast y IPv6 Unicas Peerings
+                bgp_neighbors.update(
+                    {"global": {"router_id": bgp_global_router_id, "peers": {}}}
+                )
 
             afi_list = re.split(re_separator, output_vpnv6, flags=re.M)
 
-            #       
+            #
             for vpn_peers in afi_list:
- 
                 if "VPN-Instance " not in vpn_peers:
                     for peer in vpn_peers.splitlines():
-                        match_peer = re.search(re_peers,peer, flags=re.M)
+                        match_peer = re.search(re_peers, peer, flags=re.M)
                         if match_peer:
-
-                            peer_bgp_command = "display bgp vpnv6 all peer {} verbose".format(match_peer.group('peer_ip'))            
+                            peer_bgp_command = (
+                                "display bgp vpnv6 all peer {} verbose".format(
+                                    match_peer.group("peer_ip")
+                                )
+                            )
                             peer_detail = self.device.send_command(peer_bgp_command)
-                            match_advertised_routes = re.search(re_advertised_routes, peer_detail, flags=re.M)
-
-                            #If the Peer Already Exist, just add the info of the new vpnv6.
-                            if match_peer.group('peer_ip') in bgp_neighbors["global"]["peers"]:
-                                bgp_neighbors["global"]["peers"][match_peer.group('peer_ip')]["address_family"].update(
-                                { 
-                                    "vpnv6 unicast": {
-                                    "is_up": True if "Established" in match_peer.group('state') else False, 
-                                    "received_prefixes": int(match_peer.group('received_prefixes')), 
-                                    "accepted_prefixes": -1, 
-                                    "sent_prefixes": int(match_advertised_routes.group('sent_prefixes')) if match_advertised_routes is not None else "Unknown"
-                                                }
-                                            }
-                                ) 
+                            match_advertised_routes = re.search(
+                                re_advertised_routes, peer_detail, flags=re.M
+                            )
+
+                            # If the Peer Already Exist, just add the info of the new vpnv6.
+                            if (
+                                match_peer.group("peer_ip")
+                                in bgp_neighbors["global"]["peers"]
+                            ):
+                                bgp_neighbors["global"]["peers"][
+                                    match_peer.group("peer_ip")
+                                ]["address_family"].update(
+                                    {
+                                        "vpnv6 unicast": {
+                                            "is_up": True
+                                            if "Established"
+                                            in match_peer.group("state")
+                                            else False,
+                                            "received_prefixes": int(
+                                                match_peer.group("received_prefixes")
+                                            ),
+                                            "accepted_prefixes": -1,
+                                            "sent_prefixes": int(
+                                                match_advertised_routes.group(
+                                                    "sent_prefixes"
+                                                )
+                                            )
+                                            if match_advertised_routes is not None
+                                            else "Unknown",
+                                        }
+                                    }
+                                )
                             else:
-
-                                match_remote_rid = re.search(re_remote_rid, peer_detail, flags=re.M)
-                                match_peer_description = re.search(re_peer_description, peer_detail, flags=re.M)
-                                
-                                bgp_neighbors["global"]["peers"].update( { 
-                                match_peer.group('peer_ip'): { 
-                                "local_as": int(bgp_global_local_as), 
-                                "remote_as": int(match_peer.group('as')), 
-                                "remote_id": "" if match_remote_rid is None else match_remote_rid.group('remote_rid'), 
-                                "is_up": True if "Established" in match_peer.group('state') else False, 
-                                "is_enabled": False if "Admin" in match_peer.group('state') else True, 
-                                "description": "" if match_peer_description is None else match_peer_description.group('peer_description'), 
-                                "uptime": int(self.bgp_time_conversion(match_peer.group('updown_time'))), 
-                                "address_family": { 
-                                    "vpnv4 unicast": { 
-                                        "is_up": True if "Established" in match_peer.group('state') else False,
-                                        "received_prefixes": int(match_peer.group('received_prefixes')), 
-                                        "accepted_prefixes": -1, 
-                                        "sent_prefixes": int(match_advertised_routes.group('sent_prefixes')) if match_advertised_routes is not None else "Unknown"
-                                                    }
+                                match_remote_rid = re.search(
+                                    re_remote_rid, peer_detail, flags=re.M
+                                )
+                                match_peer_description = re.search(
+                                    re_peer_description, peer_detail, flags=re.M
+                                )
+
+                                bgp_neighbors["global"]["peers"].update(
+                                    {
+                                        match_peer.group("peer_ip"): {
+                                            "local_as": int(bgp_global_local_as),
+                                            "remote_as": int(match_peer.group("as")),
+                                            "remote_id": ""
+                                            if match_remote_rid is None
+                                            else match_remote_rid.group("remote_rid"),
+                                            "is_up": True
+                                            if "Established"
+                                            in match_peer.group("state")
+                                            else False,
+                                            "is_enabled": False
+                                            if "Admin" in match_peer.group("state")
+                                            else True,
+                                            "description": ""
+                                            if match_peer_description is None
+                                            else match_peer_description.group(
+                                                "peer_description"
+                                            ),
+                                            "uptime": int(
+                                                self.bgp_time_conversion(
+                                                    match_peer.group("updown_time")
+                                                )
+                                            ),
+                                            "address_family": {
+                                                "vpnv4 unicast": {
+                                                    "is_up": True
+                                                    if "Established"
+                                                    in match_peer.group("state")
+                                                    else False,
+                                                    "received_prefixes": int(
+                                                        match_peer.group(
+                                                            "received_prefixes"
+                                                        )
+                                                    ),
+                                                    "accepted_prefixes": -1,
+                                                    "sent_prefixes": int(
+                                                        match_advertised_routes.group(
+                                                            "sent_prefixes"
+                                                        )
+                                                    )
+                                                    if match_advertised_routes
+                                                    is not None
+                                                    else "Unknown",
                                                 }
+                                            },
                                         }
-                                    })
+                                    }
+                                )
                 else:
-                    match_vrf_router_id = re.search(re_vrf_router_id, vpn_peers, flags=re.M)
+                    match_vrf_router_id = re.search(
+                        re_vrf_router_id, vpn_peers, flags=re.M
+                    )
 
                     if match_vrf_router_id is None:
                         msg = "No Match Found"
                         raise ValueError(msg)
 
-                    peer_vpn_instance = match_vrf_router_id.group('vrf')
-                    peer_router_id = match_vrf_router_id.group('vrf_router_id')
+                    peer_vpn_instance = match_vrf_router_id.group("vrf")
+                    peer_router_id = match_vrf_router_id.group("vrf_router_id")
 
-                    bgp_neighbors.update({peer_vpn_instance: {
-                                    "router_id": peer_router_id, "peers" : {}}})
+                    bgp_neighbors.update(
+                        {peer_vpn_instance: {"router_id": peer_router_id, "peers": {}}}
+                    )
 
                     for peer in vpn_peers.splitlines():
-                                
                         match_peer = re.search(re_peers, peer, flags=re.M)
                         if match_peer:
-
                             peer_bgp_command = ""
                             afi_vrf = ""
-                            peer_bgp_command = "display bgp vpnv6 vpn-instance {} peer {} verbose".format(peer_vpn_instance, match_peer.group('peer_ip'))
+                            peer_bgp_command = "display bgp vpnv6 vpn-instance {} peer {} verbose".format(
+                                peer_vpn_instance, match_peer.group("peer_ip")
+                            )
                             afi_vrf = "ipv6 unicast"
-                            
+
                             peer_detail = self.device.send_command(peer_bgp_command)
 
-                            match_remote_rid = re.search(re_remote_rid, peer_detail, flags=re.M)
-                            match_peer_description = re.search(re_peer_description, peer_detail, flags=re.M)
-                            match_advertised_routes = re.search(re_advertised_routes, peer_detail, flags=re.M)
-
-                            bgp_neighbors[peer_vpn_instance]["peers"].update( { 
-                            match_peer.group('peer_ip'): { 
-                            "local_as": int(bgp_global_local_as), 
-                            "remote_as": int(match_peer.group('as')), 
-                            "remote_id": "" if match_remote_rid is None else match_remote_rid.group('remote_rid'), 
-                            "is_up": True if "Established" in match_peer.group('state') else False, 
-                            "is_enabled": False if "Admin" in match_peer.group('state') else True, 
-                            "description": "" if match_peer_description is None else match_peer_description.group('peer_description'), 
-                            "uptime": int(self.bgp_time_conversion(match_peer.group('updown_time'))),         
-                            "address_family": { 
-                                afi_vrf: { 
-                                    "is_up": True if "Established" in match_peer.group('state') else False,
-                                    "received_prefixes": int(match_peer.group('received_prefixes')), 
-                                    "accepted_prefixes": -1, 
-                                    "sent_prefixes": int(match_advertised_routes.group('sent_prefixes')) if match_advertised_routes is not None else "Unknown"
+                            match_remote_rid = re.search(
+                                re_remote_rid, peer_detail, flags=re.M
+                            )
+                            match_peer_description = re.search(
+                                re_peer_description, peer_detail, flags=re.M
+                            )
+                            match_advertised_routes = re.search(
+                                re_advertised_routes, peer_detail, flags=re.M
+                            )
+
+                            bgp_neighbors[peer_vpn_instance]["peers"].update(
+                                {
+                                    match_peer.group("peer_ip"): {
+                                        "local_as": int(bgp_global_local_as),
+                                        "remote_as": int(match_peer.group("as")),
+                                        "remote_id": ""
+                                        if match_remote_rid is None
+                                        else match_remote_rid.group("remote_rid"),
+                                        "is_up": True
+                                        if "Established" in match_peer.group("state")
+                                        else False,
+                                        "is_enabled": False
+                                        if "Admin" in match_peer.group("state")
+                                        else True,
+                                        "description": ""
+                                        if match_peer_description is None
+                                        else match_peer_description.group(
+                                            "peer_description"
+                                        ),
+                                        "uptime": int(
+                                            self.bgp_time_conversion(
+                                                match_peer.group("updown_time")
+                                            )
+                                        ),
+                                        "address_family": {
+                                            afi_vrf: {
+                                                "is_up": True
+                                                if "Established"
+                                                in match_peer.group("state")
+                                                else False,
+                                                "received_prefixes": int(
+                                                    match_peer.group(
+                                                        "received_prefixes"
+                                                    )
+                                                ),
+                                                "accepted_prefixes": -1,
+                                                "sent_prefixes": int(
+                                                    match_advertised_routes.group(
+                                                        "sent_prefixes"
+                                                    )
+                                                )
+                                                if match_advertised_routes is not None
+                                                else "Unknown",
                                             }
-                                        }
+                                        },
                                     }
-                            })
+                                }
+                            )
 
         if output_vpntarget != "":
-    
             if output_peer == "" and output_vpnv4 == "" and output_vpnv6 == "":
                 bgp_global_router_id = ""
                 bgp_global_local_as = ""
 
-                match_afi = re.search(re_global_router_id,output_vpnv6, flags=re.M)
-                match_local_as = re.search(re_global_local_as,output_vpnv6, flags=re.M)
+                match_afi = re.search(re_global_router_id, output_vpnv6, flags=re.M)
+                match_local_as = re.search(re_global_local_as, output_vpnv6, flags=re.M)
                 if match_afi is not None:
-                    bgp_global_router_id = match_afi.group('glob_router_id')
-                    bgp_global_local_as = match_local_as.group('local_as')
+                    bgp_global_router_id = match_afi.group("glob_router_id")
+                    bgp_global_local_as = match_local_as.group("local_as")
 
-                #IPv4 Unicast y IPv6 Unicas Peerings
-                bgp_neighbors.update({"global": {"router_id": bgp_global_router_id, "peers" : {}}})
+                # IPv4 Unicast y IPv6 Unicas Peerings
+                bgp_neighbors.update(
+                    {"global": {"router_id": bgp_global_router_id, "peers": {}}}
+                )
 
-            match_afi = re.search(re_global_router_id,output_vpntarget, flags=re.M)
-            match_local_as = re.search(re_global_local_as,output_vpntarget, flags=re.M)
+            match_afi = re.search(re_global_router_id, output_vpntarget, flags=re.M)
+            match_local_as = re.search(re_global_local_as, output_vpntarget, flags=re.M)
 
             if match_afi is not None:
-                bgp_global_router_id = match_afi.group('glob_router_id')
-                bgp_global_local_as = match_local_as.group('local_as')
+                bgp_global_router_id = match_afi.group("glob_router_id")
+                bgp_global_local_as = match_local_as.group("local_as")
 
-            #IPv4 VPN-Target 
-            #bgp_neighbors.update({"global": {"router_id": bgp_global_router_id, "peers" : {}}})
+            # IPv4 VPN-Target
+            # bgp_neighbors.update({"global": {"router_id": bgp_global_router_id, "peers" : {}}})
 
             for peer in output_vpntarget.splitlines():
-
                 match_peer = re.search(re_peers, peer, flags=re.M)
-                
+
                 if match_peer:
+                    peer_bgp_command = "display bgp vpn-target peer {} verbose".format(
+                        match_peer.group("peer_ip")
+                    )
 
-                    peer_bgp_command = "display bgp vpn-target peer {} verbose".format(match_peer.group('peer_ip'))
-                    
-                    #Send Display BGP Peer Vervose
+                    # Send Display BGP Peer Vervose
                     peer_detail = self.device.send_command(peer_bgp_command)
 
                     match_remote_rid = re.search(re_remote_rid, peer_detail, flags=re.M)
-                    match_peer_description = re.search(re_peer_description, peer_detail, flags=re.M)
-                    match_advertised_routes = re.search(re_advertised_routes, peer_detail, flags=re.M)
-
-
-
-                    #If the Peer Already Exist, just add the info of the new vpnv4.
-                    if match_peer.group('peer_ip') in bgp_neighbors["global"]["peers"]:
-                        bgp_neighbors["global"]["peers"][match_peer.group('peer_ip')]["address_family"].update(
-                        { 
-                            "vpn_target": { 
-                            "is_up": True if "Established" in match_peer.group('state') else False,
-                            "received_prefixes": int(match_peer.group('received_prefixes')), 
-                            "accepted_prefixes": -1, 
-                            "sent_prefixes": int(match_advertised_routes.group('sent_prefixes')) if match_advertised_routes is not None else "Unknown"
-                                        }
-                                    }
-                        ) 
+                    match_peer_description = re.search(
+                        re_peer_description, peer_detail, flags=re.M
+                    )
+                    match_advertised_routes = re.search(
+                        re_advertised_routes, peer_detail, flags=re.M
+                    )
+
+                    # If the Peer Already Exist, just add the info of the new vpnv4.
+                    if match_peer.group("peer_ip") in bgp_neighbors["global"]["peers"]:
+                        bgp_neighbors["global"]["peers"][match_peer.group("peer_ip")][
+                            "address_family"
+                        ].update(
+                            {
+                                "vpn_target": {
+                                    "is_up": True
+                                    if "Established" in match_peer.group("state")
+                                    else False,
+                                    "received_prefixes": int(
+                                        match_peer.group("received_prefixes")
+                                    ),
+                                    "accepted_prefixes": -1,
+                                    "sent_prefixes": int(
+                                        match_advertised_routes.group("sent_prefixes")
+                                    )
+                                    if match_advertised_routes is not None
+                                    else "Unknown",
+                                }
+                            }
+                        )
                     else:
-
-                        match_remote_rid = re.search(re_remote_rid, peer_detail, flags=re.M)
-                        match_peer_description = re.search(re_peer_description, peer_detail, flags=re.M)
-                        
-                        bgp_neighbors["global"]["peers"].update( { 
-                        match_peer.group('peer_ip'): { 
-                        "local_as": int(bgp_global_local_as), 
-                        "remote_as": int(match_peer.group('as')), 
-                        "remote_id": "" if match_remote_rid is None else match_remote_rid.group('remote_rid'), 
-                        "is_up": True if "Established" in match_peer.group('state') else False, 
-                        "is_enabled": False if "Admin" in match_peer.group('state') else True, 
-                        "description": "" if match_peer_description is None else match_peer_description.group('peer_description'), 
-                        "uptime": int(self.bgp_time_conversion(match_peer.group('updown_time'))), 
-                        "address_family": { 
-                            "vpn_target": { 
-                                "is_up": True if "Established" in match_peer.group('state') else False,
-                                "received_prefixes": int(match_peer.group('received_prefixes')), 
-                                "accepted_prefixes": -1, 
-                                "sent_prefixes": int(match_advertised_routes.group('sent_prefixes')) if match_advertised_routes is not None else "Unknown"
-                                            }
+                        match_remote_rid = re.search(
+                            re_remote_rid, peer_detail, flags=re.M
+                        )
+                        match_peer_description = re.search(
+                            re_peer_description, peer_detail, flags=re.M
+                        )
+
+                        bgp_neighbors["global"]["peers"].update(
+                            {
+                                match_peer.group("peer_ip"): {
+                                    "local_as": int(bgp_global_local_as),
+                                    "remote_as": int(match_peer.group("as")),
+                                    "remote_id": ""
+                                    if match_remote_rid is None
+                                    else match_remote_rid.group("remote_rid"),
+                                    "is_up": True
+                                    if "Established" in match_peer.group("state")
+                                    else False,
+                                    "is_enabled": False
+                                    if "Admin" in match_peer.group("state")
+                                    else True,
+                                    "description": ""
+                                    if match_peer_description is None
+                                    else match_peer_description.group(
+                                        "peer_description"
+                                    ),
+                                    "uptime": int(
+                                        self.bgp_time_conversion(
+                                            match_peer.group("updown_time")
+                                        )
+                                    ),
+                                    "address_family": {
+                                        "vpn_target": {
+                                            "is_up": True
+                                            if "Established"
+                                            in match_peer.group("state")
+                                            else False,
+                                            "received_prefixes": int(
+                                                match_peer.group("received_prefixes")
+                                            ),
+                                            "accepted_prefixes": -1,
+                                            "sent_prefixes": int(
+                                                match_advertised_routes.group(
+                                                    "sent_prefixes"
+                                                )
+                                            )
+                                            if match_advertised_routes is not None
+                                            else "Unknown",
                                         }
+                                    },
                                 }
-                            })
+                            }
+                        )
 
         return bgp_neighbors
+        """
+        pass
 
     # develop
     def get_bgp_neighbors_detail(self):
         pass
 
     # develop
     def get_bgp_config(self):
@@ -1446,38 +1716,40 @@
                 'disper': '1.41 ms'
             }
         ]
         """
         ntp_peer = []
         command = "display ntp session"
         output = self.device.send_command(command)
-        re_ntp = r"clock source:\s+(?P<clock_source>\S+)$\n.*" \
-                 r"clock stratum:\s+(?P<clock_strat>\S+)$\n.*" \
-                 r"clock status:\s+(?P<sync_status>.+)$\n.*" \
-                 r"reference clock ID:\s(?P<ntp_ref_id>\S+)$\n.*" \
-                 r"reach:\s(?P<reach>\S+)$\n.*" \
-                 r"current poll:\s(?P<cur_poll>\S+)$\n.*" \
-                 r"now:\s(?P<now>\S+)$\n.*" \
-                 r"offset:\s(?P<offset>.+)$\n.*" \
-                 r"delay:\s(?P<delay>.+)$\n.*" \
-                 r"disper:\s(?P<disper>.+)$"
+        re_ntp = (
+            r"clock source:\s+(?P<clock_source>\S+)$\n.*"
+            r"clock stratum:\s+(?P<clock_strat>\S+)$\n.*"
+            r"clock status:\s+(?P<sync_status>.+)$\n.*"
+            r"reference clock ID:\s(?P<ntp_ref_id>\S+)$\n.*"
+            r"reach:\s(?P<reach>\S+)$\n.*"
+            r"current poll:\s(?P<cur_poll>\S+)$\n.*"
+            r"now:\s(?P<now>\S+)$\n.*"
+            r"offset:\s(?P<offset>.+)$\n.*"
+            r"delay:\s(?P<delay>.+)$\n.*"
+            r"disper:\s(?P<disper>.+)$"
+        )
 
         match = re.findall(re_ntp, output, re.MULTILINE)
         for ntp_info in match:
             ntp_dict = {
-                'clock source': ntp_info[0],
-                'clock stratum': int(ntp_info[1]),
-                'clock status': ntp_info[2],
-                'reference clock id': ntp_info[3],
-                'reach': ntp_info[4],
-                'current poll': ntp_info[5],
-                'now': ntp_info[6],
-                'offset': ntp_info[7],
-                'delay': ntp_info[8],
-                'disper': ntp_info[9]
+                "clock source": ntp_info[0],
+                "clock stratum": int(ntp_info[1]),
+                "clock status": ntp_info[2],
+                "reference clock id": ntp_info[3],
+                "reach": ntp_info[4],
+                "current poll": ntp_info[5],
+                "now": ntp_info[6],
+                "offset": ntp_info[7],
+                "delay": ntp_info[8],
+                "disper": ntp_info[9],
             }
             ntp_peer.append(ntp_dict)
         return ntp_peer
 
     # to modify
     def get_ntp_servers(self):
         """
@@ -1496,27 +1768,29 @@
                         'synch distanc': '0.012'
                         },
         }
         """
         ntp_server = {}
         command = "display ntp-service sessions"
         output = self.device.send_command(command)
-        re_ntp = r"server\s+(?P<ntp_server>\S+),.*" \
-                 r"stratum\s+(?P<clock_strat>\S+),\s*" \
-                 r"offset\s+(?P<offset>.+),\s.*" \
-                 r"synch distance\s(?P<synch_distance>\S+)"
+        re_ntp = (
+            r"server\s+(?P<ntp_server>\S+),.*"
+            r"stratum\s+(?P<clock_strat>\S+),\s*"
+            r"offset\s+(?P<offset>.+),\s.*"
+            r"synch distance\s(?P<synch_distance>\S+)"
+        )
 
         match = re.findall(re_ntp, output, re.MULTILINE)
 
         for ntp_info in match:
             ntp_dict = {
-                'server': ntp_info[0],
-                'clock stratum': int(ntp_info[1]),
-                'offset': ntp_info[2],
-                'synch distanc': ntp_info[3]
+                "server": ntp_info[0],
+                "clock stratum": int(ntp_info[1]),
+                "offset": ntp_info[2],
+                "synch distanc": ntp_info[3],
             }
             ntp_server.append(ntp_dict)
         return ntp_server
 
     # to modify
     def get_ntp_stats(self):
         """
@@ -1536,44 +1810,45 @@
             "offset": 2.425,
             "jitter": 4.028
         }
         """
         ntp_stats = {}
         command = "display ntp status"
         output = self.device.send_command(command)
-        re_ntp = r"clock status:\s+(?P<sync_status>\S+).*" \
-                 r"clock stratum:\s+(?P<clock_strat>\S+).*" \
-                 r"reference clock ID:\s(?P<ntp_ref_id>\S+).*" \
-                 r"reference time:\s(?P<ref_time>.+\))"
+        re_ntp = (
+            r"clock status:\s+(?P<sync_status>\S+).*"
+            r"clock stratum:\s+(?P<clock_strat>\S+).*"
+            r"reference clock ID:\s(?P<ntp_ref_id>\S+).*"
+            r"reference time:\s(?P<ref_time>.+\))"
+        )
         match = re.search(re_ntp, output, re.DOTALL)
         if match is None:
             msg = "No Match Found"
             raise ValueError(msg)
         else:
             ntp_dict = {
-                'clock_status': match.group('sync_status'),
-                'clock_stratum': int(match.group('clock_strat')),
-                'ntp_reference_id': match.group('ntp_ref_id'),
-                'reference_time': match.group('ref_time')
+                "clock_status": match.group("sync_status"),
+                "clock_stratum": int(match.group("clock_strat")),
+                "ntp_reference_id": match.group("ntp_ref_id"),
+                "reference_time": match.group("ref_time"),
             }
         ntp_stats.update(ntp_dict)
         return ntp_stats
 
     # developing
     def get_optics(self):
         pass
 
     # developing
     def get_route_to(self, destination="", protocol=""):
         pass
 
     # developing
     def get_snmp_information(self):
-
-        '''
+        """
         {
             "chassis_id": "FOC1713Z00J",
             "community": {
                 "sdve44Kurkdd": {
                     "mode": "ro",
                     "acl": "10"
                 },
@@ -1585,29 +1860,16 @@
                     "mode": "ro",
                     "acl": "12"
                 }
             },
             "contact": "unknown",
             "location": "Street 21, Santiago"
         }
-        '''
-        # snmp_information = {}
-        # command = 'display snmp-agent sys-info'
-        # output = self.device.send_command(command)
-        re_contact = r"managed node:\n\s+(?P<contact>[&,\.a-zA-Z0-9_ ]+)"
-        re_location = r"physical location of this node:\n\s+(?P<location>[&,\.a-zA-Z0-9_ ]+)"
-        re_snmp_version = r" SNMP version running in the system:\n\s+(?P<location>[&,\.a-zA-Z0-9_ ]+)"
-
-        snmp_information = {
-            'contact': '',
-            'location': '',
-            'community': {},
-            'chassis_id': ''
-        }
-        return snmp_information
+        """
+        pass
 
     # IN developing
     def get_users(self):
         """
         {
             "netconf": {
                 "level": 1,
@@ -1620,43 +1882,41 @@
         }
         """
         local_users = []
 
         command = "display local-user"
         output = self.device.send_command(command)
 
-
         if not output:
             return []
 
         re_local_users = r"^\s+(?P<username>\w+)\s+(?P<state>\w+)\s+(?P<type>\w+)"
 
         for user in output.splitlines():
-
             match_user = re.search(re_local_users, user, flags=re.M)
 
             if match_user is None:
                 continue
-            elif match_user.group('username') == 'Username':
+            elif match_user.group("username") == "Username":
                 continue
-            
+
             local_users.append(
-                {"username": match_user.group('username'),
-                "state" : match_user.group('state'),
-                "type" : match_user.group('type')
-            })
+                {
+                    "username": match_user.group("username"),
+                    "state": match_user.group("state"),
+                    "type": match_user.group("type"),
+                }
+            )
 
         return local_users
 
-
-
     # developing
     def get_vlans(self):
         pass
-        '''
+        """
         {
             "1": {
                 "name": "default",
                 "interfaces": [
                     "GigabitEthernet0/9",
                     "GigabitEthernet0/12",
                     "GigabitEthernet0/22",
@@ -1673,15 +1933,16 @@
             "800": {
                 "name": "coopero",
                 "interfaces": [
                     "GigabitEthernet0/19"
                 ]
             }
         }
-        '''
+        """
+
     @staticmethod
     def _separate_section(separator, content):
         if content == "":
             return []
 
         # Break output into per-interface sections
         interface_lines = re.split(separator, content, flags=re.M)
@@ -1698,187 +1959,165 @@
             msg = "Unexpected output data:\n{}".format(interface_lines)
             raise ValueError(msg)
 
         # Combine the separator and section into one string
         intf_iter = iter(interface_lines)
 
         try:
-            new_interfaces = [line + next(intf_iter, '') for line in intf_iter]
+            new_interfaces = [line + next(intf_iter, "") for line in intf_iter]
         except TypeError:
             raise ValueError()
         return new_interfaces
 
     def _delete_file(self, filename):
-        command = 'delete /unreserved /quiet {0}'.format(filename)
+        command = "delete /unreserved /quiet {0}".format(filename)
         self.device.send_command(command)
 
-    def _save_config(self, filename=''):
+    def _save_config(self, filename=""):
         """Save the current running config to the given file."""
-        command = 'save {}'.format(filename)
-        save_log = self.device.send_command(command, max_loops=10, expect_string=r'Y/N')
+        command = "save {}".format(filename)
+        save_log = self.device.send_command(command, max_loops=10, expect_string=r"Y/N")
         # Search pattern will not be detected when set a new hostname, so don't use auto_find_prompt=False
-        save_log += self.device.send_command('y', expect_string=r'<.+>')
+        save_log += self.device.send_command("y", expect_string=r"<.+>")
         search_result = re.search("successfully", save_log, re.M)
         if search_result is None:
             msg = "Failed to save config. Command output:{}".format(save_log)
             raise CommandErrorException(msg)
 
     def _load_config(self, config_file):
-        command = 'rollback configuration to file {0}'.format(config_file)
-        rollback_result = self.device.send_command(command, expect_string=r'Y/N')
-        rollback_result += self.device.send_command('y', expect_string=r'[<\[].+[>\]]')
+        command = "rollback configuration to file {0}".format(config_file)
+        rollback_result = self.device.send_command(command, expect_string=r"Y/N")
+        rollback_result += self.device.send_command("y", expect_string=r"[<\[].+[>\]]")
         search_result = re.search("clear the information", rollback_result, re.M)
         if search_result is not None:
-            rollback_result += self.device.send_command('y', expect_string=r'<.+>')
+            rollback_result += self.device.send_command("y", expect_string=r"<.+>")
 
         search_result = re.search("succeeded|finished", rollback_result, re.M)
         if search_result is None:
             msg = "Failed to load config. Command output:{}".format(rollback_result)
             raise CommandErrorException(msg)
 
-    def _replace_candidate(self, filename, config):
-        if not filename:
-            filename = self._create_tmp_file(config)
-        else:
-            if not os.path.isfile(filename):
-                raise ReplaceConfigException("File {} not found".format(filename))
-
-        self.replace_file = filename
-
-        if not self._enough_space(self.replace_file):
-            msg = 'Could not transfer file. Not enough space on device.'
-            raise ReplaceConfigException(msg)
-
-        need_transfer = True
-        if self._check_file_exists(self.replace_file):
-            if self._check_md5(self.replace_file):
-                need_transfer = False
-        if need_transfer:
-            dest = os.path.basename(self.replace_file)
-            # full_remote_path = 'flash:/{}'.format(dest)
-            with paramiko.SSHClient() as ssh:
-                ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-                ssh.connect(hostname=self.hostname, username=self.username, password=self.password, port=self.port,
-                            look_for_keys=False)
-
-                try:
-                    with paramiko.SFTPClient.from_transport(ssh.get_transport()) as sftp_client:
-                        sftp_client.put(self.replace_file, dest)
-                    # with SCPClient(ssh.get_transport()) as scp_client:
-                    #     scp_client.put(self.replace_file, dest)
-                except Exception as e:
-                    msg = 'Could not transfer file. There was an error during transfer:' + str(e)
-                    raise ReplaceConfigException(msg)
-        self.config_replace = True
-        if config and os.path.isfile(self.replace_file):
-            os.remove(self.replace_file)
-
-    def _verify_remote_file_exists(self, dst, file_system='flash:'):
-        command = 'dir {0}/{1}'.format(file_system, dst)
+    def _verify_remote_file_exists(self, dst, file_system="flash:"):
+        command = "dir {0}/{1}".format(file_system, dst)
         output = self.device.send_command(command)
-        if 'No file found' in output:
-            raise ReplaceConfigException('Could not transfer file.')
+        if "No file found" in output:
+            raise ReplaceConfigException("Could not transfer file.")
 
     def _check_file_exists(self, cfg_file):
-        command = 'dir {}'.format(cfg_file)
+        command = "dir {}".format(cfg_file)
         output = self.device.send_command(command)
-        if 'No file found' in output:
+        if "No file found" in output:
             return False
         return True
 
     def _check_md5(self, dst):
         dst_hash = self._get_remote_md5(dst)
         src_hash = self._get_local_md5(dst)
         if src_hash == dst_hash:
             return True
         return False
 
     @staticmethod
-    def _get_local_md5(dst, blocksize=2 ** 20):
+    def _get_local_md5(dst, blocksize=2**20):
         md5 = hashlib.md5()
-        local_file = open(dst, 'rb')
+        local_file = open(dst, "rb")
         buf = local_file.read(blocksize)
         while buf:
             md5.update(buf)
             buf = local_file.read(blocksize)
         local_file.close()
         return md5.hexdigest()
 
     def _get_remote_md5(self, dst):
-        command = 'display system file-md5 {0}'.format(dst)
+        command = "display system file-md5 {0}".format(dst)
         output = self.device.send_command(command)
         filename = os.path.basename(dst)
-        match = re.search(filename + r'\s+(?P<md5>\w+)', output, re.M)
+        match = re.search(filename + r"\s+(?P<md5>\w+)", output, re.M)
         if match is None:
             msg = "Unexpected format: {}".format(output)
             raise ValueError(msg)
-        return match.group('md5')
+        return match.group("md5")
 
     def _commit_merge(self):
         commands = [command for command in self.merge_candidate.splitlines() if command]
-        output = ''
+        output = ""
 
         try:
-            output += self.device.send_command('system-view', expect_string=r'\[.+\]')
+            output += self.device.send_command("system-view", expect_string=r"\[.+\]")
             for command in commands:
-                output += self.device.send_command(command, expect_string=r'\[.+\]')
+                output += self.device.send_command(command, expect_string=r"\[.+\]")
 
             if self.device.check_config_mode():
                 check_error = re.search("error", output, re.IGNORECASE)
                 if check_error is not None:
-                    return_log = self.device.send_command('return', expect_string=r'[<\[].+[>\]]')
-                    if 'Uncommitted configurations' in return_log:
+                    return_log = self.device.send_command(
+                        "return", expect_string=r"[<\[].+[>\]]"
+                    )
+                    if "Uncommitted configurations" in return_log:
                         # Discard uncommitted configuration
-                        return_log += self.device.send_command('n', expect_string=r'<.+>')
+                        return_log += self.device.send_command(
+                            "n", expect_string=r"<.+>"
+                        )
                     output += return_log
-                    raise MergeConfigException('Error while applying config!')
-                output += self.device.send_command('commit', expect_string=r'\[.+\]')
-                output += self.device.send_command('return', expect_string=r'<.+>')
+                    raise MergeConfigException("Error while applying config!")
+                output += self.device.send_command("commit", expect_string=r"\[.+\]")
+                output += self.device.send_command("return", expect_string=r"<.+>")
             else:
-                raise MergeConfigException('Not in configuration mode.')
+                raise MergeConfigException("Not in configuration mode.")
         except Exception as e:
-            msg = str(e) + '\nconfiguration output: ' + output
+            msg = str(e) + "\nconfiguration output: " + output
             raise MergeConfigException(msg)
 
     def _get_merge_diff(self):
         diff = []
-        running_config = self.get_config(retrieve='running')['running']
+        running_config = self.get_config(retrieve="running")["running"]
         running_lines = running_config.splitlines()
         for line in self.merge_candidate.splitlines():
             if line not in running_lines and line:
-                if line[0].strip() != '!':
+                if line[0].strip() != "!":
                     diff.append(line)
-        return '\n'.join(diff)
+        return "\n".join(diff)
+
+    def _get_contextual_diff(self):
+        running_config = self.get_config(retrieve="running")["running"]
+        running_config = IndentedConfig(running_config, sanitize=True)
+        merge_candidate = IndentedConfig(self.merge_candidate, sanitize=True)
+        diff = IncrementalDiff(merge_candidate, running_config)
+        return str(diff)
 
     def _get_diff(self, filename=None):
         """Get a diff between running config and a proposed file."""
         if filename is None:
-            return self.device.send_command('display configuration changes')
-        return self.device.send_command('display configuration changes running file ' + filename)
+            return self.device.send_command("display configuration changes")
+        return self.device.send_command(
+            "display configuration changes running file " + filename
+        )
 
     def _enough_space(self, filename):
         flash_size = self._get_flash_size()
         file_size = os.path.getsize(filename)
         if file_size > flash_size:
             return False
         return True
 
     def _get_flash_size(self):
-        command = 'dir {}'.format('flash:')
+        command = "dir {}".format("flash:")
         output = self.device.send_command(command)
 
-        match = re.search(r'\(\d.*KB free\)', output, re.M)
+        match = re.search(r"\(\d.*KB free\)", output, re.M)
         if match is None:
-            msg = "Failed to get free space of flash (not match). Log: {}".format(output)
+            msg = "Failed to get free space of flash (not match). Log: {}".format(
+                output
+            )
             raise ValueError(msg)
 
         kbytes_free = 0
-        num_list = map(int, re.findall(r'\d+', match.group()))
+        num_list = map(int, re.findall(r"\d+", match.group()))
         for index, val in enumerate(reversed([num_list])):
-            kbytes_free += val * (1000 ** index)
+            kbytes_free += val * (1000**index)
         bytes_free = kbytes_free * 1024
         return bytes_free
 
     @staticmethod
     def _parse_uptime(uptime_str):
         """Return the uptime in seconds as an integer."""
         (years, weeks, days, hours, minutes, seconds) = (0, 0, 0, 0, 0, 0)
@@ -1898,24 +2137,30 @@
         minutes_regx = re.search(r"(?P<minute>\d+)\sminute", uptime_str)
         if minutes_regx is not None:
             minutes = int(minutes_regx.group(1))
         seconds_regx = re.search(r"(?P<second>\d+)\ssecond", uptime_str)
         if seconds_regx is not None:
             seconds = int(seconds_regx.group(1))
 
-        uptime_sec = (years * YEAR_SECONDS) + (weeks * WEEK_SECONDS) + (days * DAY_SECONDS) + \
-                     (hours * 3600) + (minutes * 60) + seconds
+        uptime_sec = (
+            (years * YEAR_SECONDS)
+            + (weeks * WEEK_SECONDS)
+            + (days * DAY_SECONDS)
+            + (hours * 3600)
+            + (minutes * 60)
+            + seconds
+        )
         return uptime_sec
 
     @staticmethod
     def _create_tmp_file(config):
         tmp_dir = tempfile.gettempdir()
         rand_fname = str(uuid.uuid4())
         filename = os.path.join(tmp_dir, rand_fname)
-        with open(filename, 'wt') as fobj:
+        with open(filename, "wt") as fobj:
             fobj.write(config)
         return filename
 
     @staticmethod
     def bgp_time_conversion(bgp_uptime):
         """
         Convert string time to seconds.
@@ -1979,50 +2224,51 @@
         Convert GE to GigabitEthernet format
         """
         interface = interface.strip()
 
         re_giga = r"^GE(?P<port>[A-Za-z0-9\/\.]+)"
         re_ether = r"Ether(?P<port>\d[A-Za-z0-9\/\.]+)"
 
-        match_giga = re.search(re_giga, interface ,flags=re.M)
-        match_ether = re.search(re_ether,interface,flags=re.M)
+        match_giga = re.search(re_giga, interface, flags=re.M)
+        match_ether = re.search(re_ether, interface, flags=re.M)
 
         if match_giga:
-            return 'GigabitEthernet' + match_giga.group('port')
+            return "GigabitEthernet" + match_giga.group("port")
         elif match_ether:
-            return 'Ethernet' + match_ether.group('port')
+            return "Ethernet" + match_ether.group("port")
         else:
             return interface
 
-
     @staticmethod
     def interface_bw_conversion(bandwidth):
         """
         Convert Bandwidth to kbps
         100M = 100000
         1G = 1000000
         10G = 10000000
         100G = 1000000000
         """
         bandwidth = bandwidth.strip()
 
-        if bandwidth == '':
-            return '0'
+        if bandwidth == "":
+            return "0"
+
+        if bandwidth == "1G":
+            return "1000000"
+        elif bandwidth == "10G":
+            return "10000000"
+        elif bandwidth == "25G":
+            return "25000000"
+        elif bandwidth == "50G":
+            return "50000000"
+        elif bandwidth == "100G":
+            return "100000000"
+        elif bandwidth == "100M":
+            return "100000"
+        elif bandwidth == "10M":
+            return "10000"
 
-        if bandwidth == '1G':
-            return '1000000'
-        elif bandwidth == '10G':
-            return '10000000'
-        elif bandwidth == '25G':
-            return '25000000'
-        elif bandwidth == '50G':
-            return '50000000'
-        elif bandwidth == '100G':
-            return '100000000'
-        elif bandwidth == '100M':
-            return '100000'
-        elif bandwidth == '10M':
-            return '10000'
-            
         raise ValueError(
-            "BW Conversion: Unexpected Bandwidth for GigabitEthernet: {}".format(bandwidth)
-        )
+            "BW Conversion: Unexpected Bandwidth for GigabitEthernet: {}".format(
+                bandwidth
+            )
+        )
```

