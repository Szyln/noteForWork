# CI, CD
> [Day12 什麼是 CICD](https://ithelp.ithome.com.tw/articles/10219083)

![](https://i.imgur.com/V5nuckV.png)

將上線程式的流程自動化
- 自動 build code
- 執行 unit test
- 自動更新線上服務

## 分為兩個步驟

[CI](CI.md)：處理 build
[CD](CD.md)：處理 deploy

## 舉例
開發人員執行 `git push` 至 `Gitlab` 後，將程式更新至 `Server` 的步驟交由 `Jenkins` （自動化建置工具）負責。

![](https://i.imgur.com/aCKJLPK.png)

## CICD 工具介紹

-   GitLab (版控工具)
-   GitHub (版控工具)
-   Jenkins (自動化建置工具)
-   Drone (自動化建置工具)
-   Circle (自動化建置工具)
-   Docker (迅速佈署環境工具)
-   K8S (管理 Docker Container 工具)
-   Helm (快速建置各環境 K8S 工具)
-   Grafana (機器數據監控工具)
-   ELK (Log 蒐集工具)
-   Telegram (通訊、錯誤通知工具)
-   Slack (通訊、錯誤通知工具)
