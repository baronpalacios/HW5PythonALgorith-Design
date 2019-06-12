# HW5PythonALgorith-Design
HW5PythonALgorith

1
A small business lets say, a photocopying service with a single large machine faces the
following scheduling problem. Each morning they get a set of jobs from customers. They want
to do the jobs on their single machine in an order that keeps their cus tomers happiest. Job of
customer i will take t i time to complete. Given a schedule (i.e., an ordering of the jobs), let C i
denote the finishing time of job i. For example, if job j is the first to be done, we would have C j
= t j ; and if job j is done right after job i, we would have C j = C i + t j . Each customer i also has a
given weight w i that represents his or her importance to the business. The happiness of
customer i is expected to be dependent on the finishing time of i s job. So the company decides
tha t they want to order the jobs to minimize the weighted sum of the completion times,
Σ𝑊𝑖𝑛𝑖=1.𝐶𝑖
Propose a greedy algorithm to solve this problem. That is, you are given a set of n jobs with a
processing time t i and a weight w i for each job. You want t o order the jobs to minimize the
weighted sum of the completion times, Σ𝑊𝑖𝑛𝑖=1.𝐶𝑖 Implement the algorithm with Python.
For an example, suppose there are two jobs: the first takes time t
1 = 1 and has weight w 1 = 10,
while the second job takes time t 2 = 3 and has weight w 2 = 2. Then doing job 1 first would yield a
weighted completion time of 10.1 + 2.4 = 18, while doing the second job first would yield the larger
weighted completion time of 10.4 + 2.3 = 46.



2
Suppose you re running a lightweight consulting business just you, two associ ates, and
some rented equipment. Your clients are distributed between the East Coast and the West Coast,
and this leads to the following question. Each month, you can either run your business from an
office in New York (NY) or from an office in San Francis co (SF). In month i, you ll incur an
operating cost of N i if you run the business out of NY; you ll incur an operating cost of S i if
you run the business out of SF. (It depends on the distribution of client demands for that month.)
However, if you run the business out of one city in month i, and then out of the other city in
month i + 1, then you incur a fixed moving cost of M to switch base offices.
Given a sequence of n months, a plan is a sequence of n locations
each one equal to either NY
or SF suc h that the i th location indicates the city in which you will be based in the i th month.
The cost of a plan is the sum of the operating costs for each of the n months, plus a moving cost
of M for each time you switch cities. The plan can begin in either cit y.
The problem:
Given a value for the moving cost M, and sequences of operating costs
N
1 ..... N n and S 1 ..... S n , find a plan of minimum cost (Such a plan will be called
For an example,
let s suppose n=4, M=10 and the operating costs are given by the following
table.


![Capture](https://user-images.githubusercontent.com/32982938/59381598-7a52bf00-8d64-11e9-8ac5-af3642973cd7.PNG)
