### Result Preview

![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202402191546709.png)

### Intro

Inspired by several Spotify expanded third-party project that expand into visualizing various listening data in well-designed interfaces, but limited to the analysis of personal data. Consequently, I decided to develop a project based on the concept of "making friends through music" to compare the data of two individuals. By analyzing personal listening habits, trending artists, and song attributes, we could present several types of data analysis.

本次專題是鑒於平時經常使用Spotify收聽音樂以及對於將自己的收聽資料視覺化十分感興趣，因此選擇Spotify API結合網頁前端設計來實作出不一 樣的資料視覺呈現。 網路上有許多Spotify衍伸第三方數據可視化的先例，但都僅限個人資料的呈現，因此本次想透過雙人資料的比對，以”以樂會友”的概念發想進行設計，圍繞兩個人的收聽習慣、追蹤藝人、歌曲特色進行數據處理與呈現

### Framework and Workflow

![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202402191546086.png)

### Data Processing Detail

#### 1. Music Genere 近期收聽種類

![image.png|213](https://raw.githubusercontent.com/Ash0645/image_remote/main/202402191549525.png)
##### APIs
- `Get User's Top Items`
- `https://api.spotify.com/v1/me/top/artists?time_range=medium_term` 
- `https://api.spotify.com/v1/me/top/tracks?time_range=medium_term`
##### PROCESS
1. get user's top 50 trend artist's genere 
2. calculate the top generes
3. return and 