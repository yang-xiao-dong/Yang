# Git入门操作



+ 初始化

```bash
git init
```



- 设置提交你提交改动时使用的个人信息，只需要在安装完Git设置一次

```bash
git config --global user.name "name "
git config --global user.email "email "
```



- 添加文件,他会将指定的文件纳入一个交暂存区“staging area",可以把它想象成一辆小车。把运往仓库里存的东西都放到里面。

```bash
git add 文件名.拓展名
```



- 当前文件夹下所有文件

```bash
git add    .
```



+ 只把html文件存入，使用通配符

```bash
git add #.html
```



+ 显示存入暂存区的文件以及修改但还未放入暂存的文件

```bash
git status
```



+ 将指定文件移除缓存区

```git
git reset filename.extension
```



+ 将指定文件移除缓存区,并把文件标记为未跟踪

```bash
git rm --cached filename.extension
```



+ 把暂存的文件提交到你的本地仓库。在括号中可以写一些简单的描述和备注，保证以后的查阅

```bash
git commit -m "描述和备注"
```



+ 创建.gitignore文件，用来让git忽略一些无需记录跟踪的文件，任意编辑器打开，将不需要加入仓库的文件或者文件夹，写道里面。

```bash
touch .gitignore
```



创建分支，以便在不影响原来代码的情况下，进行一些修改

```bash
git branch 分支名
```



+ 从仓库中取出之前创建的某条分支上的代码，以进行修改，上传，删除。

 ```bash
git checkout "brachname"
 ```



+ 在master分支中，执行这条命令将会将之前提交过的那条分支里的改动合并到主仓库

```bash
git merge brachname
```



+ 将本地仓库提交到Github网站

```bash
git remote add origin https://github.com/yang-xiao-dong/Yang.git
```



+ 列出和项目相关联的远程仓库

```bash
git remote
```



+ 将本地仓库中的内容推送到远程仓库中指定分支，默认是master

```bash
git push -u origin master
```

之后就可以只写`git push`



+ 下载仓库到本地

```bash
git clone https://github.com/yang-xiao-dong/Yang.git
```



+ 如果是和多人一同修改代码库，可以将本地代码库同步到最新状态

```bash
git pull
```





