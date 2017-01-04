# HDD temperature monitoring template for Zabbix
Zabbix template for monitoring disk temperature. Uses [sysfs](https://en.wikipedia.org/wiki/Sysfs) and hddtemp command-line tool.

## Prerequisites
* Zabbix server version 3.0 or 3.2
* Zabbix database in UTF-8
* Zabbix Agent user has read access to sysfs
* hddtemp is installed
* hddtemp is executable by Zabbix Agent user: `chmod u+s $(which hddtemp)`

## Installing

### Agent
1. Copy *userparameter_hddtemp.conf* to /etc/zabbix/zabbix_agentd.d/
2. Restart Zabbix Agent service

### Server
1. Import *zbx_template_hddtemp.xml* template file into Zabbix templates

## Authors
Roman Eremeev

## License
This work is licensed under the Creative Commons Attribution Share Alike 4.0 license – see [LICENSE](LICENSE) file for details.
