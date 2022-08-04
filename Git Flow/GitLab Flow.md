# GitLab Flow
> [GitLab Flow](https://youtu.be/InKNIvky2KE)


- 介於 [Git flow](Git%20Flow/Git%20flow.md) 與 [Github flow](Git%20Flow/Github%20flow.md) 中間
- 操作大致與 [Github flow](Git%20Flow/Github%20flow.md) 相同
- [upsteam (main branch) first](upsteam%20(main%20branch)%20first.md)
	- [Environment Branches](Environment%20Branches.md)
	- [Release Branches](Release%20Branches.md)

##



## 與 Github flow 的差別
相對 [Github flow](Git%20Flow/Github%20flow.md) ，[GitLab Flow](GitLab%20Flow.md) 對發佈版本，會使用 [git cherry-pick](../dontTrustYourLittleBrain/git%20cherry-pick.md) 配合達成
- [GitLab Flow with Release Branch](GitLab%20Flow%20with%20Release%20Branch.md)


## Merge Request 的步驟

更新 main 分支時必須發起 [Merge Request](Git%20Flow/Merge%20Request.md)，經審核、討論、測試後才能與 main 合併

- [Pull, Merge Request 的生命週期](Pull,%20Merge%20Request%20的生命週期.md)


## 其他
- [GitLab Flow 的 CI, CD](GitLab%20Flow%20的%20CI,%20CD.md)
	- [CI, CD](Git%20Flow/CI,%20CD.md)
- [改良 merge 的 commit 可讀性](../dontTrustYourLittleBrain/改良%20merge%20的%20commit%20可讀性.md)