# Palmora Group HR Project (DSA)
This project is about the Palmora Group, a manufacturing company based in Nigeria, that is embroiled in issues bordering on gender inequality in its 3 regions.  I am looking to providing solution to the gender issues with my analysis of the HR dataset provided.


## Project Goals
To assist HR professionals and data analysts in identifying key workforce insights and taking necessary actions to provide fair representations, and compensation alignment.

## Raw Dataset Highlights
- **Number of Dataset Provided**: 2 ( **Palmora Group emp-data** and **Palmora Group Bonus Rules**) 
- **Palmoria Group emp-data**: Has 6 columns and 1016 Rows
- **Palmoria Group Bonus Rules**: Has 6 Columns and 13 Rows

![Raw pal](https://github.com/user-attachments/assets/bb7622bd-cb7b-4fae-841f-24c23cdefc0d)

![Raw pal 2](https://github.com/user-attachments/assets/87a098ec-30d7-41e6-b19b-b5c5592f3130)

## Tools Used
- Power Query
- Microsoft Power BI

## Data Cleaning Process
- **Ingestion:** Getting the Data Set into Power Query Environment
- **TransformationUsing:** On the Gender Column, I replaced value blank with Unknown. I delected the rows with "null" under department column by unchecking "null" in the drop-down on the column. I also deleted the blank row in the salary column by unchecking the "blank" in the drop-down on the salary column.  I selected the department column and unpivot other columns. I brought in the "Palmora Group Bonus Rules" file.
- **Creating the Bonus Rules** I used merge query then selected the Employee File first and also selected the Bonus rules file after which I select the columns similar to both of them.
- **I used custom column** To create a Bonus Column
- **I used Condition column** To create other columns like (New Salary, Salary Above 90000, Salary Groupng - which I used as Salary Band)

![Pal Additional column](https://github.com/user-attachments/assets/0d8704e1-c3c6-492f-9537-b0664eb31883)


## Creating the Dashboard
Started the creation of the Dashboard by Inserting a "Text Box" at the top of the Canvas and Typed in the Project Title and my name.
I used the "Card" to highlight major figures in my findings
1. **Total Number of Employees:** I inserted the card, selected Name and set it to count of name.
2. **Number of Female Employees:** I inserted the card, selected Gender, set it to count of gender and filter it to female.
3. **Number of Male Employees:** I inserted the card, selected Gender, set it to count of gender and filter it to male.
4. **Total Anual Salary:** I inserted the card, selected New Salary, set it to sum of new salary.
5. **Numbers of Employees that earn over N90,000:** I inserted the card, selected Salary above 90000, set it to count of salary above 90000 and filtered it to above 90000.
6. **Numbers of Employees that earn below N90,000:** I inserted the card, selected Salary above 90000, set it to count of salary above 90000 and filtered it to below 90000.
7. **Total Numbers of Departments:** I inserted the card, selected Department, set it to count of department and filtered it to distint count.
8. **Total Numbers of Regions:** I inserted the card, selected Location, set it to count of Location and filtered it to distint count.

#### **Gender Distribution and Region**
- I inserted the Clustered Bar Chart, put location on Y-Axis, count of name on X-Axis and gender on legend.



#### **Gender Distribution and Department**
- I inserted the Matrix Card, put Department on Row, Gender on Columns and Name on Value (filter to count).

#### **Rating By Gender**
- I inserted the 100% Stacked Chart, put Ratings on Y-Axis, Name on X-Axis (filter to count) and Gender on Legend.

#### **Salary by Deprtment and Gender**
- I inserted the Stacked Bar Chart, put Department on Y-Axis, New Salary on X-Axis (filter to sum) and Gender on Legend.

#### **Numbers of Employees by Salary Band**
- I inserted the Stacked Bar Chart, put Salary Grouping on X-Axis, Salary Grouping on X-Axis (filter to count).

#### **Numbers of Gender by Rating**
- I inserted Matrix, put Rating on Row, Gender on Columns, Rating on Value (filter to count).

#### **Numbers of Employees that Earn Above and Below N90,000**
- I inserted Matrix, put Salary above N90,000 on Row, Location on Columns, Name on Value (filter to count).


## Dashboard

![DASHBOARD](https://github.com/user-attachments/assets/976c6c39-1cd0-44c1-a3d7-208bae6be17a)



## My Findings

- **Total Numbers of Employees:** 874

- **Total Numbers of Female Employees:** 406

- **Total Numbers of Male Employees:** 430

- **Total Employees Salary:** N33 Million

- **Number of Employees That Earn Over N90,000:** 307
  
- **Number of Employees That Earn Below N90,000:** 570

- **Total Number of Departments:** 12

- **Total Number of Regions:** 3
  


## Gender Distribution
Gender Distribution across Palmora Group is fairly balanced as indicated by my findings across the various regions and departments which did not indicate any significant gap between the two genders, the numbers of males are higher than females in 8 departments (Training, Support, Sales, Product Management, Marketing, Legal, Engineering, and Accounting) while the numbers of females are higher than males in 4 departments (Services, Research and Development, Human Resouces, and Business Development). However, major gender gaps of over 20% and above are noticed in 3 departments (Research and Development - Females are 27% Higher, Legal - Males are 50% Higher, and Business Development - Females are 28% higher) as highlighted below:


_**Gender Distribution By Departments**_

- **Training**: Male 61  | Female 55  | Unknown 4 | (Males are 10.9% Higher)
  
- **Support**: Male 54  | Female 50  | Unknown 5  | (Males are 8% Higher)

- **Services**: Male 54  | Female  62 | Unknown 5  | (Females are 14.4% Higher)

- **Sales**: Male 50  | Female 48  | Unknown 4  | (Males are 4.2% Higher)

- **Research and Development**: Male 63  | Female 80  | Unknown 9  | (Females are 27% Higher)

- **Product Management**: Male 65  | Female 61  | Unknown 1  | (Males are 6.6% Higher)

- **Marketing**: Male 53  | Female 48  | Unknown 2  | (Males are 10.4% Higher)

- **Legal**: Male 60  | Female 40  | Unknown 9  | (Males are 50% Higher)

- **Human Resources**: Male 48  | Female 50  | Unknown 3  | (Females are 4.2% Higher)

- **Engineering**: Male 58  | Female 55  | Unknown 12  | (Males are 5.5% Higher)

- **Business Development**: Male 50  | Female 64  | Unknown 5  | (Females are 28% Higher)

- **Accounting**: Male 46  | Female 40  | Unknown 3  | (Males are 15% Higher)



![Gender distribution by Dept](https://github.com/user-attachments/assets/9006e8b1-4452-42ff-9a65-a454c6eb4aad)



_**Gender Distribution By Regions**_

- **Abuja**: Male 229  | Female 247  | Unknown 25  |  (Females are 7.9% higher)

- **Kaduna**: Male 257  | Female 233  | Unknown 24  |  (Males are 10.3% higher)

- **Lagos**: Male 176  | Female 173  | Unknown 13  |  (Males are 1.7% higher)


![Gender distribution by Region](https://github.com/user-attachments/assets/63bf141e-7652-4d21-99c7-de140b344550)



## Insight on Ratings Based on Gender

- **Very Good:** Female 105 | Male 74 | Unknown 10
  
- **Good:** Female 188 | Male 167 | Unknown 19

- **Avarage:** Female 190 | Male 212 | Unknown 18

- **Poor:** Female 98 | Male 122 | Unknown 6

- **Very Poor:** Female 37 | Male 53 | Unknown 7

- **Not Rated:** Female 35 | Male 34 | Unknown 2

![gender by rating](https://github.com/user-attachments/assets/22ba761b-533b-4d74-9119-62f1496f317f)



## Analysis of Palmora Salary Structure

### Palmora Total Salary

- N102,021,320


### Palmora Total Salary By Gender

- **Female:** N47,330,760
  
- **Male:** N49,870,490
  
- **Unknown:** N4,820,070


### Palmora Salary By Gender and Regions

-	**Abuja:** Female N17,725,870  |  Male N16,836,540  |  Unknown N1,861,680
  
-	**Kaduna:** Female N16,812,520 |  Male N19,443,670  |  Unknown N1,873,360
  
-	**Lagos:** Female N12,792,370 |  Male N13,590,280  |  Unknown N1,085,030 

![salary by gender by region](https://github.com/user-attachments/assets/3367063e-ca4d-4342-9e45-41ad11369556)


### Palmora Salary By Gender and Departments

-	**Training:** Female N4,344,390  |  Male N4,606,470  |  Unknown N339,510  |  Total N9,290,370
  
-	**Support:** Female N3,686,480 |  Male N4,269,460  |  Unknown N363,750 |  Total N8,319,690
  
-	**Services:** Female N4,657,540 |  Male N4,367,180  |  Unknown N329,950 |  Total N9,354,670
  
-	**Sales:** Female N3,350,330 |  Male N3,616,280  |  Unknown N356,500 |  Total N7,323,110
  
-	**Research and Development:** Female N5,413,270 |  Male N4,397,060  |  Unknown N707,810 |  Total N10,518,140
  
-	**Product Management:** Female N4,372,130 |  Male N5,097,190  |  Unknown N36,480 |  Total N9,505,800
  
-	**Marketing:** Female N3,754,680 |  Male N3,860,640  |  Unknown N211,740 |  Total N7,827,060
  
-	**Legal:** Female N2,759,560 |  Male N4,348,270  |  Unknown N711,370 |  Total N7,819,200
  
-	**Human Resources:** Female N3,308,790 |  Male N3,526,870  |  Unknown N282,850 |  Total N7,118,510
  
-	**Engineering:** Female N4,029,610 |  Male N4,014,490  |  Unknown N920,280 |  Total N8,964,380
  
-	**Business Development:** Female N4,778,220 |  Male N4,213,510  |  Unknown N247,600 |  Total N9,239,330
  
-	**Accounting:** Female N2,875,760 |  Male N3,553,070  |  Unknown N312,230 |  Total N6,741,060


![salary by gender by dept](https://github.com/user-attachments/assets/42bc0f80-a090-44eb-8e36-9d477c5bc3c0)

  
### Numbers of Staff By Salary Band

-	**N90,000 and above:** 490

-	**N80,100 – N90,000:** 145

-	**N70,100 – N80,000:** 180

-	**N60,100 – N70,000:** 121

-	**N50,100 – N60,000:** 130

-	**N40,100 – N50,000:** 153

-	**N30,100 – N40,000:** 145

-	**N20,100 – N30,000:** 13

![No of employee by sal band](https://github.com/user-attachments/assets/7fb362ea-4557-4972-bd6c-ae34f09fdd81)


### How Palmora stand in relation to N90,000 Minimum Wage for Manufacturing Companies
Palmora did not meet the industry standard of N90,000 minimum wage, as my analysis reveals that of the **1377** Employees of Palmora, only **490** earn N90,000 and above while a huge number of **887** earn below N90,000.

![no of staff above 90000](https://github.com/user-attachments/assets/fd30b6d3-64f9-46cc-a0c4-48430d5d46fa)


## Recommendations
- Palmora Group needs to balance Gender bias in the following Departments where major bias are noticed, bias against males in 2 departments (Research and Development - Females are 27% Higher, and Business Development - Females are 28% higher), while bias against female is noticed in 1 department (Legal - Males are 50% Higher). 
- Palmora Group needd to increase employees salary to meet the industry standard of a minimum salary on N90,000.
- There are fewer Employees in Lagos Region compare to employees in others locations this needs to be looked at.
  

## About Me
Friday Agboro ( Brand Management  |  Graphics Designer | PowerPoint Presentation Formatting |  Data Analyst )

## Contact
- Phone: +234 08059002119
- Email: widercoast@gmail.com


THank you
