# Yum repo list
[ec2-user@ip-172-31-26-173 ~]$ ls /etc/yum.repos.d
cloudera-manager.repo  
redhat.repo                     
redhat-rhui.repo
mysql-community.repo   
redhat-rhui-client-config.repo  
rhui-load-balancers.conf

# Writing db.properties
sudo /usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-16-183.eu-west-1.compute.internal scm scm 
