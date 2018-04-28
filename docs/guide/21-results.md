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
 [5] team3.bikeshare.project.BikeShareAppHDFS
 [6] team3.bikeshare.project.BikeShareAppPageRank

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
 [5] team3.bikeshare.project.BikeShareAppHDFS
 [6] team3.bikeshare.project.BikeShareAppPageRank

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
 [5] team3.bikeshare.project.BikeShareAppHDFS
 [6] team3.bikeshare.project.BikeShareAppPageRank

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
 [5] team3.bikeshare.project.BikeShareAppHDFS
 [6] team3.bikeshare.project.BikeShareAppPageRank

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

## HDFS
```
> run
[warn] Multiple main classes detected.  Run 'show discoveredMainClasses' to see the list

Multiple main classes detected, select one to run:

 [1] team3.bikeshare.project.BigBikeGraphBikeMaintainance
 [2] team3.bikeshare.project.BigBikeGraphDegreesRatio
 [3] team3.bikeshare.project.BigBikeGraphOutBoundInBound
 [4] team3.bikeshare.project.BikeShareAppFordGoDataset
 [5] team3.bikeshare.project.BikeShareAppHDFS
 [6] team3.bikeshare.project.BikeShareAppPageRank

Enter number: 5

[info] Running team3.bikeshare.project.BikeShareAppHDFS
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

+------------+--------------------+--------------------+----------------+--------------------+----------------------+-----------------------+--------------+--------------------+--------------------+---------------------+-------+----------+-----------------+-------------+
|duration_sec|          start_time|            end_time|start_station_id|  start_station_name|start_station_latitude|start_station_longitude|end_station_id|    end_station_name|end_station_latitude|end_station_longitude|bike_id| user_type|member_birth_year|member_gender|
+------------+--------------------+--------------------+----------------+--------------------+----------------------+-----------------------+--------------+--------------------+--------------------+---------------------+-------+----------+-----------------+-------------+
|       75284|2018-01-31 22:52:...|2018-02-01 19:47:...|             120|Mission Dolores Park|            37.7614205|           -122.4264353|           285|Webster St at O'F...|   37.78352083526095|  -122.43115782737732|   2765|Subscriber|             1986|         Male|
|       85422|2018-01-31 16:13:...|2018-02-01 15:57:...|              15|San Francisco Fer...|             37.795392|            -122.394203|            15|San Francisco Fer...|           37.795392|          -122.394203|   2815|  Customer|             null|         null|
|       71576|2018-01-31 14:23:...|2018-02-01 10:16:...|             304|Jackson St at 5th St|      37.3487586867448|    -121.89479783177376|           296|5th St at Virgini...|          37.3259984|           -121.87712|   3039|  Customer|             1996|         Male|
|       61076|2018-01-31 14:53:...|2018-02-01 07:51:...|              75|Market St at Fran...|      37.7737932060887|    -122.42123901844025|            47|4th St at Harriso...|   37.78095459960753|  -122.39974915981291|    321|  Customer|             null|         null|
|       39966|2018-01-31 19:52:...|2018-02-01 06:58:...|              74|Laguna St at Haye...|    37.776434819204745|    -122.42624402046204|            19|Post St at Kearny St|           37.788975|          -122.403452|    617|Subscriber|             1991|         Male|
|        6477|2018-01-31 22:58:...|2018-02-01 00:46:...|             236| Market St at 8th St|            37.8036865|            -122.282497|           160|West Oakland BART...|          37.8053183|         -122.2948365|   1306|  Customer|             null|         null|
|         453|2018-01-31 23:53:...|2018-02-01 00:01:...|             110|17th & Folsom Str...|            37.7637085|           -122.4152042|           134|Valencia St at 24...|          37.7524278|         -122.4206278|   3571|Subscriber|             1988|         Male|
|         180|2018-01-31 23:52:...|2018-01-31 23:55:...|              81|  Berry St at 4th St|              37.77588|             -122.39317|            93|4th St at Mission...|          37.7704074|         -122.3911984|   1403|Subscriber|             1980|         Male|
|         996|2018-01-31 23:34:...|2018-01-31 23:51:...|             134|Valencia St at 24...|            37.7524278|           -122.4206278|             4|Cyril Magnin St a...|   37.78588062694133|   -122.4089150084319|   3675|Subscriber|             1987|         Male|
|         825|2018-01-31 23:34:...|2018-01-31 23:47:...|             305|         Ryland Park|             37.342725|            -121.895617|           317|San Salvador St a...|           37.333955|          -121.877349|   1453|Subscriber|             1994|       Female|
|        1316|2018-01-31 23:24:...|2018-01-31 23:45:...|              98|Valencia St at 16...|             37.765052|           -122.4218661|             4|Cyril Magnin St a...|   37.78588062694133|   -122.4089150084319|   1278|  Customer|             null|         null|
|         432|2018-01-31 23:34:...|2018-01-31 23:41:...|              89|Division St at Po...|     37.76921786152374|    -122.40764558315276|            43|San Francisco Pub...|          37.7787677|         -122.4159292|   2928|Subscriber|             1993|         Male|
|         601|2018-01-31 23:29:...|2018-01-31 23:39:...|             223|16th St Mission B...|      37.7647652154977|    -122.42009103298186|            86|Market St at Dolo...|          37.7693053|         -122.4268256|   3016|Subscriber|             1957|         Male|
|         887|2018-01-31 23:24:...|2018-01-31 23:39:...|             308|    San Pedro Square|             37.336802|           -121.8940901|           297|Locust St at Gran...|          37.3229796|         -121.8879312|     55|Subscriber|             1976|       Female|
|         210|2018-01-31 23:33:...|2018-01-31 23:36:...|               7| Frank H Ogawa Plaza|      37.8045623549303|    -122.27173805236816|           186|Lakeside Dr at 14...|          37.8013189|         -122.2626418|   2602|Subscriber|             1976|         Male|
|         188|2018-01-31 23:30:...|2018-01-31 23:34:...|              98|Valencia St at 16...|             37.765052|           -122.4218661|            76|McCoppin St at Va...|   37.77166246221617|  -122.42242321372034|   2556|Subscriber|             1964|       Female|
|         808|2018-01-31 23:19:...|2018-01-31 23:33:...|              67|San Francisco Cal...|            37.7766392|           -122.3955263|            98|Valencia St at 16...|           37.765052|         -122.4218661|   3041|Subscriber|             1976|         Male|
|         378|2018-01-31 23:23:...|2018-01-31 23:29:...|              80|Townsend St at 5t...|            37.7753058|             -122.39738|            78| Folsom St at 9th St|          37.7737172|         -122.4116467|    546|Subscriber|             1995|       Female|
|         350|2018-01-31 23:13:...|2018-01-31 23:19:...|             247|Fulton St at Banc...|            37.8677892|           -122.2658964|           274|Oregon St at Adel...|          37.8575672|         -122.2675583|    431|Subscriber|             null|         null|
|         686|2018-01-31 23:07:...|2018-01-31 23:18:...|             312|San Jose Diridon ...|             37.329732|            -121.901782|           317|San Salvador St a...|           37.333955|          -121.877349|   1886|Subscriber|             1997|       Female|
+------------+--------------------+--------------------+----------------+--------------------+----------------------+-----------------------+--------------+--------------------+--------------------+---------------------+-------+----------+-----------------+-------------+
only showing top 20 rows

+----------------+--------------------+
|start_station_id|  start_station_name|
+----------------+--------------------+
|             323|  Broadway at Kearny|
|             102|  Irwin St at 8th St|
|              20|Mechanics Monumen...|
|             126|         Esprit Park|
|             149|Emeryville Town Hall|
|             259|Addison St at Fou...|
|              44|Civic Center/UN P...|
|              66|3rd St at Townsen...|
|             321|       5th at Folsom|
|             318|San Carlos St at ...|
|             296|5th St at Virgini...|
|             239|Bancroft Way at T...|
|             130|22nd St Caltrain ...|
|              76|McCoppin St at Va...|
|              39|Scott St at Golde...|
|              17|Embarcadero BART ...|
|             101|San Bruno Ave at ...|
|              30|San Francisco Cal...|
|             172|College Ave at Ta...|
|             177|MacArthur Blvd at...|
+----------------+--------------------+
only showing top 20 rows

>> Total number of stations : 240
Total Number of Stations: 240
Total Number of Trips: 828
Total Number of Trips in Original Data: 828
[success] Total time: 112 s, completed Apr 27, 2018 11:25:24 PM
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
 [5] team3.bikeshare.project.BikeShareAppHDFS
 [6] team3.bikeshare.project.BikeShareAppPageRank

Enter number: 6

[info] Running team3.bikeshare.project.BikeShareAppPageRank
Using Spark's default log4j profile: org/apache/spark/log4j-defaults.properties
Processing 999 datapoints
