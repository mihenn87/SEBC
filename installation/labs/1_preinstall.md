﻿#vm-swappiness

[root@ip-172-31-4-130 ec2-user]# cat /proc/sys/vm/swappiness  
1

[root@ip-172-31-4-23 ec2-user]# cat /proc/sys/vm/swappiness  
1

[root@ip-172-31-11-113 ec2-user]# cat /proc/sys/vm/swappiness  
1

[root@ip-172-31-3-32 ec2-user]# cat /proc/sys/vm/swappiness  
1

[root@ip-172-31-7-126 ~]# cat /proc/sys/vm/swappiness  
1

#mount

[root@ip-172-31-4-130 ec2-user]# mount
sysfs on /sys type sysfs (rw,nosuid,nodev,noexec,relatime)
proc on /proc type proc (rw,nosuid,nodev,noexec,relatime)
devtmpfs on /dev type devtmpfs (rw,nosuid,size=7599360k,nr_inodes=1899840,mode=755)
securityfs on /sys/kernel/security type securityfs (rw,nosuid,nodev,noexec,relatime)
tmpfs on /dev/shm type tmpfs (rw,nosuid,nodev)
devpts on /dev/pts type devpts (rw,nosuid,noexec,relatime,gid=5,mode=620,ptmxmode=000)
tmpfs on /run type tmpfs (rw,nosuid,nodev,mode=755)
tmpfs on /sys/fs/cgroup type tmpfs (ro,nosuid,nodev,noexec,mode=755)
cgroup on /sys/fs/cgroup/systemd type cgroup (rw,nosuid,nodev,noexec,relatime,xattr,release_agent=/usr/lib/systemd/systemd-cgroups-agent,name=systemd)
pstore on /sys/fs/pstore type pstore (rw,nosuid,nodev,noexec,relatime)
cgroup on /sys/fs/cgroup/blkio type cgroup (rw,nosuid,nodev,noexec,relatime,blkio)
cgroup on /sys/fs/cgroup/cpu,cpuacct type cgroup (rw,nosuid,nodev,noexec,relatime,cpuacct,cpu)
cgroup on /sys/fs/cgroup/hugetlb type cgroup (rw,nosuid,nodev,noexec,relatime,hugetlb)
cgroup on /sys/fs/cgroup/freezer type cgroup (rw,nosuid,nodev,noexec,relatime,freezer)
cgroup on /sys/fs/cgroup/perf_event type cgroup (rw,nosuid,nodev,noexec,relatime,perf_event)
cgroup on /sys/fs/cgroup/memory type cgroup (rw,nosuid,nodev,noexec,relatime,memory)
cgroup on /sys/fs/cgroup/cpuset type cgroup (rw,nosuid,nodev,noexec,relatime,cpuset)
cgroup on /sys/fs/cgroup/devices type cgroup (rw,nosuid,nodev,noexec,relatime,devices)
cgroup on /sys/fs/cgroup/net_cls type cgroup (rw,nosuid,nodev,noexec,relatime,net_cls)
configfs on /sys/kernel/config type configfs (rw,relatime)
/dev/xvda2 on / type xfs (rw,relatime,attr2,inode64,noquota)
mqueue on /dev/mqueue type mqueue (rw,relatime)
debugfs on /sys/kernel/debug type debugfs (rw,relatime)
hugetlbfs on /dev/hugepages type hugetlbfs (rw,relatime)
systemd-1 on /proc/sys/fs/binfmt_misc type autofs (rw,relatime,fd=31,pgrp=1,timeout=300,minproto=5,maxproto=5,direct)
binfmt_misc on /proc/sys/fs/binfmt_misc type binfmt_misc (rw,relatime)
tmpfs on /run/user/0 type tmpfs (rw,nosuid,nodev,relatime,size=1497312k,mode=700)
cm_processes on /run/cloudera-scm-agent/process type tmpfs (rw,relatime,mode=751)
tmpfs on /run/user/1000 type tmpfs (rw,nosuid,nodev,relatime,size=1497312k,mode=700,uid=1000,gid=1000)

[root@ip-172-31-4-130 ec2-user]# fdisk -l |grep dev
WARNING: fdisk GPT support is currently new, and therefore in an experimental phase. Use at your own discretion.
Disk /dev/xvda: 32.2 GB, 32212254720 bytes, 62914560 sectors
Disk /dev/xvdb: 32.2 GB, 32212254720 bytes, 62914560 sectors

# Free Space

