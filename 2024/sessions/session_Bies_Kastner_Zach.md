---
layout: session
title: "Classical Algebraic Geometry & Modern Computer Algebra: Innovative Software Design and its Applications"
---
### Organizers
   * [Martin Bies (RPTU Kaiserslautern, Germany)](https://martinbies.github.io/)<br/>
   * [Lars Kastner (TU Berlin, Germany)](https://lkastner.github.io/)<br/>
   * [Matthias Zach (RPTU Kaiserslautern, Germany)](https://github.com/HechtiDerLachs)<br/>

### Aim and Scope

Recent years have shown new applications of symbolic methods in computer algebra at scale. For instance, previously deemed impossible classification algorithms from toric and tropical geometry result in terabyte sized data sets. This calls for the development of new algorithms, allowing --for example-- for parallelization, but also new high level user interfaces. The aim is to bring together experts in computational algebraic geometry and those who want to use newly provided methods and algorithms in their research endeavors. We encourage speakers to highlight the computational aspects of their work and to augment their presentation with code examples. Our focus includes valuable application of these methods in physics, particularly in string theory and F-theory.

## Accepted Talks

   * [Simon Felten](https://simon-felten.github.io/) (Columbia University)
   * [Yang-Hui He](https://www.physics.ox.ac.uk/our-people/he) (London Institute for Mathematical Sciences)
   * [Patrick Jefferson](https://inspirehep.net/authors/1274984) (Massachusetts Institute of Technology)
   * [Chiara Meroni](https://merochia.wixsite.com/chiara-meroni) (ETH Zurich)
   * [Giosuè Muratore](https://sites.google.com/view/giosue-muratore/home-page) (Universidade de Lisboa)
   * [İrem Portakal](https://www.irem-portakal.de/) (Max Planck Institute for Mathematics in the Sciences Leipzig)
   * [Luca Remke](https://www.idsr.uni-stuttgart.de/en/institute/Remke/) (University of Stuttgart)
   * [Andrew P. Turner](https://apturner.net/) (University of Pennsylvania)

## Abstracts

### Computational analysis of logarithmic singularities

#### Simon Felten

In a smooth and proper family of algebraic varieties, the Hodge--de Rham spectral sequence degenerates at the first page, and the Hodge sheaves are locally free. Similarly, in logarithmic geometry, in a proper, log smooth, and saturated family of log schemes, the Hodge--de Rham spectral sequence degenerates at the first page, and the Hodge sheaves are locally free. This is a partial generalization of the classical theorem to degenerations. Filip, Ruddat, and the speaker have achieved a further generalization which applies to degenerations whose logarithmic singularities are toroidal. This generalization has important applications in the construction of new varieties. In an ongoing long-term project, we apply the method to the construction of Fano manifolds in arbitrary dimension. Unfortunately, in its current form, the method is not strong enough to give the desired result. To overcome the current challenges, we have to analyze more general classes of log singularities than toroidal log singularities. Any log singularity which is useful in this context has the following three properties:

 (1) its local deformation theory is under sufficient control to construct globally consistent local deformations,
 (2) a proper family with such log singularities has constant log Betti numbers, and
 (3) the Hodge--de Rham spectral sequence of a proper family with such log singularities degenerates at the first page.

Candidates for such log singularities arise from explicit constructions of singular log schemes. An important approach to establish or refute (1) for an explicit log singularity is via studying the cohomological properties of an explicit resolution of log singularities. To this end, we need to compute the derived direct images of coherent sheaves on the resolution such as the pieces of the log de Rham complex. An important approach to (2) and (3) is to test for the constancy of the log Hodge numbers in explicitly given families with the relevant singularities. Here, we need to compute the derived direct images of the pieces of the log de Rham complex of the family. In this talk, we discuss examples of these two analyses. 


### The AI Mathematician

#### Yang-Hui He

We summarize how AI can approach mathematics in three ways: theorem-proving, conjecture formulation, and language processing.
Inspired by initial experiments in geometry and string theory, we present a number of recent experiments on how various standard machine-learning algorithms can help with pattern detection across disciplines ranging from algebraic geometry to representation theory, to combinatorics, and to number theory. At the heart of the programme is the question how does AI help with mathematical discovery.

### Chebyshev varieties

#### Chiara Meroni

Chebyshev varieties are algebraic varieties parametrized by Chebyshev polynomials or their multivariate generalizations. They play the role of toric varieties in sparse polynomial root finding, when monomials are replaced by Chebyshev polynomials. We will introduce these objects and discuss their main properties, including dimension, degree, singular locus and defining equations, as well as some computational experiments.


### Localization in Gromov--Witten theory of toric varieties in a computer algebra system

#### Giosuè Muratore (Universidade de Lisboa)

Atiyah--Bott localization formula is a powerful tool for calculating the degree of equivariant classes of the moduli space of rational stable maps $\overline{M}_{0,n}(X,\beta)$, where $X$ denotes a smooth toric variety, $n$ is a non negative integer, and $\beta$ is an effective $1$-cycle. Implementation of the formula entails intricate computational challenges, involving graph theory, colorations, partitions, and other discrete objects. Furthermore, the computed solution is a large summation of rational numbers, underscoring the imperative nature of computational efficiency. This formula has been applied in very specific cases for computing Gromov--Witten invariants, addressing enumerative problems, and determining the small quantum ring of $X$, among other applications. 

A comprehensive implementation as a Julia package has been recently presented by the author.We show the features of the package with a particular emphasis to the noteworthy contribution of the package \verb!Oscar.jl!. Finally, we delve into the fundamental prerequisites for extending the implementation to encompass Algebraic GKM Manifolds.


### Algebraic sparse factor analysis

#### İrem Portakal

Factor analysis is a statistical technique that explains correlations
among observed random variables with the help of a smaller number of
unobserved factors. In traditional full factor analysis, each observed
variable is influenced by every factor. However, many applications
exhibit interesting sparsity patterns i.e. each observed variable only
depends on a subset of the factors. We study such sparse factor analysis
models from an algebro-geometric perspective. Under a mild condition on
the sparsity pattern, we compute the dimension of the set of covariance
matrices that corresponds to a given model. Moreover, we study algebraic
relations among the covariances in sparse two-factor models. In
particular, we identify cases in which a Gröbner basis for these
relations can be derived via a 2-delightful term order and joins of
toric edge ideals. The talk will be accompanied with our Macaulay2 code
respecting FAIR principles. This is a joint-work with Mathias Drton,
Alex Grosdos and Nils Sturma. 


### Exceptional sequences of line bundles on toric varieties

#### Luca Remke

We want to investigate whether every maximal exceptional sequence of line bundles is full for a smooth projective toric variety, given the existence of a full exceptional sequence of line bundles. This property has already been proved for toric varieties of Picard ranks 1 and 2. We therefore turn our attention to toric varieties of Picard rank 3, focusing on the del Pezzo surface of degree 7.
