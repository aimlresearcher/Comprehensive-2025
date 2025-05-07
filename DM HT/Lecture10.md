# 📖 Lecture 3: Data (Slides 4–13)

---

## 🔎 Slide 4: Introduction

**Key Point:**  
The success of data mining and knowledge discovery (KDP) heavily depends on:

- **Quality of data**
- **Quantity of data**

**Three focus areas:**
- **Data types** → What kind of data we are dealing with.
- **Data storage techniques** → How data is stored.
- **Amount and quality of data** → How much data we have and how clean/reliable it is.

These are the foundation for performing KDP effectively.

---

## 🔎 Slide 5: Attributes, Data Sets, and Data Storage

**Key Concepts:**
- **Attribute / Feature:** A property of data (e.g., "Age", "Blood Pressure").
- **Value:** The specific data point (e.g., 35 years, 130 mmHg).
- **Object:** An entity described by multiple features (e.g., a patient).
- **Data Set:** A collection of objects.

**Storage modes:**
- Flat files → Simple tables.
- Databases → Structured storage.
- Data Warehouses → Integrated collections from multiple sources.

---

## 🔎 Slide 6: Example – Attributes, Data Sets, and Storage
![My Diagram](https://github.com/aimlresearcher/Comprehensive-2025/blob/main/DM%20HT/images/img05.png?raw=true)

**Example:** *Heart Clinic Patient Data*

| Patient | Sex   | Blood Pressure | Chest Pain Type |
|---------|-------|----------------|-----------------|
| 1       | Male  | 117.0          | 3               |
| 2       | Female| 130.0          | 1               |
| 3       | Female| 102.0          | 1               |

**Types of values:**
- Numerical → 117.0, 130.0.
- Symbolic → Male/Female.

**Features:**
- **Sex:** {male, female}
- **Blood pressure:** [0, 250]
- **Chest pain type:** {1, 2, 3, 4}

**Objects →** Patients  
**Databases →** Edmonton, San Diego, Denver clinics  
**Data Warehouse →** Combines all three clinic databases.

---

## 🔎 Slide 7: Values, Features, and Objects (Basics)

**Types of values:**
- **Numerical:** Real numbers (e.g., 123.5), integers (e.g., 44).
- **Symbolic:** Qualitative concepts (e.g., "Male", "Normal").

---

## 🔎 Slide 8: Features (Detailed)

**Features can be:**
- **Discrete (Categorical):** Few distinct values.
  - *Example:* Chest pain type {1, 2, 3, 4}.
- **Binary:** Only two values (e.g., Yes/No).
- **Continuous:** Many possible values.
  - *Example:* Blood pressure [0, 250].

**Nominal vs Ordinal:**
- **Nominal:** No natural order (e.g., colors).
- **Ordinal:** Has an order (e.g., severity levels).

---

## 🔎 Slide 9: Objects

**Object (Record, Example, Data Point):**  
An entity described by features.

**Types:**
- **Univariate data:** One feature per object.
- **Multivariate data:** Multiple features per object.

**Example:**  
A patient → age, sex, blood pressure, cholesterol, etc.

---

## 🔎 Slide 10: Example – Patient Data
![My Diagram](https://github.com/aimlresearcher/Comprehensive-2025/blob/main/DM%20HT/images/img06.png?raw=true)


| Feature           | Value         | Type                      |
|-------------------|---------------|---------------------------|
| Name              | Konrad Black  | Symbolic                  |
| Sex               | Male          | Symbolic (Binary)         |
| Age               | 31            | Numerical (Discrete Ordinal) |
| Blood Pressure    | 130.0         | Numerical (Continuous)    |
| Cholesterol       | 331.2         | Numerical (Continuous)    |
| Chest Pain Type   | 1             | Discrete Nominal          |

Shows how a real-world entity becomes a data object in data mining.

---

## 🔎 Slide 11: Data Sets

**A data set =** Collection of objects described by the same set of features.

**Storage format:**  
Often as flat files (tables → rows = objects, columns = features).  
Commonly exported from spreadsheets or databases.

---

## 🔎 Slide 12: Example Data Set – Patients

| Name         | Age | Sex   | Blood Pressure | BP Test Date | Cholesterol | Cholesterol Test Date | Chest Pain Type | Defect Type | Diagnosis |
|--------------|-----|-------|----------------|--------------|-------------|-----------------------|-----------------|-------------|-----------|
| Konrad Black | 31  | Male  | 130.0          | 05/05/2005   | NULL        | NULL                  | NULL            | NULL        | NULL      |
| Konrad Black | 31  | Male  | 130.0          | 05/05/2005   | 331.2       | 05/21/2005            | 1               | Normal      | Absent    |
| Magda Doe    | 26  | Female| 115.0          | 01/03/2002   | NULL        | NULL                  | 4               | Fixed       | Present   |
| Anna White   | 56  | Female| 120.0          | 12/30/1999   | 45.0        | 12/30/1999            | 2               | Normal      | Absent    |

**Notes:**
- Some values are missing (**NULL**).
- One value (cholesterol = 45.0) is outside acceptable range → **Incorrect**.

---

## 🔎 Slide 13: Data Set Repositories

**Popular sources for data sets:**
- **UCI Machine Learning Repository** → http://www.ics.uci.edu/~mlearn/
- **KDD Archive** → http://kdd.ics.uci.edu/
- **StatLib Repository** → http://lib.stat.cmu.edu/

**These offer:**
- Free data sets.
- Used for benchmarking algorithms.
- Many come with analysis results for comparison.

---

## ✅ Summary of Slides 4–13

| Concept          | Key Points                                           |
|------------------|-----------------------------------------------------|
| Data Importance  | DM/KDP success depends on data quality and quantity. |
| Attributes & Objects | Objects described by features/attributes and their values. |
| Values           | Numerical or symbolic; discrete or continuous.       |
| Data Sets        | Collections of objects described by the same features. |
| Data Storage     | Flat files, databases, data warehouses.              |
| Example          | Patient data showing real-world application.         |
| Data Sources     | UCI ML Repository, KDD Archive, StatLib.             |
