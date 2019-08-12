# [ENGLISH](https://hexoscript.gitbook.io/hexo-script/)

# [hexo-script-win]更新日志

* v1.3- 2019-08-12

### v1.3更新内容

- 增加自动安装部署必备插件
- 修复无法更新的错误
- 优化内部版本获取

## 往期版本更新内容

v1.2更新内容

- 1.优化更新脚本
-  2.重改了安装命令，提升执行能力
-  3.取消低版本安装最新版的命令，使脚本更加兼容，避免低版本运行新版本命令不一致的错误

v1.1更新内容

- 修复无法执行安装hexo博客的错误
- 优化安装脚本
- 增加版本检测更新和帮助功能
- 优化上传部署功能，加入检测目录机制
- 修复生成SSH秘钥脚本的错误

v1.0原功能

- 检测node环境
- 检测git环境
- 一键安装hexo博客
- 生成SSH秘钥
- 一键上传部署博客

***

# **准备工具**

# Git工具

本脚本所有测试均在git bash上运行，建议使用git工具运行最佳。下载地址：

> Git官网下载：https://git-scm.com/
>
> 国内镜像下载：https://npm.taobao.org/mirrors/git-for-windows/v2.22.0.windows.1/Git-2.22.0-64-bit.exe
>
> 国内其他版本下载：https://npm.taobao.org/mirrors/git-for-windows/



建议使用国内镜像下载，速度最快！

下载后请自行安装

# Node.js

您需要安装node.js才能使用和安装hexo博客，无论是使用和不使用本脚本，都是必须安装的，下载地址：

> http://nodejs.cn/download/



建议使用安装程序进行安装。安装时，请勾选**Add to PATH**选项。

# 下载[hexo-script]的安装脚本

你只需要在某个目录下,打开git bash然后执行下面这条命令即可下载完成



```
curl -O https://cdn.jsdelivr.net/gh/kjhuanhao/hexo-script@master/install.sh
```

**我们更建议直接在**[**releases**](https://github.com/kjhuanhao/hexo-script/releases)**下载,选择最新版本,只需下载install.sh即可**

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-Llz5MvUaxJN5PhxsYY1%2F-Llz6JJCocpELXFXMiCv%2F66.png?alt=media&token=37c066e7-e963-42ff-adf5-10ad0dec770f)

install.sh



建议新建一个目录存放此安装脚本,最好是你想存放博客文件的地方.

如图:我创建了一个[myblog]文件夹,然后在此文件夹下右键打开git bash

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LluijETOwVdISk9cx63%2F-LlujpjLExHk7K73O-Gb%2F1.png?alt=media&token=19632c44-33dd-4025-a8e5-2042e219ff98)



然后运行了下载命令,安装脚本(install.sh)就会下载在你的当前文件夹中

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-Llujyttm0BWO_RMRg-2%2F-LlukgEwkesx8NRKmBdo%2F2.png?alt=media&token=ec7c6fd6-108a-4161-a3d5-1a67438fa83d)



***

# **检测node.js环境**

## test_node的使用

在存放install.sh脚本的目录中,右键打开git bash然后运行以下命令:

```
source install.sh test_node
```

如果出现了如图的情况证明环境变量是配置成功的

(出现了版本号和成功的提示信息代表配置成功)

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-Llul9Kdh1NJmVlnXuGd%2F-Llum1fgCUk0Unm0jlVo%2F3.png?alt=media&token=6a788601-ff5f-4f61-8862-7b179074e1c2)

如果你并发现有版本号的出现,而是红色的错误信息,你可能需要手动配置node.js的环境变量,或者重新安装node.js并注意勾选**Add to PATH**

***

# **检测git环境**

检测git环境

## test_git的使用

如果你想要检测git环境或者查看当前git的版本号,您可以在存放install.sh脚本的目录中,右键打开git bash运行以下命令:



```
source install.sh test_git
```



 一般情况下安装git工具后git环境是会自动配置的,可以无需检测git环境.此脚本可以用于linux系统,出现版本号信息则配置为成功.

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LluoKobHnM4js5SYkdo%2F-LluomhR8g4MupDKuwDk%2F4.png?alt=media&token=1e951d48-85c8-4abf-8d2e-ea48727dd5bb)

***

# **一键安装hexo博客**

自动完成全部安装过程并生成博客文件

## hexo_win的使用

您需要在存放install.sh脚本的目录中,右键打开git bash运行以下命令:



```
source install.sh hexo_win
```



 提示:此时你可以去来一杯卡布奇诺,大约两分钟的时间,博客即可自动安装完成,如图:

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LluplfJDETDQ1wIHNxR%2F-LlupnWqOZVWU6iL3uK9%2F5.png?alt=media&token=30690ad9-b4fb-4240-ad96-1ea7686d888c)

完成图



