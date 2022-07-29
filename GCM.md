# GCM (Galois, Counter Mode)

- 在 [CTR (Counter Mode)](CTR%20(Counter%20Mode).md) 的基礎上，添加了消息認證的功能
- 具有與 CTR 模式相同的並行計算能力
- 額外提供對消息 [完整性 Integrity](演算法/完整性%20Integrity.md)、[鑑別性（真實性） (Authenticity)](鑑別性（真實性）%20(Authenticity).md) 的驗證能力。
- GCM 現在屬於最嚴謹的加密模式，TLS 1.2 標準使用的就是 AES-GCM 演算法。

![](其他/附件/Pasted%20image%2020220729131639.png)

> 圖片來源： [Day 21. 加密演算法要注意的那些毛 (一) - 加密模式](https://ithelp.ithome.com.tw/articles/10249953)