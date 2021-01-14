---
layout: problem
title: The Lake Problem
permalink: /examples/lake-problem/
excerpt: The Lake Problem is a stylized decision problem regarding pollution control often used to demonstrate approaches for supporting decision making under uncertainty.
summary: The population of a city has to decide on the amount of annual pollution it will put into a lake. If the pollution in the lake passes a threshold, it will suffer irreversible eutrophication. Allowing increased pollution reduces costs. Making large changes to allowed pollution between years is also difficult.
approaches: >
  <p>The lake problem has the ability to represent tipping points, nonlinearity, and deep uncertainties. It has been used to demonstrate new methods and software, including the <a href="../../tools/emaworkbench/">EMA Workbench</a> and <a href="../../tools/OpenMORDM">OpenMORDM</a>.</p>
  <p>Methods applied include:</p>
  <ul>
  <li>Expected utility maximisation</li>
  <li><a href="../../robust-decision-making/">Robust decision making</a> and <a href="../../MORDM/">many-objective robust decision making</a>, optimising robustness with <a href="../../robustness-metrics/">robustness metrics</a></li>
  </ul>
  Variants of the problem include:
  <ul>
  <li>Known and uncertain model parameters and thresholds</li>
  <li>Representation of decision alternatives through "direct policy search", which optimises a state-aware control rule rather than the pollution releases themselves</li>
  </ul>
cases:
  - >
    Original formulation, demonstrating impact of uncertainty and lags
    <p>Carpenter SR, Ludwig D, Brock WA (1999) <a href="https://dx.doi.org/1890%2F1051-0761%281999%29009%5B0751%3AMOEFLS%5D2.0.CO%3B2">Management of eutrophication of lakes subject to potentially irreversible change</a>. Ecological Applications, 9 (751), p. 771. doi: 10.1890%2F1051-0761%281999%29009%5B0751%3AMOEFLS%5D2.0.CO%3B2</p>
  - >
    Shows that stakeholders maximizing their expected utility can cause periodic collapses of the lake ecosystem if there is uncertainty about the lake’s eutrophication thresholds
    <p>Peterson GD, Carpenter SR, Brock WA (2003) <a href="http://dx.doi.org/10.1890/0012-9658(2003)084[1403:UATMOM]2.0.CO;2">Uncertainty and the management of multistate ecosystems: an apparently rational route to collapse</a>. Ecology 84:1403-1411. doi:10.1890/0012-9658(2003)084[1403:UATMOM]2.0.CO;2</p>
  - >
    Identifies robust solutions that compromise optimality for acceptable performance under a broader envelope of uncertainty assumptions (<a href="../../efficiency-robustness-tradeoffs">Efficiency-Robustness trade-offs</a>)
    <p>R.J. Lempert, M. Collins (2007) <a href="https://doi.org/10.1111/j.1539-6924.2007.00940.x">Managing the risk of uncertain threshold response: comparison of robust, optimum, and precautionary approaches</a>. Risk Anal., 24 (4) (2007), pp. 1009-1026. doi:10.1111/j.1539-6924.2007.00940.x</p>
  - >
    Demonstration of <a href="../../MORDM/">many-objective robust decision making</a>
    <p>Singh R, Reed PM, Keller K (2015) <a href="https://dx.doi.org/10.5751/ES-07687-200312">Many-objective robust decision making for managing an ecosystem with a deeply uncertain threshold response</a>. Ecology and Society 20(3): 12. doi:10.5751/ES-07687-200312<p>
  - >
    Demonstration of the <a href="../../tools/emaworkbench/">EMA Workbench</a>
    <p>Kwakkel JH (2017) <a href="https://dx.doi.org/10.1016/j.envsoft.2017.06.054">The Exploratory Modeling Workbench: An open source toolkit for exploratory modeling, scenario discovery, and (multi-objective) robust decision making</a>. Environmental Modelling & Software 96, 239–250. doi:10.1016/j.envsoft.2017.06.054</p>
  - >
    Demonstration of the <a href="../../tools/OpenMORDM">OpenMORDM</a> R package
    <p>Hadka D, Herman JD, Reed PM, Keller K (2015) <a href="https://doi.org/10.1016/j.envsoft.2015.07.014">OpenMORDM: an open source framework for many objective robust decision making</a>. Environ. Model. Softw., 74, pp. 114-129. doi:10.1016/j.envsoft.2015.07.014</p>
  - >
    Presents a version of the lake problem as a threshold problem for benchmarking of optimisation algorithms
    <p>Ward VL, Singh R, Reed PM, Keller K (2015) <a href="https://doi.org/10.1016/j.envsoft.2015.07.020">Confronting tipping points: can multi-objective evolutionary algorithms discover pollution control tradeoffs given environmental thresholds?</a> Environ. Model. Softw., 73 (1) (2015), pp. 27-43. doi:10.1016/j.envsoft.2015.07.020</p>
  - >
    Demonstration of "direct policy search" with <a href="../../MORDM/">many-objective robust decision making</a>
    <p>Quinn JD, Reed PM, Keller K (2017) <a href="https://dx.doi.org/10.1016/j.envsoft.2017.02.017">Direct policy search for robust multi-objective management of deeply uncertain socio-ecological tipping points</a>. Environmental Modelling & Software. 92: 125–141. doi:10.1016/j.envsoft.2017.02.017</p>
---
