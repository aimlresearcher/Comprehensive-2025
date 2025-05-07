# 🔴 Comparison of the KDP Models
*(Fayyad et al., Cios et al., CRISP-DM)*

These three models—**Nine-step by Fayyad**, **Six-step by Cios**, and **CRISP-DM**—are widely used frameworks for managing Knowledge Discovery in Databases (KDD) or Data Mining projects.

---

## 📝 1️⃣ Domain of Origin

| Model      | Origin                    |
|------------|--------------------------|
| Fayyad et al. | Academic               |
| Cios et al.   | Hybrid (Academic/Industry) |
| CRISP-DM      | Industry               |

**Key Insight:**  
- Academic models → Focus on technical rigor.  
- Industry models → Emphasize practicality and business relevance.  
- **Cios et al.** → Balances both.

---

## 📝 2️⃣ Number of Steps

| Model      | Steps |
|------------|-------|
| Fayyad et al. | 9 |
| Cios et al.   | 6 |
| CRISP-DM      | 6 |

**Key Insight:**  
- **Fayyad’s model** → More detailed, finer breakdowns.  
- **Cios and CRISP-DM** → Group related activities into broader steps.

---

## 📝 3️⃣ Steps Breakdown

| Step | Fayyad                  | Cios                        | CRISP-DM                  |
|------|-------------------------|-----------------------------|---------------------------|
| 1    | Developing & Understanding the Application Domain | Understanding the Problem Domain | Business Understanding    |
| 2    | Creating a Target Data Set | Understanding of the Data | Data Understanding        |
| 3    | Data Cleaning and Preprocessing | Preparation of the Data | Data Preparation          |
| 4    | Data Reduction and Projection | Combined in Data Preparation | Included in Data Preparation |
| 5    | Choosing the DM Task | Part of Data Mining step    | Part of Modeling step     |
| 6    | Choosing the DM Algorithm | Part of Data Mining step    | Part of Modeling step     |
| 7    | Data Mining              | Data Mining                 | Modeling                  |
| 8    | Interpreting Mined Patterns | Evaluation                 | Evaluation                |
| 9    | Consolidating Discovered Knowledge | Use of the Discovered Knowledge | Deployment               |

**Key Insight:**  
The **core activities** are consistent. Differences lie in how finely steps are divided and grouped.

---

## 📝 4️⃣ Unique Features

| Model      | Notes                                                        |
|------------|--------------------------------------------------------------|
| Fayyad et al. | Technical focus on data analysis. Less business emphasis. |
| Cios et al.   | Combines academic and industrial practices. Explicit feedback loops. |
| CRISP-DM      | Simple vocabulary, strong documentation, emphasizes business understanding. Widely adopted. |

---

## 📝 5️⃣ Supporting Software

| Model      | Software                     |
|------------|-----------------------------|
| Fayyad et al. | MineSet™                  |
| Cios et al.   | N/A                       |
| CRISP-DM      | Clementine® (now IBM SPSS Modeler) |

---

## 📝 6️⃣ Reported Application Domains

| Model      | Domains                                             |
|------------|----------------------------------------------------|
| Fayyad et al. | Medicine, engineering, production, e-business, software |
| Cios et al.   | Medicine, software                               |
| CRISP-DM      | Medicine, engineering, marketing, sales          |

**Key Insight:**  
All models have been successfully applied in medical, engineering, and business domains.

---

## 🔄 7️⃣ Time and Effort Distribution (Slide 30)

| KDP Step              | Effort % (approx.)                     |
|-----------------------|----------------------------------------|
| Understanding of Domain | ~10%                                 |
| Understanding of Data   | ~10–15%                              |
| Preparation of Data     | **50–70% (Most time-consuming)**     |
| Data Mining             | ~10–15%                              |
| Evaluation              | ~5–10%                               |
| Deployment              | ~5%                                  |

**Key Insight:**  
**Data Preparation** often consumes the majority of project time—even with automation tools.

---

## ✅ Summary Table

| Feature          | Fayyad et al. | Cios et al. | CRISP-DM |
|------------------|---------------|-------------|-----------|
| Origin           | Academic      | Hybrid      | Industry   |
| Steps            | 9             | 6           | 6         |
| Feedback Loops   | Limited/implicit | Explicit | Some iteration |
| Business Emphasis| Low           | Medium      | High       |
| Software Support | MineSet™      | None        | Clementine® |
| Main Domains     | Research & engineering | Academic & applied | Industry-focused |

---

## 🔎 Final Takeaway

| Model         | Best For                                         |
|---------------|--------------------------------------------------|
| Fayyad et al. | Technical, research-heavy projects.              |
| Cios et al.   | Flexible academic-industrial collaborations.     |
| CRISP-DM      | Business-driven, real-world applications.        |

All three models share **core steps** but differ in:
- Level of detail.
- Emphasis on business vs. technical aspects.
- Flexibility through feedback loops.
