
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

<h2>Verify user privileges</h2><br>

[raken@cdh4 ~]$ beeline<br>
Beeline version 1.1.0-cdh5.9.1 by Apache Hive<br>
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/cdh4.northcentralus.cloudapp.azure.com@RAKENCDH.COM<br>
scan complete in 2ms<br>
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/cdh4.northcentralus.cloudapp.azure.com@RAKENCDH.COM<br>
Connected to: Apache Hive (version 1.1.0-cdh5.9.1)<br>
Driver: Hive JDBC (version 1.1.0-cdh5.9.1)<br>
Transaction isolation: TRANSACTION_REPEATABLE_READ<br>
0: jdbc:hive2://localhost:10000/default> show tables;<br>
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
<h2>Create a Sentry role with full authorization</h2><br><br>
: jdbc:hive2://localhost:10000/default> CREATE ROLE sentry_admin;<br>
INFO  : Compiling command(queryId=hive_20171129203131_4d1b9758-285d-4980-81c4-e9b2b4c66ecd): CREATE ROLE sentry_admin<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203131_4d1b9758-285d-4980-81c4-e9b2b4c66ecd); Time taken: 0.069 seconds<br>
INFO  : Executing command(queryId=hive_20171129203131_4d1b9758-285d-4980-81c4-e9b2b4c66ecd): CREATE ROLE sentry_admin<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203131_4d1b9758-285d-4980-81c4-e9b2b4c66ecd); Time taken: 1.212 seconds<br>
INFO  : OK<br>
No rows affected (1.296 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>
<br>

0: jdbc:hive2://localhost:10000/default> GRANT ALL ON SERVER server1 TO ROLE sentry_admin;<br>
INFO  : Compiling command(queryId=hive_20171129203232_626f383c-6764-4108-8f59-b6ea72419495): GRANT ALL ON SERVER server1 TO ROLE sentry_admin<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203232_626f383c-6764-4108-8f59-b6ea72419495); Time taken: 0.076 seconds<br>
INFO  : Executing command(queryId=hive_20171129203232_626f383c-6764-4108-8f59-b6ea72419495): GRANT ALL ON SERVER server1 TO ROLE sentry_admin<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203232_626f383c-6764-4108-8f59-b6ea72419495); Time taken: 0.24 seconds<br>
INFO  : OK<br>
No rows affected (0.359 seconds)<br>
0: jdbc:hive2://localhost:10000/default><br>
<br>
<h2>Create additional test users</h2><br><br>
 <br>
<br>
0: jdbc:hive2://localhost:10000/default> GRANT ROLE sentry_admin TO GROUP lotnavarro;<br>
INFO  : Compiling command(queryId=hive_20171129203333_39e7e370-e4fd-4621-87b8-2dffe2c0d7ac): GRANT ROLE sentry_admin TO GROUP lotnavarro<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203333_39e7e370-e4fd-4621-87b8-2dffe2c0d7ac); Time taken: 0.062 seconds<br>
INFO  : Executing command(queryId=hive_20171129203333_39e7e370-e4fd-4621-87b8-2dffe2c0d7ac): GRANT ROLE sentry_admin TO GROUP lotnavarro<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203333_39e7e370-e4fd-4621-87b8-2dffe2c0d7ac); Time taken: 0.117 seconds<br>
INFO  : OK<br>
No rows affected (0.192 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>
<br>

0: jdbc:hive2://localhost:10000/default> SHOW TABLES;<br>
INFO  : Compiling command(queryId=hive_20171129203333_e6b25c75-72ce-497d-9caf-f72ce163b939): SHOW TABLES<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203333_e6b25c75-72ce-497d-9caf-f72ce163b939); Time taken: 0.067 seconds<br>
INFO  : Executing command(queryId=hive_20171129203333_e6b25c75-72ce-497d-9caf-f72ce163b939): SHOW TABLES<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203333_e6b25c75-72ce-497d-9caf-f72ce163b939); Time taken: 0.249 seconds<br>
INFO  : OK<br>
+------------+--+<br>
|  tab_name  |<br>
+------------+--+<br>
| customers  |<br>
| sample_07  |<br>
| sample_08  |<br>
| web_logs   |<br>
+------------+--+<br>
4 rows selected (0.381 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>
<br>


0: jdbc:hive2://localhost:10000/default> CREATE ROLE reads;<br>
INFO  : Compiling command(queryId=hive_20171129203535_b38f8c53-a8a2-4307-b890-5188dfd3df8e): CREATE ROLE reads<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203535_b38f8c53-a8a2-4307-b890-5188dfd3df8e); Time taken: 0.061 seconds<br>
INFO  : Executing command(queryId=hive_20171129203535_b38f8c53-a8a2-4307-b890-5188dfd3df8e): CREATE ROLE reads<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203535_b38f8c53-a8a2-4307-b890-5188dfd3df8e); Time taken: 0.159 seconds<br>
INFO  : OK<br>
No rows affected (0.31 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>
<br>


0: jdbc:hive2://localhost:10000/default> CREATE ROLE writes;<br>
INFO  : Compiling command(queryId=hive_20171129203636_7d987d1b-a2b1-4722-a6d7-e151a99f7214): CREATE ROLE writes<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203636_7d987d1b-a2b1-4722-a6d7-e151a99f7214); Time taken: 0.06 seconds<br>
INFO  : Executing command(queryId=hive_20171129203636_7d987d1b-a2b1-4722-a6d7-e151a99f7214): CREATE ROLE writes<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203636_7d987d1b-a2b1-4722-a6d7-e151a99f7214); Time taken: 0.05 seconds<br>
INFO  : OK<br>
No rows affected (0.125 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>
<br>
<h2>Grant read privilege for all tables to reads</h2><br>

0: jdbc:hive2://localhost:10000/default> GRANT SELECT ON DATABASE default TO ROLE reads;<br>
INFO  : Compiling command(queryId=hive_20171129203636_857a1e01-4698-4455-9fc4-901c200fa5ec): GRANT SELECT ON DATABASE default TO ROLE reads<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203636_857a1e01-4698-4455-9fc4-901c200fa5ec); Time taken: 0.067 seconds<br>
INFO  : Executing command(queryId=hive_20171129203636_857a1e01-4698-4455-9fc4-901c200fa5ec): GRANT SELECT ON DATABASE default TO ROLE reads<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203636_857a1e01-4698-4455-9fc4-901c200fa5ec); Time taken: 0.186 seconds<br>
INFO  : OK<br>
No rows affected (0.282 seconds)<br>
0: jdbc:hive2://localhost:10000/default> [raken@cdh4 ~]$ <br>
<br>

