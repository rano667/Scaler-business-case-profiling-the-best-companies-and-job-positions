# 🔍 Scaler Learner Profiling & Clustering Project

This project focuses on clustering Scaler learners based on their job position, company, compensation, and other related attributes to derive actionable insights about the **best job roles and companies to work for**.

## 🚀 Objective

As part of the Scaler Analytics vertical, this project aims to:
- Segment learners into meaningful clusters using machine learning.
- Identify patterns in salary (CTC), experience, job roles, and company tiers.
- Highlight top-performing roles and companies to support career path optimization.

---

## 📂 Project Structure

| File | Description |
|------|-------------|
| [`Scaler_Clustering_Analysis.ipynb`](https://colab.research.google.com/drive/1Q_gLCFXvKudBEe1-g-omu8ufk0XQrYya?usp=sharing) | Main notebook containing the end-to-end clustering workflow and analysis |
| `README.md` | Project overview and instructions |

---

## 🧪 Methodology

### ✅ 1. Data Preprocessing
- Handled invalid or inconsistent values in `yoe`, `orgyear`, etc.
- Used **KNN imputation** for missing values.
- Encoded categorical variables like `job_position` and `company_hash`.

### 🧠 2. Clustering
- Used **KMeans** clustering (k=5, chosen via elbow method).
- Standardized features for clustering.
- Performed **PCA** for 2D visualization of cluster separation.

### 📊 3. Post-Clustering Analysis
- Cluster-wise summary of:
  - Compensation (`CTC`)
  - Years of experience (`YOE`)
  - Top job roles
  - Top companies (anonymized)
- Applied custom **Designation, Class, and Tier flags** to compare learners within company and job groups.

---

## 🔍 Key Insights

- **Cluster 4** represents ultra-high CTC earners (₹1Cr+), often in niche roles like **Research Engineers** or **Support Engineers**.
- Common job roles like **Backend Engineer**, **Data Scientist**, and **FullStack Engineer** dominate Clusters 0–3.
- **Designation, Class, and Tier flags** revealed internal salary positioning—helping identify above-average earners even within similar roles.
- Some companies consistently produce above-average CTC learners.

See full insights [here →](#)

---

## 💡 Recommendations

- Focus training and placement on high-growth roles (Backend, FullStack, Data Science).
- Build partnerships with top-paying companies identified in the analysis.
- Use internal performance flags to tailor learning paths and give feedback to learners.

---

## 📎 Dependencies

- Python 3.8+
- pandas, numpy, scikit-learn, matplotlib, seaborn

```bash
pip install pandas numpy scikit-learn matplotlib seaborn

