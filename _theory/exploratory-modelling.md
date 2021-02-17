---
layout: concept
title: Exploratory modelling
permalink: /theory/exploratory-modelling/
page_authors:
  - Joseph Guillaume
page_reviewers:
excerpt: Exploratory modelling refers to the use of computer models to explore the implications of varying assumptions and hypotheses rather than performing experiments with a model as if it is the actual system.
purpose: >
  Exploratory modelling lends itself well to situations where system behaviour cannot be reliably represented, e.g. because it will change in future. Exploratory modelling is therefore commonly used in <a href="../scenario-development/">scenario development</a> to select <a href="../multiple-plausible-futures/">multiple plausible futures</a> used to identify <a href="../robust-decisions/">robust</a> and <a href="../adaptive-decisions/">adaptive</a> decisions.
requirements: >
  <p>In the context of decision making, a computer model provides a representation of a system that shows how outputs change as a response to inputs. Exploratory modelling requires that alternative assumptions and hypotheses can be represented in the model, typically by varying parameters of a model, which may also change assumptions about model structure, i.e. how inputs and outputs are related.</p>
  <p>It is common that the computer model needs to be run many times, such that computational cost is often important. Insights are often easier to gain from simpler, faster running models than more complex, longer running models.</p>
decomposition: >
  <p>Exploring the implications of varying assumptions and hypotheses involves a series of computational experiments that reveal how the world would behave if various guesses about the system were correct.</p>
  <p>Exploratory modelling is contrasted with "consolidative modelling", which consolidates known facts into a single package and then uses it as a surrogate for the actual system [1]. Whereas consolidative modelling provides a single answer to a question (optionally with an uncertainty estimate), exploratory modelling provides a separate answer for each assumption or hypothesis. When exploring the future, this therefore provides <a href="../multiple-plausible-futures/">multiple plausible futures</a> for further analysis.</p>
  <p>The output from each individual "model scenario" should be interpreted as conditional on the assumptions used. When communicated each separate model scenario, the modeller can "make it hypothetical" [2], e.g. <a href="../stress-testing">stress testing</a> how a policy would perform across hypothetical scenarios. However, by reasoning over a set of scenarios, it becomes possible for the modeller to "demonstrate robustness" [2] of a conclusion, e.g. showing that a policy <a href="../robust-decisions/">performs well in all of the futures tested</a>.</p>
# This text could be expanded to include more specific points from Bankes (1993) and the 7 things you can do with a bad model from Hodges (1991) and Hodges and Dewar (1992)
tools:
  - slug: emaworkbench
    name: Exploratory Modelling and Analysis (EMA) Workbench
    description: Python package for setting up, performing and analysing computer model runs as part of exploratory modelling experiments.
also_see:
further_reading:
  - >
    Bankes S (1993) <a href="http://www.jstor.org/stable/171847">Exploratory Modeling for Policy Analysis</a>. Operations Research. 41 (3): 435–449
examples:
references:
  - >
    [1] <a href="http://www.jstor.org/stable/171847">Bankes (1993)</a>
  - >
    [2] <a href="http://dx.doi.org/10.1002/2017WR020609">Guillaume et al. (2017)</a>
---