0: jdbc:hive2://localhost:10000/default> GRANT ROLE reads TO GROUP selector;<br>
INFO  : Compiling command(queryId=hive_20171129203939_fc7617cc-a8c1-47d9-94a5-e53dd326ba2b): GRANT ROLE reads TO GROUP selector<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203939_fc7617cc-a8c1-47d9-94a5-e53dd326ba2b); Time taken: 0.065 seconds<br>
INFO  : Executing command(queryId=hive_20171129203939_fc7617cc-a8c1-47d9-94a5-e53dd326ba2b): GRANT ROLE reads TO GROUP selector<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203939_fc7617cc-a8c1-47d9-94a5-e53dd326ba2b); Time taken: 0.149 seconds<br>
INFO  : OK<br>
No rows affected (0.295 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>

<h2>Grant read privilege for default.sample07 only to 'writes':</h2><br><br>

0: jdbc:hive2://localhost:10000/default> REVOKE ALL ON DATABASE default FROM ROLE writes;<br>
<br>INFO  : Compiling command(queryId=hive_20171129204040_bf5db694-4810-409f-a3b6-9e1724747462): REVOKE ALL ON DATABASE default FROM ROLE writes
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129204040_bf5db694-4810-409f-a3b6-9e1724747462); Time taken: 0.446 seconds<br>
INFO  : Executing command(queryId=hive_20171129204040_bf5db694-4810-409f-a3b6-9e1724747462): REVOKE ALL ON DATABASE default FROM ROLE writes<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129204040_bf5db694-4810-409f-a3b6-9e1724747462); Time taken: 0.201 seconds<br>
INFO  : OK<br>
No rows affected (0.804 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>

0: jdbc:hive2://localhost:10000/default> GRANT SELECT ON default.sample_07 TO ROLE writes;<br>
INFO  : Compiling command(queryId=hive_20171129204141_38e12916-5378-49dd-8eec-efded2c36a98): GRANT SELECT ON default.sample_07 TO ROLE writes<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129204141_38e12916-5378-49dd-8eec-efded2c36a98); Time taken: 0.066 seconds<br>
INFO  : Executing command(queryId=hive_20171129204141_38e12916-5378-49dd-8eec-efded2c36a98): GRANT SELECT ON default.sample_07 TO ROLE writes<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129204141_38e12916-5378-49dd-8eec-efded2c36a98); Time taken: 0.063 seconds<br>
INFO  : OK<br>
No rows affected (0.142 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>

0: jdbc:hive2://localhost:10000/default> GRANT ROLE writes TO GROUP inserters;<br>
INFO  : Compiling command(queryId=hive_20171129204141_4ee0dcf1-3a14-4e30-84ed-5355c08a4510): GRANT ROLE writes TO GROUP inserters<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129204141_4ee0dcf1-3a14-4e30-84ed-5355c08a4510); Time taken: 0.065 seconds<br>
INFO  : Executing command(queryId=hive_20171129204141_4ee0dcf1-3a14-4e30-84ed-5355c08a4510): GRANT ROLE writes TO GROUP inserters<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129204141_4ee0dcf1-3a14-4e30-84ed-5355c08a4510); Time taken: 0.098 seconds<br>
INFO  : OK<br>
No rows affected (0.194 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>


<h2>kinit as george, then login to beeline</h2><br>

[raken@cdh4 ~]$ kinit george<br>
Password for george@RAKENCDH.COM: <br>
kinit: Password incorrect while getting initial credentials<br>
[raken@cdh4 ~]$ kinit george<br>
Password for george@RAKENCDH.COM: <br>
[raken@cdh4 ~]$ klist<br>
Ticket cache: FILE:/tmp/krb5cc_1000<br>
Default principal: george@RAKENCDH.COM<br>

Valid starting       Expires              Service principal<br>
11/29/2017 20:44:55  11/30/2017 20:44:55  krbtgt/RAKENCDH.COM@RAKENCDH.COM<br>
	renew until 12/06/2017 20:44:55<br>
[raken@cdh4 ~]$ beeline<br>
Beeline version 1.1.0-cdh5.9.1 by Apache Hive<br>
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/cdh4.northcentralus.cloudapp.azure.com@RAKENCDH.COM<br>
scan complete in 2ms<br>
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/cdh4.northcentralus.cloudapp.azure.com@RAKENCDH.COM<br>
Connected to: Apache Hive (version 1.1.0-cdh5.9.1)<br>
Driver: Hive JDBC (version 1.1.0-cdh5.9.1)<br>
Transaction isolation: TRANSACTION_REPEATABLE_READ<br>
0: jdbc:hive2://localhost:10000/default> show tables;<br>
INFO  : Compiling command(queryId=hive_20171129204646_40064bb6-c05d-471f-8f44-e4be7be3aedd): show tables<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129204646_40064bb6-c05d-471f-8f44-e4be7be3aedd); Time taken: 0.066 seconds<br>
INFO  : Executing command(queryId=hive_20171129204646_40064bb6-c05d-471f-8f44-e4be7be3aedd): show tables<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129204646_40064bb6-c05d-471f-8f44-e4be7be3aedd); Time taken: 0.16 seconds<br>
INFO  : OK<br>
+------------+--+<br>
|  tab_name  |<br>
+------------+--+<br>
| customers  |<br>
| sample_07  |<br>
| sample_08  |<br>
| web_logs   |<br>
+------------+--+<br>
4 rows selected (0.36 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>


<h2>kinit as ferdinand, then login to beeline</h2><br>

[raken@cdh4 ~]$ kinit ferdinand<br>
Password for ferdinand@RAKENCDH.COM: <br>
[raken@cdh4 ~]$ beeline<br>
Beeline version 1.1.0-cdh5.9.1 by Apache Hive<br>
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/cdh4.northcentralus.cloudapp.azure.com@RAKENCDH.COM<br>
scan complete in 2ms<br>
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/cdh4.northcentralus.cloudapp.azure.com@RAKENCDH.COM<br>
Connected to: Apache Hive (version 1.1.0-cdh5.9.1)<br>
Driver: Hive JDBC (version 1.1.0-cdh5.9.1)<br>
Transaction isolation: TRANSACTION_REPEATABLE_READ<br>
0: jdbc:hive2://localhost:10000/default> show tables;<br>
INFO  : Compiling command(queryId=hive_20171129204949_42d7dfa8-5d77-4f8a-bd7c-3e2f3cab78fe): show tables<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129204949_42d7dfa8-5d77-4f8a-bd7c-3e2f3cab78fe); Time taken: 0.067 seconds<br>
INFO  : Executing command(queryId=hive_20171129204949_42d7dfa8-5d77-4f8a-bd7c-3e2f3cab78fe): show tables<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129204949_42d7dfa8-5d77-4f8a-bd7c-3e2f3cab78fe); Time taken: 0.147 seconds<br>
INFO  : OK<br>
+------------+--+<br>
|  tab_name  |<br>
+------------+--+<br>
| sample_07  |<br>
+------------+--+<br>
1 row selected (0.326 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>
<br>

```
