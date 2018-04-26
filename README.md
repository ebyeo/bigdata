# Big Graph Data Analysis in Spark: Ford GoBike

## Introduction
This guide provides instruction to set up the Ford GoBike analytic application which is a big data platform designed to scale as the bike sharing scheme expands to cover more area across the states.

Here we attempt to use GraphX to model the BikeShare data from [Ford GoBike](www.fordgobike.com/system-data)

In a nutshell, the input and output of the system are:
* source data is provided by Ford GoBike at their [website](https://www.fordgobike.com/) via this [link](https://www.fordgobike.com/system-data)
* visualisation is hosted on carto.com at this [link](https://e0015358.carto.com/builder/cb097103-cd70-4d53-a749-627bad91fa95/embed).

## System Overview
For the demo, the system is put together in a VirtualBox VM with Ubuntu OS. The system covers 
* ingestion of the data using Apache Flume
* storage in HDFS
* processing using Spark RDD and GraphX
* analysis and visualisation using [Carto](https://carto.com/)

The source codes are available at github.

## Components
The system comprises the following components:

Component | Version | Website | Purpose
--------- | ------- | ------- | -------
Oracle VirtualBox | 5.2.8 | https://www.virtualbox.org | Host the VMs for the demo
Ubuntu Server | 16.04.4 LTS | https://www.ubuntu.com | Where the big data components are installed
Java 8 JDK | 1.8.0_151 | https://java.com/en |
Apache Zookeeper | 3.4.11 | http://zookeeper.apache.org | Coordinate distributed systems, required for Hadoop and Flume
Apache Hadoop | 2.7.5 | http://hadoop.apache.org | Comprise HDFS and Yarn
Apache Flume | 1.8.0 | http://flume.apache.org | To ingest the trip logs and deposit into HDFS
Apache Spark | 2.3.0 | http://spark.apache.org | To process the file and use GraphX for the graph analysis
SBT	| 1.1.1 | https://www.scala-sbt.org | Build tool for Scala

Other components installed but not use in the demo:

Component | Version | Website | Purpose
--------- | ------- | ------- | -------
HBase | 1.2.6 | https://hbase.apache.org | A distributed and scalable data store
Kafka | 1.0.1 | http://kafka.apache.org | For publishing and subscribing to messages 
Zeppelin | 0.7.3 | https://zeppelin.apache.org | A web-based notebook for interactive data analytics with Scala and more

## Installation
Please install the components in the order presented in this guide:

* [Install VirtualBox](./docs/guide/01-virtualbox.md)
* [Install Ubuntu](./docs/guide/02-ubuntu.md)
* [Configure Virtual Machine](./docs/guide/03-configure-virtualbox.md)
* [Install Java JDK](./docs/guide/04-java.md)
* [Install Hadoop, Yarn, HDFS](./docs/guide/05-hadoop.md)
* [Install sbt](./docs/guide/06-sbt.md)
* [Install Scala](./docs/guide/07-scala.md)
* [Install Apache Spark](./docs/guide/08-spark.md)
* [Install Apache Flume](./docs/guide/09-flume.md)
* [Install Application](./docs/guide/10-app.md)

Refer to [these instructions](./docs/guide/11-mac.md) for installation on a OS X.

## Results

PageRank measures the importance of each vertex in a graph, by determining which vertexes have the most edges with other vertexes. In our example, we can use PageRank to determine which bike stations are the most important by measuring which stations have the most connections to other stations.

PageRank for 201801_fordgobike_tripdata
```
Processing 94802 datapoints
Telegraph Ave at 19th St has a pagerank of 216
Frank H Ogawa Plaza has a pagerank of 215
San Jose Diridon Station has a pagerank of 190
19th Street BART Station has a pagerank of 183
Grand Ave at Webster St has a pagerank of 183
San Fernando St at 4th St has a pagerank of 179
Telegraph Ave at 23rd St has a pagerank of 178
Bay Pl at Vernon St has a pagerank of 175
West Oakland BART Station has a pagerank of 170
MacArthur BART Station has a pagerank of 160
[success] Total time: 5176 s, completed 14 Apr 2018, 1:03:12 AM
```
## References
### GraphX Resources
* <http://www.sparktutorials.net/Analyzing+Flight+Data%3A+A+Gentle+Introduction+to+GraphX+in+Spark>
* <https://github.com/caroljmcdonald/sparkgraphxexample>
* <https://docs.databricks.com/spark/latest/graph-analysis/graph-analysis-graphx-tutorial.html>

