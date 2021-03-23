---
layout: concept
title: Dynamic Adaptive Planning (DAP)
permalink: /theory/DAP/
page_authors:
  - C. Rosello
page_reviewers:
excerpt: DAP is an approach to designing adaptive and robust plans based on concepts associated with Assumption-Based Planning (ABP) in which a plan is valid under an assertion (assumption) made about future conditions. The approach is also known as (Dynamic) Adaptive Policymaking.
purpose: >
  <p> 
  DAP [1,2] aims at designing adaptive and robust plans, i.e., plans considering actions to implement immediately (near-term actions) and in the future (alternative actions) to cope with <a href="../multiple-plausible-futures/">multiple plausible futures </a>. 
  </p>
  <p>A key output is an explicit <a href="../monitoring-plan/">monitoring plan</a> to evaluate the plan/policy performance post-implementation [4,5]
  </p>
requirements: >
  <p>
  The approach requires stakeholder participation in the design process [1,4,5] and the willingness to incorporate long term monitoring into decision making.
  </p>
decomposition: >
  <p>
  Two main steps are identified: a design step and an implementation step [4]. 
  </p>
  <p> The design stage of DAP (see figure) aims at building a flexible plan, able to adapt to future conditions and reduce the vulnerabilities of the assumptions underlying the plan [1,4]. 
  </p>
  <p>
  <img src="../../images/DAP-fig1-adaptive-plan-design-steps.jpg" width=70% alt="The five steps to design the adaptive plan: 1) stage setting, 2) assembling the initial plan, 3) increasing the robustness of the initial plan, 4) setting up the monitoring system and 5) preparing the trigger responses">
  <div class=imgcredit>Figure 3.1 <a href="https://link.springer.com/chapter/10.1007/978-3-030-05252-2_3" target="_blank">Walker et al. 2019, 2013</a></div>
  </p>
  <p> The five steps of the design stage consist of [1,4]: 
  <ol>
  <li>Setting the scene, defining constraints, objectives, definition of success for the objectives and plausible actions. The definition of success is based on the specification of objectives and constraints (e.g., economic, emission loads) that stakeholders involved in the planning design stage would find acceptable.
  </li>
  <li>Assembly of the initial plan (basic policy). Two activities are considered: 1) the specification of the policy actions to achieve the objectives, and 2) the explicit outline of the necessary conditions of success (in terms of acceptable outcomes or results), to be used to identify <a href="../vulnerability-analysis/">vulnerabilities</a>, <a href="../signposts/">signposts</a> and <a href="../triggers/">triggers</a>.
  </li>
  <li>Increasing the robustness of the initial plan based on assessment of vulnerabilities or opportunities.  
    <ul>
      <li><a href="../vulnerability-analysis/">Methods to assess vulnerabilities and opportunities</a> include analytical tools such as <a href="../exploratory-modelling/">Exploratory Modelling and Assessment (EMA)</a>, scenario analysis or expert opinion, using SWOT (Strengths, Weaknesses, Opportunities, Threats) analysis.
      </li>
      <li> Five types of actions can be used based on the level of certainty regarding vulnerabilities, or to proactively deal with external events:
        <ul>
        <li> Mitigating actions (M): to reduce adverse impacts from certain or more likely vulnerabilities </li>
        <li> Hedging actions (H): to reduce adverse impacts associated with uncertain vulnerabilities </li>
        <li> Seizing actions (SZ): to take advantage of certain or more likely opportunities </li>
        <li> Exploiting actions (E): to take advantage of (uncertain) new developments to enhance the plan's chance of success </li>
        <li> Shaping actions (SH): proactive actions to affect external events or conditions that could reduce the risks of failure or increase the chance of success of the plan </li>
        </ul>
      </li>
    </ul> 
  </li>
  <li>Setting up a monitoring plan involves defining:
    <ul>
    <li><a href="../signposts/">Signposts</a>, i.e., variables to monitor, designed based on the identification of the necessary conditions of success for the plan.</li>
    <li><a href="../triggers/">Triggers</a>, i.e. threshold values for considering new actions, including contingency actions, to support the successful achievement of the plan</li>
    </ul>
    Overall, the monitoring stage in DAP is what allows for the flexibility and adaptivity of the plan.
  </li>
  <li>Preparation of the trigger responses, providing directions regarding the conditions to consider when implementing contingency actions. Preparation may include include financial and legal pre-requirements, blueprint design for engineering work, or case study analysis, among other examples. Four types of contingency actions can be considered:
  <ul>
  <li> Defensive actions (DA): responsive actions to clarify the plan, preserve its benefits or meet outside challenges in response to specific triggers, but leaving the initial plan unchanged. </li>
  <li> Corrective actions (CR): adjustments to the initial plan in response to specific triggers. </li>
  <li> Capitalizing actions (CP): responsive actions to take advantage of opportunities to improve the initial plan performance. </li>
  <li> Reassessment (RE): initiated when the analyses and assumptions underpinning the plan are no longer valid. </li>
  </ul>
  </li>
  </ol>
  </p>
  <p> 
  The implementation stage covers both the initial plan set up in step 2 of the design process, followed by adaptive actions (step 3) according to how future conditions may unfold, and the establishment of the monitoring plan (step 4). Contingency actions (step 5) are considered post-implementation of the plan based on signposts' trigger events.
  </p>
