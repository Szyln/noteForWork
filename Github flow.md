# Github flow
### 常駐分支
- main

### 短期分支 
- 都從 main 分出來
- 命名語意化
	- 例如 refactor-authentication、user-content-cache-key、make-retina-avatars
	- 或是直接加入 issue number



### 生命週期
- 創建或 fork 分支 (Create a branch)
- 提交修改 (Add commits)
- [Pull Request (PR)](Pull%20Request%20 (PR). md)：直接在 GH 網頁操作即可，或是 [Github CLI](Github%20CLI.md)（需額外安裝）
- 代碼審核 (Discuss and review your code)
- 部屬 (Deploy)，先測試是否有bug，測試完畢後再進行下一步
- 合併 (Merge)
- 該分支可以選擇刪除



## 特徵
有新需求都會採 [git rebase](dontTrustYourLittleBrain/git%20rebase.md) 後 [Fast Forward Merge 使舊版本追齊新版本](dontTrustYourLittleBrain/Fast%20Forward%20Merge%20使舊版本追齊新版本.md) 的方法合併

GitLab Flow 會常用到 [git cherry-pick](dontTrustYourLittleBrain/git%20cherry-pick.md) ，避免漏抓 commit，通常會 [改良 source tree 可讀性](dontTrustYourLittleBrain/改良%20source%20tree%20可讀性.md) 來避免這些問題
## 優缺點

### 優點

簡單、適用於「持續更新」的產品的開發流程

### 缺點

預設情況為 master 為最新的提交版本，但這造成有時可能有指定時間發佈，或是尚須審核，則這時候只有一個 master 分支就會造成困擾，需新建一個 `production` 分支追蹤線上版本。

