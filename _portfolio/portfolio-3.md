---
title: "A/B Test Analysis on a Marketing Campaign"
excerpt: "Estimated the real effect of an ad campaign on conversion by disentangling the treatment from how much users were actually exposed to ads."
collection: portfolio
---

A/B test analysis on a marketing campaign dataset (~588k users, `ad` treatment vs `psa` control). The naive comparison between groups overstates the campaign effect, because the two groups were not shown the same volume of ads: the treatment group received far more impressions, so any raw difference in conversion mixes the campaign effect with a pure dose effect.

I fit a logistic model that controls for log-transformed ad volume and includes an hour × day interaction, to separate the effect of the treatment from the effect of exposure and timing. Post-hoc contrasts on the model's marginal means then identify the specific hour × day windows with the highest conversion probability.

Group-level uncertainty is quantified with 95% bootstrap confidence intervals, which are preferable to parametric intervals given the ~96/4 group imbalance. Firth's Penalized Likelihood (`brglmFit`) is flagged as a robustness check for the logistic estimates under this imbalance.

**What this shows:** the ability to spot when a straightforward group comparison is misleading, adjust the analysis for the real drivers of the outcome, and report the effect of a campaign in a way that a marketing team can act on, exactly the kind of scrutiny you'd want applied to any experiment before making a spend decision.

[View full project on GitHub](https://github.com/MikeNeuroquant/A-B_test_analysis_demo/blob/main/notebooks/ab_test_analysis.ipynb)