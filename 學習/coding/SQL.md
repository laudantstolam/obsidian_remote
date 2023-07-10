>  [Learn SQL In 60 Minutes - YouTube](https://www.youtube.com/watch?v=p3qvj9hO_Bo)
>  [WebDevSimplified/Learn-SQL: Exercises for beginners to learn SQL (github.com)](https://github.com/WebDevSimplified/Learn-SQL)
>  
>  [【資料庫】SQL 3小時初學者教學  - YouTube](https://www.youtube.com/watch?v=gvRXjsrpCHw)
>  [hibyby/GrandmaCan_sql_tutorial (github.com)](https://github.com/hibyby/GrandmaCan_sql_tutorial)
>  

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
</br>
- 語法問題
	 1. `(*)` 跟 `*` 意思一樣 都是選擇全部
	 2. 變數外面加上反括號![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202307110022900.png)
</br>
- 其他