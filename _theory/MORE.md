---
layout: concept
title: Management Option Rank Equivalence (MORE)
permalink: /theory/MORE/
excerpt: Management Option Rank Equivalence is a form of breakpoint analysis that reports the changes in each variable required to change the preferred management option.
purpose: MORE can be used for <a href="../theory/stress-testing/">stress testing</a> of a preferred management option. It is a form of <a href="../theory/breakpoint-analysis/">breakpoint analysis</a>, i.e. it focuses on values or scenarios for which a conclusion changes.
requirements: >
  <p>A model is used to evaluate performance metrics of management options in different model scenarios (expressed in terms of parameter combinations). A reference model scenario is required, e.g. that best fits historical data.</p>
decomposition: >
  <p>A distance metric is selected to determine the difference to the reference model parameters, e.g. a normalised Euclidean distance evaluates change in parameters relative to their maximum and minimum values.</p>
  <p>Optimisation is used to minimise that distance with the constraint that the optimised parameters yield a different preferred management option to the reference model (i.e. reverse the rank of the options).</p>
  <p>Pareto Optimal Management Option Rank Equivalence (POMORE) is a variant where the distances for each parameter are optimised separately as a multi-objective optimisation rather than specifying a distance metric. This yields a set of closest scenarios rather than just one.</p>
tools:
also_see:
further_reading:
  - Ravalico JK, Dandy GC, Maier HR (2010). <a href="https://doi.org/10.1016/j.envsoft.2009.06.012">Management Option Rank Equivalence (MORE) – A new method of sensitivity analysis for decision-making</a>. Environmental Modelling & Software, 25(2), 171–181. doi:10.1016/j.envsoft.2009.06.012
  - Ravalico JK, Maier HR, Dandy GC (2009) <a href="https://doi.org/10.1016/j.ress.2009.01.009">Sensitivity analysis for decision-making using the MORE method—A Pareto approach</a>. Reliability Engineering & System Safety, 94(7), 1229–1237. doi:10.1016/j.ress.2009.01.009
examples:
  - In a <a href="../../examples/guillaume-2015">simple flood demonstration problem</a> answering the question "Will regular flooding of ecological assets occur?", POMORE is applied to identify model scenarios where the answer changes.
---
