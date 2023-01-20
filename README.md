# Analysis-on-Idian-Startup-Ecosystem-
In a group of four members called 'Team florence', we were tasked to analyse the Indian start-up ecosystem to propose working course of action. In this light, the team set out to understand the problem, the Indian start-up terrain, and how best a new business will attract funding from investors given multiple factors.

*Article about the project : https://medium.com/@richmensah1997an-exploratory-data-analysis-on-indian-start-up-ecosystem-funding-from-2018-to-2021-with-python-c4020b3e3815*

*LinkedIn : https://www.linkedin.com/in/richard-mensah-ab8564190/*

## 👋Oview 
---
I support the statement that Exploratory Data Analysis (EDA) is a critical first step in data analysis. In this case, I was helpful in analyzing the Indian setup ecosystem from 2018 to 2021 .
The main reason I employed EDA for my analysis was due to the following reasons

•	To critically investigate the data before making an assumptions for analysis 

•	To measure and compare trends and patterns among the 2018 to 2021 datasets

•	Preliminary selection of appropriate models

•	To understand how to answer both my null hypothesis and alternate hypothesis

•	To provide appropriate visualization to answer questions I want my analysis to answer that would be helpful to my clients (potential investors) 

## 💻 Introduction
---
Exploratory Data Analysis (EDA) was very sensitive on my part as a data analytics professional to explore the datasets from 2018 to 2021 to thoroughly understand the Indian Ecosystem setup funding analysis. This article outlines how EDA assisted me to explore the 4years setup funding trend in the Indian Ecosystem. The focus of the project was to analyze the Indian start-up ecosystem and propose working course of action. In this light, I needed to critically understand the problem, the Indian start-up terrain, and how best new businesses will attract funding from investors given multiple factors.
According to the Economic Survey 2021-22, India was declared the third-largest startup ecosystem in the world, after the US and China. From the Economic Survey report, it is evident that there is a significant rapid growth in Indian startups with increased funding and investments in recent years. From my analysis from the 2018 to 2021 setups funding datasets, it was revealed that statistically, Indian setups have witness an increased rate of about 20% with the majority of the setups been technology rendering, IT services and an ecommerce providing convenient shopping to consumers to  from home.
In my EDA, I first understood my clients, thus, potential investors from India and across the world willing to venture into the India ecosystem. I therefore employed libraries followed by uploading my csv datasets to do a comprehensive EDA to examine the recurring trends that have developed throughout time. This involved examining the category and numerical variables, as well as their distribution, that were present in the data. Since these can have a substantial impact on the outcomes of my analysis, it was also crucial to find any missing or outlier data in the data set.

## :blush: Data Understanding and Structure 
---
 The Indian set-up analysis had four separate csv files for 2018, 2019, 2020 and 2021 and they all needed to be explored and understood individually before merging for further thorough EDA and other vital analysis.  Listed below were the column names

•	company/Brand: name of the start-up

•	Founded: the year the start-up was founded

•	Sector: sector of operation

•	What it does: description of the company

•	Founders: founders of the company

•	Investor: investors in the deal

•	Amount ($): raised funds

•	Stage: round of funding

•	Headquarters: headquarters of the company

## :confused: Hypothesis, Questions, and Objectives
---
Below is my stated hypothesis, questions, and objective that quidded my entire analysis

🤓 **Objective**

My objective for the project was to understand the Indian start-up ecosystem to set as a base for funding start-ups in India.

🤓 **Hypothesis**

**Null hypothesis** - Low risk start-ups tend to attract higher investors
**Alternate hypothesis** - High risk start-ups tend to deflect investors interest or attract lower funding.

🤓 **Questions**

For purpose of the hypothesis, the following questions guided my analysis
•	How does the age of a company impact investment opportunity?

•	Which investment level stage attract more investors?

•	What sector will a start-up attract more investors or funding?

•	Will a location of a start-up affect investment drive?

•	What economic activity of a start-up boost investor funding?

