### 實體層(最下層)
物理連接(傳送0/1)
集線器(多hub的中繼器)/主機介面/USB/硬碟/中繼器(加強訊號用)
### 資料鏈結層
同網路之間，將資料裝進訊框傳送
MAC位址(每張網卡不一樣)
<font color="#e36c09">00:00:00</font>:<font color="#548dd4">00:00:00</font>
<font color="#e36c09">廠商代碼</font>+<font color="#548dd4">廠商設定的裝置碼</font>
Hub/橋接器(網路分割用，==廣播風暴==)/MAC/網路卡/交換器(多hub橋接器)
### 網路層
不同網路間，用加上IP後封包進行傳輸
IP是邏輯位置(by OS)
MAC是網卡實體位置
網際網路/IP/L3 switch(交換器)
### 傳輸層
把實體、鏈結、網路層和之後的層用port溝通串接
使用TCP/UTP
1. 切段後加上編號方便重組
2. 控制流量
3. 區段編號檢查資料完整性
TCP/IP
### 會議層
建立網路連線和檢查點並維護連線
帳密
### 表達層/展示層
轉譯(編碼轉換)、加密、壓縮(壓縮應用層傳到會議層)
### 應用層(最上層)
利用通訊協定進行資訊操作與整合
HTTP

---


![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202311021431999.png)

### port
~1023 預設服務/政府/必要通訊
1024~49151 半保留
49151~65535 client port

- socket pair
	client的IP/PORT
	serverr的IP/port
	一共四個連線建立

