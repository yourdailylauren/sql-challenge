# sql-challenge

Table schemas for assignment:
departments
-
dept_no PK varchar(4)
dept_name varchar(255)

employees
-
emp_no PK int
emp_title_id varchar(255)
birth_date date
first_name varchar(255)
last_name varchar(255)
sex char(1)
hire_date date

dept_emp
-
emp_no PK FK - employees.emp_no
dept_no PK FK - departments.dept_no

dept_manager
-
dept_no PK FK - departments.dept_no
emp_no PK FK - employees.emp_no

salaries
-
emp_no PK FK - employees.emp_no
salary int
