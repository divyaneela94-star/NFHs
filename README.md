# Nationa Family Health Survey

The NFHS provides detailed data on population, health, nutrition, and family welfare. Its main purpose is to help government officials, researchers, planners, and the public understand health conditions and make better decisions based on reliable data.

--------------------------
# Domain 
Health Care 

------
# Objective

 * The main objective of this project is to analyze district-level health and nutrition indicators in India using NFHS-5 data and to visualize key insights through an interactive Power BI dashboard.
* This helps in understanding anaemia levels, institutional births, female literacy, and child nutrition across districts and states.

  --------
 # Outcome
 
The project helps uncover key patterns, trends, and hidden insights from the dataset. The analysis provides a clear understanding of the data and supports decision-making with evidence-based findings.

---------
# **Dataset Information**

**Source:**  Open Government Data(OGD) Platform India

**Project Link** : https://www.data.gov.in/catalog/national-family-health-survey-5-nfhs-5-india-districts-factsheet-data-provisional

**Year / Timeline:** 2022 to 2021

**Published On:** 04/03/2022-**Updated On:** 07/11/2025

**Dataset Column Description:**

**Basic Information**

1. District Name – Name of the district

2. State/UT – Name of the state or union territory

3. Number of Households Surveyed – Total households covered in the survey

4. Women / Men Interviewed – Number of women (15–49) and men (15–54) surveyed

**Population & Education Indicators**

1. Population below 15 years – Percentage of children in the population

2. Sex Ratio – Number of females per 1,000 males

3. School Attendance / Literacy – Education level and literacy status of women

**Household Facilities & Living Conditions**

1. Electricity – Households with electricity

2. Drinking Water – Access to improved drinking water

3. Sanitation – Use of improved sanitation facilities

4. Cooking Fuel – Use of clean fuel for cooking

5. Iodized Salt – Households using iodized salt

6. Health Insurance – Coverage under health insurance schemes

**Women & Reproductive Health**

1. Early Marriage – Women married before age 18

2. Teenage Pregnancy – Young women who are mothers or pregnant

3. Family Planning – Use of any and modern contraceptive methods

4. Unmet Need – Women who want family planning but are not using it

**Maternal Health Care**

1. Antenatal Care (ANC) – Check-ups during pregnancy

2. Iron & Folic Acid Intake – Nutrition during pregnancy

3. Postnatal Care – Care received after delivery

4. Institutional Births – Births in health facilities

5. Caesarean Deliveries – Percentage of C-section births

**Child Health & Immunization**

1. Coverage – Children fully vaccinated

2. Specific Vaccines – BCG, Polio, DPT, Measles, Rotavirus

3. Vitamin A – Children receiving Vitamin A supplements

**Child Illness & Nutrition**

1. Diarrhoea & ARI – Prevalence and treatment of childhood illnesses

2. Breastfeeding – Early and exclusive breastfeeding practices

3. Child Nutrition – Stunting, wasting, underweight, overweight

4. Women’s Nutrition & Anaemia

5. BMI Status – Underweight, overweight, or obese women

6. Anaemia – Anaemia among children and women

**Non-Communicable Diseases**

1. Blood Sugar Levels – Diabetes risk among men and women

2. Blood Pressure – Hypertension indicators

**Cancer Screening & Substance Use**

1. Cancer Screening – Cervical, breast, and oral cancer tests

2. Tobacco Use – Tobacco consumption among men and women

3. Alcohol Use – Alcohol consumption among men and women

**Age** - 4 years old

---------------------
## Stage 1 – Problem Definition and Dataset Selection
**Business Problem**

Despite various government health programs, district-level differences in health, nutrition, and family welfare outcomes still exist across India. Understanding these gaps using NFHS-5 data is necessary to identify areas with poor health indicators.

----------------
**It contains district-wise health indicators such as:**

* Anaemia levels

* Institutional births

* Female literacy

* Child nutrition status

---------------
**Tools and Technologies Used**

* Google Colab (Python)

* Pandas, NumPy, Matplotlib, Seaborn

  Used for data cleaning, preprocessing, and exploratory analysis

* Power BI

 Used to create an interactive dashboard for visualization

