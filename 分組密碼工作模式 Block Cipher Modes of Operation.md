# 分組密碼工作模式 Block Cipher Modes of Operation

>[對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md)

主流的 [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md) 都是 [Block Cipher](Block%20Cipher.md) ，使用分組密碼工作模式，轉換成 [Stream Cipher](Stream%20Cipher.md)

> - [Day 21. 加密演算法要注意的那些毛 (一) - 加密模式](https://ithelp.ithome.com.tw/articles/10249953)
> - [寫給開發人員的實用密碼學（六）—— 對稱密鑰加密算法](https://thiscute.world/posts/practical-cryptography-basics-6-symmetric-key-ciphers/)

早在 1981 年，DES 演算法公佈之後，NIST 在標準文獻 FIPS 81 中公佈了 4 種工作模式：
- [ECB (Electronic Code Book Mode)](ECB%20(Electronic%20Code%20Book%20Mode).md)
- [CBC (Cipher Block Chaining Mode)](CBC%20(Cipher%20Block%20Chaining%20Mode).md)
-  密文反饋：Cipher Feedback Mode (CFB)
-  輸出反饋：Output Feedback Mode (OFB)

[AES](演算法/AES.md) 公布後
- 計數器模式：Counter Mode (CTR)

## 其他
- GCM：伽羅瓦計數器模式 Galois/Counter Mode
- CCM：Counter with CBC-MAC
