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

   