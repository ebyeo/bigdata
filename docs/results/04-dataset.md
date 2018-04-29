# Dataset

This application compiles the number of vertices, edges in the dataset.

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