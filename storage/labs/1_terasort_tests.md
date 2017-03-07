[hdfs@ip-172-31-7-126 ec2-user]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D dfs.block.size=33554432 -D mapred.map.tasks=4 10000000 /mihenn87/teragen2
17/03/07 07:27:35 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-11-113.us-west-2.compute.internal/172.31.11.113:8032
17/03/07 07:27:36 INFO terasort.TeraSort: Generating 10000000 using 4
17/03/07 07:27:36 INFO mapreduce.JobSubmitter: number of splits:4
17/03/07 07:27:36 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/03/07 07:27:36 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/03/07 07:27:36 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1488888367319_0002
17/03/07 07:27:36 INFO impl.YarnClientImpl: Submitted application application_1488888367319_0002
17/03/07 07:27:36 INFO mapreduce.Job: The url to track the job: http://ip-172-31-11-113.us-west-2.compute.internal:8088/proxy/application_1488888367319_0002/
17/03/07 07:27:36 INFO mapreduce.Job: Running job: job_1488888367319_0002
17/03/07 07:27:41 INFO mapreduce.Job: Job job_1488888367319_0002 running in uber mode : false
17/03/07 07:27:41 INFO mapreduce.Job:  map 0% reduce 0%
17/03/07 07:27:53 INFO mapreduce.Job:  map 100% reduce 0%
17/03/07 07:27:54 INFO mapreduce.Job: Job job_1488888367319_0002 completed successfully
17/03/07 07:27:54 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=498308
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=337
                HDFS: Number of bytes written=1000000000
                HDFS: Number of read operations=16
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=8
        Job Counters
                Launched map tasks=4
                Other local map tasks=4
                Total time spent by all maps in occupied slots (ms)=34445
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=34445
                Total vcore-seconds taken by all map tasks=34445
                Total megabyte-seconds taken by all map tasks=35271680
        Map-Reduce Framework
                Map input records=10000000
                Map output records=10000000
                Input split bytes=337
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=371
                CPU time spent (ms)=27960
                Physical memory (bytes) snapshot=1490649088
                Virtual memory (bytes) snapshot=6336425984
                Total committed heap usage (bytes)=1733296128
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=21472776955442690
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=1000000000
[hdfs@ip-172-31-7-126 ec2-user]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort  /mihenn87/teragen2 /mihenn87/terasort2
17/03/07 07:34:21 INFO terasort.TeraSort: starting
17/03/07 07:34:22 INFO input.FileInputFormat: Total input paths to process : 4
Spent 139ms computing base-splits.
Spent 2ms computing TeraScheduler splits.
Computing input splits took 142ms
Sampling 10 splits of 32
Making 8 from 100000 sampled records
Computing parititions took 751ms
Spent 896ms computing partitions.
17/03/07 07:34:23 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-11-113.us-west-2.compute.internal/172.31.11.113:8032
17/03/07 07:34:23 INFO mapreduce.JobSubmitter: number of splits:32
17/03/07 07:34:24 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1488888367319_0003
17/03/07 07:34:24 INFO impl.YarnClientImpl: Submitted application application_1488888367319_0003
17/03/07 07:34:24 INFO mapreduce.Job: The url to track the job: http://ip-172-31-11-113.us-west-2.compute.internal:8088/proxy/application_1488888367319_0003/
17/03/07 07:34:24 INFO mapreduce.Job: Running job: job_1488888367319_0003
17/03/07 07:34:29 INFO mapreduce.Job: Job job_1488888367319_0003 running in uber mode : false
17/03/07 07:34:29 INFO mapreduce.Job:  map 0% reduce 0%
17/03/07 07:34:41 INFO mapreduce.Job:  map 28% reduce 0%
17/03/07 07:34:43 INFO mapreduce.Job:  map 31% reduce 0%
17/03/07 07:34:44 INFO mapreduce.Job:  map 41% reduce 0%
17/03/07 07:34:50 INFO mapreduce.Job:  map 66% reduce 0%
17/03/07 07:34:51 INFO mapreduce.Job:  map 69% reduce 0%
17/03/07 07:34:56 INFO mapreduce.Job:  map 84% reduce 0%
17/03/07 07:34:57 INFO mapreduce.Job:  map 91% reduce 0%
17/03/07 07:35:00 INFO mapreduce.Job:  map 100% reduce 0%
17/03/07 07:35:07 INFO mapreduce.Job:  map 100% reduce 25%
17/03/07 07:35:11 INFO mapreduce.Job:  map 100% reduce 97%
17/03/07 07:35:12 INFO mapreduce.Job:  map 100% reduce 100%
17/03/07 07:35:12 INFO mapreduce.Job: Job job_1488888367319_0003 completed successfully
17/03/07 07:35:12 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=439892502
                FILE: Number of bytes written=878989511
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=1000003680
                HDFS: Number of bytes written=1000000000
                HDFS: Number of read operations=120
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=32
                Launched reduce tasks=8
                Data-local map tasks=32
                Total time spent by all maps in occupied slots (ms)=294203
                Total time spent by all reduces in occupied slots (ms)=92795
                Total time spent by all map tasks (ms)=294203
                Total time spent by all reduce tasks (ms)=92795
                Total vcore-seconds taken by all map tasks=294203
                Total vcore-seconds taken by all reduce tasks=92795
                Total megabyte-seconds taken by all map tasks=301263872
                Total megabyte-seconds taken by all reduce tasks=95022080
        Map-Reduce Framework
                Map input records=10000000
                Map output records=10000000
                Map output bytes=1020000000
                Map output materialized bytes=434056307
                Input split bytes=3680
                Combine input records=0
                Combine output records=0
                Reduce input groups=10000000
                Reduce shuffle bytes=434056307
                Reduce input records=10000000
                Reduce output records=10000000
                Spilled Records=20000000
                Shuffled Maps =256
                Failed Shuffles=0
                Merged Map outputs=256
                GC time elapsed (ms)=4303
                CPU time spent (ms)=171300
                Physical memory (bytes) snapshot=18447687680
                Virtual memory (bytes) snapshot=63662923776
                Total committed heap usage (bytes)=20906508288
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=1000000000
        File Output Format Counters
                Bytes Written=1000000000
17/03/07 07:35:12 INFO terasort.TeraSort: done
