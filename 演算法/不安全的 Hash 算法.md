# 不安全的 Hash 算法
- 已發現漏洞，[碰撞 collision](演算法/碰撞%20collision.md)
- 會導致
	- [數位簽章](演算法/數位簽章.md)被偽造
	- 密碼洩漏

## 例如
- MD5
- SHA-0
- SHA-1

## 避免使用
- MD2
- MD4
- MD5
- SHA-0
- SHA-1
- Panama
- **HAVAL**（有爭議的安全性，在 HAVAL-128 上發現了碰撞）
- **Tiger**（有爭議，已發現其弱點）
- **SipHash**（它屬於非加密哈希函數）