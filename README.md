# jrebel
1. chmod -R 777 JrebelBrainsLicenseServerforJava-1.0-SNAPSHOT-jar-with-dependencies.jar
2. java -jar JrebelBrainsLicenseServerforJava-1.0-SNAPSHOT-jar-with-dependencies.jar -p 18082 &
3. print INFO:
```
2018-07-31 13:51:54.835:INFO:oejs.Server:jetty-8.y.z-SNAPSHOT
2018-07-31 13:51:54.889:INFO:oejs.AbstractConnector:Started SelectChannelConnector@0.0.0.0:18082
License Server started at http://localhost:18082
JetBrains Activation address was: http://localhost:18082/
JRebel 7.1 and earlier version Activation address was: http://localhost:18082/{tokenname}, with any email.
JRebel 2018.1 and later version Activation address was: http://localhost:18082/{guid}(eg:http://localhost:18082/5eaf3650-844a-46d9-9362-8f23750f3f8b), with any email.
```
# 反向代理破解
1、下载破解工具
https://github.com/ilanyu/ReverseProxy/releases
在这个网址里，mac用户下载ReverseProxy_darwin_amd64，window用户下载相应的exe文件即可，因为window的操作比mac的相对简单，所以这里主要讲mac，window的除了打开该文件的方式不一样之外，接下来的其他操作都是一样的。

注意：mac用户用safair下载，不要用谷歌，因为谷歌下载之后会把文件后面的dms的后缀名给启动去掉，切记。

2、执行破解工具
window用户打开exe文件，在弹出的防火墙对话框中点击允许，如下图所示： 

mac用户打开终端，执行操作如下：
```
# 给该文件赋予可执行权限
chmod 777 '文件路径'
# 执行该文件，注意，前面的美元符号必须带
$bash '文件路径'
```

3、idea配置
打开idea的设置，然后在JRebel中选择输入Licence，选择第三项，输入： 
http://127.0.0.1:8888/xin，后面的xin可以随意乱填，第二行的邮箱只要填写格式正确的邮箱即可，填写完之后勾选同意协议，点击OK 
这里写图片描述

4、离线模式下使用
上面的3个步骤执行完之后，你会看到你的JRebel已经是激活好的了，状态和下图一样，但是这个时候只要你把终端刚开着的破解文件给关了，你就前功尽弃了，因为它的原来是通过那个破解文件进行一个反向代理的，这个时候，我们先不要急着关掉终端，点击JRebel的work offline，这个时候，你就可以离线使用JRebel了，你可以把终端关掉了，如第二张图所示，你可以看到你的JRebel的过期时间，一般是半年，半年过期后，你用本文的方式再执行一次就可以了。

这里写图片描述

这里写图片描述

