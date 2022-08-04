# GitLab Flow
> [GitLab Flow](https://youtu.be/InKNIvky2KE)


- 介於 [Git flow](Git%20flow.md) 與 [Github flow](Github%20flow.md) 中間
- 操作大致與 [Github flow](Github%20flow.md) 相同
- [upsteam (main branch) first](upsteam%20(main%20branch)%20first.md)

## 適用情境
- [Environment Branches & Upstream First](Environment%20Branches%20&%20Upstream%20First.md)
- [Release Branches & Upstream First](Release%20Branches%20&%20Upstream%20First.md)

- [Merge Request](Merge%20Request.md)
- [GitLab Flow 的 CI, CD](GitLab%20Flow%20的%20CI,%20CD.md)
	- [CI, CD](CI,%20CD.md)
- [改良 merge 的 commit 可讀性](dontTrustYourLittleBrain/改良%20merge%20的%20commit%20可讀性.md)

## 與 Github flow 的差別
相對 [Github flow](Github%20flow.md) 簡易的操作，[GitLab Flow](GitLab%20Flow.md) 對發佈版本會使用 [git cherry-pick](dontTrustYourLittleBrain/git%20cherry-pick.md) 配合達成
- [GitLab Flow with Release Branch](GitLab%20Flow%20with%20Release%20Branch.md)



## 特點
有新需求都會採 [git rebase](dontTrustYourLittleBrain/git%20rebase.md) 後 [Fast Forward Merge 使舊版本追齊新版本](dontTrustYourLittleBrain/Fast%20Forward%20Merge%20使舊版本追齊新版本.md) 的方法合併

GitLab Flow 會常用到 [git cherry-pick](dontTrustYourLittleBrain/git%20cherry-pick.md) ，避免漏抓 commit，通常會[改良 merge 的 commit 可讀性](dontTrustYourLittleBrain/改良%20merge%20的%20commit%20可讀性.md)來避免這些問題