# Template Proxmox - Zabbix 5.0

Versão: pve-manager/6.1-3

# Requisitos:


<ul>Instalação do sudo</ul>

apt-get install sudo

<ul>Configuração do sudoers para os comandos remoto do zabbix usando qm.</ul>

<p>
Defaults:zabbix !requiretty<br />
Cmnd_Alias ZABBIX_CMD = /usr/sbin/qm<br />
zabbix   ALL = (other_user)  NOPASSWD: ALL<br />
zabbix   ALL = (root)        NOPASSWD: ZABBIX_CMD
</p>