---
layout: case-study
title: How much climate change can reservoir operations cope with in Lake Como?
citation: (Culley et al., 2016)
permalink: /examples/culley-2016/
page_authors:
  - Caroline Rosello
  - Joseph Guillaume
page_reviewers:
excerpt: Vulnerability analysis building on decision scaling theory is used to identify changes in temperature and precipitation that would lead to flood or irrigation failures under current reservoir operations and optimal feedback control policies that increase the range of states under which minimum performance requirements are met.
approach: >
  <p>
  The authors investigate optimal <a href="../reservoir-operations/">reservoir operations</a> across hydrometeorological conditions to identify a system performance threshold under climate change uncertainty. That is, system operation is formulated as a <a href="../../theory/feedback-control/">feedback control policy</a>, and the overall objective is to find the theoretical upper limit for a water resources system's adaptation to climate change uncertainty, i.e. the <a href="../../theory/maximum-operational-adaptive-capacity">maximum operational adaptive capacity</a> beyond which even optimal operational rules fail to achieve societal objectives for a system of interest.
  </p>
  <p>
  The approach is a variant of the formal method referred to as <a href="../../theory/decision-scaling">"decision scaling"</a>. Testing performance of the optimal feedback control policies across changes in temperature and precipitation is a form of <a href="../../theory/stress-testing/">stress testing</a>, and the identification of failures to meet objectives is a form of <a href="../../theory/vulnerability-analysis/">vulnerability analysis</a>.
  </p>
  <p>Feedback control operating rules are modelled using an approximation technique called "Gaussian radial basis functions" (RBFs), describing reservoir releases over time and as a function of lake level. In addition to estimating a historical operating rule, <a href="../../theory/pareto-optimality"> Pareto-optimal </a> RBF policies are identified using evolutionary multiobjective "direct policy search". </p>
  <p>
  <h3>Methodological steps</h3>
  <p><img src="../../images/culley-2016-approach.jpg" width=90% alt="Outline of the approach to identify the maximum operational adaptive capacity of a water resource system. Four steps are described: 1) generation of an 'exposure space', 2) mapping of the current system on the 'exposure space', 3) identification of the optimal adaptive response to each exposure, 4) superimposition of climate exposure onto the exposure space">
  <div class=imgcredit>Figure 1 <a href="https://doi.org/10.1002/2015WR018253">Culley et al. 2016</a></div>
  </p>
  <ol>
  <li> Generation of an exposure space (H): <ul>
    <li> making incremental changes to hydrological variables' attributes. A n-dimensional exposure space is created, made of selected attributes (h), such as H = [h1,...,hn].  </li>
    <li> sampling the exposure space using a scaling of historical data to develop perturbed time series for the relevant climatic variables. </li> 
    </ul>
    <!-- TODO: we may need to provide more detail about perturbation and stochastic generation methods -->
  <li>Assessment of current system performance for each point of the exposure space:<ul>
    <li>Running a simulation model with current operation policy with each climate input (see <a href="../../theory/exploratory-modelling">exploratory modelling</a>)</li>
    <li>Separating "failure" from "success" conditions based on the definition of thresholds for acceptable values. </li>
    </ul>
  </li>
  <li>Assessment of the optimised system performance for each point of the exposure space, i.e. with optimal operation rules for each climate input</li>
  <li> Superimposition of climate projections onto the exposure space for the current and optimised system performance to identify climate conditions and timing for which the system may fail and when to implement management strategies to maximise a system adaptation capacity. 
  </li>
  </ol>
  </p>
problem_definition: >
  <p>Lake Como is a regulated lake in Northern Italy with an active storage capacity of 254 Mm<sup>3</sup>, sustaining water needs for irrigation and water supply, together with ensuring flood protection and environmental flow requirements in the Adda River. Its subalpine location implies that the lake is dependent on snowmelt to be filled, which requires the definition of strategic operation rules on an annual basis to support flood control and irrigation water demand objectives. In addition, changes in climate conditions and snowmelt runoff into the lake could increase tensions in the region.
  </p>
  <p> The problem is identification of operational rules to maximise the Lake Como system's adaptive capacity under climate change uncertainty</p>
  <p> Conditions of failure for the system :<ul>
  <li> daily flooded area over 100 m<sup>2</sup> </li>
  <li> daily average squared water deficit = 400 kL<sup>2</sup> </li></ul></p>
  <p>The optimal operation rule is based on a penalty function assessing <a href="../../theory/reliability">reliability</a>:<ul>
    <li>flood reliability function: the ratio of the days without a flood event within the simulation horizon</li>
    <li>irrigation reliability function: ratio of available supply to the demand averaged across all time steps, with ratio values capped at 1</li></ul>
  <p>Climate change projections in the climate exposure space are obtained from multiple models for the years 2025, 2050, 2075 and 2100, with statistical downscaling based on quantile mapping to generate future local climate change projections. </p>
  <p> Attributes for generating the climate exposure space:<ul>
  <li>Mean annual precipitation (mm): Precipitation was perturbed as a percentage change to daily wet days (over 1mm) from 90% to 130% of current values. </li>
  <li>Mean annual temperature: Temperature was perturbed for each daily time-step from -5℃ to 15℃ of current values. </li></ul></p>
  <p>
  The main result is the identification of the upper limit for adaptive capacity (failure boundary) to support irrigation and flood protection objectives in Lake Como. The identification of such a limit allows for dynamic management and the setting of optimal operating policies acoording to climate changes. It was found that the Lake Como system could adapt, by modifying operating policies, to more than three times as many hydrometeorological states compared to current operating rules.
  </p>
  <p><img src="../../images/culley-2016-results.jpg" width=90% alt="Climate projections for the years 2025, 2050, 2075 and 2100. The 22 climate scenarios are superimposed on the 'exposure space'. Conditions of success, adaptation and failure for each climate change scenario could be visualised. Eight models (climate change conditions) predict that the system would fail in the future, even under optimised operation conditions">
  <div class=imgcredit>Figure 6 <a href="https://doi.org/10.1002/2015WR018253">Culley et al. 2016</a></div>
  </p>
  <p>The result is conditional on certain key assumptions:<ul>
  <li>
  the selection of sensitive variables to generate the exposure space for which operational rules are sensitive. For that matter, a sensitivity analysis of the inputs is recommended to identify such variables.
  </li>
  <li> 
  accurate modelling of stakeholder demand to ensure the proper identification of conditions of failure
  </li>
  <li>
  the proper setting of operating policy structure and constraints for the optimisation process
  </li>
  <li>
  the choice of an appropriate model to represent reservoir decisions, able to change releases in response to extreme climate conditions
  </li>
  </ul>
  </p> 
  <p> Future considerations to improve the ability of the framework to identify upper limits include: <ul>
  <li>
  considering changes in water users' demands over time and application of a nonstationary system model within the framework 
  </li>
  <li>
  including more than two dimensions to generate the exposure space with an increased number of uncertain variables that influence the effectiveness of the operation rules
  </li>
  </ul>
  </p>
reference: >
  Culley, S., Noble, S., Yates, A., Timbs, M., Westra, S., Maier, H.R., Giuliani, M., Castelletti, A., 2016. <a href="https://doi.org/10.1002/2015WR018253">A bottom-up approach to identifying the maximum operational adaptive capacity of water resource systems to a changing climate </a>. Water Resources Research. 52, 6751–6768. doi:10.1002/2015WR018253 
  <p>Also see <a href="https://watermodelling.org/news/event-summary-coping-with-multiple-plausible-futures-in-the-face-of-climate-change">presentation for the Queensland Water Modelling Network</a>.</p>
---
