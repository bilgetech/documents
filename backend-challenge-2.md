## Bilgetech Backend Developer Challenge #2

### Introduction:
We want you to develop a full, working project and showcase your technical abilities and coding skills. You are free to do research on the topics you are not experienced yet, since we also want to evaluate your learning and adaptation skills.

### Time Limit:

Although the time limit is not strict and we encourage you to do your best while coding the project, we expect you return the challenge in a reasonable amount of time since we cross-evalute your performance with the other applicants.

### Evaluation Methodology
Please check out [this document](/evaluation-criteria.md) to learn how will your solution be evaluated by us.

### Plagiarism
Please check out [this document](/plagiarism.md) before you start to work.

### Project Specification:
The local railroad covers a number of towns. All of the tracks are 'one-way.' 
A route from town A to town B does not imply the existence of a route from town B to town A. 
Even if both of these routes exist, they are distinct and are not necessarily the same distance!
The purpose of this problem is to find all the different paths between two towns.
(You can use either depth-first or breadh-first graph traversal algorithms.)
We want you to build a .NET Core 2.0 console application with included unit tests.

#### Input:
The first line is a directed graph where a node represents a town and an edge represents a route between two towns. 
The weighting of the edge represents the distance between the two towns. 
A given route will never appear more than once, and for a given route, the starting and ending town will not be the same town.
The second line starts with PATH and asks you to find all the paths starting from a town and ending in a town having a maximum distance.
In the test input given below, you will find all paths starting at C and ending at C, with total distance less than 30.

#### Test Input:
A-B:5, B-C:4, C-D:8, D-C:8, D-E:6, A-D:5, C-E:2, E-B:3, A-E:7

PATHS(C-C,30)

#### Output:
If no such route exists, output '-', otherwise, output all the town names on the found path.

#### Test Output:
CDC, CEBC, CEBCDC, CDCEBC, CDEBC, CEBCEBC, CEBCEBCEBC


