# Machine Learning Models and Statistical Analysis
We utilized two distinct datasets to predict developers' patch acceptance. Below is a description of each dataset and the corresponding analysis:

Dataset 1:
Features: Eye gaze metrics (e.g., fixation rate, average fixation time on 6 AOIs) and patch correctness.
Target: Patch acceptance.

Analysis:

Supervised Learning:
Applied four machine learning algorithms: Logistic Regression, Random Forest, Gradient Boosting Classifier, and Support Vector Machine.
The results are provided in ml-models.ipynb.
Additionally, AutoML.ipynb uses H2O for predictions on this dataset.

Requirements:
Place dataset_1.csv in the root directory.

Results:
The best performance was achieved by Logistic Regression with an accuracy of 84\%, recall of 90\%, precision of 80\%, and F1-score of 85\%. The most significant feature was patch correctness.
Unsupervised Learning:
Applied clustering approaches both with and without the patch acceptance feature.
Folders and Files:

clustering_with_acceptance/:
Contains clustering_with_acceptance.ipynb for clustering algorithms and statistical_test.ipynb for statistical tests to identify significant differences between features in different clusters.

Requirements: dataset_1.csv in the root directory.

Results: Clustering with patch acceptance produced three categories, with results saved in clustering_with_acceptance.csv.

clustering_without_acceptance/:
Contains clustering_without_acceptance.ipynb for clustering algorithms and statistical_test.ipynb for statistical tests.

Requirements: dataset_1.csv in the root directory.

Results: Clustering without patch acceptance produced two categories, with results saved in clustering_without_acceptance.csv.

Dataset 2:
Features: Task priority level, patch author's experience level, and task difficulty.
Target: Patch acceptance.

Analysis:

Applied four machine learning algorithms: Logistic Regression, Random Forest, Gradient Boosting Classifier, and Support Vector Machine.
The results are provided in ml-models.ipynb.
Additionally, AutoML.ipynb uses H2O for predictions on this dataset.

Requirements:
Place dataset_2.csv in the root directory.

Results:
The best performance was achieved by Logistic Regression with an accuracy of 51\%, recall of 95\%, precision of 50\%, and F1-score of 65\%. The most significant feature was task difficulty.
The second dataset did not provide as strong results as the first dataset.