# 初始向量 Initialization Vector(IV)
> [The Initialization Vector (IV)](https://cryptobook.nakov.com/symmetric-key-ciphers/cipher-block-modes#the-initialization-vector-iv)

>又被稱為 Salt, Nonce（隨機數）

- 隨機且不可預知
- 不應重複使用
- 不同的明文不該使用同個 [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md) 及對應同個 IV
- 但同組資料不要多次使用同組 IV
- 需要與 Cipher Block 大小一致
	- [AES](演算法/AES.md), Serpent, Camellia: 128 bits
- GCM 的 IV 不需非公開也不須無法預測，但還是要每個明文都用不同的 IV