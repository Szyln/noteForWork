# Release Branches & Upstream First
> 版本發布

![](https://ithelp.ithome.com.tw/upload/images/20191015/20072606FvQ4et0tbJ.png)

- 與 [Environment Branches & Upstream First](Environment%20Branches%20&%20Upstream%20First.md) 不同，版本發布的下游分支是按照程式碼穩定度來發布 [release branch](release%20branch.md)
- [release branch](release%20branch.md) 會用版本號來命名分支（例如：2-3-stable）
相同的是，要修復分支、bug 的時候都是先從上游 main 開始分支做測試，完成後才能合併到下游分支，並且更新版本號
