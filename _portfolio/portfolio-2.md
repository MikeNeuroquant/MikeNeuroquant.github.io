---
title: "Turning Text into Measurable Emotional Signal"
excerpt: "Extracted interpretable, quantitative emotional and structural features from raw text to predict behavioral outcomes, not just sentiment scores."
collection: portfolio
---

Most text analysis stops at simple sentiment: positive, negative, neutral. This project goes further, extracting a richer, interpretable set of quantitative signals from raw text: eight distinct emotional dimensions (based on a well-established psychological framework) plus structural features that capture how a piece of writing is organized, not just which words appear in it. Text becomes a network, with words as connected points, and the shape of that network (how dense, how fragmented, how repetitive) turns out to carry quantitative information of its own.

The goal is to turn unstructured writing, like open-ended survey answers, feedback, or transcripts, into quantitative features that are both measurable and explainable, and that can be used to predict an outcome or classify a group. In this project, the outcome was distinguishing between two groups of writers based on their text alone. The same approach applies anywhere you have open-text data and want to quantitatively understand or predict behavior from it: customer feedback, survey verbatims, user research transcripts, before-and-after comparisons.

Because a model that predicts too well is often a warning sign rather than good news, the project also included a full validation step: checking, feature by feature, which quantitative signals were actually driving the prediction, and confirming they reflected genuine emotional and structural patterns rather than incidental quirks in the data. That check is part of the deliverable, not an afterthought, and it's what turns a promising result into one that can actually be trusted.

**What this shows:** the ability to turn raw text into interpretable, quantitative signal that maps onto real psychological constructs, and to validate that signal properly before it's used to predict or explain behavior.

[View on GitHub](https://github.com/MikeNeuroquant/text-network-emotion-classification)