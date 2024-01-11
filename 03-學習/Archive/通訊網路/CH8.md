>路徑選擇

轉送-路由器再輸入/出鏈路間傳送
繞送-演算法選擇路徑

>IPv4位址

唯一NetID+HostID=32bits

>IP分類

A-E

>網路遮罩

IP跟MASK進行AND得到NET ID

>特殊IP

NETID=0 網路主機
HOSTID=0 網路本身
NET+HOST=1 廣播
127.0.0.0-127.255-255.255 迴路測試用

>NAT

交換HEADER讓多MAC共用IP
- 靜態-內部N到外部1的固定映射
- 動態-數個外部IP被動態分配
- NAPT-內部ALL到外部1的各PORT
	(只靠一相同的IP位址就可讓很多台主機互相連線)

>IP路由器

- 傳送到目的的過程
- 需要L3的能力+2個裝置介面

>IPv6

$2^{128}$組合
自動指向+IPSEC
分八段，每段16bits
- UNICAST 單節點傳輸
- MULTICAST 單隊多節點
- ANYCAST 廣播

>IPv4/v6 轉換

雙重堆疊-兩種都可用 隨資料變化
隧道-兩邊V6中間V4標頭包起來
NAT-PT-欄位相對應 純V4/V6連線

>IPSEC

在網路層對資料分組提供加密和鑒別等安全服務(認證+加密)