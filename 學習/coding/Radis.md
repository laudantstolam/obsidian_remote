>[!note] VIDEO LINK
>[(88) 我是Redis，MySQL大哥被我坑惨了！ - YouTube](https://www.youtube.com/watch?v=D16efi0TDIs)

>簡介

幫mySQL減低重複I/O請求的暫存區

>清理緩存

(由應用程式定義)
![image.png|400](https://raw.githubusercontent.com/Ash0645/image_remote/main/202308221926698.png)

>問題 緩存穿透

不存在資料的無效請求無法被擋下，勞模MYSQL
解決:使用布爾過濾器

>問題 剛刪掉又收到一堆請求

解決: 熱點數據永不刪除+應用程式刪除時間隨機化(過期時間均勻分布)

#專業術語 緩存擊穿 緩存雪崩

---
>Radis 進程崩潰 緩存全沒

