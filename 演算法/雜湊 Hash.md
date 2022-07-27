# 雜湊 Hash

>- 特化於加密用途的內容：[Cryptographic Hash Functions](Cryptographic%20Hash%20Functions.md)
>- 也有比較注重速度，隨機均勻性的：非加密哈希函數

> Hash 函數又稱散列函數
- 將密碼存入 Database 前，會先用 Hash Function 加工
- ==不是加密，所以不能解密==
- 以目前技術近乎不可逆
- 不管原始密碼 (input) 多少，Hash Function 都會產生相同長度的 [Ciphertext](Ciphertext.md)（數字指紋、數字摘要）
- 原始密碼做些微的更動後， [Ciphertext](Ciphertext.md) 會有很大的差異
- 使用國際標準且尚未遭到破解的加密演算法(MD5 -> SHA2)

## 注意
- 因為同樣的 input 會得到相同的結果：導致 [[Dictionary Attack]] 的風險
- [碰撞 collision](碰撞%20collision.md)