[root@ip-172-31-7-126 ~]# df
Filesystem     1K-blocks     Used Available Use% Mounted on
/dev/xvda2      31444972 10556300  20888672  34% /
devtmpfs         7599360        0   7599360   0% /dev
tmpfs            7486540        0   7486540   0% /dev/shm
tmpfs            7486540    16800   7469740   1% /run
tmpfs            7486540        0   7486540   0% /sys/fs/cgroup
tmpfs            1497312        0   1497312   0% /run/user/0
cm_processes     7486540      212   7486328   1% /run/cloudera-scm-agent/process
tmpfs            1497312        0   1497312   0% /run/user/995

#hugepages

[root@ip-172-31-7-126 ~]# cat /proc/sys/vm/nr_hugepages
0


# IP Config

[root@ip-172-31-7-126 ~]# ip addr show
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 9001 qdisc pfifo_fast state UP qlen 1000
    link/ether 0a:19:d6:01:4a:59 brd ff:ff:ff:ff:ff:ff
    inet 172.31.7.126/20 brd 172.31.15.255 scope global dynamic eth0
       valid_lft 3434sec preferred_lft 3434sec
    inet6 fe80::819:d6ff:fe01:4a59/64 scope link
       valid_lft forever preferred_lft forever

#NSCD

[root@ip-172-31-7-126 ~]# service nscd status
Redirecting to /bin/systemctl status  nscd.service
● nscd.service - Name Service Cache Daemon
   Loaded: loaded (/usr/lib/systemd/system/nscd.service; disabled; vendor preset: disabled)
   Active: active (running) since Tue 2017-03-07 16:52:05 EST; 8s ago
  Process: 23201 ExecStart=/usr/sbin/nscd $NSCD_OPTIONS (code=exited, status=0/SUCCESS)
 Main PID: 23202 (nscd)
   CGroup: /system.slice/nscd.service
           └─23202 /usr/sbin/nscd

Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal nscd[23202]: 23202 monitor...
Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal nscd[23202]: 23202 monitor...
Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal nscd[23202]: 23202 monitor...
Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal nscd[23202]: 23202 monitor...
Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal nscd[23202]: 23202 monitor...
Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal nscd[23202]: 23202 monitor...
Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal nscd[23202]: 23202 monitor...
Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal nscd[23202]: 23202 disable...
Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal nscd[23202]: 23202 stat fa...
Mar 07 16:52:05 ip-172-31-7-126.us-west-2.compute.internal systemd[1]: Started Name S...
Hint: Some lines were ellipsized, use -l to show in full.

#NTPD

[root@ip-172-31-7-126 ~]# service ntpd status
Redirecting to /bin/systemctl status  ntpd.service
● ntpd.service - Network Time Service
   Loaded: loaded (/usr/lib/systemd/system/ntpd.service; disabled; vendor preset: disabled)
   Active: active (running) since Tue 2017-03-07 16:54:23 EST; 8s ago
  Process: 23525 ExecStart=/usr/sbin/ntpd -u ntp:ntp $OPTIONS (code=exited, status=0/SUCCESS)
 Main PID: 23526 (ntpd)
   CGroup: /system.slice/ntpd.service
           └─23526 /usr/sbin/ntpd -u ntp:ntp -g

Mar 07 16:54:23 ip-172-31-7-126.us-west-2.compute.internal ntpd[23526]: Listen normal...
Mar 07 16:54:23 ip-172-31-7-126.us-west-2.compute.internal ntpd[23526]: Listen normal...
Mar 07 16:54:23 ip-172-31-7-126.us-west-2.compute.internal ntpd[23526]: Listen normal...
Mar 07 16:54:23 ip-172-31-7-126.us-west-2.compute.internal ntpd[23526]: Listen normal...
Mar 07 16:54:23 ip-172-31-7-126.us-west-2.compute.internal ntpd[23526]: Listening on ...
Mar 07 16:54:23 ip-172-31-7-126.us-west-2.compute.internal systemd[1]: Started Networ...
Mar 07 16:54:23 ip-172-31-7-126.us-west-2.compute.internal ntpd[23526]: 0.0.0.0 c016 ...
Mar 07 16:54:23 ip-172-31-7-126.us-west-2.compute.internal ntpd[23526]: 0.0.0.0 c012 ...
Mar 07 16:54:23 ip-172-31-7-126.us-west-2.compute.internal ntpd[23526]: 0.0.0.0 c011 ...
Mar 07 16:54:30 ip-172-31-7-126.us-west-2.compute.internal ntpd[23526]: 0.0.0.0 c614 ...
Hint: Some lines were ellipsized, use -l to show in full.





