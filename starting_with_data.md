Question 1: find all duplicate records

SQL Queries: SELECT * FROM TABLE_NAME

Answer: ALL ROWS AND COLUMS DATA FOUND



Question 2: find the total number of unique visitors (`fullVisitorID`)

SQL Queries:
SELECT COUNT(DISTINCT (fullvisitorid))
						   FROM analytics 

Answer: 120018



Question 3: find the total number of unique visitors by referring sites

SQL Queries:SELECT COUNT(DISTINCT visitid)
FROM all_sessions
WHERE channelGrouping = 'Referral'



Answer:2488



Question 4: find each unique product viewed by each visitor

SQL Queries:SELECT DISTINCT ON (sku)sku,s.visitid,p.name
           FROM products AS p
         INNER JOIN all_sessions AS s
		 ON p.sku = s.productsku
		 ORDER BY p.sku;
       
Answer:![alt desc](img/que-4.png)
        total rows:389



Question 5: 

SQL Queries:

Answer:
