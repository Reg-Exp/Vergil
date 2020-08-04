# Git命令

#####关于提交

``` nginx
git status 查看仓库当前状态
```

```nginx
git add md.js 把一个文件添加到工作区，如果需要提交全部，使用git add .
```

```nginx
git commit -m"提交说明"  把文件提交到仓库
```

```nginx
git push origin 分支名 把代码推送到远程仓库
```

##### 关于合并

```nginx
git fetch 从远程仓库检索出分支
```

```nginx
git merge 分支名  选择分支进行合并
```

##### 关于分支

```nginx
git checkout name 切换到一个分支
```

```nginx
git checkout -b name 创建并切换到一个新的分支
```

```nginx
git branch -a 查看所有分支
```

```nginx
git branch name 创建一个分支
```

```nginx
git branch -d name 删除一个分支
```




```nginx
git init //创建并初始化一个git仓库
```
```nginx
ls -ah  列出当前文件夹的文件
```


```nginx
git diff+文件名 查看修改的内容
```
```nginx
git log 查看提交的历史记录
```
```nginx
git reflog 查看历史提交，查看到版本号 然后使用git reset可以回退版本
```
```nginx
git log --pretty=oneline  以单行显示历史记录
```
```nginx
git reset 回退到上一个版本
```
```nginx
git reset --hard 3rfe(版本号) 回退到指定版本
```
```nginx
cat test.txt（文件名）查看文件内容
```
```nginx
git checkout --文件名 可以丢弃最近工作区提交的内容
```
```nginx
git reset HEAD  文件名  可以丢弃暂存区提交的内容
```
```nginx
git rm 文件名   用于删除一个文件
```
```nginx
$ ssh-keygen -t rsa -C "1069579370@qq.com"    创建ssh key
open  ~/.ssh 找到ssh文件夹 
```
```nginx
git remote add origin git@server-name:path/repo-name.git 关联一个远程库
把本地仓库推送到远程库
```
```nginx
git merge name （在切换到master分支的情况下）合并一个分支到当前分支
```
```nginx
git log --graph --pretty=oneline --abbrev-commit  查看分支合并情况
```
```nginx
git merge --no-ff 不使用快进模式，可以看到历史合并情况
```
```nginx
git stash  存储当前工作区
```
```nginx
git stash apply 恢复工作区
```
```nginx
git stash drop 删除stash
```
```nginx
git stash pop 恢复工作区并删除stash
```
```nginx
git stash apply stash@(0)  恢复指定的stash
```
```nginx
git branch -D <name>  丢弃一个没有被合并过的分支
```
```nginx
git remote -v 查看远程库的信息，如果没有推送权限，就无法看到push地址
```
```nginx
git tag v1.0 给分支创建标签
```
```nginx
git push git dev 给远程仓库创建分支
```
