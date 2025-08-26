# Why Use Statistical Methods in Model Evaluation

When evaluating a model, relying solely on metrics like **accuracy**, **ROC AUC**, **recall**, **precision**, or **F1-score** is not enough. These metrics only provide a snapshot of performance at the output level but **do not explain model capacity, statistical risk, or generalization ability**. Therefore, it is important to use the following statistical methods:

## 1. Rademacher Complexity

Rademacher Complexity measures the **capacity of a model to fit the data**. This is important because:

- It shows how flexible a model is in capturing patterns in the data.
- It helps detect potential overfitting or underfitting theoretically.
- It provides a statistical understanding of model complexity, not just performance on a specific dataset.

## 2. Hoeffding Excess Risk Bound

The Hoeffding Bound estimates the **excess risk** of a model compared to the optimal risk. Its importance lies in:

- Providing a probabilistic bound on model performance.
- Indicating the confidence level that the model will perform well on unseen data.
- Adding a statistical dimension to evaluation, which is usually limited to deterministic metrics.

## 3. Train Risk, Test Risk, and Generalization Gap

Evaluating these aspects is crucial to understand:

- **Train Risk** → how well the model fits the training data.
- **Test Risk** → how well the model performs on unseen data.
- **Generalization Gap** → the difference between train and test risk, indicating the model’s ability to generalize.

Without this analysis, we only know performance on a specific dataset, but **cannot determine if the model is overfitting or underfitting**.

## 4. Bias-Variance Trade-off

Bias-variance analysis explains the **source of model errors**:

- **High Bias** → model is too simple → underfitting.
- **High Variance** → model is too complex → overfitting.
- **Optimal Trade-off** → model is complex enough to capture patterns but still generalizable.

This is important because standard metrics cannot distinguish whether errors come from bias or variance.

---

## References

- [Math for ML](https://drive.google.com/file/d/1R3vDKh1nuPJs6NsMfuPAKxjjnSc9wUTP/view?usp=drive_link)  

