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
