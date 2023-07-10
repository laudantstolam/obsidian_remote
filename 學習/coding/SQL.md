>  [(28) Learn SQL In 60 Minutes - YouTube](https://www.youtube.com/watch?v=p3qvj9hO_Bo)

---
Notes:

- NULL
	1. 用 IS NULL/ IS NOT NULL 判斷
	<font color="#c0504d">不能用</font>  `= NULL` 或是`!= NULL`因為 NULL 不會等於自己
	1. mySQL 中也支援 <=>
	```
	SELECT * FROM table WHERE column <=> NULL;
	```
- HAVING 跟 WHERE
	 在顯示特定條件時通常都用 WHERE
	 但是在進行 GROUP BY 操作後需要用 HAVING 來處理

- 語法問題
	 