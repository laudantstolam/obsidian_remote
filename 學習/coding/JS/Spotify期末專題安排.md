## 教學

>Oauth+backend

[Spotify OAuth- Full Tutorial](https://www.youtube.com/watch?v=mBycigbJQzA)
[Demo Code](https://github.com/katiagilligan888/Spotify-Discover-Weekly/blob/main/discoverWeekly.py)

>Front end

[next.js tutorial](https://www.youtube.com/watch?v=qwhMyVVnmKM&t=2765s)

---
> 框架: 後端(Flask)+前端(nextjs)

## 已完成
- [x] 後端測試-自動連接一個API
- [x] 前端框架架設

## 待完成
- [ ] 把後端資料丟到json裡面再讓前端存取?
- [ ] 前端硬幹
- [ ] A+C區域
- [ ] B區域
- [ ] D區域
- [ ] E區域
- [ ] F區域

---
## API及數據整理

![[概念設計圖]]
>A 區域

https://developer.spotify.com/documentation/web-api/reference/get-users-top-artists-and-tracks
`https://api.spotify.com/v1/me/top/artists?time_range=medium_term` 
`https://api.spotify.com/v1/me/top/tracks?time_range=medium_term
`
共50
拿到最近50歌手的種類>>統計>>輸出
// 拿到最近50歌曲比對最近50歌手 看集中度

> B 區域

https://developer.spotify.com/documentation/web-api/reference/get-followed
`https://api.spotify.com/v1/me/following?type=artist`

拿到關注名單(記得翻頁)>>盤點重複歌手+獲取各自歌手popu程度

> C 區域

https://developer.spotify.com/documentation/web-api/reference/get-users-top-artists-and-tracks
跟A一樣 但是是短期的
`https://api.spotify.com/v1/me/top/artists?time_range=short_term&limit=3

拿到3個照片+名字>>輸出

> D 區域

