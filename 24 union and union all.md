🧠 When do you use UNION?

You use UNION when you need to combine rows from different tables that are:

related

similar

but not joined by a key.

For example:

List all people from customers and employees

Combine all phone numbers from two tables

Combine archived and active data

Combine historical and new tables


select 'customer' as type,
       contactFirstName as firstname,
       contactLastName as lastname
from customers

UNION

select 'employee' as type,
       firstname,
       lastname
from employees;
