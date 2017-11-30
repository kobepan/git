# git1

## git基本操作流程
### 首先将所需要git的文件放在一个文件夹中，随后用git bash here打开命令行。首先要使用git init命令初始化git仓库，当然这个库是空的，文件夹中的文件还没有追踪。可以利用git status命令查看当前文件夹还没有被commit的文件的文件状态，是Untracted（位于工作区Working directory），随后利用git add index.html（多文件可用 git add  .(这里有空格) ）之类的命令将文件追踪文件，该added的文件处于待提交的状态staged（位于暂存区Staging index），再然后可以使用git commit -m "some infomation"（这里commit会将所有在staged文件commit）就可提交commited（Repository）。特别注意在commit命令可能会出现错误，计算机不知道我们是谁，这个时候就可以使用git config --global user.name KBPAN 和git config --global user.email ...来完善信息。随后可以使用git config --list命令查看完善的信息。这个时候再去commit就可以了。在commit后可以用git log查看commit记录。当某一个文件被修改，此时该文件自动被设置为modified，此时就可以依然使用git add操作，或者直接git commit -am "come info"。




