---
layout: "page"
title: Interpreting API Responses
nav_order: 8

#removed for now:
# ~~NOTE: _At this time, the Receptiviti API only accepts English language samples_~~
# {: .label .label-yellow }
---

# Interpreting API Responses

The Receptiviti API returns results based on four separate analyses:

1. LIWC scores (0-100)

2. Receptiviti scores (0-100)

3. Raw scores (5-point scale that utilizes a logarithmic distribution of results)


Based on the results, the algorithm generates a series of three personality snapshots, each comprised of two sentences that describe a personality type of a person whose language sample was analyzed, along with a one- to two-word summary, such as ‘Analytical thinker,’ ‘Persuasive,’ or ‘Easy-going.’ These snapshots follow the list of scores. See the list of metrics and scores here.

Following a personality snapshots, there are two aggregated scores referred to as Emotional Analysis:

- **Emotional Tone** Scores range from Negative (1) to Positive (99). A score around 50 is considered neutral and suggests either a lack of emotionality or similar amounts of positive and negative emotions.

- **Emotional Analysis:** Each Emotional Analysis facet score (anger, fear, sad) indicates how the percentage of the total negative emotion expressed in the language sample corresponds with each primary negative emotion.


We group Receptiviti scores into the five types of psychological insights they represent:

- Cognitive/Thinking Style

- Social Style

- Emotional Style

- Working Style

- The Big Five
