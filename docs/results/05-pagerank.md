# PageRank

PageRank measures the importance of each vertex in a graph, by determining which vertexes have the most edges with other vertexes. In our example, we can use PageRank to determine which bike stations are the most important by measuring which stations have the most connections to other stations.

```
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
```