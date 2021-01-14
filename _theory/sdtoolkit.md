---
layout: tool
title: sdtoolkit (R package)
permalink: /tools/sdtoolkit/
excerpt: <i>sdtoolkit</i> is a package for the R statistical programming language to perform scenario discovery using the PRIM algorithm
purpose: The package provides interactive functions for <a href="/scenario-discovery/">scenario discovery</a>, stepping the user through the use of PRIM. <a href="/PRIM/">PRIM</a> identifies "boxes" in parameter space with "interesting" scenarios, i.e. bounds on parameters where scenarios meets some pre-defined criteria.
requirements: >
  PRIM operates on a sample of scenarios, where each scenario is defined by a set of parameter values. Data needs to be provided with performance statistics for each scenario, along with criteria for determining whether the scenario is "interesting", e.g performance is unsatisfactory.
  <p>The <a href="https://www.r-project.org/">R software environment</a> needs to be installed, which is commonly used with the <a href="https://rstudio.com/products/rstudio/">RStudio</a> editor.</p>
  <p>See <a href="/PRIM/">PRIM</a> for discussion of advantages and disadvantages relative to other scenario discovery methods.</p>
decomposition: The main function in the package is <i>sdprim</i>, which steps through a series of questions and provides interactive visualisations of the boxes identified. This particularly addresses the trade-off between boxes including a higher proportion of the ‘interesting’ model scenarios available through parameter space (coverage), vs higher proportion of ‘interesting’ cases relative to non-interesting ones (density).
further_reading:
  - >
    <a href="https://cran.r-project.org/package=sdtoolkit">Home page</a> on the Comprehensive R Archive network (CRAN), with <a href="https://cran.r-project.org/web/packages/sdtoolkit/sdtoolkit.pdf">reference manual</a>
  - >
    Bryant BP, Lempert RJ (2010) <a href="https://dx.doi.org/10.1016/j.techfore.2009.08.002">Thinking inside the box: A participatory, computer-assisted approach to scenario discovery.</a> Technological Forecasting and Social Change, 77(1), 34–49. doi:10.1016/j.techfore.2009.08.002
examples:
---
