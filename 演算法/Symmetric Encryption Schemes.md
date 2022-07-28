# Symmetric Encryption Schemes 
> symmetric encryption construction

- [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md) 現今很少單純使用，多混合多種加密演算法，同時兼顧安全性、真實性、完整性
- [Block Cipher](演算法/Block%20Cipher.md) 最長的算法是 [AES](演算法/AES.md)256，想要加密任意長度的內容，則需要[分組密碼工作模式 Block Cipher Modes of Operation](演算法/分組密碼工作模式%20Block%20Cipher%20Modes%20of%20Operation.md) 的配合

## 舉例
- AES-256-CTR-HMAC-SHA-256：使用 AES-256 與 Counter 分組模式進行加密，使用 HMAC-SHA256 進行消息認證的加密方案。
- ChaCha20-Poly1305：是一個流密碼加密方案
- AES-128-GCM