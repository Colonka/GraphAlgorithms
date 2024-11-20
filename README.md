# GraphAlgorithms

In this project, I've implemented some basic algorithms on graphs

## Introduction

Graphs are one of the basic data structures in programming that are used everywhere. Graphs can be used to interpret road maps, electrical circuits, geographic maps, communication between people in social networks, and many other things.

### Main terms

A **Graph** has a finite set of vertices, and a set of edges. Each edge has two points from the set of graph vertices that form the edge points.

There are **types of graphs based on the type of edges:**
* *Undirected* — a graph in which movement between vertices connected by an edge is possible in any direction.

* *Directed* — a graph, the edges of which have a direction. Directed edges are also called arcs. Moving from one vertex to another is possible only by arcs of corresponding direction.

If besides the edge between two vertices, the weight of the edge is also given, then such a graph is called ***weighted***.

**Types of graphs based on the number of edges:**
* *Null graph* is a graph in which there are no edges/

* *Incomplete* — the graph has edges, but not from every vertex, there is an edge to every other vertex.

* *Complete* — the graph has an edge from each vertex to any other vertex.

**Types of graphs based on node reachability:**

* *Connected* — for any vertex in the graph there is at least one path to any other vertex in the same graph.

* *Disconnected* — the graph has no path between at least two vertices.

For directed graphs there are two more types of connectivity: *strongly connected* and *weakly connected*.
* *Strongly connected* — there is a path for any vertex in a directed graph to any other vertex and back. 
* *Weakly connected* — there is a path between any two vertices in the graph, but this path can be one-sided.
It means that from vertex A to vertex B the path can exist, but not the opposite way.

**Trees**

An important subtype of graphs are *trees*. \
***A tree*** is a connected acyclic graph in which any two vertices are connected by only one path. The following formula is the same for all trees: *q = n - 1*, where q is the number of edges, n is the number of vertices of the graph (tree). Trees can be built from either undirected or directed graphs, depending on the problem to be solved.

***A spanning tree*** is a subgraph of a given graph that contains all of its vertices and is a tree. The graph edges that are not part of the spanning tree are called chords of the graph relative to the spanning tree.

### Ways of representing a graph

The main ways of representing graphs are:
* *an adjacency matrix* is a square matrix whose dimension is equal to the number of vertices in the graph, and in which $`A_{ij}`$ element of the matrix contains information about an edge from vertex $`i`$ to vertex $`j`$. Possible values that $`A_{ij}`$ can have:
    + For an unweighted undirected graph:
        - 0 — there is no edge between the vertices;
        - 1 — there is an edge between the vertices.
    + For a weighted undirected graph:
        - 0 — there is no edge between the vertices;
        - N — there is an edge between vertices, and its weight is N.
    + For an unweighted directed graph:
        - 0 — there is no arc between the vertices;
        - 1 — there is an arc (directed edge), which is directed from vertex $`i`$ to vertex $`j`$.
    + For a weighted directed graph:
        - 0 — there is no arc between the vertices;
        - N — there is an arc (directed edge), which is directed from vertex $`i`$ to vertex $`j`$, and its weight is N.
  
## Instructons for running

Being in `src` folder run command `make`

## Instruction for archiving

Being in `src` folder run command `make dist` that create folder with archived app.

## Instruction for testing

Being in `src` folder run command `make tests`

## Instruction for gcov test coverage

Being in `src` folder run command `make gcov_report`

## Documentation

To open library documentation run command `dvi`

## App instructions

1) Run app command `make`
2) Choose file with adjacency matrix
3) Choose action what you want to do with graph
4) Tap 'Enter' to choose another action or '0' to exit 
