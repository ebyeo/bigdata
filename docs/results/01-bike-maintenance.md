# Bike Maintenance

This application compiles the top 30 most used bikes for the duration of the analysis.

```
> run
[info] Compiling 6 Scala sources to /home/bigdata/projects/bigdata/bikeshare/target/scala-2.11/classes...
[warn] Multiple main classes detected.  Run 'show discoveredMainClasses' to see the list

Multiple main classes detected, select one to run:

 [1] team3.bikeshare.project.BigBikeGraphBikeMaintainance
 [2] team3.bikeshare.project.BigBikeGraphDegreesRatio
 [3] team3.bikeshare.project.BigBikeGraphOutBoundInBound
 [4] team3.bikeshare.project.BikeShareAppFordGoDataset
 [5] team3.bikeshare.project.BikeShareAppPageRank

Enter number: 1

[info] Running team3.bikeshare.project.BigBikeGraphBikeMaintainance
Using Spark's default log4j profile: org/apache/spark/log4j-defaults.properties
Total number of unique bikes in 2018 Jan : 719
Top 30 bikes out of 719 that require maintainance in 2018 January :
+-------+---------------+
|bike_id|Number of Trips|
+-------+---------------+
|   1403|              5|
|   2421|              5|
|   2528|              4|
|   2792|              4|
|   2388|              4|
|   1096|              4|
|   3105|              4|
|   1352|              4|
|    568|              4|
|   2690|              4|
|   3008|              4|
|   1617|              4|
|   2808|              4|
|   2411|              4|
|   3354|              3|
|   1946|              3|
|   2761|              3|
|    214|              3|
|    297|              3|
|    627|              3|
|   2139|              3|
|   2900|              3|
|   1208|              3|
|   3185|              3|
|    970|              3|
|   3001|              3|
|    120|              3|
|   2888|              3|
|    512|              3|
|   3090|              3|
+-------+---------------+
only showing top 30 rows

[success] Total time: 206 s, completed Apr 27, 2018 11:16:07 PM
```