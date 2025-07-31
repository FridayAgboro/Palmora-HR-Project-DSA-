# Palmora Group HR Project (DSA)
This project is about Palmora Group, a manufacturing company based in Nigeria, which is embroiled in issues bordering on gender inequality in its 3 regions, issues on whether there is salary disparity between the male and female gender, and also issues on whether Palmora group as a manufacturing company meets the industry standards for manufacturing companies operating in Nigeria.  

In this project, I would be analyzing the HR data-sets provided using various data analysis tools and present my findings and recoommendations at the end, which would help the HR department deal with the issues raised, and come up with informed decisions that would better position Palmora Group to remain competitive in the industry.


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
- **Data Cleaning / Transformation:**
  -  The data cleaning process started on the Gender Column, where I replaced blank/empty fields with Unknown using replace value.
  -  Deleted the rows with "null" under department column by unchecking "null" in the drop-down on the column.
  -  Deleted the blank rows in the salary column by unchecking the "blank" in the drop-down on the salary column.
  -  Selected the department column and unpivot other columns.
- **Uploading the second data-set** The "Palmora Group Bonus Rules" file.
- **Creating the Bonus Rules** I used merge query then selected the Employee File first and also selected the Bonus rules file after which I select the columns similar to both of them.
- **I used custom column** To create a Bonus Column
- **I used Condition column** To create other columns like (New Salary, Salary Above 90000, Salary Groupng - which I used as Salary Band)
- **I removed the duplicate rows** I selected the name column, department column and salary column and clicked remove duplicate.
- At the end of the cleaning, the numbers of employees reduced to **874**.
  
