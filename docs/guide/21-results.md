# Results

## Bike Maintenance
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

## Degree Ratio
```
> run
[warn] Multiple main classes detected.  Run 'show discoveredMainClasses' to see the list

Multiple main classes detected, select one to run:

 [1] team3.bikeshare.project.BigBikeGraphBikeMaintainance
 [2] team3.bikeshare.project.BigBikeGraphDegreesRatio
 [3] team3.bikeshare.project.BigBikeGraphOutBoundInBound
 [4] team3.bikeshare.project.BikeShareAppFordGoDataset
 [5] team3.bikeshare.project.BikeShareAppPageRank

Enter number: 2

[info] Running team3.bikeshare.project.BigBikeGraphDegreesRatio
Using Spark's default log4j profile: org/apache/spark/log4j-defaults.properties
Processing 999 datapoints
>> Total number of stations : 240
Total Number of Stations: 240
Total Number of Trips: 828
Total Number of Trips in Original Data: 828
19th St at Mission St,37.760299,-122.418892 has a in/out degree ratio of 10.0
Mississippi St at 17th St,37.7648022,-122.3947713 has a in/out degree ratio of 6.0
Webster St at Grove St,37.7770527,-122.4295585 has a in/out degree ratio of 5.0
Duboce Park,37.7692005,-122.4338119 has a in/out degree ratio of 5.0
Grand Ave at Perkins St,37.80889393398715,-122.25646018981932 has a in/out degree ratio of 5.0
El Embarcadero at Grand Ave,37.8088479,-122.2496799 has a in/out degree ratio of 5.0
Golden Gate Ave at Hyde St,37.7816495,-122.4154077 has a in/out degree ratio of 4.0
San Francisco City Hall (Polk St at Grove St),37.77865,-122.41823 has a in/out degree ratio of 4.0
Dolores St at 15th St,37.7662102,-122.4266136 has a in/out degree ratio of 4.0
Lakeside Dr at 14th St,37.8013189,-122.2626418 has a in/out degree ratio of 4.0
Lake Merritt BART Station,37.7973195,-122.2653199 has a out/in degree ratio of 8.0
Bancroft Way at College Ave,37.8693603,-122.2543374 has a out/in degree ratio of 8.0
Howard St at 2nd St,37.787521780456245,-122.39740490913391 has a out/in degree ratio of 6.5
17th & Folsom Street Park (17th St at Folsom St),37.7637085,-122.4152042 has a out/in degree ratio of 5.0
19th Street BART Station,37.8090126,-122.2682473 has a out/in degree ratio of 5.0
Downtown Berkeley BART,37.8703477,-122.2677637 has a out/in degree ratio of 5.0
MacArthur BART Station,37.82840997305853,-122.26631462574005 has a out/in degree ratio of 4.333333333333333
Franklin Square,37.764555,-122.410345 has a out/in degree ratio of 4.0
Mechanics Monument Plaza (Market St at Bush St),37.7913,-122.399051 has a out/in degree ratio of 3.5
Rockridge BART Station,37.84427875399067,-122.251900434494 has a out/in degree ratio of 3.5
[success] Total time: 115 s, completed Apr 27, 2018 11:18:06 PM
>
```

## Out Bound / In Bound
```
> run
[warn] Multiple main classes detected.  Run 'show discoveredMainClasses' to see the list

Multiple main classes detected, select one to run:

 [1] team3.bikeshare.project.BigBikeGraphBikeMaintainance
 [2] team3.bikeshare.project.BigBikeGraphDegreesRatio
 [3] team3.bikeshare.project.BigBikeGraphOutBoundInBound
 [4] team3.bikeshare.project.BikeShareAppFordGoDataset
 [5] team3.bikeshare.project.BikeShareAppPageRank

Enter number: 3

[info] Running team3.bikeshare.project.BigBikeGraphOutBoundInBound
Using Spark's default log4j profile: org/apache/spark/log4j-defaults.properties
Processing 999 datapoints
Total Number of Stations: 240
Total Number of Trips: 828
Total Number of Trips in Original Data: 828
Bike stations with the most inbound traffic:
San Francisco Caltrain (Townsend St at 4th St),37.776598,-122.395282 has 17 in degrees.
Market St at 10th St,37.776619,-122.417385 has 17 in degrees.
Valencia St at 24th St,37.7524278,-122.4206278 has 14 in degrees.
San Francisco Caltrain Station 2  (Townsend St at 4th St),37.7766392,-122.3955263 has 12 in degrees.
Berry St at 4th St,37.77588,-122.39317 has 12 in degrees.
4th St at Mission Bay Blvd S,37.7704074,-122.3911984 has 12 in degrees.
San Francisco Ferry Building (Harry Bridges Plaza),37.795392,-122.394203 has 11 in degrees.
Valencia St at 16th St,37.765052,-122.4218661 has 11 in degrees.
Powell St BART Station (Market St at 4th St),37.78637526861584,-122.40490436553954 has 10 in degrees.
Howard St at Beale St,37.789756,-122.394643 has 10 in degrees.
Bike stations with the most outbound traffic:
Market St at 10th St,37.776619,-122.417385 has 22 out degrees.
Berry St at 4th St,37.77588,-122.39317 has 22 out degrees.
Powell St BART Station (Market St at 4th St),37.78637526861584,-122.40490436553954 has 19 out degrees.
San Francisco Caltrain (Townsend St at 4th St),37.776598,-122.395282 has 19 out degrees.
19th Street BART Station,37.8090126,-122.2682473 has 15 out degrees.
Clay St at Battery St,37.795001,-122.39997 has 14 out degrees.
Montgomery St BART Station (Market St at 2nd St),37.7896254,-122.400811 has 13 out degrees.
Howard St at 2nd St,37.787521780456245,-122.39740490913391 has 13 out degrees.
3rd St at Townsend St,37.77874161153677,-122.39274082710836 has 13 out degrees.
MacArthur BART Station,37.82840997305853,-122.26631462574005 has 13 out degrees.
======================================================================
[success] Total time: 168 s, completed Apr 27, 2018 11:21:00 PM
```

