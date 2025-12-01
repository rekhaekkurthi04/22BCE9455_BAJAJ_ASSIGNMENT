# 22BCE9455_BAJAJ_ASSIGNMENT
JAVA Intern Assignment
##code
{
  "finalQuery": "SELECT d.department_name AS DEPARTMENT_NAME, ROUND(AVG(TIMESTAMPDIFF(YEAR, e.dob, CURDATE())), 2) AS AVERAGE_AGE, GROUP_CONCAT(CONCAT(e.first_name, ' ', e.last_name) ORDER BY e.first_name SEPARATOR ', ') AS EMPLOYEE_LIST FROM department d JOIN employee e ON d.department_id = e.department JOIN payments p ON e.emp_id = p.emp_id WHERE p.amount > 70000 GROUP BY d.department_id, d.department_name ORDER BY d.department_id DESC;"
}
