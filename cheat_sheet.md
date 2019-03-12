mkdir ** 创建文件夹
cd **    前往路径
pwd      显示当前路径
git init  初始化git仓库
git config  全局配置
参数  --global user.name **
      --global user.email "**"

vi/vim命令
i    进入编辑模式
ESC  返回命令模式
:w   保存
:wq  保存并退出
:q!  不保存，强制退出
:e!  强制撤销更改
ZZ   保存退出

cat  **  显示文档内容

git add **  将工作区文件**保存至暂存区
git add .   将工作区所有文件保存至暂存区
git commit -m "**"   将暂存区文件提交，并添加注释
git status  查看git的状态
git diff    查看git修改内容
git log     查看git各个版本
git reflog  查看git历史
git reset --hard **/HEAD^ 版本库回到版本**

ssh-keygen -t rsa -C "email"  创建git公钥
git remote add **(origin) git@github.com:bigdriver/learngit  将当前仓库连接至远程库
git remote -v    查看当前所有连接的远程库
git remote rm **(origin)

git push origin master   推送到origin的master分支

首次推送  git push -u origin master
git clone git@github.com:bigdriver/learngit  克隆远程库至本地库
git branch   查看所有分支和当前分支
git branch **   创建分支**
git branch -d **  删除分支**
git checkout -b **  创建并切换至分支**
git checkout **   切换至分支**


git tag <tag-name>/v1.0  标记当前版本
git tag -d <tag-name>  删除标签
git tag   查看所有标签
git tag v1.0  f52c633 标记版本f52c633
git show v1.0 查看标签信息
git tag -a v1.0 -m "**"   创建带说明**的v1.0标签
git push origin <tagname>  推送一个本地标签
git push origin --tags   推送所有标签

git merge <branch>  合并分支<branch>到当前分支

git stash  藏匿工作内容
git stash list  查看藏匿工作内容列表
git stash apply stash{0}  恢复藏匿内容stash{0}
git stash drop 删除藏匿内容列表
git stash pop 恢复并删除藏匿内容

issue-101  bug分支
feature-101  新功能分支
git branch -D dev 强制删除dev分支

git merge --no-ff -m "**" dev  使用-no-ff模式合并dev分支到当前分支
平时在dev issue-101 feature-101 分支上工作，最后合并至master分支
git remote  查看远程库信息
git remote -v   查看远程库详细信息

git push origin dev  推送dev分支到远程库origin的dev分支上

git pull  拉取远程库分支到本地

git checkout -b branch-name origin/branch-name  在本地创建和远程库同名的分支

git branch --set-upstream branck-name origin/branch-name  |
git branch --set-upstream-to=origin/<branch> <branch>  关联远程库<branch>分支与本地<branch>分支

git merge 发生冲突后，用git status 查看冲突，用vi <file> 修改冲突