## Process Dataset
```
> run
[warn] Multiple main classes detected.  Run 'show discoveredMainClasses' to see the list

Multiple main classes detected, select one to run:

 [1] team3.bikeshare.project.BigBikeGraphBikeMaintainance
 [2] team3.bikeshare.project.BigBikeGraphDegreesRatio
 [3] team3.bikeshare.project.BigBikeGraphOutBoundInBound
 [4] team3.bikeshare.project.BikeShareAppFordGoDataset
 [5] team3.bikeshare.project.BikeShareAppPageRank

Enter number: 4

[info] Running team3.bikeshare.project.BikeShareAppFordGoDataset
Using Spark's default log4j profile: org/apache/spark/log4j-defaults.properties
root
 |-- duration_sec: string (nullable = true)
 |-- start_time: string (nullable = true)
 |-- end_time: string (nullable = true)
 |-- start_station_id: string (nullable = true)
 |-- start_station_name: string (nullable = true)
 |-- start_station_latitude: string (nullable = true)
 |-- start_station_longitude: string (nullable = true)
 |-- end_station_id: string (nullable = true)
 |-- end_station_name: string (nullable = true)
 |-- end_station_latitude: string (nullable = true)
 |-- end_station_longitude: string (nullable = true)
 |-- bike_id: string (nullable = true)
 |-- user_type: string (nullable = true)
 |-- member_birth_year: string (nullable = true)
 |-- member_gender: string (nullable = true)

+----------------+--------------------+
|start_station_id|  start_station_name|
+----------------+--------------------+
|             102|  Irwin St at 8th St|
|              20|Mechanics Monumen...|
|             149|Emeryville Town Hall|
|              66|3rd St at Townsen...|
|              44|Civic Center/UN P...|
|             321|       5th at Folsom|
|             239|Bancroft Way at T...|
|              39|Scott St at Golde...|
|              17|Embarcadero BART ...|
|              30|San Francisco Cal...|
|             150|Adeline St at 40t...|
|               9|Broadway at Batte...|
|             195| Bay Pl at Vernon St|
|             200|2nd Ave at E 18th St|
|             243|Bancroft Way at C...|
|             181|Grand Ave at Webs...|
|              64|5th St at Brannan St|
|              72| Page St at Scott St|
|              62|Victoria Manalo D...|
|               5|Powell St BART St...|
+----------------+--------------------+
only showing top 20 rows

>> Total number of stations : 104
Total Number of Stations: 104
Total Number of Trips: 94
Total Number of Trips in Original Data: 94
[success] Total time: 168 s, completed Apr 27, 2018 11:21:41 PM
>
```

## PageRank
> run
[warn] Multiple main classes detected.  Run 'show discoveredMainClasses' to see the list

Multiple main classes detected, select one to run:

 [1] team3.bikeshare.project.BigBikeGraphBikeMaintainance
 [2] team3.bikeshare.project.BigBikeGraphDegreesRatio
 [3] team3.bikeshare.project.BigBikeGraphOutBoundInBound
 [4] team3.bikeshare.project.BikeShareAppFordGoDataset
 [5] team3.bikeshare.project.BikeShareAppPageRank

Enter number: 5

[info] Running team3.bikeshare.project.BikeShareAppPageRank
Using Spark's default log4j profile: org/apache/spark/log4j-defaults.properties
Processing 999 datapoints
Valencia St at 24th St,37.7524278,-122.4206278 has a pagerank of 333
Addison St at Fourth St,37.866249,-122.2993708 has a pagerank of 320
2nd Ave at E 18th St,37.800213566969795,-122.25381016731262 has a pagerank of 228
Market St at 10th St,37.776619,-122.417385 has a pagerank of 222
Valencia St at 16th St,37.765052,-122.4218661 has a pagerank of 198
Golden Gate Ave at Polk St,37.78127,-122.41874 has a pagerank of 195
San Fernando St at 4th St,37.335885,-121.88566 has a pagerank of 193
San Francisco Caltrain (Townsend St at 4th St),37.776598,-122.395282 has a pagerank of 189
20th St at Bryant St,37.7592005,-122.409851 has a pagerank of 184
San Salvador St at 9th St,37.333955,-121.877349 has a pagerank of 182
[success] Total time: 3956 s, completed Apr 29, 2018 7:13:17 PM
>

