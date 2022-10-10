---
layout: case-study
title: Sequencing water supply options in Adelaide
citation: (Beh et al. 2015)
permalink: /examples/beh-2015-sequencing/
page_authors:
  - Caroline Rosello
  - Joseph Guillaume
page_reviewers: Leila Noble
excerpt: The analysis identifies optimal sequences for adding to an urban water supply for a set of scenarios with differing climate change, population and discount rates. Sensitivity analysis shows how the performance of each sequence for multiple criteria varies across the scenarios, and which uncertain variables have greater influence, to inform selection of an optimal sequence plan. 
approach: >
  <p> 
  The approach consists of the evaluation of the robustness of sequences of water supply augmentation options (i.e., additional options to support current water supplies) over a planning horizon to cope optimally with future conditions. The sequence of options form an <a href="../../theory/adaptation-pathways/">adaptation pathway. As a <a href="../../theory/robust-decision-making/">robust decision making</a> approach, the aim is to identify solutions able to perform well under different future conditions.
  </p>
  <p>
  <img src="../../images/beh-2015-sequencing-approach.jpg" width=70% alt="Conceptual representation of the scenario driven optimal sequencing approach. Three steps are involved: 1) the generation of the portfolio of optimal sequences under various future conditions, 2) sensitivity analysis to evaluate the robustness of the optimal sequences and identify influential critical risk factors, 3) the selection of the optimal sequence for implementation.">
  <div class=imgcredit>Figure 1 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
  </p>
  <p>
  Problem framing involves defining the objectives, the planning horizon, the intervals at which new water supply options may be added, the water supply options, and constraints. Stakeholders should be involved. 
  </p>
  <p>
  Following the problem framing stage, there are three steps:
  <ol>
  <li> <i>Generation of a portfolio of optimal sequences</i>:
    <ol style="list-style-type:lower-roman;">
      <li> defining uncertain variables and their plausible ranges over the planning horizon </li>
      <li> defining plausible future scenarios with different combinations of values of uncertain variables </li>
      <li> generating <a href="../../theory/pareto-optimality/">Pareto-optimal </a> sequences for each scenario with respect to pre-defined constraints for the different objective functions. This step may involve the use of multi-objective evolutionary algorithms (MOEAs). </li>
    </ol>
  <li> <i>Sensitivity analysis</i>: evaluating the performance the Pareto-optimal sequences under a range of future conditions and the relative contribution of uncertain variables to the performance.
    <ul>
      <li> Performance metrics should include multiple specified objectives and additional measures such as <a href="../../theory/robustness-metrics/">reliability, resilience, or vulnerability metrics</a>. </li>
      <li> To account for variability in system states, the sensitivity analysis should be repeated for different system states for each optimal sequence. </li>
    </ul>
  </li>
  <li> <i>Selection from the optimal sequences</i>, which should consider: 
    <ul>
      <li> trade-offs between performance objectives' absolute (e.g. average) values and variability </li>
      <li> the relative contribution of uncertain variables to performance variability and consideration of the feasibility of managing those variables </li>
      <li> the degree to which additional interventions could help manage constraint violations</li>
      <li> the degree of adaptability of the different optimal sequences, noting that sequences that are similar at early stages provide greater adaptability </li>
    </ul>
  </li>
  </ol>
  </p>
