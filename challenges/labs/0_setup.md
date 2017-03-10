## Cloud Provider
AWS

## Node IPs
```bash
172.31.4.147    ip-172-31-4-147.eu-central-1.compute.internal
172.31.2.93     ip-172-31-2-93.eu-central-1.compute.internal
172.31.5.58     ip-172-31-5-58.eu-central-1.compute.internal   
172.31.6.22     ip-172-31-6-22.eu-central-1.compute.internal
172.31.2.86     ip-172-31-2-86.eu-central-1.compute.internal   
```

## Linux Release
```bash
Red Hat Enterprise Linux Server release 7.2 (Maipo)
```

## Diskspace

```bash
[root@ip-172-31-4-147 ec2-user]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       30G  1.2G   29G   4% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000

```

## Repolist

```bash
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
repo id                                                                              repo name                                                                                          status
!epel/x86_64                                                                         Extra Packages for Enterprise Linux 7 - x86_64                                                     11,310
!rhui-REGION-client-config-server-7/x86_64                                           Red Hat Update Infrastructure 2.0 Client Configuration Server 7                                         4
!rhui-REGION-rhel-server-releases/7Server/x86_64                                     Red Hat Enterprise Linux Server 7 (RPMs)                                                           14,038
!rhui-REGION-rhel-server-rh-common/7Server/x86_64                                    Red Hat Enterprise Linux Server 7 RH Common (RPMs)                                                    209
repolist: 25,561

```

## User
```bash
neymar:x:2010:2010::/home/neymar:/bin/bash
ronaldo:x:2016:2016::/home/ronaldo:/bin/bash
```

##Groups

```bash
neymar:x:2010:
barca:x:2011:ronaldo
merengues:x:2012:neymar
ronaldo:x:2016:
```