![Pal Additional column](https://github.com/user-attachments/assets/0d8704e1-c3c6-492f-9537-b0664eb31883)


## Creating the Dashboard
1. The Dashboard creation started by insertion of a "Text Box" at the top of the Canvas and putting the Project Title and my name on it.
2. I used the "Card" to highlight major figures in my findings
3. **Total Number of Employees:** I inserted the card, selected Name and set it to count of name.
4. **Number of Female Employees:** I inserted the card, selected Gender, set it to count of gender and filter it to female.
5. **Number of Male Employees:** I inserted the card, selected Gender, set it to count of gender and filter it to male.
6. **Total Anual Salary:** I inserted the card, selected New Salary, set it to sum of new salary.
7. **Numbers of Employees that earn over N90,000:** I inserted the card, selected Salary above 90000, set it to count of salary above 90000 and filtered it to above 90000.
8. **Numbers of Employees that earn below N90,000:** I inserted the card, selected Salary above 90000, set it to count of salary above 90000 and filtered it to below 90000.
9. **Total Numbers of Departments:** I inserted the card, selected Department, set it to count of department and filtered it to distint count.
10. **Total Numbers of Regions:** I inserted the card, selected Location, set it to count of Location and filtered it to distint count.

#### _**Gender Distribution and Region**_
- This was done by inserting the Clustered Bar Chart, then put location on Y-Axis, count of name on X-Axis and gender on legend.

#### _**Gender Distribution and Department**_
- I inserted the Matrix Card, put Department on Row, Gender on Columns and Name on Value (filter to count).

#### _**Rating By Gender**_
- I inserted the 100% Stacked Chart, put Ratings on Y-Axis, Name on X-Axis (filter to count) and Gender on Legend.

#### _**Salary by Deprtment and Gender**_
- I inserted the Stacked Bar Chart, put Department on Y-Axis, New Salary on X-Axis (filter to sum) and Gender on Legend.

#### _**Numbers of Employees by Salary Band**_
- I inserted the Stacked Bar Chart, put Salary Grouping on X-Axis, Salary Grouping on X-Axis (filter to count).

#### _**Numbers of Gender by Rating**_
- I inserted Matrix, put Rating on Row, Gender on Columns, Rating on Value (filter to count).

#### _**Numbers of Employees that Earn Above and Below N90,000**_
- I inserted Matrix, put Salary above N90,000 on Row, Location on Columns, Name on Value (filter to count).


## Dashboards
- **Dashboard 1**

![dasboard 1](https://github.com/user-attachments/assets/4f199c72-df6e-478a-aa2c-77a6a5164ee9)

- **Dashboard 2**

![dasboard 2](https://github.com/user-attachments/assets/534bcecb-3505-47f3-978d-a39e4cc0040f)

- **Dashboard 3**
  
![dasboard 3](https://github.com/user-attachments/assets/8809ed01-7c01-4cbf-8ece-3890170e20a4)


## My Findings

- **Total Numbers of Employees:** 874

- **Total Numbers of Female Employees:** 406

- **Total Numbers of Male Employees:** 430

- **Total Employees Salary:** N67 Million

- **Highest Paid employee:** Evangelia Growers | N127,097

- **Highest Bonus Earner:** Chrisy Kyme | N9,821

- **Number of Employees That Earn Over N90,000:** 307
  
- **Number of Employees That Earn Below N90,000:** 570

- **Total Number of Departments:** 12

- **Total Number of Regions:** 3
  


### Gender Distribution
Gender Distribution across Palmora Group has a bias of 430 Male to 406 Female by my findings.

_**Gender Distribution By Departments**_


- **Training**: Male 35  | Female 34  | Unknown 3 
  
- **Support**: Male 41  | Female 30  | Unknown 4  

- **Services**: Male 35  | Female  39 | Unknown 3 

- **Sales**: Male 39  | Female 32  | Unknown 4 

- **Research and Development**: Male 28  | Female 32  | Unknown 5 

- **Product Management**: Male 40  | Female 39  | Unknown 1 

- **Marketing**: Male 31  | Female 31  | Unknown 1

- **Legal**: Male 44  | Female 32  | Unknown 4 

- **Human Resources**: Male 33  | Female 37  | Unknown 3 

- **Engineering**: Male 35  | Female 35  | Unknown 5  

- **Business Development**: Male 33  | Female 38  | Unknown 3  

- **Accounting**: Male 36  | Female 27  | Unknown 2  

![Gender distribution by Dept](https://github.com/user-attachments/assets/0cf8e88e-1fc4-417c-a0e9-95245ebcf12d)




_**Gender Distribution By Regions**_

- **Abuja**: Male 144  | Female 144  | Unknown 16 

- **Kaduna**: Male 172  | Female 151  | Unknown 14 

- **Lagos**: Male 114  | Female 111  | Unknown 8 

![image](https://github.com/user-attachments/assets/b4aed707-6716-4af2-915e-a69523d2ee8d)



### Insight on Ratings Based on Gender

Generally, the Female employees have better ratings than the male employees as shown below, where the female are more rated "Very Good" and "Good", while male are more rated "Average", "Poor", and "Very Poor". This is an indication that Female employees contribute better to Palmora Group's goals than the Male employees.

- **Very Good:** Female 44 | Male 32 | Unknown 5
  
- **Good:** Female 82 | Male 73 | Unknown 8

- **Avarage:** Female 180 | Male 203 | Unknown 17

- **Poor:** Female 49 | Male 64 | Unknown 3

- **Very Poor:** Female 19 | Male 31 | Unknown 3

- **Not Rated:** Female 32 | Male 27 | Unknown 2

![image](https://github.com/user-attachments/assets/efbe69a6-076b-4d18-b3f1-5d76c21bc5f6)



### Analysis of Palmora Salary Structure

#### *Palmora Total Salary*

- N67 Million - Approximately (N66,559,937 Actual Figure)
  

#### *Palmora Total Salary By Gender*

- **Male:** N32,984,598
  
- **Female:** N30,461,676
  
- **Unknown:** N3,113,663

![image](https://github.com/user-attachments/assets/606a52bf-bd07-45cf-ae89-e38849f3722a)


#### *Palmora Salary By Gender and Regions*

-	**Abuja:** Female N10,185,370   |  Male N10,600,240  |  Unknown N1,215,440
  
-	**Kaduna:** Female N10,957,800 |  Male N12,737,700  |  Unknown N1,101,000
  
-	**Lagos:** Female N8,336,390 |  Male N8,699,920  |  Unknown N694,880

![image](https://github.com/user-attachments/assets/2a140041-a1c4-4570-883f-c1a47d25b393)


#### *Palmora Salary By Gender and Departments*

-	**Accounting Male:** ₦ 2,832,129 | Female  ₦ 2,034,091 | Unknown  ₦ 213,292
  
-	**Business Development:** Male**  ₦ 2,743,173 | Female  ₦ 2,923,633 | Unknown  ₦ 155,893
  
-	**Engineering Male:**  ₦ 2,458,732 | Female ₦ 2,707,862 | Unknown  ₦ 414,046
  
-	**Human Resources:** Male  ₦ 2,529,724 | Female  ₦ 2,555,019 | Unknown ₦ 290,487
  
-	**Legal Male:**  ₦ 3,329,620 | Female  ₦ 2,291,993 | Unknown  ₦ 345,749
  
-	**Marketing Male:** ₦ 2,351,428 | Female  ₦ 2,548,813 | Unknown  ₦ 106,399
  
-	**Product Management Male:**  ₦ 3,019,817 | Female  ₦ 2,872,998 | Unknown  ₦ 37,647
  
-	**Research and Development:**  Male  ₦ 2,023,931 | Female  ₦ 2,270,308 | Unknown  ₦ 405,912
  
-	**Sales Male:**  ₦ 2,861,859 | Female  ₦ 2,307,704 | Unknown  ₦ 363,986
  
-	**Services Male:**  ₦ 2,896,340 | Female  ₦ 2,982,293 |Unknown  ₦ 202,590
  
-	**Support Male:**  ₦ 3,251,044 | Female | ₦ 2,219,956 | Unknown  ₦ 311,030
  
-	**Training Male"**  ₦ 2,686,801 | Female  ₦ 2,747,006 | Unknown  ₦ 266,632



![image](https://github.com/user-attachments/assets/0b4b6fd9-1b58-4173-bd46-26f06f8b6aa0)


  
#### *Numbers of Staff By Salary Band*

-	**20001 – 30000:** 9
  
-	**30001 – 40000:** 101

-	**40001 – 50000:** 94

-	**50001 – 60000:**  83

-	**60001 – 70000:** 79

-	**70001 – 80000:** 115
  
-	**80001 – 90000:** 115

-	**90001 - 100000:** 88
  
- **100001 - 110000:** 87
  
- **110001 - 120000:** 96
  
- **120001 - 130000:** 33

  


![SalaryBand](https://github.com/user-attachments/assets/ee8bf502-8841-47c0-b11a-5f52c65de82e)


<img width="274" height="241" alt="image" src="https://github.com/user-attachments/assets/c998014c-ad0b-46fe-909d-06f4287e800a" />


### Average Salary 

- Average Salary is: N76,155.53
  

#### *Average Salary by Region*

![image](https://github.com/user-attachments/assets/bc1bd556-aa05-43e9-8b9a-5deb09702e63)


#### *Total Salary by Region*

<img width="212" height="81" alt="image" src="https://github.com/user-attachments/assets/37a13e45-563d-48ae-b134-7712066aa15a" />


#### *Average Salary bye Department and Gender*

![image](https://github.com/user-attachments/assets/a67b60bc-ca46-4a95-818c-3c7609205214)




#### *Organization-wide Individual Salaries*

![individual salary](https://github.com/user-attachments/assets/0750eccb-673b-4d54-b41c-6b7c2d332bd6)


#### *Organization-wide Individual Bonuses*

![Bonus](https://github.com/user-attachments/assets/b7aedea1-d727-43aa-8949-37a10cf89997)



### How Palmora stand in relation to N90,000 Minimum Wage for Manufacturing Companies
- Palmora Group as a manufacuring company operang in Nigeria, did not meet the industry standard of N90,000 minimum wage, as my analysis reveals that of the **874** Employees of Palmora, only **304** earn N90,000 and above while a huge number of **570** earn below N90,000.
- The average salary in Palmoa Group is N76,155.53.


![no of staff above 90000](https://github.com/user-attachments/assets/89ec046d-8fde-4525-9e17-2356be921e05)


## Recommendations
- Palmora Group have a Gender bias of **430 Male Enployees** to **406 Female Employees**. This needs to be looked at especially in the Legal Department where Males are 73% Higher.
- Female employees needs to the appreciated more as findngs from rating shows they contribute better to the organisation than the male employees. (Female employees have better ratings).
- Palmora should adopt a policy of full dislosure of gender status, this would help in getting a more acurate gender disperity status in the establishment as **38** employees did not disclose their gender and this figure is higher than the difference between the male and female gender which is 24. If full disclosure had been made, probably, there won't be gender disparity or the gender disparity could go either way.
- Palmora Group needd to increase employees salary to meet the industry standard of a minimum salary of N90,000. Of the total **874** employees, only **304** earn N90,000 and above, while **570** employees earn below the N90,000 industry standard. The average salary is N76,155.53
- There are fewer Employees in Lagos Region compare to employees in others locations this needs to be looked at.


### _Please Note: You can fine The Completed Power BI File as an Upload to this Repository_

## About Me
Friday Agboro ( Brand Management  |  Graphics Designer | PowerPoint Presentation Formatting |  Data Analyst )

## Contact
- Phone: +234 08059002119
- Email: widercoast@gmail.com
- I'm available for immediate employment or to handle your data analysis jobs


THank you
