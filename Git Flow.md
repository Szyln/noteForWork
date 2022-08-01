# Flow
>- [Day29｜常見的三種工作流程 - Git flow、GitHub Flow 與 Gitlab Flow](https://ithelp.ithome.com.tw/articles/10281080)
>- [Git上的三種工作流程](https://medium.com/i-think-so-i-live/git%E4%B8%8A%E7%9A%84%E4%B8%89%E7%A8%AE%E5%B7%A5%E4%BD%9C%E6%B5%81%E7%A8%8B-10f4f915167e)


- Git flow
- GitHub Flow
- Gitlab Flow


## Git flow

### 常駐分支
- [master branch](master%20branch.md)
- [develop branch](develop%20branch.md)

### 短期分支 
- [feature branch](feature%20branch.md)
- [hotfix branch](hotfix%20branch.md)
- [release branch](release%20branch.md)

|分支|[feature branch](feature%20branch.md)|[hotfix branch](hotfix%20branch.md)|[release branch](release%20branch.md)|
|:-:|:-:|:-:|:-:|
|[git checkout -b 建立並切換分支](dontTrustYourLittleBrain/git%20checkout%20-b%20建立並切換分支.md)|[develop branch](develop%20branch.md)|[master branch](master%20branch.md)|[develop branch](develop%20branch.md)|
|[git merge](dontTrustYourLittleBrain/git%20merge.md)|[develop branch](develop%20branch.md)|兩常駐分支|兩常駐分支|
|命名習慣|feature-<版號>|bugfix-<版號>|release-<版號>|

# Github flow
### 常駐分支
- [master branch](master%20branch.md)

### 短期分支 
- 都從 [master branch](master%20branch.md) 分出來
- 不論完成或需要討論時，都向 [master branch](master%20branch.md) 發出 Pull Request (PR)
- Pull Request 被接受後，就會合併到 [master branch](master%20branch.md)
- 該分支就會刪除

-   創建分支 (Create a branch) (fork也可以)
-   提交修改 (Add commits)
-   開啟 PR (Open a Pull Request)
-   代碼審核 (Discuss and review your code)
-   部屬 (Deploy)，先測試是否有bug，測試完畢後再進行下一步
-   合併 (Merge)

## 優缺點
### 優點

簡單、適用於「持續更新」的產品的開發流程

### 缺點

預設情況為 master 為最新的提交版本，但這造成有時可能有指定時間發佈，或是尚須審核，則這時候只有一個 master 分支就會造成困擾，需新建一個 `production` 分支追蹤線上版本。