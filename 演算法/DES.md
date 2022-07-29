# DES
> DEA, Data Encryption Algorithm

> [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md)

- [對稱金鑰 Symmetric](演算法/對稱金鑰%20Symmetric.md)
- 金鑰長度為 ==64 bits== (實際使用56 bits)
- 每一次只加密 64 bits (8 byte) 區塊的明文資料，經過[混淆與擴散](演算法/混淆與擴散.md)後，輸出的加密結果也是 64 bits (8 byte)。
- 支付卡產業中，幾乎所有的驗證值，卡片磁條內的、卡片背後的、卡片晶片內的，還有許多檢算**還是維持在DEA或是2TDEA演算法**，也因為支付卡產業只使用在運算驗證值上而不是加密整段明文

## 歷史
- DES演算法是70年代末藍色巨人IBM旗下力挺的新人
- 80年代後，於許多信用卡磁條、晶片儲存的驗證值上用上

>在許多檔案傳輸與晶片卡文件中，為了和資料加密標準 DES(Data Encryption Standard)有所區隔，==DES 又稱為 :DEA(Data Encryption Algorithm)==

- 由於==DEA金鑰長度不夠而存在金鑰破解問題==，後來有衍生了兩種 Triple DEA 的演算法，主要在運算過程強化金鑰及運算步驟。
	- [TDEA](演算法/TDEA.md)
	- [2TDEA](演算法/2TDEA.md)
- DEA在2000年後已經被公認為是一種不安全的加密方法，主要原因**加密所使用的金鑰過短**(56 bits)
- [AES](演算法/AES.md) 逐漸取代，2002年後已成為美國聯邦政府新的標準。