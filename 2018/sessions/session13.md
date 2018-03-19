---
layout: default2018
title: "ICMS 2018 - Session 13: Symbolic Combinatorics"
---
## Session13. Symbolic Combinatorics 

### Organizers

*   [Stephen Melczer](mailto:smelczer@sas.upenn.edu) (University of Pennsylvania)

### Aim and Scope

Symbolic Combinatorics is roughly defined as the application of symbolic algorithms to problems in enumerative and algebraic combinatorics.  This session aims to publicize recent algorithms, software implementations, and various applications.

### Topics

Topics include the manipulation of generating functions, algorithms for asymptotics, and the study of multivariate integer sequences.

### Accepted Talks

#### guessfunc: A new software package for the automated conjecturing of generating functions
#### [Jay Pantone](http://jaypantone.com/) (Dartmouth College)

It's very common in combinatorics to have an efficient method to compute initial terms of a counting sequence, yet still not know the generating function for these terms. There are several well-known and effective tools to help you automatically conjecture the exact generating function of a sequence given some initial terms, including Gfun in Maple, Guess in Mathematica, and Guess in FriCAS. 

We present a new software package to accomplish this task: "guessfunc". Based in Maple, guessfunc has several advantages over existing tools, which either cannot search for differentially algebraic generating functions or traverse the search space of these functions in an inefficient way. In this talk we'll explain briefly how guessfunc works internally and how it can be used as an effective tool in combinatorics.


#### IntegerSequences: a package for computing with k-regular sequences
#### [Eric Rowland](https://people.hofstra.edu/Eric_Rowland/) (Hofstra University)

Sequences satisfying linear recurrences with constant coefficients are well known in combinatorial settings.  Base-k analogues, termed "k-regular sequences", were introduced by Allouche & Shallit in 1992.  The motivation primarily came from theoretical computer science as a generalization of sequences produced by finite automata, but k-regular sequences have appeared increasingly in combinatorics, particularly when one is interested in number theoretic aspects.  IntegerSequences is a Mathematica package for guessing and computing with one-dimensional and multidimensional k-regular sequences.  Recent applications have included establishing the structure of extremal a/b-power-free words, obtaining a product formula for the generating function enumerating binomial coefficients by their p-adic valuations, and computing diagonals of rational functions modulo prime powers.


#### Asymptotics from multivariate generating functions
#### [Mark C. Wilson](https://www.cs.auckland.ac.nz/people/mc-wilson) (University of Auckland)

Work by Robin Pemantle, the speaker, and several others has developed a substantial theory allowing asymptotic coefficient extraction from sufficiently nice (e.g. rational) multivariate generating functions. It involves algebraic-geometric computations at points of the variety given by the vanishing set of the denominator. A package to perform the computations, written by Alex Raichev, is now included in the core Sage distribution. It works well on cases where the relevant computations only require global factorization. However the general theory, motivated by important examples, involves local computations, and these are not implemented yet. I will describe the functionality of this package and hope to obtain audience feedback on improving it.


#### Applied symbolic combinatorics and the PI4 program
#### [Stephen Melczer](https://www.math.upenn.edu/~smelczer/) (University of Pennsylvania)

The 2018 PI4 workshop in Analytic Combinatorics ran at the University of Illinois Urbana-Champaign from June to mid-July.  This talk will describe the output of that workshop, in which graduate students arranged into teams and worked on creating and implementing algorithms related to analytic combinatorics.  In addition to the problems students addressed, potential future projects for graduate students will also be discussed.

