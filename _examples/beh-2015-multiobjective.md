---
layout: under-construction
title: Adaptive, multiobjective optimal sequencing approach for urban water supply augmentation under deep uncertainty
citation: (Beh et al., 2015)
permalink: /examples/beh-2015-multiobjective/
page_authors :
    - Caroline Rosello
page_reviewers :
excerpt: A multiobjective optimal sequencing analysis approach is used to assess the robustness, flexibility and cost-effectiveness of Pareto optimal water supply augmentation options over a 40 years planning horizon under population growth and climate change uncertainties. Sequences of actions with acceptable outcomes against future scenarios, for successive discrete time periods (10 years staging interval), could be identified for different realities (i.e., milder impact on water supply and severe impact on water supply). 
approach: >
<p>
The approach aims at optimising a set of objectives to ensure water supply security in the face of future scenarios and to help decision makers to explore the impact of deep uncertainty on <a href="../theory/pareto-optimality/">Pareto-optimal </a> sequences of water supply enhancement options. The idea is not to identify a best plan but to consider a portfolios of <a href="../theory/adaptative-pathways/"> adaptative pathways</a>.
</p>
<p>
Three steps are involved, as presented in figure 1:
<p>
<img src="../../images/beh-2015-multipleobjectives-fig1.jpg" width=70% alt="Representation of the multiobjective optimal sequencing approach. Three steps are described: 1) Identification of portfolios of optimal supply enhancement plans, 2) Portfolio plans' performance evaluation, 3) Selection of water supply enhancement actions to be implemented. Each of these step are repeated over the planning horison (e.g., 40 years) for different decision stages (e.g. every 10 years).">
<div class=imgcredit>Figure 1 <a href="https://doi.org/10.1002/2014WR016254">Beh et al. 2015</a></div>
</p>
<ol>
<li> Identification of a portfolio of optimal water supply augmentation (enhancement) sequence plans over the entire planning horizon. This step involves four stages:
<ol>
<li> The definition of objectives, planning horizon, staging interval, water supply options and constraints (figure 1, 1a).</li>
<li> The definition of uncertain variables (i.e., variables affecting the supply and/or the demand) and assiated range of values (figure 1, 1b).</li>
<li> The definition of scenarios for the development of optimal sequences (i.e. continuum of conditions from the best set of conditions to the worst) (figure 1, 1c). These scenarios should be developed and analysed in collaboration with stakeholders. </li>
<li> Following the problem formulation, Pareto-optimal sequences over the entire planning horizon are identified, based on the consideration of sequences maximising the benefits from capital and operating values over the different objectives, decision stages and water supply options, with considering the defined constraint(s). Multiobjective evolutionary algorithms (MOEAs) could be used for that purpose. The result is the visualisation of Pareto front for the sequence plans for each defined scenario. Each sequence on the Pareto front constitute the desired portfolio of optimal water supply enhancement plans (figure 1, 1d). </li>
</ol>
</li>
<li> Assessment of performance of portfolio of optimal sequence plans. This step involves two stages:
<ol>
<li> The evaluation of the robustness and flexibility of groups of optimal sequence plans for each successive decision stage (figure 1, 2a). 
<ul>
<li> The robustness at a current decision stage is computed as the ratio of the number of scenarios for which a sequence group perform acceptably over the total number of uncertain scenarios. Acceptable thresholds are case dependent and set by decision makers.</li>
<li> The flexibility at a current decision stage for sequence group is estimated based on the ratio of the number of scenarios for which a sequence group of water supply enhancement actions is optimal over the total number of uncertain scenarios - a value of 1 meaning that the fixed solution is part of all optimal sequences for every future scenarios. </li>
</ul>
</li>
<li> Assessment of the performance of each sequence group against each scenario when varying identified objectives' values for different successive decision stages. The median and range are used to evaluate the central tendency and range of outcomes (figure 1, 2b). </li>
</ol>
</li>
<li> Selection of water supply augmentation options based on the objectives results for the different sequence groups over the planning horizon. The results are displayed as value path plots and values are standardised between 0 and 1 to be compared (0 representing the worst performance and 1 the best). This selection is decision-makers' dependent and representative of preferences for different trade-offs among the different objectives. According to the number of objectives and sequence groups to evaluate, informal methods or formal processes (e.g., multi-criteria decision analysis, scenario discovery) could be used. </li>
</ol>
</p>
problem_definition: >
<p> 
Adelaide is the capital city of South Australia and home to around 1.3 million inhabitants. The climate is described as Mediterranean and Adelaide is considered as one of the driest metropole around the world. The Southern Region of the Adelaide Water Supply System (WSS) supports around 50% of the metropolitan water demand. The supply is ensured by three reservoirs: Myponga, Mount Bold and Happy Valley. Mount Bold reservoir is particularly important for the metropolitan area and relies on water inflow from local catchments anf from water transfers from the River Murray (650 GL/year based on a five year rolling license). The metropolitan region is home to 1.3 million people, with an estimate annual water demand for domestic and industrial uses of 163 GL in 2008.
</p>
<p> 
The sustainability of Adelaide metropolitan water supply is questioned in the face of population growth and climate change (especially changes in rainfalls and temperatures) and means to increase the supply are required to cope with future challenges. Plausible solutions, identified by the Government of South Australia, consist, in addition to the three existing storages, to consider desalination, diverse storm water harvesting schemes and household rainwater tanks.
</p>
<p>
The appraoch is used to evaluate the robustness and adaptive capability of different sequence of water supply augmentation options with considering multiple objectives and the impact of uncertainty on optimal sequence plans. Figure 2 provides a summary of the variables and constraints used in the case study.
<p>
<img src="../../images/beh-2015-multipleobjectives-fig2.jpg" width=70% alt="Summary of the experimental approach followed in the Adelaide case study.">
<div class=imgcredit>Figure 2 <a href="https://doi.org/10.1002/2014WR016254">Beh et al. 2015</a></div>
</p>
<ol>
<li> Steps 1a to 1c are based on the formulation of the problem and definition of scenarios to consider. In addition to scenarios (i.e., combination of values for the three uncertain variables defining a continuum in conditions from the best to the worst possible ones), two 'realities' have been considered by the authors depicting moderate and severe impacts on the water supply. These realities depict assumed known pathways for population growth and climate change impacts up to 2050. </li>
<li> Step 1d consists of the determination of the portfolio of optimal sequence plans. This portfolio is based on the minimisation of the costs associated with the two objective functions (i.e., PV (present value) of economic costs and PV of GHG emissions)). The decision variables for the objective functions are provided in table 1. WaterCress (Water Community Resource Evaluation and Simulation System) model was used to calculate the objective functions and the Water System Multiobjective Genetic Algorithm was used to identify optimal solutions. The Pareto front for the different objectives, at different decision points, could be represented for the two objective functions. These solutions represent the set of optimal sequence plans. 
<p>
<img src="../../images/beh-2015-multipleobjectives-t1.jpg" width=70% alt="Details of the nine decision variable formulation. Decision variables consist of three desalination plants options, two household rainwater tanks ones and four storm water harvesting schemes.">
<div class=imgcredit>Table 1 <a href="https://doi.org/10.1002/2014WR016254">Beh et al. 2015</a></div>
</p>
</li>
<li> Step 2 is based on the evaluation of the options for the different optimal sequence plans identified in step 1d. The Pareto solutions are first grouped based on their consideration of the same augmentation options at a current staging interval. These groups are then evaluated for their robustness and flexibility (2a) and median and range for the PV costs and PV GHG emissions (2b) over all scenarios. The results for the different groups, at a decision point, are illustrated in figure 3.
<p>
<img src="../../images/beh-2015-multipleobjectives-fig3.jpg" width=70% alt="Results of the sequence groups performance for decision stage 1. The value path of the selected option for stage 1 is highlighted in red">
<div class=imgcredit>Figure 3 <a href="https://doi.org/10.1002/2014WR016254">Beh et al. 2015</a></div>
</p>
</li>
<li> Step 3 is based on the selection of a path for a decision point (figure 3). The selected solution is fixed and the process (step 2 and step3) is re-iterated until covering the whole planning horizon.</li>
</ol>
</p>
<p> The results from the overall approach are displayed in table 2. The numbers are indicative of the decision stage in which a specific option need to be implemented. For example, for both realities, implementing a storm water harvesting scheme at Brownhill and Keswick Creek is required in 2010.
<p>
<img src="../../images/beh-2015-multipleobjectives-fig4.jpg" width=70% alt="Summary of the optimal sequence plans for the two simulated realities considered in the Adelaide water supply enhancement case study.">
<div class=imgcredit>Figure 4 <a href="https://doi.org/10.1002/2014WR016254">Beh et al. 2015</a></div>
</p>
It is noteworthy that both realities will have significant different sequences of water supply enhancement options to cope with future conditions. In addition, the costs of adaptation, in terms of economic and GHG emissions, is expected to be higher in reality 2 (i.e., more severe impacts of the water supply) than in reality 1.
</p>
<p> Future improvements for the approach involve the consideration of:
<ul>
<li> formal approaches (e.g., scenario discovery) to scenario development and identification of solutions to implement to deal with more complex problems and real-life applications.</li>
<li> dynamic changes in the problem formulation over the planning horizon to consider societal preferences. </li>
<li> a solution mathematical optimality when considering all scenario simultaneously and not individually - an optimal solution for an individual scenario being potentially sub-optimal when considering all scenarios simultaneously.</li>
<li> the approach in other water resources schedulling and sequencing problems. </li>
</ul>
</p>
reference: 
  <p> Beh, E. H. Y., Maier, H. R., & Dandy, G. C. (2015). <a href="https://doi.org/10.1002/2014WR016254">Adaptive, multiobjective optimal sequencing approach for urban water supply augmentation under deep uncertainty. </a> Water Resources Research, 51(3), 1529–1551. 
  <p>Also see <a href="https://watermodelling.org/news/       event-summary-coping-with-multiple-plausible-futures-in-the-face-of-climate-change">presentation for the Queensland Water Modelling Network</a>.</p>
---
