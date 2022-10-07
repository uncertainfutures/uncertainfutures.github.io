---
layout: under-construction
title: Scenario driven optimal sequencing under deep uncertainty - Example of the Southern Adelaide Water Supply System
citation: (Beh et al. 2015)
permalink: /examples/beh-2015-sequencing/
page_authors:
  - Caroline Rosello
  - Joseph Guillaume
page_reviewers: Leila Noble
excerpt: The analysis identifies optimal sequences for adding to an urban water supply for a set of scenarios with different values for climate change, population and discount rates. Sensitivity analysis shows how the performance of each sequence for multiple criteria varies across the scenarios, and which uncertain variables have greater influence, to help inform decision-makers. 
approach: >
<p> 
The approach consists of the evaluation of sequences of water supply augmentation options (i.e., additional options to support current water supplies) over a planning horizon to cope optimally with future conditions.
</p>
<p>
Prior to analysis, the problem needs to be defined including the objectives, the planning horizon, the intervals at which new water supply options may be added, the water supply options, and constraints. Stakeholders should be involved. 
</p>
<p>
Following the problem framing stage, there are three steps:
<p>
<img src="../../images/beh-2015-sequencing-approach.jpg" width=70% alt="Conceptual representation of the scenario driven optimal sequencing approach. Three steps are involved: 1) the generation of the portfolio of optimal sequences under various future conditions, 2) sensitivity analysis to evaluate the robustness of the optimal sequences and identify influential critical risk factors, 3) the selection of the optimal sequence for implementation.">
<div class=imgcredit>Figure 1 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
<ol>
<li> Step 1 consists of the generation of the portfolio of optimal sequences. As for <a href="../theory/robust-decision-making/"> robust decision making </a> approaches, this step aims at identifying plausible solutions able to perform under different future conditions. Three sub-steps are involved:
<ol>
<li> identifying uncertain variables and their plausible ranges over the planning horizon </li>
<li> identifying plausible future scenarios with different combinations of values of uncertain variables </li>
<li> generating <a href="../theory/pareto-optimal/">Pareto-optimal </a> sequences for each scenario with respect to pre-defined constraints for the different objective functions. This step may involve the use of multi-objective evolutionary algorithms (MOEAs). </li>
</ol>
<li> Step 2 consists of a sensitivity analysis. It evaluates the performance the Pareto-optimal sequences identified in step 1 under a range of future conditions and the relative contribution of uncertain variables to the performance. Points to consider are: 
<ul>
<li> Performance metrics should include multiple specified objectives and additional measures such as reliability, resilience, or vulnerability metrics. </li>
<li> To account for variability in system states, the sensitivity analysis should be repeated multiple times for each optimal sequence. </li>
</ul>
</li>
<li> Step 3 consists of decision-makers making a selection from the optimal sequences. Their decision should consider: <ul>
<li> trade-offs between performance objectives' absolute (e.g. average) values and variability </li>
<li> the relative contribution of uncertain variables to performance variability and consideration of the feasibility of managing those variables </li>
<li> the degree to which constraint violations could be managed </li>
<li> the degree of adaptability of the different optimal sequences (noting that sequences that are similar at early stages are more adaptable) </li>
</ul>
</li>
</ol>
</p>
problem_definition: >
<p>
Adelaide, the capital of South Australia, is one of the driest capital cities worldwide. It has a population of about 1.3 million with an estimated mean annual water consumption of 163 GL in 2008. The southern Adelaide water supply system (WSS) is the major water supplier, delivering 50% of the metropolitan water demand. Three reservoirs support the system supply. 
</p>
<p> 
To cater for the projected water demand due to population growth and climate change, different water supply augmentation sources have been considered including a desalination plant, diverse stormwater harvesting schemes and household rainwater tanks.
</p>
<p>
The robustness of sequences including existing supplies and potential supply augmentation options are evaluated against potential future conditions using the multiobjective, scenario driven optimal sequencing approach. 
</p>
<p> 
The problem formulation includes: <ul>
<li> Defining objectives and constraints:<ul>
<li> Objectives: minimisation of the PV (present value) costs and PV greenhouse gas (GHG) emissions. </li>
<li> Constraints: the supply capacity is greater or equal to the demand.</li>
</ul>
</li>
<li> Defining decision variables: <ul>
<li> Planning horizon of 40 years </li>
<li> Decision points every 10 years (staging interval) </li>
<li> Current and future water supply sources are provided in table 1. Not all of these options are independent. For instance, a specific desalination plant or stormwater harvesting scheme can only be selected once.
<p>
<img src="../../images/beh-2015-sequencing-supply-details.jpg" width=70% alt="Details of the different water supplies to be evaluated, including capital and operating costs.">
<div class=imgcredit>Table 1 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
</li>
<li> Nine decision variables are considered as described in table 2:
<p>
<img src="../../images/beh-2015-sequencing-decision-variables.jpg" width=70% alt="Details of the nine decision variables including decision point ranges from current time (0) to the end of the planning horizon (5) or based on household tank size (from 1kL to 10 kL.">
<div class=imgcredit>Table 2 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
</li>
</ul>
</li>
<li> Checking constraints and calculation of objectives. <ul>
<li> Uses a simulation of the water supply, in this case WaterCress (Water-Community Resource Evaluation and Simualtion System).<li>
<li> Check that, for each sequence, constraints on supply are not violated (i.e. demand does not exceed supply) and feasibility criteria for the desalination plant are satisifed.</li>
<li> Objective functions are calculated based on the PV capital and operation costs and PV GHG emissions for the water supply system.</li>
</ul>
</li>
</ul>
</p>
<p> Step 1: Determination of the portfolio of optimal sequences. 
<ol>
<li> The uncertain variables considered are population growth, climate change (rainfall and evaporation), and discount rates for capital and operation costs and GHG emissions.</li>
<li> Seven scenarios are considered (table 3):
<p>
<img src="../../images/beh-2015-sequencing-scenarios.jpg" width=70% alt="Details for the seven scenarios considered.">
<div class=imgcredit>Table 3 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
These scenarios are representative of a continuum in future conditions from the best possible future conditions (scenario 1) to the worst possible (scenario 7) in terms of population and climate changes. The discount rate does not vary because it does not directly influence future water supply and demand.
</li>
<li> The WaterCress simulation model is used to estimate the supply, demand and costs and GHG emissions for the water supply systems under the seven scenarios, over the planning horizon, with consideration of constraints. The Water System Multiobjective Genetic Algorithm (WSMGA) is used to generate Pareto-optimal sequences. The Pareto-front sequences are displayed in figure 2 and are associated with the sequences in table 4.
<p>
<img src="../../images/beh-2015-sequencing-pareto-front.jpg" width=70% alt="Pareto-front between PV of GHG emissions and PV of costs for the seven uncertain scenarios.">
<div class=imgcredit>Figure 2 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
<p>
<img src="../../images/beh-2015-sequencing-optimal-sequences.jpg" width=70% alt="Details for the portfolio of optimal sequence plans over the planning horizon.">
<div class=imgcredit>Table 4 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
</li>
</ol>
</p>
<p> Step 2: Sensitivity analysis. 
<ul>
<li> Sobol's method was used for senstivity analysis
<li> The performance measures were the objectives, reliability (a measure of how often supply exceeds or equals demand) and vulnerability (a measure of demand shortfall). </li> 
<li> The sensitivity analysis was repeated 20 times using stochastic daily rainfall data for the 40 year planning timeframe. The results were averaged and presented as box-and-whisker plots (figure 3).
<p>
<img src="../../images/beh-2015-sequencing-sensitivity-analysis.jpg" width=70% alt="Sensitivity analysis of the optimal sequence plans to uncertain variables. The variation around the mean is displayed for PV costs, PV GHG emissions, relibility and vulnerability.">
<div class=imgcredit>Figure 3<a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
Sequence plans with higher mean values for PV costs and PV GHG emissions are generally more robust with respect to reliability and vulnerability. There is a trade-off betwen costs and GHG emissions on the one hand and water security (reliability and vulnerability metrics) on the other hand. Sequences 18-30 have greater reliability and less vulnerability because of early implementation of the 50 GL desalination plant expansion. Sequence 17 has less vulnerability compared to sequences 1-16 because of early implementation of stormwater schemes to reduce costs and GHG emissions.
</li>
<li> Analysis of the Sobol sensitivity indices shows that PV costs and PV GHG emissions are primarily influenced by the discount rate, with a smaller influence from population growth and climate change. Reliability and vulnerability are influenced by population growth and climate change.</li>
</ul>
</p>
<p> Step 3: Selection of optimal sequence plan. An informal process is used, based on decision-makers' definition of acceptable conditions  and appraisal of the following factors: <ul>
<li> the trade-offs between the average values and variation for the four objectives (i.e., PV costs, PV GHG emissions, reliability, vulnerability) </li>
<li> the relative contribution of uncertain variables (i.e., population, climate change, discount rate) to the performance results and potential for those variables to be managed </li>
<li> the maximum vulnerability should be less than 27% (corresponding to what can be achieved with temporary water restrictions) </li>
<li> the degree of adaptability </li>
</ul>
Based on figure 3, sequences 1-16 are excluded because the maximum vulnerability is greater than 27%. Of the remaining sequences, sequence 17 has slightly lower reliability but also lower PVs costs and GHG emissions because the the 50 GL desalination expansion occurs in 2050 instead of 2030 as in sequences 18-30. The later implementation of the desalination expansion also means sequence 17 has greater adaptability. Demand restrictions have the potential to manage shortfalls due to lower reliability. Therefore, sequence 17 is selected.
</p>
reference: >
  Beh EHY, Maier HR, Dandy GC (2015). <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Scenario driven optimal sequencing under deep uncertainty</a>. Environmental Modelling & Software 68, 181–195. doi: 10.1016/j.envsoft.2015.02.006. [<a href="https://digital.library.adelaide.edu.au/dspace/bitstream/2440/90636/2/hdl_90636.pdf">Open Access version</a>]
  <p>Also see <a href="https://watermodelling.org/news/event-summary-coping-with-multiple-plausible-futures-in-the-face-of-climate-change">presentation for the Queensland Water Modelling Network</a>.</p>
  <p>Also see <a href="../examples/beh-2015-multiobjective/"> Beh et al., 2015, Adaptive, multiobjective optimal sequencing approach for urban water supply augmentation under deep uncertainty </a> </p>
---
