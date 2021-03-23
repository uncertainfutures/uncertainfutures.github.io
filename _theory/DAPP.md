---
layout: concept
title: Dynamic Adaptive Policy Pathways (DAPP)
permalink: /theory/DAPP/
excerpt: DAPP is a framework to evaluate policy robustness and adaptiveness under deep uncertainty. The approach combines adaptive planning and adaptive pathways concepts.
purpose: >
  <p>DAPP  [1] aims at guiding the design of a robust and adaptive plan as a sequence of actions (near term and alternative future actions) over time through [2]: <ul>
  <li>exploration of sequences of decisions through an <a href="../adaptation-pathways/">adaptation pathways</a> approach. This provides a portfolio of plausible robust and adaptive actions, consisting of near term and long term options, to be used within <a href="../adaptive-pathways/">adaptive pathways</a> for a system to cope under plausible futures (i.e., scenarios)</li>
  <li> making visible <a href="../path-dependency/">path dependency</a> of alternative future strategies</li>
  </ul>
  </p>
  <p> DAPP also supports participatory modelling through engaging stakeholders and decision makers in problem-solving activities [2,3]</p>
  <p> The approach was originally built to implement climate-resilient pathways for long-term water resources strategic planning but can be applied to other long-term strategic planning problems under <a href="../DMDU/">deep uncertainty</a> [2,13] </p> 
  <p> The approach is useful [2]: <ul>
  <li> when applied to facilitate decision-making understanding and to support the acknowledgement of uncertainties in plans </li>
  <li> as an enabler for action </li>
  <li> when considering coupled physical-technical-human systems and long time planning horizons </li>
  <li> when considering the potential for implementing alternative adaptation actions to solve issues according to how the future may unfold </li> 
  </ul></p>
requirements: >
  <p> Operationalising the DAPP approach requires: <ul>
  <li> setting the scene for a system of interest and defining a vision [2] </li>
  <li> defining narratives describing future plausible conditions [2] </li>
  <li> identifying indicators of change for the system and for actions and associated threshold values [2]</li>
  <li> stakeholder buy-in and engagement in relevant activities [3] </li>
  <li> considering the intervention of local knowledge-brokers to facilitate the application of the approach and stakeholder engagement [3] </li>
  </ul></p>
decomposition: >
  <p> The DAPP framework can be decomposed into eight main iterative steps [2]:
  <ol>
  <li> Participatory problem framing, defining:
   <ul>
   <li>boundaries of a system of interest</li>
   <li>performance objectives, including conditions of success for the system used to evaluate performance of policy options</li>
   <li>current and future vulnerabilities (i.e., conditions/risk factors for which the system (will) fail to achieve acceptable objectives). Vulnerabilities may be:<ul>
     <li>intended to be managed by actions or policy options, e.g., reservoir development to support water users and associated uses, education to support the adoption of best practices, microirrigation systems to improve water efficient uses at the field level</li>
     <li>non-manageable factors with uncertainty as to how they may evolve, to be described within narratives (<a href="../scenario-development/">scenarios</a>), e.g., climate change, national legislation, global markets, population growth. </li>
   </ul></ul> 
  </li>
  <li> Identification of adaptation <a href="../tipping-points/">tipping points</a> (ATPs), i.e. conditions and timing of failure for the current system when facing different future scenarios. Approaches to identify ATPs (i.e., threshold values) include: <ul>
   <li> 'bottom-up' approaches: <a href="../stress-testing/">stress tests</a> through sensitivity analyses, <a href="../scenario-discovery/">scenario discovery</a> [5], expert judgement [1], and/or stakeholder consultation [3]</li>
   <li> 'top-down' approaches: model-based assessment using static or transient [9] <a href="../scenario-development/">scenarios</a></li></ul>
  </li>
  <li> Identification of alternative actions based on step 1 and 2, to address identified vulnerabilities or opportunities, followed by determination of their ATPs </li>
  <li> Design and assessment of the <a href="../adaptive-pathways">adaptive pathways</a>. This stage leads to the design of a pathway map (see figure below), also referred to as a "metro map", with different pathways evaluated in terms of performance objectives for the system [2]. 
  </li>
  <p>Opportunities, no-regret actions, lock-ins and their associated timing of implementation under changing conditions can be inferred from the map.</p>
  <p>
    <img src="../../images/haasnoot-2019-metro-map.jpg" alt="Illustration of an adaptation pathways' metro map and its associated scorecard">
  </p>
  Methods to develop and explore adaptive pathways include:
  <ul>
   <li>drawing them manually</li>
   <li>using a dedicated application such as the <a href="../../tools/pathways-generator/">Pathways Generator</a> [4] </li>
   <li> based on models such as agent-based models [14], using multi-objective robust optimisation [6], serious games [7,8] </li>
   <li> during stakeholder focus group discussions [3]</li>
   <li> using a combination of model-based assessment and group discussions </li></ul>
   </li>
  <li>
  The performance of each pathway is then evaluated and recorded in a scorecard. Methods of evaluation include:<ul>
  <li> cost-benefit analysis [16]</li>
  <li> multi-criteria analysis [12] </li>
  <li> real options analysis [12] </li>
  </ul></li>
  <li> Design of the adaptive strategy in terms of:
  <ul>
   <li>Selection of near term and alternative (long-term) actions from the map</li>
   <li>Contingency actions to support the achievement of the selected pathways</li>
   <li>A <a href="../monitoring-plan/">monitoring plan</a>, describing signposts (indicators) and <a href="../triggers/">triggers</a> (threshold values) for implementing or not actions according to future conditions</li>
  </ul>
  <li> Implementation of the adaptive plan </li>
  <li> Monitoring of the strategy and re-evaluation of the plan, if necessary </li>
  </ol></p>
  <p>The summary figure provided by Haasnoot et al. [2] is shown below.
    <img align="center" src="../../images/Haasnoot et al_2019_DAPP framework.jpg" width=70% alt="Description of the seven steps to implement the DAPP framework process from problem framing to evaluation and monitoring of a plan.">
  </p>
