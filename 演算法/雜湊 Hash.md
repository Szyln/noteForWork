# 雜湊 Hash

>- 特化於加密用途的內容：[Cryptographic Hash Functions](演算法/Cryptographic%20Hash%20Functions.md)
>- 也有比較注重速度，隨機均勻性的：非加密哈希函數

>演示：[sha256-hash-calculator](https://xorbin.com/tools/sha256-hash-calculator)
%%不管我打什麼，都會產生固定長度的 hash 值，
同樣內容不管生成幾遍，結果一樣
只做小小的更改，值就會大幅更動%%

> Hash 函數又稱散列函數
- 將密碼存入 Database 前，會先用 Hash Function 加工
- ==不是加密，所以不能解密==
- 以目前技術近乎不可逆
- 不管原始密碼 (input) 多少，Hash Function 都會產生相同長度的 [Ciphertext](演算法/Ciphertext.md)（數字指紋、數字摘要）
- 原始密碼做些微的更動後， [Ciphertext](演算法/Ciphertext.md) 會有很大的差異


## 注意
- 因為同樣的 input 會得到相同的結果：導致 [Dictionary Attack](演算法/Dictionary%20Attack.md) 的風險
- [碰撞 collision](演算法/碰撞%20collision.md)




