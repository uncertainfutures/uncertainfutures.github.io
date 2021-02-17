---
layout: problem
title: Reservoir operations
banner: WIP
permalink: /examples/reservoir-operations/
page_authors:
  - Joseph Guillaume
page_reviewers:
excerpt: Planning of reservoir releases or operational rules is moving away from historical inflows and demand estimates to consider possible future climates and operation conditions, while also playing a key role in adaptation of water resource systems more generally.
summary: >
  <p>Planning of reservoir operations involves defining reservoir releases, release rules, or regulations limiting operators' decisions. Release rules may be dependent on reservoir conditions, season, or other conditions.</p>
  <p>Objectives include flood protection, hydropower production, and maximising water supply or guaranteeing its reliability. This may include environmental flows.</p>
  <p>Performance of reservoir operations depends on climate (especially inflows), but also on other water management options in use, changing management priorities over time, and the <a href="../../theory/value-of-information/">value of forecasts</a>. These are aspects that can be described as <a href="../../theory/multiple-plausible-futures/">multiple plausible futures</a>. Interaction between water management options is particularly relevant in multi-reservoir systems and <a href="../urban-water-resource-planning">urban water resource planning</a>.</p>
# TODO: mention hedging rules
approaches: >
  <p>Optimisation is commonly used to identify best performing releases or rules. Optimisation can therefore be repeated for multiple plausible futures, or optimising <a href="../../theory/robustness-metrics/">robustness metrics</a> across scenarios.</p>
  <p><a href="../../theory/vulnerability-analysis">Vulnerability analysis</a> has been used to identify climate changes in rainfall and temperature in which flood or irrigation failure may occur [1]</p>
# TODO: add Direct Policy Search. Giuliani et al. 2016
cases:
  - >
    <a href="../culley-2016/">Culley et al (2016)</a> uses <a href="../../theory/vulnerability-analysis">vulnerability analysis</a> to test and improve how much climate change reservoir operations can cope with in Lake Como, Italy. The analysis identifies changes in temperature and precipitation that would lead to flood or irrigation failures under current reservoir operations and optimal feedback control policies that increase the range of states under which minimum performance requirements are met.
references:
  - >
    [1] <a href="../culley-2016/">Culley et al. 2016</a>
---
