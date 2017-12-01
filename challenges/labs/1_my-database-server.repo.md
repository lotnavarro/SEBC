<h1>CLOUDERA BOOT CAMP - Challenges - Dec 1, 2017 - CDMX</h1>

<h2>Challenge 1: Install a MySQL server</h2>

<br>
<b>1</b><br>
<b>Use a YUM repository to install the package</b><br>
<b>
Install/b><br>


[raken@sserverln ~]$ <code>ls</code><br>
mysql-community-client-5.7.20-1.el7.x86_64.rpm<br>
mysql-community-common-5.7.20-1.el7.x86_64.rpm<br>
mysql-community-libs-5.7.20-1.el7.x86_64.rpm<br>
mysql-community-libs-compat-5.7.20-1.el7.x86_64.rpm<br>
mysql-community-server-5.7.20-1.el7.x86_64.rpm<br>
<br>
[raken@sserverln ~]$ <b>sudo su</b> <br>
[root@sserverln raken]# <code>yum localinstall mysql-community-common-5.7.20-1.el7.x86_64.rpm mysql-community-libs-* mysql-community-client-5.7.20-1.el7.x86_64.rpm mysql-community-server-5.7.20-1.el7.x86_64.rpm</code><br>
Loaded plugins: ulninfo<br>
Examining mysql-community-common-5.7.20-1.el7.x86_64.rpm: mysql-community-common-5.7.20-1.el7.x86_64<br>
Marking mysql-community-common-5.7.20-1.el7.x86_64.rpm to be installed<br>
Examining mysql-community-libs-5.7.20-1.el7.x86_64.rpm: mysql-community-libs-5.7.20-1.el7.x86_64<br>
Marking mysql-community-libs-5.7.20-1.el7.x86_64.rpm to be installed<br>
Examining mysql-community-libs-compat-5.7.20-1.el7.x86_64.rpm: mysql-community-libs-compat-5.7.20-1.el7.x86_64<br>
Marking mysql-community-libs-compat-5.7.20-1.el7.x86_64.rpm to be installed<br>
Examining mysql-community-client-5.7.20-1.el7.x86_64.rpm: mysql-community-client-5.7.20-1.el7.x86_64<br>
Marking mysql-community-client-5.7.20-1.el7.x86_64.rpm to be installed<br>
Examining mysql-community-server-5.7.20-1.el7.x86_64.rpm: mysql-community-server-5.7.20-1.el7.x86_64<br>
Marking mysql-community-server-5.7.20-1.el7.x86_64.rpm to be installed<br>
Resolving Dependencies<br>
--> Running transaction check<br>
---> Package mysql-community-client.x86_64 0:5.7.20-1.el7 will be installed<br>
---> Package mysql-community-common.x86_64 0:5.7.20-1.el7 will be installed<br>
---> Package mysql-community-libs.x86_64 0:5.7.20-1.el7 will be installed<br>
---> Package mysql-community-libs-compat.x86_64 0:5.7.20-1.el7 will be installed<br>
---> Package mysql-community-server.x86_64 0:5.7.20-1.el7 will be installed<br>
--> Processing Dependency: /usr/bin/perl for package: mysql-community-server-5.7.20-1.el7.x86_64<br>
ol7_UEKR4                                                | 1.2 kB     00:00     <br>
ol7_addons                                               | 1.2 kB     00:00     <br>
ol7_latest                                               | 1.4 kB     00:00     <br>
(1/2): ol7_latest/x86_64/updateinfo                        | 1.6 MB   00:00     <br>
(2/2): ol7_latest/x86_64/primary                           |  31 MB   00:00     <br>
ol7_latest                                                          23401/23401<br>
<br>
...<br>
<b>Complete!
</b>
