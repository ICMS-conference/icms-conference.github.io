---
layout: session
title: "ICMS 2024 - Session 10: Mathematical research data"
---
### Organizers
   * [Jeroen Hanselman (RPTU Kaiserslautern, Germany)](https://hanselmanj.eu/)<br/>

### Aim and Scope

Computers have allowed mathematicians to do things that used to be practically impossible. Huge databases, complicated computer algebra packages, proof assistants and more and more computational tools have become crucial for doing mathematics.

This session aims to provide a mix of two important aspects of mathematical research data: The data itself and how to treat the data correctly. 

**Databases:**
The main topic of mathematical research data is of course, the data itself. The session will therefore show off various existing databases. Producing data for databases, the difficulties of managing a database, discussing off the newest features of existing databases are all possible topics speakers could talk about. 

**FAIR data:**
As research data becomes more important, we need to start thinking about how to handle the data. For this, it is useful to talk about the concept of FAIR data. FAIR is short for Findable, Accessible, Interoperable and Reusable. In short, we want to talk about measures we can take to ensure that other mathematicians have access to the work we did and are actually able to reproduce our results and reuse them. It happens far too often that data that was produced, say, two years ago can no longer be used for a variety of potential reasons. The session will also concern itself solutions to can help addressing the current state of affairs.

## Schedule

All talks in this session will take place on Wednesday, July 24. The schedule is as follows:

| Time &nbsp; &nbsp; | Title | Speaker |
| -------- | -------- | -------- |
| 9.00 - 10.00 | Plenary Talk |
| 10.00 - 10.30 | Coffee | 
| 10.30 - 11.00 | [Data related to the Atlas of Finite Groups](https://raw.githubusercontent.com/JHanselman/icms-conference.github.io/master/2024/sessions/Talks-Session10/Breuer.pdf) | Breuer |
| 11.00 - 11.30 | The Graded Ring Database | Brown |
| 11.30 - 12.00 | MaRDI Packaging System, a solution for predefined software environments | Kaushik |
| 12.30 - 13.00 | Towards a FAIR Documentation of Workflows and Models in Applied Mathematics | Reidelbach |
| 12.30 - 13.30 | Lunch | |
| 13.30 - 14.00 | [polyDB: An open database for combinatorial and geometric data](https://raw.githubusercontent.com/JHanselman/icms-conference.github.io/master/2024/sessions/Talks-Session10/Paffenholz.pdf) | Paffenholz |
| 14.00 - 14.30 | [Managing Data in the L-functions and Modular Forms Database (LMFDB)](https://raw.githubusercontent.com/JHanselman/icms-conference.github.io/master/2024/sessions/Talks-Session10/Paulhus.pdf) | Paulhus |
| 14.30 - 15.00 | A FAIR File Format for Mathematical Software | Della Vecchia |
| 15.00 - 15.30 | [Peer reviewing software in Mathematical papers](https://raw.githubusercontent.com/JHanselman/icms-conference.github.io/master/2024/sessions/Talks-Session10/Hanselman.pdf)| Hanselman |
| 15.30 - 16.00 | Coffee | 
| 16.00 - 16.30 | How to share large data in mathematics? | Schröter |
| 16.30 - 17.00 | Integrating Mathematical Data and Resources: Advancements in zbMATH Open| Azzouz-Thuderoz |
| 17.00 - 17.30 | Addressing Centralization Concerns in Software Development | Azzouz-Thuderoz |

#### Data related to the Atlas of Finite Groups
#### Thomas Breuer (RWTH Aachen, Germany)
A lot of information from the Atlas of Finite Groups
is available in electronic form,
and using these data in computations often leads to new information.

It is valuable to store such extensions --about larger groups or new aspects
or both-- in such a way that they can be used together inside one computer algebra system.
Usually the available data are incomplete, and the open questions get answered incrementally.
Keeping the data consistent is a challenge.

The talk will discuss several data libraries that are available in the systems GAP and Oscar.



#### Towards a FAIR Documentation of Workflows and Models in Applied Mathematics
#### Marco Reidelbach (ZIB Berlin, Germany)

The Mathematical Research Data Initiative (MaRDI) has developed a FAIR and machine-interpretable template for documenting Model-Simulation-Optimization workflows in applied mathematics. It captures the mathematical models utilized and individual process steps, detailing methods, software, hardware, input, and output data to address specific research objectives. To enable scientists across disciplines to document and publish their workflows on the MaRDI Portal, we introduce the MaRDMO Plugin for the Research Data Management Organiser, the most widely used Data Management Planning software in Germany. MaRDMO facilitates the workflow documentation semi-automatically, fetching additional information from sources like Wikidata, swMath, zbMath or the MaRDI Portal. Central to these workflows are mathematical models, necessitating proper documentation, for which MaRDI has developed the MathModDB ontology to capture the research fields and problems, formulations, quantities, and tasks associated with the model. Here we present the interaction of MaRDMO and MathModDB Knowledge Graph using a "Logical Data Analysis" workflow from the digital humanities.


#### The Graded Ring Database
#### Gavin Brown (University of Warwick, United Kingdom)

The Graded Ring Database (GRDB) holds data related to the rings of functions of geometrical objects.
The main focus is on classification questions in algebraic geometry where the key objects are often graded polynomial rings and their quotients. The GRDB houses several complete classifications of different types of objects, but the main focus is on a list of Hilbert series (the generating functions for dimensions of graded pieces) of Fano 3-folds, which continue to be at the cutting edge of birational geometry and far from fully classified even after 50 years of intensive study and two Fields medals. In fact, this list is not a classification: it is a list of partial data for potential candidates to be Fano 3-folds, and as such some members of the list will not exist while others may exist in multiple ways yet to be discovered - that is the classification problem in a nutshell. Despite the subtlety of these flaws, the list, presented as a map of Fano 3-folds, complete with unexplored regions, has proved remarkably valuable to ongoing work and is cited by users across a range of different geometrical applications. I will describe the GRDB, its main aims, and the way it interacts with other databases to make progress.


#### A FAIR File Format for Mathematical Software
#### Antony Della Vecchia (TU Berlin, Germany)

We describe a generic JSON based file format which is suitable for computations in computer algebra. This is
implemented in the computer algebra system OSCAR, but we also indicate how it can be used in a different context.



#### polyDB: An open database for combinatorial and geometric data
#### Andreas Paffenholz (TU Darmstadt, Germany)

polyDB (polydb.org) is an open database for combinatorial and geometric objects. The project started in 2015 as an extension for the computer algebra system polymake (polymake.org). Though it still has close ties with the polymake project, the database aims to be a general storage option for mathematical research data, independent of any particular software.

All data objects in polyDB are stored as JSON documents, grouped into collections. The structure of each data item in a collection is fixed by a JSON schema. The schema provides a description of the data in a collection and specifies its format. It allows to reconstruct the datatypes of all fields. This serialization format has originally been designed for polymake. polyDB aims to satisfy the FAIR principles for accessibility and reusability of the data. Data from polyDB can be searched and obtained via a REST interface, but there are also tailored interfaces for the software systems polymake and OSCAR, and basic interfaces for python and Julia.

In my talk I will discuss the background and general design of polyDB, explain the data model used, and show some further directions for development. I will also present examples how the data can be accessed using the various interfaces.


#### Managing Data in the L-functions and Modular Forms Database (LMFDB)
#### Jennifer Paulhus (Grinnell College, USA)

The L-functions and Modular Forms Database (LMFDB) is a mature, massive online database of mathematical objects from number theory and arithmetic geometry. It was primarily conceived to help find connections between objects which are part of the Langlands program, but it has also branched out to other related mathematical objects, including a new database of half a million finite groups, and a quarter of a billion of their subgroups. In the years of developing LMFDB, we've learned many lessons about creating mathematical databases including how to present data to an average user, how to design advanced searches and download features for users with more specialized interests, and how to test for reliability and correctness of the data. This talk will focus on those lessons, using the new database of finite groups as a lens through which to tell this story.



#### MaRDI Packaging System, a solution for predefined software environments
#### Aaruni Kaushik (RPTU Kaiserslautern-Landau, Germany)

We have developed a way to enshrine a software package into an easy to deploy and use sandbox environment we call a "runtime", via a program we developed called MaPS : MaRDI Packaging System. The program relies on Linux user namespaces to isolate a library environment from the host system, making the sandboxed software reproducible on other systems, with minimal effort, and an overlay filesystem to make local edits persistent. This project will aid reproducibility efforts of research papers: both mathematical and from other disciplines. As a proof of concept, we already provide runtimes for the OSCAR Computer Algebra System, polymake software for research in polyhedral geometry, and VIBRANT Virus Identification By iteRative ANnoTation. The software is in a pre release state: the interface for creating, deploying, and executing runtimes is final, and an interface for easily publishing runtimes is under active development.

#### Peer reviewing software in Mathematical papers
#### Jeroen Hanselman (RPTU Kaiserslautern, Germany)

The advent of computers has allowed mathematicians to do increasingly more difficult computations that used to be practically impossible. We now have databases of mathematical objects of multiple Terabytes in size, huge computer algebra packages, proof assistants and many more computational tools to help us do mathematics.

But, despite the usefulness of computation in mathematics, it rarely gets used correctly. Mathematicians have spent decades refining the way one should write down mathematics, but, all of this rigor seems to be thrown out of the window as soon as a paper relies on a computational part. As a consequence, there are most assuredly papers floating around that contain proofs relying on source code that no one can run. Which essentially means that these results come without a proof.

It is crucial that we start thinking of guidelines and general practices that improve the reproducibility of our code. One way to help with this is to introduce a software peer reviewing process. In this talk I will talk about the importance of software peer reviewing and my experiences I had while doing this.


#### How to share large data in mathematics?
#### Benjamin Schröter (KTH Royal Institute of Technology, Sweden)

I will present two examples of large data collections that are relevant in my own research.
Namely, the tropical Grassmanniann $TGr_0(3,8)$ which is a fairly large fan wich can be equipped with various polyheadral structures and the `polyDB' database which has many collections of data, including for example polyhedral and matroidal data.

I will very briefly discuss the relevance of the particular data from my perspective, but the focus will lie on the following general questions and problems:

- How to verify the data?
- How to update, extend or modify data?
- How to make the data accessible and useable for other users?

The goal of this talk is to start an discussion within the community about the handling of data in the long run.

#### Integrating Mathematical Data and Resources: Advancements in zbMATH Open for Enhanced Mathematical Research Accessibility and Reproducibility
#### Maxence Azzouz-Thuderoz (FIZ Karlsruhe, Germany)

zbMATH Open is emerging as a unified platform offering a spectrum of mathematical resources comprising mathematical software, formulae, reviews, and serial and mathematical item classification.
zbMATH Open offers connection to external partners, DLMF and OEIS, via its Links API by indexing approximately 6330 documents containing 65,069 references to OEIS sequences and 15,858 references to 2053 DLMF functions. Significantly, the collection of 44,594 software entries from swMATH is entirely accessible through zbMATH Open. Here, we emphasize the accurate referencing of mathematical software in swMATH for maintaining integrity, advancing mathematical research, and enhancing reproducibility. We intend to report the ongoing efforts of swMATH, an integral part of zbMATH Open, to collect precise referencing software metadata. We describe how swMATH is embedded into zbMATH open and elaborate on the relationship of software and other mathematical research data like OEIS and DLMF, ensuring a complete and FAIR resource for the mathematical research community.

#### Addressing Centralization Concerns in Software Development: Towards a Decentralized Version Control System
#### Maxence Azzouz-Thuderoz (FIZ Karlsruhe, Germany)

The software development domain has seen scholars' growing reliance on platforms like Github, raising issues regarding monopolization. Such centralized platforms raise concerns about data sovereignty and long-term viability. Moreover, a discrepancy in the resilience of the internet infrastructure could affect the proper functioning of a centralized forge. We explore the potential of a decentralized Version Control System (VCS) tailored to academic needs. We investigate the first prototypes of Interplanetary File System-based services for VCSs.

