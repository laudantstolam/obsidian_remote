>[!example]+ tutorials
>https://www.youtube.com/playlist?list=PLW8bTPfXNGdC5Co0VnBK1yVzAwSSphzpJ

- `TCP Segment len` 可以看到乘載的byte數量而不僅是長度

---
### Dumpcap

- `dumpcap -D` 目前的區域連線(出現亂碼是因為那是區域連線) 
![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202310021536354.png)

- `dumpcap -i 6 -w /users/rache/Desktop/wireshark/test.pcapng -b filesize:500000 -b files:10` 
	- `-i 6` 擷取六號連線(wifi)的封包
	- `-w /users/rache/Desktop/wireshark/test.pcapng` 存檔到wireshark資料夾直到暫停擷取
	- `-b filesize:500000 -b files:10` ringbuffer每500000KB一包，一共10包
---
### Filter
- 篩選連線
![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202310040835407.png)
- 篩選細部
![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202310040839853.png)
	- ip
	- ip.addr = 192.168.0.23
- 新增條件
	- 右鍵>converesation filter>指定想要看到的ip/tcp/...通訊包，會自動幫忙filter![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202310040843994.png)
	- 也可以在封包底下資訊選擇![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202310040847741.png)
- 排除條件
	- 範例(filter command)
	- `not (ssl or ipv4 or TCP) 排除這三種通訊方式`
	- `tcp.port in {80 1443 8080} 找到TCP在80/1443/8080三個端口的通訊紀錄`
	- `frame contains google` 大小寫敏感搜尋str
	- `frame matches google` 不敏感搜尋str

### Setting
![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202310042055657.png)
- 為自訂IP命名: 右鍵>`edit resloved name`>命名
	- 檢視所有命名與原IP對照: `statistics/reesloved addresses`
- 改變時間顯示方式![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202310051732449.png)
- 計時:`右鍵>set/unset time reference`設定0點
- 展開到主畫面中![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202310051750941.png)
#### Statistics
- `statistics>conversation`