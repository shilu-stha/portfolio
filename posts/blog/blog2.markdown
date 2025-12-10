---
layout: post
title: "Bayesian Linear Regression: Embracing Uncertainty"
date: 2024-10-15
tags: ["bayesian", "regression", "probabilistic-modelling"]
summary: "Why moving from point estimates to distributions over parameters changes how we think about predictions."
category: blog
permalink: /blog/bayesian-linear-regression/
---

Traditional linear regression gives point estimates: one fixed value per parameter and one fixed prediction per input. In contrast, **Bayesian linear regression** gives us a *distribution* over parameters, and therefore a distribution over predictions.

This shift from single values to distributions is more than a mathematical detail—it changes how we interpret model outputs.

In Bayesian linear regression:

- We start with a **prior** over parameters (e.g. a Gaussian).
- We observe data and update this prior using **Bayes’ theorem**.
- We obtain a **posterior** distribution that reflects both prior beliefs and evidence.
- The **posterior predictive** distribution gives us not just a mean prediction, but also uncertainty intervals.

During my coursework, I implemented Bayesian linear regression and compared it to standard ridge regression. A key realisation was that ridge regression can be interpreted as Bayesian linear regression with a Gaussian prior on the weights. What appears as “regularisation” in frequentist language becomes “prior belief” in the Bayesian view.

I explored small-data regimes and noisy environments where uncertainty is crucial. Instead of asking “What is the prediction?”, I learned to ask “How **confident** is the model in this prediction?”

Coming from industry, where decisions often have consequences—financial, safety, or user experience—this ability to express and reason about uncertainty feels essential. It is also a critical ingredient for building safer, more robust ML systems in deployment.