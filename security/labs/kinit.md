[ec2-user@ip-172-31-16-120 ~]$ sudo kinit -kt /opt/hive.keytab hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM

[ec2-user@ip-172-31-16-120 ~]$ sudo klist
Ticket cache: FILE:/tmp/krb5cc_0
Default principal: hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM

Valid starting       Expires              Service principal
06/08/2017 09:44:29  06/09/2017 09:44:29  krbtgt/CMREALM@CMREALM
        renew until 06/13/2017 09:44:29

