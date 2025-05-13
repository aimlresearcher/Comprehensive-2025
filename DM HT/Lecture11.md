# 🗄 Data Storage (Slides 14–16)

---

## 🔎 Slide 14: Data Storage

**Key Idea:**  
The way data is stored affects how easily it can be accessed, queried, and used for data mining.

**Main storage types:**
- Flat Files
- Relational Databases (RDB)
- Data Warehouses (DW)

---

## 🔎 Slide 15: Flat Files

**Description:**  
Simplest form of data storage.  
Data is saved as plain text—rows and columns separated by commas, tabs, or other delimiters.

**Example:**

| Name         | Age | Gender | Blood Pressure |
|--------------|-----|--------|----------------|
| Konrad Black | 31  | Male   | 130            |
| Magda Doe    | 26  | Female | 115            |

**Advantages:**
- Easy to create and edit.
- Portable and readable in many programs (Excel, Notepad, etc.).

**Disadvantages:**
- Cannot handle complex relationships.
- Not ideal for large datasets.
- Lacks advanced querying (beyond basic search or filter).

✅ **Best For:**  
Small or simple datasets where advanced data manipulation isn’t needed.

---

## 🔎 Slide 16: Relational Databases (RDB) and Data Warehouses (DW)

### 🔷 Relational Databases (RDB)

**Description:**  
Stores data in tables (relations).  
Tables can be connected using **primary keys** and **foreign keys**.  
Uses **SQL (Structured Query Language)** for data retrieval.

**Example:**

| Patients Table  |            | Blood Pressure Table |          |
|-----------------|------------|----------------------|----------|
| PatientID       | Name       | PatientID            | BP_Value |
| 1               | Konrad Black | 1                  | 130.0    |

**Advantages:**
- Handles large structured datasets efficiently.
- Supports complex queries and multi-user access.

**Disadvantages:**
- Requires technical knowledge to set up and manage.
- Less suitable for unstructured data (like images, videos).

---

### 🔷 Data Warehouses (DW)

**Description:**  
Combines data from multiple sources into one large system.  
Optimized for querying, reporting, and data mining.

**Structure:**
- Uses schemas (e.g., **star schema**, **snowflake schema**).
- Stores cleaned and transformed data in a central repository.

**Example:**  
Combines patient data from:
- Edmonton Clinic
- San Diego Clinic
- Denver Clinic

**Advantages:**
- Supports complex analytical queries.
- Excellent for historical analysis and trend detection.
- Facilitates enterprise-wide data mining.

**Disadvantages:**
- High cost and setup complexity.
- Not designed for real-time data updates.

---

## ✅ Comparison Table

| Storage Type   | Structure                | Best For                    | Limitations                          |
|----------------|-------------------------|-----------------------------|-------------------------------------|
| Flat Files     | Simple tables            | Small, simple datasets      | Not scalable, no complex queries    |
| Relational DB  | Related tables (SQL)     | Medium-large structured data| Requires technical setup            |
| Data Warehouse | Integrated multi-source data | Large-scale analytical tasks | High cost, not for real-time use |

---

## 🔎 Why Does Storage Matter for Data Mining?

- **Efficient Access:** DM algorithms need quick access to large volumes of data.
- **Integration:** Data often comes from multiple sources → warehouses help consolidate it.
- **Performance:** Storage method affects speed, scalability, and accuracy in data mining.
