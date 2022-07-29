# 雜湊 Hash

>- 特化於加密用途的內容：[Cryptographic Hash Functions](演算法/Cryptographic%20Hash%20Functions.md)
>- 也有比較注重速度，隨機均勻性的：非加密哈希函數

> [演示](https://totools.site/SHA)

%%不管我打什麼，都會產生固定長度的 hash 值，
同樣內容不管生成幾遍，結果一樣
只做小小的更改，值就會大幅更動%%

> Hash 函數又稱散列函數

- ==不是加密，所以不能解密==（只能暴力破解）
- 以目前技術近乎不可逆
- 不管輸入值多少，Hash Function 都會產生相同長度的 Hash 值（數字指紋、數字摘要）
- 輸入值做些微的更動後，  Hash 值會有很大的差異



## 注意
- [碰撞 collision](演算法/碰撞%20collision.md)
- 因為同樣的 input 會得到相同的結果：導致 [Dictionary Attack](演算法/Dictionary%20Attack.md) 的風險




