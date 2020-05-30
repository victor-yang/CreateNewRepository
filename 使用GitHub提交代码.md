#### 使用GitHub提交代码

##### 安装Git和TortoiseGit

在官网https://gitforwindows.org/和https://tortoisegit.org/download/分别下载对应版本和操作系统的Git（命令行）和TortoiseGit（图形界面），先安装Git再安装TortoiseGit

安装TortoiseGit后需要配置SSH Client:

![image-20200531000455432](.\image-20200531000455432.png)

##### 配置Git

###### 本地配置

1）配置用户名

打开Git Bash，在命令行输入git config --global user.name "your name"

2）配置邮箱

在命令行输入git config --global user.email "your email"

使用git config -l命令检查user.name及user.email是否配置正确

###### 添加公钥

SSH协议是一种非常常用的Git仓库访问协议，使用公钥认证、无需输入密码，加密传输，操作既便利又保证了安全性。公钥是iSource识别用户身份的一种认证方式，通过公钥，可以将本地git项目与iSource建立联系，然后就可以很方便的将本地代码上传到iSource，或者将iSource代码下载到本地了。

1）生成公钥

运行Git Bash，在命令行输入ssh-keygen -t rsa -C "your email"

一直回车直到结束，公钥将存储在默认地址下：C:\Users\用户名\\.ssh  打开id_rsa.pub文件，将里面的公钥复制下来

2）添加公钥

登录github -> settings -> SSH and GPG keys -> New SSH key 输入title并把上一步复制的公钥粘贴进key中

##### 新建代码仓库

![image-20200531000105570](.\image-20200531000105570.png)

##### 新建MR

###### Clone代码仓到本地

1)进入新建好的代码仓，复制代码仓的SSH链接

![image-20200531000618358](.\image-20200531000618358.png)

2)本地新建文件夹，鼠标右键选择Git Clone

![image-20200531000829321](.\image-20200531000829321.png)

###### 本地新增文件

###### 提交文件

