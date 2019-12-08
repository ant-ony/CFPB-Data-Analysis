## Exploratory Data Analysis and NLP of Consumer Financial Protection Bureau Complaints

## Introduction
The Consumer Financial Protection Bureau receives survey data from US consumers regarding complaints against financial companies and their business practices.  This data provides informaton on complaints regarding different companies, regions, and types of products.

## Purpose
The purpose of this project is to analyze a CFPB dataset containing information about consumer complaints in two ways.  First, to analyze 
the complete landscape of complaints for all financial companies.  Second, to 
look at a single company and connect the analysis to different business impacts.

This repository includes the following main files:

* a dataset `Consumer_Complaints.csv` used to perform the analysis.
* a jupyter notebook that shows data cleaning and exploratory data analysis of the financial industry at-large called `exploratoryDataAnalysis.ipynb`. 
* a jupyter notebook that shows the exploratory data analysis of a single company performed called `exploratoryDataAnalysisMTBank.ipynb`. 
* a jupyter notebook that shows the data cleaning process used called `cleaningData`. 


## Data Set Information
Information contained in the raw_data file.

## Analysis

`exploratoryDataAnalysis.ipynb` perform the following tasks:

* Reads the `CSV file` into a **Pandas DataFrame**.
* Replacing categorical values like CompanyResponseToConsumer, TimelyResponse, and ConsumerDisputed for `1` or `0`.
* *Exploratory Data Analysis*:
    - Checks if dataset suffers of **Class imbalance**
    - Obtains descriptive statistics summarizing central tendency, dispersion and shape of the dataset’s distribution
    - Creates visuals in order to explore the relationships existent in the dataset
    - Conclusions:  On a broad scale, US consumers are experiencing the most issues with credit reporting and mortgages -- two integral products for everyday Americans that are practically unavoidable. Debt collection is a major issue and raises questions of how prepared and educated consumers are when taking on debt. Credit cards are not far behind in terms of consumer complaints, this may suggest covariation between debt collection and credit card complaints, especially given that credit card debt has soared past $1 trillion this year. (https://www.debt.org/faqs/americans-in-debt/)  These findings are confirmed through sentiment analysis and natural language processing.

`exploratoryDataAnalysisMTBank.ipynb` perform the following tasks:

* Reads the `CSV file` into a **Pandas DataFrame**.
* *Exploratory Data Analysis*:
    - Obtains descriptive statistics summarizing central tendency, dispersion and shape of the dataset’s distribution
    - Creates visuals in order to explore the relationships existent in the dataset
    - Conclusions:  In our single company analysis, there are a number of business proposals we can make centered around mortgages, bank services, and checking/savings accounts. The top priority to address consumer complaints should be around payments/managing a mortgage. The next would be the account opening, closing, management process. Lastly, would be to address deposits and withdrawals complaints.  Proposals include: For Mortgages: 1. Raise standards for the underwriting process to reduce the number of consumers who may run into difficulty making payments. 2. Hands-on approach to outreach when a customer is late on a payment, mailing out a notice could be combined with outreach from a local Branch representative who may be familiar with the customer and could understand what their situation is and properly advise. For Account Opening, Closing, and Management: 1. Simplify and target the pain points of account opening so that the process is less troublesome and confusing. 2. Better training for employees to emphasize specific disclosures and rules. 3. For the mobile opening process, highlight key areas of the terms of service / disclosures either through video or quick summaries. For Deposits and Withdrawals: 1. Greater communication to the customer from branch representatives on why a deposit would be held up. 2. Including on the receipt when the funds will be available as Bank of America does.


## References
1. Downloaded financial services consumer complaint raw data from CFPB, data from 12/1/2011 until 10/25/2019.  1,048,576 rows, 18 columns. https://catalog.data.gov/dataset/consumer-complaint-database#topic=consumer_navigation
