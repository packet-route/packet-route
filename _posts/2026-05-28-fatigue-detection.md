---
layout: post
title: "Fatigue Detection System"
date: 2026-05-28
class: "2025-2026"
author: "Matteo Melo and Pedro Ferreira"
categories: ["Big Idea 5 - Impact of Computing"]
tags: ["Teachable Machine"]
---

Identifying if someone is tired through human eyes might seem like an easy task, as you can just look at their posture, breathing rate, and other factors, but for our machine learning model, it is not that simple. Here is how we built a fatigue detection system that is able to distinguish between fatigued and not fatigued people.

We trained our model to distinguish fatigued and not fatigued people, specifically in sports. We provided over 140 samples for each category: fatigued and not fatigued. It identifies fatigue easily by matching the input with the posture samples in the fatigued category.

On the other hand, while testing the machine, we noticed it had trouble identifying people who were not fatigued, often considering everyone fatigued. During initial testing, the model suffered from a high rate of false positives, classifying non-fatigued individuals as fatigued until we adjusted our training parameters. To fix this, we tried adding more samples and increasing the epochs. This enabled the program to get more precise results because it analyzed the samples with more depth and complexity.

We wanted our machine learning model to identify fatigue through posture. At first, despite having similar images with similar postures, it was providing negative outcomes. However, after increasing the epochs, it was able to distinguish the variables. 

Overall, our program is definitely able to distinguish between fatigued and not fatigued individuals, but it does make mistakes despite the increased epochs. We were able to make this with little resources. Now, imagine what AI is capable of detecting, including things human eyes cannot detect.
