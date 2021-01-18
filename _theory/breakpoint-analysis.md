---
layout: concept
title: Breakpoint analysis
permalink: /theory/breakpoint-analysis/
excerpt: Breakpoint analysis identifies values of a variable at which a change occurs, e.g. a management option fails, or the preferred solution changes.
purpose: >
  While breakpoint analysis is a general concept, it can specifically be used for decision making in the face of multiple plausible futures to perform <a href="../vulnerability-analysis/">vulnerability analysis</a> (which is itself a form of <a href="../stress-testing/">stress testing</a>).
requirements: >
  Breakpoint analysis needs to be evaluate success/failure while varying values of a variable, and therefore requires a system model where the relevant variables can be modified by an external algorithm.
decomposition: >
  <p>A range of algorithms are possible depending on the number of variables and the nature of the boundary between success and failure. In general, the boundary forms a lower dimensional "manifold" in model scenario space, such that even with only two variables there are an infinite number of possible breakpoints. Selecting interesting breakpoints is therefore a key issue.</p>
  Specific approaches implementing breakpoint analysis include:
  <ul>
  <li><a href="../MORE/">Management Option Rank Equivalence (MORE)</a>, which uses optimisation to report the changes in each variable required to change the preferred management option</li>
  <li><a href="../crossover-point-scenarios/">Crossover point scenarios</a>, i.e. scenarios where the preferred option changes</li>
  <li><a href="../info-gap/">Info-gap decision theory</a></li>
  </ul>
tools:
also_see:
further_reading:
examples:
  - In a <a href="../../examples/guillaume-2015">simple flood demonstration problem</a> answering the question "Will regular flooding of ecological assets occur?", breakpoint analysis is performed using <a href="../MORE/">POMORE</a> (a variant of MORE), and through <a href="../optimisation-based-hypothesis-testing/">optimisation-based hypothesis testing</a>
references:
---
