---
layout: session
title: "ICMS 2024 - Session 1: Number theory and related areas"
---
### Organizers
   * [John Abbott (RPTU Kaiserslautern, Germany)](mailto:john:abbott@rptu.de) but replace the colon by a dot<br/>

### Aim and Scope
Number theory underlies many techniques for symbolic computation, and also in several neighbouring disciplines such as modern cryptography & cryptanalysis.  In this session we shall see and discuss various state-of-the-art implementations as well as bring together researchers with varied applications and using different software systems. Topics may include, but are not limited to, certificates of correctness of computational results (e.g. primality certification), algebraic field extensions, local fields, arithmetic geometry.  Details about important implementation techniques are also encouraged (e.g. exploiting parallellism, new empirically-confirmed complexity results, adroit use of approximation).

### Schedule
All talks in this session will take place in MCS3052 on Thursday afternoon (25th July) at the Department of Mathematical Sciences.  The schedule is as follows:
| Time | Title | Speaker |
| ---- | ----- | ------- |
| 16:00--16:30 | ECPP over MPI | A. Enge |
| 16:30--17:00 | Determinants over ZZ | J. Abbott |
| 17:00--17:30 | A weakness in GSW Encryption | A. Kaushik |

Each 30 minute slot comprises approx 23 mins presentation, 5 mins questions, 2 mins changeover

  ---
  
## Accepted Talks

Title:  **ECPP over MPI**

Speaker: *Andreas ENGE*

The *FastECPP* algorithm is currently the fastest approach to prove the
primality of general numbers, and has the additional benefit of creating
certificates that can be checked independently and with a lower complexity.
It crucially relies on the explicit construction of elliptic curves with
complex multiplication, to which I have contributed over the last two
decades.

I will present the FastECPP implementation in my [CM code](https://www.multiprecision.org/cm/ecpp.html)
which has pushed the record for the largest ECPP certified prime from
49000 digits in 2022 to 86000 digits in 2023, and which is available under
a free license.  I will explain how the possibilities and the limits of
massive parallelisation have informed the algorithmic choices made in the
code.  Looking at the wall-clock time complexity when the number of cores
tends to infinity shows where the practical limits of the algorithm lie
to certify larger numbers.

---

Title: **A weakness in GSW Encryption**

Speaker: *Aaruni KAUSHIK*

In this talk, we look at the **Fully Homomorphic Encryption** system proposed by
*Craig Gentry, Amit Sahai, and Brent Waters* in 2013.  We present a restated version
of the proposed cryptosystem, and then try to look at the ciphertexts resulting from
the use of this system, to try to find patterns in them.  For this task, we train a
machine learning pipeline, utilizing *Topological Data Analysis.*  We show that, even
for supposedly secure parameters, this machine learning approach can simply guess what
the plain text should have been in a majority of cases (accuracy > 70%), in very good
time complexity (< O(n^3)).  However, this attack was ineffective against the
*Shortest Vector Problem (SVP)*, the base problem upon which the encryption is based.
This hints at a possible flaw somewhere in the reduction from SVP (via Gap-SVP and LWE) to the cryptosystem.

---
Title: **Determinants over ZZ**

Speaker: *John ABBOTT*

The computation of the determinant of an integer matrix is a well-studied problem.
We present some practical improvements over the current, best, practical algorithm.
Our method achieves better complexity on a specific class of matrices; it is
implemented in the [OSCAR system](https://www.oscar-system.org).  Joint work with
*Claus FIEKER*.
