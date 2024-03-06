---
layout: session
title: "ICMS 2024 - Session 12: Polyhedral geometry and combinatorics</b>"
---
## Organizers
   * [Victoria Schleis (Universität Tuebingen, Germany)](https://victoriaschleis.github.io/)<br/>

## Aim and Scope

This session covers new developments in computational combinatorics and polyhedral geometry.
Particular topics include (but are not limited to) computational methods and new software developed in:<br/>
* polyhedral geometry,<br/>
* tropical geometry, in particular tropical intersection theory and methods on graphs,<br/>
* matroid theory, both purely combinatorial and in its interactions with other areas of mathematics, in particular polyhedral and algebraic geometry.<br/>

The aim of the session is to bring together researchers in different areas of polyhedral and tropical geometry and combinatorics, but also users of different software systems. Details about important implementation techniques are particularly encouraged!

## Accepted Talks

### Eigenvalue Methods for Sparse Tropical Polynomial Systems<br/>
* [Antoine Béreau (École polytechnique, Paris, France)](https://antoine-bereau.fr/)<br/>
We develop an analogue of eigenvalue methods to construct solutions of systems of tropical polynomial equalities and inequalities. We show that solutions can be obtained by solving parametric mean-payoff games, arising to approriate linearizations of the systems using tropical Macaulay matrices. We implemented specific algorithms adapted to the large scale parametric games that arise in this way, and present numerical experiments.<br/>


### Secondary fans of hypersimplices and finite metric spaces<br/>
* [Laura Casabella (MPI Leipzig, Germany)](https://sites.google.com/view/lauracasabella)<br/>
The secondary fan Σ(k,n) is a polyhedral fan which stratifies the regular subdivisions of the hypersimplices Δ(k,n). Using TOPCOM, MTOPCOM and POLYMAKE, we compute the fans Σ(2,7) and Σ(3,6). We also find new families of rays of Σ(k,n) which do not lie on the respective Dressians.
In the special case k=2 our results are closely related to metric spaces on n points. This is joint work with Michael Joswig and Lars Kastner.<br/>



### Counting Tropical Curves in P1xP1: Computation & Polynomiality Properties<br/>
 * [Daniel Corey (University of Nevada, Las Vegas, United States)](https://sites.google.com/site/dcorey2814/)<br/>
 By the celebrated correspondence theorem of Mikhalkin, counting curves in P2 with prescribed numerical restrictions can be achieved by counting tropical curves with similar numerical restrictions, and in turn, by counting lattice paths in a triangle with a suitable multiplicity function. This correspondence readily generalizes to any smooth toric surface. We implement Mikhalkin's lattice path algorithm for an arbitrary lattice polygon and with arbitrary boundary conditions in Polymake, and use this to determine new polynomial structures on counts of rational curves in P1xP1 with fixed contact orders to the 0 and infinity sections, and variable contact orders to the 0 and infinity fibers. This is based on joint work with Hannah Markwig and Dhruv Ranganathan.<br/>



### Generalising Tropical Homotopies towards Tropical Intersection Products<br/>
 * [Oliver Daisey (Durham University, UK)](https://www.durham.ac.uk/staff/oliver-j-daisey/)<br/>
In 2016, Anders Jensen developed a tropical analogue of homotopy continuation to compute the stable intersection of n tropical hypersurfaces in R^n.  Jensen's main motivation was the computation of mixed volumes and applications to polyhedral homotopies. The algorithm was initially implemented in Gfan, where it is still powering the mixed volume computation to date.  Since then, polynomial system solvers like HomotopyContinuation.jl have picked up the algorithm and are using it for polyhedral homotopies.

In this talk, we will formalise Jensen's approach to families of balanced polyhedral complexes that we consider “properly dualisable”, with the aim of laying the foundations for future generalisations of Jensen's approach. We provide concrete details for tropical hypersurfaces, tropical linear spaces, and what we call “inverted tropical linear spaces”. Finally, we will introduce a Julia package for performing these computations on top of OSCAR and discuss implementation details. This is a joint work with Yue Ren.<br/>



### q-Matroids in Julia/Oscar<br/>
* [Sebastian Degen (Universität Bielefeld, Germany)](https://ekvv.uni-bielefeld.de/pers_publ/publ/PersonDetail.jsp?personId=421945308)<br/>
In combinatorics we can consider the q-analogue as theory of generalizazing from finite sets
to finite dimensional vector spaces. In particular we can view q-matroids as q-analogues of matroids.
In this talk I will present parts of an Oscar based program, written by my advisor Lukas Kühne and me, encoding several aspects of q-matroids.
For this purpose I will first present the definition of a q-matroid in terms of a few cryptomorpic axioms systems, for example base-spaces and independent-spaces as well as the definitions of some basics objects associated to a given q-matroid, like flats, circuits, its dual, its projectivization matroid, etc.
After that I will show how we implemented the aforementioned objects in our program and how they may be generated.
If time permits, I will explain the implementation of the algorithm in an on-going project of my advisor and me, where we try to enumerate all different isomorphism classes of q-matroids in a fixed dimension.<br/>


### Application of dynamic decomposition for tropical prevarieties to celestial mechanics <br/>
* [Anders Nedergaard Jensen (Aarhus University, Denmark)](https://users-math.au.dk/jensen/)<br/>
Every tropical hypersurface is the union of finitely many polyhedra. By the distributive law, intersecting a list of tropical hypersurfaces amounts to doing a huge computation of intersections of polyhedra that may be naturally organised in an enumeration tree. The idea of Dynamic Enumeration proposed by Mizutani, Takeda and Kojima (2007) is extended to Dynamic Decomposition where tropical hypersurfaces are not just chosen dynamically but also split dynamically into disjoint half-open polyhedra. This has the advantage of making the enumeration tree even thinner.
We present an implementation of the this enumeration algorithm in the C++ library gfanlib.
In recent joint work with Anton Leykin this implementation was used to confirm the celebrated generic finiteness result for relative equilibria in the Newtonian 5-body problem by Albouy and Kaloshin (2012) with a five minute computation. <br/>




### Checking regularity on the flip graph of triangulations<br/>
* [Lars Kastner (TU Berlin, Germany)](https://lkastner.github.io/)<br/>
A triangulation of a point configuration is regular if it can be given by a
height function, that is every point gets lifted to a certain height and
projecting the lower convex hull gives the triangulation. Checking regularity of
a triangulation usually is done by solving a linear program. However when
checking many flip-connected triangulations for regularity, one can instead ask
which flips preserve regularity. When traversing the flip graph for enumerating
all regular triangulations, this allows for vast reduction of the linear
programs needing to be solved. At the same time the remaining linear programs
will be much smaller.<br/>


### Singular Matroid Realization Spaces<br/>
* [Dante Luber (TU Berlin, Germany)](https://sites.google.com/view/dantelubermath/home)<br/>
Due to Mnev universality, we know realization spaces of rank 3 matroids can be arbitrarily singular. The proof is constructive, but impractical for obtaining concrete examples. We use software to study a large dataset of matroids, isolating examples of matroids whose realization space is singular. After obtaining such singular spaces, we use them to construct a singular initial degeneration of the Grassmannian.


### Divisors on Metric Graphs<br/>
* [Thomas Saillez (Université libre de Bruxelles, Belgium)](https://www.ulb.be/fr/thomas-saillez-1)<br/>
In tropical geometry, trying to understand divisors on curves gave rise to a
variant of the dollar game named chip firing on metric graphs. In this game, you
put integer values at any point of edges, such configuration is called a divisor,
and you have some rules on how to turn a divisor into other ones.
We will introduce a Matlab Toolbox allowing to do several computations
such as equivalence of divisors, Dhar’s algorithm, Euclidean norm... <br/>


### Cross-ratios and perfect matchings<br/>
* [Rob Silversmith (University of Warwick, UK)](https://sites.google.com/view/rob-silversmith/)<br/>
I’ll discuss a simple combinatorial problem in algebraic geometry, the "cross-ratio degree problem", that turns out to be surprisingly difficult, and to have connections to many areas. I will talk about how to compute cross-ratio degrees, and present a perhaps-surprising upper bound in terms of counting perfect matchings.<br/>


### Quantum Automorphism Groups of Matroids <br/>
   * [Marcel Wack (TU Berlin, Germany)](https://page.math.tu-berlin.de/~wack/)<br/>
Quantum automorphism groups of discrete structures such as graphs have been studied extensively in the last two decades. We define and study quantum automorphism groups of matroids, and describe the primary computational techniques used to generate and study them, namely implementations of free associative algebra and non-commutative Groebner basis algorithms in OSCAR. Finally, we discuss the computational results obtained for the quantum automorphism groups of matroids, as well as the limitations of the algorithms used. Based on joint work with Daniel Corey, Michael Joswig, Julien Schanz and Moritz Weber.<br/>
