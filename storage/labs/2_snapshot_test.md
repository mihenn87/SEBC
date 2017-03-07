[hdfs@ip-172-31-7-126 hdfs]$ hadoop fs -put /home/hdfs/SEBC.zip /precious
[hdfs@ip-172-31-7-126 hdfs]$ hdfs dfs -createSnapshot /precious [SEBC_Snapshot_2]
Created snapshot /precious/.snapshot/[SEBC_Snapshot_2]
[hdfs@ip-172-31-7-126 hdfs]$ hadoop fs -rm  /precious/SEBC.zip
17/03/07 08:32:35 INFO fs.TrashPolicyDefault: Moved: 'hdfs://nameservice1/precious/SEBC.zip' to trash at: hdfs://nameservice1/user/hdfs/.Trash/Current/precious/SEBC.zip1488893555760
