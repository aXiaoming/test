
# 教程
Well404教程：
https://zhuanlan.zhihu.com/p/373323656

官方文档
https://v2.nonebot.dev/docs/start/installation

https://github.com/nonebot/nonebot2


# 环境

python3.8.10+
安装：add to path
python --version

nb-cli脚手架：
官方文档
https://v2.nonebot.dev/docs/start/installation


go-cqhttp下载安装
https://github.com/Mrs4s/go-cqhttp/releases/tag/v1.0.0-rc1

![image](https://user-images.githubusercontent.com/84505329/167170389-81d43100-c567-49bb-8fc8-49735609e22a.png)



# 第一个机器人
双击运行exe会得到一个bat

双击bat，选择3，反向websoctet   
![image](https://user-images.githubusercontent.com/84505329/167170544-f9ac42dc-18fe-49c1-b4cb-bc23b0f63512.png)   


得到yml配置文件，修改qq账号、端口号   
![image](https://user-images.githubusercontent.com/84505329/167170999-ceb77122-9c7a-41ae-af53-3f965abac6d3.png)   

![image](https://user-images.githubusercontent.com/84505329/167171221-cea84166-197b-42be-a0bb-1098e0ff3a6f.png)   


修改完成保存后，再次执行bat文件   

换成对应的qq账号，扫码登陆，如果登录不上，可以删除session.token文件   
![image](https://user-images.githubusercontent.com/84505329/167171503-b2da6166-281c-4d2d-89d1-b0045ea6260f.png)   

之后运行go-cqhttp要使用bat执行，不要使用exe执行   



然后创建nb项目：
nb命令在环境变量中添加：
D:\Application\Anaconda3\envs\nonebot_env\Scripts

![image](https://user-images.githubusercontent.com/84505329/167171967-b2eaec24-6d5b-4cfe-aff8-8b602722aab7.png)   
   

项目创建完成后，修改配置文件
nb在环境的   

![image](https://user-images.githubusercontent.com/84505329/167172186-515872c5-3d08-4d82-97db-9c4abf1d417b.png)   
将刚才配置的端口号复制进去。

具体配置见下：

```xml
HOST=127.0.0.1  # 配置 NoneBot2 监听的 IP/主机名
PORT=10800  # 配置 NoneBot2 监听的端口
SUPERUSERS=["320976399", "987654321"]  # 配置 NoneBot 超级用户，配qq号就行
NICKNAME=["awesome", "bot"]  # 配置机器人的昵称
COMMAND_START=["/","rb"]  # 配置命令起始字符
# COMMAND_SEP=["."]  # 配置命令分割字符

# Custom Configs
CUSTOM_CONFIG1="config in env file"
CUSTOM_CONFIG2=  # 留空则从系统环境变量读取，如不存在则为空字符串
```

然后就可以启动了
先启动python程序，再启动go-cqhttp




# nonebot-plugin-gocqhttp插件

https://github.com/mnixry/nonebot-plugin-gocqhttp

nb create先创建项目。   

![image](https://user-images.githubusercontent.com/84505329/167173293-03055e3f-a63d-467e-bc99-4f4b9ed998cf.png)   

安装插件
pip命令

配置端口号

导入插件
![image](https://user-images.githubusercontent.com/84505329/167173991-728eb103-9d0d-460e-8e5c-76de612f8ad6.png)   

启动

然后就可以浏览器打开了
![image](https://user-images.githubusercontent.com/84505329/167174233-89fc8d02-d562-4189-b900-98a9de73aab1.png)   


## 关闭机器人：
先在web页面停止
然后ctrl + c停止服务



# 使用插件

进入官方文档的插件库中：
https://v2.nonebot.dev/store

进入后，可以使用pip安装，然后在启动文件中加载   

![image](https://user-images.githubusercontent.com/84505329/167175148-99525ae9-b1a3-4d61-8f50-61e41531e109.png)   


# 适配旧版插件
robot adapt cq-http   
![image](https://user-images.githubusercontent.com/84505329/167175790-7a2199c0-f116-4762-aa69-753e54bf6697.png)   

点击最后一个链接   
![image](https://user-images.githubusercontent.com/84505329/167175905-e4fb4a78-6ce8-40a9-9a44-ca355741e55e.png)   

把红线部分删掉，替换为
![image](https://user-images.githubusercontent.com/84505329/167842670-54997006-98b5-4d81-8c14-5670caf902ca.png)   



![image](https://user-images.githubusercontent.com/84505329/167176163-40f28722-a042-43a3-a65a-26b3e0e04367.png)   























