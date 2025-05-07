# 📊 Lecture 3: Data (Slides 46–60)
**Data Preprocessing & Data Mining Functionalities**

---

## 🔎 Slide 46–48: Data Preprocessing

**Why Preprocessing?**  
Raw data is often:
- Noisy
- Incomplete
- Inconsistent

**Preprocessing =** Essential for improving data quality before applying data mining algorithms.

---

## 🔎 Slide 49: Data Cleaning

**Goal:**  
Fix or remove incorrect, missing, or irrelevant data.

| Problem         | Solution                                 |
|-----------------|-----------------------------------------|
| Missing values  | Ignore, fill with mean/mode, predict missing value |
| Noisy data      | Smoothing, binning, regression          |
| Inconsistent data | Correct using validation rules or external sources |

**Example:**  
Missing patient age → Replace with average age.

---

## 🔎 Slide 50: Data Integration

**Goal:**  
Combine data from multiple sources into a consistent format.

**Challenges:**  
Different databases may have different formats or conflicting data.

**Example:**  
Merge patient records from multiple hospitals.

**Key Point:**  
Integration may lead to redundancy → Handled using entity resolution and duplicate detection.

---

## 🔎 Slide 51: Data Transformation

**Goal:**  
Convert data into a suitable format for mining.

| Method         | Purpose                                     |
|----------------|---------------------------------------------|
| Normalization  | Scale data to a standard range (e.g., 0–1)   |
| Aggregation    | Summarize data                              |
| Generalization | Replace detailed data with higher-level concepts |

**Example:**  
Change "Salary = 60000" → "Income Level = Medium".

---

## 🔎 Slide 52: Data Reduction

**Goal:**  
Reduce data volume while preserving meaningful information.

| Method                | Purpose                                  |
|-----------------------|-----------------------------------------|
| Dimensionality Reduction | Reduce number of variables            |
| Numerosity Reduction  | Replace data with smaller representations (e.g., sampling, clustering) |

**Why Important?**  
Smaller data → Faster algorithms and simpler models.

---

## 🔎 Slide 53: Data Discretization

**Goal:**  
Convert continuous data into categorical form.

| Original | Discretized |
|----------|-------------|
| Age = 25 | Young       |
| Age = 45 | Middle-aged |
| Age = 70 | Senior      |

**Why?**  
Many algorithms work better with categorical data.

---

## 🔎 Slide 54: Summary of Preprocessing Tasks

| Task          | Purpose                           |
|---------------|----------------------------------|
| Cleaning      | Fix errors, fill missing values  |
| Integration   | Combine data from different sources |
| Transformation| Convert data into suitable format |
| Reduction     | Simplify data                    |
| Discretization| Turn continuous data into categories |

---

## 🔎 Slide 55: Data Mining Functionalities – Overview

**Main Question:**  
*What can we do with preprocessed data?*

**Two major categories:**
- **Descriptive tasks** → Summarize data and find patterns.
- **Predictive tasks** → Use data to predict future outcomes.

---

## 🔎 Slide 56: Descriptive Tasks

| Task                  | Description                            | Example                                     |
|-----------------------|----------------------------------------|---------------------------------------------|
| Clustering            | Group similar data points              | Group customers by buying behavior          |
| Association Rule Mining | Discover relationships between variables | "People who buy diapers often buy beer." |
| Summarization         | Provide compact descriptions of data   | Average income by age group                 |

---

## 🔎 Slide 57: Predictive Tasks

| Task             | Description                        | Example                                       |
|------------------|------------------------------------|-----------------------------------------------|
| Classification   | Assign data to predefined categories | Predict if a loan applicant is high-risk or low-risk |
| Regression       | Predict a continuous value          | Forecast next month’s sales                   |
| Anomaly Detection| Identify unusual data points        | Fraud detection in banking                    |

---

## 🔎 Slide 58: Clustering vs. Classification

| Aspect       | Clustering                    | Classification                       |
|--------------|------------------------------|-------------------------------------|
| Labels       | No predefined labels         | Uses predefined labels              |
| Purpose      | Find natural groupings       | Assign new data to known categories |
| Example      | Segment customers            | Classify emails as spam or not spam |

---

## 🔎 Slide 59: Classification vs. Regression

| Aspect   | Classification                  | Regression                      |
|----------|---------------------------------|--------------------------------|
| Output   | Category/label                  | Numeric value                  |
| Example  | Disease diagnosis (Yes/No)      | Predicting house prices        |

---

## 🔎 Slide 60: Summary – Data Mining Functionalities

| Category    | Tasks                                        |
|-------------|----------------------------------------------|
| Descriptive | Clustering, Association Rule Mining, Summarization |
| Predictive  | Classification, Regression, Anomaly Detection |

**Key Message:**  
*The choice of data mining functionality depends on the problem you are trying to solve!*

---

## ✅ Quick Recap of Slides 46–60

| Topic                 | Key Points                                                      |
|-----------------------|------------------------------------------------------------------|
| Data Preprocessing    | Cleaning, integration, transformation, reduction, discretization |
| Data Mining Functionalities | Descriptive (clustering, association, summarization) and Predictive (classification, regression, anomaly detection) |
| Importance            | Preprocessing ensures data quality → leads to better mining results |
