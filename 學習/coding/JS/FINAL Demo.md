### 基本架構
- 個人向
- 分析
- 有趣
- 會讓人想重複使用
(不知道能不能第三方authenticate 或是變成一個url讓大家試試)

### 根據API
1. 排名追蹤的藝人的Popularity
1. genres
2. 收聽歷史
3. 

### 延伸發想
1. 歌單對比
2. 光譜對照-相似程度(基於追蹤的藝人的genre) 用色譜表示 或是彩虹一樣的雨落下 呈現不一樣的顏色做出區別
3. 重複(追蹤藝人重疊程度) 用
4. 選一手你們的代表歌吧[Web API Reference | Spotify for Developers](https://developer.spotify.com/documentation/web-api/reference/get-audio-features)
用分析API分析一些東西
1. 或是針對最近聽的100首歌進行細部分析看得出一些Key的分布/能量分布/類型分類之類的東西

```json
{  
"acousticness": 0.0881,  >>原聲程度
"analysis_url": "https://api.spotify.com/v1/audio-analysis/63mdJr3NMY3wReOkNE6c6W",  
"danceability": 0.695,  >>舞曲性
"duration_ms": 194900,  
"energy": 0.62,  
"id": "63mdJr3NMY3wReOkNE6c6W",  
"instrumentalness": 0.0000543,  >>純音樂性比例
"key": 8,             >>高低頻率
"liveness": 0.111,    >>現場程度
"loudness": -8.082,  
"mode": 0,           (大小調)
"speechiness": 0.0521,  >>含文字量。可製作lyrical喜愛程度
"tempo": 150.032,        >>節奏快慢
"time_signature": 4,  (拍數)
"track_href": "https://api.spotify.com/v1/tracks/63mdJr3NMY3wReOkNE6c6W",  "type": "audio_features",  
"uri": "spotify:track:63mdJr3NMY3wReOkNE6c6W",  
"valence": 0.62       >>情緒樣態
}
```
找相似程度最高的3個數值(需要制定一套相近辦法)
不太需要一個general的標準 因為只是兩人對比

- rap's instrumentalness was LOW
- acousticness sometimes also
- 