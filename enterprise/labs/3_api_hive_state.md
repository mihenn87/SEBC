## stop

[root@ip-172-31-7-126 ~]# curl -X POST -u mihenn87:cloudera 'http://localhost:7180/api/v1/clusters/mihenn87/services/hive/commands/stop'
```json{
  "id" : 1170,
  "name" : "Stop",
  "startTime" : "2017-03-08T10:19:17.086Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}```

## start

[root@ip-172-31-7-126 ~]# curl -X POST -u mihenn87:cloudera 'http://localhost:7180/api/v1/clusters/mihenn87/services/hive/commands/start'
```json{
  "id" : 1173,
  "name" : "Start",
  "startTime" : "2017-03-08T10:19:34.848Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}```

## state

[root@ip-172-31-7-126 ~]# curl -u mihenn87:cloudera 'http://localhost:7180/api/v1/clusters/mihenn87/services/hive'
```json{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-7-126.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive",
  "serviceState" : "STARTING",
  "healthSummary" : "DISABLED",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "DISABLED"
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "DISABLED"
  } ],
  "configStale" : false
}```