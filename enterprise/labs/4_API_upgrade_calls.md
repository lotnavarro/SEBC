<h1>CM Lab</h1><br>

<h2>Upgrade Cloudera Manager</h2><br>


<b>CLI upgrade</b><br>

<code>[root@cdh1 CDH13]# ls</code><br>
cloudera-manager-agent-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm<br>
cloudera-manager-daemons-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm<br>
cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm<br>
cloudera-manager-server-db-2-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm<br>
oracle-j2sdk1.7-1.7.0+update67-1.x86_64.rpm<br>
<code>[root@cdh1 CDH13]# yum localinstall cloudera-manager-server- cloudera-manager-daemons cloudera-manager-agent<br></code>
cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm<br>
cloudera-manager-server-db-2-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm<br>
<code>[root@cdh1 CDH13]# yum localinstall cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm cloudera-manager-daemons-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm cloudera-manager-agent-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm <br></code>
Loaded plugins: ulninfo<br>
Examining cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm: cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64<br>
Marking cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm as an update to cloudera-manager-server-5.9.1-1.cm591.p0.8.el7.x86_64<br>
Examining cloudera-manager-daemons-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm: cloudera-manager-daemons-5.13.0-1.cm5130.p0.55.el7.x86_64<br>
Marking cloudera-manager-daemons-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm as an update to cloudera-manager-daemons-5.9.1-1.cm591.p0.8.el7.x86_64<br>
Examining cloudera-manager-agent-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm: cloudera-manager-agent-5.13.0-1.cm5130.p0.55.el7.x86_64<br>
Marking cloudera-manager-agent-5.13.0-1.cm5130.p0.55.el7.x86_64.rpm as an update to cloudera-manager-agent-5.9.1-1.cm591.p0.8.el7.x86_64<br>
Resolving Dependencies<br>
--> Running transaction check<br>
---> Package cloudera-manager-agent.x86_64 0:5.9.1-1.cm591.p0.8.el7 will be updated<br>
---> Package cloudera-manager-agent.x86_64 0:5.13.0-1.cm5130.p0.55.el7 will be an update<br>
---> Package cloudera-manager-daemons.x86_64 0:5.9.1-1.cm591.p0.8.el7 will be updated<br>
---> Package cloudera-manager-daemons.x86_64 0:5.13.0-1.cm5130.p0.55.el7 will be an update<br>
---> Package cloudera-manager-server.x86_64 0:5.9.1-1.cm591.p0.8.el7 will be updated<br>
---> Package cloudera-manager-server.x86_64 0:5.13.0-1.cm5130.p0.55.el7 will be an update<br>
--> Finished Dependency Resolution<br>
<br>
Dependencies Resolved<br>
<br>
================================================================================<br>
 Package<br>
    Arch   Version<br>
               Repository                                                  Size<br>
================================================================================<br>
Updating:<br>
 cloudera-manager-agent<br>
    x86_64 5.13.0-1.cm5130.p0.55.el7<br>
               /cloudera-manager-agent-5.13.0-1.cm5130.p0.55.el7.x86_64    76 M<br>
 cloudera-manager-daemons<br>
    x86_64 5.13.0-1.cm5130.p0.55.el7<br>
               /cloudera-manager-daemons-5.13.0-1.cm5130.p0.55.el7.x86_64 846 M<br>
 cloudera-manager-server<br>
    x86_64 5.13.0-1.cm5130.p0.55.el7<br>
               /cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64   12 k<br>
<br>
Transaction Summary<br>
================================================================================<br>
Upgrade  3 Packages<br>
<br>
Total size: 922 M<br>
<code>Is this ok [y/d/N]: y<br></code><br>
Downloading packages:<br>
Running transaction check<br>
Running transaction test<br>
Transaction test succeeded<br>
Running transaction<br>
  Updating   : cloudera-manager-daemons-5.13.0-1.cm5130.p0.55.el7.x86_64    1/6 <br>
  Updating   : cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64     2/6 <br>
  Updating   : cloudera-manager-agent-5.13.0-1.cm5130.p0.55.el7.x86_64      3/6 <br>
