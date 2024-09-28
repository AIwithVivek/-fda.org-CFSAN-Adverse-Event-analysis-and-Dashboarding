

---

<h1 align="center">CFSAN Adverse Event Reporting System Analysis[fda.org] </h1>

<p align="center"> 
<img src="https://qtxasset.com/cdn-cgi/image/w=850,h=478,f=auto,fit=crop,g=0.5x0.5/https://qtxasset.com/quartz/qcloud5/media/image/FDAWHITEOAK.jpg?VersionId=LjiYOu1IpRi1Lr5AFyfPg4UfAZRO.azo" alt="divider">
</p>

| **Sections**                                                                        |
|-------------------------------------------------------------------------------------|
| [Introduction](#1-introduction)                                                     |
| [Data Source](#2-data-source)                                                       |
| [Data Cleaning, Modeling, and DAX](#3-data-cleaning-modeling-and-dax-in-power-bi)   |
| [Dashboard Overview](#4-dashboard-overview)                                         |
| [Key Insights and Data Storytelling](#5-key-insights-and-data-storytelling)         |
| [Conclusions](#6-conclusions)                                                       |

<p align="center"> 
<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" alt="divider">
</p>

## **1. Introduction**

The primary objective of analyzing the **CFSAN Adverse Event Reporting System (CAERS)** dataset is to gain a comprehensive understanding of adverse events associated with foods, dietary supplements, and cosmetics reported to the FDA. 

This analysis aims to identify patterns and trends in these events, including their distribution across product categories, demographic characteristics, and the severities of reported outcomes. These insights can contribute to enhanced product safety surveillance and inform regulatory decisions to improve public health.

---

## **2. Data Source**

The analysis uses the **CAERS_ASCII_2004_2017Q2.csv** file, covering reports from 2004 to the second quarter of 2017. Key fields in the dataset include:

- **RA_Report:** Unique identifier for each adverse event.
- **RA_CAERS Created Date:** Entry date in CAERS database.
- **AEC_Event Start Date:** Date when the adverse event started.
- **PRI_Product Role:** Role of the product (e.g., suspect or concomitant).
- **PRI_Reported Brand/Product Name:** Product name associated with the event.
- **PRI_FDA Industry Code & Name:** Industry categorization (e.g., 'Bakery Prod/Dough/Mix/Icing').
- **CI_Age at Adverse Event:** Age of the individual affected.
- **CI_Gender:** Gender of the individual affected.
- **AEC_One Row Outcomes:** Event outcomes (hospitalization, ER visit, etc.).
- **SYM_One Row Coded Symptoms:** Coded symptoms linked to the event.

---

## **3. Data Cleaning, Modeling, and DAX in Power BI**

### **Data Importing and Preprocessing**

- Imported the dataset into Power BI for initial exploration and cleaning.
- Addressed issues such as missing values, incorrect data types, and inconsistent entries.

### **Analysis Breakdown:**

- **Product Role Categorization:** Grouped products based on their role (e.g., suspect or concomitant) to assess distribution across roles.
- **Industry-Based Analysis:** Analyzed FDA industry names to understand adverse event frequency within different industries.
- **Demographic and Gender Analysis:** Investigated age and gender distribution of adverse events.
- **Symptom Frequency and Correlation:** Assessed common symptoms and their correlation with patient demographics.
- **Outcome and Industry Relationships:** Explored the link between product categories and event outcomes.
- **Time Series Analysis:** Conducted a time-based analysis of reports to identify reporting trends.

### **Advanced DAX Modeling:**

- Developed predictive models to estimate risks based on age, product type, and symptom severity using DAX calculations.

---

## **4. Dashboard Overview**

### **Adverse Event Reporting Dashboard**

- This interactive Power BI dashboard showcases the frequency of reports, common symptoms, and product roles, allowing users to explore the data by industry, product role, age group, and gender.

![Adverse Event Reporting Dashboard](https://github.com/AIwithVivek/-fda.org-CFSAN-Adverse-Event-analysis-and-Dashboarding/blob/main/adverse%20event%20reporting.PNG)

### **Demographic Analysis Dashboard**

- The dashboard visualizes adverse event trends by age and gender, highlighting demographic patterns in reported events.

![Demographic analysis.PNG](https://github.com/AIwithVivek/-fda.org-CFSAN-Adverse-Event-analysis-and-Dashboarding/blob/main/Demographic%20analysis.PNG)

### **Industry and Outcome Analysis Dashboard**

- Interactive visuals show the relationship between industries and reported outcomes, revealing high-risk product categories and patterns in severity.

![Industry and Outcome Analysis](https://github.com/AIwithVivek/-fda.org-CFSAN-Adverse-Event-analysis-and-Dashboarding/blob/main/Industry%20and%20Outcome%20Analysis.PNG)



### **Interactive Dashboard**

- Explore the interactive dashboard [here](https://drive.google.com/file/d/1Vp3hX67uPlMUlHmBYVXQXc_jOcFDulNG/view?usp=sharing) to dive deeper into the data and uncover more insights.

---

## **5. Key Insights and Data Storytelling**

The analysis provided valuable insights, including:

- **Product Role Insights:** Products classified as "suspect" had higher reporting rates of adverse events compared to "concomitant" products.
- **Demographic Trends:** Most reports were associated with middle-aged individuals, and women reported more adverse events than men.
- **Industry Patterns:** Certain industries, such as dietary supplements and cosmetics, had a higher incidence of severe outcomes.
- **Time-Based Reporting Trends:** Adverse event reports increased significantly from 2010 onwards, suggesting a growing awareness or increased product use.
- **Common Symptoms:** Symptoms such as nausea, dizziness, and allergic reactions were frequently reported, particularly in the dietary supplements category.

---

## **6. Conclusions**

This analysis of the **CFSAN Adverse Event Reporting System** provided critical insights into the safety and risks associated with food and cosmetic products. These findings can inform future safety regulations and product development strategies, ensuring that potential risks are identified and addressed proactively. 

By leveraging Power BI and DAX, we gained a deeper understanding of the relationships between demographic factors, product types, and the severity of adverse events, which can ultimately contribute to improving public health and product safety.

---

**Explore the complete dashboard [here](https://drive.google.com/file/d/19J-p6-oZLs2k-G-BOMmnz03g8ILszw-A/view?usp=drive_link)**


