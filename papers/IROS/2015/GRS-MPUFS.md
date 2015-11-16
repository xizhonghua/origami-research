# Motion planning using first-order synergies
N. García, J. Rosell and R. Suárez

### Abstract
This paper proposes a novel motion planning
approach that exploits the concept of synergies (correlations)
between degrees of freedom, extending it to the velocity space
and calling them first-order synergies. An automatic partition
method is defined to optimally divide the configuration space
into cells where first-order synergies are significantly different.
Using this partition, an algorithm that tends to grow a tree
by extending the branches in the directions determined by the
the first-order synergies of the cell where the leaf to be grown
lies is introduced and called FOS-RRT. This allows the natural
expansion of the tree along the directions determined by the
data used to define the synergies. 2D examples illustrate the
performance of the proposed approach, which is particularly
attractive for potential applications in human-like robots using
human synergies.

### Summary
Partion the configuration spaces into zones according to the first-order synergies (velocity). Fos-RRT expansion in each zone has different weights along each axis according to the synergies.

### Pros
* More nature solutions

### Cons
* Samples required (training)
* No completeness proof
* Can lead to poor performance if cross zone extension happened at improper location
* Unfair experiments
