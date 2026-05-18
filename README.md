# telecom-analysis
# 📱 ConnectaTel User Behavior Analysis

## 📌 Project Overview

This project analyzes customer behavior for ConnectaTel, a telecommunications company operating in Mexico and Colombia.

The objective is to understand how users interact with mobile services such as calls and text messages, identify usage patterns, detect atypical behaviors, and generate actionable business insights that help improve customer experience and optimize commercial plans.

The analysis was developed using Python in Jupyter Notebook as part of a Data Analytics portfolio project.

---

# 📂 Datasets Used

This project integrates three different data sources:

## 1. `plans.csv`
Contains information about available mobile plans:
- Monthly price
- Included minutes
- Included GB
- Extra usage costs

## 2. `users_latam.csv`
Contains customer information:
- User ID
- Age
- City
- Registration date
- Assigned plan
- Churn information

## 3. `usage.csv`
Contains real usage activity:
- Calls
- Messages
- Call duration
- Message length

> These datasets were combined to analyze customer behavior, usage intensity, segmentation, and potential commercial opportunities.

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Jupyter Notebook

---

# 🔄 Analysis Workflow

The project followed the following analytical process:

1. Load datasets
2. Explore data structure
3. Detect data quality issues
4. Clean invalid values and dates
5. Handle missing values
6. Generate summary statistics
7. Create visualizations
8. Detect outliers using IQR
9. Segment users by:
   - Age
   - Usage level
10. Generate business insights
11. Export and document results

---

# 🔍 Main Analysis Performed

## Data Cleaning
- Converted invalid sentinels (`-999`) in age
- Replaced invalid city values (`?`)
- Converted date columns to datetime format
- Identified and handled out-of-range dates
- Validated structural missing values in usage data

## User Behavior Analysis
- Total calls per user
- Total messages per user
- Total call minutes per user
- Distribution analysis by plan type
- Outlier detection with boxplots and IQR

## Customer Segmentation
Users were segmented into:
- Low usage
- Medium usage
- High usage

And also by age group:
- Young
- Adult
- Senior

---

# 📊 Key Findings

- Most users fall into the medium usage segment.
- Premium users generally consume more minutes and messages.
- Usage variables show right-skewed distributions with high-consumption outliers.
- Outliers appear realistic and may represent valuable heavy users instead of data errors.
- Different age groups show different communication behaviors.

---

# 💡 Business Recommendations

- Create differentiated plans based on real customer behavior.
- Develop loyalty programs for high-usage customers.
- Monitor extreme usage patterns for fraud detection or premium opportunities.
- Improve customer segmentation using behavioral metrics.

---

# ▶️ How to Run This Project

## Option 1 — Jupyter Notebook
1. Clone the repository
2. Open the notebook in Jupyter
3. Install dependencies if needed:
```bash
pip install pandas numpy matplotlib seaborn
