# data-portfolio
Portfolio of my current projects
# SAP Access Risk Analysis – Identifying High-Risk Users

Analyze SAP user access to identify elevated and conflicting rights, quantify risk, and provide clear, visual insights for audit and management.

---

## 🔍 Project Overview

**Context**  
Organizations running SAP often struggle to keep user access aligned with least-privilege and segregation-of-duties principles. Over time, elevated roles, emergency access, and poor deprovisioning create hidden risks in the environment.

**Problem Statement**  
The goal of this project is to detect users with excessive or conflicting access in an SAP landscape and to highlight areas where access design or monitoring needs improvement.

**Approach**  
I simulated an SAP user and role dataset based on typical IT audit scenarios and applied SQL and Python (Pandas) to:  
- Clean and prepare user, role, and transaction data  
- Flag elevated and sensitive roles  
- Identify potential SoD conflicts  
- Summarize risk at user, role, and department level  
- Visualize the results in an interactive dashboard

**Outcome**  
The analysis produces a ranked list of high-risk users and roles, along with visual summaries that can be used by IT, security, and audit teams to prioritize remediation and improve access governance.

---

## 🧰 Tools & Technologies

- **Languages:** SQL, Python (Pandas, NumPy, Matplotlib/Seaborn)  
- **Visualization:** Power BI or Tableau  
- **Data Handling:** CSV/Excel files for user, role, and transaction mappings  
- **Other Concepts:** SAP security, access management, segregation of duties, ITGCs

---

## 📂 Repository Structure

```text
sap-access-risk-analysis/
│
├── data/
│   ├── users.csv
│   ├── roles.csv
│   ├── user_role_mapping.csv
│   └── role_transaction_mapping.csv
│
├── notebooks/
│   └── sap_access_risk_analysis.ipynb
│
├── sql/
│   └── access_risk_queries.sql
│
├── dashboards/
│   ├── sap_access_dashboard.pbix      # Power BI (optional)
│ 
│
└── README.md
