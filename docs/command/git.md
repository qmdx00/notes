### Git 常用操作

Git 提交规范
```text
feat - A new feature
fix - A bug fix
docs - Documentation only changes
style - Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
refactor - A code change that neither fixes a bug nor adds a feature
perf - A code change that improves performance
test - Adding missing tests or correcting existing tests
build - Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
ci - Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
chore - Other changes that don't modify src or test files
revert - Reverts a previous commit
```

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