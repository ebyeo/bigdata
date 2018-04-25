# Zeppelin
http://zeppelin.apache.org/docs/0.7.3/install/install.html
Move to /usr/local/zeppelin
If you are configuring auto start, note the path to zeppelin
http://192.168.56.101:8080

# ZooKeeper
https://www.tutorialspoint.com/zookeeper/zookeeper_installation.htm
zookeeper-3.4.11.tar.gz
/opt/zookeeper
make a copy of zoo.cfg from zoo_sample.cfg in /opt/zookeeper/conf
change dataDir=/home/bigdata/data/zookeeper
sudo mkdir /opt/zookeeper/logs
update log4j.properties zookeeper.log.dir, zookeeper.tracelog.dir to /opt/zookeeper/logs

# Apache HBase
Download from https://hbase.apache.org/, stable release hbase-1.2.6-bin.tar.gz
Configure https://www.tutorialspoint.com/hbase/hbase_installation.htm
Note that the path to store the name nodes is /home/bigdata instead of /home/hadoop
Turn off hbase managing zookeeper
export HBASE_MANAGES_ZK=false

# Kafka
https://devops.profitbricks.com/tutorials/install-and-configure-apache-kafka-on-ubuntu-1604-1/
kafka_2.11-1.0.1.tgz
/opt/kafka
sudo mkdir /opt/kafka/logs
export LOG_DIR=/opt/kafka/logs
sudo nohup /opt/kafka/bin/kafka-server-start.sh /opt/kafka/config/server.properties /tmp/kafka.log 2>&1 
https://kafka.apache.org/quickstart