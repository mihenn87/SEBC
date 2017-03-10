```bash
[root@ip-172-31-2-93 ec2-user]# ls /etc/yum.repos.d
cloudera-manager.repo  epel-testing.repo     mysql-community-source.repo  redhat-rhui-client-config.repo  rhui-load-balancers.conf
epel.repo              mysql-community.repo  redhat.repo                  redhat-rhui.repo

```

## Script

```bash
/usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-4-147.eu-central-1.compute.internal -utemp -ptemp --scm-host ip-172-31-2-93.eu-central-1.compute.internal scm scm scm
```


## First Line of Log

```
2017-03-10 04:44:44,389 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.9.1 (#8 built by jenkins on 20170112-1158 git: a66d8bbdbe8bc3ee54235e55423f2f76c7d9f3b1)

```

## Jetty
```
[root@ip-172-31-2-93 cloudera-scm-server]# cat /var/log/cloudera-scm-server/cloudera-scm-server.log | grep 'Started Jetty server'
2017-03-10 04:45:58,234 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.
```