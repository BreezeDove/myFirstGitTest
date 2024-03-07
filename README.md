# myFirstGitTest
a test for git

🎈🎆🎇🎄🎊

### 1 仓库操作

##### 1.1 指定当前目录为git仓库

使用当前目录作为 Git 仓库，我们只需使它初始化。

```
git init  		该命令执行完后会在当前目录生成一个 .git 目录。
```

使用我们指定目录作为Git仓库。

```
git init newrepo
```

初始化后，会在 newrepo 目录下会出现一个名为 .git 的目录，所有 Git 需要的数据和资源都存放在这个目录中。

##### 1.2 绑定本地与github仓库

```shell
  git remote add origin https://github.com/wobukewu/git-test.git
```

##### 1.3 提交

提交的文件必须已纳入版本控制， git add 命令告诉 Git 开始对这些文件进行跟踪

```
git add *.c
git add README
```

```shell
git commit -m '提交描述descrp' 以m分支提交
```

> **注：** 在 Linux 系统中，commit 信息使用单引号 **'**，Windows 系统，commit 信息使用双引号 **"**。

##### 1.4 克隆

```shell
git clone <repo><directory>  克隆<repo>地址的仓库到本地目录<directory>
```

### 2 分支管理

几乎每一种版本控制系统都以某种形式支持分支，一个分支代表一条独立的开发线。

使用分支意味着你可以从开发主线上分离开来，然后在不影响主线的同时继续工作。

![img](https://static.jyshare.com/images/svg/git-brance.svg)

Git 分支实际上是指向更改快照的指针。

有人把 Git 的分支模型称为**必杀技特性**，而正是因为它，将 **Git** 从版本控制系统家族里区分出来。

##### 2.1 列举分支

```
git branch
```

##### 2.2 创建分支

```
git branch (branchname)	会在创建分支后立即切换到该分支下
```

##### 2.3 切换分支

```
git checkout (branchname)
```

切换分支的时候，Git 会用该分支的最后提交的快照替换你的工作目录的内容， 所以多个分支不需要多个目录。

##### 2.4 合并分支

```
git merge 
```

合并并不会删除当前分支，可以继续在当前分支工作与合并

##### 2.5 删除分支

```
$ git branch -d name
```

