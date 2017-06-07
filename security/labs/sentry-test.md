```
[ec2-user@ip-172-31-18-76 ~]$ beeline
Beeline version 1.1.0-cdh5.8.5 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM
Enter username for jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM: hive
Enter password for jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM: ************
Connected to: Apache Hive (version 1.1.0-cdh5.8.5)
Driver: Hive JDBC (version 1.1.0-cdh5.8.5)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-16-120.eu-west-1.co> show tables;
INFO  : Compiling command(queryId=hive_20170607112323_4fa1b063-5544-475d-b10c-a98df931321a): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170607112323_4fa1b063-5544-475d-b10c-a98df931321a); Time taken: 0.649 seconds
INFO  : Executing command(queryId=hive_20170607112323_4fa1b063-5544-475d-b10c-a98df931321a): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170607112323_4fa1b063-5544-475d-b10c-a98df931321a); Time taken: 0.226 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (1.133 seconds)
0: jdbc:hive2://ip-172-31-16-120.eu-west-1.co>


[ec2-user@ip-172-31-16-120 ~]$ kinit -kt george.keytab george/user@CMREALM
[ec2-user@ip-172-31-16-120 ~]$ beeline
Beeline version 1.1.0-cdh5.8.5 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM
Enter username for jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM: hive
Enter password for jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM: ************
Connected to: Apache Hive (version 1.1.0-cdh5.8.5)
Driver: Hive JDBC (version 1.1.0-cdh5.8.5)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-16-120.eu-west-1.co> show tables;
INFO  : Compiling command(queryId=hive_20170607122121_908e1e7a-5d72-489e-b5be-0e37b1a5f06e): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170607122121_908e1e7a-5d72-489e-b5be-0e37b1a5f06e); Time taken: 0.059 seconds
INFO  : Executing command(queryId=hive_20170607122121_908e1e7a-5d72-489e-b5be-0e37b1a5f06e): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170607122121_908e1e7a-5d72-489e-b5be-0e37b1a5f06e); Time taken: 0.112 seconds
INFO  : OK
+-------------+--+
|  tab_name   |
+-------------+--+
| my_table    |
| my_table_1  |
| my_table_3  |
+-------------+--+
3 rows selected (0.249 seconds)
0: jdbc:hive2://ip-172-31-16-120.eu-west-1.co>


[ec2-user@ip-172-31-16-120 ~]$ beeline
Beeline version 1.1.0-cdh5.8.5 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM
Enter username for jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM: hive
Enter password for jdbc:hive2://ip-172-31-16-120.eu-west-1.compute.internal:10000/default;principal=hive/ip-172-31-16-120.eu-west-1.compute.internal@CMREALM: ************
Connected to: Apache Hive (version 1.1.0-cdh5.8.5)
Driver: Hive JDBC (version 1.1.0-cdh5.8.5)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-16-120.eu-west-1.co> show tables;
INFO  : Compiling command(queryId=hive_20170607122222_310cfd42-53b2-481b-b260-8bd331ab5365): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170607122222_310cfd42-53b2-481b-b260-8bd331ab5365); Time taken: 0.059 seconds
INFO  : Executing command(queryId=hive_20170607122222_310cfd42-53b2-481b-b260-8bd331ab5365): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170607122222_310cfd42-53b2-481b-b260-8bd331ab5365); Time taken: 0.11 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
| my_table  |
+-----------+--+
1 row selected (0.247 seconds)
0: jdbc:hive2://ip-172-31-16-120.eu-west-1.co>

```
