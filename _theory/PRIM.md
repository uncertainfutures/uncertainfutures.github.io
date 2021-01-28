---
layout: concept
title: PRIM
permalink: /theory/PRIM/
excerpt: PRIM (Patient Rule Induction Method) is a "bump-hunting" algorithm that identifies "boxes" in the input parameter space containing scenarios matching specified properties.
purpose: >
  <p>PRIM can be used for <a href="../../theory/scenario-discovery/">scenario discovery</a> where the scenarios identified will be represented as bounds on parameter values within which scenarios meet some pre-defined criteria [1].</p>
  <p>Technically, PRIM identifies (boxes) within the input space in which the mean of the output is significantly higher that the mean of the output over the entire dataset (also described as regions of high density and high coverage) [1].</p>
requirements: >
  <p> To be operationalised, PRIM requires three main features [1]:<ul>
  <li>The generation of an input database consisting of results of a target performance objective obtained by running a simulation model for different input parameters (predictors), i.e. scenarios are defined by a set of parameter values.</li>
  <li>User selection of boxes that best balance criteria of coverage (i.e., ratio of relevant cases) and density (i.e., fraction of relevant points) for 'pasting'</li>
  <li>User selection of pasted boxes for the 'covering' stage </li>
  </ul></p>
decomposition: >
  <p> The PRIM iterative process consists of a peeling/pasting stage and a covering stage [5]<ol>
  <li> a primary 'peeling' stage in which PRIM algorithm explores the input space where the mean of the output is significantly different from the mean value over the entire dataset. Boxes of increasingly smaller and denser size are generated and successively removed from the input space forming a 'peeling trajectory' [5]. </li>
  <li> a 'pasting' stage (i.e., expansion of a box boundary to include some unnecessarily restricted dimensions) in which a user selects a peeling box that best balances objectives of high density and high coverage to be expanded [5]. 
  <p>The user typically selects boxes from graphical representations of the peeling trajectory, plotting the density of each box against its coverage [1].</p>
  </li>
  <li> a 'covering' stage in which data points within a chosen pasted box are removed from the dataset and the peeling/pasting process is repeated with the remaining data [5].</li></ol></p>
  <p> At the end of the process, the relevance of each parameter defining a specific box is  evaluated by users based on coverage, density and interpretability of results [1]. </p>
  <p>High coverage means that the box includes a higher proportion of the ‘interesting’ model scenarios available through parameter space. High density means that the box includes a higher proportion of ‘interesting’ cases relative to non-interesting ones [1]. High interpretability means that some bounds (expanded or not) may be more interpretable than others [1]. </p>
  <p>Variants of PRIM for identification of candidate boxes include:<ul>
    <li> PCA-PRIM and CPCA-PRIM [6] don't use the original parameters, but instead identify boxes using orthogonal rotations obtained through principal component analysis (PCA). This may improve density and coverage of boxes when parameters are correlated. Constrained PCA (CPCA) limits rotations to groups of similar parameters to improve interpretability.</li>
    <li> Application of a meta-model using rule extraction can reduce run times [7].</li>
    <li> Consideration of more than two classes in scenario discovery's identification of boxes and of integers or categories based on modified objective functions [9].</li>
# TODO: providing an example peeling trajectory
tools:
  - slug: sdtoolkit
    name: sdtoolkit
    description: an R package implementing PRIM specifically for scenario discovery
  - slug: emaworkbench
    name: Exploratory Modelling and Analysis (EMA) Workbench
    description: a Python package that includes a scenario discovery oriented implementation of PRIM.
  - slug: primpackage
    name: prim package
    description: non-interactive package written in R programming language [2]
  - slug: openMORDM
    name: openMORDM
    description: An R package for <a href="../MORDM/">many-objective robust decision making</a> [3]
also_see:
  - permalink: /theory/CART/
    name: CART
    description: A common alternative algorithm for scenario discovery
further_reading:
  - >
    Bryant BP, Lempert RJ (2010) <a href="https://dx.doi.org/10.1016/j.techfore.2009.08.002">Thinking inside the box: A participatory, computer-assisted approach to scenario discovery.</a> Technological Forecasting and Social Change, 77(1), 34–49. doi:10.1016/j.techfore.2009.08.002
