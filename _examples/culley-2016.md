---
layout: case-study
title: How much climate change can reservoir operations cope with in Lake Como?
citation: (Culley et al., 2016)
permalink: /examples/culley-2016/
excerpt: Vulnerability analysis building on decision scaling theory is used to identify changes in temperature and precipitation that would lead to flood or irrigation failures under current reservoir operations and optimal feedback control policies that increase the range of states under which minimum performance requirements are met.
approach: >
  <p> Summary of the problem: 
  <li> Lake Como is a regulated lake in Northern Italy with an active storage capacity of 254 Mm<sup>3</sup>, sustaining water needs for irrigation and water supply, together with ensuring flood protection and environmental flow requirements in the Adda River. Its subalpine location implies that the lake is dependent on snowmelt to be filled, which implies the definition of strategic operation rules on an annual basis to support flood control and irrigation water demand' s objectives. In addition, changes in climate conditions and snowmelt runoff into the lake could increase tensions in the region. </li>
  </p>
  <p> Concepts and methods used to solve the problem: <ul>
  <li> The authors used a <a href="../therory/decision-scaling"> decsion scaling </a> approach based to identify a system performance threshold under climate change uncertainty (see <a href="../theory/multiple-plausible-futures">multiple plausible futures</a> and, in the context of operational rules effectiveness, to identify vulnerable hydrometeorological conditions in which operational rules may fail to achieve societal objectives for a system of interest. </li>
  <li> The approach is based on the formulation of the system operation as a feedback control policy to maximise the <a href="../theory/robust-decisions">robustness</a> and <a href="../theory/adaptive-decisions">adaptive</a> capacity of a system. The process is repeated for different hydrometeorological conditions to identify optimal operational rules decisions. The overall objective is to find the theoretical upper limit (i.e., the maximum operational adaptive capacity) for a water resources system's adaptation to climate change uncertainty by identifying optimal management policies. </li>
  <li> The mathematical formulation of the operating policy is based on the application of Gaussian radial basis functions (RBFs). The approach estimates multiple input parameters for a single output. <a href="../theory/pareto-optimality> Pareto-optimal </a> RBF policies are identified based on the use of the evolutionary multiobjective direct policy search. </li>
  <li> Overall, the approach could be described as a <a href="../theory/stress-testing> stress testing </a> approach to map the performance of current and optimised operational rules (see <a href="../theory/management-options">management options</a>). </li>
  <li> Methodological steps: <ol>
  <li> Generation of an exposure space (H), using a simulation model (see <a href="../theory/exploratory-modelling">exploratory modelling</a>), by: <ol>
  <li> making incremental changes to hydrological variables' attributes. A n-dimensional exposure space is created, made of selected attibutes (h), such as H = [h1,...,hn].  </li>
  <li> sampling the exposure space using a scaling of historical data to develop perturbed time series for the relevant climatic variables. </li> </ol>
  <li> Assessment of the current system performance based on the application of the current operation policy and simulation of the system performance for each point of the exposure space. Boundary conditions are identified separating "failure" conditions from "success" ones and based on the definition of a threshold for acceptable values. </li>
  <li> Assessment of the optimised system performance based on the identification of operational rules maximising the system performance for each hydrometeorological state in the exposure space. Boundary conditions are delineated between "failure" and "success" based on the given optimal policy.</li>
  <li> Superimposition of climate projections onto the exposure space with the boundary representations for the current system performance and the optimised one to identify climate conditions and timing (see <a href="../theory/triggers"> triggers</a>) for which the system may fail and when to implement management strategies to maximise a system adaptation capacity. </li>
  </ol></li>
  </ul></p>
problem_definition: >
  <p> The problem is "how to define operational rules to maximise the Lake Como system's adaptive capacity under climate change uncertainty?" </p>
  <p> Objectives for the system: flood control and water <a href="../theory/reliability">reliability</a> for irrigation. </p>
  <p> Conditions of failure for the system :<ul>
  <li> daily flooded area over 100 m2 </li>
  <li> daily average squared water deficit = 400 kL2 </li></ul></p>
  <p> Downscaling approach to climate change scenarios based on the application of a statistical downscaling method based on quantile mapping to generate future local climate change projections. Climate change projections in the climate exposure space are obtained for the years 2025, 2050, 2075 and 2100. </p>
  <p> Attributes for generating the climate exposure space: mean annual precipitation (mm) and mean annual temperature. <ul>
  <li> Precipitation was perturbed as a percentage change to daily wet days (over 1mm) from 90% to 130% of current values. </li>
  <li> Temperature was perturbed for each daily time-step from -5℃ to 15℃ of current values. </li></ul></p>
reference: >
  Culley, S., Noble, S., Yates, A., Timbs, M., Westra, S., Maier, H.R., Giuliani, M., Castelletti, A., 2016. <a href="https://doi.org/10.1002/2015WR018253">A bottom-up approach to identifying the maximum operational adaptive capacity of water resource systems to a changing climate </a>. Water Resources Research. 52, 6751–6768. doi:10.1002/2015WR018253 
  <p>Also see <a href="https://watermodelling.org/news/event-summary-coping-with-multiple-plausible-futures-in-the-face-of-climate-change">presentation for the Queensland Water Modelling Network</a>.</p>
---
