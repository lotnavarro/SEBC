<h1>CLOUDERA BOOT CAMP - Challenges - Dec 1, 2017 - CDMX</h1>

<h2>INSTALL CM</h2>

<br>
<b>1</b><br>
<b>dbproperties</b><br>
<br>


[root@rkn1 raken]# <code>cat /etc/cloudera-scm-server/db.properties</code><br>
com.cloudera.cmf.db.type=mysql<br>

com.cloudera.cmf.db.host=sserverln.northcentralus.cloudapp.azure.com<br>

com.cloudera.cmf.db.name=scm<br>

com.cloudera.cmf.db.user=scm<br>

com.cloudera.cmf.db.password=Raken.2017<br>

com.cloudera.cmf.db.setupType=EXTERNAL<br>
[root@rkn1 raken]# <br>

<b>2</b><br>
<b>The first line of the server log</b><br>
<br>

[root@rkn1 raken]# cat /var/log/cloudera-scm-server/cloudera-scm-server.log
2017-12-01 12:52:13,711 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.9.1 (#8 built by jenkins on 20170112-1158 git: a66d8bbdbe8bc3ee54235e55423f2f76c7d9f3b1)


<b>3</b><br>
<b>The line(s) that contain the phrase "Started Jetty server"</b><br>
<br>

2017-12-01 12:58:03,520 INFO WebServerImpl:org.mortbay.log: jetty-6.1.26.cloudera.4<br>
2017-12-01 12:58:03,522 INFO WebServerImpl:org.mortbay.log: Started SelectChannelConnector@0.0.0.0:7180<br>
2017-12-01 12:58:03,522 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.<br>



