---
link: https://www.notion.so/Hash-6fdaf3ef12da405ab74ffdfe0cc3ce33
notionID: 6fdaf3ef-12da-405a-b74f-fdfe0cc3ce33
---
# 雜湊 Hash
- 將密碼存入 Database 前，會先用 Hash Function 加工
- ==不是加密，所以不能解密==
- 以目前技術近乎不可逆
- 不管原始密碼(input)多少，Hash Function 都會產生相同長度的 [[Cipher]]
- 原始密碼做些微的更動後，[[Cipher]] 會有很大的差異
- 使用國際標準且尚未遭到破解的加密演算法(MD5 -> SHA2)
- 但是同樣的 input 會得到相同的結果，導致 [[Dictionary Attack]] 的風險，使用 [[Salting]] 避免

## 問題：[[Dictionary Attack]]
由於同一個密碼 Hash Function 的結果一樣，駭客會透過 [[Dictionary Attack]] 的方法破解

### 解決方式：[[Salting]]


## 舉例
- MD5
- SHA1
- SHA2



