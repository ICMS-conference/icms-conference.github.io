---
layout: session
title: "ICMS 2024 - Session 2: Novel Formalisations of Mathematics in Lean"
---

### Organizers

* [Amelia Livingston (University College London, UK)](mailto:ucahali@ucl.ac.uk)
* [David Ang (University College London, UK)](mailto:ucahdka@ucl.ac.uk)
* [Fangming Li (Imperial College London, UK)](mailto:fangming.li17@imperial.ac.uk)
* [Jujian Zhang (Imperial College London, UK)](mailto:jujian.zhang19@imperial.ac.uk)

### Aim and Scope

Interactive theorem provers are pieces of software that allow one to express mathematical constructs and arguments and check them interactively. Formalisation, the process of writing mathematical proofs in these systems, is becoming increasingly popular amongst mathematicians. In this session, we will be focusing on the Lean4 theorem prover and exhibit recent novel formalisation projects.

### Schedule

All talks in this session will take place on Thursday, July 25 in MCS3052 at the Department of Mathematical Sciences. The schedule is as follows:

<table>
  <thead>
    <tr>
      <th>Time</th>
      <th>Title</th>
      <th>Speaker</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>09.00 - 10.00</td>
      <td>Plenary talk in MCS0001</td>
      <td></td>
    </tr>
    <tr>
      <td>10.00 - 10.30</td>
      <td>Coffee in front of MCS0001</td>
      <td></td>
    </tr>
    <tr>
      <td>10.30 - 11.00</td>
      <td>Towards a formal proof of the Freyd-Mitchell embedding theorem</td>
      <td>Markus Himmel</td>
    </tr>
    <tr>
      <td>11.00 - 11.30</td>
      <td>Formalising Analysis in Lean: Compactness and Dimensionality</td>
      <td>Dawid Lipinski</td>
    </tr>
    <tr>
      <td>11.30 - 12.00</td>
      <td>Formalising Families of `l`-adic Galois Representations in Lean 4</td>
      <td>Ivan Farabella</td>
    </tr>
    <tr>
      <td>12.00 - 12.30</td>
      <td>Formalisation of the Category of Hopf Algebras in Lean 4</td>
      <td>Yunzhou Xie, Yichen Feng, Yanqiao Zhou</td>
    </tr>
    <tr>
      <td>12.30 - 13.30</td>
      <td>Lunch in front of MCS0001</td>
      <td></td>
    </tr>
    <tr>
      <td>13.30 - 14.00</td>
      <td>Protein folding by recursive backtracking</td>
      <td>Bjørn Kjos-Hanssen</td>
    </tr>
    <tr>
      <td>14.00 - 14.30</td>
      <td>Stacks in Lean</td>
      <td>Calle Sonne, Paul Lezeau</td>
    </tr>
    <tr>
      <td>14.30 - 15.00</td>
      <td>Groups of order `p * q`</td>
      <td>Peiran Wu</td>
    </tr>
    <tr>
      <td>15.00 - 15.30</td>
      <td>Formalization of the Existence of Frobenius Elements</td>
      <td>Jou Glasheen</td>
    </tr>
    <tr>
      <td>15.30 - 16.00</td>
      <td>Coffee in front of MCS0001</td>
      <td></td>
    </tr>
  </tbody>
</table>

### Titles and Abstracts

#### Towards a formal proof of the Freyd-Mitchell embedding theorem

* [Markus Himmel](mailto:markus@himmel-villmar.de)

Lean's mathlib currently provides several tools to facilitate diagram chasing in general abelian categories, but they suffer from deficiencies which make their application less straightforward than simply adapting an elementwise proof in a category of modules.

I will report on an ongoing project to formalize a proof of the Freyd-Mitchell embedding theorem, which states that every small abelian category can be embedded into a category of modules. This theorem vastly strengthens the existing diagram chasing techniques.

