# Salting
- 在執行 [雜湊 Hash](演算法/雜湊%20Hash.md) 之前多一道手續── Salting ──原始密碼先加上一些隨機字元之後再執行加密，使同一組密碼在數據庫內也長得不一樣
- 加上去的隨機字元並不是隱密的，但因為 [雜湊 Hash](演算法/雜湊%20Hash.md) 是近乎不可逆的，所以也近乎不能回推原始密碼

## 應用
[KDF (Key Derivation Functions)](演算法/KDF%20(Key%20Derivation%20Functions).md)