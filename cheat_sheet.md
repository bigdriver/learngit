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

git add **  将工作区文件保存至暂存区
git commit -m "**"   将暂存区文件提交，并添加注释
git status  查看git的状态
git diff    查看git修改内容
git log     查看git各个版本
git reflog  查看git历史
git reset --hard **/HEAD^ 版本库回到版本**

ssh-keygen -t rsa -C "email"  创建git公钥
git remote add **(origin) git@github.com:bigdriver/learngit  将当前仓库连接至远程库
git push origin master   推送到origin的master分支
首次推送  git push -u origin master
git clone origin git@github.com:bigdriver/learngit  克隆远程库至本地库
git branch   查看所有分支和当前分支
git branch **   创建分支**
git checkout -b **  创建并切换至分支**
git checkout **   切换至分支**







