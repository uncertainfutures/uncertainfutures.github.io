---
layout: problem
banner: WIP
title: Urban water resource planning
permalink: /examples/urban-water-resource-planning/
page_authors:
  - Joseph Guillaume
page_reviewers:
excerpt: Urban water resource planning involves selecting supply and demand management options for future scenarios, especially climate changes and population growth.
summary: >
  <p>Supply capacity planning has long recognised the uncertainty in forecasting water demand, and the need to plan for climate change is now mainstream. New water supply options are  often capital intensive, which means that careful planning in the face of multiple plausible futures is typically worthwhile, while recognising that political concerns also play a role in final decisions.</p>
  <p>Water supply options include new dams, rainwater tanks, stormwater harvesting, recycled water, and desalination. Water demand options include permanent and temporary water restrictions, changing water pricing, and supporting adoption of more water efficient fixtures. <a href="../reservoir-operations/">Reservoir operations</a> may also influence available supply at critical times, and urban water supply options may interact with other uses of water, including hydropower, irrigation, recreation, environmental and cultural. Planning may involve selecting the level of investment/capacity and sequencing of options over time.</p>
  <p>Objectives include reliability of supply, maximum shortfall, cost, and greenhouse gas emissions.</p>
  <p>Key assumptions about the future include climate change, population growth, discount rates, and changes in prioritisation of objectives.</p>
approaches: >
  <p>Optimisation is commonly used to identify optimal sequences of investment for multiple plausible futures [1,2], which can be evaluated in terms of their <a href="../../theory/robustness-metrics/">robustness</a> [2].</p>
  <p>Sequences of management options can form <a href="../../theory/adaptive-pathways/">adaptive pathways</a>, investing only in a first management option while expecting changes to be made during implementation of the plan. <a href="../../theory/flexibility/">Flexibility</a> to change pathways can been explicitly quantified [2].</p>
cases:
  - >
    <a href="../beh-2015-sequencing/">Beh et al. (2015)</a> identify optimal sequences of additional water supply options for Adelaide for a set of scenarios with different climate change, population growth, and discount rates. Sensitivity analysis shows how performance of each plan varies across scenarios, and which variables have greater influence, to help inform selection of an optimal sequence plan.
  - >
    In a second article, <a href="../beh-2015-multiobjective/">Beh et al. (2015)</a> assess <a href="../../theory/robustness-metrics/">robustness</a> and <a href="../../theory/flexibility/">flexibility</a> of <a href="../../theory/pareto-optimality/">Pareto optimal</a> water supply sequences in multiple 10 year planning horizons, selecting a plan using an explicit <a href="../../theory/efficiency-robustness-tradeoffs/">efficiency-robustness tradeoff</a>.
  - In a collaboration with the Inland Empire Utilities Agency, California, <a href="../groves-2008/">Groves et al. (2008)</a> use a <a href="../../theory/robust-decision-making/">robust decision making</a> approach evaluating existing and alternative <a href="../../theory/adaptive-decisions/">adaptive</a> plans against climate change and planning uncertainties. <a href="../../theory/scenario-discovery/">Scenario discovery</a> is used to identify vulnerable scenarios, and <a href="../../theory/robustness-metrics/">robustness</a> is evaluated in terms of number of cases where failure occurs.
references:
  - >
    [1] <a href="../beh-2015-sequencing/">Beh et al. (2015)</a>, involving sequencing water supply options in Adelaide
  - >
    [2] <a href="../beh-2015-multiobjective/">Beh et al. (2015)</a>, involving robust and flexible water supply sequences in Adelaide
---
