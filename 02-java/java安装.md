## 1. jdk安装

### 1.1 jdk下载

官网地址：<https://www.oracle.com/>

![官网地址](..\images\orcle官网.png)



![](..\images\图片1.png)

建议安装1.8

![](..\images\图片2.png)



### 1.2 jdk安装

双击安装即可

### 1.3 配置环境变量

新建JAVA_HOME，在PATH变量最后面添加一条变量值

![](..\images\图片3.png)



![](..\images\图片4.png)

### 1.4 检查是否成功

通过【win+r】调出【运行】弹窗，输入“cmd”之后打开【命令提示符】。

输入<font color="red" size=4>**java -version**</font>，出现以下表示安装成功

![](..\images\图片5.png)

## 2. maven 安装

### 2.1 下载maven

官方网址：<https://maven.apache.org/download.cgi>

![](..\images\图片6.png)

### 2.2 安装maven

解压即安装

### 2.3 配置环境变量

![](..\images\图片7.png)



通过【win+r】调出【运行】弹窗，输入“cmd”之后打开【命令提示符】。

输入<font color="red" size=4>**mvn -v**</font>，出现以下信息表示配置成功

![](..\images\图片8.png)

### 2.4 配置仓库地址

在电脑建一个文件，命名为repository

![](..\images\图片9.png)



进入路径为../apache-maven-3.9.0/conf，然后打开settings.xml文件

找到 <localRepository>/path/to/local/repo</localRepository> 这个标签

复制一个到下面，写上我们上面创建的本地仓库路径，例如我的路径在这里：

```htm
<localRepository>C:/ruanjian/maven/repository</localRepository>
```

![](..\images\图片10.png)



接下来把默认的远程仓库换成阿里的仓库，找到<mirrors></mirrors>标签，在里面复制一个子标签到下面

```hxml
<mirror>  
     <id>alimaven</id>  
     <name>aliyun maven</name>  
     <url>http://maven.aliyun.com/nexus/content/groups/public/</url>  
     <mirrorOf>central</mirrorOf>        
</mirror>
```

![](..\images\图片11.png)





## 3. idea 安装

### 3.1 安装idea

![](..\images\图片12.png)

### 3.2 idea破解

把JetbrainsCrack-release-enc.jar放在idea的bin目录下，然后在bin目录下两个文件（idea.exe.vmoptions、idea64.exe.vmoptions）追加以下一句

```txt
-javaagent:C:\ruanjian\idea\IDEA2018.2.5\bin\JetbrainsCrack-release-enc.jar
```

打开idea，复制下面的代码到Activation code里面

```txt
ThisCrackLicenseId-{
“licenseId”:“ThisCrackLicenseId”,
“licenseeName”:“username”,
“assigneeName”:"",
“assigneeEmail”:“XXXX@163.com”,
“licenseRestriction”:“For This Crack, Only Test! Please support genuine!!!”,
“checkConcurrentUse”:false,
“products”:[
{“code”:“II”,“paidUpTo”:“2019-12-31”},
{“code”:“DM”,“paidUpTo”:“2019-12-31”},
{“code”:“AC”,“paidUpTo”:“2019-12-31”},
{“code”:“RS0”,“paidUpTo”:“2019-12-31”},
{“code”:“WS”,“paidUpTo”:“2019-12-31”},
{“code”:“DPN”,“paidUpTo”:“2019-12-31”},
{“code”:“RC”,“paidUpTo”:“2019-12-31”},
{“code”:“PS”,“paidUpTo”:“2019-12-31”},
{“code”:“DC”,“paidUpTo”:“2019-12-31”},
{“code”:“RM”,“paidUpTo”:“2019-12-31”},
{“code”:“CL”,“paidUpTo”:“2019-12-31”},
{“code”:“PC”,“paidUpTo”:“2019-12-31”}
],
“hash”:“2911276/0”,
“gracePeriodDays”:7,
“autoProlongated”:false}
```



### 3.3 idea配置jdk

![](..\images\图片14.png)

![](..\images\图片15.png)

![](..\images\图片16.png)

### 3.4 idea配置maven

![](..\images\图片17.png)



![](..\images\图片18.png)