tools:
  - slug: pathways-generator
    name: Pathways Generator
    description: Software to design and generate adaptive pathways [4]
also_see:
  - permalink: /theory/scenario-discovery/
    name: Scenario Discovery
    description: A form of vulnerability analysis that can be used within DAPP (Step 2) to identify policy-relevant plausible future scenarios or a limited of future scenarios to focus on.
  - permalink: /theory/DAP/
    name: Dynamic Adaptive Planning
    description: An approach to design adaptive and robust plans also known as (Dynamic) Adaptive Policymaking.
  - permalink: /theory/adaptive-pathways/
    name: Adaptive pathways
    description: Descriptions of the sequences of options that can be taken and the circumstances in which alternative sequences might be selected.
  - permalink: /theory/adaptation-pathways/
    name: Adaptation pathways
    description: A family of approaches for learning and decision aiding to help decision makers reflect on the ability of decision strategies to prevent maladaptation when facing multiple plausible futures.
further_reading:
  - >
    Haasnoot, M., Kwakkel, J. H., Walker, W. E., & Maat, J. ter. (2013). <a href="https://doi.org/10.1016/j.gloenvcha.2012.12.006">Dynamic adaptive policy pathways: A method for crafting robust decisions for a deeply uncertain world. </a> Global Environmental Change, 23(2), 485–498.
  - >
    Haasnoot, M., Warren, A., & Kwakkel, J. H. (2019). <a href="https://link.springer.com/chapter/10.1007/978-3-030-05252-2_4">Dynamic adaptive policy pathways (DAPP)</a>. In Decision Making under Deep Uncertainty (pp. 71–92). Springer, Cham.
  - >
    Lawrence, J., Haasnoot, M., McKim, L., Atapattu, D., Campbell, G., & Stroombergen, A. (2019). <a href="https://link.springer.com/chapter/10.1007/978-3-030-05252-2_9">Dynamic adaptive policy pathways (DAPP): From theory to practice</a>. In Decision Making under Deep Uncertainty (pp. 187–199). Springer, Cham.
examples:
  - >
    Sustainable Delta Game: A simulation of a decision setting in a river catchment to support participant learning and preparation of a water management plan to deal with future situations [8]
  - Application of DAPP for the Dutch Delta Programme to support adaptive planning for flood protection in the face of future climate and socio-economic changes [11].
  - Application and uptake of DAPP for flood risk management and planning under climate change uncertainty in New Zealand [3]
  - Application of the different steps of the DAPP approach in the context of the Rhine Delta in The Netherlands for flood risk adaptation against future climate change [1]
