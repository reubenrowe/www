---
layout: page
permalink: /research/
title: Research
---

My research interests include (but are not limited to) the following topics.

- Formal verification
- Refactoring and program synthesis
- Semantics
- Logic and proof theory
- Inductive and coinductive reasoning
- Metaprogramming and intensional computation
- Type systems and computational models

Some things I have worked on include the following.
See my
  [publications]({{ '/publications/' | prepend:site.baseurl | prepend:site.url }})
    and
  [software]({{ '/software/' | prepend:site.baseurl | prepend:site.url }})
pages for more details.

#### Trustworthy Refactoring for OCaml

Whilst at the University of Kent, I worked on the
  '[Trustworthy Refactoring](https://www.cs.kent.ac.uk/projects/trustworthy-refactoring/)'
  project (EPSRC Grant [EP/N028759/1](http://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/N028759/1))
with
[Simon Thompson](https://www.cs.kent.ac.uk/people/staff/sjt/),
[Scott Owens](https://www.cs.kent.ac.uk/people/staff/sao/),
and [Hugo Férée](https://hugo.feree.fr/).
The aim of this project was to develop a framework in which refactorings for the
OCaml programming language can be formally specified, and verified to be
behaviour preserving.
We developed a prototype tool called
  [ROTOR](https://trustworthy-refactoring.gitlab.io/refactorer/),
and an abstract static [semantics](https://doi.org/10.1145/3314221.3314600)
for a subset of OCaml that formalises our approach.

#### Cyclic Proof and Program Verification

I work on aspects of proof theory, specifically a notion of proof which allows
derivations of infinite height but with a well-formedness condition that
guarantees soundness. This essentially encodes forms of inductive reasoning.
A natural finite representation of infinite proofs is using finite derivation
trees with cycles, hence the term "cyclic" proof. I have investigated the
theory of non-wellfounded and cyclic proofs in different contexts, including
  [first order logic](https://doi.org/10.4230/LIPIcs.CSL.2018.17),
  [Herbrand logics](https://doi.org/10.1093/logcom/exz011),
  and [modal logics](https://doi.org/10.1007/978-3-030-29026-9_19).

I worked with
  [James Brotherston](http://www0.cs.ucl.ac.uk/staff/J.Brotherston/)
at University College London on investigating how to expand verification
techniques making use of separation logic and cyclic proofs.
This project (funded by EPSRC Grant [EP/K040049/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/K040049/1))
focused on the development of the
  [Cyclist](https://www.cyclist-prover.org/)
theorem proving framework. My work in particular added capabilities for proving
termination of procedural code with recursion.

#### Abductive Programming for Machine Learning

With colleagues at the University of Birmingham, I implemented an
  [abductive calculus](https://doi.org/10.1007/978-3-319-90686-7_6)
for machine learning as a PPX
  [extension](https://github.com/reubenrowe/ocaml-decml)
to OCaml.
This represents a new, principled paradigm for programming machine learning.
It is based on the observation that the process of learning the parameters of a
model can be seen as an analogue of C.&nbsp;S.&nbsp;Peirce's logical principle
of abduction. The calculus allows models to be defined using the functional
programming paradigm and their tunable parameters, denoted by provisional
constants, to be handled implicitly in a clean way.

#### Factorisation Calculus

The [Factorisation Calculus](https://doi.org/10.2178/jsl/1309952521) is a
combinatory rewrite system with the capability to analyse the syntactic
structure of a wide class of its own terms, making it a good candidate for a
fundamental model in which to study intensional computation, reflection, and
meta-programming.
I have [described](http://dx.doi.org/10.4204/EPTCS.190.6)
an encoding of the Factorisation Calculus into the &lambda;-Calculus;
I also supervised an MEng
  [dissertation]({{ '/assets/pdf/arb10.pdf' | prepend:site.baseurl | prepend:site.url }})
looking at a structural type system for the Factorisation Calculus.

#### Intersection Types for Featherweight Java

In my
  [MSc Dissertation]({{ '/publications/' | prepend:site.baseurl | prepend:site.url }}#MScDissertation)
and
  [PhD Thesis]({{ '/publications/' | prepend:site.baseurl | prepend:site.url }}#PhDThesis)
I investigated intersection type assignment for Featherweight Java, under the
supervision of
  [Steffen van Bakel](https://www.doc.ic.ac.uk/~svb/).
Intersection types are a type-theoretic approach for ad-hoc polymorphism,
allowing to specify that an expression has a particular number of different
types all at once.
This allows an exact type-based analysis, even with recursion, since each
expression can be given a type for each time it is used.
Featherweight Java is a formal calculus modelling the core features of
class-based object-oriented programming. I defined an intersection-based type
system for it, and showed that this can be used as a basis for a denotational
semantics.
I also looked at type inference for Nakano's
[guarded recursion](https://doi.org/10.1109/LICS.2000.855774).

#### Recursive Adaptive Grammars

An older research interest, which has been on the back burner for a while,
is in frameworks for extensible programming languages, and
[recursive adaptive grammars](http://web.cs.wpi.edu/~jshutt/thesis/top.html)
(RAGs) in particular.
I have written a RAG-based parser in Java which is hosted on
[Sourceforge](http://ragtools.sourceforge.net/).
(I really should move this over to Github, or similar!)
