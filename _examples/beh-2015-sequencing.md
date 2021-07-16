---
layout: under-construction
title: Scenario driven optimal sequencing under deep uncertainty - Example of the Southern Adelaide Water Supply System
citation: (Beh et al. 2015)
permalink: /examples/beh-2015-sequencing/
page_authors:
  - Caroline Rosello
  - Joseph Guillaume
page_reviewers:
excerpt: The analysis identifies optimal sequences of additional water supply options for a set of scenarios with different climate change, population growth, and discount rates. Sensitivity analysis shows how performance of each plan varies across scenarios, and which variables have greater influence, to help inform selection of an optimal sequence plan.
approach: >
<p> 
The approach consists of the evaluation of the robustness of water supply management plans by considering the sequencing/schedulling of water supply enhancement options (i.e., additional options to support current water supplies) over a planning horizon to cope optimally with future conditions.
</p>
<p>
Prior to engaging in the analysis approach, the problem needs to be clearly defined and involves stakeholders participation.
</p>
<p>
Following the problem framing stage, three analytical steps are considered:
<p>
<img src="../../images/beh-2015-sequencing-approach.jpg" width=70% alt="Conceptual representation of the scenario driven optimal sequencing approach. Three steps qre considered: 1) the generation of the portfolio of optimal sequences under various future condtions, 2) sensitivity analysis to evaluate the robustness of the optimal sequences and identify influential critical risk factors, 3) the selection of the optimal sequence for implementation.">
<div class=imgcredit>Figure 1 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
<ol>
<li> Step 1 involves the generation of the portfolio of optimal sequences. As for <a href="../theory/robust-decision-making/"> robust decision making </a> approaches, this step aims at identifying plausible solutions able to perform differently under different future conditions. Three sub-steps are considered:
<ol>
<li> identifying uncertain variables and their plausible ranges over the planning horizon </li>
<li> identifying plausible future scenarios combining uncertain variables and asociated values </li>
<li> generating <a href="../theory/pareto-optimal/">Pareto-optimal </a> sequences for each scenario with respect to pre-defined constraints for the different objective functions. This step involves the use of multi-objective evolutionary algorithms (MOEAs) to generate the front of (near) Pareto-optimal solutions. </li>
</ol>
<li> Step 2 consists of the evaluation of the sensitivity of the Pareto-optimal sequences identified in step 1 to changes in conditions (values) for different uncertain future variables. This step also involves the identification of influential uncertain variables on the sensitivity analysis results. The identifcation of the nature of influential factors would be deterministic on the selection of adaptation measures. Points to consider are: 
<ul>
<li> Performance metrics should not be restricted to the specified objectives for a system but could include additional measures such as reliability, resilience, or vulnerability metrics. </li>
<li> To account for variability in system states, the sensitivity analysis should be repeated for each optimal sequences. </li>
</ul>
</li>
<li> Step 3 aims at decision-makers consideration of the performance of the different optimal sequences and selection based on their preferences. This choice is based on: <ul>
<li> trade-offs between performance objectives'absolute values (e.g., average) and variability </li>
<li> the relative contribution of uncertain variables to performance variability and consideration of the feasibility for managing such variables </li>
<li> the degree to which different constraint violations, due to uncertain factors and associated values, could be managed </li>
<li> the degree of adaptability of the different optimal sequences in terms of time of implementation; sequences with similar decisions at early stages of the planning horizon being considered more adaptible than the ones with different decisions. </li>
</ul>
</li>
</ol>
</p>
problem_definition: >
<p>
Adelaide, the capital of South Australia, is one of the driest metropolitan centre worldwide, having a Mediterranean climate. It is host of 1.3 million inhabitants with an estimated mean annual water consumption of 163 GL in 2008. The Southern Adelaide water supply system (WSS) is the major water supplier, with delivering 50% of the metropolitan water demand. Three reservoirs support the system supply: Myponga, Mount Bold and Happy Valley; Mount Bold being the major provider. 
</p>
<p> 
To catter for the projected water demand due to population growth and climate change in metropolitan Adelaide, different water supply augmentation sources have been considered including a desalination plant, diverse stormwater harvesting schemes and household rainwater tanks.
</p>
<p>
To support metropolitan supply under future population and climate uncertainties, the robustness of  sequences including existing supplies and potential supply augmentation options is evaluated against potential future conditions using the multiobjective, scenario driven optimal sequencing approach. 
</p>
<p> 
Prior to applying the approach, the problem needs to be framed which includes: <ul>
<li> Defining objectives and contraints: <ul>
<li> Objectives: minimisation of the PV (present value) costs and PV GHG emissions. </li>
<li> Constraints: the supply capacity is greater or equal to the demand.</li>
</ul>
</li>
<li> Defining decision variables: <ul>
<li> Planning horizon of 40 years </li>
<li> Decision points (staging interval): every 10 years </li>
<li> Current and future water supply sources estimates are provided in table 1. Not all of these options are independent of each others. For instance, i) once a desalination plant has been selected, it can't be selected again, or ii) one or more storm water harvesting schemes can be selected at any decision points but once only.
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
<li> The verification approach aims at checking the absence of violation of the defined constraint for the supply and that the generated combination of options satisfies the feasibility criteria for the desalination plant (e.g., the 50 GL/year expansion could only occur after implementation of the original 50 GL/year plant).</li>
<li> Objective functions are calculated based on the determination of PV capital and operation costs and PV GHG emissions for the water supply system, according to a chosen sequence plan. WaterCress (Water-Community Resource Evaluation and Simualtion System) is used for that purpose.</li>
</ul>
</li>
</ul>
</p>
<p> Step 1: Determination of the portfolio of optimal sequences. 
<ol>
<li> Uncertain variables are based on the consideration of population growth, rainfalls and evaporation rates, and discount rates for both capital and operation costs  (low-4% per year; medium-6% per year; high-8% per year) and GHG emissions (low-0% per year; medium-1.4% per year; high-3% per year). Values associated to these uncertain variables are used for the sensitivity analysis. </li>
<li> Seven scenarios are considered for identifying Pareto-optimal sequence plans (table 3):
<p>
<img src="../../images/beh-2015-sequencing-scenarios.jpg" width=70% alt="Details for the seven scenarios considered.">
<div class=imgcredit>Table 3 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
These scenarios are representative of a continuum in future conditions from the best possible future conditions (scenario 1) to the worst possible one (scenario 7) in terms of population and climate changes. The discount rate considered do not vary as not directly influential on future water supply security.
</li>
<li> The WaterCress simulation model is used to estimate the supply, demand and costs and GHG emissions for the water supply systems under the seven scenarios, over the planning horizon, with considering the defined constraints. To generate the sequences with Pareto-optimal results for the objective functions, the Water System Multiobjective Genetic Algorithm (WSMGA) is used. The Pareto-front sequences are displayed in figure 2 and are associated to the sequences in table 4.
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
<li> The Sobol's method was used to evaluate the global sensitivity of the objectives to uncertain variables. In addition, the reliability of the supply and the vulnerability of the demand to supply shortfall is estimated. </li> The analysis is repeated 20 times based on 20 sequences of 40 years daily stochastic rainfall sequences and the results of the sensitivity analysis are presented as average values over the 20 sequences. </li>
<li> Optimal sequence plans' performance to uncertain variables is presented as box-and-whiskers plots displaying the variation of the avarage values for the PV costs, PV GHG emissions, reliability and vulnerability (figure 3) 
<p>
<img src="../../images/beh-2015-sequencing-sensitivity-analysis.jpg" width=70% alt="Sensitivity analysis of the optimal sequence plans to uncertain variables. The variation around the mean is displayed for PV costs, PV GHG emissions, relibility and vulnerability.">
<div class=imgcredit>Figure 3<a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
</p>
Sequence plans with higher mean values for PV costs and PV GHG emissions are generally more robust with respect to reliability and vulnerability and are generally more effective to meet the demand for more extreme scenarios and under a wider range of plausible future conditions. The consideration of the trade-offs between costs and GHG emissions, on the one hand, and water security (reliability and vulnerability metrics), on the other hand, shows that actions influential on increased water security (from 18 onward) are associated to the early implementation of the 50 GL desalination plant expansion. Also, sequence 17 presents noticeable reduction in vulnerability compared to the sequences 1 to 16 due to earlier implementation of stormwater schemes to reduce costs and GHG emissions.
</li>
<li> In addition to evaluating the sensitivity of different optimal sequence plans to uncertain scenarios, key uncertain variables influential on the performance of the sequences could be identified based on the variability of the Sobol sensitivity indices. This analysis shows that PV costs and PV GHG emissions are directly influences by the discount rate, which is expected. In addition, the capital costs being fixed in a plan, changes in PV costs and PV GHG emissions due to population growth and climate change are associated to changes in operational costs, within the constraint conditions range (i.e., for the supply above or equa to the demand). Regarding reliability and vulnerability, changes in population and climate are the variables affecting the optimal sequence plans' peformance. </li>
</ul>
</p>
<p> Step 3: Selection of optimal sequence plan. An informal process is used, based on decision-makers' definition of acceptable conditions  and appraisal of the following factors: <ul>
<li> the trade-offs between the average values and variation for the four objectives (i.e., PV costs, PV GHG emissions, reliability, vulnerability) </li>
<li> the relative contribution of uncertain variables to the performance results and potential to be managed </li>
<li> the maximum vulnerability should be less than 27% </li>
<li> the degree of adaptability associated with different sequences </li>
</ul>
Based on figure 3, the sequences with an average value under 27% for the vulnerability are considered, leading to the exclusion of plans 1 to 16. Of the remaining sequences, the major tradeoffs occur between sequence 17 and all the other remaining sequences; the difference being the consideration of the 50 GL desalination plant expansion in 2050 for sequence 17 and earlier (2030) for the other sequences. Due to the potential for demand restrictions to manage population growth and associated demand, and lower PV costs and PV GHG emissions compared to the remaining sequences, the optimal sequence plan 17 is selected by the decision-makers. 
</p>
reference: >
  Beh EHY, Maier HR, Dandy GC (2015). <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Scenario driven optimal sequencing under deep uncertainty</a>. Environmental Modelling & Software 68, 181–195. doi: 10.1016/j.envsoft.2015.02.006. [<a href="https://digital.library.adelaide.edu.au/dspace/bitstream/2440/90636/2/hdl_90636.pdf">Open Access version</a>]
  <p>Also see <a href="https://watermodelling.org/news/event-summary-coping-with-multiple-plausible-futures-in-the-face-of-climate-change">presentation for the Queensland Water Modelling Network</a>.</p>
  <p>Also see <a href="../examples/beh-2015-multiobjective/"> Beh et al., 2015, Adaptive, multiobjective optimal sequencing approach for urban water supply augmentation under deep uncertainty </a> </p>
---
