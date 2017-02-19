# ansible-hive

ansible-galaxy -r ansible/requirements.yml install
ansible-playbook -i ansible/inventory ansible/deployHive.yml


``` bash
sudo su - hadoop
/usr/lib/hadoop/bin/hdfs dfs -mkdir -p /user/hadoop
/usr/lib/hadoop/bin/hdfs dfs -put /etc/hadoop input
/usr/lib/hadoop/bin/hadoop jar /usr/lib/hadoop/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.7.3.jar grep input output 'dfs[a-z.]+'

/usr/lib/hadoop/bin/hdfs dfs -cat output/*

```

# darkedges.hive