## :relieved: Further Exploratory Data Analysis, Data Preparation and Processing 
---
As part of my EDA, data preparation assisted me in preparing the raw datasets for suitable further processing and analysis. Also, to see to it that the 2018 to 2021 datasets are in formats that allow for easy and accurate analysis, so any data errors or discrepancies identified are corrected to ease analysis, visualization and finding of trends or patterns.

**Analysis and Visualizations Libraries**

Based on the columns of the datasets, libraries for analysis and those that would aid visualizations were employed respectively.

1. *Analysis libraries*
: Pandas and NumPy were used to aid data cleaning and manipulation 
2.  *Visualization libraries*
: Matplotlib and Season to aid visualizations 
3. *Warning library*
: Warnings (warnings.filterwarnings("ignore")) was used to terminate occurring errors

## 👋Preliminary Data Frame Notes
---
The 2018, 2019, 2020 and 2021 csv datasets were loaded into Jupyter notebook separately for an in-depth insight and data understanding. From my observation, it was realized that there were inconsistencies in among the four datasets. The following observation were made 

**:kissing:Observation** : It was observed that;   
•	The Amount column had different data types 

•	There were more missing Values

•	There were non-matching columns

•	There was misrepresentation of data values in the ‘Stage Columns’

•	The amounts have both INDR (Indian Rupee) and Dollar (USD) currencies needed to be converted same currency to ease analysis.

•	Some data had missing currencies in the Amount column.

## Overview of 2018, 2019, 2020 and 2021 Data Frames
---
**💻2018 Data Frame**

•	There are 526 rows and 6 columns in the Data Frame.

• Indian Rupees (INR) and US Dollars (USD ) currencies were mixed in the amount column of  the 2018 Data Frame 

•	New columns were to be created for the ‘Founders’ and ‘Investors’

•	Some columns were changed to match the 2019, 2020 and 2021 datasets

•	Some inconsistent datatypes were changed to ease analysis


**💻2019 Data Frame**

•	The “Founded” column was in float that needed to be converted to a string

•	I used the lambda function to clean the data by using replace method to change appropriate values

•	Index 465 and 472 in the amount column contained two separate funding amounts that needed to be summed.

**💻2020 data Frame**

•	During the EDA, it was realized that there was a column name called “Unnamed:9” that needed to be dropped to match the other three datasets before I merge them.

•	The ‘founded’ column was in object and needed to be changed into a float

**💻2021 Data Frame**

•	The amount column of 2021 data Frame was in object and need to be converted into a float

•	Lambda, strip and replace methods were adopted to clean the data

## :a:ssumptions
---
•	For currency conversions, the average Indian Rupee (INR) to US Dollar (USD) rate for the relevant year will be used.

•	Amounts in the 2018 dataset that do not have currency symbols are in USD.
•	All null values for the Stage column are Unknown Venture Series.

## :v: Data Cleaning for Merging 2018, 2019, 2020 and 2022 datasets
---
Before I merged the four datasets, I did the following data cleaning

•	All columns except the amounts columns were formatted as strings 

•	I used a comma to separate the values in the location and industry columns, and the first value in the split column was chosen as the primary sector.

•	I added two new columns to the 2018 Amount column to help with currency conversion, but I removed them after standardizing the amounts.

•	All commas and currency signs were removed from the "Amounts" columns.

•	I replaced the “Undisclosed” text in the “Amounts”.

•	 The “nan” values in the “Founders” column were replaced with nulls.

•	I replaced notable misplaced and/or erroneous values in the respective rows.

•	I dropped the extra unnamed in the 2020 Data Frame.

•	For each Data Frame, I appended a column indicating the year of funding

•	The columns in the 2018 Data Frame were renamed to match the other Data Frames, after which it was concatenated with the other Data Frames. I then brushed up with the following: 

:o: Reformatted all amounts as numeric and replaced nulls with zeros.

:o: Formatted funding years and years founded as strings.

:o: Dropped all duplicates and reset the index.

