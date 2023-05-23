
[[雜湊函式]]

又稱雜湊演算法，是一種從任何一種資料中建立小的數字「指紋」的方法。雜湊函式把訊息或資料壓縮成摘要，使得資料量變小，將資料的格式固定下來。該函式將資料打亂混合，重新建立一個叫做雜湊值的指紋。雜湊值通常用一個短的隨機字母和數字組成的字串來代表。好的雜湊函式在輸入域中很少出現雜湊衝突。

> [SHA-256]([iT 邦幫忙::一起幫忙解決難題，拯救 IT 人的一天 (ithome.com.tw)](https://ithelp.ithome.com.tw/m/articles/10271904))

[雜湊函數簡介 (tsnien.idv.tw)](http://www.tsnien.idv.tw/Security_WebBook/chap4/4-1%20%E9%9B%9C%E6%B9%8A%E5%87%BD%E6%95%B8%E7%B0%A1%E4%BB%8B.html)

---

[[XSS 1] 從攻擊自己網站學 XSS (Cross-Site Scripting) | by Hannah Lin | Hannah Lin | Medium](https://medium.com/hannah-lin/%E5%BE%9E%E6%94%BB%E6%93%8A%E8%87%AA%E5%B7%B1%E7%B6%B2%E7%AB%99%E5%AD%B8-xss-cross-site-scripting-%E5%8E%9F%E7%90%86%E7%AF%87-fec3d1864e42)

---

SSDLC
[資安新人30 Day22 安全系統發展生命週期 SSDLC - iT 邦幫忙::一起幫忙解決難題，拯救 IT 人的一天 (ithome.com.tw)](https://ithelp.ithome.com.tw/articles/10305700)

---
### 資訊系統安全分析

-   弱點分析
    -   整個系統架構進行瞭解及測試
-   威脅分析
    -   分析系統可能遭受的安全威脅及攻擊
-   對策分析
    -   針對弱點及所面臨的安全威脅，研擬安全策略及所需的安全機制
-   風險分析
    -   評估及分析系統風險，對於部分重要資料必須採取更進一步的防護

---
### 弱點掃描

- 以自動化軟體實現，只檢測既有安全漏洞

### 滲透測試

- 以駭客的思維手法發覺安全漏洞，實戰找出突破安全防護的方式

[弱點掃描VS滲透測試，有何差別？3分鐘了解兩者差異、運作流程與常見問答 (gaia.net)](https://www.gaia.net/tc/news_detail/2/121/soc)

---
### ERROR

- 400 bad gateway
	_400_ 錯誤代碼是表明服務器不理解請求的HTTP 狀態代碼。 這些錯誤可能是由無效請求引起的，也可能是由於服務器遇到問題而未能提供您要查找的內容。

- 403 forbidden
	網站出現 _403_ Forbidden_的原因，是因為客戶端沒有存取與訪問資源的權限，但伺服器是可以正常解析與請求的，可能是因為IP被阻擋，或是被防火牆認定為不安全所以才會回傳403

- 404 not found
- 500 internal server error

[關於418的小補帖](https://blog.techbridge.cc/2019/06/15/iam-a-teapot-418/))

---

#### IaaS 基礎架構即服務
雲端伺服器 虛擬數據中心

#### SaaS 軟體即服務
管理軟體即部屬交給第三方 如google map

#### PaaS 平台即服務
可開發部屬的軟體平台

#### HaaS 硬體即服務
實體數據中心

-----
### 密碼學

經典密碼學
	經典密碼大致上分為替換式密碼和移項式密碼

- 凱薩密碼

	關鍵字:cipher
	`一般字母: a b c d e f g h i j k l m n o p q r s t u v w x y z`
	`密碼字母: c i p h e r s t u v w x y z a b d f g j k l m n o q

- 維吉尼亞密碼
- 
---
撞庫攻擊>利用在別的網站上登錄洩漏出的密碼進行第四方登入破解

---
## CVSS 

CVSS是一個開放式架構，由下列度量群組組成:
-   基本
-   時間
-   環境

### 基本

基本評分嚴重性範圍是 0-10 ，代表漏洞的固有性質。 基本評分對最終 CVSS 評分具有最大影響，且可以進一步分成下列子評分:

-   影響
    影響子評分代表成功惡意探索漏洞的機密性影響、完整性影響及可用性影響的度量值。

-   可利用性
    在 CVSS v2中，可利用性子評分代表「存取向量」、「存取複雜度」及「鑑別」的度量值。 子評分會測量如何存取漏洞、攻擊的複雜性，以及攻擊者必須鑑別以順利不當運用漏洞的次數。
  
	在 CVSS v3中，可利用性子評分代表「攻擊向量」、「攻擊複雜度」、「需要專用權」、「使用者互動」及「範圍」的度量值。 子評分會測量如何存取漏洞、攻擊的複雜性、任何必要的專用權、攻擊者與另一個使用者之間所需的互動，以及對有漏洞元件以外資源的影響。

### 時間

時間評分代表隨時間變化的漏洞威脅性質，由下列度量值組成:

-   可利用性 (CVSS v2) 或不當利用程式碼成熟度 (CVSS v3)    
    可用來利用漏洞的技術或程式碼的可用性，此漏洞會隨著時間而變更。

-   修復級別    
    可用於漏洞的補救層次。

-   報告信心度
    對脆弱性的存在及其技術細節的可信度的信任程度。


### 環境

環境評分代表受使用者環境影響的漏洞性質。 透過套用更高的環境度量值，配置下列環境度量值以強調顯示重要或重要資產的漏洞。 將最高評分套用至最重要的資產，因為與這些資產相關聯的損失對組織有更大的影響。

-   潛在抵押品損壞 (CDP) (僅限 CVSS v2 )    
    透過此資產的損壞或竊取，或生產力或收入的經濟損失，造成生命或實體資產損失的可能性。
  
-   目標分佈 (TD) (僅限 CVSS v2 )
    使用者環境中有漏洞的系統比例。
 
-   機密性需求 (CR)
    在此資產上利用漏洞時，對機密性流失的影響層次。

-   完整性需求 (IR)   
    此度量值指出在此資產上順利利用漏洞時，對失去完整性的影響層次。

-   可用性需求 (AR)
    當在此資產上順利利用漏洞時，對資產可用性的影響層次。

---

[iT 邦幫忙::一起幫忙解決難題，拯救 IT 人的一天 (ithome.com.tw)](https://ithelp.ithome.com.tw/m/articles/10272348)

---

## 防火牆(Firewall)

架設[防火牆(Firewall](http://zh.wikipedia.org/w/index.php?title=%E9%98%B2%E7%81%AB%E5%A2%99&variant=zh-tw "防火牆定義"))，就是在企業內部網路(Intranet)及網際網路(Internet)之間架設一道可監控管理的緩衝界面(Gateway), 管制所有網路封包的進出, 允許或禁止網路上特定之資料存取行為。

[防火牆(Firewall](http://zh.wikipedia.org/w/index.php?title=%E9%98%B2%E7%81%AB%E5%A2%99&variant=zh-tw "防火牆定義"))主要工作就是檢查所有通過的 IP 封包，藉由 IP 位址、Port及封包傳送方向來控制網路資訊封包傳播。 每家企業都需要根據實際網路運作需求，在網路使用便利與安全之間做取捨， 制定企業最佳網路保全政策(Security Policy)。

### Cisco 思科

Cisco是著名網路設備商，其防火牆產品從早期的 PIX 系列，至目前的 ASA 5500 系列，效能與穩定度均有一定口碑。

### Fortinet 美國防特網

Fortinet 是多層威脅防禦系統的創新者和先鋒，該系統能夠為業務通信提供最佳安全、優秀性能和低總體佔用成本。 基於Fortinet的ASIC創新和性能加速能力，FortiGate系統能即時地、不影響網路性能地從郵件和Web流量中檢測和清除具有破環性的內容威脅，如 病毒/蠕蟲、入侵、不合適的Web內容等。 FortiGate 號稱是當前業界整合最多安全防護功能的資安產品，包括提供防火牆(Firewall)、虛擬私人網路(VPN)、 防病毒、入侵防禦(IPS), Web內容、反垃圾郵件、反間諜件和流量管理等功能。這些功能既可以單獨開啟應用，也可以作為統一威脅管理系統(UTM)之解決方案綜合應用。

### Palo Alto Networks

傳統防火牆的技術仰賴連接埠(port)、通訊協定(protocol)進行通訊流的分類，導致精心設計的應用程式及技術高超的使用者可以輕鬆地規避它們，例如：在連接埠間轉換、使用SSL、暗中跨過連接埠80，或使用通常會保持開啟的非標準連接埠。Palo Alto Networks 推出新一代防火牆系列產品，回復原屬於防火牆應該具備的高效能，以及以政策為基礎，對應用程式、使用者與通訊內容的可視性和控制能力。

詳細資訊可參閱 新世代AP防火牆 - 單通道平行處理架構

### 自由軟體防火牆

如果預算經費有限，或想更有彈性的架構防火牆，可考慮導入Linux [IPTables Firewall](http://zh.wikipedia.org/w/index.php?title=Iptables&variant=zh-tw "IPTables Firewall定義")。[IPTables](http://zh.wikipedia.org/w/index.php?title=Iptables&variant=zh-tw "IPTables定義") 是一套 自由軟體[防火牆](http://zh.wikipedia.org/w/index.php?title=%E9%98%B2%E7%81%AB%E5%A2%99&variant=zh-tw "防火牆定義")，只要一台 1U 的主機，安裝 Linux OS，建置 [IPTables](http://zh.wikipedia.org/w/index.php?title=Iptables&variant=zh-tw "IPTables定義") 即可有一台效能與穩定度防火牆設備為您的企業網路安全把關。

需要技術服務？ [IPRO 網際家](https://www.ipro.tw/about_us.html)可提供專業安裝建置服務，請洽詢 sales@ipro.tw

## 入侵偵測(IDS)、入侵防護(IPS)

入侵偵測(IDS)系統主要功能在負責監聽網路封包，依據預先設定的安全策略(Security Policy)，對網路與系統的運行狀況進行監測，當發現異常，自動發出警訊通報給網管人員，記錄各種攻擊企圖、攻擊行為或者攻擊結果。入侵防護(IPS)系統則化被動為主動，當發現網路異常封包或行為時，系統除發送警訊通報給網管人員，並立即採取必要的處置措施，例如阻斷來源IP。

### TippingPoint IPS

TippingPoint IPS獲得NSS Gold金牌獎、multi-gigabit ICSA Labs認證以及其他多項業界獎賞，成為網路入侵防護方案的確切標竿。

TippingPoint 認為要發揮 IPS 的全部功能，第一步便是要將 IPS 安裝為「In-band」模式」，也就是安裝於企業網路的主要幹道上。如此才能夠真正即時阻斷惡意流量保護企業網路安全。

TippingPoint開發領先業界的網路入侵預防系統(Intrusion Prevention Systems; IPS)，提供無人能及的安全性、效能、高可用性和簡易使用性。

---

## Jenkins 是什麼？

持續整合、持續交付 (CI/CD) 的觀念在近幾年來越來越被開發人員所重視。透過 CI/CD 概念的實踐，我們可以針對每一次產品的修改，或是週期性地對產品進行各種單元 (unit testing) 或整合測試 (integration testing)。若產品發生狀況，我們可以藉此在第一時間內找出發生問題的最接近位置。同時，我們也可以透過持續整合的工具替我們建置 (build) 服務，並在建置完成後產生報表分析或做自動通知等其他的動作。

---
### 資安三大目標

（一）機密性：適當保護資訊資產，讓資訊資產均為合法使用。
（二）完整性：維持資訊資產內容的正確與完整。
（三）可用性：確保資訊資產能隨時提供使用

***
### 驗證因子
-   知識因子（Knowledge Factor）：代表您所知道的內容，例如密碼。
-   擁有因子（Possession Factor）：代表您所擁有的東西，例如身分證、信用卡、電話等。
-   生物辨識因子（Inherence Factor）：能代表您的生物特徵，例如指紋、虹膜、臉部辨識等。
- ---
### 攻擊行為

##### 緩衝區溢位（buffer overflow）
向程式輸入緩衝區寫入使之溢位的內容（通常是超過緩衝區能儲存的最大數據量的資料），從而破壞程式執行、趁著中斷之際並取得程式乃至系統的控制權

[[Day23] 攻擊行為－緩衝區溢位 Buffer Overflow - iT 邦幫忙::一起幫忙解決難題，拯救 IT 人的一天 (ithome.com.tw)](https://ithelp.ithome.com.tw/articles/10188599)

##### 跨網站指令碼（Cross-site scripting，XSS）
是一種網站應用程式的安全漏洞攻擊，是代碼注入的一種。 它允許惡意使用者將程式碼注入到網頁上，其他使用者在觀看網頁時就會受到影響。 這類攻擊通常包含了HTML以及使用者端手稿語言。

---
![image.png](https://raw.githubusercontent.com/laudantstolam/imagesource/main/ctf1.png)
---
[RAID 磁碟陣列是什麼？一篇文章就理解（2022年最新） - 凌威科技 (linwei.com.tw)](https://www.linwei.com.tw/forum-detail/45/)

---





$ \displaystyle\sum_{ i =  1  }^{ n  } \left( \right) $