* Excel / CSV

Used as an intermediate data format

------------
## Stage 2 – Data Cleaning and Pre-processing

* The NFHS dataset was imported into Google Colab using Pandas.

**Data cleaning was done by:**

* Handling missing values

* Renaming columns for clarity

* Categorizing anaemia risk into High, Medium, and Normal

  --------------
## Exploratory Data Analysis (EDA) was performed using:

* Bar charts

* Pie charts

* Count plots

* Key metrics like average anaemia, female literacy, and institutional birth rate were calculated.

* The cleaned dataset was then exported and connected to Power BI.

---------------
## Univariate Analysis

**1.Histogram - Distribution of Institutional Births (%)**

1. Shows that most districts have high institutional birth rates, indicating improved maternal healthcare access, while a few districts still lag behind and need targeted interventions.


2. *   X-axis: Represents the percentage of institutional births in each district.
   * 
   *   Y-axis: Represents the number of districts (frequency) falling within each percentage range.

3. That maternal healthcare access has improved significantly across most districts, but some districts still lag behind. These low-performing districts require targeted policy interventions, improved healthcare infrastructure, and awareness programs.

   ------------
   **2.Count Plot - Sanitation Status Distribution**

1. X-axis: Shows sanitation status categories of districts.

2. Y-axis: Shows the number of districts in each category.

3. It highlights how sanitation coverage is distributed across districts and identifies areas needing improvement.

   ---------------

   **3.Box Plot -Distribution of Anaemia Among Women (15–49 years)**

 1. This box plot shows the spread, median, and outliers of anaemia prevalence among women across districts..

2. *  X-axis: Represents overall district-wise distribution (no categories).
   *  
   *  Y-axis: Percentage of women (15–49 years) who are anaemic.

3.It highlights variability and outliers in anaemia levels across districts, helping identify high-risk regions.

---------

## Bivariate Analysis

**4.Bar Plot- Sanitation Status vs Child Nutrition**

1. This bar plot shows how the number of districts with different child nutrition statuses varies across sanitation levels.
   
2. *  X-axis: Sanitation status of districts.

   *  Y-axis: Number of districts.

3. It shows that better sanitation is associated with improved child nutrition outcomes across districts.

   -----------

   **5.Pie chart - Distribution of Institutional Birth Levels Across Districts**

1. X-axis / Y-axis: Not applicable (pie chart shows proportions, not axes)

2. It shows the proportion of districts in each Institutional Birth Level category (Low, Medium, High).

3. Most districts fall into the High or Medium institutional birth categories, indicating generally good maternal healthcare access, but some districts still have low institutional births, needing targeted policy interventions.

------------------

**6.Scatter Plot - # Institutional Births vs Anaemia Among Women**

1. This scatter plot shows the relationship between institutional birth rates and anaemia prevalence among women across districts.

2. * X-axis: Percentage of institutional births in each district.

   * Y-axis: Percentage of women (15–49 years) who are anaemic.
   
3. It shows that districts with higher institutional birth rates generally tend to have lower anaemia prevalence, indicating better maternal healthcare outcomes.

   ------

   **7.correlation heatmap - Insurance Coverage vs BMI Indicators**

1. This heatmap shows the strength and direction of relationships between insurance coverage and women’s BMI indicators across districts.

2. X-axis & Y-axis: Health insurance coverage and women’s BMI-related indicators compared with each other.

3. Districts with higher health insurance coverage tend to have lower undernutrition and relatively higher overweight prevalence, indicating better access to healthcare.

---------------   

# Multivariate Analysis

**8.Pair plot - Health Indicators**

1. The pair plot visualizes how key health indicators are related to each other across districts.

2. Each row and column represent a different health indicator, and the plots show pairwise relationships between them.

3. Institutional births, anaemia among women, health insurance coverage, and women’s BMI status.

4. Multiple maternal and healthcare indicators are interrelated and together reflect the overall health infrastructure of districts.

   ------
 **9.Pivot Tables**

 This pivot table summarizes the average percentage of stunted children by grouping districts based on health insurance coverage level and anaemia risk category, helping compare child nutrition outcomes across different health conditions.

