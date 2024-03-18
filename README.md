# TITANIC DATA ANALYSIS WITH EXCEL
### Project Overview

Analyzing the Titanic dataset to derive meaningful insights that can impact a travel and tourism company. By analyzing this dataset, we aim to gain a deeper understanding of passenger demographics, travel patterns, and factors influencing survival outcomes. This analysis will enable us to tailor our marketing strategies, enhance customer experiences.

![Screenshot (60)](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/451f78cc-fceb-45b8-a7b4-fb46f1f3e75c)

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
10. Data cleaning and formatting

### Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions:
1. How do passenger demographics such as age, gender, and passenger class correlate with survival outcomes, and how can we leverage this information to tailor our travel packages and services?
2. Can we identify any patterns or trends in passenger travel preferences, such as ticket class, cabin location, or port of embarkation, that may inform our marketing strategies and service offerings?
3. Are there any insights from the analysis that suggest opportunities for enhancing safety measures or risk mitigation strategies in our travel operations?
4. How can we segment passengers based on their characteristics and travel preferences to personalize our marketing campaigns and promotional offers effectively?
5. Are there any outliers or anomalies in the dataset that may require further investigation, and how can we address them to ensure the accuracy and reliability of our analysis?
6. What visualization techniques in Excel can effectively communicate our findings to stakeholders and facilitate data-driven decision-making within our organization?
7. How can we leverage historical insights from the Titanic dataset to anticipate and mitigate potential risks or challenges in our travel operations, especially in emergency scenarios?
8. Are there any additional data sources or external datasets that we can incorporate into our analysis to enrich our understanding of passenger behavior and preferences?
9. How can we use Excel to automate repetitive tasks in data preprocessing, analysis, and reporting, to streamline our analytical workflows and improve efficiency in decision-making processes?


### Data Anaysis
Using pivotTable, I summarized the survival rate using the new attribute i extracted while cleaning; such as:
1. Age
2. Sex
3. Family Size
4. Fare
5. Title
6. Cabin
7. Ticket
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/f716e5fb-6e77-4430-a0b7-51217b430d23)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/2cfd8a32-898a-45e3-aedf-db6dd4bff434)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/fb3af3a2-7163-4928-bc43-05374bd52a3b)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/224f0b24-26ab-4be6-8bb3-5d34d3a4f87b)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/8b7f029a-de1f-4891-924a-229ff3dcefcb)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/5fc3a411-fb87-46c3-ac76-a26d27afb35d)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/334b2bd3-3db8-4f80-b36f-2ecc60ba51f4)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/c904a75d-47ec-4739-8361-85cebb51af12)

For the passenger travel preferences, i used PivotTable to check what demographics prefer most. Such demographics include:
1. Ticket
2. Pclass
3. Cabin
4. Embarkation
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/11a4b044-a0f6-4ff9-b3db-6d99a5b2fde0)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/304d5611-bcfd-4a90-a4c8-45496fa3b1c2)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/075a278d-dd64-4327-8fb0-c713c713fd64)
![image](https://github.com/Uccodes/TITANIC-DATA-ANALYSIS-WITH-EXCEL/assets/122783699/5a008135-b8db-41a5-8f93-12de9255e615)


### Results/ Findings
The analyss results are summarized as follows:
**TRAVEL PREFERENCE ANALYSIS**
From observation, passengers were more in the "S" embarkation port, purchased tickets of type "1601" and occupied "E121" cabin.	
This trend informs marketing strategies such as focusing marketing campaigns on promoting travel packages departing from "S" port, featruing the tickets and cabin	
for the opportunities for enhacing safety measure and risk mitigation, since "E121" has highest occupancy rate, safety protocls sholud be deployed more here.	
**Survival Rate** 
From Analysis, I observed that the following set of people have higher survival rates	
	1.Middle-aged Passengers
	2. female Passengers
	3. females who are unmarried i.e. with title of 'Miss'
	4. embarkation port 'S'
	5. smaller family size

 **Visualization Techniques in Excel to Convey Insights**
For this project, I made use of		
	1. PivotTable	
	2. Charts	
		- Pie
		- Bar
		 -Graphs
**Use of Excel to perform Repetitve Tasks**
 
### Recommendation 

Based on the analysis, I recommend the following actions:

1. Channel marketing and campaigns to these demographics of high survival rate 
2. Provide them with incentives to retain and increases their numbers
3. Deploy safety protocols to the sites of the demographics with lesser survival rates.
4. To achieve the above, glean insights from the habits prevalent in the demographics with higher survival rate
5.  Passengers are adviced to travel with less family size. In emergency situations, it is easier to manage.
6.  The younglings and elderly are to extremely cautious when traveling. They have loweR survival rate.

The following tools were quite useful in this analysis	
	1. functions for data cleaning
	2. the fill and flash fill 
	3. the 'create menu selection'

### Limitations

I observed that the tickets without text strings are higher. I grouped them into 'xxx' during cleaning to have them all in one place and get a more accurate analysis.


Refrences


😄

The End. 💻
