# Wool-Sucking Cat Adoption Predictive Modeling
<img src=".\images\cat-sucking-on-blanket-scaled.jpg" alt="Alt Text" width="700" height="400">

**Welcome to the Wool-Sucking Cat Adoption Predictive Modeling project!** 
This repository contains the findings and conclusions of Cat-pstone 1 and Cat-pstone 2, which aimed to develop a predictive model for distinguishing wool-sucking cats from non-suckers. Our ultimate goal was to enhance the cat adoption process and provide better matches between cats and potential owners. The general backstory is that BuddyTheCat, a famous ClikClok influencer, has increased demand for wool-sucking kitties. Unfortunately, however, this behavioral trait is hard to assess manually as it takes a lot of time and trust from the animal. 

# Project Overview
Cat-pstone 1 initially utilized a logistic regression model to identify patterns and factors related to wool-sucking behavior in cats. However, concerns about data integrity and the desire to leverage deep learning techniques led us to Cat-pstone 2. In Cat-pstone 2, we explored the potential of incorporating a multilayer perceptron (MLP) algorithm, a powerful deep learning approach, to improve predictive accuracy.

## Approach
### Data Preprocessing
We paid careful attention to data preprocessing to ensure accurate modeling. In Cat-pstone 1, we imputed missing data using the whole dataset prior to the train/test split. However, in Cat-pstone 2, we addressed data leakage concerns by imputing missing data exclusively within the training set.

### Feature Selection
To streamline the modeling process, we carefully selected predictors. We ended up with a reduced feature set of 25 predictors after one-hot encoding breed group as compared to the original 35 factors.

### Model Selection
Given the small dataset, we decided to leverage the power of deep learning by using a basic multilayer perceptron (MLP) algorithm. The MLP model uses multiple layers of calculations to generate predictions and categorize samples as non-suckers or suckers.

## Key Findings
### Deep Learning vs. Logistic Regression
Deep learning algorithms are renowned for capturing complex hierarchical relationships and patterns. However, in our project, the MLP model did not outperform the logistic regression model in terms of predictive accuracy. Surprisingly, the logistic regression model, even without incorporating grooming as a feature (which was found to be highly predictive in Cat-pstone 1), performed comparably to the MLP model.

### Efficiency and Class Imbalance
One drawback of the MLP model was its significantly slower training and prediction times compared to the logistic regression model. Additionally, the logistic regression model, when trained with balanced class weights, did not require resampling the training data to address class imbalance, unlike the MLP model.

## Conclusion and Recommendations
Based on our extensive experimentation and analysis, we recommend leveraging the logistic regression model with balanced class weights due to its comparable performance and efficiency. Further research can focus on refining the feature set and addressing concerns related to behavioral problems. Additionally, investigating the impact of the grooming feature on predictive accuracy is essential.

Feel free to explore the repository for more details on the data, modeling approaches, and findings. Enjoy your journey into the world of wool-sucking cats!

Note: Please refer to the full report in the repository for a comprehensive overview of the project.
