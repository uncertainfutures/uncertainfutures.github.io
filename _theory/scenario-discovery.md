---
layout: concept
title: Scenario discovery
permalink: /theory/scenario-discovery/
excerpt: Scenario discovery involves identifying policy-relevant plausible future scenarios as a form of vulnerability analysis or to identify a limited number of future scenarios to focus on
purpose: >
  <p>Scenario discovery is a form of <a href=”../../vulnerability-analysis”>vulnerability analysis</a>. It is a participatory computer-assisted scenario development approach used to summarise multiple plausible future scenarios and identify scenarios relevant to the design and choice of policies. Such policy relevant scenarios consist of sets of future states of the world representing vulnerabilities for the proposed policy i.e., either conditions in which a policy may fail to meet its performance goals or in which its performance deviates significantly from the optimum policy [1].</p>
  <p>Scenario discovery algorithms aim to capture sets of uncertain model input parameter values:<ul>
    <li>with a high proportion of policy-relevant cases (high coverage),</li>
    <li>primarily relevant to policy cases (high density i.e., that minimise decision-irrelevant inputs within a region), and</li> 
    <li>easy to understand (high interpretability i.e., describing relevant parameter dimensions with influential input parameters for an output) [2].</li>
  </ul></p>
requirements: >
  Requirements:
  <ol><li>One or more computer simulation models to generate uncertain model input parameters datasets,</li>
  <li>Statistical and/or data-mining algorithms to identify candidate scenarios,</li> <li>Diagnostic tools for evaluating the significance of the parameter constraints proposed by scenario discovery algorithms [1]</li></ol>
decomposition: >
  <p>Three steps are involved in scenario discovery: database generation, algorithm selection, and scenario assessment and selection.</p>
  <b>Database generation</b><br/>
    Database generation with a simulation model links policy actions to consequences of interest, with each scenario described by a vector representing a particular point in a dimensional space of uncertain model input parameters. 
    <p>A threshold performance level is applied to select a set of cases of interest, using some policy-relevant criteria [1]. To avoid aggregation of performance criteria, scenario discovery has also been applied to multiple performance metrics separately, yielding a set of scenarios, explicitly describing the sensitivity of scenario discovery results to the choice of different metrics [12].</p>
    <p>The system model of interest is sampled based on the application of an experimental design over the uncertain inputs for a candidate strategy, e.g. using the <a href="../../tools/emaworkbench/">Exploratory Modelling & Analysis Workbench</a> [11]. Two approaches to sampling include [13]: </p>
    <ul>
    <li> static input-oriented sampling (e.g., Monte Carlo, Latin Hypercube sampling, criterion based sampling) which consider the input space without considering the resulting output space.</li>
    <li> adaptive output-oriented sampling, which considers the resulting output space and a dynamical approach to complex issues or system non-linearities, e.g. using a roughness measure to characterise the dynamic complexity of simulation runs and direct the adaptive sampling process to potentially areas of interest in the output space [13]</li>
    </ul>
    <p>To speed up database generation, scenario discovery algorithms can also be used with "surrogate models" or "meta-models" that provide a faster running model that is trained to replicate the relationship between inputs and outputs, e.g. with PRIM using "rule extraction" [4].</p>
    <p><b>Algorithm selection</b></p>
    One or more algorithms are applied to identify candidate scenarios. Each algorithm can define groups of scenarios in their own way.<ul>
        <li><a href="../../theory/PRIM/">PRIM (Patient Rule Induction Method)</a> identifies "boxes" in parameter space, i.e. bounds on parameter values within which scenarios meet some pre-defined criteria. PRIM is a bump-hunting (activity region finding) algorithm used to achieve a desired balance between coverage, density and interpretability.</li>
        <li>PCA-PRIM and CPCA-PRIM [3] don't use the original parameters, but instead identify boxes using orthogonal rotations obtained through principal component analysis (PCA), optionally with constraints to improve interpretability. This may improve density and coverage of boxes.</li>
        <li><a href="../../theory/CART/">CART (Classification and Regression Tree)</a> is a classification algorithm that typically provide outputs as a decision tree. The algorithm successively partitions the input space with a sequence of binary splits. Discovered scenarios are therefore described by a sequence of classification rules.
        </li>
        <li>Behaviour-based scenario discovery [10] considers model dynamics over time based on the use of time series clustering during the scenario discovery algorithms' identification stage to identify common macro-level behaviours in the ensemble of output time series. Two interests of the approach are:<ol>
          <li> to induce regions in the input parameter space associated with model behaviours over time rather than considering a static state of the model.</li>
          <li> to consider every output in an ensemble included in a cluster and mapped to a region (box) in the input parameter space, rather than a small subset.</li>
        </li>
        </ul>
        <p><b>Assessment and selection of scenarios</b></p>
        The user assesses scenario quality using diagnosis tools, including measures of coverage, density and interpretabiliy, to improve understanding of the identified scenarios and evaluate the ability of the algorithm to characterise cases of interest in the database. Diagnostic tools include [1]:<ul>
            <li>Resampling test, to evaluate the reproducibility of the scenario discovery algorithm results.</li>
            <li>Quasi-p-value test, to estimate the likelihood that algorithm constrains some parameter by chance.</li>
            </ul>
        <p>Selection of criteria may be performed informally (including drawing on diagnosis metrics) or formally, e.g. based on the consideration of utility scores for failure scenarios [1].
        </p>
