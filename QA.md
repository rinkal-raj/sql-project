What are your risk areas? Identify and describe them.
Risk areas are:
when i tried to delete duplicate and null values i deleted my all data from table.


QA Process:
Describe your QA process and include the SQL queries used to execute it.
First i removed all messy and duplicate data from all tables.
Here the query of one table i removed duplicate data.
```CREATE TABLE new_all_sessions AS
SELECT DISTINCT* FROM all_sessions;

DROP TABLE all_sessions;

ALTER TABLE new_all_sessions RENAME TO all_sessions;
```
CREATE TABLE new_analytics AS
SELECT DISTINCT* FROM analytics;

DROP TABLE analytics;

ALTER TABLE new_analytics RENAME TO analytics;


i wrote query in proper way which saw in QA process and  also i gave proper name to allises.

i tried to write code proper way which included in QA process.
made code more precise.