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
- `(some_filter_or_action).explain("executionState")` 顯示詳細資料調動過程
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
- `db.books.updateOne({(filter_key): (filter_value)}, {$set: {(target_key): (target_value_changed)}})` 更新一筆資料
	- 通常一筆的情況`filter_key` 會使用`ObjectId` 進行篩選
- `db.books.updateMany({(filter_key): (filter_value)}, {$set: {(target_key): (target_value_changed)}})` 更新多筆資料

- `db.books.updateMany({(filter_key): (filter_value)}, {$inc: {(target_key): +/-N}})` 把數值增減N
- `db.books.updateMany({(filter_key): (filter_value)}, {$push/$pull: {(target_key): (target_value)}})` 增/減矩陣中的值
	- `(target_value)`改成`$each: [(val_1), (val_2)]`可以新增多個值
	- 舉例`db.books.updateOne({_id: ObjectId("64f9fd37db3e39addbcb7598")}, {$push: {genres: {$each: ["1", "2"]}}})`
- 

###### <font color="#8db3e2">D</font>
- `db.books2.deleteOne({(target_key): (target_value)})` 刪除一筆document
- `db.books2.deleteMany({(target_key): (target_value)})`  刪除多筆document

###### <font color="#8db3e2">Index</font>
- `db.books.createIndex({(target_key): (target_value)})` 建立搜尋索引
- `db.books.showIndex()` 顯示所有索引
	- 會有一個預設排列 `_id` 的索引
- `db.books.dropIndex({(target_key): (target_value)})` 刪除索引


---
## <font color="#4f81bd">MongoServer</font>

#### 啟動並監聽

1. `npm init` 初始化
2. install packages
	1. `npm install express`
	2. `npm install mongodb`
	3. `npm install (-g) nodemon`
3. 新增一個 `(file_name).js`
```
const express = require('express')

// init app + middleware
const app = express()
app.listen(3000, () => {
    console.log("LISTENING at 3000")
})

// routes
app.get('/books', (req, res)=>{
    res.json({mssg: "welcome to the api"})
})
```
4. `nodemon (file_name)`
5. 打開localhost 3000/books就會看到mssg 內容





#### 範例程式內容列表
- 基本CRUD方法
- 翻頁方法
- 防呆方法

---
- `db.js` 處理跟mongoDB的連線問題
```javascript
// db.js
const { MongoClient } = require('mongodb')
let dbConnection
module.exports={
    connectToDb: (cb) => {
        MongoClient.connect('mongodb://127.0.0.1:27017/bookstore')
        .then((client)=>{
            dbConnection = client.db()
            return cb()
        })
        .catch(err => {
            console.log(err)
            return cb(err)
        })
    },
    getDb: () => dbConnection
}
```

> memo

`mongodb://127.0.0.1:27017/bookstore` 需要注意是IPV4/IPV6 這邊用的是IPV6寫法

---
- `app.js` 處理資料庫操作+CRUD
```javascript
// app.js
const express = require('express')
const { connectToDb, getDb } = require('./db')
const { ObjectId } = require('mongodb')

// init app + middleware
const app = express()
app.use(express.json())

// db connection
let db

connectToDb((err)=>{
    if(!err){
        app.listen(3000, () => {
            console.log("LISTENING to 3000")
        })
        db = getDb()
    }
})

// routes

/// fetch all datas
app.get('/books', (req, res)=>{
//params passed in
    const page = req.query.page || 0
    const booksPerPages = 2
    
    let books = []

    db.collection('books')
    .find() // find documents in the collection 'books'
    .sort({author: 1})
    .skip(page * booksPerPages)
    .limit(booksPerPages)
    .forEach(book => books.push(book))
    //`then` after all the aboves are done
    .then(() => {
        res.status(200).json(books)
    })
    .catch(() => {
        res.status(500).json({error: "Could not fetch documents QQ"})
    })
})

/// fetch single document
app.get('/books/:id', (req, res)=>{
    if(ObjectId.isValid(req.params.id)){
        console.log(`GET /books/${req.params.id}`)
            db.collection('books')
            .findOne({'_id': new ObjectId(req.params.id)})
            .then(doc=>{
                res.status(200).json(doc)
            })
            .catch(err=>{
                res.status(500).json({error: "Could not fetch documents QQ"})
            })
    }
    else{
        res.status(400).json({"message": `Invalid id ${req.params.id}`});
    }
})

/// Create a document
app.post('/books', (req, res) =>{
    const book = req.body
    db.collection('books')
    .insertOne(book)//insert request body
    .then(result => {
        res.status(201).json(result)
    })
    .catch(err =>{
        res.status(500).json({err: 'could not create a new doc'})
    })
})

/// Delete single document
app.delete('/books/:id', (req, res) =>{
    if(ObjectId.isValid(req.params.id)){
        console.log(`DEL /books/${req.params.id}`)
            db.collection('books')
            .deleteOne({'_id': new ObjectId(req.params.id)})
            .then(result => {
                res.status(200).json(result)
            })
            .catch(err => {
                res.status(500).json({error: "delete fail"})
            })
    }
    else{
        res.sendStatus(400).json({"message": `Invalid id ${req.params.id}`});
    }
})

/// Update single document
app.patch('/books/:id', (req,res) => {
    const updates = req.body
 
    if(ObjectId.isValid(req.params.id)){
        console.log(`UPDATE /books/${req.params.id}`)
            db.collection('books')
            .updateOne({'_id': new ObjectId(req.params.id)}, {$set: updates})
            .then(result => {
                res.status(200).json(result)
            })
            .catch(err => {
                res.status(500).json({error: "update fail"})
            })
    }
    else{
        res.status(400).json({error: `Invalid id ${req.params.id}`})
    }
})
```
