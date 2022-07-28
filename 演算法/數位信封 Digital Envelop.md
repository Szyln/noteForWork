# 數位信封 Digital Envelop
> [Day22 資料傳輸安全(機密性) RSA x AES 混搭風(上)](https://ithelp.ithome.com.tw/articles/10188528)

>[Asymmetric Encryption Schemes](演算法/Asymmetric%20Encryption%20Schemes.md)好像有點像？


## 混搭
- [非對稱金鑰 Asymmetric](演算法/非對稱金鑰%20Asymmetric.md)：[RSA](演算法/RSA.md)
- [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md)：[AES](演算法/AES.md) （也有搭配 [DES (DEA, Data Encryption Algorithm)](演算法/DES%20(DEA,%20Data%20Encryption%20Algorithm).md), [2TDEA](演算法/2TDEA.md), 3DES 等）

## 步驟
![](http://ithelp.ithome.com.tw/upload/images/20170106/20103434cTJ19UZgTu.jpg)
![](http://ithelp.ithome.com.tw/upload/images/20170106/20103434tEe0Y1MwCN.jpg)

>圖片來源：[Day22 資料傳輸安全(機密性) RSA x AES 混搭風(上)](https://ithelp.ithome.com.tw/articles/10188528)
- [非對稱金鑰 Asymmetric](演算法/非對稱金鑰%20Asymmetric.md) 公開金鑰加密 Session Key 
- Session Key 是 [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md) ，用來加解密會議內容


### 商家發送資料給銀行

- 銀行（接收解密）
	- [RSA](演算法/RSA.md) [非對稱金鑰 Asymmetric](演算法/非對稱金鑰%20Asymmetric.md) 定期生成
		- 生成公開金鑰（商家加密 Session Key）
		- 生成私密金鑰（銀行解密 Session Key）
	- 使用 Session Key （商家生成）解密資料內容
- 商家（傳送加密）
	- 生成 Session Key
		- [AES](演算法/AES.md) [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md) 
		- 加密資料內容
	- 使用公開金鑰加密 Session Key
	- 使用 Session Key 加密資料內容
- 
### 銀行發送請款資料給商家
- 商家（接收解密）
	- [RSA](演算法/RSA.md) [非對稱金鑰 Asymmetric](演算法/非對稱金鑰%20Asymmetric.md) 定期生成
		- 生成公開金鑰（銀行加密 Session Key）
		- 生成私密金鑰（商家解密 Session Key）
	- 使用 Session Key （銀行生成）解密資料內容
- 銀行（傳送加密）
	- 生成 Session Key
		- [AES](演算法/AES.md) [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md) 
		- 加密資料內容
	- 使用公開金鑰加密 Session Key
	- 使用 Session Key 加密資料內容