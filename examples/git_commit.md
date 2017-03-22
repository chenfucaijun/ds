# GitHub交作业流程 for windows
## 1.注册账号
 * 如果你还没有Github账号，请去[Github](https://github.com/)注册并登录

## 2.安装Git
> github是一个代码存放网站，如果进行克隆、提交代码等操作，要使用Git工具

 * Windows安装Git
  * 进入[git官网下载](https://git-scm.com/downloads),选择对应系统版本下载
 ![Markdown](http://i2.buimg.com/576036/e80424e5ae6eaa9d.png)

## 3.使用Git
* windows下找到安装后的Git（bash是Linxu的命令行终端，CMD是windows的命令行终端，GUI是图形化界面）
![Markdown](http://i2.buimg.com/576036/b0e48ba676baafcc.png)
* 我选择的是Git Bash终端,它可以使用基本的Linux系统指令
* mac和linux系统自带终端，基本指令基本相同，如果出现权限的问题，请使用`sudo`执行命令，比如`sudo git clone https://github.com/chenfucaijun/ds.git`

## 4.fork仓库，克隆仓库
* 进入老师的仓库，点击fork(分支)
![Markdown](http://i2.buimg.com/576036/20969aac1c310025.png)

* fork完之后，你会有一个和老师一样的仓库，它的位置在"username/ds"下，我的username是chenfucaijun，如下图
![Markdown](http://i2.buimg.com/576036/62ae4eccedba8767.png)
* 克隆仓库
 * 点击"clone or download"会出现仓库的地址，复制该地址，进入“git bash”
 * 输入`git clone https://github.com/chenfucaijun/ds.git`进行代码克隆
![Markdown](http://i2.buimg.com/576036/91d27bf75ab2edbe.png)

## 5.进入到ds目录新建作业文件
* 方法1：打开git bash命令行中进入ds目录，进入文件夹```cd  2017-1```,在其中新建文件夹（命名为姓名拼音首字母或英文昵称）```mkdir cfcj```,新建程序文件```touch 2-12.cpp```,如下图：

> 常用linux命令介绍：
> 
> * cd 进入目录 cd ..返回上一级目录
> * ls 查看当前目录有哪些文件
> * mkdir 新建目录
> * touch 新建文件
> * pwd 查看当前路径

![Markdown](http://i2.buimg.com/576036/633eeac7a4a2c815.png)
* 如果你熟悉vim操作的话，你可以继续使用命令行进行文件编辑，如果不熟悉，你可以直接进入你的ds目录新建文件夹和文件，如方法2

* 方法2：图形界面进入目录中,使用`pwd`查看ds目录在哪里
![Markdown](http://i4.buimg.com/576036/f7d4ea09ac945133.png)
  * 对应的windows目录就是在`C:\Users\Caijun\ds`
![Markdown](http://i4.buimg.com/576036/7729ef082bb7facd.png)


## 6.代码提交
> 基本的git操作
> 
> * git status 查看仓库的状态
> * git add 添加内容到暂存区
> * git commit -m "the commit
 message" 提交当前内容到本地分支
> * git push 将本地分支的内容，推送到远程主机

* 如下图：
![Markdown](http://i2.buimg.com/576036/f9898fba13b484a6.png)
* 注意：第一次提交的时候要配置你的邮箱和用户名 

  ```
  git config --global user.name "chenfucaijun"
   
  git config --global user.email chenlei163mail@163.com
  ```
   
  
## 7.pull request
* 在CUCCS/ds中新建一个pull request
![Markdown](http://i2.buimg.com/576036/ccdd6b46adbcef3e.png)

* 比对差异
![Markdown](http://i4.buimg.com/576036/18f1a903f14148c9.png)

* 选择比对对象，base fork:你fork的自己的仓库，我的是chenfucaijun/ds
![Markdown](http://i4.buimg.com/576036/dff2e94384719266.png)

* 选择比对对象，head fork:老师的仓库
![Markdown](http://i4.buimg.com/576036/3dc15d7d29388fb3.png)

* 查看具体的代码差异
![Markdown](http://i4.buimg.com/576036/db311d3bcb3e0d80.png)

* 确认无误，创建pull request
![Markdown](http://i2.buimg.com/576036/7630bdb46c01487a.png)

* 填上一些信息后，就完成pull request了
![Markdown](http://i2.buimg.com/576036/7b0113a2dbc7d506.png)

## 参考文献
* [史上最浅显易懂的Git教程！](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/)
* [文科妹纸教你mac下使用git](https://www.zhihu.com/question/20070065)
* [git - 简明指南](http://rogerdudler.github.io/git-guide/index.zh.html)