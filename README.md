# 通过github来搭建一个属于自己的免费博客吧！
##一，一切基于目的
搭建属于自己的博客能更加自由，更加独立。“不喜欢被他人约束的精神，从此刻从新定义自己”，以显得够逼格为目的，程序猿必备口粮！
通过github来搭建一个属于自己的免费博客吧！show
##二，安装所需软件
**1，以下为所需：**
Git
Node.js

**2，安装Git和Node.js**
具体可以参考Hexo的官方文档，里面含有不同系统的安装方法，我以window10为例。在安装Node.js时候需要注意，如果安装的是.exe后缀结尾，则需要手动添加环境变量，.msi则不用。
通过github来搭建一个属于自己的免费博客吧！

**3，新版的Node.js已经集成了npm**，所以之前的npm也一并安装好了，当我们分别把Git与Node.js安装好后，通过在cmd命令窗口下分别输入以下命令：“git –version”，“node -v”，“npm -v”来验证是否安装成功！
通过github来搭建一个属于自己的免费博客吧！

Success
##三，注册Github账户
**1，**首先你要注册一个属于你的Github账户，拥有账户的可以忽略，注册过程中所填写的username会被定义为username.github.io，所以希望你还是认真思考，写一个自己喜欢的名字。
通过github来搭建一个属于自己的免费博客吧！Registered account

**2，**注册成功后，邮箱认证。然后登陆账号通过Github创建新的容器，点击New repository。
通过github来搭建一个属于自己的免费博客吧！

Find button
**3，**在Repository name的下方填写username.github.io一定要与左边的Owner名称一致噢。最后，点击Create repository成功创建！
通过github来搭建一个属于自己的免费博客吧！

Registered repository
**4，**因为要启用GitHub，点击Your repositories，进入你的容器：
通过github来搭建一个属于自己的免费博客吧！

Your repositories

**5，**点击右边的Setting菜单进入设置，点击Launch automatic page generator，点击底部的Continue to layouts，最后点击Publish page，发布Github默认生成的静态站点。
通过github来搭建一个属于自己的免费博客吧！

Launch automatic page generator
##四，安装Hexo
**1，**Hexo是一款基于Node.js的静态博客框架，在电脑上面新建一个blog文件夹，该文件夹是用来存放你的博客地址的，然后鼠标右键选择Git Bash。
通过github来搭建一个属于自己的免费博客吧！

New blog

**2，**避免被“墙”，安装Hexo我使用了淘宝的NPM镜像，在打开的命令窗口输入“$ npm install -g cnpm –registry=https://registry.npm.taobao.org”，与原来的npm完全一样的，只是将命令改为cnpm，稍等Hexo的安装完成。
通过github来搭建一个属于自己的免费博客吧！

Complete

**3，**输入以下命令“$ cnpm install hexo –save”，再输入“$ hexo -v”，验证是否安装正确。
通过github来搭建一个属于自己的免费博客吧！

Try

**4，**本地运行Hexo。
初始化“$ hexo init”
安装生成器“$ cnpm install”
运行Hexo“$ hexo s -g”
通过github来搭建一个属于自己的免费博客吧！

Local
打开浏览器，输入“localhost:4000”，看看你在本地的博客地址是否搭建成功了没，可以用Ctrl+C停止的。
##五，博客的配置
**1，将你的博客换新衣，**“$ git clone https://github.com/iissnan/hexo-theme-next themes/next”，我这里只示例了一个目前比较热门的主题，Hexo也有更多的主题供你选择的。

**2，修改配置信息，**打开blog/_config.yml文件，进行配置 ,下面给大家提供一些常用的设置列出来给大家修改, 注意配置的键值之间一定要有空格。更多设置参考这里。
title: kevin的代码人生 //你博客的名字
author: kevin //你的名字
language: zh-Hans //语言 中文
theme: next //刚刚安装的主题名称
deploy:
type: git //使用Git 发布
repo: https://github.com/yujiewong/yujiewong.github.io.git // 刚创建的Github容器

**3，**当所有的基础框架都创建完毕，接下来你可以写文章了。在\blog\source\_posts用Markdown大显生手吧！
title: hello
date: 2015-07-01 22:37:23
categories:
– 日志
– 二级目录
tags:
– hello
—
摘要:
<!–more–>
正文:
4，另外主题的配置是能在、blog/themes/next/_config.yml中修改，这里略过。设置详情可以到theme-next查看。

##六，部署上线
**1，设置你的Git身份信息。**
$ git config –global user.name “你的用户名”
$ git config –global user.email “你的邮箱”

**2，**安装hexo-deployer-git自动部署发布工具，“$ cnpm install hexo-deployer-git –save”。
通过github来搭建一个属于自己的免费博客吧！

Save

**3，**发布更新到你的Github上，“$ hexo d -g”，发布时候需要输入你的Github账号和密码，大功告成。是不是很好玩，试试访问你的”https://username.github.io/”看看效果吧！
每天分享一些自学经验与他山之石，欢迎编程爱好者能添加微信"NetItCeo"，一起坐看风云变幻。
=======
## BuildMyVim
Use zsh,oh my zsh macvim,tmux ...
* 1.安装homebrew 
登陆网站 http://brew.sh/index_zh-cn.html
复制命令到命令行执行 /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
* 2.安装zsh 
brew install zsh
* 3.安装oh my zsh sh 
-c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
* 4.安装macvim 
brew install macvim
* 5.git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
* 6. git clone https://github.com/datamaning/BuildMyVim.git
* 7. mv datamaning/.vimrc ~
* 8. vim .vimrc & :PluginInstall

#end
* 1.brew install wget
* 2.Homebrew 会将套件安装到独立目录，并将文件软链接至 /usr/local 
* 3.cd /usr/local
* 4.find Cellar
* 5.Cellar/wget/1.16.1
* 6.Cellar/wget/1.16.1/bin/wget
* 7.Cellar/wget/1.16.1/share/man/man1/wget.1
* 8.ls -l bin
* 9.bin/wget -> ../Cellar/wget/1.16.1/bin/wget
>>>>>>> f9fd03fa4e8072f8c5ad3418856baed99c853658
