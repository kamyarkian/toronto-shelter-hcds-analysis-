# Human-Centered Audit: Toronto Shelter System Capacity (2024)

## 📌 Project Overview
This repository contains a quantitative analysis of the City of Toronto's shelter system for the full year of **2024**. Using a **Human-Centered Data Science (HCDS)** framework, this project audits the "capacity strain" on critical social infrastructure.

The core objective is to move beyond simple occupancy metrics and visualize the tension between **algorithmic resource allocation** and **human vulnerability**.

## 📂 Files in this Repository
* `analysis.ipynb`: The Jupyter Notebook containing the full Python ETL pipeline, visualization, and probabilistic reasoning.
* `shelter_2024.csv`: The dataset used for this analysis (Source: Toronto Open Data, Daily Shelter & Overnight Service Occupancy).

## 🔍 Key Findings (2024 Audit)
My analysis of daily occupancy rates revealed systemic saturation:
1.  **Zero Margin for Error:** Specific sectors, notably **Women** and **Mixed Adult**, are consistently operating at or near **100% capacity**.
2.  **Structural Strain:** The data indicates a system in a state of chronic "overflow management" rather than temporary housing.
3.  **The Hidden Risk:** When average occupancy hits >99%, the system loses its elasticity, meaning any sudden spike in demand (weather, economic) results in immediate denial of service.

## 🛠️ Technical Workflow
The analysis is built using the **Python Data Science Stack**:
* **Data Engineering:** `Pandas` for cleaning, handling missing capacity values (median imputation), and creating the "Occupancy Rate" metric.
* **Visualization:** `Seaborn` & `Matplotlib` to map capacity strain across different shelter sectors.
* **Probabilistic Reasoning:** A statistical calculation estimating the probability of a family shelter being "overcrowded" (>95% usage) on any given night.

## 🧠 Human-Centered Reflection
In HCDS, we recognize that a "row" in this dataset is a human life in crisis. The red dashed line in the visualization (100% Capacity) is not just a mathematical limit; it represents the threshold of **exclusion**. 

This project demonstrates that while data can measure efficiency, it often fails to capture the *outcome* of that efficiency—specifically, where do people go when the algorithm says "Full"?

---
*Created as a portfolio artifact for the University of Toronto HCDS concentration.*
