# Big Data Assignment: Ford GoBike System Guide

## Introduction
This guide provides instruction to set up the Ford GoBike analytic application which is a big data platform designed to scale as the bike sharing scheme expands to cover more area across the states.

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
