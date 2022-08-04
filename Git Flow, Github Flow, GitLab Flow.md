# Flow
>- [Day29｜常見的三種工作流程 - Git flow、GitHub Flow 與 Gitlab Flow](https://ithelp.ithome.com.tw/articles/10281080)
>- [Git上的三種工作流程](https://medium.com/i-think-so-i-live/git%E4%B8%8A%E7%9A%84%E4%B8%89%E7%A8%AE%E5%B7%A5%E4%BD%9C%E6%B5%81%E7%A8%8B-10f4f915167e)


- [Git flow](Git%20flow.md)
- [Github flow](Github%20flow.md)
- [GitLab Flow](GitLab%20Flow.md)



|類型|[Git flow](Git%20flow.md)|[Github flow](Github%20flow.md)|[GitLab Flow](GitLab%20Flow.md)|
|:-:|:-:|:-:|:-:|
|常駐分支|[master(main) branch](master(main)%20branch.md), [develop branch](develop%20branch.md)|[master(main) branch](master(main)%20branch.md)|[master(main) branch](master(main)%20branch.md)|
|遇到 bug|- 從 [master(main) branch](master(main)%20branch.md) 分出來<br>- 完成後合併到兩常駐分支|- 從 [master(main) branch](master(main)%20branch.md) 分出來<br>- 發 [Pull Request (PR)](Pull%20Request%20(PR).md)<br>- 討論後合併進 [master(main) branch](master(main)%20branch.md)|- 從 [master(main) branch](master(main)%20branch.md) 分出來<br>- 發 [Merge Request](Merge%20Request.md)<br>- 討論後合併進 [master(main) branch](master(main)%20branch.md)<br>- 再往下游分支（release、environment）合併|
|適用場合|版本發布|持續更新|持續更新或版本發布|
|缺點|複雜，操作時間成本高|不適合版本發布|指令較難|