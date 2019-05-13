# TSP
The travelling salesman problem (TSP) is well-known in computer science and combinatorial optimization. It is the "meta-problem" in many applications in operation research problems. Though NP-hard problem, but it has tons of heuristic algorithms, where Lin–Kernighan is one of the best heuristics for solving the symmetric travelling salesman problem. 

# Lin–Kernighan Algorithm
The idea of Lin–Kernighan is simple: keep swap nodes such that the formed new tour has low cost, and terminate if loop for every nodes until no improvement found. Lin–Kernighan is very efficient (I didn't believe it until I coded it out) and has add-on refinements. The most refinements I learned are about how to choose a neighbor set for a swapping node, where LKH algorithm almost outperform others.

During the intern, I implemented LK algorithm tested with graph (100~1000 nodes). The gap-to-optimal are within 2% for ~100 nodes and 5% for ~1000 nodes.

# GTSP
With LK algorithm, we are able to solve some generilzed TSP problems as follows


where we try to loop one node for each cluster with minimum cost. The generilzed TSP has many real applications (e.g. ).
