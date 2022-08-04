# Github flow

- 只有一個常駐分支 main
- main 的更新需透過 [Pull Request (PR)](Pull%20Request%20(PR).md) 從 fork 或是其他的 branch 來合併
- 適合持續更新的專案
- 適合開源軟體
- 需要版本發布的會比較不適合

## 分支
### 常駐分支
- main

### 短期分支 
- 都從 main 分出來
- 命名語意化
	- 例如 refactor-authentication、user-content-cache-key、make-retina-avatars
	- 或是直接加入 issue number（可搭配像是 Jira, Asana 任務管理軟體）

### 其他分支
> 可以看 [GitLab Flow](GitLab%20Flow.md) 的方法 

- 當有發布時程上的需求時，可能會需要 production 分支
	- 需要發布不同版本（發布 IOS 版）
	- 按照時間排程發布而非按照更新進度發布的內容


## [Pull Request (PR)](Pull%20Request%20(PR).md) 的步驟
[Pull, Merge Request 的生命週期](Pull,%20Merge%20Request%20的生命週期.md)




