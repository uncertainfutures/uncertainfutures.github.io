---
layout: concept
title: Stress testing
permalink: /theory/stress-testing/
excerpt: Stress testing involves evaluating how decision alternatives perform in different conditions.
purpose: >
  Understanding how performance of decision alternatives can vary in future can help <a href="../../theory/management-options/"
    >design better management options</a
  > by understanding in what conditions an alternative is "<a href="../../theory/robust-decisions/"
    >robust</a
  >" and performs well, or under what circumstances changes will need to made within an "<a href="../../theory/adaptive-decisions/">adaptive</a>" solution.
requirements: >
  <p>Measures of performance and one or more decision alternatives need to be specified. Stress testing can be performed in an optimisation context (e.g. to identify <a href="../../theory/robust-decisions/">robust decisions</a>), in which case the decision alternatives are defined within a model.</p>
decomposition: >
  <p>Stress testing methods differ in how they characterise scenarios and the form of output they provide. Scenarios can be pre-determined, defined by model parameters, or created within the stress testing process. Stress testing may report failures, simply show how performance varies, or aim to compare decision alternatives.</p>
  Specific classes of approaches therefore include:
  <ul>
  <li><a href="../../theory/vulnerability-analysis/">Vulnerability analysis</a> specifically identifies conditions in which management options can fail</li>
  <li>Mapping performance as a function of external drivers, e.g. in <a href="../../theory/decision-scaling/">Decision scaling</a></li>
  <li>Evaluating <a href="../../theory/robustness-metrics/">robustness metrics</a>, e.g. in <a href="../../theory/robust-optimisation/">Robust optimisation</a> or "<a href="../../theory/robust-decision-making/">Robust decision making</a>"</li>
  <ul>
tools:
  - slug: foreSIGHT
    name: foreSIGHT
    description: An R package to to create hydroclimate scenarios, stress test systems and visualize system performance in scenario-neutral climate change impact assessments.
also_see:
  - permalink: /theory/scenario-neutral-climate-impact-assessment/
    name: Scenario-neutral climate impact assessment
    description: Evaluates system performance across a range of possible climates rather than a pre-determined set of scenarios
examples:
further_reading:
references:
---
