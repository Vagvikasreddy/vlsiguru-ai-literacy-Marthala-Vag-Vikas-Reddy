# Mission 04 - Understand ML Task Types

## Research Question

**What kinds of problems can Machine Learning solve?**

## My Understanding

Machine Learning can solve different types of problems depending on what output we want from the model. Some common ML task types are classification, regression, clustering, anomaly detection, dimensionality reduction, and recommendation or ranking. The task type is selected based on the problem we are trying to solve and the expected output.

Classification predicts a category such as Pass or Fail, while regression predicts a numerical value such as delay or power. Clustering groups similar data without already knowing the groups. Anomaly detection finds unusual observations that are different from normal data. Dimensionality reduction represents data using fewer dimensions so that complex data can be easier to explore. Recommendation or ranking suggests or orders different options based on their usefulness.

## ML Task Types

### 1. Classification

Classification is used when the output belongs to a category.

For example, an email spam filter can classify an email as `Spam` or `Not Spam`.

**Input:** Email information such as words, sender information and other features.

**Output:** Spam or Not Spam.

---

### 2. Regression

Regression is used when we want to predict a numerical value.

For example, an ML model can predict the price of a house using information such as its size, location and number of rooms.

**Input:** House size, location, number of rooms and other features.

**Output:** Predicted house price.

---

### 3. Clustering

Clustering is used to group similar observations when the groups are not already provided.

For example, customers can be grouped based on similar purchasing behaviour.

**Input:** Customer purchase history and behaviour.

**Output:** Groups of customers with similar characteristics.

---

### 4. Anomaly Detection

Anomaly detection is used to identify unusual observations that are different from normal patterns.

For example, a banking system can identify a transaction that looks very different from the customer's normal transactions.

**Input:** Transaction amount, location, time and other transaction information.

**Output:** Normal or unusual transaction / anomaly score.

---

### 5. Dimensionality Reduction

A dataset can contain many different features, which can make it difficult to understand or analyse. Dimensionality reduction represents the data using fewer dimensions while trying to preserve useful information.

For example, if a dataset contains many different measurements for every observation, dimensionality reduction can create a smaller representation that is easier to explore.

**Input:** Data containing many features.

**Output:** A representation containing fewer dimensions.

---

### 6. Recommendation / Ranking

Recommendation or ranking is used to suggest or order different options.

For example, a movie recommendation system can rank movies based on what a user may be interested in watching.

**Input:** User history, preferences and information about available movies.

**Output:** A ranked list of recommended movies.

---

## Real-World and Semiconductor Examples

| Problem | Task Type | Input | Expected Output |
|---|---|---|---|
| Detect whether an email is spam | Classification | Email information | Spam / Not Spam |
| Predict the price of a house | Regression | Size, location and other house features | Predicted price |
| Group customers with similar behaviour | Clustering | Customer behaviour and purchase data | Groups of similar customers |
| Detect an unusual bank transaction | Anomaly Detection | Transaction information | Unusual observation / anomaly indication |
| Reduce many measurements into fewer dimensions for exploration | Dimensionality Reduction | Dataset containing many measurements | Lower-dimensional representation |
| Recommend movies to a user | Recommendation / Ranking | Viewing history and preferences | Ranked movie recommendations |
| Predict whether a timing run passes or fails | Classification | Timing/design measurements | Pass / Fail |
| Estimate the delay or power of a design | Regression | Design measurements and characteristics | Estimated delay or power |

## Semiconductor Examples

### Timing Pass/Fail Prediction

A Machine Learning model could use measurements from previous design runs and predict whether a new timing run will pass or fail. Since the expected output is a category, `Pass` or `Fail`, this is a **classification** task.

### Delay or Power Estimation

A model could use information about a design to estimate its delay or power. Since the expected output is a numerical value, this is a **regression** task.

## Task Type vs Learning Approach

A task type and a learning approach are not the same thing. A **task type** describes what we want the model to produce, such as a category, numerical value or group. A **learning approach** describes how the model learns, such as supervised, unsupervised or reinforcement learning.

For example, predicting whether a timing run will Pass or Fail is a **classification task**. If we train the model using previous timing runs where the correct Pass/Fail answer is provided, then **supervised learning** is the learning approach.

This means:

```text
Learning Approach
= How does the model learn?

Task Type
= What should the model produce?
```

Different algorithms or learning approaches may sometimes be used to solve similar task types, so knowing that a problem is classification or regression does not by itself explain how the model was trained.

## Conclusion

This mission helped me understand that Machine Learning is not one single type of problem. Classification predicts categories, regression predicts numbers, clustering finds groups, anomaly detection finds unusual observations, dimensionality reduction simplifies data, and recommendation or ranking orders useful choices. I also understood that ML task types should not be confused with learning approaches because one describes the expected output while the other describes how learning happens.
