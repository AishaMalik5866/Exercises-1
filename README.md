# Exercises-1


*these are basic query exercies I did from made-up databases from a made-up company*

*the database names for the made-up company are sql_invoicing, sql_store, sql_inventory, sql_hr*

-------------------------------------------------------------------------------------------

USE store;

*doing exercises from store database*

----------

SELECT * 

FROM customers

WHERE points >=1000 AND points <=3000;

*finding customers who have over 1000 points and under 3000 points*

-----------------

SELECT * 

FROM customers

WHERE points BETWEEN 1000 AND 3000;

*doing the same as above, but with BETWEEN operator*

--------------

SELECT * 

FROM customers

WHERE birth_date BETWEEN '1990-01-01' AND '2000-01-01';

*finding customers born betwee 1/1/1990 and 1/1/2000*

-----------

SELECT * 

FROM customers

WHERE last_name LIKE '%y' OR 
      last_name LIKE '____tt' OR 
      last_name LIKE 'b%';

*finding last names that end with 'y', start with 'b', or contain 4 characters before 'tt'*

--------------

SELECT * 

FROM customers

WHERE last_name 

REGEXP 'field$|^mac|rose|[am]g';

*finding last names that end in 'field', start with 'mac', contain 'rose', or contain 'a' or 'm' before a 'g'*

-------------------

SELECT * 

FROM customers

WHERE phone IS NULL;

*finding customers who have not provided a phone number*

----------------

SELECT * 

FROM customers

ORDER BY points DESC 

LIMIT 3;

*finding the 3 customers with the highest points*

-------------






