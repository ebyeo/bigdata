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

3. Start Flume
```
cd ~/bikeshare/bin
./start-flume-bike.sh
```

4. Copy data from sample folder to Flume's source folder to simulate data arriving from GoBike
```
cp ~/bikeshare/data/sample/201801_fordgobike_tripdata_001.csv ~/bikeshare/data/bike
```
After the file is processed by Flume, it is renamed to 201801_fordgobike_tripdata_001.csv.COMPLETED

5. Start application
```
cd ~/projects/bigdata/bikeshare
sbt
>run
```
You should see this menu.
```
[warn] Multiple main classes detected.  Run 'show discoveredMainClasses' to see the list

Multiple main classes detected, select one to run:

 [1] team3.bikeshare.project.BigBikeGraphBikeMaintainance
 [2] team3.bikeshare.project.BigBikeGraphDegreesRatio
 [3] team3.bikeshare.project.BigBikeGraphOutBoundInBound
 [4] team3.bikeshare.project.BikeShareAppFordGoDataset
 [5] team3.bikeshare.project.BikeShareAppHDFS
 [6] team3.bikeshare.project.BikeShareAppPageRank

Enter number: 
```
Type the number of the program to run.

6. Type _Exit_ to return

7. Stop Flume
```
ps -ef |grep flume
```
Note the process ID and issue kill -9 <process id> to fill the Flume process

8. Stop Hadoop
```
stop-yarn.sh
stop-dfs.sh
```