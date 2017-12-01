<h1>CLOUDERA BOOT CAMP - Challenges - Dec 1, 2017 - CDMX</h1>

<h2>Challenge 4 HDFS TESTING</h2>

<br>
<b>1</b><br>
<b>TERAGEN</b><br>
<br>

[root@rkn1 raken]# HADOOP_USER_NAME=hdfs hdfs dfs -chmod 777 /user/saturn<br>
[root@rkn1 raken]# <CODE>HADOOP_USER_NAME=saturn time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen 65536000 /user/saturn/tgen</code><br>
17/12/01 14:26:42 INFO Configuration.deprecation: session.id is deprecated. Instead, use dfs.metrics.session-id<br>
17/12/01 14:26:42 INFO jvm.JvmMetrics: Initializing JVM Metrics with processName=JobTracker, sessionId=<br>
17/12/01 14:26:42 INFO terasort.TeraSort: Generating 65536000 using 1<br>
17/12/01 14:26:42 INFO mapreduce.JobSubmitter: number of splits:1<br>
17/12/01 14:26:42 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_local604591396_0001<br>
17/12/01 14:26:42 INFO mapreduce.Job: The url to track the job: http://localhost:8080/<br>
17/12/01 14:26:42 INFO mapreduce.Job: Running job: job_local604591396_0001<br>
17/12/01 14:26:42 INFO mapred.LocalJobRunner: OutputCommitter set in config null<br>
17/12/01 14:26:42 INFO output.FileOutputCommitter: File Output Committer Algorithm version is 1<br>
17/12/01 14:26:42 INFO mapred.LocalJobRunner: OutputCommitter is org.apache.hadoop.mapreduce.lib.output.FileOutputCommitter<br>
17/12/01 14:26:42 INFO mapred.LocalJobRunner: Waiting for map tasks<br>
17/12/01 14:26:42 INFO mapred.LocalJobRunner: Starting task: attempt_local604591396_0001_m_000000_0<br>
17/12/01 14:26:42 INFO output.FileOutputCommitter: File Output Committer Algorithm version is 1<br>
17/12/01 14:26:42 INFO mapred.Task:  Using ResourceCalculatorProcessTree : [ ]<br>
17/12/01 14:26:42 INFO mapred.MapTask: Processing split: org.apache.hadoop.examples.terasort.TeraGen$RangeInputFormat$RangeInputSplit@12e6ca10<br>
17/12/01 14:26:43 INFO mapreduce.Job: Job job_local604591396_0001 running in uber mode : false<br>
17/12/01 14:26:43 INFO mapreduce.Job:  map 0% reduce 0%<br>
17/12/01 14:26:48 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:26:49 INFO mapreduce.Job:  map 8% reduce 0%<br>
17/12/01 14:26:51 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:26:52 INFO mapreduce.Job:  map 13% reduce 0%
17/12/01 14:26:54 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:26:55 INFO mapreduce.Job:  map 17% reduce 0%<br>
17/12/01 14:26:57 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:26:58 INFO mapreduce.Job:  map 21% reduce 0%<br>
17/12/01 14:27:00 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:01 INFO mapreduce.Job:  map 25% reduce 0%<br>
17/12/01 14:27:03 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:04 INFO mapreduce.Job:  map 27% reduce 0%<br>
17/12/01 14:27:06 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:07 INFO mapreduce.Job:  map 29% reduce 0%<br>
17/12/01 14:27:09 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:10 INFO mapreduce.Job:  map 31% reduce 0%<br>
17/12/01 14:27:12 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:13 INFO mapreduce.Job:  map 35% reduce 0%<br>
17/12/01 14:27:15 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:16 INFO mapreduce.Job:  map 37% reduce 0%<br>
17/12/01 14:27:18 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:19 INFO mapreduce.Job:  map 41% reduce 0%<br>
17/12/01 14:27:21 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:22 INFO mapreduce.Job:  map 43% reduce 0%<br>
17/12/01 14:27:24 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:25 INFO mapreduce.Job:  map 48% reduce 0%<br>
17/12/01 14:27:27 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:28 INFO mapreduce.Job:  map 51% reduce 0%<br>
17/12/01 14:27:30 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:31 INFO mapreduce.Job:  map 55% reduce 0%<br>
17/12/01 14:27:33 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:34 INFO mapreduce.Job:  map 57% reduce 0%<br>
17/12/01 14:27:36 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:37 INFO mapreduce.Job:  map 60% reduce 0%<br>
17/12/01 14:27:39 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:40 INFO mapreduce.Job:  map 63% reduce 0%<br>
17/12/01 14:27:42 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:43 INFO mapreduce.Job:  map 66% reduce 0%<br>
17/12/01 14:27:45 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:46 INFO mapreduce.Job:  map 69% reduce 0%<br>
17/12/01 14:27:48 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:49 INFO mapreduce.Job:  map 71% reduce 0%<br>
17/12/01 14:27:51 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:52 INFO mapreduce.Job:  map 73% reduce 0%<br>
17/12/01 14:27:54 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:55 INFO mapreduce.Job:  map 76% reduce 0%<br>
17/12/01 14:27:57 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:27:58 INFO mapreduce.Job:  map 79% reduce 0%<br>
17/12/01 14:28:00 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:01 INFO mapreduce.Job:  map 81% reduce 0%<br>
17/12/01 14:28:03 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:04 INFO mapreduce.Job:  map 84% reduce 0%<br>
17/12/01 14:28:06 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:07 INFO mapreduce.Job:  map 85% reduce 0%<br>
17/12/01 14:28:09 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:10 INFO mapreduce.Job:  map 88% reduce 0%<br>
17/12/01 14:28:12 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:13 INFO mapreduce.Job:  map 90% reduce 0%<br>
17/12/01 14:28:15 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:16 INFO mapreduce.Job:  map 93% reduce 0%<br>
17/12/01 14:28:18 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:19 INFO mapreduce.Job:  map 95% reduce 0%<br>
17/12/01 14:28:21 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:22 INFO mapreduce.Job:  map 98% reduce 0%<br>
17/12/01 14:28:24 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:25 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:25 INFO mapred.Task: Task:attempt_local60459<br>1396_0001_m_000000_0 is done. And is in the process of committing
17/12/01 14:28:25 INFO mapred.LocalJobRunner: map > map<br>
17/12/01 14:28:25 INFO mapred.Task: Task attempt_local60459<br>1396_0001_m_000000_0 is allowed to commit now
17/12/01 14:28:25 INFO mapreduce.Job:  map 100% reduce 0%<br>
17/12/01 14:28:26 INFO output.FileOutputCommitter: Saved outp<br>ut of task 'attempt_local604591396_0001_m_000000_0' to hdfs://rkn2.northcentralus.cloudapp.azure.com:8020/user/saturn/tgen/_temporary/0/task_local604591396_0001_m_000000
17/12/01 14:28:26 INFO mapred.LocalJobRunner: map<br>
17/12/01 14:28:26 INFO mapred.Task: Task 'attempt_local604591396_0001_m_000000_0' done.<br>
17/12/01 14:28:26 INFO mapred.LocalJobRunner: Finishing task: attempt_local604591396_0001_m_000000_0<br>
17/12/01 14:28:26 INFO mapred.LocalJobRunner: map task executor complete.<br>
17/12/01 14:28:27 INFO mapreduce.Job: Job job_local604591396_0001 completed successfully<br>
17/12/01 14:28:27 INFO mapreduce.Job: Counters: 21<br>
	File System Counters<br>
		FILE: Number of bytes read=276333<br>
		FILE: Number of bytes written=565335<br>
		FILE: Number of read operations=0<br>
		FILE: Number of large read operations=0<br>
		FILE: Number of write operations=0<br>
		HDFS: Number of bytes read=0<br>
		HDFS: Number of bytes written=6553600000<br>
		HDFS: Number of read operations=4<br>
		HDFS: Number of large read operations=0<br>
		HDFS: Number of write operations=3<br>
	Map-Reduce Framework<br>
		Map input records=65536000<br>
		Map output records=65536000<br>
		Input split bytes=83<br>
		Spilled Records=0<br>
		Failed Shuffles=0<br>
		Merged Map outputs=0<br>
		GC time elapsed (ms)=820<br>
		Total committed heap usage (<br>bytes)=252706816
	org.apache.hadoop.examples.terasort.<br>TeraGen$Counters
		CHECKSUM=140750829423462787<br>
	File Input Format Counters <br>
		Bytes Read=0<br>
	File Output Format Counters <br>
		Bytes Written=6553600000<br>