tools:
  - slug: sdtoolkit
    name: sdtoolkit
    description: an R package implementing PRIM specifically for scenario discovery
  - slug: emaworkbench
    name: Exploratory Modelling and Analysis (EMA) Workbench
    description: a Python package that includes a scenario discovery oriented implementation of PRIM.
also_see:
  - permalink: /theory/MORDM/
    name: Multi-Objective Robust Decision Making (MORDM)
    description: a method for robust decision making that uses scenario discovery
  - permalink: /theory/DAPP/
    name: Dynamic Adaptive Policy Pathways (DAPP)
    description: a method that combines <a href="../adaptive-pathways/">adaptive pathways</a> and Dynamic Adaptive Planning (DAP), and can use scenario discovery to identify tipping points.
further_reading:
  - >
    Bryant BP, Lempert RJ (2010) <a href="https://dx.doi.org/10.1016/j.techfore.2009.08.002">Thinking inside the box: A participatory, computer-assisted approach to scenario discovery.</a> Technological Forecasting and Social Change, 77(1), 34–49. doi:10.1016/j.techfore.2009.08.002
references:
  - >
    [1] Bryant BP, Lempert RJ (2010) <a href="https://dx.doi.org/10.1016/j.techfore.2009.08.002">Thinking inside the box: A participatory, computer-assisted approach to scenario discovery.</a> Technological Forecasting and Social Change, 77(1), 34–49. doi:10.1016/j.techfore.2009.08.002
  - >
    [2] Lempert, R. J., Bryant, B. P., & Bankes, S. C. (2008). Comparing algorithms for scenario discovery. RAND, Santa Monica, CA.
  - >
    [3] Dalal, S., Han, B., Lempert, R., Jaycocks, A., & Hackbarth, A. (2013) <a href="https://doi.org/10.1016/j.envsoft.2013.05.013">. Improving scenario discovery using orthogonal rotations.</a> Environmental Modelling & Software, 48, 49–64.
  - >
    [4] Arzamasov, V., & Böhm, K. (2019). <a href="https://arxiv.org/pdf/1910.01713v1.pdf">Scenario Discovery via Rule Extraction</a>. ArXiv Preprint ArXiv:1910.01713.
  - >
    [10] Steinmann, P., Auping, W. L., & Kwakkel, J. H. (2020).<a ref="https://doi.org/10.1016/j.techfore.2020.120052"> Behavior-based scenario discovery using time series clustering.</a> Technological Forecasting and Social Change, 156, 120052.
  - >
    [11] Kwakkel, J. H. (2017). <a href="https://doi.org/10.1016/j.envsoft.2017.06.054">The Exploratory Modeling Workbench: An open source toolkit for exploratory modeling, scenario discovery, and (multi-objective) robust decision making. </a> Environmental Modelling & Software, 96, 239–250.
  - >
    [12] Shortridge, J. E., & Guikema, S. D. (2016).<a href="https://doi.org/10.1111/risa.12582"> Scenario Discovery with Multiple Criteria: An Evaluation of the Robust Decision-Making Framework for Climate Change Adaptation.</a> Risk Analysis, 36(12), 2298–2312.
  - >
    [13] Islam, T., & Pruyt, E. (2016). <a href="https://doi.org/10.1016/j.envsoft.2015.09.014">Scenario generation using adaptive sampling: The case of resource scarcity. </a> Environmental Modelling & Software, 79, 285–299.
  - >
    [14] Lempert, R. J., & Groves, D. G. (2010). <a href="https://doi.org/10.1016/j.techfore.2010.04.007">Identifying and evaluating robust adaptive policy responses to climate change for water management agencies in the American west. </a>Technological Forecasting and Social Change, 77(6), 960–974.
  - >
    [15] Rozenberg, J., Guivarch, C., Lempert, R., & Hallegatte, S. (2014).<a href="https://doi.org/10.1007/s10584-013-0904-3"> Building SSPs for climate policy analysis: A scenario elicitation methodology to map the space of possible future challenges to mitigation and adaptation. </a> Climatic Change, 122(3), 509–522.
  - >
    [16] Greeven, S., Kraan, O., Chappin,  E. & Kwakkel, J. H. (2016). <a href="https://doi.org/10.18564/jasss.3134"> The Emergence of Climate Change Mitigation Action by Society: An Agent-Based Scenario Discovery Study. </a> Journal of Artificial Societies and Social Simulation, 19(3), 9.
  - >
    [17] Gerst, M. D., Wang, P., & Borsuk, M. E. (2013). <a href="https://doi.org/10.1016/j.envsoft.2012.09.001">Discovering plausible energy and economic futures under global change using multidimensional scenario discovery. </a> Environmental Modelling & Software, 44, 76–86.
  - >
    [18] Matrosov, E. S., Woods, A. M., & Harou, J. J. (2013). <a href="https://doi.org/10.1016/j.jhydrol.2013.03.006">Robust Decision Making and Info-Gap Decision Theory for water resource system planning. </a> Journal of Hydrology, 494, 43–58.
  - >
    [19] Watson, A. A., & Kasprzyk, J. R. (2017). <a href="https://doi.org/10.1016/j.envsoft.2016.12.001">Incorporating deeply uncertain factors into the many objective search process. </a> Environmental Modelling & Software, 89, 159–171.
  - >
    [20] Kasprzyk, J. R., Nataraj, S., Reed, P. M., & Lempert, R. J. (2013). <a href="https://doi.org/10.1016/j.envsoft.2012.12.007">Many objective robust decision making for complex environmental systems undergoing change.</a> Environmental Modelling & Software, 42, 55–71.
  - >
    [21] Ramm, T. D., Watson, C. S., & White, C. J. (2018). <a href="https://doi.org/10.1016/j.compenvurbsys.2018.01.002">Describing adaptation tipping points in coastal flood risk management.</a> Computers, Environment and Urban Systems, 69, 74–86.
  - >
    [22] Groves, D. G., Knopman, D., Lempert, R. J., Berry, S. H., & Wainfan, L. (2008). <a href="https://www.rand.org/pubs/technical_reports/TR505.html">Presenting Uncertainty About Climate Change to Water-Resource Managers: A Summary of Workshops with the Inland Empire Utilities Agency. </a> RAND Corporation.
  - >
    [23] Groves, D. G., Lempert, R. J., Knopman, D., & Berry, S. H. (2008). <a href="https://www.rand.org/pubs/documented_briefings/DB550.html">Preparing for an Uncertain Future Climate in the Inland Empire: Identifying Robust Water-Management Strategies.</a> RAND Corporation.
examples:
  - Climate adaptation e.g.,[12],[14],[23]
  - Climate mitigation e.g.,[15],[16],[17]
  - Water resources management e.g.[18],[19],[22]
  - Application to robust decision making (RDM) and MORDM e.g.,[19],[20]
  - Application to agent based modelling e.g., [16]
  - Application to DAPP and identification of tipping points [21]
---
