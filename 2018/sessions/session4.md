---
layout: default2018
title: "ICMS 2018 - Session 4: Polyhedral methods in geometry and optimization"
---
## Session 4. Polyhedral methods in geometry and optimization

### Organizers

*   [Michael Joswig](mailto:joswig@math.tu-berlin.de) (Institut für Mathematik der Technischen Universität Berlin)
*   [Yue Ren](mailto:yueren@mis.mpg.de) (Max-Planck-Institut für Mathematik in den Naturwissenschaften)

### Aim and Scope

Convex polyhedra occur in optimization as the feasible regions of linear programs.
Moreover, integer linear programming is the same as linear programming over the
convex hull of the lattice points in a polyhedron.
In algebraic geometry and its applications piecewise-linear shapes occur in the
guise of polyhedral fans.
Examples include secondary and Groebner fans, which play major roles, e.g., in
tropical geometry.
This session wants to bring together people working on algorithms and software
dealing with any of the above.


### Topics

Specific topics include, but are not restricted to, the following:
*    convex hull computations
*    mixed integer linear programming
*    explicit methods for triangulating point configurations
*    computations in toric or tropical geometry
*    parallelization of polyhedral computations
*    polyhedral methods in algebraic statistics
*    algorithms exploiting symmetry in any of the above


#### Accepted Talks

* *First steps in the formalization of convex polyhedra in Coq*

  Xavier Allamigeon, INRIA and Ecole Polytechnique

  We present the foundations of our project "Coq-Polyhedra" aiming at formalizing convex polyhedra in the proof assistant Coq. The originality of our approach lies in the fact that our formalization is carried out in an effective way, in the sense that the basic predicates over polyhedra (emptiness, boundedness, membership, etc) are defined by means of Coq programs. All these predicates are then proven to correspond to the usual logical statements. To this end, we make an extensive use of the Boolean reflection methodology which was developed in the proof of Feit-Thompson Theorem by Gonthier et al. Our effective approach allows to overcome the intuitionistic nature of the logic used by Coq, and is made possible by implementing the simplex method (Phase I and Phase II) inside the proof assistant. Termination is proved by using the lexicographic pivot rule of Dantzig et al. In this way, we easily arrive at the proof of important results on polyhedra, such as several versions of Farkas Lemma, duality theorem of linear programming, separation from convex hulls, Minkowski Theorem, etc. We finally report on recent progress on the formalization of faces. This is joint work with Ricardo D. Katz (CIFASIS-CONICET, Argentina).


* *Counting lattice points in lattice polytopes*

  Ben Braun, University of Kentucky

  To determine the Ehrhart series of an arbitrary lattice polytope P, i.e. to determine the number of lattice points in integer dilates of P, Barvinok's algorithm is a wonderful tool for computational experiments. However, the dimensions for which these computations can be done are limited. I will discuss an alternative method for computing Ehrhart series of a special family of high-dimensional lattice polytopes, and mention recent work that is based on computational experiments for this family using SageMath.


* *Numerical Software for Computing Newton Polytopes*

  Taylor Brysiewicz, Texas A&M University

  We present our implementation of an algorithm which functions as a numerical oracle for the Newton polytope of a hypersurface in the Macaulay2 package NumericalNP.m2. To showcase this software, we investigate the Newton polytope of both a hypersurface coming from algebraic vision and the classical Lüroth invariant.


* *Investigating Chvatal's conjecture using exact SCIP and VIPR.*

  Leon Eiffler, Zuse Intitute Berlin

  Chvatal's conjecture in extremal combinatorics states a property of decreasing families over a finite ground set. The claim is that among the maximal sized intersecting subfamilies, there always exists a star.  We formulate a MIP that is equivalent to the correctness of the conjecture in the sense that the MIP is infeasible if and only if the conjecture holds. Floating point MIP solvers are unfit to solve such a problem, as the use of tolerances and inexact data cannot result in a certain proof. To overcome this problem, the exact variant of the solver SCIP uses a combination of exact rational arithmetic and safe dual bounding methods for floating point arithmetic. However, the possibility of algorithmic or programming errors remains. To increase confidence in the correctness of computational proofs, we use text-based certificates that are automatically generated during the solving process. The VIPR certificate format presents a possibility to verify results of branch-and-cut solvers externally, using simple inference rules that can be checked independently of the solver.


* *Enumerating triangulations of cyclic polytopes*

  Michael Joswig and Lars Kastner, TU Berlin

  We report on a case study for enumerating triangulations of a given point set with the new software mptopcom (co-authored with Skip Jordan).  Especially, we focus on the triangulations of cyclic polytopes.  These are particularly interesting due to their connections with higher Stasheff-Tamari orders, cluster algebras and related combinatorial, algebraic and topological structures.


* *Tropical Principal Component Analysis and its Applications to Phylogenetics*

  Qiwen Kang and Ruriko Yoshida, University of Kentucky

  Principal component analysis is a widely-used method for the dimensionality reduction of a given data set in a high-dimensional Euclidean space. Here we define and analyze two analogues of principal component analysis in the setting of tropical geometry. In one approach, we study the Stiefel tropical linear space of fixed dimension closest to the data points in the tropical projective torus; in the other approach, we consider the tropical polytope with a fixed number of vertices closest to the data points. We then give approximative algorithms for both approaches and apply them to phylogenetics, testing the methods on simulated phylogenetic data and on an empirical dataset of Apicomplexa genomes.


* *Tropicalized quartic curves of genus 3*

  Yue Ren, Max Planck Institute MIS Leipzig

  Tropical geometry is commonly described as a combinatorical shadow of algebraic geomtry: under good conditions, many geometric properties of an algebraic variety are preserved in its tropicalization, under bad conditions, all information is lost. In this talk, we will study tropicalizations of quartic curves of genus 3 from all possible angles. We will put special emphasis on the mathematical software that were employed and their contributions to the results that were obtained. This is joint work with Marvin Hahn, Hannah Markwig and Ilya Tyomkin.


* *Computing tropical prevarieties*

  Jeff Sommars, University of Illinois at Chicago

  The computation of the tropical prevariety is the first step in the application of polyhedral methods to finding positive dimensional solution sets of polynomial systems. I’ll describe several algorithms that can be used to compute tropical prevarieties and also present a related software package. I'll conclude by reporting on several computational results, including the first computation of the tropical prevariety of the cyclic 16-roots problem.