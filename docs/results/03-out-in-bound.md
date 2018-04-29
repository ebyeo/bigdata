# Out Bound / In Bound

This application convert the file into graph, computes the in and out degree of each vertex and stores the lists to HDFS.

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