﻿# git_study
用来git的相关学习

Git的思想和基本工作原理

    git完全可以在本地玩转。在本地建立并初始化一个库，作为远程库（服务端），然后在本地（客户端）通过git clone 命令拉取文件（就如同从https//github.com上拉取），git push 命令上传文件。
    git和gitub不是同一个东西。git的作为一个工具，而GitHub和Conding.net等。。不同库都可以用git的命令来操作管理不同库。
    可以和SVN作个比较，有客户端和服务端。

git的使用：
1.登录 https//github.com/ 注册Github账号，并创建一个repository.
	HTTPS : https://github.com/账号名/仓库名.git
	SSH : git@github.com:账号名/仓库名.git
	Subversion : https://github.com/账号名/仓库名.git
2.安装git
3.生成ssh-key的私钥和公钥
	ssh-keygen -t rsa  //一路回车
注：Windows下使用git bash操作命令行
4.ssh 在github中的设置
	将public key(id_rsa.pub)内容拷贝到GitHub服务器的SSH Keys中。Account setting -> SSH Keys
5.上传文件到GitHub中建立的仓库
	git init
	git add .
	git commit -m ''
	git remote add origin https://github.com/wuhuamian/git_study.git
	git push origin master
配置全局用户名和邮箱
	git config --global user.name "xxx"
	git config --global user.email "xxx@xxx.com"

从远程仓库中拉取本地工作区没有的文件
git checkout -- file 撤销对工作区修改；这个命令是以最新的存储时间节点（add和commit）为参照，覆盖工作区对应文件file；这个命令改变的是工作区

删除远程仓库上 本地没有的文件
git reset HEAD <file> 清空add命令向暂存区提交的关于file文件的修改（Ustage）；这个命令仅改变暂存区，并不改变工作区

从仓库里clone代码
	git clone https://github.com/wuhuamian/git_study.git

   