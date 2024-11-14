
# Skincare Reaction Prediction Model

##  Project Overview

This project aims to predict skin reactions based on various user-specific attributes, including skin type, age, melanin concentration, and the concentration of specific skincare ingredients. 

By analyzing these factors with machine learning, the model helps develop inclusive skincare recommendations for diverse skin types.

### Methodology

#### 1. Data Collection and Preprocessing

Attributes Analyzed: Age, melanin concentration, collagen amount, epidermis thickness, hydration level, skin type, ingredient used, and ingredient concentration.

Target Variable: The model predicts Reaction with possible outcomes like Neutral, Positive, Brightening, Irritation, and Negative.

##### Preprocessing Steps:

Cleaned missing values and handled inconsistencies in data.

Standardized the input values to ensure consistency across skin types, ingredient concentrations, and reactions.

#### 2. Data Encoding
   
One-Hot Encoding: Used for categorical columns (Skin Type and Ingredient) to transform them into a numerical format compatible with machine learning algorithms.

Feature Matrix: Combined the one-hot encoded columns with other numerical attributes to create the final feature matrix.

#### 3. Model Selection and Training
   
Three machine learning models were implemented and tested to predict skincare reactions:

Random Forest Classifier (RFC): Selected for its robustness and ability to handle complex data relationships. Achieved the highest accuracy and precision in predictions.

Naïve Bayes (NB): Tested for its simplicity and efficiency, though it showed moderate accuracy.

Support Vector Machine (SVM): Evaluated for potential precision, though it did not perform as effectively in this application.

#### Training Process:

Split Dataset: Divided the data into training (70%) and testing (30%) sets.

Train Models: Each model was trained on the training set and tuned to maximize performance.

Feature Importance (RFC): Analyzed feature importance in RFC to understand which attributes most influenced skincare reactions.

#### 4. Model Evaluation
   
Metrics Used: Accuracy, Precision, and Confusion Matrix.

### Performance Summary:

RFC: Achieved an accuracy of 98% with high precision across all classes, especially for Brightening and Neutral reactions.

NB: Achieved 86% accuracy but showed lower precision in Brightening and Positive predictions.

SVM: Displayed an accuracy of 21%, indicating challenges in classifying reactions accurately.

### Results

Model	Accuracy	Notable Precision for Brightening	Notable Precision for Neutral

Random Forest	98%	1.00	0.99

Naïve Bayes	86%	0.33	0.45

Support Vector Machine	21%	0.10	0.05

The Random Forest Classifier was selected as the final model due to its superior accuracy and precision in predicting the skin reaction classes.

### Conclusion

This model highlights the potential of machine learning to provide inclusive, personalized skincare recommendations. 

By continuously iterating with new data, skincare companies can improve product efficacy and target diverse skin types more effectively.

