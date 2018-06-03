---
layout: default2018
title: "ICMS 2018 - Session 14: Towards Composable Mathematical Software"
---
## Session14. Towards Composable Mathematical Software

### Organizers

*   [Markus Pfeiffer](mailto:markus.pfeiffer@st-andrews.ac.uk) (School of Computer Science, St Andrews, UK)
*   [Florian Rabe](mailto:f.rabe@jacobs-university.de) (Jacobs University, Bremen, Germany)
*   [Nicolas Thiéry](mailto:Nicolas.Thiery@u-psud.fr) (Université Paris Sud, France)


### Aim and Scope

There is a wealth of mathematical software available today, most of which are
  free and open-source, but very specialised: for example nauty for graph
  isomorphism, Singular for polynomials, Pari for number theory. Additionally
  there are databases of objects like the OEIS, or the Small Group Library.
  
  In contemporary mathematics research, we use and combine these specialised
  tools, which requires domain-specific knowledge, data access and conversion,
  and low-level programming for interfacing between them.

  This is tedious, error-prone, and does not scale: Addressing the demand for
  better composability there are huge software packages like SageMath, data
  description languages like OpenMath, and RPC mechanisms like SCSCP.

  The aim of this session is to provide a forum for developers and users of
  mathematical software with an interest in composablity and interoperability of,
  and knowledge and data exchange between systems, to share experiences, solutions,
  and a vision for the future.

## Accepted Talks

### Integrating GAP and Julia - JuliaInterface and Gap.jl (Sebastian Gutsche, University of Siegen)

OSCAR (Open Source Computer Algebra Resource) is a new project to build a
visionary computer algebra system integrating GAP, Singular, polymake, and Antic
by using the Julia programming language.

The GAP package JuliaInterface and the Julia package Gap.jl provide the
low-level part of integrating GAP and Julia. They combine several features,
including
* accessing all functionality in Julia from GAP,
* accessing all functionality in GAP from Julia,
* and conversion of basic types between GAP and Julia.

Unlike interfaces, the integration aims providing compatibility at the lowest
level, trying to make the wall separating the two systems as low as possible. To
achieve this, several technical difficulties had to be tackled, of which some
will be presented in the talk.

Together with the integration of Singular and polymake into Julia (also part of
the OSCAR project), JuliaInterface and Gap.jl will be used to provide
integration of GAP with Singular and polymake.

Because of the low penalty when switching between the GAP and the Julia layer,
this integration enables one to write algorithms combining the computational
power of all four systems.

In this regard, JuliaInterface will be used to replace incomplete interface from
GAP to polymake and the outdated interface from GAP to Singular, using as few
binding code as possible to transparently access all foreign functionality.

Furthermore, the highly efficient integration of Julia into GAP allows one to
implement fast versions of algorithms for GAP in Julia instead of C.

This is joint work with Thomas Breuer.

### SageMath: an approach to unifying open source mathematical software (William Stein, SageMath Inc)

In 2004, I started the Sage software project to create, for me,
a viable alternative to Magma for my number theory teaching and research.
It has grown much larger in scope and contributors over the last 14 years.
I will describe the motivation behind Sage, what technology has come out of
the project over the years (such as Cython and web-based code notebook
interfaces), and where Sage might go when we have the resources that we need.

### Composing Mathematical Software Systems via the Math-in-the-Middle Paradigm (Michael Kohlhase, University of Erlangen)

There is a large ecosystem of mathematical software systems. Individually, these
are optimized for particular domains and functionalities, and together they
cover many needs of practical and theoretical mathematics. However, each system
specializes on one particular area, and it remains very difficult to solve
problems that need to involve multiple systems. Some integrations exist, but the
are ad-hoc and have scalability and maintainability issues. In particular, there
is not yet an interoperability layer that combines the various systems into a
virtual research environment (VRE) for mathematics.
  
The OpenDreamKit project aims at building a toolkit for such VREs. It suggests
using a central system-agnostic formalization of mathematics
(Math-in-the-Middle, MitM) as the needed interoperability layer. In this talk,
we report on a case study that instantiates the MitM paradigm the systems GAP,
Sage, LMFDB and Singular to perform computation in group and ring theory.
  
Our work involves massive practical efforts, including a novel formalization of
computational group theory, improvements to the involved software systems, and a
novel mediating system that sits at the center of a star-shaped integration
layout between mathematical software systems.

### Proving Axiom Sane (Tim Daly,)

In Computational Mathematics, Computer Algebra and Proof systems have grown up
in parallel with little crossover. Two approaches seem to dominate their
combination. There have been efforts to prove individual algorithms, such as
Groebner Basis, inside a Proof system. There have been efforts to communicate
between systems where the Computer Algebra system is used as an untrusted Oracle
for the Proof system. Could the Computer Algebra system be made trustworthy?

Typeclasses have three components: Signatures, Carriers, and Propositions. Axiom
assigns Signatures through its "Category" hierarchy. It assigns Carriers, known
as the Representation through its "Domain". This partition defines an API but
allows multiple representations such as sparse and dense polynomials.

The missing component is Propositions. This research effort associates
Propositions with both the Category and Domain components. The goal is to
collect both Category-level and Domain-level Propositions and use them to prove
algorithms 'in-situ'. In Axiom, GCD occurs in 22 different Domains, each of
which has different Propositions available. In addition, the collected
Propositions define properties for user-level operations, e.g. commutitivity.

Algorithms proven correct would allow Axiom to be a Trusted Oracle.
