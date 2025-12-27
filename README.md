Ad Click Prediction using Wide & Deep Learning

**Project Overview**

This project explores how user behavior and context can be used to predict whether a digital advertisement will be clicked. Using a structured ad interaction dataset, we built and evaluated a Wide & Deep learning model to better capture both simple feature relationships and more complex behavioral patterns. The broader objective was to understand which signals meaningfully influence ad engagement and how predictive modeling can support more efficient ad targeting.

**Dataset Description**

The dataset contains individual ad interaction records with a mix of demographic, behavioral, contextual, and device-level features. These include age and gender, browsing behavior, time of day, ad position, and device type. The target variable is a binary indicator of whether the ad was clicked.

Some fields contained missing values, particularly in demographic and categorical columns. These were addressed during preprocessing to ensure the model could train effectively without introducing bias or instability.

**Methodology**

We implemented a Wide & Deep neural network to balance memorization and generalization:

The wide component captures explicit feature interactions, such as combinations of device type and time of day.

The deep component uses embeddings and nonlinear transformations to learn broader behavioral patterns.

The workflow included data cleaning, categorical encoding, feature crossing, and model training. Performance was evaluated using ROC curves and AUC scores to assess how well the model distinguishes between clicked and non-clicked ads. Dimensionality reduction techniques were also used for exploratory analysis to visualize how user interactions cluster across outcomes.

**Key Findings**

The model showed that feature interactions play a meaningful role in predicting ad clicks. Contextual combinations, particularly those involving device usage and timing, consistently improved predictive performance. Compared to simpler models, the Wide & Deep approach was better able to capture both high-signal rules and subtler nonlinear trends in the data.

**Business Relevance**

From a business perspective, this approach helps improve how ads are delivered by identifying users who are more likely to engage. More accurate click predictions can reduce wasted impressions, support smarter ad placement decisions, and improve overall return on ad spend. The model framework is flexible and can be extended to larger or more granular datasets used in real advertising systems.

**Tools and Technologies**

Python
TensorFlow / Keras
Pandas, NumPy
Scikit-learn
