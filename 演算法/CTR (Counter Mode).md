# CTR (Counter Mode)
> 計數器模式

![](其他/附件/Pasted%20image%2020220729112541.png)

> 圖片來源： [Day 21. 加密演算法要注意的那些毛 (一) - 加密模式](https://ithelp.ithome.com.tw/articles/10249953)

- [AES](演算法/AES.md) 公布後發布
- Counter block 是
	- 從 [初始向量 Initialization Vector(IV)](演算法/初始向量%20Initialization%20Vector(IV).md) 生成
	- 有順序的數字字串
	- 長度同明文區塊（常見：64 [位元 bit](計算機/位元%20bit.md)）
- 最後一塊不用 [填充 Padding](演算法/填充%20Padding.md)

## 步驟
1. 金鑰加密 counter
2. 加密後的 counter 與明文區塊 [異或 (⊕)](演算法/異或%20(⊕).md)
3. 得區塊密文

- 每個區塊的加密都會[疊代](計算機/疊代.md)執行
- Counter 會按照他的順序增加
- 影響每次與明文區塊 [異或 (⊕)](演算法/異或%20(⊕).md) 時的結果
	- 就算有明文區塊相同，Counter 不會一樣，所以結果會不一樣

> 每個區塊並沒有直接關聯（沒有 Feedback Mechanism）