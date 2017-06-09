#HDFS Directories
[ec2-user@ip-172-31-16-183 ~]$ hdfs dfs -ls /user
Found 8 items
drwxr-xr-x   - admin  admin               0 2017-06-09 06:11 /user/admin
drwxr-xr-x   - hdfs   supergroup          0 2017-06-09 06:11 /user/hdfs
drwxrwxrwx   - mapred hadoop              0 2017-06-09 05:50 /user/history
drwxrwxr-t   - hive   hive                0 2017-06-09 05:54 /user/hive
drwxrwxr-x   - hue    hue                 0 2017-06-09 05:54 /user/hue
drwxr-xr-x   - hdfs   supergroup          0 2017-06-09 06:12 /user/jeremy
drwxrwxr-x   - oozie  oozie               0 2017-06-09 06:01 /user/oozie
drwxr-xr-x   - hdfs   supergroup          0 2017-06-09 06:12 /user/theresa


#Hosts
[ec2-user@ip-172-31-16-183 ~]$ curl -u 'admin:Chandra@123' http://ec2-52-19-86-176.eu-west-1.compute.amazonaws.com:7180/api/v1/hosts
{
  "items" : [ {
    "hostId" : "e7ed8783-16c3-4953-92f8-8df80398d5bc",
    "ipAddress" : "172.31.16.183",
    "hostname" : "ip-172-31-16-183.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-26-173.eu-west-1.compute.internal:7180/cmf/hostRedirect/e7ed8783-16c3-4953-92f8-8df80398d5bc"
  }, {
    "hostId" : "ecb85c23-247d-418e-b301-24a4665896bb",
    "ipAddress" : "172.31.19.187",
    "hostname" : "ip-172-31-19-187.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-26-173.eu-west-1.compute.internal:7180/cmf/hostRedirect/ecb85c23-247d-418e-b301-24a4665896bb"
  }, {
    "hostId" : "18366472-0e65-4348-9f74-e988459ad2b3",
    "ipAddress" : "172.31.25.135",
    "hostname" : "ip-172-31-25-135.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-26-173.eu-west-1.compute.internal:7180/cmf/hostRedirect/18366472-0e65-4348-9f74-e988459ad2b3"
  }, {
    "hostId" : "8157cc2c-7ded-4c1e-bb58-6611065cf41c",
    "ipAddress" : "172.31.26.101",
    "hostname" : "ip-172-31-26-101.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-26-173.eu-west-1.compute.internal:7180/cmf/hostRedirect/8157cc2c-7ded-4c1e-bb58-6611065cf41c"
  }, {
    "hostId" : "cc580721-7e63-4382-8660-01699ac127de",
    "ipAddress" : "172.31.26.173",
    "hostname" : "ip-172-31-26-173.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-26-173.eu-west-1.compute.internal:7180/cmf/hostRedirect/cc580721-7e63-4382-8660-01699ac127de"
  } ]
