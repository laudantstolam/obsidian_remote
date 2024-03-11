| MAC   | IP    |
| ----- | ----- |
| L2    | L3    |
| ONLY  | MULTY |
| 32bit | 24bit |

>ARP用途

解析IP位址或是主機名稱所對應的MAC
$IP\rightarrow MAC$

>ARP傳輸步驟

1. 生成ARP快取對應表
2. 傳輸檢查對應(有就傳 沒有就廣播)
3. 檢查並回復
4. 收到登記傳輸

>ARP cache

- 靜態-手動添加
- 動態-自動添加
>RARP

已知MAC不知IP可以發個封包了解一下自己

>ICMP

ICMP-回報IP路由問題
TCP-解決問題
| IP標頭 | ICMP標頭8bit | 資料

訊息類型
- 查詢 8/0 10/19 13/14 req/reply
- 錯誤回報 3 4 5 11 12
