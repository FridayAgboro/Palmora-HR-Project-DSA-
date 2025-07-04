# Palmora Group HR Project (DSA)
This project is about the Palmoria Group, a manufacturing company based in Nigeria, that is embroiled in issues bordering on gender inequality in its 3 regions.  I am looking to providing solution to the gender issues with this project.


## Project Goal
To assist HR professionals and data analysts in identifying key workforce insights and taking data-driven actions to improve fairness, representation, and compensation alignment.

## Raw Dataset Highlights
- **Number of Dataset Provided**: 2 ( **Palmora Group emp-data** and **Palmora Group Bonus Rules**) 
- **Palmoria Group emp-data**: Has 6 columns and 1016 Rows
- **Palmoria Group Bonus Rules**: Has 6 Columns and 13 Rows

## Tools Used
- Power Query
- Microsoft Power BI

## Data Cleaning Process
- **Ingestion:** Getting the Data Set into Power Query Environment
- **TransformationUsing:** On the Gender Column, I replaced value blank with Unknown. I delected the rows with "null" under department column by unchecking "null" in the drop-down on the column. I also deleted the blank row in the salary column by unchecking the "blank" in the drop-down on the salary column.  I selected the department column and unpivot other columns. I brought in the "Palmora Group Bonus Rules" file.
- **Creating the Bonus Rules** I used merge query then selected the Employee File first and also selected the Bonus rules file after which I select the columns similar to both of them.
- **I used custom column** To create a Bonus Column
- **I used Condition column** To create other columns like (New Salary, Salary Above 90000, Salary Groupng - which I used as Salary Band)

## Creating the Dashboard
Started the creation of the Dashboard by Inserting a "Text Box" at the top of the Canvas and Typed in the Project Title and my name.
I used the "Card" to highlight major indices of my findings
1. **Total Number of Employees:** I inserted the card, selected Name and set it to count of name.
2. **Number of Female Employees:** I inserted the card, selected Gender, set it to count of gender and filter it to female.
3. **Number of Male Employees:** I inserted the card, selected Gender, set it to count of gender and filter it to male.
4. **Total Anual Salary:** I inserted the card, selected New Salary, set it to sum of new salary.
5. **Numbers of Employees that earn over N90,000:** I inserted the card, selected Salary above 90000, set it to count of salary above 90000 and filtered it to above 90000.
6. **Numbers of Employees that earn below N90,000:** I inserted the card, selected Salary above 90000, set it to count of salary above 90000 and filtered it to below 90000.
7. **Total Numbers of Departments:** I inserted the card, selected Department, set it to count of department and filtered it to distint count.
8. **Total Numbers of Regions:** I inserted the card, selected Location, set it to count of Location and filtered it to distint count.

### Gender Distribution and Region
- I inserted the Clustered Bar Chart, put location on Y-Axis, count of name on X-Axis and gender on legend.

### Gender Distribution and Department
- I inserted the Matrix Card, put Department on Row, Gender on Columns and Name on Value (filter to count).

### Rating By Gender
- I inserted the 100% Stacked Chart, put Ratings on Y-Axis, Name on X-Axis (filter to count) and Gender on Legend.

### Salary by Deprtment and Gender
- I inserted the Stacked Bar Chart, put Department on Y-Axis, New Salary on X-Axis (filter to sum) and Gender on Legend.

### Numbers of Employees by Salary Band
- I inserted the Stacked Bar Chart, put Salary Grouping on X-Axis, Salary Grouping on X-Axis (filter to count).

### Numbers of Gender by Rating
- I inserted Matrix, put Rating on Row, Gender on Columns, Rating on Value (filter to count).

### Numbers of Employees the Earn Above and Below N90,000
- I inserted Matrix, put Salary above 90000 on Row, Location on Columns, Name on Value (filter to count).


## Dashboard

![PALMORA DASHBOARD](https://github.com/user-attachments/assets/d201daed-1474-453f-aa13-428fcf2c9da4)

## My Findings

- **Total Numbers of Employees:** 1377

- **Total Numbers of Female Employees:** 653

- **Total Numbers of Male Employees:** 662

- **Total Employees Salary:** N52 Million

### Gender Distribution
Gender Distribution is fair across Palmora Group as indicated by my findings across the various regions as highlighted below:

**Abuja**: Male 229  | Female 247  | Unknown 25

**Kaduna**: Male 257  | Female 233  | Unknown 24

**Lagos**: Male 176  | Female 173  | Unknown 13


## About Me
Friday Agboro ( Brand Management  |  Graphics Designer | PowerPoint Presentation Formatting |  Data Analyst )

## Contact
- Phone: +234 08059002119
- Email: widercoast@gmail.com


## About Me
Friday Agboro ( Brand Management  |  Graphics Designer | PowerPoint Presentation Formatting |  Data Analyst )

## Contact
- Phone: +234 08059002119
- Email: widercoast@gmail.com


THank you