## 💻💻Final Merged dataset 
---
The 2018, 2019, 2020 and 2021 dataset were concatenated into a merged data Frame. At this stage of the analysis, further EDA was performed to further understand and clean the final merged datasets. However, visualizations were performed to given a visual understanding of the trends in the data.
 Some of these are,

:kissing: A bar plot showing the top 10 Start-up Funding by Company/Brand in India from 2018, 2019,2020 and 2021

:kissing: Fintech was the sector that received the highest funding among all ther sectors from 2018 to 2021

:kissing: Among the stages of setup funding, Venture series unknown was the highest among them

:kissing: The range of the top 10 se-up founding amount was between $6000000.0 to $1000000.0

:kissing: Among all the headquarters, Bangalore received the highest funding followed by Mumbai

:kissing: The analysis revealed that most of the setups were funded in 2019

:kissing: Inflection Point Ventures and Venture Catalysts were the highest investors from 2018 to 2021 in the India funding ecosystem 

## :question: Questions Answered by The Analysis
---
At part of the article, I will present how I used the analysis to answer 5 major questions that was asked to support my hypothesis after I understood to find pattern or trend in the Indian set-up funding ecosystem

**How does the age of a company impact investment opportunity?**

According to the trend shown below, the age of the company in relation to funding in a given year has no bearing on investment decisions. The differences between years, particularly between 2011 and 2015 data, suggest that economic variables such as the consumer price index and interest rates, rather than the company's age, may be the major determinant of the amount of capital provided.
Pic

**Which investment level stage attract more investors?**

According to the analysis, Venture-Series Unknown is the most common type of funding for startups, but this is irrelevant because the funding series is unknown. As a result, it could be argued that investors provide additional funds to a start-up during its seed stage, and then again during its Series A stage. This demonstrates that the majority of investors in India's startup ecosystem prefer early-stage investments.

**What sector will a start-up attract more investors or funding?**

From the two graphs provided below, the sectors that received the most funding are Fintechs, Edtechs, and Tech, with fintech leading the way. These industries attract the majority of startups and receive the most funding.

**Will a location of a start-up affect investment drive?**

Bangalore is known as India's Silicon Valley due to its high rate of startup and investment. The majority of startups, according to the bar graph, are located in the top four spots and receive more funding.

**What economic activity of a start-up boost investor funding?**

Venture debt financing, online shopping, and a chain of neighborhood stores and supermarkets are major activities that boost investor funding (e-commerce and commerce). Companies that run a cloud data platform that provides data warehousing services, energy, petrochemicals, textiles, and educational technology that develops personalized learning programs are among these.


**😡Obstacles and Difficulties**
-
Notwithstanding, with regards to the increased number of the Indian startup ecosystem, there are still challenges and barriers to fundraising for Indian startups. One of the most significant challenges is a lack of early-stage funding. Many Indian startups struggle to raise seed or angel funding, making it difficult for them to launch their businesses. Another issue is a lack of investor trust. Many Indian investors are still hesitant to invest in startups, making it difficult for startups to raise the necessary funding.

**:heart_eyes: Summary, Conclusion and Recommendations**
-
•	The majority of start-ups in India revolve around technology, with the majority of them being FINTECHS.

•	In India, finance and location are positively associated. If we locate our startup in Bangalore, there is a strong likelihood that we will find finance quickly.

•	Investors favor the seed stage of a business.

•	Insight from the analysis indicates that we should anticipate more funding in a given year the more start-ups there are.

•	It is recommended that new potential investors should look up for Banglore which is considered as the Silicon Valley of India because it has the greatest setups and funding from the analysis

*Insight gained from the analysis can be concluded that, the Indian startup ecosystem has grown significantly in recent years, with an increase in funding and the number of startups launched. The most funding has gone to the e-commerce, fintech, and healthcare sectors, and the number of startups founded has increased significantly. This is a good sign for the Indian startup ecosystem, and we can anticipate even more growth in the coming years.*




