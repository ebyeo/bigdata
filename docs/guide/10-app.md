# Install Application
1. Start hdfs and yarn
```
start-dfs.sh
start-yarn.sh
```

2. Create the hdfs sink directory
```
hadoop fs -mkdir /flume_sink
```

3. Clone the codes from github
```
cd ~
mkdir projects
git clone https://github.com/e0015358/big-graph-data.git
```

4. Create the following application directory
````
cd ~
cp ~/projects/bigdata/app-template .
mv app-template bikeshare
chmod 777 ./bikeshare/bin/start-flume-bike.sh
````

5. Build and run the application for the first time
```
cd ~/projects/big-graph-data/bikeshare
sbt
...
> run
> exit
```

6. Stop dfs and yarn processes
```
stop-yarn.sh
stop-dfs.sh
```