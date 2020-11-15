# Pewlett-Hackard-Analysis

Bobby's manager gave us two assignments: determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. 

## Retiring employees per title
We had six csv data files which includes : Deparments, Manager, Employees, Deparment Employee, Salaries, and Title. Our task are to create database for retiring employees per tile. First we create a table named "Retirement Title " using inner join beweent Employees and Title list including filtering base on birth_date from '1952-01-01' AND '1955-12-31'. This table gave the list of employees who eligible for retirement with more than 100k data . The table is show as below :

https://github.com/ttan0408/Pewlett-Hackard-Analysis/blob/main/Retirement_Titles.PNG

After review the data, we found that the list has duplicate employee data since some employees got promoted or change title. Then we use DISTINCT ON the employee number to retrieve the first occurrence of the employee number for each set of rows. After filter out duplicate data we were able to create unique title list as shown :

https://github.com/ttan0408/Pewlett-Hackard-Analysis/blob/main/unique_titles.PNG

Now with the clean employee retirement title table, our final task is to find out how many position for each title will be retired so that our HR department can have the hiring plan in the future. By using COUNT 