warning: /etc/cloudera-scm-agent/config.ini created as /etc/cloudera-scm-agent/config.ini.rpmnew<br>
  Cleanup    : cloudera-manager-agent-5.9.1-1.cm591.p0.8.el7.x86_64         4/6 <br>
  Cleanup    : cloudera-manager-server-5.9.1-1.cm591.p0.8.el7.x86_64        5/6 <br>
  Cleanup    : cloudera-manager-daemons-5.9.1-1.cm591.p0.8.el7.x86_64       6/6 <br>
  Verifying  : cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64     1/6 <br>
  Verifying  : cloudera-manager-daemons-5.13.0-1.cm5130.p0.55.el7.x86_64    2/6 <br>
  Verifying  : cloudera-manager-agent-5.13.0-1.cm5130.p0.55.el7.x86_64      3/6 <br>
  Verifying  : cloudera-manager-agent-5.9.1-1.cm591.p0.8.el7.x86_64         4/6 <br>
  Verifying  : cloudera-manager-daemons-5.9.1-1.cm591.p0.8.el7.x86_64       5/6 <br>
  Verifying  : cloudera-manager-server-5.9.1-1.cm591.p0.8.el7.x86_64        6/6 <br>
<br>
Updated:<br>
  cloudera-manager-agent.x86_64 0:5.13.0-1.cm5130.p0.55.el7                     <br>
  cloudera-manager-daemons.x86_64 0:5.13.0-1.cm5130.p0.55.el7                   <br>
  cloudera-manager-server.x86_64 0:5.13.0-1.cm5130.p0.55.el7                    <br>
<br>
Complete!<br>
<code>[root@cdh1 CDH13]# rpm -qa 'cloudera-manager-*'</code><br>
cloudera-manager-daemons-5.13.0-1.cm5130.p0.55.el7.x86_64<br>
cloudera-manager-agent-5.13.0-1.cm5130.p0.55.el7.x86_64<br>
cloudera-manager-server-5.13.0-1.cm5130.p0.55.el7.x86_64<br>
<code>[root@cdh1 CDH13]# sudo service cloudera-scm-server start<br></code>
Starting cloudera-scm-server (via systemctl):              [  <b>OK</b>  ]<br>
<code>[root@cdh1 CDH13]# sudo service cloudera-scm-agent start</code><br>
Starting cloudera-scm-agent (via systemctl):               [  <b>OK</b>  ]<br>
[root@cdh1 CDH13]# sudo su<br>
<code>[root@cdh1 CDH13]# yum clean all</code><br>
Loaded plugins: ulninfo<br>
Cleaning repos: cloudera-manager ol7_UEKR4 ol7_addons ol7_latest<br>
Cleaning up everything<br>
[root@cdh1 CDH13]# <br>

<br>
<b>Use the API on the command line</b><br>

<b>Report the latest available version of the API</b><br>

<code>[root@cdh1 CDH13]# curl -u lotnavarro:cloudera <br>
>  'http://localhost:7180/api/version'</code><br>
<b>18<br></b>[root@cdh1 CDH13]# 


<b>Report the CM version</b><br>

<code>[root@cdh1 CDH13]# curl -u lotnavarro:cloudera <br></code>
>  'http://localhost:7180/api/v18/cm/version'<br>
{<br>
  "version" : "5.13.0",<br>
  "buildUser" : "jenkins",<br>
  "buildTimestamp" : "20171002-1719",<br>
  "gitHash" : "bd657e597e6743c458ee2c9aabe808b7c972981c",<br>
  "snapshot" : false<br>
}<br>
[root@cdh1 CDH13]# 


<b>List all CM users</b><br>

<code>[root@cdh1 CDH13]# curl -u lotnavarro:cloudera  'http://localhost:7180/api/v18/users'</code><br>
{<br>
  "items" : [ {<br>
    "name" : "admin",<br>
    "roles" : [ "ROLE_LIMITED" ]<br>
  }, {<br>
    "name" : "lotnavarro",<br>
    "roles" : [ "ROLE_ADMIN" ]<br>
  }, {<br>
    "name" : "minotaur",<br>
    "roles" : [ "ROLE_CONFIGURATOR" ]<br>
  } ]<br>
}<br>[root@cdh1 CDH13]# <br>




<b>LReport the database server in use by CM</b><br>


<code>[root@cdh1 CDH13]# curl -u lotnavarro:cloudera  'http://localhost:7180/api/v18/cm/scmDbInfo'</code><br>
{<br>
  "scmDbType" : "MYSQL",<br>
  "embeddedDbUsed" : false<br>
}<br>[root@cdh1 CDH13]#<br>
 



