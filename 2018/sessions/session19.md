---
layout: default2018
title: "ICMS 2018 - Session 19: Formal and Informal Mathematical Corpora"
---
## Session 19. Formal and Informal Mathematical Corpora

### Organizers

*   [Yihe Dong](mailto:yihed@wolfram.com) (Wolfram Research, Champaign, IL, USA)
*   [Robert Y. Lewis](mailto:rob.y.lewis@gmail.com) (Vrije Universiteit, Amsterdam, NL)

### Aim and Scope

This session aims to connect a constellation of topics related to processing
corpora of mathematical texts. NLP on informal mathematical documents
presents many interesting challenges, and can be aided by the presence of 
corresponding formal documents (interpreted broadly). Creating and maintaining
these corpora presents even more challenges. We hope to bring together
researchers thinking about the retrieval, curation, and interpretation
of formal and informal mathematical texts, as well as the underlying languages
used in these projects and the connections between them. There are many exciting projects 
underway in all of these areas, and a combined session will spur fruitful
discussions and help to align the work of different groups.

#### Topics (including, but not limited to)

* The creation and curation of mathematical corpora (e.g. Hales'
  Formal Abstracts project)
* The parsing and interpreting of natural language mathematics into more
  formal domains (e.g. symbolic or AI techniques for mining and searching the arXiv)
* Target languages for these interpretations and the connections between them
  (e.g. computer algebra systems and proof assistants)

#### Accepted Talks

* *The Lean 3 Mathematical Library*
  
  Mario Carneiro, Carnegie Mellon University

  The Lean 3 "mathlib" library has been rewritten from the ground up to take advantage of the new features and tactics framework. In this article we take stock of the meteoric growth of the library in the past several months, which covers elementary number theory, algebra, ring theory, topology and analysis, set theory, as well as support for verified pure-functional programming with lists, maps, arrays, quotient types, and coinductive types. This is supplemented with additional tactics, written in Lean on top of the Lean 3 tactic framework, for proving arithmetic equalities and inequalities, deciding the equational theory of commutative rings, as well as general automation tactics based on heuristic instantiation and resolution proving.

* *NLP and Large-scale Information Retrieval on Mathematical Texts*

  Yihe Dong, Wolfram Research

  We present a recommender system covering math and math physics papers from the arXiv to date, to assist researchers quickly retrieve theorems and discover similar results from this vast corpus. The retrieval aims to discover not just syntactic, but also semantic similarity. We will discuss the challenges encountered and the experimental methodologies used.

* *Is Univalence Inevitable?*

  [Krzysztof Kapulkin](http://www.math.uwo.ca/faculty/kapulkin/), University of Western Ontario

  Voevodsky's Univalence Axiom (UA) is a major contribution to the area
  of computer formalization of mathematics. It significantly extends
  depended type theory, the underlying system of proof assistants such
  as Coq, Agda, or Lean; for instance, it is known that UA implies the
  principle of Functional Extensionality. In practical terms, it brings
  foundations of mathematics closer to human intuition, providing a
  foundation that justifies common abuses of notation, e.g., writing G=H
  when the groups G and H were only proven to be isomorphic. The use of
  the Univalence Axiom was instrumental in formalization of category
  theory (cf. Ahrens-Kapulkin-Shulman 2015), an area that had previously
  proven particularly ill-suited for formalization.

  This talk will be a survey of Univalence, covering the necessary
  mathematical background, advantages it gives in formalization, and
  predictions for the future. I will also report on the progress in
  developing a new generation of proof assistant, based on cubical type
  theory and created in an attempt to give a computational
  interpretation of the Univalence Axiom.

* *A Bi-directional Extensible Ad Hoc Interface between Lean and Mathematica*

  [Robert Y. Lewis](https://robertylewis.com), Vrije Universiteit Amsterdam

  We implement a user-extensible ad hoc connection between the Lean proof assistant and the computer algebra system Mathematica. By reflecting the syntax of each system in the other and providing a flexible interface for extending translation, our connection allows for the exchange of arbitrary information between the two systems. We show how to make use of the Lean metaprogramming framework to verify certain Mathematica computations, so that the rigor of the proof assistant is not compromised. We also establish a connection in the opposite direction, using Mathematica to import and process proof terms from Lean. This allows one to process and explore the mathematical library of the proof assistant, using the data processing and display tools of the CAS.

* *Set-Theoretic Type Theory*

  [David McAllester](http://ttic.uchicago.edu/~dmcallester/), Toyota Technological Institute at Chicago

  The talk will present a set-theoretic model of dependent type theory handling isomorphism. In this model expressions are given their naive set-theoretic compositional meaning. For example a dependent pair type Sigma x:A B[x] denotes (literally) the set (or class) of pairs (c,d) with c a member of A and d a member of B[c]. This has the consequence that semantic values do not have unique types --- Abelian groups and permutation groups are also (literally) groups as implied by the standard naive set-theoretic definition of a group. Contrasts with homotopy type theory will be discussed from both semantic and proof-theoretic perspectives.


* *Representing Mathematical Formulae in Content MathML using Wikidata*

  [Moritz Schubotz](https://www.moritzschubotz.de/wiki/Main_Page), National Institute of Informatics (Tokyo)

  We represent mathematical formulae in Content MathML
  referring to Wikidata as the knowledge base for the grounding of the
  semantics. By doing so, we link items in the Wikidata knowledge base
  to mathematical identifiers or operators. In contrast to other
  mathematical knowledge bases which define symbols in a deductive
  fashion, the terms in Wikidata emerged inductively from Wikipedia
  articles in different languages. To maximize the interoperability with
  non-strict content MathML, we create a Wikidata based content
  dictionary group.

* *First Experiments with Neural Translation of Informal Mathematics to Formal*

  [Josef Urban](https://www.ciirc.cvut.cz/~urbanjo3/), Czech Technical University

  Abstract TBA.