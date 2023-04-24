# downdetector_2023

Instale
		 apt install python3-pip
		 pip3 install bs4
		 pip3 install requests
		 pip3 install cloudscraper
		 apt install unzip
*[/tmp]# wget https://github.com/remontti/downdetector_zbx_grafana-DESCONTINUADO-/archive/refs/heads/master.zip*
*/tmp]# ls -lh*
*[/tmp]# unzip master.zip*
*cd downdetector_zbx_grafana-DESCONTINUADO--master/*
*mv downdetector* /usr/lib/zabbix/externalscripts*
*cd/usr/lib/zabbix/externalscripts*
*vim /usr/lib/zabbix/externalscripts/downdetector.py*
*		(remover o https para http)*
*chown zabbix. /usr/lib/zabbix/externalscripts/downdetector**
*chmod a+x /usr/lib/zabbix/externalscripts/downdetector*.py*
*[/usr/lib/zabbix/externalscripts]# ./downdetector.py whatsapp*
