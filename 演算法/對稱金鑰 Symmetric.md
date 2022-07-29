# 對稱金鑰 Symmetric
- 對稱金鑰使用同一把金鑰（共享密鑰（Shared Secret Key））作加解密
- 執行速度快
- 適合加密大量資料
- 資料可逆
- 現今很少單獨使用：[加密方案 Encryption Schemes](演算法/加密方案%20Encryption%20Schemes.md)
- 可用於[消息認證（MAC）算法](演算法/消息認證（MAC）算法.md)
##  舉例
- [DES](演算法/DES.md)
	- [TDEA](演算法/TDEA.md)
	- [2TDEA](演算法/2TDEA.md)
- [AES](演算法/AES.md)(AES-128、AES-192、AES-256)
- ChaCha20
- Twofish
- IDEA
- Serpent
- Camelia
- RC6
- CAST


## 分類
- [Block Cipher](演算法/Block%20Cipher.md)
- [Stream Cipher](演算法/Stream%20Cipher.md)

|分類|[Block Cipher](演算法/Block%20Cipher.md)|[Stream Cipher](演算法/Stream%20Cipher.md)|
|:-:|:-:|:-:|
|加密數據的長度限制|固定大小|任意|
|KEY 是否更動|否|是|
|舉例|[AES](演算法/AES.md), RC6, Camellia, Serpent 等相關主流 [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md)|較少，例 ChaCha20|
|[分組密碼工作模式 Block Cipher Modes of Operation](演算法/分組密碼工作模式%20Block%20Cipher%20Modes%20of%20Operation.md)|轉換成 [Stream Cipher](演算法/Stream%20Cipher.md) 加密任意長度數據|不需要|


[分組密碼工作模式 Block Cipher Modes of Operation](演算法/分組密碼工作模式%20Block%20Cipher%20Modes%20of%20Operation.md) 可以將前者轉換成後者，使 [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md) 可以加密任意長度的明文
