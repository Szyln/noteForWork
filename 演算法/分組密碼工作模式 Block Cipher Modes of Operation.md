# 分組密碼工作模式 Block Cipher Modes of Operation
> 可簡稱 Cipher Block Modes, Block Modes, 分組模式

> - [Day 21. 加密演算法要注意的那些毛 (一) - 加密模式](https://ithelp.ithome.com.tw/articles/10249953)
> - [寫給開發人員的實用密碼學（六）—— 對稱密鑰加密算法](https://thiscute.world/posts/practical-cryptography-basics-6-symmetric-key-ciphers/)


主流的 [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md) 幾乎都是 [Block Cipher](演算法/Block%20Cipher.md) ，使用分組密碼工作模式，轉換成 [Stream Cipher](演算法/Stream%20Cipher.md)

將明文分成多個長度固定的分組，使用分組密碼算法進行加解密，實現加解密任意長度的數據



## 基本流程
1.   初始化加密算法狀態（使用加密密鑰 + [初始向量 Initialization Vector(IV)](演算法/初始向量%20Initialization%20Vector(IV).md)）
1.   加密數據的第一個分組
1.   使用加密密鑰和其他參數轉換加密算法的當前狀態
1.   加密下一個分組
1.  再次轉換加密狀態
1.   再加密下一分組
1.   依此類推，直到處理完所有輸入數據



## 是否需要填充
部分分組模式會要求分組後使用 [填充 Padding](演算法/填充%20Padding.md) 將最後的分組填充到 block 的大小
- 會
	- [CBC (Cipher Block Chaining Mode)](演算法/CBC%20(Cipher%20Block%20Chaining%20Mode).md)
- 不會
	- [CTR (Counter Mode)](CTR%20(Counter%20Mode).md)、CFB、OFB、CCM、EAX 和 GCM（因為在每個步驟中，都直接在明文部分和內部密碼狀態之間執行異或（XOR）運算）


## 歷史

- 早在 1981 年，DES 演算法公佈之後，NIST 在標準文獻 FIPS 81 中公佈了 4 種
	- [ECB (Electronic Code Book Mode)](演算法/ECB%20(Electronic%20Code%20Book%20Mode).md)
	- [CBC (Cipher Block Chaining Mode)](演算法/CBC%20(Cipher%20Block%20Chaining%20Mode).md)
	-  密文反饋：Cipher Feedback Mode (CFB)
	-  輸出反饋：Output Feedback Mode (OFB)
- [AES](演算法/AES.md) 公布後
	- 計數器模式：[CTR (Counter Mode)](CTR%20(Counter%20Mode).md)

## 其他分組密碼工作模式
- [GCM](GCM.md)：伽羅瓦計數器模式 Galois/Counter Mode
- CCM：Counter with CBC-MAC


## 舉例

-   **AES-256-GCM** - the AES cipher with a 256-bit encryption key and GCM block mode
-   **AES-128-CTR** - the AES cipher with a 128-bit encryption key and CTR block mode
- **Serpent-128-CBC** - the Serpent cipher with 128-bit encryption key and CBC block mode