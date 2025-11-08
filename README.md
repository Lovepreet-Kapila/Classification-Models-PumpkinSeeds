# Classification-Models-PumpkinSeeds
A machine learning project to classify two varieties of pumpkin seeds (Çerçevelik and Ürgüp Sivrisi) using a public dataset.

This project demonstrates a full classification pipeline, from data loading to model evaluation and interpretation. It compares three different classification algorithms and uses PCA for visualizing the complex, high-dimensional decision boundaries.

**Objectives**
Implement and compare three powerful classifiers: Decision Tree, Random Forest, and Support Vector Machine (SVM).

Use Principal Component Analysis (PCA) to reduce the dataset's 12 features to 2 components for visualization.

Plot the 2D decision boundaries to visually understand how each model separates the data.

Analyze feature importance from the Random Forest model to identify the most predictive physical measurements.

**Tech Stack**
Language: Python 3

Libraries: Scikit-Learn (for all models and PCA), Pandas, NumPy

Visualization: Matplotlib, Seaborn

**Tools:** Jupyter Notebook

**Techniques Explored**
**1. Classification Models**
Decision Tree: A simple, interpretable model that splits data based on feature thresholds.

Random Forest: An ensemble model that builds multiple decision trees and merges them to get a more accurate and stable prediction. It's also excellent for preventing overfitting.

Support Vector Machine (SVM): A powerful classifier that finds the optimal "hyperplane" that best separates the two classes.

**2. PCA for Visualization**
The original dataset has 12 features (like Area, Perimeter, Major_Axis_Length, etc.), making it impossible to visualize.

PCA was used to transform these 12 dimensions into 2 "principal components" that capture the most variance.

This 2D data was then used to plot the decision boundaries, allowing us to "see" how each model made its decisions.

**3. Feature Importance**
The Random Forest model was used to rank which of the 12 features were most important for a successful classification.

This provides real-world, interpretable insights (e.g., "Seed shape, not size, was the most important factor").

**What I Learned**

Model Comparison is Key: All three models performed well, but the Random Forest and SVM were slightly more robust and accurate, likely due to their ability to handle complex, non-linear relationships.

Interpreting "Black Box" Models: While an SVM is powerful, its decision boundary can be hard to interpret. A Random Forest provides a great balance of high accuracy and interpretability through its feature importance rankings.

PCA as a Storytelling Tool: Learned that PCA is not just a preprocessing step but a powerful tool for communicating a model's results. Visualizing the decision boundaries made the difference between the models immediately obvious.
