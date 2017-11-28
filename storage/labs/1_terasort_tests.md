
<h1>Test HDFS throughput</code><br></h1><br>
<b>Create an end-user Linux account named with your GitHub handle</b><br>
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
<b><h2>Create a 10 GB file using teragen</h2></b><br>
<code>
[raken@cdh1 ~]$ HADOOP_USER_NAME=lotnavarro time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen 100000000 /user/lotnavarro/teragen_lot</code><br>
17/11/28 11:32:37 INFO client.RMProxy: Connecting to ResourceManager at cdh2.northcentralus.cloudapp.azure.com/10.0.1.6:8032<br>
17/11/28 11:32:37 INFO terasort.TeraSort: Generating 100000000 using 2<br>
17/11/28 11:32:37 INFO mapreduce.JobSubmitter: number of splits:2<br>
17/11/28 11:32:38 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1511835351299_0001<br>
17/11/28 11:32:38 INFO impl.YarnClientImpl: Submitted application application_1511835351299_0001<br>
17/11/28 11:32:38 INFO mapreduce.Job: The url to track the job: http://cdh2.northcentralus.cloudapp.azure.com:8088/proxy/application_1511835351299_0001/<br>
17/11/28 11:32:38 INFO mapreduce.Job: Running job: job_1511835351299_0001<br>
17/11/28 11:32:44 INFO mapreduce.Job: Job job_1511835351299_0001 running in uber mode : false<br>
17/11/28 11:32:44 INFO mapreduce.Job:  map 0% reduce 0%<br>
17/11/28 11:32:54 INFO mapreduce.Job:  map 4% reduce 0%<br>
17/11/28 11:32:55 INFO mapreduce.Job:  map 9% reduce 0%<br>
17/11/28 11:32:57 INFO mapreduce.Job:  map 11% reduce 0%<br>
17/11/28 11:32:58 INFO mapreduce.Job:  map 13% reduce 0%<br>
17/11/28 11:33:00 INFO mapreduce.Job:  map 16% reduce 0%<br>
17/11/28 11:33:01 INFO mapreduce.Job:  map 18% reduce 0%<br>
17/11/28 11:33:05 INFO mapreduce.Job:  map 22% reduce 0%<br>
17/11/28 11:33:08 INFO mapreduce.Job:  map 25% reduce 0%<br>
17/11/28 11:33:12 INFO mapreduce.Job:  map 29% reduce 0%<br>
17/11/28 11:33:15 INFO mapreduce.Job:  map 34% reduce 0%<br>
17/11/28 11:33:18 INFO mapreduce.Job:  map 39% reduce 0%<br>
17/11/28 11:33:21 INFO mapreduce.Job:  map 43% reduce 0%<br>
17/11/28 11:33:24 INFO mapreduce.Job:  map 47% reduce 0%<br>
17/11/28 11:33:27 INFO mapreduce.Job:  map 49% reduce 0%<br>
17/11/28 11:33:30 INFO mapreduce.Job:  map 54% reduce 0%<br>
17/11/28 11:33:33 INFO mapreduce.Job:  map 58% reduce 0%<br>
17/11/28 11:33:37 INFO mapreduce.Job:  map 59% reduce 0%<br>
17/11/28 11:33:40 INFO mapreduce.Job:  map 64% reduce 0%<br>
17/11/28 11:33:43 INFO mapreduce.Job:  map 67% reduce 0%<br>
17/11/28 11:33:46 INFO mapreduce.Job:  map 72% reduce 0%<br>
17/11/28 11:33:49 INFO mapreduce.Job:  map 75% reduce 0%<br>
17/11/28 11:33:52 INFO mapreduce.Job:  map 76% reduce 0%<br>
17/11/28 11:33:55 INFO mapreduce.Job:  map 77% reduce 0%<br>
17/11/28 11:33:58 INFO mapreduce.Job:  map 78% reduce 0%<br>
17/11/28 11:34:01 INFO mapreduce.Job:  map 79% reduce 0%<br>
17/11/28 11:34:04 INFO mapreduce.Job:  map 80% reduce 0%<br>
17/11/28 11:34:07 INFO mapreduce.Job:  map 82% reduce 0%<br>
17/11/28 11:34:13 INFO mapreduce.Job:  map 83% reduce 0%<br>
17/11/28 11:34:16 INFO mapreduce.Job:  map 85% reduce 0%<br>
17/11/28 11:34:19 INFO mapreduce.Job:  map 87% reduce 0%<br>
17/11/28 11:34:22 INFO mapreduce.Job:  map 88% reduce 0%<br>
17/11/28 11:34:25 INFO mapreduce.Job:  map 90% reduce 0%<br>
17/11/28 11:34:28 INFO mapreduce.Job:  map 91% reduce 0%<br>
17/11/28 11:34:31 INFO mapreduce.Job:  map 92% reduce 0%<br>
17/11/28 11:34:34 INFO mapreduce.Job:  map 94% reduce 0%<br>
17/11/28 11:34:37 INFO mapreduce.Job:  map 95% reduce 0%<br>
17/11/28 11:34:40 INFO mapreduce.Job:  map 97% reduce 0%<br>
17/11/28 11:34:47 INFO mapreduce.Job:  map 99% reduce 0%<br>
17/11/28 11:34:48 INFO mapreduce.Job:  map 100% reduce 0%<br>
17/11/28 11:34:49 INFO mapreduce.Job: Job job_1511835351299_0001 completed successfully<br>
17/11/28 11:34:49 INFO mapreduce.Job: Counters: 31<br>
	File System Counters<br>
		FILE: Number of bytes read=0<br>
		FILE: Number of bytes written=245820<br>
		FILE: Number of read operations=0<br>
		FILE: Number of large read operations=0<br>
		FILE: Number of write operations=0<br>
		HDFS: Number of bytes read=170<br>
		HDFS: Number of bytes written=10000000000<br>
		HDFS: Number of read operations=8<br>
		HDFS: Number of large read operations=0<br>
		HDFS: Number of write operations=4<br>
	Job Counters <br>
		Launched map tasks=2<br>
		Other local map tasks=2<br>
		Total time spent by all maps in occupied slots (ms)=244291<br>
		Total time spent by all reduces in occupied slots (ms)=0<br>
		Total time spent by all map tasks (ms)=244291<br>
		Total vcore-seconds taken by all map tasks=244291<br>
		Total megabyte-seconds taken by all map tasks=250153984<br>
	Map-Reduce Framework<br>
		Map input records=100000000<br>
		Map output records=100000000<br>
		Input split bytes=170<br>
		Spilled Records=0<br>
		Failed Shuffles=0<br>
		Merged Map outputs=0<br>
		GC time elapsed (ms)=1469<br>
		CPU time spent (ms)=150380<br>
		Physical memory (bytes) snapshot=401956864<br>
		Virtual memory (bytes) snapshot=3186462720<br>
		Total committed heap usage (bytes)=800063488<br>
	org.apache.hadoop.examples.terasort.TeraGen$Counters<br>
		CHECKSUM=214760662691937609<br>
	File Input Format Counters <br>
		Bytes Read=0<br>
	File Output Format Counters <br>
		Bytes Written=10000000000<br>
