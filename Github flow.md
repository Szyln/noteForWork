# Github flow

- 只有一個常駐分支 main
- main 的更新需透過 [Pull Request (PR)](Pull%20Request%20 (PR). md) 從 fork 或是其他的 branch 來合併
- 適合持續更新的專案（例如每天）
- 適合開源軟體

## 分支
### 常駐分支
- main

### 短期分支 
- 都從 main 分出來
- 命名語意化
	- 例如 refactor-authentication、user-content-cache-key、make-retina-avatars
	- 或是直接加入 issue number（可搭配像是 Jira, Asana 任務管理軟體）

### 其他分支
- 當有發布時程上的需求時，可能會需要 production 分支
	- 需要發布不同版本（發布 IOS 版）
	- 按照時間排程發布而非按照更新進度發布的內容
	- 
### 分支的生命週期
- 創建或 fork 分支 (Create a branch)
- 提交修改 (Add commits)
- [Pull Request (PR)](Pull%20Request%20(PR).md)：直接在 GH 網頁操作即可，或是 [Github CLI](Github%20CLI.md)（需額外安裝）
- 代碼審核 (Discuss and review your code)
- 部屬 (Deploy)，先測試是否有bug，測試完畢後再進行下一步
- 合併 (Merge)
- 該分支可以選擇刪除




