# 📚 Guftgu Publications — Book Order Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Numerical-013243?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-Dataset-20BEFF?logo=kaggle&logoColor=white)
![Pakistan](https://img.shields.io/badge/Dataset-Pakistan%20Books-01796F)

A complete Exploratory Data Analysis (EDA) on Gufhtugu Publications' real-world book order dataset — uncovering top-selling books, city-wise order patterns, revenue estimates, payment method preferences, and time-based sales trends across Pakistan.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [About the Dataset](#-about-the-dataset)
- [Analysis Sections](#-analysis-sections)
- [Visualizations](#-visualizations)
- [Tech Stack](#️-tech-stack)
- [Project Structure](#-project-structure)
- [How to Run](#-how-to-run)
- [Key Insights](#-key-insights)
- [Author](#-author)

---

## 🌍 Overview

**Gufhtugu (Guftgu) Publications** is a well-known Pakistani book publisher. This project performs an end-to-end EDA on their real book order dataset — one of the most popular Pakistani datasets on Kaggle — to answer real business questions like:

- Which books sell the most?
- Which cities order the most books?
- How does payment method vary across customers?
- How have orders changed over time?
- What is the estimated revenue by book and category?

---

## 📂 About the Dataset

- **Source:** [Gufhtugu Publications Dataset Challenge — Kaggle](https://www.kaggle.com/datasets/zusmani/gufhtugu-publications-dataset-challenge)
- **Records:** ~20,000 book order records from Pakistan
- **Context:** Real sales data from a Pakistani publication house
- **Notebook Size:** 3,518 lines · 349 KB

### Dataset Columns

| Column | Description |
|--------|-------------|
| `Order ID` | Unique identifier for each order |
| `Book Title` | Name of the book ordered |
| `Author` | Author of the book |
| `Category` | Genre/category of the book |
| `Price` | Price of the book (PKR) |
| `Quantity` | Number of copies ordered |
| `City` | City from which the order was placed |
| `Payment Method` | How the customer paid (e.g., COD, Online) |
| `Order Date` | Date the order was placed |
| `Revenue` | Estimated revenue = Price × Quantity |

---

## 🔍 Analysis Sections

### 🧹 1. Data Loading & Exploration
- Loaded dataset using Pandas
- Checked shape, data types, null values, and duplicate records
- Basic `.info()`, `.describe()`, `.head()` exploration
- Fixed incorrect data types (dates, numerics)

### 📊 2. Exploratory Data Analysis (EDA)
- Distribution of orders across all columns
- Frequency analysis of books, cities, categories, and payment methods
- Value counts for categorical features

### 📈 3. Orders Over Time
- Monthly and yearly order trends
- Identified peak sales periods
- Time-series line charts to show growth or decline patterns

### 💳 4. Payment Method Usage
- Breakdown of how customers pay (COD vs Online etc.)
- Payment preference by city
- Bar charts comparing payment methods

### 🏙️ 5. Top 10 Cities by Order Count
- Ranked list of cities with highest book orders
- Karachi, Lahore, Islamabad and others compared
- Horizontal bar charts for easy reading

### 📖 6. Top-Selling Books
- Most ordered book titles across the entire dataset
- Revenue contribution per book
- Bar charts of top 10 / top 20 best sellers

### 💰 7. Revenue Estimates
- Calculated estimated revenue (Price × Quantity)
- Revenue by book title, author, and category
- Identified highest-revenue generating products

### 🗂️ 8. Category Analysis
- Which book genres/categories are most popular
- Category-wise order count and revenue comparison

---

## 📉 Visualizations Used

| Chart Type | Purpose |
|---|---|
| Bar Charts (H & V) | Top cities, top books, payment methods, categories |
| Line Charts | Orders over time — monthly/yearly trends |
| Pie Charts | Payment method share, category distribution |
| Count Plots | Frequency distributions across categorical columns |
| Box Plots | Price and quantity outlier detection |
| Grouped Bar Charts | City vs payment method comparisons |

---

## 🛠️ Tech Stack

```
Python 3.x
├── pandas        # Data loading, cleaning, groupby, aggregation
├── numpy         # Numerical operations and calculations
└── matplotlib    # All charts and visualizations
```

---

## 📁 Project Structure

```
GuftguPublications-Book-Order-Data-Analysis-/
│
├── gp-book-order-dataset-analysis.ipynb   # Full EDA notebook
│                                           # 3,518 lines · 349 KB
│                                           # Data loading → Cleaning → EDA → Visuals
│
└── README.md                               # Project documentation
```

> **Note:** The dataset CSV is not included. Download it from [Kaggle](https://www.kaggle.com/datasets/zusmani/gufhtugu-publications-dataset-challenge) and place it in the project root before running.

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/Azharaliii/GuftguPublications-Book-Order-Data-Analysis-.git
cd GuftguPublications-Book-Order-Data-Analysis-
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib jupyter
```

### 3. Download the Dataset
- Go to [Kaggle Dataset](https://www.kaggle.com/datasets/zusmani/gufhtugu-publications-dataset-challenge)
- Download the CSV file
- Place it in the project root directory

### 4. Run the Notebook
```bash
jupyter notebook gp-book-order-dataset-analysis.ipynb
```

---

## 💡 Key Insights

- 📖 **Best Sellers** — A small number of books account for a large percentage of total orders, showing a classic long-tail distribution
- 🏙️ **City Dominance** — Lahore, Karachi, and Islamabad lead in order volume, reflecting Pakistan's major urban book-buying population
- 💳 **Payment Preferences** — Cash on Delivery (COD) dominates as the preferred payment method, consistent with Pakistani e-commerce trends
- 📅 **Seasonal Trends** — Order volume peaks during certain months, likely tied to academic seasons and festive periods
- 💰 **Revenue Drivers** — High-price books don't always generate the most revenue — volume of orders matters more for certain titles
- 📚 **Category Trends** — Certain genres consistently outperform others in both order count and revenue

---

## 🔮 Future Improvements

- 🤖 Order prediction model using regression
- 🗺️ Geographic map of orders using `folium`
- 📊 Interactive dashboard with `Plotly` or `Streamlit`
- 🔁 Recommender system — "customers who bought this also bought..."
- 📦 Inventory optimization suggestions based on order trends

---

## 👤 Author

**Azhar Ali Soomro**
[![GitHub](https://img.shields.io/badge/GitHub-Azharaliii-181717?logo=github&logoColor=white)](https://github.com/Azharaliii)
[![Kaggle](https://img.shields.io/badge/Kaggle-azharalisoomro-20BEFF?logo=kaggle&logoColor=white)](https://www.kaggle.com/azharalisoomro)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

⭐ **Found this analysis helpful? Give it a star!**
