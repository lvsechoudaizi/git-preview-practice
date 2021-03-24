# git 命令
#### git init 初始化Git相当将⽂件夹升级为仓库

#### git status 查看版本库的状态

#### git add README.md 将未跟踪的文件【Untracked】添加到版本库,文件转变为【Add】可提交状态，同时将README文件的快照已经缓存了到暂存盘Staged，若删除该文件，可以从暂存中恢复出来

#### git checkout README.md 将文件从暂存盘中检出

#### git commit -m '提交注释' 提交代码到本地仓库，命令只能提交暂存区的文件，vscode提交可以一次性执行文件到暂存区并同时提交

#### git stash 保存临时工作到栈中（将修改新增的数据全部保存起来，工作目录恢复到未修改之前，这时可以优先处理紧急的工作）

#### git stash pop 将栈中弹出工作现场（将之前保存的临时工作弹出）

#### git log  查看提交日志记录

#### git log --oneline 查看提交的简短日志记录

#### git reflog  操作记录 包括回退记录也会被显示

#### git reset HEAD@{} 版本回退，不更新工作区（用的少）

#### git reset --hard HEAD@{} 版本回退，并且更新工作区的文件到回退的版本（用的多，因为版本回退通常都是需要更新工作区文件的）


# git认识

####       |-----------------------------------pull-------------------------------------------->|
####       |                                                   |          
#### 1.远程版本库Remote -----fetch/clone------> 2.本地仓库Repository------checkout----> 3.工作区Workspace
####         |                                         |                                        |
####         |<--------------push-------------------------|<-----commit----缓存区Staged <---add----|    

# git分支管理 --branch

#### git checkout -b develop 创建develop分支并切换分支到develop

#### git checkout master 检出【切换】master分支

#### git merge develop 合并分支，将develop分支合并到当前分支

#### git merge -d develop 合并develop分支的同时删除develop分支

#### git branch 查看分支

#### git branch -a 查看分支，包括远程分支

#### git branch -d develop 删除develop分支

# git 清洗提交历史--squash方式合并

#### git merge --squash develop 使用squash方式合并代码，只是合并不commit【合并develop时会有很多commit记录信息一起被保留下来，使用squash将不会保留commit信息，只是简单的合并代码，并且合并的代码没有提交，将所有develop的提交整合到了暂存区，需要我们自己执行Commit, 这样保证主分支的提交记录干净整洁】


# git 标签管理（标签管理就是给自己的代码打上版本标记。其实就是给自己的版本设置里程碑。）

#### git tag 查看打标签

#### git tag v1.0  将最新提交打上标签v1.0

#### git tag v1.0 4854541 将指定的commit记录打上标签

#### git show v0.9 查看与v0.9标签之间的差距


# git 远程仓库
### 1.Github 世界上最大的开源社区/2.Gitee 国内速度快/3.GitLab 私有的远程仓库

#### 添加远程分支
##### git remote add origin git@github.com:lvsechoudaizi/git-preview-practice.git

#### git push  推送本地仓库代码到远程仓库

#### git pull 拉取远程仓库代码到工作区（fetch/）

#### git fetch 拉取源（远程仓库的内容拉回到本地仓库）

#### git clone 拉取 （本地仓库不存在的情况下，远程仓库的内容一比一的克隆复制到本地，产生本地仓库）







