
Understand and apply `CREATE VIEW` to:
- Simplify complex SQL queries
- Abstract database structure
- Enhance data security by limiting access

1. **Created complex SQL views** using JOINs and conditions to filter meaningful data.
2. **Used views for abstraction**, hiding complex JOINs and calculations behind simple SELECTs.
3. **Implemented secure views** to restrict sensitive columns like `salary` from general access.

CREATE VIEW HighSalaryEmployees AS
SELECT e.Name AS EmployeeName, d.DeptName AS Department, e.Salary
FROM Employees e
JOIN Departments d ON e.DepartmentID = d.DepartmentID
WHERE e.Salary > 50000;
