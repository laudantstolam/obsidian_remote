>[!example] 安裝說明
>1. https://www.tenforums.com/tutorials/5558-windbg-basics-debugging-crash-dumps-windows-10-a.html
>2. SYMBOL記得安裝
>https://youtu.be/QuFJpH3My7A?t=1022



說明:
X86 DBG -> 32bit file
X64 DBG -> 64bit file


###  一些指令

- `u <位址>` 查看該位址附近的code
- `bp <位址>` 設定中斷點
	- `bp $exentry` 在程式EXE的進入口設定中斷點
	- 也可以用function設BP
- `bc <bp's index>` 清除特定的中斷點(用`*`則全刪)
- `bl` 中斷點一覽
- `k` 待執行列表
- `r` 執行序情況
- `g` 執行
- `!address` 所有記憶體位址
	- 也可以接位址查看更多資訊(佔位頭尾///)
- `lm`
	- `-a <address>` 查詢位址
	- `-m <keyword/query>` 查詢模組
- `ln` 對特定位址的符號進行查詢
- `x <addr>/<query name>` 