# CBC (Cipher Block Chaining Mode)
> 安全，但 CBC 阻塞模式可能容易受到「padding oracle」攻擊，因此**最好避免使用 CBC 模式**

>- [Cipher Block Chaining (CBC) | Algorithm Modes in Cryptography](https://youtu.be/NnLLkmgBhCY)
>- [Day 21. 加密演算法要注意的那些毛 (一) - 加密模式](https://ithelp.ithome.com.tw/articles/10249953)
- 引入 [初始向量 Initialization Vector(IV)](初始向量%20Initialization%20Vector(IV).md) 的概念（金鑰不變）
- 但同組資料不要多次使用同組 IV

## 步驟
> - [初始向量 Initialization Vector(IV)](初始向量%20Initialization%20Vector(IV).md) 只會跟第一組分組進行[異或 (⊕)](異或%20(⊕).md)

![](https://i.imgur.com/5Hn8Bif.png)

- 第一個分組的明文在加密運算前先與 [初始向量 Initialization Vector(IV)](初始向量%20Initialization%20Vector(IV).md) 進行 [異或 (⊕)](異或%20(⊕).md) （會轉換成二進位資料）
- 第二組之後會跟前一個 ciphertext 進行[異或 (⊕)](異或%20(⊕).md)
- 最後一組會需要 [填充 Padding](填充%20Padding.md) 至 block 大小

### 注意
- 因為其將密文引入運算，加解密操作無法並行操作
- [初始向量 Initialization Vector(IV)](初始向量%20Initialization%20Vector(IV).md)，需要加、解密雙方共同知曉

## 優點
相同明文，會因為前一個的密文不同造就出不同的密文，也就是加密器多一個新的狀態。

## 缺點
- 出錯的時候會連環錯下去