## 教學

>Oauth+backend

[Spotify OAuth- Full Tutorial](https://www.youtube.com/watch?v=mBycigbJQzA)
[Demo Code](https://github.com/katiagilligan888/Spotify-Discover-Weekly/blob/main/discoverWeekly.py)

>Front end

[next.js tutorial](https://www.youtube.com/watch?v=qwhMyVVnmKM&t=2765s)
[How To Use The Spotify API In Your React JS App (youtube.com)](https://www.youtube.com/watch?v=wBq3HCvYfUg)

---
> 框架: 後端(Flask)+前端(nextjs)

## 已完成
- [x] 後端測試-自動連接一個API
- [x] 前端框架架設

## 待完成
- [ ] 把後端資料丟到json裡面再讓前端存取?
- [ ] 前端硬幹 煩鼠
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
~~拿到最近50歌曲比對最近50歌手 看集中度~~

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

https://developer.spotify.com/documentation/web-api/reference/get-several-audio-features

一次可以全部丟進去 讚

提取 `instrumentalness` `energy` `speechiness` `valence` `tempo` `danceability` 六個參數>>比對最接近的三個組合成句子 >> 顯示在雷達圖上

句子邏輯: normalize之後>> `你們都喜愛著**性和**性強、富含**的歌曲類型`

> E 區域

https://developer.spotify.com/documentation/web-api/reference/get-the-users-currently-playing-track

拿到正在撥放曲目+照片

> F 區域

https://developer.spotify.com/documentation/web-api/reference/get-recommendations

`https://api.spotify.com/v1/recommendations?seed_artists=4NHQUGzhtTLFvgF5SZesLK&seed_genres=classical%2Ccountry&seed_tracks=0c6xIDDpzE81m2q797ordA

把D區拿到的共同音樂特徵平均丟進去(ALL)上下界線+A區共同種類+(如果有重複歌手的話)>>拿到推薦歌單(拜託10首就好 預設limit10 其中找到有url的在顯示 抱歉我真的無法了)>>預覽顯示(照片+會附贈mp3連結)

如果有時間的話再變成Iframe 或是直接把推薦割去推到歌單裡面生成iframe
(需要控制用戶權限 有點煩)