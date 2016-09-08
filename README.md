"# Traveling-Salesman-Problem" 

From Wikipedia:
The travelling salesman problem (TSP) asks the following question: Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city exactly once and returns to the origin city? It is an NP-hard problem in combinatorial optimization, important in operations research and theoretical computer science.

My goal is to implement multiple approaches to solving this problem. This is more an intellectual excersize than an attempt at finding the most optimal solution. As such, for the most part these documents will include limited testing and benchmarking.

Here are the approaches I've taken to date:
 - Brute force solution: enumerate all possible routes given a set of cities, and choose the one with the shortest overall route distance. This works for N <= 10 cities, but quickly becomes unmanageable for larger Ns. O(N!)
 - Nearest neighbor algorithm: randomly choose a starting city, and sequentially choose the closest city until all cities have been traversed. An approximation algorithm that results in fast solutions, but rarely results in the most optimal solution for larger sets.
 - Improved nearest neighbor algorithm: an implementation of the nearest neighbor algorithm that runs the algorithm once for each city, alternating starting points. The aim is to select the starting point which results in the greatest efficiency with an NN approach.
