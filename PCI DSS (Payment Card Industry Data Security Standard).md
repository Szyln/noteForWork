# PCI DSS(Payment Card Industry Data Security Standard)
>- [PCI (Payment Card Industry)](PCI%20(Payment%20Card%20Industry).md)
>- [DSS](DSS.md)


>- [想製作線上支付服務？但等等，你了解支付規範龍頭PCI-DSS嗎?](https://progressbar.tw/posts/126)
>- [Day02 支付卡產業資料安全標準(PCI DSS、PA DSS)](https://ithelp.ithome.com.tw/articles/10186215)

- 現在最新大概 6 多，但並不會每年機器都更新，要$
- 2004 年國際信用卡組織(VISA、Mastercard、 JCB、AE與Discover)共同制定的安全標準
- 為保護支付卡片資料
- 支付卡產業資料安全標準

> 支付程式開發商要遵守：支付程式資料安全標準：[PA DSS (Payment Application Data Security Standard)](PA%20DSS%20(Payment%20Application%20Data%20Security%20Standard).md)

### PCI-DSS 的目的
- 構建並維護安全的交易系統及網路(Build and Maintain a Secure Network and Systems)
- 保護交易持卡人數據及資料安全(Protect Cardholder Data)
- 維護漏洞管理程式(Maintain a Vulnerability Management Program)
- 執行嚴格的訪問權限控制措施(Implement Strong Access Control Measures)
- 定期監控並測試服務之網路安全(Regularly Monitor and Test Networks)
- 維護資訊安全政策(Maintain an Information Security Policy)

### 大略的審核階段
1. 自我安全檢測(self security probe)：針對網站的資訊安全、防火牆、硬體架構、敏感資訊流以及相關單位的權責範圍進行檢測
2. 漏洞分析(analysis of the vulnerabilities)：透過由 PCI-DSS 受權認證的廠商進行掃描，避免有相關資安漏洞(像是 SSL 的漏洞，也是容易被掃描出來的核心問題之一)
3. 由認證協會所執行的安全調查(security investigation by the council)：對員工資安概念、公司資安機制導入等相關議題，進行調查並作出綜合評斷，以小編的經歷，甚至會有稽核員來到公司進行督導、訪查喔

>不過現在一般的網站都是串接第三方服務居多，比方說[智付通](https://www.spgateway.com/info/site_description/secure_transaction)、[綠界](https://www.ecpay.com.tw/About/Certificate)等，這些公司都有符合 PCI-DSS 規範。所以一般的開發者如果不涉及”建立“金流服務的話就不需要太過擔心。




