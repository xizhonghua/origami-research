# Multi-Objective Cost-to-Go Functions on Robot Navigation in Dynamic
Environments
Gonzalo Ferrer and Alberto Sanfeliu

### Abstract
 In our previous work we introduced the
Anticipative Kinodynamic Planning (AKP): a robot navigation
algorithm in dynamic urban environments that seeks to minimize
its disruption to nearby pedestrians. In the present paper,
we maintain all the advantages of the AKP, and we overcome
the previous limitations by presenting novel contributions to our
approach. Firstly, we present a multi-objective cost function to
consider different and independent criteria and a well-posed
procedure to build a joint cost function in order to select the
best path. Then, we improve the construction of the planner
tree by introducing a cost-to-go function that will be shown to
outperform a classical Euclidean distance approach. In order to
achieve real time calculations, we have used a steering heuristic
that dramatically speeds up the process. Plenty of simulations
and real experiments have been carried out to demonstrate the
success of the AKP.

### Summary
Extend their previous work Anticipative Kinodynamic Planning (AKP) using cost-to-go metric instead of Euclidean distance. The the cost function is defined as accumulated weighted normalized average of multiple objectives along the path based on Extended Social Force Model (ESFM). Using Monte Carlo approach to sample the weights, carry out simulations on many different scenarios and compute the costs associated to the sampled weights.

### Pros
1. Higher space coverage
2. Lower cost to reach the goal

### Cons
1. Parameter learning is not optimal
