
<h1>Tuning for YARN</code><br></h1><br>
<b><h2>Review, modify and run the file tools/YARNtest.sh</h2></b><br>
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

<b><h2>Second run: YARNtest.sh</h2></b><br>
*MAP_MB=`echo "($k*0.6)/1" | bc`*<br>
*RED_MB=`echo "($k*0.8)/1" | bc`*<br>

<code>
[raken@cdh1 ~]$ HADOOP_USER_NAME=lotnavarro ./YARNtest.sh</code><br>
<br>
Testing loop started on Tue Nov 28 16:21:30 EST 2017<br>
Mapper Containers: 8<br>
Reducer Containers: 1<br>
Container memory: 512<br>
Mapper JVM: 409<br>
Reducer JVM: 409<br>
<br>
real	1m5.763s<br>
user	0m5.642s<br>
sys	0m0.327s<br>
<br>
real	2m34.730s<br>
user	0m7.169s<br>
sys	0m0.473s<br>
Deleted /user/lotnavarro/results/tg-10GB-8-1-512<br>
Deleted /user/lotnavarro/results/ts-10GB-8-1-512<br>
Mapper Containers: 8<br>
Reducer Containers: 1<br>
Container memory: 1024<br>
Mapper JVM: 819<br>
Reducer JVM: 819<br>
<br>
real	1m6.252s<br>
user	0m5.294s<br>
sys	0m0.302s<br>
<br>
real	2m32.549s<br>
user	0m7.524s<br>
sys	0m0.439s<br>
Deleted /user/lotnavarro/results/tg-10GB-8-1-1024<br>
Deleted /user/lotnavarro/results/ts-10GB-8-1-1024<br>
Testing loop ended on Tue Nov 28 16:28:58 EST 2017<br>
[raken@cdh1 ~]$ <br>

