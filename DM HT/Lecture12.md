# 🗄 Lecture 3 (Slides 17–35)
**Data Quality, Data Preprocessing, and Data Types**

---

## 🔎 Slide 17: Issues Related to Data

**Common data problems:**
- **Missing values** → Empty fields.
- **Noise** → Random errors or irrelevant data.
- **Inconsistencies** → Conflicting or duplicate records.
- **Outliers** → Data points very different from others.
- **Redundancy** → Repeated information.

**🔥 Example:**  
- Patient’s age = "200" → Outlier.  
- Blood pressure missing → Missing value.

---

## 🔎 Slide 18: Data Quality

**Four dimensions of data quality:**

| Dimension    | Meaning                    | Example                          |
|--------------|---------------------------|----------------------------------|
| Accuracy     | Data is correct and reliable | Correct spelling of names        |
| Completeness | No missing values            | All patients’ blood pressure recorded |
| Consistency  | No contradictions            | Same patient has consistent gender |
| Timeliness   | Data is up to date           | Last month’s data used instead of last year’s |

**Note:** Poor quality data → Poor models!

---

## 🔎 Slide 19–20: Handling Missing Data

| Method          | Description                                             |
|-----------------|---------------------------------------------------------|
| Ignore the record | Remove rows with missing data (if few missing records). |
| Manual input    | Human expert fills missing values.                       |
| Mean/Mode imputation | Replace missing values with average or most common value. |
| Prediction      | Use a model to estimate missing values.                  |

⚠ **Note:**  
Imputation can introduce bias — use carefully.

---

## 🔎 Slide 21–22: Handling Noisy Data

| Method     | Description                                           |
|------------|-------------------------------------------------------|
| Binning    | Sort data and smooth values in each bin.              |
| Regression | Fit a function (like a line) and remove deviations.   |
| Clustering | Group similar data points and treat outliers separately.|

**Noise reduction → Cleaner, more accurate data mining.**

---

## 🔎 Slide 23: Data Transformation

| Method         | Purpose                        | Example                         |
|----------------|-------------------------------|--------------------------------|
| Normalization  | Scale values to a small range | Age scaled from 0–100 to 0–1   |
| Aggregation    | Summarize data                | Daily sales → Monthly sales     |
| Generalization | Broader categories            | "21 years old" → "Young adult" |

**Why?**  
Some algorithms work better when data is scaled or simplified.

---

## 🔎 Slide 24–25: Feature Selection & Feature Extraction

### 🔷 Feature Selection
- Choose the most important variables.
- Removes irrelevant or redundant data.

### 🔷 Feature Extraction
- Create new features from existing ones.
- **Example:** Combine "Height" and "Weight" → BMI.

**Result:**  
Simpler models, faster training, better accuracy.

---

## 🔎 Slide 26–27: Data Reduction

| Method                | Purpose                                  |
|-----------------------|-----------------------------------------|
| Dimensionality Reduction | Reduce number of variables (e.g., PCA) |
| Numerosity Reduction  | Reduce volume of data (e.g., sampling, clustering) |

**Why?**  
Helps deal with high-dimensional data (avoids the curse of dimensionality).

---

## 🔎 Slide 28: Types of Data Attributes

| Attribute Type | Description                   | Example                               |
|----------------|-------------------------------|--------------------------------------|
| Nominal        | Categories without order      | Gender: Male/Female                  |
| Ordinal        | Ordered categories            | Education level: High School < Bachelor < Master |
| Interval       | Ordered, equal intervals, no true zero | Temperature in Celsius         |
| Ratio          | Ordered, equal intervals, true zero | Weight, Age                      |

---

## 🔎 Slide 29–30: Data Types – Example Table

| Attribute        | Type        |
|------------------|-------------|
| Sex              | Nominal     |
| Blood Pressure   | Ratio       |
| Chest Pain Type  | Ordinal     |
| Age              | Ratio       |

⚡ **Tip:**  
Knowing attribute types helps select the right algorithms (some require numerical data, others work with categories).

---

## 🔎 Slide 31: Structured vs. Unstructured Data

| Type         | Description                   | Example                        |
|--------------|-------------------------------|--------------------------------|
| Structured   | Organized in rows and columns | Databases, spreadsheets        |
| Unstructured | No predefined format          | Text documents, images, videos |

---

## 🔎 Slide 32–33: Static vs. Dynamic Data

| Type    | Description                      | Example                       |
|---------|----------------------------------|-------------------------------|
| Static  | Data doesn’t change over time    | Archived census data          |
| Dynamic | Data updates regularly           | Stock market prices, social media feeds |

**Important:**  
Dynamic data often requires real-time data mining techniques.

---

## 🔎 Slide 34: Single vs. Multidimensional Data

| Type              | Description                | Example                          |
|-------------------|----------------------------|----------------------------------|
| Single-Dimensional | One feature                 | Height only                      |
| Multidimensional   | Multiple features           | Height, Weight, Age, Gender      |

**Note:**  
Data warehouses typically store multidimensional data for advanced analysis.

---

## 🔎 Slide 35: Summary – Why Data Matters

| Aspect             | Importance                                                   |
|--------------------|--------------------------------------------------------------|
| Data Quality       | Affects the accuracy and reliability of data mining results. |
| Data Type Awareness | Helps choose suitable algorithms and preprocessing methods. |
| Data Preparation   | Takes up 50–70% of the data mining process.                  |

**Key Message:**  
*"Better data → Better mining → Better knowledge."*