The project has several interesting properties: it is being carried out entirely in the form of pull requests to mathlib, with only minimal amounts of code that is not merged at any time. We carefully selected a proof strategy that works well for mathlib, deducing the embedding theorem from various general theories that are useful outside of the embedding theorem. In set-based mathematics, the embedding theorem is accompanied by a "meta-theorem" explaining how the embedding theorem can be applied. I will explain how Lean's universes alleviate the need for such a meta-theorem in the formal setting.

#### Formalising Analysis in Lean: Compactness and Dimensionality

* [Dawid Lipinski](mailto:dawid.lipinski23@imperial.ac.uk)

The theorem that a closed unit ball is compact if, and only if, its vector space is finite-dimensional showcases how unintuitive infinite dimensional spaces can be. Many proofs skip over what's considered obvious, leaving readers unaware of the underlying assumptions until they attempt formalization. We will begin the talk by proving a particular formulation of Riesz's lemma in Lean. We will then use it to construct a sequence in the unit ball where the distance between all elements is 1 and show that such a sequence cannot contain a convergent subsequence. Subsequently, we'll establish that a closed unit ball is not sequentially compact. A significant challenge we encountered during this proof was the necessity to define the sequence through strong recursion, which posed some difficulties in its formalisation. We hope this talk will showcase Lean's role in enhancing understanding and generalization of proofs by prompting us to explore broader definitions and theorems within the Mathlib library.

#### Formalising Families of `l`-adic Galois Representations in Lean 4

* [Ivan Farabella](mailto:ivan.farabella21@imperial.ac.uk)

Families of `l`-adic Galois representations are an important tool in modern algebraic number theory. Andrew Wiles used families of representations associated with elliptic curves to prove Fermat's Last Theorem and the Langlands philosophy conjectures a deep connection to the theory of automorphic forms. We formalise of the definition of families of `l`-adic Galois representations as well as the definition of compatibility on them for the first time in an interactive theorem prover and discuss the formalisation process.

#### Formalisation of the Category of Hopf Algebras in Lean 4

* Speaker: [Yunzhou Xie](mailto:yunzhou.xie21@imperial.ac.uk)
* Speaker: [Yichen Feng](mailto:yichen.feng21@imperial.ac.uk)
* Speaker: [Yanqiao Zhou](mailto:yanqiao.zhou21@imperial.ac.uk)
* [Jujian Zhang](mailto:jujian.zhang19@imperial.ac.uk)

This project delves into the progression of algebraic structures from coalgebra and bialgebra to Hopf algebra, with a special focus on affine group schemes. A key aspect of our study is the group structure that arises from Hopf algebra homomorphisms and the categorization of Hopf algebra, particularly their role within monoidal categories. Additionally, we aim to thoroughly investigate affine group schemes, examining their categorical representation and the implications of their anti-equivalence with commutative Hopf algebra, employing the Lean theorem prover for all formalizations.
<ol>
    <li>Coalgebraic and Bialgebraic Foundations:
        <ol>
            <li>To explore and formalize Coalgebra and Bialgebra within Lean, detailing their foundational properties, homomorphisms, and equivalence relations, setting the stage for the progression to more complex algebraic structures.</li>
            <li>This exploration naturally extends to Hopf algebra, illustrating the seamless progression within the algebraic hierarchy from coalgebra and Bialgebra to Hopf algebra.</li>
        </ol>
    </li>
    <li>Group Structure in Hopf Algebra Homomorphisms:
        <ol>
            <li>To rigorously investigate the group structure that emerges from algebra homomorphisms between Hopf algebra and algebra, emphasizing its pivotal role in algebraic studies.</li>
            <li>To formalize the conditions that allow these homomorphisms to form a group, particularly focusing on the existence of inverses and the identity element.</li>
        </ol>
    </li>
    <li>Formalization and Extension of Hopf Algebra Categorization:
        <ol>
            <li>To initiate the categorization of Hopf algebra in Lean, focusing on the defining categorical structures, objects, and morphisms, and their intrinsic properties.</li>
            <li>To extend this categorization, illustrating how Hopf Algebra Category evolves into a monoidal category.</li>
        </ol>
    </li>
    <li>Exploration of Affine Group Schemes and Their Anti-Equivalence:
        <ol>
            <li>To articulate the sophisticated representation of affine group schemes through corepresentable functors and the application of group axioms, setting the foundation for their algebraic and categorical analysis.</li>
            <li>To conclusively demonstrate the anti-equivalence between the category of affine group schemes and the category of commutative Hopf algebra, showcasing the culmination of this algebraic exploration and its implications for the broader mathematical landscape.</li>
        </ol>
    </li>
