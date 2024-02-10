# Diversity-and-Inclusion Analysis

![](diw.jpg)

### BACKGROUND
Human Resources at a telecom client is highly into diversity and inclusion. They’ve been working hard to improve gender balance at the executive management level, but they’re not seeing any progress. They’re reaching out for help. I as a data analyst will try to access the provided data and use data manipulation and analysis will define relevant KPIs in hiring, promotion, performance, and will create a visualization dashboard to show useful insights to the Stakeholders.

### DATA COLLECTION
The dataset was provided as an excel file by PwC from the Human Resources department of a Telecom client during PwC Power Bi in Data Analytics Virtual Case Experience Internship, consisting of 500 rows and 32 columns of the Employees hiring and performance. And the data was gotten from [forage](https://cdn.theforage.com/vinternships/companyassets/4sLyCPgmsy8DA6Dh3/03%20Diversity-Inclusion-Dataset.xlsx)

### SKILL/CONCEPTS DEMONSTRATED
- Defining KPIs.
- Data Cleaning in Power Query.
- DAX Concepts – To Calculate measures
- Data visualization.

### DATA CLEANING AND TRANSFORMATION
The dataset was imported into Power BI Power Query for data validation and transformation.
To accomplish this project, I utilized Power query to clean the data, such as:
- Abbreviated values were expanded e.g. Y replaced with Yes.
- Column datatypes were validated properly.
- Removing missing values and unwanted columns.

### DAX CONCEPTS
To analyze and visualize metrics that show gender distribution in hiring, and promotion. The following DAX measures were created.

**Calculating total number of female employees.**

```
Female Employees = CALCULATE(
    COUNTROWS(
        FILTER('Pharma Group AG',
        'Pharma Group AG'[Gender] = "Female")
    ))
```
**Calculating total number of male employees.**

```
Male Employees = CALCULATE(
    COUNTROWS(
        FILTER('Pharma Group AG',
        'Pharma Group AG'[Gender] = "Male")
    ))
```
**Calculating male percentage hired in this company.**
```
% Of Male = DIVIDE(
    [Male Employees],[Total Employees],0)
```
**Calculating Female percentage hired in this company.**
```
% Of Female = DIVIDE(
    [Female Employees],[Total Employees],0)
```
### INSIGHTS AND RECOMMENDATIONS
- The current workforce comprises of 453 employees of which 59% are males and 41% are females.
- Senior management, where all senior management and leadership are predominantly male, lacks diversity, indicating that there may be bias in recruitment and gender inequality in promotion.
- Since the majority of female employees are in junior positions, organizations can review recruitment and hiring practices and provide training and development opportunities to help women develop the skills needed for senior positions. This may include mentoring and sponsorship programs, leadership training.
- A critical parcel of the senior-level workforce comprises youthful grown-ups (matured 20–29), contributing a important mix of imagination and young vitality to the organization.
