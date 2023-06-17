Give me an example of what coding in SQL is like

-- Select all columns from the employees table
SELECT * FROM employees;

-- Select specific columns from the employees table
SELECT employee_id, first_name, last_name FROM employees;

-- Select all employees with a specific job title
SELECT * FROM employees WHERE job_title = 'Manager';

-- Select employees with a salary greater than a certain amount
SELECT * FROM employees WHERE salary > 50000;

-- Select employees whose last name starts with 'S' and work in the Sales department
SELECT * FROM employees WHERE last_name LIKE 'S%' AND department = 'Sales';

-- Select employees sorted by their hire date in descending order
SELECT * FROM employees ORDER BY hire_date DESC;

-- Select the average salary of all employees
SELECT AVG(salary) FROM employees;

-- Update the salary of an employee with a specific ID
UPDATE employees SET salary = 60000 WHERE employee_id = 123;

-- Insert a new employee into the table
INSERT INTO employees (employee_id, first_name, last_name, job_title, salary, hire_date)
VALUES (124, 'John', 'Doe', 'Analyst', 45000, '2022-01-01');

-- Delete an employee with a specific ID
DELETE FROM employees WHERE employee_id = 124;
