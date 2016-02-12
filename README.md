### SNMP Builder - SNMP MIB Import for Zabbix Monitoring System

This repository contains files that are needed to add SNMP MIB Import functionality to Zabbix Monitoring System.

Please select a branch according to the Zabbix version you use.

#### Installation
1. Get SNMP Builder

   ```shell
   git clone -b <ver> https://github.com/macrokernel/zabbix-snmpbuilder
   ```
2. Go to to Zabbix frontend directory on your Zabbix server

   ```shell
   cd /usr/share/zabbix
   ```
3. Copy snmpbuilder patch file and images archive to this directory
4. Apply snmpbuilder patch

   ```shell
   patch -p3 < zabbix-<ver>-snmpbuilder.patch
   ```
5. Unpack images archive

   ```shell
   unzip zabbix-<ver>-snmpbuilder-imgs.zip -d /usr/share/zabbix
   ```
6. Remove patch file and images archive

   ```shell
   rm zabbix-<ver>-snmpbuilder.patch zabbix-<ver>-snmpbuilder-imgs.zip
