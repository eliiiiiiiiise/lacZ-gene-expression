# Predicting lacZ Gene Expression Using Neural Networks

## Project Overview

This project explores the use of deep learning to predict the expression level of the lacZ gene from the expression levels of 45 other genes.

Using Python and PyTorch, I developed and iteratively refined a neural network model to investigate whether patterns in the expression of other genes could help predict lacZ expression. The project involved exploratory data analysis, data preprocessing, neural network experimentation, feature selection, and model evaluation.

A key focus was exploring different modelling strategies and regularisation techniques while assessing the limitations of applying neural networks to the available biological data.

## Objectives

Explore relationships between gene expression features and the target gene, lacZ.

Investigate whether the expression levels of 45 other genes can help predict lacZ expression.

Develop and refine a neural network architecture for a regression task.

Experiment with regularisation techniques and feature selection methods.

Evaluate the final model on a held-out test dataset and analyse its predictive limitations.

## Tools

Python: Main programming language

Jupyter Notebooks: Interactive analysis and experimentation

pandas: Data manipulation and preprocessing

PyTorch: Neural network implementation and training

scikit-learn: Data preprocessing, feature selection, and model evaluation

## Methodology

1. Exploratory Data Analysis

I began by exploring the dataset to understand the available gene expression measurements and the relationships between the 45 input features.

I investigated correlations between features to identify potential relationships and better understand the structure of the data before building the model.

This initial analysis helped inform the subsequent preprocessing and modelling steps.

2. Data Preprocessing and Feature Selection

I prepared the data for neural network training and explored different feature selection approaches to investigate whether using a subset of the available genes could improve predictive performance.

Feature selection was an important part of the experimentation, as not all input features necessarily provide equally useful information for predicting the target gene's expression.

3. Neural Network Development

I implemented a neural network in PyTorch and iteratively experimented with different model configurations to identify an appropriate architecture for the regression task.

The experimentation included:

Refining the neural network architecture

Applying regularisation techniques to help control overfitting

Experimenting with batch normalisation and dropout

Testing different feature selection approaches

These experiments allowed me to investigate how architectural choices, regularisation, and input feature selection affected the model's predictive performance.

4. Model Evaluation

I evaluated the final model on a held-out test dataset using the coefficient of determination ((R^2)).

The final model achieved an R² close to 0 on the test dataset. This indicates that the model explained very little of the variation in lacZ expression compared with a baseline that predicts the mean target value.

The result highlighted the difficulty of predicting the target gene's expression from the available input features using the tested neural network approach. It also demonstrated the importance of evaluating model performance on unseen data rather than relying solely on training results.

## Results and Key Takeaways

Developed a neural network regression model using PyTorch.

Investigated relationships between 45 gene expression features and the target gene.

Experimented with neural network architecture, regularisation, batch normalisation, dropout, and feature selection.

Evaluated predictive performance using a held-out test dataset.

Identified limitations in the model's ability to predict lacZ expression from the available data.

Although the final model achieved an R² close to zero, the project provided an opportunity to investigate the challenges of deep learning with biological data and to evaluate how different modelling choices affect predictive performance.

## Conclusion

This project gave me practical experience in developing and evaluating neural networks for a biological regression problem. It involved more than implementing a model: I explored feature relationships, tested alternative modelling configurations, and assessed the final results critically.

The findings highlight that neural network complexity alone does not guarantee predictive performance. The usefulness of the input features, the quality of the data, and the underlying relationships between variables all matter when developing predictive models.

