### Git语法
#### 本地仓库
##### 创建版本库
```
$ mkdir <name>
$ cd <name>
$ pwd 
```
##### 初始化仓库
```
$ git init
```
##### 添加到暂存区
```
$ git add <filename>
```
##### 提交到仓库
```
$ git commit -m "message"
```
##### 查看运行状态
```
$ git status
```
##### 查看修改内容
```
$ git diff <filename>
```
##### 查看命令日志
```
$ git log    # 最近到最远的提交日志
$ git log --pretty=oneline  # 显示一行信息
```
##### 版本回退
```
$ git reset --hard HEAD^   # 回退到前一个版本
$ git reset --hard HEAD^^   # 回退到前两个版本
$ git reset --hard HEAD~100   # 回退到前一百版本
```
##### 查看文件内容
```
$ cat <filename>
```
##### 版本恢复
```
$ git reset --hard <commit id>  # commit id可以在log中查找
```
##### 记录命令
```
$ git reflog
```
##### 撤销工作区修改
```
$ git checkout -- <filename>
$ git restore <filename>
```
##### 撤销暂存区修改
```
$ git reset HEAD <filename>
$ git restore --staged <filename>
```
暂存区修改撤销后工作区修改仍然存在
##### 移除文件
```
$ rm <filename>
```
##### 从版本库中删除
```
$ git rm <filename>
$ git commit -m "message"
```
误删可以使用撤销修改的命令还原
##### 创建SSH密钥
```
ssh-keygen -t rsa -C"email adress"
```
##### 连接远程仓库
```
$ git remote add <name> <SSH>
```
##### 本地库推送到远程库
```
$ git push -u <name> master
# 第一次推送加-u 后续可以简化命令
$ git push origin master
```
##### 查看远程库信息
```
$ git remote -v
```
##### 删除远程库
```
$ git remote rm <name>
```
##### 克隆远程库到本地
```
$ git clone <SSH>
```
##### 查看分支
```
$ git branch
```
##### 创建分支
```
$ git branch <name>
```
##### 切换分支
```
$ git checkout <name> 或者 $ git withch <name>
```
##### 创建+切换分支
```
$ git checkout -b <name> 或者 $ git switch -c <name>
```
##### 合并分支到当前分支
```
$ git merge <name>
```
##### 删除分支
```
$ git branch -d <name>
```
##### 分支合并图
```
$ git log --graph
```

