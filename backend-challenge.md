## Bilgetech Backend Developer Challenge

### Introduction:
We want you to develop a full, working project and showcase your technical abilities and coding skills. You are free to do research on the topics you are not experienced yet, since we also want to evaluate your learning and adaptation skills.

### Time Limit:

Although the time limit is not strict and we encourage you to do your best while coding the project, we expect you return the challenge in a reasonable amount of time since we cross-evalute your performance with the other applicants.

### Evaluation Methodology
Please check out [this document](/evaluation-criteria.md) to learn how will your solution be evaluated by us.

### Plagiarism
Please check out [this document](/plagiarism.md) before you start to work.

### Project Specification:
There are 10 white-collar workers who will be taken to their homes after long hours of work. They work for a big corporation which arrange them personnel vehicles from the office (starting point) to their houses (destination points). The corporation wants to determine the optimal count of vehicles and their routes to minimise fuel consumption.

We want you to build a .NET Core 2.0 console application that will calculate an [efficient¹](#1-the-term-efficient-does-not-imply-optimality-the-algorithm-or-heuristic-may-be-semi-optimal-or-non-deterministic-it-may-produce-bad-results-for-some-inputs) way to distribute passengers to the vehicles and output the result. Please note that the project will be evaluated by humans and not by automated scripts, so the format of output is up to you as long as it's human-readable :)

For sake of this problem, lets say the only cost is fuel cost (driver costs are neglected) and total fuel spent is proportionate to the total distance travelled. Besides, the capacity of one vehicle is more than 10, so you don't need to consider it in your solution.

The geolocations of the office (Kolektif House) and the passengers can be found in this map: https://goo.gl/H926Q3

To compute an efficient distribution and route you will need to get the travel distance between locations by using a service like: https://developers.google.com/maps/documentation/distance-matrix/

#### Example with 2 passengers:

    S: starting point
    1: destination of the first passenger
    2: destination of the second passenger
    
    distance(S,1) = 5 km
    distance(S,2) = 9 km
    distance(1,2) = 7 km
    
#### Solution to 2 passengers example:

possibility | number of vehicles | route | distance
--|---------------|-------|----------
1 (optimal) | One vehicle | S-1-2 | 5+7=12 km
2 | One vehicle | S-2-1 | 9+7=16 km
3 | Two vehicles | S-1 and S-2 | 5+9=14 km
    
We see that the optimal solution is the first one (S-1-2) which has the smallest distance hence the smallest fuel consumption.



##### [1] The term efficient does not imply optimality. The algorithm (or heuristic) may be semi-optimal or non-deterministic. It may produce bad results for some inputs.</a>
