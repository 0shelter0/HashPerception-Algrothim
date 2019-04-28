### README.MD

作者：Comen Rider ShelterX

Date：2019年4月28日

Notice：转载联系作者，原创不易。

参考文献： https://github.com/wxxhub/my_study/blob/master/git.md

＞＜＞＜

使用git将本地库同步到远程:

```
create a new repository on the command line
echo "# HashPerception-Algrothim" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/0shelter0/HashPerception-Algrothim.git
git push -u origin master

```

###### 使用git将本地库同步到远程:

* 关联一个远程库: `git remote add origin git@server-name:path/repo-name.git`；

* 关联后，`git push -u origin master` ' _**第一次**_推送master分支的所有内容；

* 每次 **本地提交后 **，只要有必要，就可以使用命令`git push origin master`推送最新修改。
* 将库同步到本地库， **git pull origin master**
* remote-->自己机器的仓库 origin-->github的仓库
* 如果origin和remote端同时修改且都保存成功了，要使一方向另外一方同步，则应该合并修改后再同步，具体做法是先pull origin master再push origin master.
