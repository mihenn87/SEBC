## User

```bash

[hdfs@ip-172-31-2-93 ec2-user]$ hdfs dfs -ls /user
Found 6 items
drwxrwxrwx   - mapred  hadoop             0 2017-03-10 05:16 /user/history
drwxrwxr-t   - hive    hive               0 2017-03-10 05:17 /user/hive
drwxrwxr-x   - hue     hue                0 2017-03-10 05:17 /user/hue
drwxr-xr-x   - neymar  merengues          0 2017-03-10 05:17 /user/neymar
drwxrwxr-x   - oozie   oozie              0 2017-03-10 05:18 /user/oozie
drwxr-xr-x   - ronaldo barca              0 2017-03-10 05:17 /user/ronaldo

```

```
[hdfs@ip-172-31-2-93 ec2-user]$ curl admin:admin@localhost:7180/api/v14/hosts
{
  "items" : [ {
    "hostId" : "i-047e962ad108e8391",
    "ipAddress" : "172.31.2.86",
    "hostname" : "ip-172-31-2-86.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-93.eu-central-1.compute.internal:7180/cmf/hostRedirect/i-047e962ad108e8391",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-027a45f99afcef6ed",
    "ipAddress" : "172.31.2.93",
    "hostname" : "ip-172-31-2-93.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-93.eu-central-1.compute.internal:7180/cmf/hostRedirect/i-027a45f99afcef6ed",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-09b0e3a8acc9689ca",
    "ipAddress" : "172.31.4.147",
    "hostname" : "ip-172-31-4-147.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-93.eu-central-1.compute.internal:7180/cmf/hostRedirect/i-09b0e3a8acc9689ca",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-0038c8ab9d9d448ac",
    "ipAddress" : "172.31.5.58",
    "hostname" : "ip-172-31-5-58.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-93.eu-central-1.compute.internal:7180/cmf/hostRedirect/i-0038c8ab9d9d448ac",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-04399bd9cf507e4a5",
    "ipAddress" : "172.31.6.22",
    "hostname" : "ip-172-31-6-22.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-93.eu-central-1.compute.internal:7180/cmf/hostRedirect/i-04399bd9cf507e4a5",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  } ]
}
```