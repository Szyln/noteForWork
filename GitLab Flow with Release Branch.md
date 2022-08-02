# GitLab Flow with Release Branch

> 適用於可以公開下載的軟體，公司內部使用，或是非開源軟體不需要這樣使用

![](其他/附件/Pasted%20image%2020220802155838.png)

[GitLab Flow](GitLab%20Flow.md) 搭配 [release branch](release%20branch.md)，可以版本控制發布軟體的內容

會使用到 [git cherry-pick](dontTrustYourLittleBrain/git%20cherry-pick.md)

可以避免緊急 bugfix 的時候，把 main merge 到 release 時，造成下版才要上線的功能被提早上線