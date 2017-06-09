```
#Cloud Provider :  
AWS

#Linux Release:
[ec2-user@ip-172-31-16-183 ~]$ cat /etc/system-release
Red Hat Enterprise Linux Server release 7.3 (Maipo)

#Disk Space:
[ec2-user@ip-172-31-16-183 ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2      100G  1.9G   99G   2% /
devtmpfs        7.8G     0  7.8G   0% /dev
tmpfs           7.7G     0  7.7G   0% /dev/shm
tmpfs           7.7G   25M  7.7G   1% /run
tmpfs           7.7G     0  7.7G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000

# Yum repo list
[ec2-user@ip-172-31-16-183 ~]$ sudo yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
repo id                                                             repo name                                                                          status
!rhui-REGION-client-config-server-7/x86_64                          Red Hat Update Infrastructure 2.0 Client Configuration Server 7                         6
!rhui-REGION-rhel-server-releases/7Server/x86_64                    Red Hat Enterprise Linux Server 7 (RPMs)                                           14,447
!rhui-REGION-rhel-server-rh-common/7Server/x86_64                   Red Hat Enterprise Linux Server 7 RH Common (RPMs)                                    228
repolist: 14,681

# User addition
theresa:x:2000:1003::/home/theresa:/bin/bash
jeremy:x:3000:1004::/home/jeremy:/bin/bash

#Group addition
conservative:x:1003:
labour:x:1004:


