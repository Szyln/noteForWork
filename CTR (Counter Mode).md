# CTR (Counter Mode)
> 計數器模式

![](其他/附件/Pasted%20image%2020220729112541.png)

> 圖片來源： [Day 21. 加密演算法要注意的那些毛 (一) - 加密模式](https://ithelp.ithome.com.tw/articles/10249953)

- [AES](演算法/AES.md) 公布後發布
- Counter block 是
	- 有順序的數字字串
	- 長度同明文區塊（常見：64 [位元 bit](計算機/位元%20bit.md)）


## 步驟
1. 金鑰加密 counter
2. 加密後的 counter 與明文區塊 [異或 (⊕)](演算法/異或%20(⊕).md)
3. 得區塊密文

每個明文區塊都會[疊代](計算機/疊代.md)執行，Counter 會按照他的順序增加，影響每次加密