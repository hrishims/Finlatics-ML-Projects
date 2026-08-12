# Wine Quality Classification — Decision Tree vs. Random Forest

Analyzed physicochemical properties of red wine samples to identify what drives wine quality, then trained classification models to predict it.

## Dataset
1,599 red wine samples with 11 physicochemical features (fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free/total sulfur dioxide, density, pH, sulphates, alcohol) and a quality score (0–10 scale).

## Approach
- Checked for and handled missing values
- Explored the distribution of quality scores (most frequent, highest, lowest)
- Examined correlations between individual features (fixed acidity, alcohol, free sulfur dioxide, volatile acidity) and quality
- Compared average residual sugar between the best- and worst-rated wines
- Trained a Decision Tree Classifier and a Random Forest Classifier (80/20 train-test split) to predict quality
- Compared train vs. test accuracy across both models, and tested accuracy across a range of tree depths to visualize overfitting

## Key Findings
- Quality scores were concentrated around 5–6, with few samples at the extremes (min: 3, max: 8)
- Alcohol content showed a clear positive relationship with quality — average alcohol rose from ≈ 9.9% for the lowest-rated wines to ≈ 12.1% for the highest-rated
- Volatile acidity showed a moderate negative correlation with quality (≈ −0.39) — higher volatile acidity tended to mean lower quality
- Fixed acidity and free sulfur dioxide showed weak correlation with quality
- Random Forest outperformed the Decision Tree on test accuracy (≈ 66% vs. ≈ 56%), but showed clear overfitting (≈ 99% training accuracy vs. ≈ 66% test accuracy)

## Tools
Python, Pandas, Scikit-learn, Matplotlib
