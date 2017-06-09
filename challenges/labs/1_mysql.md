#MySQL Hostname:
ip-172-31-16-183.eu-west-1.compute.internal

#MySQL version
[ec2-user@ip-172-31-16-183 ~]$ mysql --version
mysql  Ver 14.14 Distrib 5.7.18, for Linux (x86_64) using  EditLine wrapper

#MySQL databases
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
| sys                |
+--------------------+
10 rows in set (0.01 sec)
