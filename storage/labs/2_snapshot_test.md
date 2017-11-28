<h1>Test HDFS Snapshots</code><br></h1><br>
<b>Create a precious directory in HDFS; copy the ZIP course file into it.</b><br>
<code>
[raken@cdh1 ~]$ HADOOP_USER_NAME=hdfs hadoop fs -mkdir /user/lotnavarro<br>
[raken@cdh1 ~]$ <br>
[raken@cdh1 ~]$ HADOOP_USER_NAME=hdfs hadoop fs -mkdir /user/lotnavarro<br>
[raken@cdh1 ~]$ HADOOP_USER_NAME=hdfs hadoop fs -chown -R lotnavarro:supergroup /user/lotnavarro<br>
[raken@cdh1 ~]$ hadoop fs -ls /user<br>
Found 5 items<br></code>
drwxrwxrwx   - mapred     hadoop              0 2017-11-27 21:15 /user/history<br>
drwxrwxr-t   - hive       hive                0 2017-11-27 21:16 /user/hive<br>
drwxrwxr-x   - hue        hue                 0 2017-11-27 21:17 /user/hue<br>
drwxr-xr-x   - lotnavarro supergroup          0 2017-11-28 11:10 /user/lotnavarro<br>
drwxrwxr-x   - oozie      oozie               0 2017-11-27 21:18 /user/oozie<br>
<br>
<b><h2>Create a precious directory in HDFS; copy the ZIP course file into it.</h2></b><br>

raken@cdh1 ~]$ 

[raken@cdh1 ~]$ HADOOP_USER_NAME=lotnavarro hadoop fs -mkdir /user/lotnavarro/precious/
[raken@cdh1 ~]$ hadoop fs -ls /user/lotnavarroFound 4 items
drwx------   - lotnavarro supergroup          0 2017-11-28 11:48 /user/lotnavarro/.staging
drwxr-xr-x   - lotnavarro supergroup          0 2017-11-28 12:20 /user/lotnavarro/precious
drwxr-xr-x   - lotnavarro supergroup          0 2017-11-28 11:34 /user/lotnavarro/teragen_lot
drwxr-xr-x   - lotnavarro supergroup          0 2017-11-28 11:48 /user/lotnavarro/terasort-lot
[raken@cdh1 ~]$ 

[raken@cdh1 ~]$ ls
CDH5.9  mysql-connector-java-5.1.44  mysql-connector-java-5.1.44.zip  <b>SEBC.zip</b>
[raken@cdh1 ~]$ HADOOP_USER_NAME=lotnavarro hadoop fs -put SEBC.zip /user/lotnavarro/precious/
[raken@cdh1 ~]$ hadoop fs -ls /user/lotnavarro/precious/
Found 1 items
-rw-r--r--   3 lotnavarro supergroup     474833 2017-11-28 12:32 /user/lotnavarro/precious/SEBC.zip
[raken@cdh1 ~]$ 

<b><h2>Delete the directory</h2></b><br>

[raken@cdh1 ~]$ HADOOP_USER_NAME=lotnavarro hadoop fs -rm -R /user/lotnavarro/precious/
rm: Failed to move to trash: hdfs://cdh1.northcentralus.cloudapp.azure.com:8020/user/lotnavarro/precious: The directory /user/lotnavarro/precious cannot be deleted since /user/lotnavarro/precious is snapshottable and already has snapshots
[raken@cdh1 ~]$ 

<b><h2>Delete the ZIP file</h2></b><br>

[raken@cdh1 ~]$ HADOOP_USER_NAME=lotnavarro hadoop fs -rm /user/lotnavarro/precious/SEBC.zip
17/11/28 12:50:53 INFO fs.TrashPolicyDefault: Moved: 'hdfs://cdh1.northcentralus.cloudapp.azure.com:8020/user/lotnavarro/precious/SEBC.zip' to trash at: hdfs://cdh1.northcentralus.cloudapp.azure.com:8020/user/lotnavarro/.Trash/Current/user/lotnavarro/precious/SEBC.zip
[raken@cdh1 ~]$ 
