---
layout: concept
title: Robustness metrics
permalink: /theory/robustness-metrics/
excerpt: Robustness metrics measure how performance of an alternative changes in different scenarios
purpose: Alternatives can be ranked according to their robustness, including as part of <a href="../../theory/efficiency-robustness-tradeoffs/">Efficiency-Robustness trade-offs</a>. This is a quantitative form of <a href="../stress-testing/">stress testing</a>.
requirements: Evaluation of metrics requires performance measures across multiple scenarios, e.g. produced from multiple model runs with different settings.
decomposition: >
  <p>A wide range of robustness metrics are possible, depending on 1) how performance measures transformed, 2) scenarios are subsetted, 3) subsetted performance measures are aggregated [McPhail-2018]. See Resources for further details</p>
  <ul><li>Performance measures can, for example, be transformed by calculating regret from the best alternative, or by evaluating whether performance satisfies constraints</li>
  <li>Subsetting scenarios might involve taking the best or worst case, or another percentile</li>
  <li>Aggregation might involve taking mean, sum, variance or skew</li>
  </ul> Common robustness metrics include:
  <li>Maximin: Maximising worst-case performance</li>
  <li>Minimax regret: Minimising worst-case regret from best decision alternative</li>
  <li>Starr's domain criterion: Maximising proportion of scenarios where a performance threshold is satisfied</li>
tools:
also_see:
further_reading:
  - >
    McPhail C, Maier HR, Kwakkel JH, Giuliani M, Castelletti A, Westra S (2018) <a href="https://dx.doi.org/10.1002/2017EF000649">Robustness metrics: How are they calculated, when should they be used and why do they give different results?</a>. Earth's Future. doi:10.1002/2017EF000649
  - >
    Herman JD, Reed PM, Zeff HB, Characklis GW (2015). <a href="https://dx.doi.org/10.1061/(ASCE)WR.1943-5452.0000509">How Should Robustness Be Defined for Water Systems Planning under Change?</a>. Journal of Water Resources Planning and Management. 141 (10): 04015012. doi:10.1061/(ASCE)WR.1943-5452.0000509
examples:
---
