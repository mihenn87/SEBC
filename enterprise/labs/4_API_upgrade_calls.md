## API Version

[root@ip-172-31-7-126 ~]# curl -u mihenn87:cloudera 'http://localhost:7180/api/version'  
```json
v15
```

## CM Version

[root@ip-172-31-7-126 ~]# curl -u mihenn87:cloudera 'http://localhost:7180/api/v15/cm/version'
```json
{
  "version" : "5.10.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20170120-1037",
  "gitHash" : "aa0b5cd5eceaefe2f971c13ab657020d96bb842a",
  "snapshot" : false
}
```

## Users

[root@ip-172-31-7-126 ~]# curl -u mihenn87:cloudera 'http://localhost:7180/api/v15/users'
```json
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ]
  }, {
    "name" : "mihenn87",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  } ]
}
```

## Database

[root@ip-172-31-7-126 ~]# curl -u mihenn87:cloudera 'http://localhost:7180/api/v15/cm/scmDbInfo'
```json
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}
```
