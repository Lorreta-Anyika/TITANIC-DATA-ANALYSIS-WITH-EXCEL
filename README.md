# TITANIC DATA ANALYSIS WITH EXCEL

### Project Overview

Analyzing the Titanic dataset to derive meaningful insights that can impact a travel and tourism company. By analyzing this dataset, we aim to gain a deeper understanding of passenger demographics, travel patterns, and factors influencing survival outcomes. This analysis will enable us to tailor our marketing strategies, enhance customer experiences.

### Data Sources

Sales Data: The primary dataset for this analysis is the "titanic data analysis 2.xlsx" file, containing detailed information about passenger surivival rate and travel prefrences. Download here

### Tools

- Microsoft Excel: Data Cleaning, Data Processing, Data Analysis, Report [Download Here](https://microsoft.com)

### Data Cleaning/ Preparation
I performed the following in the data preparation phase:

1. Data loading and inspection
2. Finding missing values
3. Removal of duplicate values
4. Clean_Cabin:  It contains many missing values so I need to go through some processes. After removing duplicates, I extracted the first letters of the values; the ones without text strings, I grouped as under "M". That way i am able to make the values less volumionous and easy to work with. The result? From 891 values to 9 unique values.
5. Sibsp(Sibling and spouse): I needed to find the family size of the passenger. This is because it is easier to safe a passenger who is alone or with lesser family members than its counterpart.
6. Parents and children: uses the logic of the SibSp
7. Title: I extracted the title of the passenger from the column 'name'.
8. Ticket: it had so many duplicates. First I removed the '/' and '.'.Then I extracted the first two letters like 'A5' and removed the many duplicate values. Yet I was not satisfied with the number after the count of each set. So for all the tickets with '1' as the count, I changed them to single. This helped minimze the tickets from 891 to just 23 unique values.
9. Creating dummies before uploading to python or R: the dumies are created for the string values and NOT NUMBERS LIKE THE FARE_1, AGE_1. things to Note: 1) you transpose the unique vales in you working sheet 2.) you delete one before creating the hot codes

![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/d7a4c9f6-d565-45fe-8476-47b0db27d5f0)

5. Checks for consistency in the quantity and gender columns
Data cleaning and formatting
Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions:

Compare the sales and orders using chart
Which month got the highest sales and orders?
Who purchased more-men or women in 2022?
What are differnt order status in 2022?
List top 10 states contributing to the sales?
Relation between age and gender based on number
Which channel is contributing to maximum sales?
Highest selling category?
Data Anaysis
Using pivotTable, I created charts for:

Amount Vs Order ID Vs Month
Gender Vs Amount
Order Vs Status
Ship-state vs Amount
Top 5 sales
Age Group vs Order ID
Results/ Findings
The analyss results are summarized as follows:

March had the highest sales
Women purchase more than men
Maharatrash has the highest sales by state.
Recommendations
Based on the analysis, I recommend the following actions:

Provide more of female products since those are their main customers
efforts must be made to idenfify why sales drop dratsically from August and act accordingly.
Limitations
None

Refrences
Rishab Mishra

Her Data projects

😄

The End. 💻
