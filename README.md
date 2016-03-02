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
