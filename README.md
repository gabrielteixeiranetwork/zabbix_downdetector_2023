# downdetector_2023
Instale

 apt install python3-pip
 pip3 install bs4
 pip3 install requests
 pip3 install cloudscraper
 apt install unzip
		 
Acesse a pasta cd /tmp

		 wget https://github.com/remontti/downdetector_zbx_grafana-DESCONTINUADO-/archive/refs/heads/master.zip
Verifique os arquivos dentro da pasta cd /tmp
		 
		 ls -lh
Descompate o arquivo		 
		 
		unzip master.zip
Entre na pasta descompactada
		
		cd downdetector_zbx_grafana-DESCONTINUADO--master/
Mova os arquivos para a pasta /usr/lib/zabbix/externalscripts
		 
		 mv downdetector* /usr/lib/zabbix/externalscripts
Entre na pasta /usr/lib/zabbix/externalscripts

		cd/usr/lib/zabbix/externalscripts
Agora vamos editar o arquivo (remover o https para http)

		 vim /usr/lib/zabbix/externalscripts/downdetector.py
Agora vamos dar permissão para o usuário zabbix
		
		 chown zabbix. /usr/lib/zabbix/externalscripts/downdetector*
		 chmod a+x /usr/lib/zabbix/externalscripts/downdetector*.py
Agora vamos verificar se está retornando algo (1 ou 2) dentro da pasta /usr/lib/zabbix/externalscripts execute
		 
		 ./downdetector.py whatsapp*