**Insurance Coverage vs Anaemia Risk vs Child Stunting**

1. The pivot table calculates the average percentage of stunted children by grouping districts according to insurance coverage level and anaemia risk category.

2. * X-axis- Shows Health Insurance Coverage Level of districts (Low, Medium, High).
   * Y-axis- Shows the average percentage of children under 5 who are stunted.

3. Districts with higher insurance coverage and lower anaemia risk generally show lower child stunting, indicating better health outcomes.

   ----------------
**10.Grouped Analysis: Top 10 States by Average Institutional Births**

1. * X-axis- Represents the top 10 states/UTs with the highest average institutional births.

   * Y-axis- Represents the average percentage of institutional births in each state/UT.

2. States with higher institutional birth rates have better access to maternal healthcare and higher adoption of hospital deliveries.

3. The chart helps identify low-performing states where policy interventions and healthcare infrastructure improvements are needed to increase institutional births.

   --------------

**11.Advanced Plot: Sanitation Coverage vs Child Stunting**

1. * X-axis- Represents the percentage of population living in households with improved sanitation.

   * Y-axis- Represents the percentage of children under 5 years who are stunted (height-for-age).

2. It shows a negative relationship: districts with better sanitation generally have lower child stunting rates.

3. Improving sanitation coverage is associated with better child nutrition outcomes, highlighting the importance of hygiene and sanitation interventions in reducing stunting.

-----------------
## Dashboard Explanation (Key Insights)
**1. KPI Cards**

***Average Anaemia: 2.72K***
→ Shows that anaemia is a major health issue across districts.

***Institutional Birth: 64.98%***
→ Indicates moderate usage of hospital delivery services.

***Female Literacy: 74.72%***
→ Shows improvement but still scope for growth.

***Child Nutrition: 75.56%***
→ Reflects overall child nutrition status in India.

**2. Public Health Facility Delivery Gauge**

* Displays 9.03K deliveries, showing reliance on public healthcare facilities.

* Helps assess healthcare infrastructure effectiveness.

**3. Caesarean Section Delivery (Donut Chart)**

* Shows births delivered by High and Medium risk categories.

* Indicates medical intervention trends during childbirth.

**4. Anaemia Risk Map (India Map)**

***Visualizes district-wise anaemia risk:***

🔴 High Risk

🟡 Medium Risk

🟢 Normal

Helps identify high-priority regions for government intervention.

**5. Child Nutrition vs Anaemia Risk (Bar Chart)**

* Shows a clear relationship between poor nutrition and high anaemia.

* States like Rajasthan and Madhya Pradesh show higher risk.

**6. Top 10 High Anaemia Districts**

* Highlights districts with the highest anaemia burden.

* Useful for targeted health policy planning.

**7. Schooling Overview Indicator**

* Shows improvement in schooling levels.

* Education is linked with better health awareness and outcomes.

-------------------------

## Stage 4 – Documentation, Insights and Presentation

**NFHS Documentation:** https://drive.google.com/file/d/16DmfT7Rj-EMJXuO_CNgE24DtNRNHmA6a/view?usp=drive_link

**Descriptive**

 It summarizes the data using averages, percentages, and counts. From the NFHS data, we can see that anaemia levels are high in many districts, institutional birth rates are moderate, and female literacy is fairly good.

 **Diagnostic**

 The data shows that districts with low institutional birth rates and poor healthcare facilities tend to have higher anaemia levels. Lack of nutrition awareness and limited access to medical services are major reasons.

 **Predictive**

 Based on current trends, districts with poor healthcare and low institutional births are likely to continue having high anaemia cases if no action is taken.

 **Prescriptive**

 The data indicates that improving hospital facilities, increasing nutrition programs, and spreading health awareness can reduce anaemia and improve maternal health outcomes.

 -------------------

 ## Conclusion

From the analysis,  NFHS dashboard shows that India has made good progress in maternal healthcare and female education, indicating better awareness and access to health services. However, anaemia and child nutrition problems are still common in many districts, with clear differences across regions. The analysis highlights the importance of focusing on high-risk areas and using targeted health and nutrition programs to improve overall maternal and child health outcomes.
   
-------------------