tools:
also_see:
  - permalink: /theory/DAPP/
    name: Dynamic Adaptive Policy Pathways (DAPP)
    description: The DAP approach has been combined with <a href="../adaptation-pathways/"> adaptation pathways </a> to design the DAPP approach, another <a href="../dmdu/"> DMDU </a> approach.
further_reading:
  - >
    Walker, W. E., Marchau, V. A., & Kwakkel, J. H. (2019). <a href="https://link.springer.com/chapter/10.1007/978-3-030-05252-2_3" target="_blank">Dynamic Adaptive Planning (DAP)</a>. In Decision Making under Deep Uncertainty (pp. 53–69). Springer, Cham.
  - >
    Rahman, S. A., Walker, W. E., & Marchau, V. (2008). <a href="https://www.rli.nl/sites/default/files/Achtergrondstudie%20Coping%20with%20Uncertainties.pdf" target="_blank">Coping with uncertainties about climate change in infrastructure planning–an adaptive policymaking approach</a>. ECORYS and Delft University of Technology: Delft, The Netherlands.
examples:
  - Illustration of the approach in the context of sea level rise uncertainty in The Netherlands [5].
references:
  - >
    [1] Walker, W. E., Rahman, S. A., & Cave, J. (2001). <a h ref="https://doi.org/10.1016/S0377-2217(00)00071-0">Adaptive policies, policy analysis, and policy-making.</a> Complex Societal Problems, 128(2), 282–289.
  - >
    [2] Kwakkel, J. H., Walker, W. E., & Marchau, V. (2010). <a href="https://doi.org/10.18757/ejtir.2010.10.3.2891"> Adaptive airport strategic planning. </a> European Journal of Transport and Infrastructure Research, 10(3).
  - >
    [3] Dewar, J. A., Builder, C. H., Hix, W. M., & Levin, M. H. (1993). <a href="https://www.rand.org/pubs/monograph_reports/MR114.html" target="_blank">Assumption-based planning; a planning tool for very uncertain times</a>. RAND CORP SANTA MONICA CA.
  - >
    [4] Walker, W. E., Marchau, V. A., & Kwakkel, J. H. (2019). <a href="https://link.springer.com/chapter/10.1007/978-3-030-05252-2_3" target="_blank">Dynamic Adaptive Planning (DAP)</a>. In Decision Making under Deep Uncertainty (pp. 53–69). Springer, Cham.
  - >
    [5] Rahman, S. A., Walker, W. E., & Marchau, V. (2008). <a href="https://www.rli.nl/sites/default/files/Achtergrondstudie%20Coping%20with%20Uncertainties.pdf" target="_blank">Coping with uncertainties about climate change in infrastructure planning–an adaptive policymaking approach</a>. ECORYS and Delft University of Technology: Delft, The Netherlands.
---
