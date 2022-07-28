# 非對稱金鑰 Asymmetric
> 又稱公開金鑰加密法


非對稱金鑰利用數學上兩個巨大質數的乘積與因式分解產生兩把金鑰
- 公開金鑰 (發送端加密用)
- 私密金鑰 (接收端解密用)

實作出`解密(加密(明文))=明文`的加解密流程。

## 特性

- 速度較慢
- 可==解決加解密端使用同把金鑰的問題==
- 公開金鑰 (public key) 與私密金鑰 (private key)
- 公開金鑰可以存在於非安全的管道中（被監聽也不會被破解）
- [加密方案 Encryption Schemes](演算法/加密方案%20Encryption%20Schemes.md)

## 舉例
- 量子不安全
	- [RSA](演算法/RSA.md)
	- [ECC](演算法/ECC.md)
- 量子安全
		- NewHope、NTRU、GLYPH、BLISS、XMSS、[Picnic](https://github.com/Microsoft/Picnic)