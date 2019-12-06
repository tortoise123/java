#修复bug 场景：
##基于master 修复bug
```text
1，新建一个分支 git checkout -b issuce-101  ---修改
2，提交修改到issuce-101
3，git checkout master 分支
4，合并分支 git merge issuce-101
5，bug 复制到dev 使用命令 git cherry-pick 4c805e2（合并到master 的id）
如果dev 在开发阶段没有提交保存本地现场用 git stash 
恢复现场用git stash pop  
一是用git stash apply恢复，但是恢复后，stash内容并不删除，你需要用git stash drop来删除；
另一种方式是用git stash pop，恢复的同时把stash内容也删了：
本地文件不提交不保存现场不能切到其他分支
```