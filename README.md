# UploadGithub

# 如何使用git将项目上传到GitHub

#### 1.首先需要一个github账号
>首先需要GitHub网址，如果还没有账号的话，可以先注册。  
>[https://github.com/](https://github.com/)

#### 2.需要下载git工具
>这里给出下载地址，下载后一路安装即可。  
>[https://git-for-windows.github.io/](https://git-for-windows.github.io/)  

![avatar](/imgs/1.png)  
![avatar](/imgs/2.png)

#### 3.进入github首页，点击New Repository新建一个项目
![avatar](/imgs/3.png)

#### 4.填写相应信息后，点击create即可
>Repository name: 仓库名称  
>Description(可选): 仓库描述介绍  
>Public, Private : 仓库权限（公开共享，私有或指定合作者）  
>Initialize this repository with a README: 添加一个README.md  
>gitignore: 不需要进行版本管理的仓库类型，对应生成文件.gitignore  
>license: 证书类型，对应生成文件LICENSE  

![avatar](/imgs/4.png)

#### 5.开始克隆
>点击Clone or dowload会出现一个地址，copy这个地址备用。 
 
![avatar](/imgs/5.png)

#### 6.本地操作
###### ①首先右键你的项目，如果你之前安装git成功的话，右键会出现两个新选项，分别为Git Gui Here,Git Bash Here,这里我们选择Git Bash Here，进入如下界面，UploadGithub即为我的项目名。
![avatar](/imgs/6.png)

###### ②接下来输入如下代码（关键步骤），把github上面的仓库克隆到本地  
>**git clone https://github.com/lixl163/UploadGithub.git**
>（https://github.com/lixl163/UploadGithub.git替换成你之前复制的地址）   

![avatar](/imgs/7.png) 

###### ③这个步骤以后你的本地项目文件夹下面就会多出个文件夹，该文件夹名即为你github上面的项目名，如图我多出了个Test文件夹，我们把本地项目文件夹下的所有文件（除了新多出的那个文件夹不用），其余都复制到那个新多出的文件夹下。  
![avatar](/imgs/8.png)   

###### ④接着继续输入命令 cd UploadGithub，进入Test文件夹  
![avatar](/imgs/9.png)   


###### ⑤接下来依次输入以下代码即可完成其他剩余操作：  
>git add .  （注：别忘记后面的.，此操作是把Test文件夹下面的文件都添加进来）  

>git commit  -m  "提交信息"  （注：“提交信息”里面换成你需要，如“first commit”）  

>git push -u origin master   （注：此操作目的是把本地仓库push到github上面，此步骤需要你输入帐号和密码）  
 
![avatar](/imgs/10.png)  

 
 
# ----------------------------我是分割线--------------------------

## 使用git命令新增和修改文件

>1.修改项目之后，查看项目状态，命令：git status。如下图：

![avatar](/imgs/git_status.png)  

从图中的标注可以看出，README.md  和 imgs/demo_print1.png 被修改了


>2.将修改的文件 提交到本地暂存区，命令：git add file，file 为修改文件名。如下图所示：

![avatar](/imgs/git_add.png)  

由图中的指令可以看出来，已将README.md添加到本地暂存区了，颜色从红色 变成了 绿色。


>3.剩下被修改的文件，也按照原来的方式，分别将文件提交到本地暂存区，命令：git add file，file 为修改文件名；再然后通过命令：git status 查询是否添加到暂存区成功。如下图所示：

![avatar](/imgs/git_add_status.png) 

注意：每次修改后的文件，都必须添加到本地暂存区后，才能更新到项目上

>4.提交当前工作空间的修改内容，命令：git commit -m "修改"，引号里面是提交信息，自己可以填写其他内容。如下图所示：

![avatar](/imgs/git_commit.png) 

>5.将项目更新到github或服务器，命令：git push。如下图：

![avatar](/imgs/git_push.png) 

项目上传成功。