</ol>

#### Protein folding by recursive backtracking

* [Bjørn Kjos-Hanssen](mailto:bjoernkh@hawaii.edu)

The hydrophobic-polar (HP) protein folding model was introduced by Ken A. Gill in 1985. It attracted a great deal of attention, at least until the advent of Google's AlphaFold in 2018.

In this model, a binary string like 0110 is interpreted as a polymer, a sequence HPPH of amino acids of two types. The string is embedded in an ambient space, and this embedding is called a fold. Some folds are better than others and this is quantified by the score of the fold.

In this project I formalize basic definitions and facts for the HP model in such a way that Lean can automatically calculate optimal scores. To speed up the calculation I use recursive backtracking. For good measure, I prove in Lean that my implementation of recursive backtracking and its application are correct.

A critical issue when formalizing the HP model seems to be the choice of definition for the path induced by a sequence of folding moves (like up, down, left, right). I will present a couple of approaches used with varying success.

#### Stacks in Lean

* Speaker: [Calle Sonne](mailto:calle.sonne.23@ucl.ac.uk)
* Speaker: [Paul Lezeau](mailto:paul.lezeau.23@ucl.ac.uk)

In this talk, we plan to explain some of our work that has led to defining Stacks in Lean. We will introduce some of the basic mathematical theory around this topic (categories fibered in groupoids, etc) and explain the various challenges that arise when formalising this. Finally, we will discuss our more recent efforts to redefine these notions using structures and data types that are more adapted to Lean, and advertise our upcoming project to use this work as a basis to formalize some basic deformation theory (Schlessinger's criterion, etc) for Kevin Buzzard's FLT project.

#### Groups of order `p * q`

* [Peiran Wu](mailto:pw72@st-andrews.ac.uk)

We formalise in Lean a proof that any finite group of order `p q` with `p` and `q` distinct prime numbers is isomorphic to the semidirect product of a cyclic group of order `p` and one of order `q`. We apply the result to classify groups of certain small orders in Lean. Joint work with Scott Harper.

#### Formalization of the Existence of Frobenius Elements

* [Jou Glasheen](mailto:jou.glasheen23@imperial.ac.uk)

I will present a formalization in Lean 4 of `exists_frobenius`, a proof of the existence of the Frobenius element for finite Galois extensions `L / K` of number fields. This formalization constitutes some of the groundwork for Kevin Buzzard's project to formalize the proof of Fermat's Last Theorem. In terms of methodology, I will highlight the following components of `exists_frobenius`:
<ol>
    <li>firstly, application of the `A K L B` setup to:
        <ol>
            <li>define a finite extension `L / K` of number fields, with `B`, `A` respective rings of integers;</li>
            <li>construct the transitive action of the Galois group `L ≃a[K] L` on the set of non-zero prime ideals which lie above a certain non-zero prime ideal `P ⊂ A`;</li>
            <li>define the decomposition subgroup of a nonzero prime ideal `Q` lying over `P`; and</li>
            <li>in combination with the orbit-stabilizer and Chinese remainder theorems, to characterize the orbit of `Q` under the action of `L ≃a[K] L`;</li>
        </ol>
    </li>
    <li>secondly, synthesis of the characteristic, exponential characteristic, and Frobenius endomorphism of finite fields; the Galois correspondence; and integrality; to show that a polynomial `(F : B[X])` which is a product of linear factors `(X - C (galRestrict A K L B τ α))`, `(τ : L ≃a[K] L)`, `(α : B)` algebraic over K; has coefficients in A, the ring of integers of the base field of the extension.</li>
</ol>
