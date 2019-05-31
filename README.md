# zabbix template and user parameters to monitor zfs on linux

This template is a modified version of the original work done by pbergdolt and posted on the zabbix forum a while ago here: https://www.zabbix.com/forum/zabbix-cookbook/35336-zabbix-zfs-discovery-monitoring?t=43347 .

I have maintained and modified this template over the year and the different version of ZoL on a large number of servers so I'm pretty confident that it works ;)

# Supported OS and ZoL version
Any Linux variant should work, tested version by myself include:
- Debian 8 and 9
- Ubuntu 16.04 and 18.04
- CentOS 6 and 7

About the ZoL version, this template is intended to be used by ZoL version 0.7.0 or superior but still works on the 0.6.x branch.

# Installation

To use this template, you need:
1. to import the template on your zabbix installation, it is currently working on zabbix version 3.0 or supperior
1. add the userparameter file on the server you want to monitor, this is usually done by adding it to the `/etc/zabbix/zabbix_agentd.d` folder, if in doubt, just look at your `zabbix_agentd.conf` file for the line begining by `Include=`, it will show you in which directory you must put it
1. that's all!
