# git-try
    Only be used to be familiar for Git.
## Base Command

|命令|描述|例子|
|:---:|:---|:---:|
|git help|-a:显示所有<br />-g显示所有手册|git help add|
|git config|--unset 重新配置<br />--global 针对用户 <br />--list显示列表|git config --global user.name|
|git init|初始化.git文件夹||
|git commit|-m<br />-am 可以直接add进缓存区后提交|git commit -m "for test"|
|git status|显示分支||
|git add|添加到工作区<br />. 添加全部<br />[filename] 添加对应文件|git add .|
|git rename|重命名已跟踪的文件||
|git rm|删除文件<br />--cache 仅从暂存区删除|git rm src/test.txt|
|git mv|移动文件|git mv test.txt src/test.txt|
|git reset|重置 add添加的文件<br />HEAD 全部<br />HEAD [filename] 重置对应文件|git reset HEAD README.md|
|git revert|[id] 恢复到指定版本号(更新的代码会丢失)|git revert [id]|
|git reset|--soft 会保留更新，不会影响工作区和暂存区，回退的代码更新会出现在暂存区<br />--hard 会影响工作区（更新的代码会被丢弃，！！！不可恢复）<br />--mixed 默认 ，只会更新暂存区（不会导致代码丢失） |git reset --soft [id]|
|git branch|[] 查看全部分支，标记*号 为当前分支<br /> [new branchname] 创建新分支<br />[target branch] [newbranchname] 重命名分支||
|git checkout |[branchname] 切换到新分支||
|git diff|[分支1]..[分支2] 显示两个分支之间的区别 <br />[分支1]..[分支2] [文件名] 显示两个分支之间某个文件的区别||
|git merge|[分支名] 把目标分支的提交合并到当前分支上<br /> abort 取消这次merge|git merge abort|