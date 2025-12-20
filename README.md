# Laptop-Data-Analysis-MiniProject
Laptop Price Analysis – Mini Project:
This repository contains a complete exploratory data analysis (EDA) of a laptop dataset, performed as part of the Neuroscience Data Analysis with Python Workshop. The project focuses on understanding how different hardware and software features influence laptop prices.

Dataset Description:
The dataset includes 1,275 laptops with the following key attributes:
Company – Manufacturer
Product – Model name
TypeName – Category (Ultrabook, Notebook, Gaming, etc.)
Inches – Screen size
ScreenResolution – Display resolution
CPU_Company / CPU_Type / CPU_Frequency – Processor details
RAM (GB) – Memory size
Memory – Storage description (e.g., “256GB SSD”)
GPU_Company / GPU_Type – Graphics card
OpSys – Operating system
Weight (kg) – Laptop weight
Price (Euro) – Laptop price

Data Cleaning & Feature Engineering:
The following preprocessing steps were applied:
✔ Operating System Normalization
Mapped raw OS strings into categories: Windows, macOS, Linux, Chrome OS, DOS, Other.
✔ RAM Extraction
Converted RAM values to numeric (GB).
✔ Storage Type Extraction
Parsed the Memory column to identify: SSD, HDD, Flash, eMMC, Hybrid, Unknown.
✔ RAM Category Binning
Grouped RAM into meaningful categories (e.g., 5–8GB, 9–16GB).

Statistical Analysis:
The notebook includes:
Basic dataset statistics (describe())
Price distribution analysis
Company-level price comparison
Operating system distribution
RAM distribution and categories
Storage type distribution

Visualizations:
A variety of visualizations were created using Matplotlib and Seaborn:

Price Analysis
Histogram of laptop prices
Line plot of all prices

Company Analysis
Bar plot of average price per company
Boxplot of price distribution per company

Operating System Analysis
Price distribution for each OS type

RAM Analysis
Scatter plot: RAM vs Price
Boxplot: Price by RAM category

Storage Analysis
Bar plot: Average price by storage type

Outlier Detection
Boxplot showing price outliers
IQR-based outlier detection
Z-score outlier detection

Outlier Detection Methods:
Two methods were used to identify unusual price values:
✔ IQR Method
Values outside the range: Q1 - 1.5*IQR to Q3 + 1.5*IQR
✔ Z‑Score Method
Values where |z| > 3 were flagged as outliers.

How to Run the Project:
Install required packages:

1. pip install pandas numpy matplotlib seaborn scipy
2. Place the dataset in the same folder as the notebook.
3. Open the notebook (.ipynb) in Jupyter or VS Code.
4. Run all cells from top to bottom.

Repository Structure:

Laptop-Price-Analysis

laptop_price - dataset.csv
Laptop_Analysis.ipynb
README.md
Author:
Eden Elkoubi
Neuroscience Data Analysis Workshop
