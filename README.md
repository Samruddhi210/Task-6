# Task-6
Elevate Labs Internship Task 6:
This project implements and evaluates the K-Nearest Neighbors (KNN) Classification Algorithm using the classic Iris dataset. The objective was to understand the working of the KNN model on a multiclass classification problem through feature preprocessing, model tuning, performance evaluation, and decision boundary visualization. The dataset used (Iris.csv) contains four numerical features (sepal and petal dimensions) and one categorical target (Species) with three distinct flower classes: Setosa, Versicolor, and Virginica. The data was first loaded using pandas, and the Id column was dropped as it did not contribute to the classification task. Features were then normalized using StandardScaler to ensure all attributes contribute equally to the Euclidean distance-based KNN algorithm.

A KNN classifier was trained using KNeighborsClassifier from Scikit-learn. The dataset was split using train_test_split, ensuring stratified sampling for class balance. Various values of k (number of neighbors) from 1 to 20 were tested to observe the impact on accuracy. These results were visualized using accuracy vs. k plots, and further compared through train vs. test accuracy plots to analyze overfitting or underfitting behavior. The best-performing k value was chosen based on test accuracy.

Model evaluation was conducted using standard classification metrics such as accuracy score, confusion matrix, and classification report. A heatmap visualization of the confusion matrix was also created using seaborn for enhanced interpretability. To better understand the model’s fairness, per-class accuracy was computed from the confusion matrix.

To visualize how KNN separates classes in space, Principal Component Analysis (PCA) was applied to reduce the four-dimensional dataset into two dimensions. KNN was retrained on this reduced dataset, and decision boundaries were visualized using a 2D contour plot. This offered a clear and intuitive view of how different regions of the feature space were classified into flower categories.

Innovative and optional enhancements included plotting train/test accuracy curves, per-class accuracy analysis, confusion matrix heatmaps, and PCA-based decision boundary visualizations. Further suggestions were included such as using t-SNE for nonlinear embeddings, cross_val_score for model stability validation, GridSearchCV for hyperparameter tuning, and wrapping the entire process in a Pipeline for cleaner code and modularity.

📁 Files Included:
Iris.csv: Original dataset used for training and testing the model.
database.sqlite: SQLite version of the dataset (unused in this task).
KNN_Iris_Classification_Task6.md: Markdown summary of the complete KNN project.
