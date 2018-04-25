# Hadoop, Yarn, HDFS
The following instruction is based on these links:
- https://www.digitalocean.com/community/tutorials/how-to-install-hadoop-in-stand-alone-mode-on-ubuntu-16-04
- http://techsphot.com/set-up-hadoop-in-pseudo-distributed-mode-on-ubuntu/
- https://www.tutorialspoint.com/hadoop/hadoop_enviornment_setup.htm

Hadoop is installed in pseudo distributed mode. The version to install is 2.7.5.

1. Download the Hadoop distribution in the server as follows:
```
cd ~
mkdir downloads
cd downloads
wget http://archive.apache.org/dist/hadoop/common/hadoop-2.7.5/hadoop-2.7.5.tar.gz
```
2. Untar the file and move the extracted files to /opt/hadoop
```
tar -xzvf hadoop-2.7.5.tar.gz
sudo mv hadoop-2.7.5 /opt/hadoop
```
3. Set Hadoop environment variables by appending the following commands to ~/.bashrc file.
```
export HADOOP_HOME=/opt/hadoop 
export HADOOP_MAPRED_HOME=$HADOOP_HOME 
export HADOOP_COMMON_HOME=$HADOOP_HOME 
export HADOOP_HDFS_HOME=$HADOOP_HOME 
export YARN_HOME=$HADOOP_HOME 
export HADOOP_COMMON_LIB_NATIVE_DIR=$HADOOP_HOME/lib/native 
export PATH=$PATH:$HADOOP_HOME/sbin:$HADOOP_HOME/bin 
export HADOOP_INSTALL=$HADOOP_HOME
```
4. Now apply all the changes into the current running system.
```
source ~/.bashrc
```
5. Configure Hadoop configuration files in the /opt/hadoop/etc/hadoop. 
6. The core-site.xml file contains information such as the port number used for Hadoop instance, memory allocated for the file system, memory limit for storing the data, and size of Read/Write buffers. Open the core-site.xml and add the following properties in between <configuration>, </configuration> tags.
```
   <property>
      <name>fs.default.name</name>
      <value>hdfs://localhost:9000</value> 
   </property>
```
7. The hdfs-site.xml file contains information such as the value of replication data, namenode path, and datanode paths of your local file systems. It means the place where you want to store the Hadoop infrastructure. Open this file and add the following properties in between the <configuration> </configuration> tags in this file.
```
   <property>
      <name>dfs.replication</name>
      <value>1</value>
   </property>

   <property>
      <name>dfs.name.dir</name>
      <value>file:///home/bigdata/hadoopinfra/hdfs/namenode </value>
   </property>
    
   <property>
      <name>dfs.data.dir</name> 
      <value>file:///home/bigdata/hadoopinfra/hdfs/datanode </value> 
   </property>
```
8. The yarn-site.xml file is used to configure yarn into Hadoop. Open the yarn-site.xml file and add the following properties in between the <configuration>, </configuration> tags in this file.
```
   <property>
      <name>yarn.nodemanager.aux-services</name>
      <value>mapreduce_shuffle</value> 
   </property>
```  
9. The mapred-site.xml file is used to specify which MapReduce framework we are using. By default, Hadoop contains a template of yarn-site.xml. First of all, it is required to copy the file from mapred-site.xml.template to mapred-site.xml file using the following command.
```
cp mapred-site.xml.template mapred-site.xml
```
10. Open mapred-site.xml file and add the following properties in between the <configuration>, </configuration>tags in this file.
```
   <property> 
      <name>mapreduce.framework.name</name>
      <value>yarn</value>
   </property>
```   
11. Set up namenode
```
cd ~ 
hdfs namenode -format
```
12. Verify Hadoop dfs and yarn script
```
start-dfs.sh
start-yarn.sh
```
13. Check that the processes are started successfully:
```
bigdata@ubuntu:~$ jps
6707 Jps
6150 SecondaryNameNode
6295 ResourceManager
5817 NameNode
6428 NodeManager
5966 DataNode
```
14. Accessing Hadoop on browser on the host machine
The default port number to access Hadoop is 50070. Use the following url to get Hadoop services on browser.
```
http://192.168.56.102:50070/
```
15. Verify All Applications for Cluster
The default port number to access all applications of cluster is 8088. Use the following url to visit this service.
```
http://192.168.56.102:8088/
```
16. Stop dfs and yarn script
```
stop-yarn.sh
stop-dfs.sh
```