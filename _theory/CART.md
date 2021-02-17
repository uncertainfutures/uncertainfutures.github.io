---
layout: concept
title: CART
permalink: /theory/CART/
page_authors:
  - Caroline Rosello
  - Joseph Guillaume
page_reviewers:
excerpt: >
  CART (Classification and Regression Trees) predicts outcomes based on binary splits of input variables. It can be used for scenario discovery to identify vulnerable scenarios for policy measures.
purpose: >
  <p> CART [1] is a rule-based method that can be used for <a href="../scenario-discovery/">scenario discovery</a> to  discover relationships between a set of uncertain input variables (predictors) and a target objective.</p>
  <p>CART generates binary trees based on the application of an iterative binary partitioning procedure.</p>
  <p>The final tree includes a series of nodes and branches, each branch being representative of a scenario.</p>
requirements: >
  <p>There are two main requirements [2]:<ul>
  <li>Generation of a database representing the results for a target objective from different combinations of predictors' values and based on the use of simulation model (see <a href="../scenario-discovery/">scenario discovery</a>)</li>
  <li>Definition of a splitting rule for each predictor to divide the tree into branches and construct a fully grown decision tree </li></ul></p>
decomposition: >
  <p>Application of CART is usually performed with existing software packages (see Tools), specifying the target outcome (e.g. success vs failure of a policy) and the predictor variables to be split (e.g. variables describing states of multiple plausible futures).</p>
  <p> The algorithm involves three major steps can be identified:<ol>
  <li>A 'splitting' stage in which a decision tree is grown [2], involving: <ul>
  <li>the definition of a threshold value for each predictor explaining the target outcome [16]. One example of a splitting method (i.e., heterogeneity criteria) is the Gini index [2] </li>
  <li> the division of the main tree into two child trees split at a node featuring a predictor in a given input combination, with each branch representing the outcome of interest when the predictor is under or above the defined threshold [16] </li>
  <li> the continuation of the procedure with the remaining predictors on the newly formed branches, forming new nodes and branches, until no more splitting is possible [16] </li>
  </ul>
  <li> A 'pruning' stage in which the maximal-sized tree is pruned back to the root and where a split contributing the least to the overall performance of the tree is removed [16]. Remaining nodes are then recombined. The process continues to find the tree with the best predictive power in terms of coverage (i.e., ratio of relevant cases) and density (i.e., fraction of relevant points) [2]. Examples of pruning methods include cost-complexity pruning, weakest link pruning [8]. </li>
  <li> User selection among the generated trees (fully grown one and pruned alternatives) of a tree with high coverage and high density [2].</li>
  </ol></p>
# TODO: would be good to have a simple example here
tools:
  - slug: rpart
    name: Recursive Partitioning (rpart) and Regression Trees R package
    description: Recursive partitioning for classification, regression and survival trees [3]
  - slug: openMORDM
    name: openMORDM
    description: An R package for <a href="../MORDM/">many-objective robust decision making</a> [4]
  - slug: Orange
    name: Orange
    description: open source data mining package that consists of a C++ library with python bindings [5,6]
  - slug: MATLAB
    name: MATLAB
    description: Matlab Statistics and Machine Learning Toolbox includes CART functions [7]
    # TODO: list the specific functions involved
also_see:
  - permalink: /theory/PRIM/
    name: PRIM
    description: A common alternative algorithm for scenario discovery
  - permalink: /theory/exploratory-modelling/
    name: Exploratory modelling
    description: Scenario-based approach using computational experiments to analyse complex and uncertain issues and support decisions.
further_reading:
  - Lempert, R. J., Bryant, B. P., & Bankes, S. C. (2008). <a href="https://www.rand.org/pubs/working_papers/WR557.html">Comparing algorithms for scenario discovery</a>. RAND, Santa Monica, CA.
examples:
  - Application to the <a href="../../examples/lake-problem/">"lake problem"</a> to identify robust water pollution management policies [15]
  - CART provides short-term prediction that a flood will occur in a highly urbanised watershed, identifying the conditions leading to that prediction [10]
  - Use of CART to discover knowledge and predictive variables for evaluation of the impacts of land cover/land use change (including waterbodies) and climate change on the conservation of ecosystem services [11]
  - Scenario discovery of distinct scenario drivers explaining poor or good performance of climate mitigation strategies, using an agent-based model [12]
