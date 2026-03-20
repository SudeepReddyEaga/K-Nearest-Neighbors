# K-Nearest-Neighbors
K-Nearest Neighbors (KNN) is a simple, intuitive supervised machine learning algorithm used for both classification and regression. It is based on the idea that "similar things exist in close proximity"—often summarized by the phrase "birds of a feather flock together". 

How It Works
The algorithm doesn't "learn" a model in the traditional sense; instead, it memorizes the entire training dataset. When a new data point needs to be predicted, KNN performs these steps: 
Choose 'K': Select the number of nearest neighbors to consider (e.g., K=3 or K=5).
Calculate Distance: Measure the distance between the new point and all points in the training set, typically using Euclidean distance.
Identify Neighbors: Sort these distances and pick the top 
 closest points.
Vote or Average:
Classification: The new point is assigned to the class that is most common among its 
 neighbors (majority voting).
Regression: The new point is assigned the average value of its neighbors. 

Key Characteristics
Lazy Learner: It has no specialized training phase and performs all calculations at the time a prediction is requested.
Non-Parametric: It makes no assumptions about the underlying distribution of the data.
Sensitive to Scale: Because it relies on distance, features with larger numerical ranges can dominate the model. Feature scaling (normalization or standardization) is usually required. 

Pros and Cons
Pros 	                                                    Cons
Easy to understand and implement.	                        Computationally expensive as the dataset grows.
No training time required.	                              High memory usage since it must store all data.
Naturally handles multi-class classification.	            Sensitive to noisy data and outliers.
Real-World Examples
Recommendation Systems: Companies like Netflix and Amazon use KNN to find users with similar viewing or buying habits to suggest new content.
Medical Diagnosis: Predicting the likelihood of diseases by comparing a patient's data to historically similar cases.
Finance: Used for credit rating and detecting fraudulent transactions by identifying "neighboring" patterns of normal versus suspicious behavior. 
