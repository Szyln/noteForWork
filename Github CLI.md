#  Github CLI
> 需安裝：[CLI](https://cli.github.com/)

安裝完後，就可以用終端機執行看看了（WINDOWS 的 PowerShell 沒辦法，要用命令提示字元）

```shell
$ gh # 不知道該怎麼辦的時後，先執行看看，有沒有成功安裝
```
## 登入 Github
```shell
$ gh auth login
```
### 驗證步驟
```shell
? What account do you want to log into? GitHub.com
? What is your preferred protocol for Git operations? HTTPS # 不確定就先用這個
? Authenticate Git with your GitHub credentials? Yes
? How would you like to authenticate GitHub CLI? Login with a web browser

! First copy your one-time code: XXXX-XXXX # 一串認證碼，上 GH 登入取得授權
Press Enter to open github.com in your browser...
✓ Authentication complete.
- gh config set -h github.com git_protocol https
✓ Configured git protocol
✓ Logged in as Szyln
```

## [Pull Request (PR)](Pull%20Request%20(PR).md)

```shell
gh pr create # 建立
```


```shell
Creating pull request for 貢獻者:main into main in 開發者 REPO

? Title (szyen add words 1) # 輸入 PR 標題

? Title # PR 標題
? Body <Received> # 選填
? What's next? Submit # 會有幾個選項，我選直接提交
https://github.com/Shay-castles/learnGithubFlow/pull/1

# 這樣開發者的 REPO 上就會收到通知了（GH 專案頁面上 + EMAIL 通知）
```

如果開發者選擇 merge 貢獻者的更改，就會在
![](其他/附件/Pasted%20image%2020220801173743.png)