[ec2-user@ip-172-31-11-218 ~]$sudo sysctl -w vm.swappiness=1
[ec2-user@ip-172-31-11-218 ~]$ sudo cat /proc/sys/vm/swappiness
1

[ec2-user@ip-172-31-2-61 ~]$ sudo sysctl -w vm.swappiness=1
vm.swappiness = 1
[ec2-user@ip-172-31-2-61 ~]$ sudo cat /proc/sys/vm/swappiness
1

[ec2-user@ip-172-31-13-97 ~]$ sudo sysctl -w vm.swappiness=1
vm.swappiness = 1
[ec2-user@ip-172-31-13-97 ~]$ sudo cat /proc/sys/vm/swappiness
1

[ec2-user@ip-172-31-11-252 ~]$ sudo cat /proc/sys/vm/swappiness
1

[ec2-user@ip-172-31-11-208 ~]$ sudo sysctl -w vm.swappiness=1
vm.swappiness = 1
[ec2-user@ip-172-31-11-208 ~]$ sudo cat /proc/sys/vm/swappiness
1
###########################################

[ec2-user@ip-172-31-11-218 ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       10G  1.7G  8.4G  17% /
devtmpfs        3.9G     0  3.9G   0% /dev
tmpfs           3.7G     0  3.7G   0% /dev/shm
tmpfs           3.7G   25M  3.7G   1% /run
tmpfs           3.7G     0  3.7G   0% /sys/fs/cgroup
tmpfs           757M     0  757M   0% /run/user/1000

###########################################

[ec2-user@ip-172-31-11-218 ~]$ grep -i HugePages_Total /proc/meminfo
HugePages_Total:       0

[ec2-user@ip-172-31-2-61 ~]$ grep -i HugePages_Total /proc/meminfo
HugePages_Total:       0

[ec2-user@ip-172-31-11-252 ~]$ grep -i HugePages_Total /proc/meminfo
HugePages_Total:       0

[ec2-user@ip-172-31-13-97 ~]$ grep -i HugePages_Total /proc/meminfo
HugePages_Total:       0

[ec2-user@ip-172-31-11-208 ~]$ grep -i HugePages_Total /proc/meminfo
HugePages_Total:       0

#############################################

[ec2-user@ip-172-31-11-218 ~]$ ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 9001
        inet 172.31.11.218  netmask 255.255.240.0  broadcast 172.31.15.255
        inet6 fe80::4d1:c2ff:fe18:c95  prefixlen 64  scopeid 0x20<link>
        ether 06:d1:c2:18:0c:95  txqueuelen 1000  (Ethernet)
        RX packets 136490  bytes 196886870 (187.7 MiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 36759  bytes 3771480 (3.5 MiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1  (Local Loopback)
        RX packets 4  bytes 340 (340.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 4  bytes 340 (340.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

[ec2-user@ip-172-31-2-61 ~]$ ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 9001
        inet 172.31.2.61  netmask 255.255.240.0  broadcast 172.31.15.255
        inet6 fe80::400:4aff:fe42:2ef7  prefixlen 64  scopeid 0x20<link>
        ether 06:00:4a:42:2e:f7  txqueuelen 1000  (Ethernet)
        RX packets 1901  bytes 220029 (214.8 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 1924  bytes 274122 (267.6 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1  (Local Loopback)
        RX packets 4  bytes 340 (340.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 4  bytes 340 (340.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

[ec2-user@ip-172-31-11-252 ~]$ ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 9001
        inet 172.31.11.252  netmask 255.255.240.0  broadcast 172.31.15.255
        inet6 fe80::489:58ff:fecf:48bf  prefixlen 64  scopeid 0x20<link>
        ether 06:89:58:cf:48:bf  txqueuelen 1000  (Ethernet)
        RX packets 1142  bytes 121611 (118.7 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 1210  bytes 134355 (131.2 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1  (Local Loopback)
        RX packets 4  bytes 340 (340.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 4  bytes 340 (340.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

[ec2-user@ip-172-31-13-97 ~]$ ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 9001
        inet 172.31.13.97  netmask 255.255.240.0  broadcast 172.31.15.255
        inet6 fe80::433:7aff:fef8:449  prefixlen 64  scopeid 0x20<link>
        ether 06:33:7a:f8:04:49  txqueuelen 1000  (Ethernet)
        RX packets 1350  bytes 154375 (150.7 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 1366  bytes 205078 (200.2 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1  (Local Loopback)
        RX packets 4  bytes 340 (340.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 4  bytes 340 (340.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

[ec2-user@ip-172-31-11-208 ~]$ ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 9001
        inet 172.31.11.208  netmask 255.255.240.0  broadcast 172.31.15.255
        inet6 fe80::45d:32ff:fef2:1865  prefixlen 64  scopeid 0x20<link>
        ether 06:5d:32:f2:18:65  txqueuelen 1000  (Ethernet)
        RX packets 1334  bytes 154331 (150.7 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 1396  bytes 218122 (213.0 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1  (Local Loopback)
        RX packets 4  bytes 340 (340.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 4  bytes 340 (340.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

###############################################################

[ec2-user@ip-172-31-11-218 ~]$ nslookup google.com
Server:         172.31.0.2
Address:        172.31.0.2#53

Non-authoritative answer:
Name:   google.com
Address: 209.85.203.100
Name:   google.com
Address: 209.85.203.101
Name:   google.com
Address: 209.85.203.102
Name:   google.com
Address: 209.85.203.113
Name:   google.com
Address: 209.85.203.138
Name:   google.com
Address: 209.85.203.139

[ec2-user@ip-172-31-2-61 ~]$ nslookup google.com
Server:         172.31.0.2
Address:        172.31.0.2#53

Non-authoritative answer:
Name:   google.com
Address: 209.85.203.100
Name:   google.com
Address: 209.85.203.101
Name:   google.com
Address: 209.85.203.102
Name:   google.com
Address: 209.85.203.113
Name:   google.com
Address: 209.85.203.138
Name:   google.com
Address: 209.85.203.139

[ec2-user@ip-172-31-11-252 ~]$ nslookup google.com
Server:         172.31.0.2
Address:        172.31.0.2#53

Non-authoritative answer:
Name:   google.com
Address: 209.85.202.113
Name:   google.com
Address: 209.85.202.138
Name:   google.com
Address: 209.85.202.139
Name:   google.com
Address: 209.85.202.100
Name:   google.com
Address: 209.85.202.101
Name:   google.com
Address: 209.85.202.102

[ec2-user@ip-172-31-13-97 ~]$ nslookup google.com
Server:         172.31.0.2
Address:        172.31.0.2#53

Non-authoritative answer:
Name:   google.com
Address: 209.85.203.138
Name:   google.com
Address: 209.85.203.139
Name:   google.com
Address: 209.85.203.100
Name:   google.com
Address: 209.85.203.101
Name:   google.com
Address: 209.85.203.102
Name:   google.com
Address: 209.85.203.113

[ec2-user@ip-172-31-11-208 ~]$ nslookup google.com
Server:         172.31.0.2
Address:        172.31.0.2#53

Non-authoritative answer:
Name:   google.com
Address: 209.85.203.139
Name:   google.com
Address: 209.85.203.100
Name:   google.com
Address: 209.85.203.101
Name:   google.com
Address: 209.85.203.102
Name:   google.com
Address: 209.85.203.113
Name:   google.com
Address: 209.85.203.138

#####################################################

[ec2-user@ip-172-31-11-218 ~]$ sudo nscd -g

[ec2-user@ip-172-31-11-218 ~]$ sudo nscd -g
nscd configuration:

              0  server debug level
             2s  server runtime
              5  current number of threads
             32  maximum number of threads
              0  number of times clients had to wait
             no  paranoia mode enabled
           3600  restart internal
              5  reload count

passwd cache:

            yes  cache is enabled
            yes  cache is persistent
            yes  cache is shared
            211  suggested size
         216064  total data pool size
            344  used data pool size
            600  seconds time to live for positive entries
             20  seconds time to live for negative entries
              0  cache hits on positive entries
              0  cache hits on negative entries
              2  cache misses on positive entries
              0  cache misses on negative entries
              0% cache hit rate
              4  current number of cached values
              4  maximum number of cached values
              0  maximum chain length searched
              0  number of delays on rdlock
              0  number of delays on wrlock
              0  memory allocations failed
            yes  check /etc/passwd for changes

group cache:

            yes  cache is enabled
            yes  cache is persistent
            yes  cache is shared
            211  suggested size
         216064  total data pool size
             80  used data pool size
           3600  seconds time to live for positive entries
             60  seconds time to live for negative entries
              0  cache hits on positive entries
              0  cache hits on negative entries
              0  cache misses on positive entries
              1  cache misses on negative entries
              0% cache hit rate
              1  current number of cached values
              1  maximum number of cached values
              0  maximum chain length searched
              0  number of delays on rdlock
              0  number of delays on wrlock
              0  memory allocations failed
            yes  check /etc/group for changes

hosts cache:

            yes  cache is enabled
            yes  cache is persistent
            yes  cache is shared
            211  suggested size
         216064  total data pool size
              0  used data pool size
           3600  seconds time to live for positive entries
             20  seconds time to live for negative entries
              0  cache hits on positive entries
              0  cache hits on negative entries
              0  cache misses on positive entries
              0  cache misses on negative entries
              0% cache hit rate
              0  current number of cached values
              0  maximum number of cached values
              0  maximum chain length searched
              0  number of delays on rdlock
              0  number of delays on wrlock
              0  memory allocations failed
            yes  check /etc/hosts for changes

services cache:

            yes  cache is enabled
            yes  cache is persistent
            yes  cache is shared
            211  suggested size
         216064  total data pool size
              0  used data pool size
          28800  seconds time to live for positive entries
             20  seconds time to live for negative entries
              0  cache hits on positive entries
              0  cache hits on negative entries
              0  cache misses on positive entries
              0  cache misses on negative entries
              0% cache hit rate
              0  current number of cached values
              0  maximum number of cached values
              0  maximum chain length searched
              0  number of delays on rdlock
              0  number of delays on wrlock
              0  memory allocations failed
            yes  check /etc/services for changes

netgroup cache:

            yes  cache is enabled
            yes  cache is persistent
            yes  cache is shared
            211  suggested size
         216064  total data pool size
              0  used data pool size
          28800  seconds time to live for positive entries
             20  seconds time to live for negative entries
              0  cache hits on positive entries
              0  cache hits on negative entries
              0  cache misses on positive entries
              0  cache misses on negative entries
              0% cache hit rate
              0  current number of cached values
              0  maximum number of cached values
              0  maximum chain length searched
              0  number of delays on rdlock
              0  number of delays on wrlock
              0  memory allocations failed
            yes  check /etc/netgroup for changes

SELinux AVC Statistics:

              6  entry lookups
              5  entry hits
              1  entry misses
              0  entry discards
              1  CAV lookups
              0  CAV hits
              0  CAV probes
              1  CAV misses

###################################################

[ec2-user@ip-172-31-11-218 ~]$ sudo service ntpd status
Redirecting to /bin/systemctl status  ntpd.service
? ntpd.service - Network Time Service
   Loaded: loaded (/usr/lib/systemd/system/ntpd.service; enabled; vendor preset: disabled)
   Active: active (running) since Mon 2017-06-05 09:47:34 EDT; 5s ago
  Process: 26732 ExecStart=/usr/sbin/ntpd -u ntp:ntp $OPTIONS (code=exited, status=0/SUCCESS)
 Main PID: 26733 (ntpd)
   CGroup: /system.slice/ntpd.service
           +-26733 /usr/sbin/ntpd -u ntp:ntp -g

Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal ntpd[26733]: Listen and drop on 1 v6wildcard :: UDP 123
Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal ntpd[26733]: Listen normally on 2 lo 127.0.0.1 UDP 123
Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal ntpd[26733]: Listen normally on 3 eth0 172.31.11.218 UDP 123
Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal ntpd[26733]: Listen normally on 4 lo ::1 UDP 123
Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal ntpd[26733]: Listen normally on 5 eth0 fe80::4d1:c2ff:fe18:c95 UDP 123
Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal ntpd[26733]: Listening on routing socket on fd #22 for interface updates
Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal systemd[1]: Started Network Time Service.
Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal ntpd[26733]: 0.0.0.0 c016 06 restart
Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal ntpd[26733]: 0.0.0.0 c012 02 freq_set kernel 0.000 PPM
Jun 05 09:47:34 ip-172-31-11-218.eu-west-2.compute.internal ntpd[26733]: 0.0.0.0 c011 01 freq_not_set