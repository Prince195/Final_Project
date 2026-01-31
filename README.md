# Final_Project 

# 📊 Sales Data Analyzer (Python Project)

## 📌 Overview

The **Sales Data Analyzer** is a **menu-driven Python application** designed to perform **data analysis, cleaning, transformation, statistical operations, and visualization** on CSV datasets.
It uses **Pandas**, **NumPy**, **Matplotlib**, and **Seaborn** to provide an end-to-end data analysis workflow through a simple **console-based interface**.

This project is ideal for:

* Learning **data analysis fundamentals**
* Understanding **real-world CSV handling**
* Practicing **Python OOP (Object-Oriented Programming)**
* Demonstrating **EDA (Exploratory Data Analysis)** skills

---

## 🧠 Key Concepts Used

* Object-Oriented Programming (OOP)
* CSV file handling
* Pandas DataFrame operations
* NumPy array conversion & slicing
* Data cleaning & preprocessing
* Mathematical & statistical analysis
* Pivot tables
* Data visualization
* Memory management (figure cleanup)

---

## 🗂️ Project Structure

```
SalesDataAnalyzer/
│
├── main.py          # Main program file
├── README.md        # Project documentation
├── dataset.csv      # User-provided CSV file
└── output_plots/    # Saved visualizations (optional)
```

---

## 🏗️ Class Description

### `SalesDataAnalyzer`

This class handles **all data operations** and maintains the dataset throughout the program lifecycle.

#### Attributes:

* `df` → Stores the Pandas DataFrame
* `numpy_array` → Stores converted NumPy data
* `file_path` → CSV file path
* `last_plot` → Stores last generated visualization

#### Special Methods:

* `__init__()` → Initializes variables and optionally loads CSV
* `__del__()` → Cleans up memory and confirms object destruction

---

## 📥 Dataset Handling

### Load Dataset

* Reads a CSV file using Pandas
* Converts the DataFrame into a NumPy array
* Handles file-not-found and invalid file errors

---

## 🔍 Data Exploration Features

Allows users to:

* View first & last 5 rows
* Check column names
* Inspect data types
* Display dataset structure using `info()`

---

## 🧹 Data Cleaning

* Detects missing values
* Removes rows with missing critical values
* Replaces remaining missing entries
* Ensures dataset consistency before analysis

---

## 🔢 NumPy Conversion

* Converts full or selected columns into NumPy arrays
* Supports:

  * Indexing
  * Row & column slicing
* Demonstrates array-level operations

---

## ➕ Mathematical Operations

* Dynamically calculates:

  * Tax (5%)
  * Cost (Sales − Profit − Tax)
* Adds computed columns to the DataFrame

---

## 🔗 Data Combination & Splitting

### Combine

* Merges another CSV dataset into the current one

### Split

* Divides dataset based on user-defined column conditions

---

## 🔎 Search, Sort & Filter

* Search values using partial matching
* Sort data by any column (descending)
* Filter numeric data using threshold values

---

## 📊 Aggregate Functions

Provides:

* Sum
* Mean
* Count
  on numeric columns selected by the user

---

## 📈 Statistical Analysis

Includes:

* Standard Deviation
* Variance
* Quartiles (25%, 50%, 75%)

---

## 📐 Pivot Table Creation

* User-defined index, values, and aggregation function
* Generates summarized views of the dataset

---

## 🎨 Data Visualization Module

Interactive visualization menu supports:

1. Bar Plot
2. Box Plot
3. Scatter Plot
4. Histogram
5. Heatmap (Correlation Matrix)
6. Pie Chart
7. Stack Plot

✔ Uses Seaborn themes
✔ Automatically manages figure memory
✔ Saves plots on user request

---

## 💾 Save Visualization

* Saves the **last generated plot**
* Automatically closes figures to free memory

---

## 📜 Menu System

### Main Menu

* Load Dataset
* Explore Data
* Perform DataFrame Operations
* Clean Data
* Statistical Analysis
* Visualization
* Save Plot
* Exit Program

Each menu is **loop-controlled** to ensure smooth navigation.

---

## ⚙️ Requirements

Install required libraries before running:

```bash
pip install pandas numpy matplotlib seaborn

## ▶️ How to Run

```bash
python main.py

---