references:
  - >
    [1] Bryant BP, Lempert RJ (2010) <a href="https://dx.doi.org/10.1016/j.techfore.2009.08.002">Thinking inside the box: A participatory, computer-assisted approach to scenario discovery.</a> Technological Forecasting and Social Change, 77(1), 34–49. doi:10.1016/j.techfore.2009.08.002
  - >
    [2] Duong, T. (2014). <a href="http://www.mvstat.net/tduong">Patient Rule Induction Method (PRIM) (1.0.15) </a>[Computer software].
  - >
    [3] Hadka, D., Herman, J., Reed, P., & Keller, K. (2015). <a href="https://doi.org/10.1016/j.envsoft.2015.07.014">An open source framework for many-objective robust decision making.</a> Environmental Modelling & Software, 74, 114–129.
  - >
    [4] Friedman, J. H., & Fisher, N. I. (1999). <a href="https://doi.org/10.1023/A:1008894516817">Bump hunting in high-dimensional data. </a>Statistics and Computing, 9(2), 123–143.
  - >
    [5] Lempert, R. J., Bryant, B. P., & Bankes, S. C. (2008). Comparing algorithms for scenario discovery. RAND, Santa Monica, CA.
  - >
    [6] Dalal, S., Han, B., Lempert, R., Jaycocks, A., & Hackbarth, A. (2013) <a href="https://doi.org/10.1016/j.envsoft.2013.05.013">. Improving scenario discovery using orthogonal rotations.</a> Environmental Modelling & Software, 48, 49–64.
  - >
    [7] Arzamasov, V., & Böhm, K. (2019). Scenario Discovery via Rule Extraction. ArXiv Preprint ArXiv:1910.01713.
  - >
    [8] Hadka, D., Herman, J., Reed, P., & Keller, K. (2015).<a href="https://doi.org/10.1016/j.envsoft.2015.07.014"> An open source framework for many-objective robust decision making.</a> Environmental Modelling & Software, 74, 114–129.
  - >
    [9] Kwakkel, J. H., & Jaxa-Rozen, M. (2016).<a href="https://doi.org/10.1016/j.envsoft.2015.11.020"> Improving scenario discovery for handling heterogeneous uncertainties and multinomial classified outcomes.</a> Environmental Modelling & Software, 79, 311–321.
  - >
    [10] Herman, J. D., Zeff, H. B., Reed, P. M., & Characklis, G. W. (2014).<a href="https://doi.org/10.1002/2014WR015338"> Beyond optimality: Multistakeholder robustness tradeoffs for regional water portfolio planning under deep uncertainty. </a> Water Resources Research, 50(10), 7692–7713.
  - >
    [11] Ren, K., Huang, S., Huang, Q., Wang, H., Leng, G., & Wu, Y. (2019). <a href="https://doi.org/10.1016/j.jhydrol.2019.124134">Defining the robust operating rule for multi-purpose water reservoirs under deep uncertainties.</a> Journal of Hydrology, 578, 124134.
  - >
    [12] Urich, C., & Rauch, W. (2014). <a href="https://doi.org/10.1016/j.watres.2014.08.020">Exploring critical pathways for urban water management to identify robust strategies under deep uncertainties. </a> Water Research, 66, 374–389.
  - >
    [13] Groves, D. G., & Bloom, E. (2013). Robust Water-Management Strategies for the California Water Plan Update 2013. RAND Corporation, Santa Monica, CA.
examples:
  - Boxes are shown in a <a href="../../examples/guillaume-2015/">simple flood demonstration problem</a> answering the question "Will regular flooding of ecological assets occur?"
  - Examples are provided using EMA Workbench in its <a href="https://emaworkbench.readthedocs.io/en/latest/indepth_tutorial/open-exploration.html#Scenario-Discovery">documentation</a> and on the <a href="https://waterprogramming.wordpress.com/2015/08/05/scenario-discovery-in-python/">waterprogramming blog</a> (with comparison with CART)
  - Application of PRIM in the <a href="../../examples/lake-problem/">"lake problem"</a>, a hypothetical environmental management problem, to identify robust water pollution management policies. The algorithm was used in conjunction with the <a href="../../tools/openMORDM/">OpenMORDM</a> software [8]
  - PRIM is applied to identify uncertain factors likely to reduce the performance of cooperative regional water planning under deep uncertainty. More specifically, PRIM was used the help identify decision paths and critical deep uncertainties that reveal some potential competitions [10]
  - >
    Application of PRIM for both scenario discovery and sensitivity analysis to design robust operation rules for multi-purpose reservoirs: identifying the scenarios and associated most sensitive factors, then exploring the relationships between optimised operating rule curves and system performance [11]
  - >
    Testing the robustness of adaptation strategies for urban water management; identifying clusters of climate change and population growth scenarios that fail to meet performance targets: protecting the urban environment from minor flood events and providing wastewater drainage [12]
  - Identifying a decision-relevant scenario where the planned management strategy performed poorly. The scenario is then used to evaluate performance of other strategies to support urban and irrigation water demands and instream water requirements in the 2013 California Water Plan for the Central Valley of California [13]
---