problem_definition: >
  <p>
  Adelaide, the capital of South Australia, is one of the driest capital cities worldwide. It has a population of about 1.3 million with an estimated mean annual water consumption of 163 GL in 2008. The southern Adelaide water supply system (WSS) is the major water supplier, delivering 50% of the metropolitan water demand. Three reservoirs support the system supply. 
  </p>
  <p> 
  To cater for the projected water demand due to population growth and climate change, water supply augmentation sources considered include a desalination plant, diverse stormwater harvesting schemes and household rainwater tanks.
  </p>
  <p> 
  The problem formulation includes: 
  <ul>
    <li> Objectives: minimisation of the PV (present value) costs and PV greenhouse gas (GHG) emissions. </li>
    <li> Constraints: the supply capacity is greater or equal to the demand.</li>
    </li>
    <li> Decision variables: 
    <ul>
      <li> Planning horizon of 40 years </li>
      <li> Decision points every 10 years (staging interval) </li>
      <li> Current and future water supply sources are provided in Table 1, and the decision variable is the year in which to implement the option (Table 2). Not all of these options are independent, e.g., a specific desalination plant or stormwater harvesting scheme can only be selected once.</li>
    </ul>
  </ul>
  <p>
  <a href="../../images/beh-2015-sequencing-supply-details.jpg" target="_blank"><img src="../../images/beh-2015-sequencing-supply-details.jpg" width=100% alt="Details of the different water supplies to be evaluated, including capital and operating costs."></a>
  <div class=imgcredit>Table 1 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
  </p>
  <p>
  <img src="../../images/beh-2015-sequencing-decision-variables.jpg" width=70% alt="Details of the nine decision variables including decision point ranges from current time (0) to the end of the planning horizon (5) or based on household tank size (from 1kL to 10 kL.">
  <div class=imgcredit>Table 2 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
  </p>
  
  Checking constraints and calculation of objectives uses a simulation of the water supply using WaterCress (Water-Community Resource Evaluation and Simulation System).  
  
  </p>
  <p> <b>Step 1: Determination of the portfolio of optimal sequences</b> 
  <p>Seven scenarios are considered across three uncertain variables (Table 3). Climate change impact is represented in terms of rainfall and evaporation. Discount rates are applied to capital and operation costs and GHG emissions:
  <p>
  <img src="../../images/beh-2015-sequencing-scenarios.jpg" width=70% alt="Details for the seven scenarios considered.">
  <div class=imgcredit>Table 3 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
  </p>
  These scenarios are representative of a continuum in future conditions from the best possible future conditions (scenario 1) to the worst possible (scenario 7) in terms of population and climate changes. The discount rate is kept constant here because it does not directly influence future water supply and demand.
  </p>
  <p>The WaterCress simulation model is used to estimate the supply, demand and costs and GHG emissions for the water supply systems under the seven scenarios, over the planning horizon, with consideration of constraints. The Water System Multiobjective Genetic Algorithm (WSMGA) is used to generate Pareto-optimal sequences. Pareto fronts are displayed in Figure 2, with selected sequences shown in Table 4.</p>
  <p>
  <img src="../../images/beh-2015-sequencing-pareto-front.jpg" width=70% alt="Pareto-front between PV of GHG emissions and PV of costs for the seven uncertain scenarios.">
  <div class=imgcredit>Figure 2 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
  </p>
  <p>
  <a href="../../images/beh-2015-sequencing-optimal-sequences.jpg" target="_blank"><img src="../../images/beh-2015-sequencing-optimal-sequences.jpg" width=100% alt="Details for the portfolio of optimal sequence plans over the planning horizon."></a>
  <div class=imgcredit>Table 4 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
  </p>
  </p>
  <p><b>Step 2: Sensitivity analysis</b></p>
  <p> Sobol's method was used for sensitivity analysis, providing sensitivity indices representing the proportion of variance in performance measures attributable to changes in single and combinations of uncertain variables.</p>
  <p> The performance measures were the objectives, reliability (a measure of how often supply exceeds or equals demand) and vulnerability (a measure of demand shortfall). </p> 
  <p> The sensitivity analysis was repeated 20 times using stochastic daily rainfall data for the 40 year planning timeframe. </p>
  <p> Analysis of the Sobol sensitivity indices shows that PV costs and PV GHG emissions are primarily influenced by the discount rate, with a smaller influence from population growth and climate change. Reliability and vulnerability are influenced by population growth and climate change.</p>
  <p>Performance of optimal sequence plans across uncertain variables is presented as box-and-whiskers plots displaying the variation of the average values (over the stochastic rainfall realisations) (Figure 3).</p>
  <p>
  <a href="../../images/beh-2015-sequencing-sensitivity-analysis.jpg" target="_blank"><img src="../../images/beh-2015-sequencing-sensitivity-analysis.jpg" width=100% alt="Sensitivity analysis of the optimal sequence plans to uncertain variables. The variation around the mean is displayed for PV costs, PV GHG emissions, relibility and vulnerability."></a>
  <div class=imgcredit>Figure 3 <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Beh et al. 2015</a></div>
  </p>
  <p>
  Sequence plans with higher mean values for PV costs and PV GHG emissions are generally more robust with respect to reliability and vulnerability. There is a trade-off between costs and GHG emissions on the one hand and water security (reliability and vulnerability metrics) on the other hand. Sequences 18-30 have greater reliability and less vulnerability because of early implementation of the 50 GL desalination plant expansion. Sequence 17 has less vulnerability compared to sequences 1-16 because of early implementation of stormwater schemes to reduce costs and GHG emissions.
  </p>
  <p><b>Step 3: Selection of optimal sequence plan</b></p>
  <p>An informal process is used, based on decision-makers' definition of acceptable conditions and appraisal of the following factors: 
  <ul>
    <li> the trade-offs between the average values and variation for the four objectives, i.e., PV costs, PV GHG emissions, reliability, vulnerability </li>
    <li> the relative contribution of uncertain variables (i.e., population, climate change, discount rate) to the performance results and potential for those variables to be managed </li>
    <li> the maximum vulnerability should be less than 27% - corresponding to what can be achieved with temporary water restrictions </li>
    <li> the degree of adaptability </li>
  </ul>
  Based on Figure 3, sequences 1-16 are excluded because the maximum vulnerability is greater than 27%. Of the remaining sequences, sequence 17 has slightly lower reliability but also lower PV costs and GHG emissions because the the 50 GL desalination expansion occurs in 2050 instead of 2030 as in sequences 18-30. The later implementation of the desalination expansion also means sequence 17 has greater adaptability. Demand restrictions have the potential to manage shortfalls due to lower reliability. Therefore, sequence 17 is selected.
  </p>
reference: >
  Beh EHY, Maier HR, Dandy GC (2015). <a href="https://doi.org/10.1016/j.envsoft.2015.02.006">Scenario driven optimal sequencing under deep uncertainty</a>. Environmental Modelling & Software 68, 181–195. doi: 10.1016/j.envsoft.2015.02.006. [<a href="https://digital.library.adelaide.edu.au/dspace/bitstream/2440/90636/2/hdl_90636.pdf">Open Access version</a>]
  <p>Also see <a href="https://watermodelling.org/news/event-summary-coping-with-multiple-plausible-futures-in-the-face-of-climate-change">presentation for the Queensland Water Modelling Network</a>.</p>
  <p>Also see <a href="../beh-2015-multiobjective/"> Beh et al., 2015, Adaptive, multiobjective optimal sequencing approach for urban water supply augmentation under deep uncertainty </a> </p>
---
