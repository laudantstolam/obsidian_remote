
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
