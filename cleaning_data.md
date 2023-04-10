What issues will you address by cleaning the data?
the data was too messy i faced many issues with data.
when i deleted duplicate data from there i deleted my all data then i added tables and data again
when i divided value of unit price is not working because of data type after that i changed it
i faced many issues with data types





Queries:
Below, provide the SQL queries you used to clean your data.
remove all duplicate data and try make all data unique

CREATE TABLE new_all_sessions AS
SELECT DISTINCT* FROM all_sessions;

DROP TABLE all_sessions;

ALTER TABLE new_all_sessions RENAME TO all_sessions;

for unit price
UPDATE analytics 
SET unit_price = unit_price /100000


