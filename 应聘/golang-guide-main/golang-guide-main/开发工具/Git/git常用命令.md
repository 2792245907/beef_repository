##辅助操作

git -v ：查看git版本

git config user.name yourName ：指定使用当前仓库的用户名

git config user.email yourEmail ：指定使用当前仓库的用户email

git config --global user.name yourName ：指定全局用户名

git config --global user.email yourEmail ：指定全局用户email

git config list ：查看已有配置信息

git status ：查看当前仓库状态，显示有变更的文件

git log (--oneline)：查看git提交日志，每条提交用一行显示

##仓库操作

git init ：初始化本地git仓库

git clone URL (repositoryName)：克隆远程仓库，并指定拷贝后的本地仓库名

git push URL(或配置文件中指定的远程仓库名) ：把当前仓库推送到远程仓库

git pull URL(或配置文件中指定的远程仓库名) ：把远程仓库的更新内容拉取下来

##文件操作

git add fileName ：把指定文件从工作区放到暂存区

git commit -m Comment：把暂存区文件全部提交到本地仓库,-m后面代表描述信息

git rm --cached fileName ：把暂存区的指定文件撤回工作区

git restore fileName ：撤回工作区中对文件的修改

git reset --hard 版本号 ：仓库版本回退到指定版本号（中间的提交记录会丢失）

git revert 版本号 ：仓库回退到指定版本的前一个版本（中间的提交记录不会丢失，等于创建一条新的提交记录）

##分支操作

git branch branchName ：创建分支，指定分支名

git branch -v ：查看当前具备的所有分支，以及当前所在分支

git checkout branchName ：切换到指定分支

git checkout -b branchName ：创建新分支并切换到该分支

git branch -d branchName ：删除指定分支

git merge branchName ：把指定分支合并到当前分支

##标签操作

git tag ：查看当前有哪些标签

git tag tagName 版本号 ：给某一次提交的版本号打上标签

git tag -d tagName ：删除标签
