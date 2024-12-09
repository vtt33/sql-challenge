# sql-challenge
QuickDBR

Employees
--
emp_no PK int
title_id int
birth_date date
first_name string
last_name string
sex string
hire_date date

Departments
--
dept_no PK int
dept_name string

Dept_emp
--
emp_no int FK >- Employees.emp_no
dept_no int FK >- Departments.dept_no

Dept_manager
--
dept_no int FK >- Departments.dept_no
emp_no int FK >- Employees.emp_no

Salaries
--
emp_no int FK >- Employees.emp_no
salary

Titles
--
title_id int FK >- Employees.title_id
title string
