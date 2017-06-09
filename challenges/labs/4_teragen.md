#Teragen command
sudo -u theresa time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen 
      -D dfs.block.size=33554432 51200000 /user/theresa/tgen512m

#Time command
	  
5.54user 0.28system 1:08.37elapsed 8%CPU (0avgtext+0avgdata 187424maxresident)k
0inputs+1072outputs (0major+40171minor)pagefaults 0swaps

#HDFS command

[ec2-user@ip-172-31-16-183 ~]$ hdfs dfs -ls /user/theresa/tgen512m
Found 3 items
-rw-r--r--   3 theresa supergroup          0 2017-06-09 06:28 /user/theresa/tgen512m/_SUCCESS
-rw-r--r--   3 theresa supergroup 2560000000 2017-06-09 06:28 /user/theresa/tgen512m/part-m-00000
-rw-r--r--   3 theresa supergroup 2560000000 2017-06-09 06:28 /user/theresa/tgen512m/part-m-00001


	  
	  
