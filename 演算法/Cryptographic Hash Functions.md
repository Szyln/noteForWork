# 加密 Hash Functions 
>Cryptographic Hash Functions

>[雜湊 Hash](演算法/雜湊%20Hash.md)


- 抗[碰撞 collision](演算法/碰撞%20collision.md)（輸出越長越抗）
- 不可逆
- [理想的 Hash Functions](演算法/理想的%20Hash%20Functions.md)



## 舉例
- [不安全的 Hash 算法](演算法/不安全的%20Hash%20算法.md)
	- [MD5](演算法/MD5.md)
	- SHA1
- 高度安全
	- [SHA2](演算法/SHA2.md)
	- [SHA3](演算法/SHA3.md)



## 量子安全性

現代密碼學哈希函數（如 SHA2, SHA3, BLAKE2）都被認為是量子安全的，無懼量子計算機的發展。


## 應用
- [數據完整性校驗](演算法/數據完整性校驗.md)
	- [CRC](演算法/CRC.md)
- [安全的保存密碼](演算法/安全的保存密碼.md)
- 生成唯一 ID（數字指紋）
- 偽隨機數生成：哈希值可以被當作一個隨機數看待
- [KDF (Key Derivation Functions)](演算法/KDF%20(Key%20Derivation%20Functions).md)



