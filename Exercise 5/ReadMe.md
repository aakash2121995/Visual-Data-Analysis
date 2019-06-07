## Graph Visualization

a) Use the Breast Cancer Dataset dataset breast-cancer-wisconsin.xlsx and fill in the missing
values. Then compute the Pearson correlation between any pair of variables,
and store them in a matrix.

b) Create a graph from the correlation matrix and visualize it with a force-directed layout. Represent each variable as a node in the graph. Insert an edge between two variables whenever the Pearson correlation between them exceeds the threshold ρ > 0.6.

c) Modify the visual attributes of edges to reflect the magnitude of the correlation.

d) Produce an alternative visualization with a circular layout. Color the nodes so that there are four
set of nodes, one color for having at least one correlation more than 0.9 to other nodes, another for
having at least a correlation 0.8 < ρ max <= 0.9, one for having a correlation 0.6 < ρ max <= 0.8
and the last for the remaining nodes.

e) Answer the following questions:
- At the selected threshold, which nodes are disconnected from the rest of the graph and what
do they indicate?
- If two nodes A and B are strongly correlated, and node C is strongly correlated with node
B, can we conclude that node C will be also strongly correlated with node A?
- Based on the visualization, which variables would you propose to predict the class? (1P)
