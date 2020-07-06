# Template Proxmox - Zabbix 5.0

Versão: pve-manager/6.1-3

# Requisitos:


Instalação do sudo

apt-get install sudo

Configuração do sudoers para os comandos remoto do zabbix usando qm.

Defaults:zabbix !requiretty
Cmnd_Alias ZABBIX_CMD = /usr/sbin/qm
zabbix   ALL = (other_user)  NOPASSWD: ALL
zabbix   ALL = (root)        NOPASSWD: ZABBIX_CMD
