SELECT *
  
FROM CLASSICMODELS.EMPLOYEES T1
LEFT JOIN CLASSICMODELS.CUSTOMERS T2
ON T1.EMPLOYEENUMBER = T2.SALESREPEMPLOYEENUMBER
where t2.customerNumber is NULL
and jobTitle  = 'Sales Rep'




SELECT A.customerName, B.amount, B.paymentDate
FROM classicmodels.customers A
LEFT JOIN classicmodels.payments B
    ON A.customerNumber = B.customerNumber
WHERE B.customerNumber IS NULL;
