systemctl stop chronyd
systemctl disable chronyd
systemctl status chronyd

sudo yum install ntp -y
sudo nano /etc/ntp.conf cronos.cenam.mx
sudo systemctl start ntpd
sudo systemctl enable ntpd

sudo systemctl restart ntpd
sudo ntpq -p

yum install nscd -y
systemctl start nscd
systemctl enable nscd
nscd -g
time nslookup www.google.com

1. Desactivar SELINUX
	Modificar archivo /etc/sysconfig/selinux
	SELINUX=disabled
2.- Deshabilitar IPV6
	Modificar archivo /etc/sysctl.conf:
	net.ipv6.conf.all.disable_ipv6 = 1
	net.ipv6.conf.default.disable_ipv6 = 1
3.- Reducir swappiness a 1
	Modificar archivo /etc/sysctl.conf
	sysctl vm.swappiness=1
	echo "vm.swappiness = 1" >> /etc/sysctl.conf

4.- Deshabilitar transparent hugepage defrag
	Ejecutar comando:
	echo never > /sys/kernel/mm/transparent_hugepage/defrag
	y agregarlo a archivo /etc/rc.local para que se ejecute siempre al arrancar

5.- Incrementar límites  nproc y nofiles a 32768 para los usuarios hdfs, hbase, yarn y mapred*
	Modificar archivo /etc/security/limits.conf
	hdfs  -       nofile  32768
	hdfs  -       nproc   2048
	hbase -       nofile  32768
	hbase -       nproc   2048
	yarn  -       nofile  32768
	yarn  -       nproc   2048
	mapred -       nofile  32768
	mapred -       nproc   2048
