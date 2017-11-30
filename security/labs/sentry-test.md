
<h1>Lab: Integrating Kerberos with Cloudera Manager</h1><br> 
<h2>Sentry Lab</h2><br> 



<code>
[raken@cdh4 ~]$ beeline</b><br> </code>
<b>Beeline version 1.1.0-cdh5.9.1 by Apache Hive<br> 
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/cdh4.northcentralus.cloudapp.azure.com@RAKENCDH.COM<br> 
scan complete in 2ms<br> 
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/cdh4.northcentralus.cloudapp.azure.com@RAKENCDH.COM<br> 
Connected to: Apache Hive (version 1.1.0-cdh5.9.1)<br> 
Driver: Hive JDBC (version 1.1.0-cdh5.9.1)<br> 
Transaction isolation: TRANSACTION_REPEATABLE_READ<br> 
<code>0: jdbc:hive2://localhost:10000/default> show tables;<br> </code>
INFO  : Compiling command(queryId=hive_20171129200202_b074068c-0ff2-4fe3-95c6-ae7c357f368b): show tables<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129200202_b074068c-0ff2-4fe3-95c6-ae7c357f368b); Time taken: 0.851 seconds<br>
INFO  : Executing command(queryId=hive_20171129200202_b074068c-0ff2-4fe3-95c6-ae7c357f368b): show tables<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129200202_b074068c-0ff2-4fe3-95c6-ae7c357f368b); Time taken: 0.248 seconds<br>
INFO  : OK<br>
+-----------+--+<br>
| tab_name  |<br>
+-----------+--+<br>
+-----------+--+<br>
No rows selected (2.516 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>






[raken@cdh4 ~]$<br> 
<br> 


```

```
