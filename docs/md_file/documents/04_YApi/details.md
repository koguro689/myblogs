标题
# Windwos10 搭建YApi
# 前言
  YApi是去哪儿网开源的一款接口管理工具。在工作中接口返回的参数值包含很多的异常场景，前端不得不写一大串的判断逻辑。配合前端调试需要模拟很多场景，比较费时费力，而且很多场景到了后期才可以调试，在提交测试的时候就会显得紧张。
  总结起来文档式的接口管理方式浪费时间，YApi这款工具的旨意将接口作为一个公共的可视化的方式打通前端、后台、测试环节，整合在一起，共同使用维护，降低接口的维护成本

# 环境准备
+ 操作系统：Windows10
+ 环境要求：
	+ NodeJS：v13.4.0
		注意1：需要安装在不含空格的文件目录下，否则会产生【MODUL NOT FOUND】异常
		注意2：不要使用最新版本的NodeJS，否者会产生【non-existen】异常
	+ MongoDB：v4.2.13
	
# 查看版本信息
## NodeJS的版本信息
```
node -v
```
![nodejs版本](.\images\image001.png)

## npm的版本信息
```
npm -v
```
![npm版本](.\images\image002.png)

## 启动MongoDB
![npm版本](.\images\image003.png)

# 安装YApi
```
npm install -g yapi-cli --registry https://registry.npm.taobao.org
```
![安装YApi](.\images\image004.png)

# 启动YApi
```
yapi server
```
![启动YApi服务](.\images\image005.png)
```
访问：http://localhost:9090/
```
![访问YApi平台部署](.\images\image006.png)

# 开始部署
输入公司名，其他的默认即可，执行【开始部署】
![开始部署](.\images\image007.png)

部署执行中（需要等待一段时间，知道部署成功）
![部署执行中](.\images\image008.png)

部署成功
![部署成功](.\images\image009.png)

CMD命令提示符窗口
![CMD命令提示符窗口](.\images\image010.png)

# 启动部署的服务
根据提示，在CMD命令提示符窗口中切换到部署目录下，执行启动命令
```
node vendors/server/app.js
```
![启动服务](.\images\image011.png)

在浏览器中输入访问地址
```
http://127.0.0.1:3000/
```
![访问页面](.\images\image012.png)

# 登录部署的管理平台
登录管理平台（用户名和密码在发布成功后，在CMD窗口中打印出来）
```
用户名：admin@admin.com
密码：ymfe.org
```
![登录管理平台](.\images\image013.png)

![管理平台页面](.\images\image014.png)