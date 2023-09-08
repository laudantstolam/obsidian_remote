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
- `db.(collection_name).findOne({(target_key): (target_value)})` 單一特定搜尋
- `it` 繼續顯示

>[!example]+ 限定顯示
>![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202309082314388.png)
> 第一個{}中篩選條件
> 第二個{}中選擇要顯示的`target_key` 

- `db.books.find().count()` 顯示collection裡面的資料總數





