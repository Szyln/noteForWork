# RSA
- [非對稱金鑰 Asymmetric](演算法/非對稱金鑰%20Asymmetric.md)
- 廣泛運用在商業中
- RSA以三個發明人姓氏首字母縮寫組合成
	- 麻省理工教授Ron Rivest
	- 以色列密碼學家Adi Shamir
	- 南加大教授Leonard Adleman
- 多用於 [數位信封 Digital Envelop](演算法/數位信封%20Digital%20Envelop.md)，加密[對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md)

![](http://ithelp.ithome.com.tw/upload/images/20170111/201034346zInPKC8sK.png)

>圖片來源：[Day27 非對稱金鑰加密系統(RSA)](https://ithelp.ithome.com.tw/articles/10188824)

## 長度
>~~2009年12月12日，編號為RSA-768（768 bits, 232 digits）數也被成功分解。這一事件威脅了現通行的1024-bit金鑰的安全性，**普遍認為用戶應儘快升級到2048-bit或以上**。~~ ==現在建議 3072 以上==

-   RSA 1024
	- 加密時最大明文長度為**117 Byte**
	- 解密時最大密文長度為128 Byte
-   RSA 2048
	- 加密時最大明文長度為**245 Byte**
	- 解密時最大密文長度為256 Byte

超過時得分段處理（[Asymmetric Encryption Schemes](演算法/Asymmetric%20Encryption%20Schemes.md)），不過 RSA 大部分的用途是在保護 [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md)，像是會議基碼 Session key 等（[數位信封 Digital Envelop](演算法/數位信封%20Digital%20Envelop.md)）。


## 用途
- 成對的金鑰生成（私密、公開）
- 加解密
- [數位簽章](演算法/數位簽章.md)
- 金鑰交換