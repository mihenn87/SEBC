## Teragen

[neymar@ip-172-31-2-93 ec2-user]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D dfs.block.size=16777216 -D mapred.map.tasks=4 65536000 /user/neymar/tgen640-2
17/03/10 05:48:17 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-2-86.eu-central-1.compute.internal/172.31.2.86:8032
17/03/10 05:48:17 INFO terasort.TeraSort: Generating 65536000 using 4
17/03/10 05:48:17 INFO mapreduce.JobSubmitter: number of splits:4
17/03/10 05:48:17 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/03/10 05:48:17 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/03/10 05:48:17 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1489142135298_0002
17/03/10 05:48:18 INFO impl.YarnClientImpl: Submitted application application_1489142135298_0002
17/03/10 05:48:18 INFO mapreduce.Job: The url to track the job: http://ip-172-31-2-86.eu-central-1.compute.internal:8088/proxy/application_1489142135298_0002/
17/03/10 05:48:18 INFO mapreduce.Job: Running job: job_1489142135298_0002
17/03/10 05:48:23 INFO mapreduce.Job: Job job_1489142135298_0002 running in uber mode : false
17/03/10 05:48:23 INFO mapreduce.Job:  map 0% reduce 0%
17/03/10 05:48:34 INFO mapreduce.Job:  map 4% reduce 0%
17/03/10 05:48:37 INFO mapreduce.Job:  map 7% reduce 0%
17/03/10 05:48:38 INFO mapreduce.Job:  map 13% reduce 0%
17/03/10 05:48:39 INFO mapreduce.Job:  map 16% reduce 0%
17/03/10 05:48:40 INFO mapreduce.Job:  map 18% reduce 0%
17/03/10 05:48:41 INFO mapreduce.Job:  map 21% reduce 0%
17/03/10 05:48:42 INFO mapreduce.Job:  map 22% reduce 0%
17/03/10 05:48:43 INFO mapreduce.Job:  map 23% reduce 0%
17/03/10 05:48:44 INFO mapreduce.Job:  map 25% reduce 0%
17/03/10 05:48:45 INFO mapreduce.Job:  map 26% reduce 0%
17/03/10 05:48:46 INFO mapreduce.Job:  map 27% reduce 0%
17/03/10 05:48:47 INFO mapreduce.Job:  map 28% reduce 0%
17/03/10 05:48:48 INFO mapreduce.Job:  map 29% reduce 0%
17/03/10 05:48:53 INFO mapreduce.Job:  map 30% reduce 0%
17/03/10 05:48:56 INFO mapreduce.Job:  map 31% reduce 0%
17/03/10 05:48:58 INFO mapreduce.Job:  map 32% reduce 0%
17/03/10 05:49:05 INFO mapreduce.Job:  map 33% reduce 0%
17/03/10 05:49:14 INFO mapreduce.Job:  map 34% reduce 0%
17/03/10 05:49:20 INFO mapreduce.Job:  map 35% reduce 0%
17/03/10 05:49:35 INFO mapreduce.Job:  map 36% reduce 0%
17/03/10 05:49:39 INFO mapreduce.Job:  map 37% reduce 0%
17/03/10 05:49:41 INFO mapreduce.Job:  map 38% reduce 0%
17/03/10 05:49:42 INFO mapreduce.Job:  map 39% reduce 0%
17/03/10 05:49:52 INFO mapreduce.Job:  map 40% reduce 0%
17/03/10 05:49:53 INFO mapreduce.Job:  map 41% reduce 0%
17/03/10 05:49:55 INFO mapreduce.Job:  map 42% reduce 0%
17/03/10 05:50:02 INFO mapreduce.Job:  map 44% reduce 0%
17/03/10 05:50:03 INFO mapreduce.Job:  map 49% reduce 0%
17/03/10 05:50:04 INFO mapreduce.Job:  map 52% reduce 0%
17/03/10 05:50:05 INFO mapreduce.Job:  map 53% reduce 0%
17/03/10 05:50:06 INFO mapreduce.Job:  map 55% reduce 0%
17/03/10 05:50:14 INFO mapreduce.Job:  map 56% reduce 0%
17/03/10 05:50:21 INFO mapreduce.Job:  map 57% reduce 0%
17/03/10 05:50:27 INFO mapreduce.Job:  map 58% reduce 0%
17/03/10 05:50:32 INFO mapreduce.Job:  map 60% reduce 0%
17/03/10 05:50:33 INFO mapreduce.Job:  map 62% reduce 0%
17/03/10 05:50:34 INFO mapreduce.Job:  map 64% reduce 0%
17/03/10 05:50:35 INFO mapreduce.Job:  map 65% reduce 0%
17/03/10 05:50:43 INFO mapreduce.Job:  map 66% reduce 0%
17/03/10 05:50:45 INFO mapreduce.Job:  map 67% reduce 0%
17/03/10 05:50:46 INFO mapreduce.Job:  map 68% reduce 0%
17/03/10 05:50:49 INFO mapreduce.Job:  map 69% reduce 0%
17/03/10 05:50:53 INFO mapreduce.Job:  map 70% reduce 0%
17/03/10 05:50:55 INFO mapreduce.Job:  map 71% reduce 0%
17/03/10 05:51:06 INFO mapreduce.Job:  map 72% reduce 0%
17/03/10 05:51:10 INFO mapreduce.Job:  map 73% reduce 0%
17/03/10 05:51:20 INFO mapreduce.Job:  map 74% reduce 0%
17/03/10 05:51:22 INFO mapreduce.Job:  map 76% reduce 0%
17/03/10 05:51:25 INFO mapreduce.Job:  map 77% reduce 0%
17/03/10 05:51:33 INFO mapreduce.Job:  map 78% reduce 0%
17/03/10 05:51:34 INFO mapreduce.Job:  map 80% reduce 0%
17/03/10 05:51:35 INFO mapreduce.Job:  map 81% reduce 0%
17/03/10 05:51:37 INFO mapreduce.Job:  map 82% reduce 0%
17/03/10 05:51:39 INFO mapreduce.Job:  map 83% reduce 0%
17/03/10 05:51:40 INFO mapreduce.Job:  map 84% reduce 0%
17/03/10 05:51:52 INFO mapreduce.Job:  map 85% reduce 0%
17/03/10 05:51:58 INFO mapreduce.Job:  map 86% reduce 0%
17/03/10 05:52:07 INFO mapreduce.Job:  map 87% reduce 0%
17/03/10 05:52:16 INFO mapreduce.Job:  map 92% reduce 0%
17/03/10 05:52:19 INFO mapreduce.Job:  map 98% reduce 0%
17/03/10 05:52:22 INFO mapreduce.Job:  map 99% reduce 0%
17/03/10 05:52:25 INFO mapreduce.Job:  map 100% reduce 0%
17/03/10 05:52:28 INFO mapreduce.Job: Job job_1489142135298_0002 completed successfully
17/03/10 05:52:30 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=491772
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=339
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=16
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=8
        Job Counters
                Launched map tasks=4
                Other local map tasks=4
                Total time spent by all maps in occupied slots (ms)=912767
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=912767
                Total vcore-seconds taken by all map tasks=912767
                Total megabyte-seconds taken by all map tasks=934673408
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=339
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1350
                CPU time spent (ms)=119060
                Physical memory (bytes) snapshot=956710912
                Virtual memory (bytes) snapshot=6297985024
                Total committed heap usage (bytes)=1012400128
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000



```

## ls

```
[neymar@ip-172-31-2-93 ec2-user]$ hdfs dfs -ls /user/neymar/tgen640-2
Found 5 items
-rw-r--r--   3 neymar hadoop          0 2017-03-10 05:52 /user/neymar/tgen640-2/_SUCCESS
-rw-r--r--   3 neymar hadoop 1638400000 2017-03-10 05:52 /user/neymar/tgen640-2/part-m-00000
-rw-r--r--   3 neymar hadoop 1638400000 2017-03-10 05:52 /user/neymar/tgen640-2/part-m-00001
-rw-r--r--   3 neymar hadoop 1638400000 2017-03-10 05:52 /user/neymar/tgen640-2/part-m-00002
-rw-r--r--   3 neymar hadoop 1638400000 2017-03-10 05:51 /user/neymar/tgen640-2/part-m-00003

```