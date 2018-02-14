## Bilgetech Backend Developer Challenge #3

### Introduction:
We want you to develop a full, working project and showcase your technical abilities and coding skills. You are free to do research on the topics you are not experienced yet, since we also want to evaluate your learning and adaptation skills.

### Time Limit:

Although the time limit is not strict and we encourage you to do your best while coding the project, we expect you return the challenge in a reasonable amount of time since we cross-evalute your performance with the other applicants.

### Evaluation Methodology
Please check out [this document](/evaluation-criteria.md) to learn how will your solution be evaluated by us.

### Plagiarism
Please check out [this document](/plagiarism.md) before you start to work.

### Project Specification:
The local railroad company needs a text interface to add new routes between towns, update the distance of the existing routes, and query existing routes.
Write a program which parses the commands given in the input text and then executes those commands, producing the desired output. The query command should output '-' in case there is no such route. (Think of utilizing the Command Pattern when thinking of a solution.)
We want you to build a .NET Core 2.0 console application with included unit tests.

#### Test Input:
A-B:5, B-C:4, QUERY(A-B), C-D:1, D-C:8, D-E:6, QUERY(C-D), A-D:5, C-D:8, QUERY(C-D), C-E:2, E-B:3, QUERY(A-C), A-E:7

#### Test Output:
A-B:5

C-D:1

C-D:8

A-C:-
