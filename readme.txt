Git is a version control system.
Git is free software.
I'm learning git.

设置用户名：git config --global user.name"your name"
设置Email：git config --global user.email"email name"
创建目录：mkdir name
退回目录：cd name
显示当前目录：pwd

把目录变成git可管理的仓库：git init
添加文件到仓库：git add 文件名
提交文件到仓库：git commit
掌握仓库当前的状态:git status
查看具体修改内容：git diff

查看历史记录：git log
回退版本：git reset --hard HEAD^
恢复回退的版本：git reset --hard 版本号
记录每一次记录：git reflog
把readme.txt文件在工作区的修改全部撤销：git checkout --文件名
删除一个文件：git rm 文件名
版本库里的版本替换工作区的版本：git checkout -- 文件名

创建SSH key：ssh-keygen -t rsa -C "邮箱名称"
本地关联远程数据库：git remote add origin git@git.oschina.net:yanglijing2015.com/testGit.git
git@git.oschina.net:yanglijing2013/newFile.git
git@git.oschina.net:yanglijing2013/helloWord.git

将本地数据推送到远程仓库中：git push -u origin master(注意本地仓库名称一定跟远程仓库名称相同)
将远程仓库中的数据下载到本地仓库：git clone  git@git.oschina.net:yanglijing2015.com/gitSkills.git

创建并切换分支：git checkout -b 分支名称
查询所有分支：git branch
切换分支：git checkout 分支名称
合并指定分支到当前分支：git merge dev
删除分支：git branch -d 分支名称
合并分支：git merge 分支名称

合并分支禁用Fast forward：git merger --no-ff -m "注释" dev
 把当前现场“储存起来”：git stash
查看工作现场列表：git stash list
恢复现场：1  git stash apply  stash内容并不删除，你需要用git stash drop来删除；
          2  git stash pop  恢复的同时把stash内容也删了
强行删除分支：git branch -D 分支名
将分支推送到远程仓库的对应分支上：git push origin 分支名称
抓取最新的提交从远程仓库中：git pull
建立本地分支和远程分支的关联：git branch --set-upstream dev origin/dev
在本地创建和远程分支对应的分支：git checkout -b branch-名字 origin/branch-名字

创建标签：git tag 标签名
查看标签：git tag
对指定的commit打标签：git tag commitId 
创建带说明的标签：git tag -a 标签名 -m "说明" commit的ID
删除标签：git tag -d 标签名
推送标签名到远程：git push origin 标签名
一次性推送所有的标签名：git push origin --tags
从远程仓库删除标签：gitpush origin :refs/tags/标签名


为命令配置别名：git config --global alias.st status


