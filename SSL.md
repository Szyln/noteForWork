# SSL
> 安全通訊協定（英語：Secure Sockets Layer，縮寫：SSL）

包含
- 記錄層（Record Layer）
- [傳輸層](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E5%B1%82 "傳輸層")

## SSL 在紀錄層
- 記錄層協定確定傳輸層資料的封裝格式。
## SSL 在傳輸層

>[數位信封 Digital Envelop](演算法/數位信封%20Digital%20Envelop.md)


- 傳輸層安全協定使用[X.509](https://zh.wikipedia.org/wiki/X.509 "X.509")認證
- 之後利用非對稱加密演算（[非對稱金鑰 Asymmetric](演算法/非對稱金鑰%20Asymmetric.md)）來對通訊方做身分認證
- 之後交換[對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md) 作為會談金鑰（[Session key](https://zh.wikipedia.org/wiki/Session_key "Session key")）
- 這個會談金鑰是用來將通訊兩方交換的資料做加密，保證兩個應用間通訊的 [機密性 Confidentiality](演算法/機密性%20Confidentiality.md) 和 [可靠性 Reliability](演算法/可靠性%20Reliability.md)，使客戶與伺服器應用之間的通訊不被攻擊者竊聽。