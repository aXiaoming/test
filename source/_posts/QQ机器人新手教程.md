
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
![image](https://user-images.githubusercontent.com/84505329/167171967-b2eaec24-6d5b-4cfe-aff8-8b602722aab7.png)

项目创建完成后，修改配置文件
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




















