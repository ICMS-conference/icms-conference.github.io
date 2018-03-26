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
