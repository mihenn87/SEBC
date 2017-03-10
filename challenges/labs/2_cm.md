```bash
[root@ip-172-31-2-93 ec2-user]# ls /etc/yum.repos.d
cloudera-manager.repo  epel-testing.repo     mysql-community-source.repo  redhat-rhui-client-config.repo  rhui-load-balancers.conf
epel.repo              mysql-community.repo  redhat.repo                  redhat-rhui.repo

```

## Script

```bash
/usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-4-147.eu-central-1.compute.internal -utemp -ptemp --scm-host ip-172-31-2-93.eu-central-1.compute.internal scm scm scm
```
