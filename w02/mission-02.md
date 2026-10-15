# Mission 02 - Understand Data

## Research Question

**What does it mean for a Machine Learning system to learn a pattern from data?**

## My Understanding

Machine Learning learns patterns from data instead of depending only on rules written by a programmer. A **dataset** is the complete collection of data that we give to the ML system. Each individual row or example inside the dataset is called a **sample** or **observation**. The information describing each sample is called a **feature**. For example, if I want to predict whether a timing run will pass or fail, features could include clock frequency, temperature and voltage.

A **label or target** is the answer that we want the model to learn to predict. In the timing example, `Pass` or `Fail` can be the target. If the examples already contain the correct target, it is called **labelled data**. If the data contains only the input information without the expected answer, it is called **unlabelled data**. The model learns by finding relationships and patterns between the available features and, when labels are provided, the target.

## Example Dataset

Suppose I have historical data from six timing runs.

| Run | Clock Frequency (MHz) | Voltage (V) | Temperature (°C) | Timing Result |
|---|---:|---:|---:|---|
| 1 | 800 | 1.00 | 25 | Pass |
| 2 | 900 | 1.00 | 30 | Pass |
| 3 | 1000 | 0.95 | 45 | Fail |
| 4 | 850 | 1.00 | 35 | Pass |
| 5 | 1050 | 0.90 | 55 | Fail |
| 6 | 950 | 0.95 | 40 | Fail |

### Features

The features in this dataset are:

- Clock Frequency
- Voltage
- Temperature

### Target

The target is:

**Timing Result → Pass or Fail**

The idea is that an ML model could learn patterns from previous timing runs and then predict whether a new timing run is likely to pass or fail.

## Structured and Unstructured Data

**Structured data** is organized into a fixed format such as rows and columns. The timing dataset above is structured because every run contains the same fields such as frequency, voltage and temperature.

**Unstructured data** does not have the same fixed table format. Examples include images, audio, videos, documents and simulation log text.

## Numerical and Categorical Features

A **numerical feature** contains numbers that represent measurements or quantities. In my dataset, clock frequency, voltage and temperature are numerical features.

A **categorical feature** represents a group or category instead of a continuous numerical measurement. For example, a design corner could contain categories such as `slow`, `typical` and `fast`.

## Labelled and Unlabelled Data

If every timing run contains the correct result such as `Pass` or `Fail`, the examples are labelled. The model can use these known answers during learning.

If I only have frequency, voltage and temperature without knowing whether each run passed or failed, the examples are unlabelled.

## Data Collection and Cleaning

Before using data for Machine Learning, the data needs to be checked and cleaned. Real datasets may contain missing values, incorrect measurements, duplicate records, noisy data or inconsistent labels.

For example, if one timing run has no temperature value, the dataset contains a missing value. If the same type of timing result is written as `Pass`, `PASS` and `P`, the labels are inconsistent and should be cleaned before using the data.

## Why More Data Does Not Always Mean Better Data

Having a large amount of data does not automatically make a Machine Learning model better. If the data contains incorrect values, missing information, wrong labels or examples that do not represent the real problem, the model may learn incorrect patterns.

A smaller dataset containing accurate and representative examples can sometimes be more useful than a very large dataset containing poor-quality information.

## Two Ways Data Quality Can Affect the Model

### 1. Incorrect or Inconsistent Labels

If a timing run that actually failed is incorrectly labelled as `Pass`, the model may learn the wrong relationship between the features and the target. If many labels are incorrect, the predictions can become unreliable.

### 2. Missing or Noisy Measurements

If important values such as temperature or voltage are missing or measured incorrectly, the model does not receive an accurate representation of the situation. This can reduce the quality of the patterns it learns and lead to incorrect predictions.

## Conclusion

This mission helped me understand that data is the foundation of Machine Learning. A model learns from samples, features and targets available in the dataset. I also understood that simply collecting more data is not enough. The data should be accurate, consistent and representative of the actual problem because poor-quality data can result in a poor-quality model.
