### 一、创建github账号
![图](https://github.com/bringbird/myFirstRespository/raw/master/image/1.png)

`接着会来到这 `
![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/2.png)

然后会收到一封github发的邮件，进入邮箱验证
### 二、创建个人仓库
验证成功是这样的 !
![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/4.png)

也可以来到个人中心里创建仓库
![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/5.png)
![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/6.png)
![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/7.png)

创建完成好之后是这样子的。创建仓库的时候最好别用中文，不然你的仓库名就会显示 - 这样一条小横线

![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/8.png)

### 三、配置SSH keys
终端里输入显示隐藏文件：defaults write com.apple.finder AppleShowAllFiles -bool true

关闭：defaults write com.apple.finder AppleShowAllFiles -bool true

输入命令完成之后需要重启Finder 桌面顶部苹果logo->强制退出-> 就可显示隐藏文件 


![图](https://github.com/bringbird/myFirstRespository/raw/master/image/9.png)


然后前往个人文件查看有没有 .ssh 文件夹，有的话个人建议删除掉，从新配置 

![图](https://github.com/bringbird/myFirstRespository/raw/master/image/10.png)

来到终端里输入指令：mkdir .ssh 创建一个 .ssh 文件夹 #####cd .ssh 进入刚创建的 .ssh文件夹目录里
输入指令：ssh-Keygen -t rsa -C “youEmail”双引号里填写你的邮箱地址 #####输入完成之后一直按回车键 中间会提示你要输入密码，不用管一直按回车直到出现这样。输入指令：ls -la 查看 如果输出类似这样的信息，就说明配置成功 。

![图](https://github.com/bringbird/myFirstRespository/raw/master/image/11.png)

![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/12.png)

登陆github 进入 SSH keys 添加刚刚拷贝的东西 


![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/13.png)


![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/14.png)

添加完成之后是这样的

![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/15.png)

然后回到终端输入指令：ssh -T git@github.com 执行完这条指令之后会输出 Are you sure you want to continue connecting (yes/no)? 输入 yes 回车 #####回到github，刷新网页就可以看到钥匙旁的灰色小圆点变绿，就表明已经添加成功了。

![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/16.png)

### 四、上传本地项目到github上
上传项目，这里是用的是[github客户端](https://desktop.github.com/)下载好之后输入用户名 邮箱 密码登陆之后clone刚创建的仓库到本

![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/17.png)

接着打开clone到本地的文件夹 将需要上传的项目添加进去，这里以 FirstRespository 这个文件夹为例。

![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/18.png)

回到github客户端 

![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/19.png)


然后点击右上角的![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/20.png)按钮提交完成之后到仓库的首页刷新即可看到上传成功！ 

![图](https://raw.githubusercontent.com/bringbird/WJFirstRespository/master/image/21.png)


# [恭喜你，已经成功的上传项目到自己的仓库了](https://github.com/gugejun/luan/wiki)

