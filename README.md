DRBD Resources monitoring template for Zabbix
=============================================

Using _drbdadm_ tool for monitoring of DRBD Resources

Tested on Zabbix Version 3.0
Tested on DRBD 8.3.x

FEATURES
--------
* LLD for DRBD Resources
* Monitoring of Role, Device state and Connection state
* Triggers for degraded situation

REQUIREMENTS
------------
* Zabbix server version 3.0
* drbdadm tool

INSTALLATION
------------
* Agent
  * Copy __userparameter_drbd.conf__ to __/etc/zabbix/zabbix_agentd.d/userparameter_drbd.conf__
  * Restart zabbix agent
* Server
  * Import template __template_drbd.xml__ file
  * Modify /etc/sudoers file to include directives from __sudo__ file (or fill in __/etc/sudoers.d/zabbix__ if supported. Remember to chmod it to 0440)

AUTHOR
------
Stefano Buelow - stefano.buelow@gmail.com

LICENSE
-------
GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007

See [LICENSE](LICENSE)

