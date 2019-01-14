$ pwd  创建
$ git init 初始化
$ git add readme.txt   把文件添加到仓库(缓存区stage)
$ git commit -m "wrote a readme file"  把文件提交到仓库“注释” -m后面输入的是本次提交的说明（分支master）
                                                           1 file changed：1个文件被改动（我们新添加的readme.txt文件）；
                                                           2 insertions：插入了两行内容（readme.txt有两行内容）。
                                                           需要提交的文件修改通通放到暂存区，然后，一次性提交暂存区的所有修改。
$ git status 命令可以让我们时刻掌握仓库当前的状态，readme.txt被修改过了，但还没有准备提交的修改。

####撤销
$ git checkout -- readme.txt  可以撤销工作区的修改,让这个文件回到最近一次git commit或git add时的状态
$ git reset HEAD readme.txt   把暂存区的修改撤销掉（unstage），重新放回工作区：

####删除
$ git rm test.txt   从版本库中删除该文件，那就用命令git rm删掉，并且git commit：

$ git diff 看具体修改了什么内容，比较的是工作区文件与暂存区文件的区别
$ git diff --cached 比较的是暂存区的文件与仓库分支里（上次git commit 后的内容）的区别
$ git diff HEAD -- readme.txt命令可以查看工作区和版本库里面最新版本的区别：

####版本控制
$ git log  提交历史
$ git log --pretty=oneline 版本号
$ git reset --hard HEAD^ 上个版本   HEAD~10版本号  HEAD指向的版本就是当前版本
$ git reset --hard 1094a    可以还原版本  1094a
$ git reflog 查看命令历史，以便确定要回到未来的哪个版本。

####远程仓库GitHub
$ git remote add origin git@github.com:txte/txt.git    
 远程库的名字就是origin
$ git push -u origin master   本地库的所有内容推送到远程库上， -u参数，会把本地的master分支内容推送的远程新的master分支，本地的master分支和远程的master分支关联起来
$ git push origin master  以后的推送或者拉取时就可以简化命令
