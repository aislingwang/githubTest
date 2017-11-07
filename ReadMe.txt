初步使用git在GitHub上创建仓库的详细步骤

使用GitHub仓库人员：
a.GitHub端
	1> 注册账户以及创建仓库

b.本地
http://www.runoob.com/w3cnote/git-guide.html

	1> 安装git 和 openssh，本地创建ssh key
		$ ssh-keygen -t rsa -C "your_email@youremail.com"
		后面的your_email@youremail.com改为你在github上注册的邮箱，之后会要求确认路径和输入密码，我们这使用默认的一路回车就行。成功的话会在~/下生成.ssh文件夹，进去，打开id_rsa.pub，复制里面的key。
		回到github上，进入 Account Settings（账户配置），左边选择SSH Keys，Add SSH Key,title随便填，粘贴在你电脑上生成的key。
	
	2> 验证是否成功，在git bash下输入：
		$ ssh -T git@github.com

	3> 设置username和email，因为GitHub每次commit都会记录他们
		$ git config --global user.name "your name"
		$ git config --global user.email "your_email@youremail.com"
		
	4> clone仓库
		$ git clone git@github.com:aislingwang/githubTest.git
		
	5> 修改后提交
	6> 添加文件后提交
		
		
		
/////////////////////////////////////////////////////////////////////////////////////////////////////////////



		
创建仓库人员：
a.GitHub端
	1> 注册账户以及创建仓库
		github官网地址：https://github.com/
		Create a New Repository，填好名称后Create，之后会出现一些仓库的配置信息
	
b.本地
http://www.runoob.com/w3cnote/git-guide.html

	1> 安装git 和 openssh，本地创建ssh key
		$ ssh-keygen -t rsa -C "your_email@youremail.com"
		后面的your_email@youremail.com改为你在github上注册的邮箱，之后会要求确认路径和输入密码，我们这使用默认的一路回车就行。成功的话会在~/下生成.ssh文件夹，进去，打开id_rsa.pub，复制里面的key。
		回到github上，进入 Account Settings（账户配置），左边选择SSH Keys，Add SSH Key,title随便填，粘贴在你电脑上生成的key。
	
	2> 验证是否成功，在git bash下输入：
		$ ssh -T git@github.com
	
	3>添加远程地址：
		$ git remote add origin git@github.com:yourName/yourRepo.git
		后面的yourName和yourRepo表示你再github的用户名和刚才新建的仓库，加完之后进入.git，打开config，这里会多出一个remote "origin"内容，这就是刚才添加的远程地址，也可以直接修改config来配置远程地址。
		创建新文件夹，打开，然后执行 git init 以创建新的 git 仓库。
	
	4> 设置username和email，因为GitHub每次commit都会记录他们
		$ git config --global user.name "your name"
		$ git config --global user.email "your_email@youremail.com"
	
	5> 添加文件，提交到远程仓库，推送到远程master分支
		$ git add .
		$ git commit -m “first commit”
		$ git push -u origin master
	
	6> 多人共同开发
		http://blog.csdn.net/song_shui_lin/article/details/52685780