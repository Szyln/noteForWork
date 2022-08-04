## Git flow

![](https://ithelp.ithome.com.tw/upload/images/20191013/20072606m7Qy0zFdnR.jpg)

### 常駐分支
- [master(main) branch](master(main)%20branch.md)
- [develop branch](develop%20branch.md)

### 短期分支 
- [feature branch](feature%20branch.md)
- [hotfix branch](hotfix%20branch.md)
- [release branch](release%20branch.md)

|分支|[feature branch](feature%20branch.md)|[hotfix branch](hotfix%20branch.md)|[release branch](release%20branch.md)|
|:-:|:-:|:-:|:-:|
|[git checkout -b 建立並切換分支](dontTrustYourLittleBrain/git%20checkout%20-b%20建立並切換分支.md)|[develop branch](develop%20branch.md)|[master(main) branch](master(main)%20branch.md)|[develop branch](develop%20branch.md)|
|[git merge](dontTrustYourLittleBrain/git%20merge.md)|[develop branch](develop%20branch.md)|兩常駐分支|兩常駐分支|
|命名習慣|feature-<版號>|bugfix-<版號>|release-<版號>|

## 實作
```mermaid  
gitGraph
	commit id: "plan the flow"
	branch dev order: 3
	checkout dev
	commit id: "plan"
	branch release-1.0 order: 2
	commit id: "release 1.0"
	checkout dev
	branch feature-0.1 order: 4
	branch feature-0.2 order: 5
	checkout feature-0.1
	commit id: "add f1.txt"
	checkout dev
	merge feature-0.1
	checkout feature-0.2
	commit id: "add f2.txt"
	commit id: "add lines in f2.txt"
	checkout dev
	merge feature-0.2
	checkout main
	merge release-1.0
	
	
```