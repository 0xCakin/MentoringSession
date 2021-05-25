
## Query examples
```
SELECT account_id, MAX(standard_qty)
FROM orders
WHERE total_amt_usd > 500
GROUP BY account_id;
```
SELECT *
FROM orders
GROUP BY account_id;

SELECT  account_id,
		MAX(occurred_at),
		MIN(standard_qty),
        SUM(gloss_qty)
FROM orders
GROUP BY account_id;


SELECT 	account_id,
		DATE_PART('year', occurred_at) as Year,
        DATE_PART('month', occurred_at) as month,
        occurred_at
FROM orders
limit 100;

## DBMS VS Database
https://www.geeksforgeeks.org/difference-between-database-and-dbms/

## Resume Website
https://www.canva.com/

## Git/GitHUB
- Version Controling with git: https://www.udacity.com/course/version-control-with-git--ud123
- How to write Readme/Markdown language: https://www.udacity.com/course/writing-readmes--ud777
- Markdown Language Cheatsheet: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
