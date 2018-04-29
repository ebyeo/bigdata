# Installation on OS X

* Install or update to Java SE Development Kit 8 >> https://docs.oracle.com/javase/8/docs/technotes/guides/install/install_overview.html
* Install Scala >> https://www.scala-lang.org/download/
* Install SBT >> https://www.scala-sbt.org/1.0/docs/Setup.html
* Install Apache Spark >> https://spark.apache.org/downloads.html
* [Install Hadoop and Flume](#install-hadoop-and-flume)

## Install Hadoop and Flume
For the purpose of consuming large amount of data we decided to use Flume to write to HDFS

OS X setup instructions:
* Install Hadoop >> <https://macmetric.com/how-to-install-hadoop-on-mac/>
* Install Flume >> <https://brewinstall.org/install-flume-on-mac-with-brew/>

To start HDFS on OS X:
* Enable Remote Login by navigating the following path :“System Preferences” -> “Sharing”. Check “Remote Login”
* run "/usr/local/Cellar/hadoop/3.0.0/sbin/start-dfs.sh"

Sample Flume config for Bikeshare is found in https://github.com/ebyeo/bigdata/tree/master/app_template/conf/bikeshare.conf

Place the sample config in /usr/local/Cellar/flume/1.6.0/libexec/conf/

Flume read CSV Instructions >> <https://acadgild.com/blog/loading-files-into-hdfs-using-flumes-spool-directory/>

To run flume:
> /usr/local/Cellar/flume/1.6.0/bin/flume-ng agent --name agent1 -f /usr/local/Cellar/flume/1.6.0/libexec/conf/bikeshare.conf

To list files in HDFS:
> hdfs dfs -ls /flume_sink | sort -k6,7

To view the HDFS:
> hdfs dfs -cat /flume_sink/FlumeData.*

To delete folder in HDFS:
> hadoop fs -rm -r /flume_sink/

## Run GraphX Program
To execute GraphX program:

- Run sbt at command prompt
```
$ cd bikeshare
$ sbt
...
> run
```
