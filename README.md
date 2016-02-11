## SNMP Builder - SNMP MIB Import for Zabbix Monitoring System

This repository contains files that are needed to add SNMP MIB Import functionality to Zabbix Monitoring System

#### Installation
1. Go to to Zabbix frontend directory on your Zabbix server
   
   ```shell
   cd /usr/share/zabbix
   ```
2. Copy snmpbuilder patch file and images archive to this directory
3. Apply snmpbuilder patch
   
   ```shell
   patch -p3 < snmpbuilder-<ver>.patch
   ```
4. Unpack images, JavaScript and CSS archive
   
   ```shell
   tar zxf zabbix-2.0-snmpbuilder-imgs.tgz -C /usr/share/zabbix
   ```
5. Remove patch file and images archive
   
   ```shell
   rm snmpbuilder-<ver>.patch zabbix-2.0-snmpbuilder-imgs.tgz
   ```
