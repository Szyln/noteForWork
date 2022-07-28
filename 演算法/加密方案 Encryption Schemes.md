# 加密方案 Encryption Schemes

>- 對稱金鑰加密方案：[Symmetric Encryption Schemes](Symmetric%20Encryption%20Schemes.md)
>- 非對稱金鑰加密方案：[Asymmetric Encryption Schemes](Asymmetric%20Encryption%20Schemes.md)


單純使用[對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md)、[非對稱金鑰 Asymmetric](演算法/非對稱金鑰%20Asymmetric.md)，只能顧及[機密性 Confidentiality](機密性%20Confidentiality.md)，混合多種加密演算法，同時兼顧
- [機密性 Confidentiality](機密性%20Confidentiality.md)
- [可歸責性 Accountability](可歸責性%20Accountability.md)
- [完整性 Integrity](完整性%20Integrity.md)


## 通常包含
- 延緩破解速度：[KDF (Key Derivation Functions)](演算法/KDF%20(Key%20Derivation%20Functions).md)
- 通常為 [Block Cipher](演算法/Block%20Cipher.md)：例如 [AES](演算法/AES.md)
- 使 [Block Cipher](演算法/Block%20Cipher.md) 加密任意大小數據
	- [分組密碼工作模式 Block Cipher Modes of Operation](演算法/分組密碼工作模式%20Block%20Cipher%20Modes%20of%20Operation.md)
		- [CBC (Cipher Block Chaining Mode)](演算法/CBC%20(Cipher%20Block%20Chaining%20Mode).md)
		- [ECB (Electronic Code Book Mode)](演算法/ECB%20(Electronic%20Code%20Book%20Mode).md)
		- CTR
	- [填充 Padding](填充%20Padding.md)
- 驗證消息的[可歸責性 Accountability](可歸責性%20Accountability.md)、[完整性 Integrity](完整性%20Integrity.md)：[消息認證（MAC）算法](演算法/消息認證（MAC）算法.md)




