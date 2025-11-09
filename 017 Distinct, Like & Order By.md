SELECT *
FROM customers
WHERE city LIKE '%New%';
Explanation:

SELECT * → fetches all columns from the table.

FROM customers → means you’re querying data from the customers table.

WHERE city LIKE '%New%' → filters rows where the city name contains the word “New” anywhere.

The % is a wildcard that means “any number of characters.”

So it will match cities like New York, Newark, Newcastle, etc

Cities starting with "New":
WHERE city LIKE 'New%';

Cities ending with "York":
WHERE city LIKE '%York';

SELECT DISTINCT country
FROM customers;
Explanation:

SELECT DISTINCT → removes duplicates so each country appears only once.

country → the column you’re listing.

FROM customers → gets data from the customers table.

SELECT *
FROM employees
ORDER BY lastName DESC, firstName DESC;
