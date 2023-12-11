# Repulsive Curves
Paper review of  ["Repulsive Curves"](https://arxiv.org/pdf/1802.06552.pdf)

### Context
 
- Program: [MVA Master's degree](https://www.master-mva.com/) class on Geometric Data Analysis. ENS Paris-Saclay.
- Authors:
    - [David Sahna](https://github.com/Dave78300)
    - [Mathis Embit](https://github.com/mathisemb)
    

------
## Abstract
Curves play a fundamental role across computer graphics, physical simulation, and mathematical visualization, yet most tools for curve design do nothing to prevent crossings or self-intersections. 
This paper develops efficient algorithms for (self-)repulsion of plane and space curves that are well-suited to problems in computational design. Our starting point is the so-called tangent-point energy, 
which provides an infinite barrier to self-intersection. In contrast to local collision detection strategies used in, e.g., physical simulation, this energy considers interactions between all pairs 
of points, and is hence useful for global shape optimization: local minima tend to be aesthetically pleasing, physically valid, and nicely distributed in space. 
A reformulation of gradient descent, based on a Sobolev-Slobodeckij inner product enables us to make rapid progress toward local minima---independent of curve resolution. 
We also develop a hierarchical multigrid scheme that significantly reduces the per-step cost of optimization.
The energy is easily integrated with a variety of constraints and penalties (e.g., inextensibility, or obstacle avoidance), which we use for applications including curve packing, knot untangling, graph embedding, non-crossing spline interpolation, flow visualization, and robotic path planning.
