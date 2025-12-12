Breast Cancer Prediction using KNN and K-Means

This project uses machine learning to classify breast cancer diagnoses as Malignant (M) or Benign (B) using the Breast Cancer Wisconsin dataset. Both unsupervised and supervised learning techniques are demonstrated.

Approach
1. Data Preprocessing

Dropping irrelevant columns: Removed id and Unnamed: 32 to reduce noise.

Encoding: Converted diagnosis to numeric:

M → 1 (Malignant)

B → 0 (Benign)

Feature-target split: Features stored in X, target in y.

Normalization: Applied Min-Max Scaling to scale all features between 0 and 1.

Train-test split: 80% data for training, 20% for testing.

2. K-Means Clustering (Unsupervised Learning)

Applied K-Means with k=2 to cluster the data without using labels.

Observation: Cluster labels were compared with actual diagnosis labels to see how well unsupervised clustering separates benign and malignant cases.

3. K-Nearest Neighbors (KNN) Classifier (Supervised Learning)

Training: KNN classifier trained with k=5 on the training set.

Prediction: Model tested on the 20% unseen test data.

Results

KNN Model Performance:

Metric	Score
Accuracy	0.9649
Precision	0.9535
Recall	0.9535
F1-Score	0.9535

Classification Report:

Class 0 (Benign): Precision 0.97, Recall 0.97

Class 1 (Malignant): Precision 0.95, Recall 0.95

The model shows high accuracy and reliably classifies both benign and malignant cases.

