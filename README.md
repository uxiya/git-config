git config
====

git 设置
* git log `git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --"`
* git diff `git config color.ui true`

git 使用
* `git log -p -2`  -p选项展开显示每次提交的内容差异 -2仅显示最近两次的更新
* `git log -p --grep keyword` 展开显示每次提交的内容差异 并搜索
* `git log --stat` --stat 仅显示简要的增改行数统计 
* `git log --author=zjt --since=2016-01-01` 增加显示条件  
* `git add -p file` -p 分阶段提交代码
* `git reset --hard commit_id`,`git push origin HEAD -force` 撤销到某次提交
* `git checkout master` `git pull` `git merge --no-ff develop` 合并分支 --no-ff 取消快进合并fast-farward merge,产生一个节点
* `git fetch origin` `git rebase origin/master` 与主干同步

git flow
* `git checkout -b develop master` 创建开发分支
* `git checkout -b feature/x develop` 创建功能分支
* `git branch -d featurex` 删除功能分支
* `git push origin --delete xxx` 删除远程分支
* `git push origin --delete tag xxx` 删除tag
* `git checkout -b release/0.1 develop` 创建预发布分支 
* `git tag -a 0.1 -m "tag info" master` `git push --tags` 创建标签 推送标签
* `git remote prune origin` 删除本地但在远程不存在的远程分支

