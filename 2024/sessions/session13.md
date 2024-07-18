---
layout: session
title: "ICMS 2024 - Session 13: General Session"
---
### Organizers
   * [Bettina Eick](http://www.iaa.tu-bs.de/beick/)<br/>
   * [Yue Ren](https://yueren.de)<br/>

### Aim and Scope
This session addresses aspects of mathematical software that not covered by the other sessions.

## Schedule

All talks in this session will take place on Tuesday, July 23. The schedule is as follows:

| Time &nbsp; &nbsp; | Title                                                                                                  | Speaker                 |
|--------------------|--------------------------------------------------------------------------------------------------------|-------------------------|
| 9:00 - 10:00       | Plenary Talk                                                                                           |                         |
| 10:00 - 10:30      | Coffee                                                                                                 |                         |
| 10:30 - 11:00      | DetGB: A Software Package for Computing Groebner Bases of Determinantal Ideals                         | Mou, Song, Zhou         |
| 11:00 - 11:30      | Integrating GeoGebra with React and WebAssembly                                                        | Fujimoto                |
| 11:30 - 12:00      | The use of HTML-based dynamic content for the learning of statistical test                             | Kaneko, Kitamoto, Noda  |
| 12:30 - 13:00      | Estimating the Relative Position of Small Multiple Rovers for an Asteroid Wide-area Exploration System | Kasai, Terui, Mikawa    |
| 12:30 - 13:30      | Lunch                                                                                                  |                         |
| 13:30 - 14:00      | Cylindrical Algebraic Decomposition in Macaulay2                                                       | Lee                     |
| 14:00 - 14:30      | Local duality in multi-parameter persistent homology                                                   | Lenzen                  |
| 14:30 - 15:00      | Extrapolating Solution Paths of Polynomial Homotopies towards Singularities with PHCpack and phcpy     | Verschelde, Viswanathan |
| 15:00 - 15:30      |                                                                                                        |                         |
| 15:30 - 16:00      | Coffee                                                                                                 |                         |

## Abstracts

#### Integrating GeoGebra with React and WebAssembly: A Web-Based Approach for Mathematical Software Development
#### [Mitsushi Fujimoto](mailto:fujimoto@fukuoka-edu.ac.jp) (University of Teacher Education Fukuoka, Japan)

A dynamic mathematics software GeoGebra can be embedded on the web, and a
JavaScript API is provided for interaction. By utilizing web platforms, GeoGebra
can collaborate with various web technologies. In this talk, I would like to
introduce a method for creating a GeoGebra-based web app using React for the UI
and WebAssembly for the computational engine.

React is a JavaScript library for creating rich UI components and writing clean
code using JSX. It can detect code errors during the transpilation of JSX to
regular JavaScript. The use of React can address the limitations of GeoGebra's
script input dialog. WebAssembly (Wasm) is a binary format that can run C
functions in web browsers. The web app version of GeoGebra can access external
computational engines created in C language using WebAssembly.

The implementation process includes creating a React component for GeoGebra
using react-geogebra, developing a computational engine in C, converting it to a
Wasm binary with Emscripten, and executing C functions from the React side to
update the UI dynamically.

Some considerations are required for the collaboration between React and
WebAssembly. I will explain the details through the implementation of a
mathematical puzzle, 'Lights Out'. The source code consists of 200 lines of
React code and 100 lines of C code. The web app can be accessed at
https://mitsushi-fujimoto.github.io/geo-lights/


#### The use of HTML-based dynamic content for the learning of statistical test
#### [Masataka Kaneko](mailto:masataka.kaneko@phar.toho-u.ac.jp) (Toho University, Japan)
#### [Takuya Kitamoto](mailto:kitamoto@yamaguchi-u.ac.jp) (Yamaguchi University, Japan)
#### [Takeo Noda](mailto:noda@c.sci.toho-u.ac.jp) (Toho University, Japan)

With the wide-spread availability of high-speed internet,
an HTML-based system is one of the most promising options
for mathematical software in this post COVID-19 era.
While many web-based software libraries are available
for specific purposes, including ones for symbolic calculations
and dynamic visualizations, extra elaboration is needed
to integrate their capabilities so that users can perform
mathematical activities on a single HTML content.

Moreover, it seems that the realities and benefits derived from
the use of those systems have not yet been fully investigated.
Especially in the complex case of statistics learning, more precise
knowledge about them will likely help maximize the effect of
using newly developed systems. This research is mainly concerned
with the use of our newly developed system for the learning
of the $\chi^2$ test for independence.
Through the comparative study of the log of simulations,
which learners performed on the HTML content between
experimental and control groups, it has been shown that
some restrictions to the context of its use can have
a large influence on learners' thinking.


#### Estimating the Relative Position of Small Multiple Rovers for an Asteroid Wide-area Exploration System by Solving Nonlinear Equations
#### Takefumi Kasai (University of Tsukuba)
#### [Akira Terui](https://researchmap.jp/aterui) (University of Tsukuba)
#### [Masahiko Mikawa](https://mikawalab.org/) (University of Tsukuba)

We propose a new method for estimating the relative position of small multiple rovers for an asteroid wide-area exploration system by solving nonlinear equations. A set of small multiple rovers, which are landed and scattered on the ground for asteroid exploration, communicate with each other using radio to estimate their relative position. They use the Received Signal Strength Indicator (RSSI) of the radio received by each rover to estimate each other’s distance and several antennas to estimate each other’s relative directions. According to the mathematical model of the RSSI, one needs to solve a system of nonlinear equations involving rational, trigonometric, and logarithmic functions.

While previous studies used robust but relatively slow Evolutionary Algorithms (EA), we reduce the system of nonlinear equations to a system of linear equations by substituting nonlinear functions as variables, then directly solve it quickly to estimate the relative direction and the distance of a pair of rovers. Furthermore, we combine our proposed method with the least-squares method to estimate the relative positions of more than two rovers and correct the errors. The results of the experiments are shown.


#### Cylindrical Algebraic Decomposition in Macaulay2
#### [Corin Lee](https://people.bath.ac.uk/cel34/) (University of Bath, UK)


We are presenting the first implementation of Cylindrical Algebraic Decomposition (CAD) in Macaulay2, which is the algorithm (and the namesake algebraic object) that can be used to solve real quantifier elimination problems. Our implementation generates an open CAD for a given set of real polynomial expressions with rational coefficients. We are using the relatively newly justified projection/lifting scheme due to Lazard. Moreover, a new heuristic for variable ordering is considered. This work is joint with Tereso del Río and Hamid Rahkooy.


#### Local duality in multi-parameter persistent homology
#### [Fabian Lenzen](mailto:fabian.lenzen@tu-berlin.de) (TU Berlin, Germany)

Persistent homology, a central tool in topological data analysis, computes and analyses the topology of a filtration of topological spaces. The case of 𝐙-indexed filtrations is algebraically simple, and highly efficient implementations are available for this case. Computing the persistent homology of 𝐙ⁿ-indexed filtrations is much more challenging computationally. Specifically, we will consider the problem of computing minimal free resolutions of the persistent homology of 𝐙ⁿ-indexed filtration. Although this can be done in principle with standard Gröbner base methods, these are not fast enough for practical applications; partly because they do not use the specifics of the problem. For the case n = 2, a more specialised algorithm by Lesnick and Wright has been shown to outperform common computer algebra systems. However, this algorithm is still much slower than what is achievable for n = 1, also it is unclear how to generalise it to n > 2. In this talk, I will explain some of the optimisations that are responsible for the efficiency of implementations for n = 1. We will see how these arise as an instance of local duality, and how this can be used to develop a new algorithm for n = 2, and possibly beyond. This algorithm has been implemented in our software 2pac. We explain some non-trivial algorithmic details behind the software, and explain how to apply multi-parameter persistent homology in practice.


#### DetGB: A Software Package for Computing Grobner Bases of Determinantal Ideals
#### [Chenqi Mou](http://www.cmou.net/) (Beihang University, Beijing, China)
#### [Qiuye Song](mailto:qiuye.song@buaa.edu.cn) (Beihang University, Beijing, China)
#### [Yutong Zhou](mailto:zpengyt@buaa.edu.cn) (Beihang University, Beijing, China)

Determinantal ideals are a fundamental concept in commutative algebra and algebraic geometry with deep connections to combinatorics and symbolic computation and have various applications in the MinRank problem from cryptography, Schubert enumerative calculus, and low-rank matrix completion, etc. The software package DetGB we develop is a collection of functions for computing Grobner bases of determinantal ideals and thus facilitates the study, analysis, and visualization of determinantal ideals in a computational way.

The developed package consists of three modules which compute the Grobner bases of normal, (mixed) ladder, and Schubert determinantal ideals respectively and one module with supporting functions like those for the RSK correspondence, the straightening law, and pipe dreams from combinatorics. Two underlying philosophies for our design of the package are: (1) In addition to traditional results on Grobner bases of determinantal ideals, we also want to include the latest development in this direction, like the minimal Grobner bases of Schubert determinantal ideals via elusive minors and our recent algorithm for computing their reduced Grobner bases and the study on the initial ideals of products of determinantal ideals via the RSK correspondence and increasing decomposition. (2) We try to provide as many plotting functions as possible, like those for the ladders of (mixed) ladder determinantal ideals, for the essential sets to construct Fulton generators of Schubert determinantal ideals, and for reduced pipe dreams which are inherently related to the initial ideals of Schubert determinantal ideals.


#### Extrapolating Solution Paths of Polynomial Homotopies towards Singularities with PHCpack and phcpy
#### [Jan Verschelde](https://homepages.math.uic.edu/~jan/) (University of Illinois at Chicago, USA)
#### [Kylash Viswanathan](mailto:kviswa5@uic.edu) (University of Illinois at Chicago, USA)


A robust path tracker computes the radius of convergence of Newton’s method, estimates the distance to the nearest path, and then applies Pade approximants to predict the next point on the path. Apriori step size control is less sensitive to finely tuned tolerances than aposteriori step size control and is therefore robust. Extrapolation methods are effective to accurately locate the singular points at the end of solution paths. Computations are executed with phcpy, the scripting interface to PHCpack, which now compiles with the project manager of the gnu-ada compiler, available via alire (alr), the package manager of Ada. All software is free and open source, released under version 3 of the GNU GPL license. This talk will describe the effectiveness of extrapolation methods.
