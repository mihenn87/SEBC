```bash
[root@ip-172-31-7-126 ~]# kadmin.local
Authenticating as principal root/admin@MIHENN87.LOCAL with password.

kadmin.local:  xst -k hdfs-unmerged.keytab hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL
Entry for principal hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL with kvno 4, encryption type aes256-cts-hmac-sha1-96 added to keytab WRFILE:hdfs-unmerged.keytab.
Entry for principal hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL with kvno 4, encryption type aes128-cts-hmac-sha1-96 added to keytab WRFILE:hdfs-unmerged.keytab.
Entry for principal hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL with kvno 4, encryption type des3-cbc-sha1 added to keytab WRFILE:hdfs-unmerged.keytab.
Entry for principal hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL with kvno 4, encryption type arcfour-hmac added to keytab WRFILE:hdfs-unmerged.keytab.
Entry for principal hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL with kvno 4, encryption type camellia256-cts-cmac added to keytab WRFILE:hdfs-unmerged.keytab.
Entry for principal hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL with kvno 4, encryption type camellia128-cts-cmac added to keytab WRFILE:hdfs-unmerged.keytab.
Entry for principal hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL with kvno 4, encryption type des-hmac-sha1 added to keytab WRFILE:hdfs-unmerged.keytab.
Entry for principal hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL with kvno 4, encryption type des-cbc-md5 added to keytab WRFILE:hdfs-unmerged.keytab.
kadmin.local:  exit

[root@ip-172-31-7-126 ~]# kinit -k -t hdfs-unmerged.keytab hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL

[root@ip-172-31-7-126 ~]# hadoop fs -ls /
Found 6 items
drwxr-xr-x   - hdfs supergroup          0 2017-03-07 07:34 /mihenn87
drwxr-xr-x   - hdfs supergroup          0 2017-03-07 08:32 /precious
drwxr-xr-x   - hdfs supergroup          0 2017-03-07 11:54 /results
drwxr-xr-x   - hdfs supergroup          0 2017-03-07 05:38 /sebastiankramp
drwxrwxrwx   - hdfs supergroup          0 2017-03-09 04:14 /tmp
drwxr-xr-x   - hdfs supergroup          0 2017-03-08 09:53 /user

[root@ip-172-31-7-126 ~]# klist
Ticket cache: FILE:/tmp/krb5cc_0
Default principal: hdfs/ip-172-31-7-126.us-west-2.compute.internal@MIHENN87.LOCAL

Valid starting       Expires              Service principal
03/09/2017 04:31:38  03/10/2017 04:31:38  krbtgt/MIHENN87.LOCAL@MIHENN87.LOCAL
        renew until 03/16/2017 05:31:38
		
```