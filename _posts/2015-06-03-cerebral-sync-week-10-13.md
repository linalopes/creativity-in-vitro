---
layout: post
title: Cerebral Sync - Week 10/13
id: 2015-06-03-cerebral-sync-week-10-13.md
categories:
  - meta-codex
image: assets/images/favicon.png
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2015-06-03-cerebral-sync-week-10-13.md
tags: 
date: 2015-06-03
author: lina
---
> “Life itself is noisy; our job is to find clarity amidst the static.”


### Objective

This meeting aimed to explore the analysis of EEG signals, emphasizing signal-to-noise ratio, feature selection, and testing preliminary Machine Learning models to identify patterns in cerebral responses during musical and linguistic stimulation.

---

### Summary

- **Signal-to-Noise Exploration**: Lina detailed the complexity of extracting meaningful data from EEG recordings, describing the omnipresent noise factors such as body movements, sweat, and environmental influences. The discussion revolved around optimizing the signal-to-noise ratio (SNR), crucial in distinguishing genuine neurological signals.
    
- **Channel Analysis and Selection**: Lina presented a detailed assessment of EEG channels, pinpointing F3, F4, Fz, O1, and Pz as channels showing the best SNR. Despite initial assumptions favoring temporal regions (T3, T4) for musical and linguistic insights, frontal and occipital channels emerged prominently.
    
- **Filtering Techniques**: A thorough explanation of filtering methods, including high-pass and low-pass filters, was discussed. These techniques mitigate drift and electrical noise, ensuring clearer data representation aligned closely to zero reference levels.
    
- **Initial Machine Learning Experiments**: Four preliminary ML models—K-Nearest Neighbors (KNN), Logistic Regression, Random Forest, and Support Vector Machine (SVM)—were evaluated. Logistic Regression and Random Forest showed promising results, suggesting both linear and non-linear patterns in EEG signals.
    
- **Principal Component Analysis (PCA)**: PCA was introduced as a dimensionality reduction method, though results remained exploratory and visually intriguing rather than conclusively interpretable at this stage.
    
- **ICA for Artifact Removal**: Lina introduced Independent Component Analysis (ICA) to isolate and remove artifacts, describing the process vividly through the metaphor of the "cocktail party problem," highlighting its potential in refining EEG data quality.
    
- **Literature Review and Comparative Study**: An in-depth examination of recent EEG research guided methodological decisions, emphasizing the practicality of ICA combined with wavelet transforms, and insights into successful machine learning techniques.
    

---

### Action Items

- Refine EEG dataset precision and standardization.
    
- Implement and test ICA artifact removal comprehensively.
    
- Explore deeper into wavelet transforms and their applicability to EEG spectral analysis.
    
- Experiment further with neural network models (CNN specifically designed for EEG).
    

---

### Final Notes

This cerebral syncing marked significant progress in understanding the complexities and potentials of EEG signal analysis. The revelation of distinct linear and non-linear patterns encourages further exploration of machine learning models. The extensive literature review provided a strong methodological foundation, shaping future experimental designs.

---

### Creative Insights

- **Machine Intuition**: Leveraging AI interpretations (via GPT) brought poetic reflections to technical analyses, suggesting a symbiotic relationship between computational clarity and creative speculation.
    
- **Speculative Futures**: Conversations hinted at broader speculative questions about cognition, creativity, and identity, suggesting intriguing avenues such as "brain donations" from artists, highlighting the speculative essence of Creativity in Vitro’s ambitious vision.
