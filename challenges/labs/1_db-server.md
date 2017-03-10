## Hostname

```bash
[root@ip-172-31-4-147 ec2-user]# hostname
ip-172-31-4-147.eu-central-1.compute.internal
```


## MySQL Version

```bash
[root@ip-172-31-4-147 ec2-user]# mysql --version
mysql  Ver 14.14 Distrib 5.6.35, for Linux (x86_64) using  EditLine wrapper
```

## Databases

```
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
9 rows in set (0.00 sec)
```