# hello_world

just trying out github 
hello
world

select employee.employee_name from employee, works, company where employee.employee_name = works.employee_name and employee.city = company.city and works.company_name = company.company_name

select employee_name from employee where employee_name not in (select employee_name from works where company_name = 'First Bank Corporation');

# Use alias 'p' for the first employee category, alias 'r' for the second employee category and alias 'm' manages relation. 

select p.employee_name from employee p, employee r, manages m where p.employee_name = m.employee_name and m.manager_name = r.employee_name and p.street = r.street and p.city = r.city;

select * from employee where employee_name in (select employee_name from works where company_name = 'First Bank Corporation' and salary = '10000');