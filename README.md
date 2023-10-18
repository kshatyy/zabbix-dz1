# Домашнее задание к занятию "`Система мониторинга Zabbix`" - `Шатый Константин`


---

### Задание 1

Скриншот-1 к заданию 1:
![Скриншот-1](https://github.com/kshatyy/zabbix-dz1/blob/main/img/1-1.png)

 wget https://repo.zabbix.com/zabbix/6.0/debian/pool/main/z/zabbix-release/zabbix-release_6.0-4+debian11_all.deb
 
 dpkg -i zabbix-release_6.0-4+debian11_all.deb
 
 apt update
 
 apt install zabbix-server-pgsql zabbix-frontend-php php7.4-pgsql zabbix-apache-conf zabbix-sql-scripts zabbix-agent
 
 sudo -u postgres createuser --pwprompt zabbix
 
 sudo -u postgres createdb -O zabbix zabbix
 
 zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql zabbix
 
 DBPassword=password
 
 systemctl restart zabbix-server zabbix-agent apache2
 
 systemctl enable zabbix-server zabbix-agent apache2

### Задание 2

Скриншот-1 к заданию 2:
![Скриншот-1](https://github.com/kshatyy/zabbix-dz1/blob/main/img/2-1.png)
Скриншот-2 к заданию 2:
![Скриншот-1](https://github.com/kshatyy/zabbix-dz1/blob/main/img/2-02.png)
Скриншот-3 к заданию 2:
![Скриншот-1](https://github.com/kshatyy/zabbix-dz1/blob/main/img/2-3.png)
Скриншот-4 к заданию 2:
![Скриншот-1](https://github.com/kshatyy/zabbix-dz1/blob/main/img/2-4.png)



wget https://repo.zabbix.com/zabbix/6.0/debian/pool/main/z/zabbix-release/zabbix-release_6.0-4+debian11_all.deb

dpkg -i zabbix-release_6.0-4+debian11_all.deb

apt update

apt install zabbix-agent

systemctl restart zabbix-agent

systemctl enable zabbix-agent

### Задание 3

Скриншот-1 к заданию 3:
![Скриншот-1](https://github.com/kshatyy/zabbix-dz1/blob/main/img/3.png)
