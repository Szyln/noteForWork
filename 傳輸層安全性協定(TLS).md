# 傳輸層安全性協定 (TLS)
>wiki 太深奧了看影片，介紹 TLS, 1.2, 1.3 協定：[Transport Layer Security, TLS 1.2 and 1.3 (Explained by Example)](https://youtu.be/AlE5X1NlHgg)
>- Transport Layer Security，縮寫：TLS

>- 前身為：[SSL](SSL.md) 

- 提供 [機密性 Confidentiality](演算法/機密性%20Confidentiality.md) 與 資料[完整性 Integrity](演算法/完整性%20Integrity.md) 的保障
- 是一種[安全協定](https://zh.wikipedia.org/wiki/%E5%AE%89%E5%85%A8%E5%8D%8F%E8%AE%AE "安全協定")

## 歷史
- 1994: Netscape 推出 HTTPS 協定 + SSL 加密
- 1999年公布TLS 1.0標準檔案（[RFC 2246](https://tools.ietf.org/html/rfc2246)）
- 隨後又公布TLS 1.1（[RFC 4346](https://tools.ietf.org/html/rfc4346)，2006年）
- TLS 1.2（[RFC 5246](https://tools.ietf.org/html/rfc5246)，2008年）
- TLS 1.3（[RFC 8446](https://tools.ietf.org/html/rfc8446)，2018年）。



## 概論

TLS協定採用[主從式架構](https://zh.wikipedia.org/wiki/%E4%B8%BB%E5%BE%9E%E5%BC%8F%E6%9E%B6%E6%A7%8B "主從式架構")模型，用於在兩個應用程式間透過網路建立起安全的連線，防止在交換資料時受到[竊聽](https://zh.wikipedia.org/wiki/%E7%AB%8A%E8%81%BD "竊聽")及篡改。

- 由TLS協定進行建立加密通道需要的協商和認證
- 應用層協定傳送的資料在通過TLS協定時都會被加密，從而保證通訊的 [機密性 Confidentiality](演算法/機密性%20Confidentiality.md)。

- 與高層的[應用層](https://zh.wikipedia.org/wiki/%E5%BA%94%E7%94%A8%E5%B1%82 "應用層")協定（如[HTTP](https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "超文字傳輸協定")、[FTP](https://zh.wikipedia.org/wiki/%E6%96%87%E4%BB%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "檔案傳輸協定")、[Telnet](https://zh.wikipedia.org/wiki/Telnet "Telnet")等）無耦合。（不會交互影響）
- 應用層協定能透明地執行在TLS協定之上
- 由TLS協定進行建立加密通道需要的協商和認證
- 應用層協定傳送的資料在通過TLS協定時都會被加密，從而保證通訊的 [機密性 Confidentiality](演算法/機密性%20Confidentiality.md)。

一旦客戶端和伺服器都同意使用TLS協定，他們通過使用一個交握過程協商出一個有狀態的連接以傳輸資料[[1]](https://zh.wikipedia.org/wiki/%E5%82%B3%E8%BC%B8%E5%B1%A4%E5%AE%89%E5%85%A8%E6%80%A7%E5%8D%94%E5%AE%9A#cite_note-1)。通過交握，客戶端和伺服器協商各種參數用於建立安全連接：
