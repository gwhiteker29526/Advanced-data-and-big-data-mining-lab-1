# Advanced-data-and-big-data-mining-lab-1
# KNN vs RNN Classification Lab (Wine Dataset)

## Purpose of the Lab
The purpose of this lab was to explore and compare the performance of two classification algorithms: K-Nearest Neighbors (KNN) and Radius Neighbors (RNN) using the Wine Dataset from sklearn. The goal was to understand how different parameter values (k for KNN and radius for RNN) affect model accuracy and overall classification performance. Additionally, this lab helped build practical experience with training, testing, and evaluating machine learning models.

---

## Key Insights and Observations

- **KNN Performance:**
  - Smaller values of k (such as k=1) tended to overfit the data, resulting in high variance.
  - Moderate values of k (such as 5 or 11) produced more stable and accurate results.
  - Larger k values reduced sensitivity to noise but could lead to underfitting.

- **RNN Performance:**
  - The model was highly sensitive to the choice of radius.
  - Smaller radius values often resulted in too few neighbors, lowering accuracy.
  - Larger radius values included too many points, which reduced classification precision.
  - Feature scaling was important for improving RNN performance.

- **Comparison:**
  - KNN generally produced more consistent and reliable accuracy across different parameter values.
  - RNN required more careful tuning and was less stable overall.
  - KNN is typically more practical for general use, while RNN may be useful when distance thresholds are meaningful.

---

## Challenges and Decisions

One of the main challenges faced during this lab was difficulty connecting to a Python kernel in Jupyter Notebook within VS Code. Initially, the environment was connected to a SQL kernel, which prevented execution of Python code. Resolving this issue required installing the appropriate Python kernel (ipykernel), selecting the correct interpreter, and restarting the environment.

Another challenge was understanding how parameter choices impact model performance. Deciding on appropriate values for k and radius required experimentation and observation of accuracy trends.

Additionally, scaling the dataset was an important decision for improving the performance of the Radius Neighbors model, as it is highly sensitive to feature magnitudes.

---

## Conclusion

This lab demonstrated the importance of parameter tuning in machine learning models. KNN proved to be more stable and easier to optimize, while RNN required more careful handling but provided insight into distance-based classification methods. Overall, this lab reinforced key concepts in model evaluation and selection.
