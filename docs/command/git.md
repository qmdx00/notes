### Git 常用操作

创建远端分支
```git
 git push --set-upstream origin [branch-name]
```

删除远端分支
```git
git push origin :[branch-name]
```

git 删除分支
```git 
git branch -D [branch-name]
```

交互式变基到指定记录
```git
git rebase -i [commit-hash]
```

继续变基操作
```git
git rebase --continue
```