references:
  - >
    [1] Breiman, L. (1984). Algorithm cart. Classification and Regression Trees. California Wadsworth International Group, Belmont, California.
  - >
    [2] Lempert, R. J., Bryant, B. P., & Bankes, S. C. (2008). Comparing algorithms for scenario discovery. RAND, Santa Monica, CA.
  - >
    [3] Therneau, T., Atkinson, B., & Ripley, B. (2019) Recursive Partitioning and Regression Trees (“rpart” package) on <a href="https://github.com/bethatkinson/rpart">GitHub</a> and <a href="https://cran.r-project.org/package=rpart">CRAN</a>.
  - >
    [4] Hadka, D., Herman, J., Reed, P., & Keller, K. (2015). <a href="https://doi.org/10.1016/j.envsoft.2015.07.014">An open source framework for many-objective robust decision making.</a> Environmental Modelling & Software, 74, 114–129.
  - >
    [5] Curk, T., Demsar, J., Xu, Q., Leban, G., Petrovic, U., Bratko, I., Shaulsky, G., & Zupan, B. (2005). <a href="https://doi.org/10.1093/bioinformatics/bth474">Microarray data mining with visual programming. </a> Bioinformatics, 21(3), 396–398.
  - >
    [6] Kwakkel, J. H., & Pruyt, E. (2013). <a href="https://doi.org/10.1016/j.techfore.2012.10.005">Exploratory Modeling and Analysis, an approach for model-based foresight under deep uncertainty. </a>Technological Forecasting and Social Change, 80(3), 419–431.
  - >
    [7] MathWorks Inc. (2015). MATLAB and Statistics and Machine Learning Toolbox.
  - >
    [8] Hastie, T., Tibshirani, R., & Friedman, J. (2009). The elements of statistical learning: Data mining, inference, and prediction. Springer Science & Business Media.
  # TODO: find a way to automate numbering
  - >
    [10] Erechtchoukova, M. G., Khaiter, P. A., & Saffarpour, S. (2016). <a href="https://doi.org/10.1007/s11269-016-1423-6">Short-Term Predictions of Hydrological Events on an Urbanized Watershed Using Supervised Classification. </a>Water Resources Management, 30(12), 4329–4343.
  - >
    [11] García, V. J., Márquez, C. O., Isenhart, T. M., Rodríguez, M., Crespo, S. D., & Cifuentes, A. G. (2019).<a href="https://doi.org/10.1016/j.heliyon.2019.e02701"> Evaluating the conservation state of the páramo ecosystem: An object-based image analysis and CART algorithm approach for central Ecuador. </a> Heliyon, 5(10), e02701.
  - >
    [12] Gerst, M. D., Wang, P., Roventini, A., & Dosi, G. (2012). Integrated assessment of mitigation strategies using an agent-based model of the linked energy, economic, and climate system. International Environmental Modelling Software Society (IEMSs), International Congress on Environmental Modelling and Software. Managing Resources of a Limited Planet, Sixth Biennial Meeting, Leipzig, Germany.
  - >
    [13] Kumar, R., Jaiswal, A., & Rai, D. (2013). Privacy Preserving CART Algorithm over Vertically Partitioned Data. International Journal of Innovative Research in Computer and Communication Engineering, 1(9).
  - >
    [14] Naghibi, S. A., Pourghasemi, H. R., & Dixon, B. (2015). <a href="https://doi.org/10.1007/s10661-015-5049-6">GIS-based groundwater potential mapping using boosted regression tree, classification and regression tree, and random forest machine learning models in Iran.</a> Environmental Monitoring and Assessment, 188(1), 44.
  - >
    [15] Hadka, D., Herman, J., Reed, P., & Keller, K. (2015).<a href="https://doi.org/10.1016/j.envsoft.2015.07.014"> An open source framework for many-objective robust decision making.</a> Environmental Modelling & Software, 74, 114–129.
  - >
    [16] Steinberg, D. (2009). CART: classification and regression trees. In The top ten algorithms in data mining (CRC Press, Vol. 9, p. 179). Taylor & Francis Group.
---
