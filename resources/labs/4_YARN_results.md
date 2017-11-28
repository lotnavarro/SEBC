
<h1>Tuning for YARN</code><br></h1><br>
<b><h2>Review and modify the file tools/YARNtest.sh</h2></b><br>
<code>
[raken@cdh1 ~]$ HADOOP_USER_NAME=lotnavarro ./YARNtest.sh</code><br>
Testing loop started on Tue Nov 28 16:05:46 EST 2017<br>
Mapper Containers: 8<br>
Reducer Containers: 1<br>
Container memory: 512<br>
Mapper JVM: 409<br>
Reducer JVM: 409<br>
<br>
real	1m10.295s<br>
user	0m5.680s<br>
sys	0m0.332s<br>
<br>
real	2m44.246s<br>
user	0m7.252s<br>
sys	0m0.430s<br>
Deleted /user/lotnavarro/results/tg-10GB-8-1-512<br>
Deleted /user/lotnavarro/results/ts-10GB-8-1-512<br>
Mapper Containers: 8<br>
Reducer Containers: 1<br>
Container memory: 1024<br>
Mapper JVM: 819<br>
Reducer JVM: 819<br>
<br>
real	1m8.983s<br>
user	0m5.542s<br>
sys	0m0.277s<br>
<br>
real	2m32.890s<br>
user	0m7.780s<br>
sys	0m0.450s<br>
Deleted /user/lotnavarro/results/tg-10GB-8-1-1024<br>
Deleted /user/lotnavarro/results/ts-10GB-8-1-1024<br>
Testing loop ended on Tue Nov 28 16:13:31 EST 2017<br>
[raken@cdh1 ~]$ <br>


