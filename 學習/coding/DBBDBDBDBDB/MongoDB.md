#### 安裝步驟
1. 下載本體
2. 下載shell

#### 安裝備註
shell 的位置在
` C:\Users\rache\Downloads\mongosh-1.10.6-win32-x64\mongosh-1.10.6-win32-x64\bin`
已新增至系統變數

#### 教學連結
https://www.youtube.com/playlist?list=PL4cUxeGkcC9h77dJ-QJlwGlZlTd4ecZOA

---
## <font color="#4f81bd">基本知識</font>

#### 資料儲存方式

- <font color="#4f81bd">BSON</font> - binary JSON
>[!example]+ 
>![image.png|525](https://raw.githubusercontent.com/Ash0645/image_remote/main/202309070227799.png)
>一個文件就是一個collection，故DB Blog Posts裡面有9個 collection


#### Shell 指令

- `mongosh` 在CMD開啟mongo shell
- `cls` 清除
- `exit` 離開
- `show dbs` 顯示所有DB
- `it` 繼續顯示
- `show collection` 顯示該DB下的所有collection
- `use (DB_name)` 進入該DB的操作區
// 該DB可以是不存在的 一但新增資料 芒果會幫你自動新建DB
*看吧 芒果還是對你很好的*

###### <font color="#8db3e2">C</font>

- `db.(collection_name).insertOne()` 插入一筆資料
- `db.(collection_name).insertMany()` 插入多筆資料
collection_name可以是不存在的

###### <font color="#8db3e2">R</font>

- `db.(collection_name).find({(target_key): (target_value)})` 搜尋
- `db.books.findOne({(target_key): (target_value)})` 單一特定搜尋
>[!example]+ 限定顯示
>![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202309082314388.png)
> 第一個{}中篩選條件
> 第二個{}中選擇要顯示的`target_key` 

- `db.books.find().count()` 顯示collection
- `db.books.find().limit(N)` 限定顯示N筆資料

- `db.books.find().sort({(target_key): 1/-1})` 1>>A-Z，-1>>Z-A
	- `1` A-Z 升冪排列
	- `-1` Z-A 降冪排列
- `db.books.find({(target_key): {$lt: N}})` 限定範圍
	- `$lt` <
	- `$gt`>
	- `lte` <=

- `db.books.find({$or: [{(target_key1)): (target_value1)},{(target_key2)): (target_value2)}]})` OR條件
>[!example]+  "$" 複合條件
>![image.png|525](https://raw.githubusercontent.com/Ash0645/image_remote/main/202309090031432.png)
> 應用範例: 在OR裡面串入多個{}條件進行篩選
> ```
> db.books.find({$or: [{},{},{}......]})

- `db.books.find({(target_key): {$in/$nin: [N, M, K]}})` 多條件篩選
	- `N/M/K` 為 target_value1/2/3
	- `$in` 搜尋在`[]`條件內的
	- `$nin` 搜尋不在`[]`條件內的
- `db.books.find({(target_key)): [(target_value)]})` 尋找矩陣中的唯一值
	- 一般搜尋可用之前最簡易的方式，此方法找到的`target_value`會是那個key的唯一值
- `db.books.find({(target_key): {$all: [(target_value1), (target_value2)]}})` 找矩陣中包含的多個值
	- 該結果的`key`裡面一定會有`target1/2`
- `db.books2.find({(target_name).(target_key): (target_value)})` 多層搜尋
>[!example]+ 多層搜尋範例
>![image.png|375](https://raw.githubusercontent.com/Ash0645/image_remote/main/202309111556920.png)

###### <font color="#8db3e2">U</font>

###### <font color="#8db3e2">D</font>
- 