5.65user 0.34system 2:14.79elapsed 4%CPU (0avgtext+0avgdata 250108maxresident)k
0inputs+2032outputs (0major+70291minor)pagefaults 0swaps<br></code>
<code>[raken@cdh1 ~]$ hadoop fs -ls /user/lotnavarro<br>
Found 2 items<br>
drwx------   - lotnavarro supergroup          0 2017-11-28 11:34 /user/lotnavarro/.staging<br>
drwxr-xr-x   - lotnavarro supergroup          0 2017-11-28 11:34 /user/lotnavarro/teragen_lot<br>
[raken@cdh1 ~]$ <br>
<br>
<b><h2>Create a 10 GB file using terasort</h2></b><br>

[raken@cdh1 ~]$ HADOOP_USER_NAME=lotnavarro time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort /user/lotnavarro/teragen_lot /user/lotnavarro/terasort-lot<br>
17/11/28 11:44:43 INFO terasort.TeraSort: starting<br>
17/11/28 11:44:45 INFO input.FileInputFormat: Total input paths to process : 2<br>
Spent 164ms computing base-splits.
Spent 3ms computing TeraScheduler splits.
Computing input splits took 168ms
Sampling 10 splits of 76
Making 12 from 100000 sampled records
Computing parititions took 555ms
Spent 725ms computing partitions.
17/11/28 11:44:45 INFO client.RMProxy: Connecting to ResourceManager at cdh2.northcentralus.cloudapp.azure.com/10.0.1.6:8032
17/11/28 11:44:46 INFO mapreduce.JobSubmitter: number of splits:76
17/11/28 11:44:46 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1511835351299_0002
17/11/28 11:44:46 INFO impl.YarnClientImpl: Submitted application application_1511835351299_0002
17/11/28 11:44:46 INFO mapreduce.Job: The url to track the job: http://cdh2.northcentralus.cloudapp.azure.com:8088/proxy/application_1511835351299_0002/
17/11/28 11:44:46 INFO mapreduce.Job: Running job: job_1511835351299_0002
17/11/28 11:44:52 INFO mapreduce.Job: Job job_1511835351299_0002 running in uber mode : false
17/11/28 11:44:52 INFO mapreduce.Job:  map 0% reduce 0%
17/11/28 11:45:05 INFO mapreduce.Job:  map 2% reduce 0%
17/11/28 11:45:06 INFO mapreduce.Job:  map 4% reduce 0%
17/11/28 11:45:07 INFO mapreduce.Job:  map 5% reduce 0%
17/11/28 11:45:08 INFO mapreduce.Job:  map 10% reduce 0%
17/11/28 11:45:09 INFO mapreduce.Job:  map 20% reduce 0%
17/11/28 11:45:11 INFO mapreduce.Job:  map 23% reduce 0%
17/11/28 11:45:13 INFO mapreduce.Job:  map 25% reduce 0%
17/11/28 11:45:14 INFO mapreduce.Job:  map 29% reduce 0%
17/11/28 11:45:15 INFO mapreduce.Job:  map 30% reduce 0%
17/11/28 11:45:22 INFO mapreduce.Job:  map 32% reduce 0%
17/11/28 11:45:23 INFO mapreduce.Job:  map 34% reduce 0%
17/11/28 11:45:24 INFO mapreduce.Job:  map 36% reduce 0%
17/11/28 11:45:25 INFO mapreduce.Job:  map 37% reduce 0%
17/11/28 11:45:26 INFO mapreduce.Job:  map 39% reduce 0%
17/11/28 11:45:27 INFO mapreduce.Job:  map 43% reduce 0%
17/11/28 11:45:28 INFO mapreduce.Job:  map 44% reduce 0%
17/11/28 11:45:29 INFO mapreduce.Job:  map 51% reduce 0%
17/11/28 11:45:30 INFO mapreduce.Job:  map 53% reduce 0%
17/11/28 11:45:31 INFO mapreduce.Job:  map 54% reduce 0%
17/11/28 11:45:32 INFO mapreduce.Job:  map 57% reduce 0%
17/11/28 11:45:33 INFO mapreduce.Job:  map 58% reduce 0%
17/11/28 11:45:34 INFO mapreduce.Job:  map 61% reduce 0%
17/11/28 11:45:36 INFO mapreduce.Job:  map 62% reduce 0%
17/11/28 11:45:39 INFO mapreduce.Job:  map 66% reduce 0%
17/11/28 11:45:40 INFO mapreduce.Job:  map 68% reduce 0%
17/11/28 11:45:41 INFO mapreduce.Job:  map 69% reduce 0%
17/11/28 11:45:42 INFO mapreduce.Job:  map 70% reduce 0%
17/11/28 11:45:45 INFO mapreduce.Job:  map 72% reduce 0%
17/11/28 11:45:46 INFO mapreduce.Job:  map 75% reduce 0%
17/11/28 11:45:47 INFO mapreduce.Job:  map 76% reduce 0%
17/11/28 11:45:48 INFO mapreduce.Job:  map 79% reduce 0%
17/11/28 11:45:49 INFO mapreduce.Job:  map 84% reduce 0%
17/11/28 11:45:50 INFO mapreduce.Job:  map 85% reduce 0%
17/11/28 11:45:51 INFO mapreduce.Job:  map 91% reduce 0%
17/11/28 11:45:52 INFO mapreduce.Job:  map 94% reduce 0%
17/11/28 11:45:53 INFO mapreduce.Job:  map 95% reduce 0%
17/11/28 11:45:54 INFO mapreduce.Job:  map 98% reduce 0%
17/11/28 11:45:55 INFO mapreduce.Job:  map 99% reduce 0%
17/11/28 11:45:56 INFO mapreduce.Job:  map 100% reduce 0%
17/11/28 11:46:03 INFO mapreduce.Job:  map 100% reduce 8%
17/11/28 11:46:06 INFO mapreduce.Job:  map 100% reduce 11%
17/11/28 11:46:07 INFO mapreduce.Job:  map 100% reduce 19%
17/11/28 11:46:08 INFO mapreduce.Job:  map 100% reduce 24%
17/11/28 11:46:09 INFO mapreduce.Job:  map 100% reduce 33%
17/11/28 11:46:10 INFO mapreduce.Job:  map 100% reduce 36%
17/11/28 11:46:12 INFO mapreduce.Job:  map 100% reduce 38%
17/11/28 11:46:13 INFO mapreduce.Job:  map 100% reduce 41%
17/11/28 11:46:14 INFO mapreduce.Job:  map 100% reduce 46%
17/11/28 11:46:15 INFO mapreduce.Job:  map 100% reduce 47%
17/11/28 11:46:16 INFO mapreduce.Job:  map 100% reduce 49%
17/11/28 11:46:17 INFO mapreduce.Job:  map 100% reduce 50%
17/11/28 11:46:18 INFO mapreduce.Job:  map 100% reduce 51%
17/11/28 11:46:19 INFO mapreduce.Job:  map 100% reduce 55%
17/11/28 11:46:20 INFO mapreduce.Job:  map 100% reduce 74%
17/11/28 11:46:21 INFO mapreduce.Job:  map 100% reduce 75%
17/11/28 11:46:22 INFO mapreduce.Job:  map 100% reduce 77%
17/11/28 11:46:23 INFO mapreduce.Job:  map 100% reduce 78%
17/11/28 11:46:26 INFO mapreduce.Job:  map 100% reduce 80%
17/11/28 11:46:29 INFO mapreduce.Job:  map 100% reduce 83%
17/11/28 11:46:32 INFO mapreduce.Job:  map 100% reduce 85%
17/11/28 11:46:35 INFO mapreduce.Job:  map 100% reduce 86%
17/11/28 11:46:50 INFO mapreduce.Job:  map 100% reduce 87%
17/11/28 11:46:59 INFO mapreduce.Job:  map 100% reduce 88%
17/11/28 11:47:08 INFO mapreduce.Job:  map 100% reduce 89%
17/11/28 11:47:14 INFO mapreduce.Job:  map 100% reduce 90%
17/11/28 11:47:20 INFO mapreduce.Job:  map 100% reduce 91%
17/11/28 11:47:27 INFO mapreduce.Job:  map 100% reduce 92%
17/11/28 11:47:33 INFO mapreduce.Job:  map 100% reduce 93%
17/11/28 11:47:39 INFO mapreduce.Job:  map 100% reduce 94%
17/11/28 11:47:45 INFO mapreduce.Job:  map 100% reduce 95%
17/11/28 11:47:51 INFO mapreduce.Job:  map 100% reduce 96%
17/11/28 11:47:57 INFO mapreduce.Job:  map 100% reduce 97%
17/11/28 11:48:03 INFO mapreduce.Job:  map 100% reduce 98%
17/11/28 11:48:12 INFO mapreduce.Job:  map 100% reduce 99%
17/11/28 11:48:17 INFO mapreduce.Job:  map 100% reduce 100%
17/11/28 11:48:18 INFO mapreduce.Job: Job job_1511835351299_0002 completed successfully
17/11/28 11:48:18 INFO mapreduce.Job: Counters: 49
	File System Counters
		FILE: Number of bytes read=4444257828
		FILE: Number of bytes written=8826072170
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=10000011856
		HDFS: Number of bytes written=10000000000
		HDFS: Number of read operations=264
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=24
	Job Counters 
		Launched map tasks=76
		Launched reduce tasks=12
		Data-local map tasks=76
		Total time spent by all maps in occupied slots (ms)=1245312
		Total time spent by all reduces in occupied slots (ms)=1265275
		Total time spent by all map tasks (ms)=1245312
		Total time spent by all reduce tasks (ms)=1265275
		Total vcore-seconds taken by all map tasks=1245312
		Total vcore-seconds taken by all reduce tasks=1265275
		Total megabyte-seconds taken by all map tasks=1275199488
		Total megabyte-seconds taken by all reduce tasks=1295641600
	Map-Reduce Framework
		Map input records=100000000
		Map output records=100000000
		Map output bytes=10200000000
		Map output materialized bytes=4370860826
		Input split bytes=11856
		Combine input records=0
		Combine output records=0
		Reduce input groups=100000000
		Reduce shuffle bytes=4370860826
		Reduce input records=100000000
		Reduce output records=100000000
		Spilled Records=200000000
		Shuffled Maps =912
		Failed Shuffles=0
		Merged Map outputs=912
		GC time elapsed (ms)=34232
		CPU time spent (ms)=1110890
		Physical memory (bytes) snapshot=55580270592
		Virtual memory (bytes) snapshot=140331200512
		Total committed heap usage (bytes)=56051105792
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=10000000000
	File Output Format Counters 
		Bytes Written=10000000000
17/11/28 11:48:18 INFO terasort.TeraSort: done
7.81user 0.46system 3:35.45elapsed 3%CPU (0avgtext+0avgdata 250320maxresident)k
0inputs+2216outputs (0major+68925minor)pagefaults 0swaps
[raken@cdh1 ~]$ 




