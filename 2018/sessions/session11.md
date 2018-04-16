---
layout: default2018
title: "ICMS 2018 - Session 11: Backtrack search techniques in groups and combinatorics"
---
## Session11. Backtrack search techniques in groups and combinatorics

### Organizers

*   [Markus Pfeiffer](mailto:markus.pfeiffer@st-andrews.ac.uk) (School of Computer Science, St Andrews, UK)
*   [Christopher Jefferson](mailto:caj21@st-andrews.ac.uk) (School of Computer Science, St Andrews, UK)

### Aim and Scope

Backtrack search is a vital part of solving many problems in computational group
  theory, such as graph isomorphism, finding (non-point) stabilisers and
  normalisers in permutation groups, finding canonical images of objects under a
  group action, or short solutions to equations over a free group.

  Efficient backtrack search implementations require a symbiosis of efficient algorithms,
  high-performance code, and sophisticated mathematical methods to prune search
  space. Some of the most prominent backtrack methods in computational mathematics
  are McKay's graph isomorphism algorithm, Jeffrey Leon's partition backtrack
  method for permutation groups, and Bernd Schmalz' "snakes and ladders" algorithm.

  Many breakthroughs in AI-search, such as learning, heuristics and parallelism,
  can improve performance by multiple orders of magnitude, and are applicable in
  computational group theory.

### Topics

  We would like to invite experts from AI, combinatorics, computational group
  theory and related areas with the aim of sharing and exchanging ideas, problems,
  results and implementations.

### Accepted Talks

#### The Theory and Practice of Refiners in Partition Backtracking
#### [Christopher Jefferson](https://caj.host.cs.st-andrews.ac.uk/) (St Andrews, UK)


The Partition Backtracking algorithm of Jeffrey S. Leon has provided the basis for the state of the art for a large range of permutation group problems, including intersection, stabilizer and normaliser, for almost 30 years. This algorithm is however poorly understood.

This talk will give a rapid overview of the most important parts of the algorithm. In particular, I will talk about refiners, which are the central core of the algorithm. I will demonstrate some new refiners, and show how adding new refiners can provide and easy way to both improve performance on existing problems and extend existing partition backtrack systems to support new problems.


#### Towards practical subgroup conjugacy
#### Robin Candy (Australian National University, Australia)

Leon claims that a method related to his celebrated Partition Backtrack Algorithm (PBA) can be used to solve canonical-representative-type problems, however speciﬁc details were never given. Although the PBA has been used to vastly speed up computation of normalisers and subgroup conjugacy in permutation groups, there has been very little progress made in methods to ﬁnd canonical subgroups up to conjugacy.

In this talk I describe how to combine aspects of the PBA and McKay’s graph isomorphism algorithm nauty to ﬁnd canonical images of groups up to conjugacy in the symmetric group. I will focus on speciﬁc diﬀerences between the two algorithms and how they relate to pruning the search tree. In addition, I will address practical concerns such as implementation and performance details.

#### Questions on orbital graphs
#### Paula Hähndel, Rebecca Waldecker (Martin Luther University of Halle-Wittenberg, Germany) 
Short abstract:
Building on previous work on orbital graphs, we consider questions of 
theoretical interest that are also directly relevant for backtrack search algorithms. The underlying 
idea is to use orbital graphs as a tool for pruning the search tree in 
backtrack methods. Just two examples:
Can we characterise the groups that can be recognised from their orbital 
graphs?
When dealing with groups that have orbital graphs of different "quality" 
as a pruning tool, how can we efficiently detect the best graphs?

#### [A Rainbow Clique Search Algorithm for BLT-Sets](../session11-rainbow.pdf)
#### Abdullah Al-Azemi (Kuwait University), Anton Betten and Sajeeb Roy Chowdhury  (Colorado State University)

We consider the problem of classifying combinatorial-geometric structures by computer. A BLT-set is a set of q + 1 points in an orthogonal space Q(4,q) deﬁned over a ﬁnite ﬁeld with q elements. The points satisfy a quadratic equation such as x²₀+x₁x₂+x₃x₄=0 and there is a triple condition which says that no other point on the quadric is collinear to three of the points in the chosen set. The problem is that of classifying the possibilities of these sets up to equivalence under the orthogonal group.

After some reductions which involve the symmetry of the quadric, the problem can be phrased as a problem of ﬁnding rainbow cliques in suitable graphs. This is a diﬃcult problem in computer science and quite a few CPU-cycles have been utilized to push the classiﬁcation further. Several inﬁnite families of BLT-sets are known but there is still a lot of example which are sporadic. The present talk describes work to make the search more eﬃcient and extend the classiﬁcation to the next open case, which is when q = 73. Our computations are facilitated using the C++ package Orbiter as well as some independent implementations ustilizing multithreading.

#### [How fast can we compute orbits of groups?](../session11-orbits.pdf)
#### Anton Betten (Colorado State University)

Many problems in Combinatorics and related ﬁelds reduce to the problem of computing orbits of groups acting on ﬁnite sets. These problems are about classifying objects of a certain type. The main techniques are these: There is canonical augmentation and Snakes and Ladders. In this talk, we would like to give the theoretical framework for both techniques and compare the performance of some of the available implementations. Orbiter is a C++ package which provides an implementation of Snakes and Ladders. Another implementation exists in the computer algebra system GAP, using the Fining package for ﬁnite geometry. An implementation in Magma would be desirable. The canonical augmentation algorithm has been implemented in Nauty and more recently in Traces.

