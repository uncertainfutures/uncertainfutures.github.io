---
layout: concept
title: Multiple Plausible Futures
permalink: /theory/multiple-plausible-futures/
excerpt: >
  "Multiple plausible futures" describes a distinct way of describing uncertainty about the future, with its own distinct approaches for handling that uncertainty.
purpose: >
  <p>Describing uncertainty in terms of multiple plausible futures recognises that there is certain information we do not have <i>(see (a) and (b) in the figure below)</i>:<ol>
  <li>it does not make sense to plan for a single best projection of the future</li>
  <li>we cannot use probabilities, e.g. to select a solution that <a href="../theory/expected-utility-maximisation/">performs well on average</a>, <a href="../theory/maximise-reliability.">guarantees a specific level of reliability</a> or <a href="../theory/expected-shortfall/">minimises expected shortfall</a></li>
  <li>the future is not bounded, so we cannot simply <a href="../robust-optimisation/">plan for the worst case</a>.</li>
  </ol>
  </p>
  <p>Instead, we have to act and plan as if any of the multiple plausible futures could occur -  and possibly others <i>(see (c) in the figure)</i>.</p>
  <p>It may be that we have more information about some aspects of the future, such that "multiple plausible futures" may be mixed with other ways of describing the future <i>(see (d) in the figure)</i>.</p>
  <p>
    <img src="../../images/maier-2016-fig1.jpg" width=50% alt="The difference between describing future system states through: a) anticipating the future based on best available knowledge, b) quantifying future uncertainty, c) exploring multiple plausible futures, d) combining the three paradigms to address different sources of uncertainty within a problem".
  </p>
requirements: >
  <p>Given that "multiple plausible futures" is a way of describing uncertainty about the future, in principle it can be used even if one future is considered more likely than all others, or bounds and probabilities could be assigned. However, the result is that this extra information is discarded (e.g. because it is considered insufficiently unreliable), which may not be what you are after.<p>
  <p>Multiple plausible futures are commonly encountered in strategic decision making in the face of climate change and global change, and where there are known tipping points with unknown thresholds.</p>
decomposition: >
  <p>The basic element for handling multiple plausible futures is a "<a href="../theory/scenario-development">scenario</a>", which describes a future either in terms of states of the world (e.g. values of different of variables), or coherent storylines. Each scenario should be based on different assumptions about the future.</p>
  <p>Scenarios are often quantified using computational models. In that case, we distinguish between "model scenarios" that capture a best available understanding of a system from model scenarios that explore different assumptions about the future, which we refer to as <a href="../theory/exploratory-modelling">exploratory modelling</a>.</p>
  <p>In the context of multiple plausible futures, "decision making" means that we need to develop a single plan of action that somehow achieves its objectives regardless of which of the plausible futures occurs. There are two key strategies:
  </p>
  <ul>
  <li>"<a href="../theory/robust-decisions/">Robust decisions</a>" literally perform well across a range of scenarios. Their robustness can be <a href="../theory/robustness-metrics/">measured</a>, or we can <a href="../theory/stress-testing/">evaluate how their performance varies across scenarios</a>, including <a href="../theory/vulnerability-analysis/">circumstances where the plan of action fails</a>.</li>
  <li>"<a href="theory/adaptive-decisions">Adaptive decisions</a>" recognise that the single plan of action can actually change over time as the future unfolds, resulting in "<a href="../theory/adaptive-pathways">adaptive pathways</a>", which may involve assessing the <a href="../theory/value-of-information/">value of information</a> or identifying <a href="../theory/triggers">triggers</a> to change direction.</li>
  </ul>
  <p>Adaptive solutions can be robust, so the adaptive approach in fact contrasts with a static, single fixed strategy, which may be preferable if uncertainty over the planning horizon is not too high, there is limited flexibility in the decision to be made, and it would take too long to change the plan of action.</p>
  <p>
    <img src="../../images/maier-2016-fig4.jpg" alt="Adaptive rather than static approaches to robustness are more appropriate when uncertainty over the planning horizon is high, flexibility of solutions is high, and implementation time relative to rate of change is high.".
  </p>
  <p>
  Robust and adaptive decisions allow a course of action to be selected because they provide confidence that we have considered how that course of action might play out across plausible scenarios, and the course of action is either superior to alternatives (i.e. it is an optimal solution), or meets all requirements (i.e. it is a "satisficing" solution).
  </p>
  <p>As a decision maker, if you'd like an analyst to help identify robust or adaptive decisions, ask for:</p>
  <ul>
  <li><a href="../theory/exploratory-modelling">Exploratory modelling</a> and <a href="../theory/scenario-development">scenarios</a> to explore how the future might unfold under different assumptions</li>
  <li><a href="../theory/robustness-metrics/">Evaluation of robustness</a>, <a href="../theory/stress-testing/">stress testing</a> or <a href="../theory/vulnerability-analysis/">vulnerability analysis</a> of decision alternatives</li>
  <li><a href="../theory/adaptive-pathways">Design of adaptive pathways</a>, <a href="../theory/monitoring-plan/">monitoring plans</a> or <a href="../theory/triggers/">identification of triggers</a>
  </li>
  </ul>
tools:
also_see:
further_reading:
  - >
    Maier HR, Guillaume JHA, van Delden H, Riddell GA, Haasnoot M, Kwakkel JH (2016) <a href="https://dx.doi.org/10.1016/j.envsoft.2016.03.014">An Uncertain Future, Deep Uncertainty, Scenarios, Robustness and Adaptation: How Do They Fit Together?</a>. Environmental Modelling & Software 81 (July): 154–64. doi:10.1016/j.envsoft.2016.03.014
examples:
  - <a href="../../examples/environmental-water-management">Environmental water management</a> in the face of climate uncertainty
  - <a href="../../examples/reservoir-operations">Reservoir operations</a> in the face of climate uncertainty
  - <a href="../../examples/urban-water-resource-planning">Urban water resource planning</a> with uncertain climate and population
  - The <a href="../../examples/lake-problem">Lake Problem</a>, handling tipping points
references:
---