当您看到出现`Please run hexo s to check it out!`的提示,证明您已经安装成功,此时你可以运行hexo s 然后查看你的博客



```
cd hexobloghexo s
```



注意:要先cd到hexoblog目录哦!执行以上命令即可

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LluplfJDETDQ1wIHNxR%2F-LluqmWs7L0rHAJhJkR-%2F6.png?alt=media&token=88e71510-22da-4c59-bd41-1d7bb2909436)

本地预览

可以看到出现了一段地址:[http://localhost:4000](http://localhost:4000/)

> 在浏览器访问:[http://localhost:4000 ](http://localhost:4000/),你就可以在本地预览了,浏览情况如图:

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LluplfJDETDQ1wIHNxR%2F-LlurN1aku8F_ZGR35Av%2F7.png?alt=media&token=c9b96207-b162-43de-839b-1837d1241566)

# **一键生成SSH秘钥**

部署hexo博客的必要之物

## git_ssh的使用

您需要在存放install.sh脚本的目录中,右键打开git bash运行以下命令:



```
source install.sh git_ssh
```

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LlyrhN541A0nwXokcle%2F-Llysn3EaGuJyGT8TerP%2F33.png?alt=media&token=444ef29f-36ca-44f6-b935-92d8f0883dfe)



可以看到会有四条可执行命令,输入对应数字可以执行对应的命令

> 1)Key
>
> 2)SSH
>
> 3)Verify-github
>
> 4)Verify-coding



> 1)Key 执行1后可以一键生成秘钥

如果你的电脑已经存在秘钥,程序将会自动退出



> 2)SSH 执行2后可以查看你电脑中已生成的秘钥]



> 3)Verify-github 执行3后可以检查秘钥是否配置github成功



> 4)Verify-coding 执行4后可以检查秘钥是否配置coding成功



> 生成秘钥后别忘记将秘钥添加到账号里,否则秘钥不会配置成功

***

# **一键部署hexo博客**

一键上传到你的github或者coding

## up.sh的使用



在这之前你需要确认你已经配置了SSH秘钥, 如果没有, 具体操作可以看一键生成SSH秘钥教程, 它在上一篇.

您需要在存放install.sh脚本的目录中,右键打开git bash运行以下命令:



```
source install.sh deploy
```

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LlurwQcZHGhMvMGz358%2F-LlutGTSONJsGgLT-HB3%2F8.png?alt=media&token=6b16f0f3-aaa4-4083-960c-e41031408d1a)

下载up.sh



你需要将up.sh复制到hexoblog文件,也就是复制到你的博客根目录下

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LluvTLNmEKB-I1ZDiSA%2F-LluzdSM_MrB7O9qCs1Z%2F9.png?alt=media&token=bce8b33c-c6ec-4242-80fb-a0ac97e99d1a)



然后在存放up.sh脚本的目录中,右键打开git bash运行以下命令:



```
source up.sh
```



之后即可自动部署到你的github或者coding上



如果上传失败你需要检查是否安装的是最新版本的[hexo-script] ,或者在根目录配置了deploy信息.



如果你不会配置,可以看下面的教程:

# **部署博客必要的配置**

首先你需要打开根目录配置文件_config.yml

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LluvTLNmEKB-I1ZDiSA%2F-LluxHhrwiYvRhAnlHXs%2F11.png?alt=media&token=e5ccc9e5-a30f-4a56-86de-4bced0dae279)



> 找到deploy,它一般在最后一行,按照以下的格式修改即可

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LluvTLNmEKB-I1ZDiSA%2F-LluyCdpQ92nd8tuqn9Z%2F22.png?alt=media&token=05f14980-032b-4997-b2b2-9bb31c28332d)





你只需要修改repo后面的信息即可



```
deploy:  type: git  repo: 这里填你的仓库地址,建议使用SSH地址,它是以git开头的  branch: master
```

在1.3版本的[heox-script]后你无需自己安装上传插件,但如果报出了not found git的错误证明上传插件没有安装成功,你需要执行以下命令



```
cnpm install hexo-deployer-git --save或者是npm install hexo-deployer-git --save
```

***

# **版本查看和升级**

## version和update的使用

您需要在存放install.sh脚本的目录中,右键打开git bash运行以下命令:



```
source install.sh version
```



之后便会提示你当前的版本和最新版本

![img](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LlpfTEtpw-XHjloYx-t%2F-LlyuKtrtLXzDhNesCyR%2F-LlyyYM--o3GG4n15z90%2F55.png?alt=media&token=217f021e-cec3-4df4-8164-8904abef55f2)



如果出现了蓝色的文字提示证明当前是最新版本

如果出现了红色的文字提示证明当前不是最新版本,你需要升级一下

您需要在存放install.sh脚本的目录中,右键打开git bash运行以下命令:



```
source install.sh update
```



> 执行之后当前目录会下载一个压缩包,压缩包中的文件便是最新的版本,请解压后使用