# Dynamically Pruned A* for Re-planning in Navigation Meshes
Wouter van Toll and Roland Geraerts

### Abstract 
Modern simulations feature crowds of AIcontrolled
agents moving through dynamic environments, with
obstacles appearing or disappearing at run-time. A dynamic
navigation mesh can represent the traversable space of such environments.
The A* algorithm computes optimal paths through
the dual graph of this mesh. When an obstacle is inserted
or deleted, the mesh changes and agents should re-plan their
paths. Many existing re-planning algorithms are too memoryintensive
for crowds, or they cannot easily be used on graphs
where vertices and edges are added or removed.
In this paper, we present Dynamically Pruned A* (DPA*), an
extension of A* for re-planning optimal paths in dynamic navigation
meshes. DPA* has similarities to adaptive algorithms that
make the A* heuristic more informed based on previous queries.
However, DPA* prunes the search using only the previous path
and its relation to the dynamic event. We describe the four replanning
scenarios that can occur; DPA* uses different rules
in each scenario. Our algorithm is memory-friendly and robust
against structural changes in the graph, which makes it suitable
for crowds in dynamic navigation meshes. Experiments show
that DPA* performs particularly well in complex environments
and when the dynamic event is visible to the agent. We integrate
the algorithm into crowd simulation software to model large
crowds in dynamic environments in real-time.

### Summary
Graph serach on dual graph of the walkable mesh. Propose DPA* that only remembers the previous optimal path and handles dynamic events (insertion and deletion) properly to improve the replanning efficiency by resuing the path segments from previous path which also guarantees the optimality of the path.

### Pros
1. Better performance on large mesh compare to A*

### Cons
1. negtive improvement on smaller mesh
2. hard to implement
3. poor performance when there are lots of dynamic events (estimated)
