# KDF (Key Derivation Functions)
>密鑰派生函數，又稱慢 hash 算法

- Deriving Key from Password
- 將 Password （一般人設定的密碼，語意化且不會太長）安全地派生出 Hash 值（或密鑰）
- 安全的值可以延緩破解速度
- 直接使用像是 [SHA2](演算法/SHA2.md) 等 [Cryptographic Hash Functions](演算法/Cryptographic%20Hash%20Functions.md) 生成是不夠安全的
	- 不夠安全的值很容易會被暴力破解、字典攻擊、彩虹表攻擊

## KDF 如何增強安全性（增強 [碰撞 collision](演算法/碰撞%20collision.md) 難度）
- 密鑰拉伸 Key stretching
	- [Salting](演算法/Salting.md) 
	- 多次 [疊代](計算機/疊代.md)




## 舉例

- PBKDF2：簡易，不推薦
- Bcrypt：安全性在下降了，不建議使用
- Scrypt：可以靈活地設定使用的內存大小，在 argon2 不可用時，可使用它。
- Argon2：目前最強