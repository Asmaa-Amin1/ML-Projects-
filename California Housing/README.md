# California Housing Dataset Analysis

This repository contains a Python script and data exploration workflow for loading, inspecting, and analyzing the well-known **California Housing Dataset** using `pandas`, `numpy`, and `scikit-learn`.

## 📋 Table of Contents
- [Dataset Overview](#-dataset-overview)
- [Features Description](#-features-description)
- [Prerequisites](#-prerequisites)
- [Code Workflow & Implementation](#-code-workflow--implementation)
- [Exploratory Data Analysis (EDA) Insights](#-exploratory-data-analysis-eda-insights)
- [Usage](#-usage)

---

## 📊 Dataset Overview

The **California Housing Dataset** is derived from the 1990 U.S. Census. It contains **20,640 instances** (rows) and **8 numeric predictive features** along with a target variable (`MedHouseVal`). 

* **Number of Instances:** 20,640
* **Number of Attributes:** 8 numeric features + 1 target variable
* **Missing Values:** None
* **Target Variable:** `MedHouseVal` (Median house value for California districts, expressed in hundreds of thousands of dollars - `$100,000`)

---

## 📝 Features Description

1. **`MedInc`**: Median income in block group.
2. **`HouseAge`**: Median house age in block group.
3. **`AveRooms`**: Average number of rooms per household.
4. **`AveBedrms`**: Average number of bedrooms per household.
5. **`Population`**: Block group population[cite: 4].
6. **`AveOccup`**: Average number of household members[cite: 4].
7. **`Latitude`**: Block group latitude[cite: 4].
8. **`Longitude`**: Block group longitude[cite: 4].
9. **`MedHouseVal`** *(Target)*: Median house value[cite: 4].

---

##  Prerequisites

Make sure you have the following Python libraries installed before running the code:

```bash
pip install numpy pandas scikit-learn
