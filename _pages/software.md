---
layout: page
permalink: /software/
title: Software
---

The following is a list of software that I have been involved in developing as
part of my academic research activties.

### Rotor

<span class="smallcaps">Rotor</span> is a protoype automatic refactoring tool
for the [OCaml](https://ocaml.org/) programming language. Currently, it supports
renaming of top-level values within modules.
[Joe Harrison](https://www.cs.kent.ac.uk/people/rpg/jrh53/) and
[Steven Varoumas](https://www-apr.lip6.fr/~varoumas/index-en.html)
are currently working on implementing other kinds of refactoring.
We have had support from [Jane Street](https://www.janestreet.com/) in London.

<span class="smallcaps">Rotor</span> is currently hosted on
[Gitlab](https://gitlab.com/trustworthy-refactoring/refactorer) and is published
in the [OPAM](https://opam.ocaml.org/packages/rotor/) package repository for
OCaml.

Please visit <span class="smallcaps">Rotor</span>'s
[homepage](https://trustworthy-refactoring.gitlab.io/refactorer/) for more
details.

### Cyclist

Cyclist is a framework for building automatic deductive verifiers based on
cyclic proofs.
It contains a suite of related tools making use of the symbolic heap fragment
of Separation Logic.
These include:
  an entailment prover and disprover;
  a satisfiability checker;
  a model checker;
  a (termination) verifier for simple imperative programs with loops and
  recursive procedures;
  a verifier for temporal properties of simple imperative programs with loops;
  and a tool for abducing inductive predicates and sufficient conditions for memory-safe (terminating) execution of simple imperative programs with loops;
It also includes an entailment prover for inductive definitions over
first-order logic with successor.

Cyclist was originally developed by
[Nikos Gorogiannis](https://ngorogiannis.bitbucket.io/)
and is hosted on [Github](https://github.com/ngorogiannis/cyclist).
Please visit Cyclist's [homepage](https://www.cyclist-prover.org/) for more
details.

### DecML OCaml Extension

DecML is a PPX extension for the OCaml programming language that implements the
abductive calculus described in
[this paper]({{ '/publications/#DecML-FLOPS' | prepend:site.baseurl | prepend:site.url }}).
Further details can be found in this
[technical report](https://arxiv.org/abs/1710.03984).
It allows machine learning models to be specified as functions with specially
marked constants denoting tunable parameters. These constants can then be
'decoupled' from the function, to give a parameterised function that can be used
to learn the correct value of the parameters using observed data
(e.g. using gradient descent).

The extension is hosted on [Github](https://github.com/reubenrowe/ocaml-decml).

An [alternative implementation](https://github.com/DecML/decml-ppx) was
developed by [Victor Darvariu](https://victor.darvariu.me/) for his MSci
dissertation.

### RAG Parser

The [recursive adaptive grammar](https://web.cs.wpi.edu/~jshutt/rags.html)
(RAG) formalism was devised by [John Shutt](https://web.cs.wpi.edu/~jshutt/).
It is a grammar formalism for declaratively specifying arbitrary, recursively
enumerable languages.
A recursive adaptive grammar can be seen as a kind of attribute grammar, in
which each non-terminal is synthesises a single (semantic) attribute.
The expressive power derives from a *query* operator, which allows a
synthesised attribute to be treated and parsed as *syntax*.

I constructed and implemented a RAG parsing algorithm.
It is hosted on
[Github](https://github.com/reubenrowe/rags).
