# myFirstGitTest
a test for git

Git能进行的操作很多，先主要了解

- 绑定本地与远程git仓库
- 创建/切换/删除分支
- commit提交
- push推送
- 合并分支
- 撤销合并

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



##### 1.5 克隆

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

##### 2.4 提交代码/暂存

提交的文件必须已纳入版本控制， git add 命令告诉 Git 开始对这些文件进行跟踪

```
git add *.c
git add README
```

```shell
git commit -m '提交描述descrp' 以m分支提交
```

> **注：** 在 Linux 系统中，commit 信息使用单引号 **'**，Windows 系统，commit 信息使用双引号 **"**。

##### 2.5 推送代码/请求合并

```shell
git push origin master		origin 是远程仓库的别名，master 是要推送的本地分支名称
```

推送代码前必须先commit

##### 2.6 合并分支

推送代码后需要合并才会覆盖

```shell
git merge (branch)	合并指定分支到当前分支
```

合并并不会删除当前分支，可以继续在当前分支工作与合并

##### 2.7 删除分支

```
$ git branch -d name
```

# 我首个Git尝试

A test for Git

Git offers a variety of operations; initially, let's focus on:

- Connecting local and remote Git repositories
- Creating, switching, and deleting branches
- Committing changes
- Pushing commits
- Merging branches
- Reverting merges

🎉🎆🎇🎄🎊

### 1 Repository Operations

#### 1.1 Designating the current directory as a Git repository

To use the current directory as a Git repository, simply initialize it.

```shell
git init  	// This command will create a hidden `.git` directory in the current directory after execution.
```

For using a specified directory as a Git repository:

```shell
git init newrepo
```

After initialization, a `.git` directory will appear within the `newrepo` directory, containing all data and resources required by Git.

#### 1.2 Connecting local and GitHub repositories

```shell
git remote add origin https://github.com/wobukewu/git-test.git
```

#### 1.5 Cloning

```shell
git clone <repo> <directory>  // Clone the repository at <repo> address to the local directory <directory>
```

### 2 Branch Management

Nearly every version control system supports branches in some form, where a branch represents an independent line of development.

Using branches means you can diverge from the main development line and continue working without affecting it.

In Git, branches are essentially pointers to snapshots of changes.

Git's branching model is often referred to as its **killer feature**, setting it apart from other version control systems.

#### 2.1 Listing branches

```
git branch
```

#### 2.2 Creating a branch

```
git branch (branchname)    // You'll switch to this newly created branch immediately after creating it
```

#### 2.3 Switching branches

```
git checkout (branchname)
```

When switching branches, Git replaces the contents of your working directory with the snapshot pointed to by the last commit on that branch, meaning multiple branches don't require separate directories.

#### 2.4 Staging/Pushing code

Files to be committed must be under version control. The `git add` command tells Git to start tracking those files.

```shell
git add *.c
git add README
```

```shell
git commit -m 'commit description descrp'  // Commit with message using the `-m` option
```

> **Note:** In Linux systems, commit messages should be enclosed in single quotes **'**. In Windows systems, commit messages should be enclosed in double quotes **"**.

#### 2.5 Pushing code/Making a merge request

```shell
git push origin master     // 'origin' is an alias for the remote repository, and 'master' is the name of the local branch to be pushed
```

Pushing code requires a prior commit.

#### 2.6 Merging branches

After pushing code, merging is necessary to incorporate changes.

```shell
git merge (branch)        // Merge the specified branch into the current branch
```

Merging does not delete the current branch; work can continue and further merges can be performed.

#### 2.7 Deleting a branch

```shell
$ git branch -d name
```





