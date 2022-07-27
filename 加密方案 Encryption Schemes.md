# 加密方案 Encryption Schemes
混合多種加密演算法，同時兼顧安全性、真實性、完整性


## 通常包含
- 延緩破解速度：[KDF](KDF.md)
	- [Cryptographic Hash Functions](Cryptographic%20Hash%20Functions.md)
	- [Salting](Salting.md)
	- 使用大量迭代和計算資源
- 通常為 [Block Cipher](Block%20Cipher.md)：例如 [AES](演算法/AES.md)
- 使 [Block Cipher](Block%20Cipher.md) 加密任意大小數據
	- [分組密碼工作模式 Block Cipher Modes of Operation](分組密碼工作模式%20Block%20Cipher%20Modes%20of%20Operation.md)
		- [CBC (Cipher Block Chaining Mode)](CBC%20(Cipher%20Block%20Chaining%20Mode).md)
		- [ECB (Electronic Code Book Mode)](ECB%20(Electronic%20Code%20Book%20Mode).md)
		- CTR
	- 消息填充算法（如 PKCS7）
- 驗證消息的真實性、完整性、不可否認性：[消息認證（MAC）算法](消息認證（MAC）算法.md)

ECIES-secp256k1-AES-128-GCM

## Symmetric Encryption Schemes 
- AES-256-CTR-HMAC-SHA-256：使用 AES-256 與 Counter 分組模式進行加密，使用 HMAC-SHA256 進行消息認證的加密方案。
- ChaCha20-Poly1305：是一個流密碼加密方案
- AES-128-GCM

