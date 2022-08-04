# Environment Branches & Upstream First
> 持續發布的專案

- 有持續發布需求的專案，可以開 production, pre-production 的分支
- 要一次和並且確保通過測試才可以往下游合併
- 除非是緊急情況，才允許跳過上游直接在下游操作合併。

![](https://ithelp.ithome.com.tw/upload/images/20191015/20072606Bsq4LWrZKR.png)

> master 為 upsteam


## 舉例
如果 production 分支遇到問題，必須先從 main 開分支修正錯誤，測試無誤之後才可以從上游往下併到生產環境
