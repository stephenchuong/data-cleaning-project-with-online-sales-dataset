# data-cleaning-project-with-online-sales-dataset

    Project Overview
Real-world transactional data is often messy, containing missing values, duplicates, formatting inconsistencies, and statistical outliers. This project demonstrates a structured data preprocessing workflow using Python libraries (pandas, numpy, and plotly) to transform raw retail data into an analysis-ready format.

    Online Retail Data Analysis & Preprocessing Pipeline
An end-to-end exploratory data analysis (EDA) and data cleaning pipeline built in Python using Google Colab. This project processes an online retail transactions dataset to clean raw transactional data, handle outliers, standardize features, and prepare it for deeper exploratory insights and visualization.

    Key Pipeline Steps & Methodology
1.Dataset Loading & Initial Inspection

Loaded transaction records via pandas (/content/Online_Retail_Dataset - Sheet1.csv).

Reviewed structural properties, data types, and descriptive statistics.

2. Missing Value Handling

Identified and managed missing entries across columns.

Dropped null records in non-critical descriptive fields (CustomerName, ProductCategory, and Price).

Imputed missing geographic data in the Country column with 'Unknown'.

3. Duplicate Removal

Checked for full-row redundancies and invoice-specific duplicates.

Successfully cleaned and removed 19 full-row duplicate records.

4. Data Type Casting & Standardization

Converted OrderDate and ShippingDate fields into proper datetime objects.

Cast quantitative metrics like Quantity into integer-compatible nullable types (Int64).

Standardized column headers by stripping whitespace, converting text to lowercase, and replacing spaces with underscores (_).

5. Outlier Detection

via IQRApplied the Interquartile Range (IQR) method ($Q3 - Q1 \times 1.5$) on the price attribute to isolate and filter out extreme price anomalies, refining the dataset down to 1,485 validated rows.

 6. Data Visualization

 Generated distribution histograms of the cleaned price data utilizing Plotly Express (px.histogram).
