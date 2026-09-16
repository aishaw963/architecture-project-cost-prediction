# Architecture & Design Project Cost Prediction Dashboard

## Project Overview

A predictive analytics project for an Architecture & Design business that uses **Python, Machine Learning, and Power BI** to analyze project costs and generate preliminary cost estimates.

The project uses **Linear Regression** to predict project cost based on project characteristics such as area, floors, project type, complexity, duration, and location.

> **Note:** This project uses a sample dataset created for educational and demonstration purposes.

---

## Business Problem

Architecture and design projects can vary in size, complexity, duration, and location, making early cost estimation challenging.

### Business Question

**Can project cost be predicted using project characteristics?**

---

## Dataset

The dataset contains **150 sample architecture and design projects**.

| Feature           | Description                                |
| ----------------- | ------------------------------------------ |
| `Project_ID`      | Unique project identifier                  |
| `Project_Type`    | Residential, Commercial, Office, or Retail |
| `Area_sqft`       | Project area in square feet                |
| `Floors`          | Number of floors                           |
| `Complexity`      | Low, Medium, or High                       |
| `Duration_Months` | Project duration                           |
| `Location`        | Urban, Suburban, or Rural                  |
| `Project_Cost`    | Estimated project cost                     |

---

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* Power BI
* GitHub

---

## Analysis & Key Findings

* **Area_sqft** had the strongest relationship with project cost, with a correlation of **0.894**.
* High-complexity projects had the highest average project cost in the dataset.
* Floors and project duration showed weaker positive relationships with project cost.
* Exploratory analysis was performed using project type, complexity, location, and numerical variables.

---

## Machine Learning Model

**Model:** Linear Regression

**Features:**

* Project Type
* Area
* Floors
* Complexity
* Duration
* Location

**Target:** `Project_Cost`

### Model Performance

| Metric              |               Result |
| ------------------- | -------------------: |
| R² Score            |                0.958 |
| Mean Absolute Error | 11,053.29 cost units |
| Training Records    |                  120 |
| Testing Records     |                   30 |

The model was evaluated using an **80/20 train-test split**.

---

## New Project Prediction

A sample project was used to demonstrate prediction:

* **Project Type:** Residential
* **Area:** 3,000 sqft
* **Floors:** 2
* **Complexity:** High
* **Duration:** 7 months
* **Location:** Urban

**Predicted Cost: 176,681.64 cost units**

---

## Power BI Dashboard

The interactive dashboard includes:

* Total Projects
* Average Project Cost
* Average Project Area
* Average Project Duration
* Average Cost by Project Type
* Average Cost by Complexity
* Average Cost by Location
* Area vs Project Cost
* Actual vs Predicted Project Cost
* Model R² and MAE
* Project Type, Complexity, and Location filters

---

## Business Recommendations

1. Use project area as an important input during early cost estimation.
2. Consider project complexity when preparing preliminary budgets.
3. Use predictive modeling to support early-stage project planning.
4. Review larger projects carefully because larger areas are associated with higher costs.
5. Use real historical project data to improve and validate the model for real-world use.

---

## Project Structure

```text
architecture-project-cost-prediction/
│
├── architecture_project.ipynb
├── architecture_projects.csv
├── README.md
└── dashboard/
```

---

## Project Purpose

This project was developed for **learning and portfolio purposes** to demonstrate data analysis, machine learning, and business intelligence skills using Python and Power BI.
