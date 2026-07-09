---
title: "Validating a Mental Health Screening Tool at Scale"
excerpt: "Checked whether a widely used psychological questionnaire holds up across very different age groups, then tested how well background information alone can flag people at risk."
collection: portfolio
---

This project validated a well-known psychological screening tool (the DASS-42, used to measure depression, anxiety, and stress) on a public dataset of nearly 40,000 people. The goal was simple to state but hard to get right: does this questionnaire actually measure what it claims to measure, and does it work the same way for everyone?

The tool held up well in young adults, and reliably measured the same three things (depression, anxiety, stress) it was designed to measure. In an older adult sample, the picture was more nuanced: the depression items worked cleanly, but some anxiety and stress items started to overlap with each other, a common and well documented issue when a questionnaire is used outside the population it was originally built for.

The second half of the project asked a different question: using only background information, personality traits, and how long someone took to answer, without any of the actual symptom answers, how well can you flag someone's likely risk level? The model got it right about 6 times out of 10 overall, and it was especially good at catching the most severe cases, which is usually what matters most in a real screening context.

**What this shows:** the ability to validate a measurement tool properly before trusting it, and to report a model's real-world performance honestly, exactly the kind of scrutiny you'd want applied to a customer survey or employee wellbeing tool before rolling it out.

[View on GitHub](https://github.com/MikeNeuroquant/survey-validation-behavioral-scoring)