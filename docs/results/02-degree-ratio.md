# Degree Ratio

This application converts the input to a graph, compute the out to in degree ratio of each vertex and stores the result back to HDFS.

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