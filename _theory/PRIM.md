---
layout: concept
title: PRIM
permalink: /PRIM/
excerpt: PRIM (Patient Rule Induction Method) is a "bump-hunting" algorithm that identifies "boxes" in parameter space with "interesting" scenarios.
purpose: PRIM can be used for <a href="/scenario-discovery/">scenario discovery</a> where the scenarios identified will be represented as bounds on parameter values within which scenarios meet some pre-defined criteria.
requirements: Scenarios need to be defined by a set of parameter values and PRIM requires a sample of scenarios across parameter space.
decomposition: >
  <p>Scenarios can be randomly or systematically sampled but need to cover the parameter space well to obtain sensible parameter bounds</p>
  <p>Scenarios are identified as interesting based on pre-defined criteria, e.g. scenarios where the selected decision alternative fails to meet required performance criteria (or succeeds).</p>
  <p>The PRIM algorithm is provided each scenario's parameter values and classification (interesting/uninteresting).</p>
  <p>The algorithm identifies boxes in parameter space. There is a trade-off between coverage, density, and interpretability. High coverage means that the box includes a higher proportion of the ‘interesting’ model scenarios available through parameter space. High density means that the box includes a higher proportion of ‘interesting’ cases relative to non-interesting ones. Some bounds may be more interpretable than others </p>
  <p>The selection of boxes is usually interactive to address this trade-off, using graphs or constraints on the algorithm to find a box of interest.</p>
tools:
  - slug: sdtoolkit
    name: sdtoolkit
    description: an R package implementing PRIM specifically for scenario discovery
  - slug: emaworkbench
    name: Exploratory Modelling and Analysis (EMA) Workbench
    description: a Python package that includes a scenario discovery oriented implementation of PRIM.
also_see:
  - permalink: tools/CART
    name: CART
    description: A common alternative algorithm for scenario discovery
further_reading:
  - >
    Bryant BP, Lempert RJ (2010) <a href="https://dx.doi.org/10.1016/j.techfore.2009.08.002">Thinking inside the box: A participatory, computer-assisted approach to scenario discovery.</a> Technological Forecasting and Social Change, 77(1), 34–49. doi:10.1016/j.techfore.2009.08.002
examples:
---
