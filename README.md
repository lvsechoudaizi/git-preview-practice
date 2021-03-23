# git 命令
## git init 初始化Git相当将⽂件夹升级为仓库

## git status 查看版本库的状态

## git add README.md 将未跟踪的文件【Untracked】添加到版本库,文件转变为【Add】可提交状态，同时将README文件的快照已经缓存了到暂存盘Staged，若删除该文件，可以从暂存中恢复出来

## git checkout README.md 将文件从暂存盘中检出

## git commit -m '提交注释' 提交代码到本地仓库，命令只能提交暂存区的文件，vscode提交可以一次性执行文件到暂存区并同时提交

## git stash 保存临时工作到栈中（将修改新增的数据全部保存起来，工作目录恢复到未修改之前，这时可以优先处理紧急的工作）

## git stash pop 将栈中弹出工作现场（将之前保存的临时工作弹出）

## git log  查看提交日志记录

## git log --oneline 查看提交的简短日志记录

## git reflog  操作记录 包括回退记录也会被显示

## git reset HEAD@{} 版本回退，不更新工作区

## git reset --hard HEAD@{} 版本回退，并且更新工作区的文件到回退的版本


# git认识

##         |-----------------------------------pull-------------------------------------->|
##         |                                                                              |          
## 1.远程版本库Remote -----fetch/clone------> 2.本地仓库Repository------checkout----> 3.工作区Workspace
##         |                                         |                                        |
##         |<--------------push----------------------|<-----commit----缓存区Staged <---add----|    

# git分支管理 --branch

## git checkout -b develop 创建develop分支并切换分支到develop

## git checkout master 检出【切换】master分支

## git merge develop 合并分支，将develop分支合并到当前分支

## git merge -d develop 合并develop分支的同时删除develop分支

## git branch 查看分支

## git branch -a 查看分支，包括远程分支

## git branch -d develop 删除develop分支

# git 清洗提交历史--squash方式合并









