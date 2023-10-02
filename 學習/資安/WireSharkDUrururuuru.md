- `TCP Segment len` 可以看到乘載的byte數量而不僅是長度

---
### Dumpcap

- `dumpcap -D` 目前的區域連線(出現亂碼是因為那是區域連線) 
![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202310021536354.png)

- `dumpcap -i 6 -w /users/rache/Desktop/wireshark/test.pcapng -b filesize:500000 -b files:10` 
	- `-i 6` 擷取六號連線(wifi)的封包
	- `-w /users/rache/Desktop/wireshark/test.pcapng` 存檔到wireshark資料夾直到暫停擷取
	- `-b filesize:500000 -b files:10` ringbuffer每500000KB一包，一共10包
- 