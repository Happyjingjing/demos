# demos
git-study:


git init  // git 文件

ssh-keygen  //关联本地文件

git config --global user.name 名字    //设置名字

git config --global user.email 邮箱

git remote add origin 地址  //建立联系

git config --list  // 查看目录

git pull origin master  //查看远端分支

ls  // 当前文件



git add .  // 添加 . 代表所有更改  (git add index.html 指定一个)

git commit -m 'first'  // 添加名字 first

git push origin master   // 推送到Git更新  （origin 是可更改别名）


git remote rename origin dev  //重命名  （原来的名字是 origin  现在的名字是 dev）

git push dev master // 推送到Git更新


git remote -v   // 查看远程仓库

git remote rename old new  // 远程仓库重命名

git remote add <name> <remote>  // 添加源仓库地址为远程仓库

git status  //工作目录和暂存是否一致

基础工作流

克隆仓库： git clone <repository>

提交到本地仓库： git commit -m '...'

查看当前文件状态： git status 

提交内容到远程仓库： git push <remote><branch>

提交到暂存区：git add <pathspec>

git checkout -- index.html //撤销

git log   // 修改列表

git reset HEAD^   // 回退到（HEAD）版本，回退一个版本

git reset --hard HEAD~1  // 回退到前一个版本

git reflog  // 版本列表

git reset --hard  版本号   // 回退到指定版本


比较工作区与暂存区 ： git diff 

比较暂存区与本地版本库最近一次commit的内容： git diff -- cached

比较工作区与本地版本库中最近一次commit的内容： git diff HEAD 

比较两个commit之间的差异： git diff <commit-id> <commit-id>

查看状态： git status 

查看历史操作记录： git reflog

查看日志： git log <fileName>

查看分支：git branch

创建并切换分支： git checkout -b <name>

创建新分支： git branch <name>

切换分支： git checkout <name>

删除本地分支： git branche -d <name>

删除远程分支： git push -d <origin> <branch>

无冲突合并： git merge <branch>

有冲突合并： git merge <branch> 解决冲突 git add <pathspec>   和   git commit -m "..."


git clone github地址  // 自动下载