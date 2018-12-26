# kbnumber
Six Degrees of Kevin Bacon is a game based on the concept of "six degrees of separation", which posits that any two people on Earth are six or fewer acquaintance links apart. Movie buffs challenge each other to find the shortest path between an arbitrary actor and actor Kevin Bacon.
The “Six Degrees of Kevin Bacon” game is really a graph problem. If you assign each actor to a vertex, and add an edge between two actors if they have appeared together in a movie, then you have a graph that represents the data for this game. Then the problem of finding a trail of actors to Kevin Bacon becomes a traditional graph problem: that of finding a path between two vertices. Since we wish to find a shortest path, one might think to apply Dijkstra's shortest path algorithm to this problem, but that would be overkill since Dijkstra's algorithm is meant for situations when each edge has an associated length (or weight) and the goal is to find the path with the shortest cumulative length. Because we are only concerned with finding the shortest paths in terms of the number of edges, the Breadth-First Search algorithm will solve the problem. Breadth-First Search builds a tree of shortest paths from every actor who can reach Kevin Bacon back to Kevin Bacon. Or more generally, given a root, Breadth-First Search builds a shortest-path tree from every vertex that can reach the root back to the root.
In this problem I used C++ to generate the Bacon Number for any actor input by the user. Running the program defaultly (./PA3) via terminal on mac, or a linux based vm, will read default files.
