# Run the analysis
1. Start Hadoop
```
start-dfs.sh
start-yarn.sh
```
2. Check that the processes are started successfully:
```
bigdata@ubuntu:~$ jps
6707 Jps
6150 SecondaryNameNode
6295 ResourceManager
5817 NameNode
6428 NodeManager
5966 DataNode
```
10. Stop Hadoop
```
stop-yarn.sh
stop-dfs.sh
```