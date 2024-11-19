# CodePro: Reducing Customer Acquisition Costs through Lead Scoring

## Overview
CodePro is an EdTech startup that experienced a phenomenal Seed A funding round. The funds were used to increase brand awareness, which led to a surge in leads from various sources. Despite significant spending on customer acquisition, achieving long-term profitability remains a key objective for CodePro. 

The company’s primary cost driver is **Customer Acquisition Cost (CAC)**. While high CAC is typical for early-stage companies, businesses eventually shift their focus toward profitability. Many startups initially offer free or discounted services to build brand awareness and later begin monetizing their offerings once they have an established customer base.

CodePro aims to **reduce its customer acquisition costs** over time by improving the efficiency of its sales process.

---

## Objective: Lead Scoring System
To optimize the sales process, CodePro's data science team is tasked with building a **lead scoring system** that categorizes leads based on their likelihood to purchase. This system will help:

1. **Remove junk leads** by categorizing them based on their propensity to purchase.
2. **Streamline lead conversion** by gaining insights and addressing improper targeting.

The chosen business metric is **L2AC (Leads to Application Completion)**, as using L2P (Leads to Payment) could aggressively drop leads. A lead is generated when a user visits CodePro’s website and submits their contact details. Junk leads—those with no genuine interest in the product—create inefficiencies in the sales pipeline, which this system aims to mitigate.

---

## Project Scope
The project is divided into the following components:

### 1. **Model Experimentation**
- **Environment Setup**:
  - Configure PyCaret and MLflow environments.
- **Model Development**:
  - Train all specified models in PyCaret using all available features.
  - Identify the best-performing model with optimized feature sets and minimal transformations.

---

### 2. **Data Pipeline**
- **Utility Functions**:
  - Develop utility functions for data preprocessing.
- **Data Validation**:
  - Create checks for input raw data and the output of the preprocessing pipeline.
- **Testing**:
  - Write unit tests for pipeline functions.
- **Constants and Macros**:
  - Separate macros and constants into a dedicated file for better maintainability.
- **Feature Mapping**:
  - Map categorical values to fields such as `first_platform_c`, `first_utm_medium_c`, and `first_utm_source_c`.
- **Airflow DAG**:
  - Develop an Airflow DAG Python file to orchestrate the data pipeline.

---

### 3. **Training Pipeline**
- **Utility Functions**:
  - Develop reusable training pipeline functions.
- **MLflow Setup**:
  - Integrate MLflow for model tracking and experimentation.
- **Constants**:
  - Centralize constants for training pipeline configurations.
- **Airflow DAG**:
  - Create an Airflow DAG Python file for automating the training process.

---

### 4. **Inference Pipeline**
- **Inference Functions**:
  - Implement functions for the inference pipeline in `utils.py`.
- **Constants File**:
  - Centralize constants in `constants.py` for inference.
- **Airflow DAG**:
  - Develop an Airflow DAG Python file to automate the inference pipeline.

---

By implementing these steps, CodePro aims to enhance the efficiency of its sales pipeline, reduce customer acquisition costs, and move toward sustainable profitability.


## Contributors
- Sirin Shaikh
