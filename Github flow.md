# Github flow
### 常駐分支
- [master branch](master%20branch.md)

### 短期分支 
- 都從 [master branch](master%20branch.md) 分出來
- 不論完成或需要討論時，都向 [master branch](master%20branch.md) 發出 [Pull Request (PR)](Pull%20Request%20(PR).md)
- Pull Request 被接受後，就會合併到 [master branch](master%20branch.md)
- 該分支可以選擇刪除


### 生命週期
-   創建分支 (Create a branch) (fork也可以)
-   提交修改 (Add commits)
-   開啟 PR (Open a Pull Request)：直接在 GH 網頁操作即可，或是 [Github CLI](Github%20CLI.md)（需額外安裝）
-   代碼審核 (Discuss and review your code)
-   部屬 (Deploy)，先測試是否有bug，測試完畢後再進行下一步
-   合併 (Merge)

## 優缺點

### 優點

簡單、適用於「持續更新」的產品的開發流程

### 缺點

預設情況為 master 為最新的提交版本，但這造成有時可能有指定時間發佈，或是尚須審核，則這時候只有一個 master 分支就會造成困擾，需新建一個 `production` 分支追蹤線上版本。

