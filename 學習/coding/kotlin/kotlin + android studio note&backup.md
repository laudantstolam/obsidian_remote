[[代辦事項#^5q4ozf]]
- 相關截圖
	- SDK版本和兼容性知識 https://www.bilibili.com/video/BV11Q4y1D7rg?t=209.4&p=3


#### 定義

val=read only
var=read+write

gradle 檔案
- build.gradle>>應用到ALL
- setting.gradle>>需要被IMPORT的套件包

setContentView(R.layout.activity_main)
- R:設置每一個資源文件類別分配一個索引
- 可以透過R.類別名/資源名去操作對應資源

res/layout裡面放布局文件 檔名需小寫

流程(會自動完成)
1. 創建activity(頁面)
2. 指定layout
3. 把activity配置在manifets/manifets中