77.16user 6.19system 1:47.62elapsed 77%CPU (0avgtext+0avgdata 230592maxresident)k<br>
48inputs+3360outputs (1major+107128minor)pagefaults 0swaps<br>
[root@rkn1 raken]# <br>


<b>2</b><br>
<b>TIME</b><br>
<br>
77.16user 6.19system 1:47.62elapsed 77%CPU (0avgtext+0avgdata 230592maxresident)k<br>
48inputs+3360outputs (1major+107128minor)pagefaults 0swaps<br>

<b>3</b><br>
<b>hdfs dfs -ls /user/saturn/tgen</b><br>
<br>

 hdfs dfs -ls /user/saturn/tgen<br>
Found 2 items<br>
-rw-r--r--   3 saturn supergroup          0 2017-12-01 14:28 /user/saturn/tgen/_SUCCESS<br>
-rw-r--r--   3 saturn supergroup 6553600000 2017-12-01 14:28 /user/saturn/tgen/part-m-00000<br>
[root@rkn1 raken]# <br>


<b>3</b><br>
<b>hadoop fsck -blocks /user/saturn</b><br>
<br>

[root@rkn1 raken]# <code>hadoop fsck -blocks /user/saturn</code><br>
DEPRECATED: Use of this script to execute hdfs command is deprecated.<br>
Instead use the hdfs command for it.<br>
<br>
Connecting to namenode via http://rkn2.northcentralus.cloudapp.azure.com:50070<br>
FSCK started by root (auth:SIMPLE) from /10.0.1.9 for path /user/saturn at Fri Dec 01 14:32:20 EST 2017<br>
..Status: HEALTHY<br>
 Total size:	6553600000 B<br>
 Total dirs:	2<br>
 Total files:	2<br>
 Total symlinks:		0<br>
 Total blocks (validated):	49 (avg. block size 133746938 B)<br>
 Minimally replicated blocks:	49 (100.0 %)<br>
 Over-replicated blocks:	0 (0.0 %)<br>
 Under-replicated blocks:	0 (0.0 %)<br>
 Mis-replicated blocks:		0 (0.0 %)<br>
 Default replication factor:	3<br>
 Average block replication:	3.0<br>
 Corrupt blocks:		0<br>
 Missing replicas:		0 (0.0 %)<br>
 Number of data-nodes:		3<br>
 Number of racks:		1<br>
FSCK ended at Fri Dec 01 14:32:20 EST 2017 in 3 milliseconds<br>
<br>

The filesystem under path '/user/saturn' is HEALTHY<br>
[root@rkn1 raken]# <br>

 
