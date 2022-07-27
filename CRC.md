# CRC
> Cyclic redundancy check 循環冗餘校驗

>[Day 22 022 - 雜湊 - Hash（番外）](https://ithelp.ithome.com.tw/articles/10243268)


- CRC 跟其他 [Cryptographic Hash Functions](Cryptographic%20Hash%20Functions.md) 來說更偏向「簡單」的比對
- 而 CRC 是線性的變化，可以很簡單的偽造
- 一般是用來檢查錯誤的，非用來處理數據完整
- 可以在第一時間先優先排除簡單的問題，檢查不出來再做更複雜的 Hash 驗證
- 用來實體層傳輸的檢查碼

## CRC-1
- 奇偶校驗位
- 檢查傳輸中奇數位元的損失


## 應用
-   USB傳輸協定
-   Bus傳輸協定
-   Bluetooth（藍牙）傳輸協定
-   乙太網路傳輸協定
