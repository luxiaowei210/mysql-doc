# git的安装
在linux中输入git安装命令：sudo apt-get install git 进行git的安装。

# git的基本命令
* mkdir myweb（创建一个目录）
* cd myweb（进入myweb目录）
* git init（将当前目录（myweb）转化为git仓库）
* ls （查看当前目录（myweb）或仓库下的文件（不包括隐藏文件））
* ls -al （查看当前目录（myweb）或仓库下的所有文件（包括隐藏文件））
* touch demo（创建一个名为demo的文件）
* vim demo（在demo中编辑）
* git status（查看当前目录下的文件状态）
* git add demo（把demo文件加到仓库中）
* git add .（将当前目录下的所有文件加到仓库中）
* git commit（提交）
* git config --global user.name（配置用户名）
* git config --global user.email（配置用户邮箱）
* git config --global core。editor vim（配置提交信息的编辑器为vim）
* git log （查看提交的信息）
* git reflog(查看最后一次提交的CommitID)
* git rm 文件名（从库中删除文件）
* git diff（版本间对比）
* git format-patch -p1（git生成patch）
* git am patch-name（git打patch）
