# **Pewlett-Hackard-Analysis**
# *Overview of the Analysis*
The purpose of this analysis is to prepare Pewlett-Hackard for the upcoming “silver tsunami”. A large number of employees will begin retiring in upcoming years and the company wants to be prepared with the retirement packages, open positions and employees’ training. Company managers wants to get analysis on the basis of following:

1) Determine the number of retiring employees per title
2) Identify employees who are eligible to participate in a mentorship program

## **Tools**

- PostgreSQL
- pgAdmin
- Visual studio
- Quick DBD 

# *Results*
## **ERD Schema**

The image below is the ERD schema that was used to build queries for this challenge.

![EmployeeDBD-export](https://user-images.githubusercontent.com/96033163/154849177-93f33355-77d6-4029-8dba-23910eaa54ff.png)


## **The Number of Retiring Employees by Title**

Created a Retirement Titles table that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. Because some employees had multiple titles in the database—for example, due to promotions— so used the *DISTINCT ON* statement to create a table that contains the most recent title of each employee.Below is the image of the coding:

![Number of retiring employees by title](https://user-images.githubusercontent.com/96033163/154849172-6a8921aa-882c-4098-90c2-4d2e06166c73.PNG)

We got the below table from above coding

![retiring list with titles](https://user-images.githubusercontent.com/96033163/154849174-5f5c01ca-bd46-4675-8364-511dd4ed5e56.PNG)

 Then finally, used the *COUNT()* function to create a table that has the number of retirement-age employees by most recent job title.Below is the image of the table count

![total count of with titles](https://user-images.githubusercontent.com/96033163/154849176-f2c66167-8ac2-41f5-becb-f8f9b652bae1.PNG)


## **Mentorship Program**

Created a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965. Below is the code

![mentorship eligibilty](https://user-images.githubusercontent.com/96033163/154849171-76df35b7-678a-4e64-bf34-7de436fe3dd9.PNG)

We got the following table from the coding

![mentorship eligibilty list](https://user-images.githubusercontent.com/96033163/154849170-f27e4a84-6d03-4b7a-9516-8746f227bdde.PNG)


# *Summary*
**1) Total roles to be filled?** 
  
  * 72,458 roles are in need to be filled out

**2) How many are eligible for mentorship program**

   * Only 1,549 employees are eligible to participate in a mentorship program.