references:
  - >
    [1] Haasnoot, M., Kwakkel, J. H., Walker, W. E., & Maat, J. ter. (2013). <a href="https://doi.org/10.1016/j.gloenvcha.2012.12.006">Dynamic adaptive policy pathways: A method for crafting robust decisions for a deeply uncertain world. </a> Global Environmental Change, 23(2), 485–498.
  - >
    [2] Haasnoot, M., Warren, A., & Kwakkel, J. H. (2019). <a href="https://link.springer.com/chapter/10.1007/978-3-030-05252-2_4">Dynamic adaptive policy pathways (DAPP)</a>. In Decision Making under Deep Uncertainty (pp. 71–92). Springer, Cham.
  - >
    [3] Lawrence, J., Haasnoot, M., McKim, L., Atapattu, D., Campbell, G., & Stroombergen, A. (2019). <a href="https://link.springer.com/chapter/10.1007/978-3-030-05252-2_9">Dynamic adaptive policy pathways (DAPP): From theory to practice</a>. In Decision Making under Deep Uncertainty (pp. 187–199). Springer, Cham.
  - >
    [4] <a href="https://publicwiki.deltares.nl/display/AP/Pathways+Generator">Pathways Generator</a>. Deltares.
  - >
    [5] Ramm, T. D., Watson, C. S., & White, C. J. (2018). <a href="https://doi.org/10.1016/j.compenvurbsys.2018.01.002">Describing adaptation tipping points in coastal flood risk management.</a> Computers, Environment and Urban Systems, 69, 74–86.
  - >
    [6] Kwakkel, J. H., Haasnoot, M., & Walker, W. E. (2015). <a href="https://doi.org/10.1007/s10584-014-1210-4">Developing dynamic adaptive policy pathways: A computer-assisted approach for developing adaptive strategies for a deeply uncertain world.</a> Climatic Change, 132(3), 373–386.
  - >
    [7] Lawrence, J., & Haasnoot, M. (2017). <a href="https://doi.org/10.1016/j.envsci.2016.12.003">What it took to catalyse uptake of dynamic adaptive pathways planning to address climate change uncertainty.</a> Environmental Science & Policy, 68, 47–57.
  - >
    [8] <a href="https://www.deltares.nl/en/software/sustainable-delta-game/#1">Sustainable Delta game</a>. Deltares.
  - >
    [9] Haasnoot, M., Schellekens, J., Beersma, J. J., Middelkoop, H., & Kwadijk, J. C. J. (2015).<a href="https://doi.org/10.1088/1748-9326/10/10/105008"> Transient scenarios for robust climate change adaptation illustrated for water management in The Netherlands.</a> Environmental Research Letters, 10(10), 105008.
  - >
    [10] Haasnoot, M., Middelkoop, H., Offermans, A., Beek, E. van, & Deursen, W. P. A. van. (2012).<a href="https://doi.org/10.1007/s10584-012-0444-2"> Exploring pathways for sustainable water management in river deltas in a changing environment. </a> Climatic Change, 115(3), 795–819.
  - >
    [11] Bloemen, P. J., Hammer, F., van der Vlist, M. J., Grinwis, P., & van Alphen, J. (2019). <a href="https://link.springer.com/chapter/10.1007/978-3-030-05252-2_14">DMDU into practice: Adaptive delta management in The Netherlands</a>. In Decision Making under Deep Uncertainty (pp. 321–351). Springer, Cham.
  - >
    [12] Lawrence, J., Bell, R., & Stroombergen, A. (2019) <a href="https://doi.org/10.3390/su11020406">A hybrid process to address uncertainty and changing climate risk in coastal areas using dynamic adaptive pathways planning, multi-criteria decision analysis & real options analysis: A New Zealand application</a>. Sustainability, 11(2), 406.
  - >
    [13] Michas, S., Stavrakas, V., Papadelis, S., & Flamos, A. (2020).<a href="https://doi.org/10.1016/j.enpol.2020.111350"> A transdisciplinary modeling framework for the participatory design of dynamic adaptive policy pathways.</a> Energy Policy, 139, 111350.
  - >
    [14] Magliocca, N., & Walls, M. (2018). <a href="https://scholarsarchive.byu.edu/iemssconference/2018/Stream-F/41/">Exploring distributional influences on and effects of dynamic adaptive policy pathways for repeated coastal hazards</a>. iEMSs2018 Fort Collins, Colorado, USA. (abstract only)
  - >
    [15] Smit, B., & Wandel, J. (2006). <a href="https://doi.org/10.1016/j.gloenvcha.2006.03.008">Adaptation, adaptive capacity and vulnerability.</a> Global Environmental Change, 16(3), 282–292.
  - >
    [16] de Ruig, L. T., Barnard, P. L., Botzen, W. J. W., Grifman, P., Hart, J. F., de Moel, H., Sadrpour, N., & Aerts, J. C. J. H. (2019). <a href="https://doi.org/10.1016/j.scitotenv.2019.04.308">An economic evaluation of adaptation pathways in coastal mega cities: An illustration for Los Angeles.</a> Science of The Total Environment, 678, 647–659.
---
