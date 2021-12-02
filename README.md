# Coolie

技术 angular，nestjs，mongoDB cloud, docker, linux 

## v1.0.0
目标：创建一个爬虫系统来自动爬取lv和爱马仕的网站，通过爬虫实现自动抢购到购物车，并通过后台来随机选择购买账号实现自动登陆，但在支付方面要通过人工进行输入支付信息和确认收货人
（这算是一个网购网站的bug，通过购物车能在没有登陆账号的情况下）

进程
1. 创建一个简单易操作的前台，通过登陆账号来实现对后台所有接口和所有数据库的操作(登陆界面，取消注册，通过手机验证或者邮箱验证，token可以持续用12小时)
2. 用户在前台输入多个账号信息（记录到数据库，是否加密需要思考)，后台记录好每个账户的账户信息，每次可以进行一键操作来登录所有的账户
3. 创建一个ip地址池，最好都是法国ip，从而做到让每个登陆的账号在不同的IP地址上发出command
4. 用户可以通过前台来选择登陆某个账号
5. 通过爬虫来监控几个特定（产品id）的产品，从而实现抢购到购物篮并卡在支付界面，然后会自动发给用户邮箱来确认支付(paypal）,支付成功后记录到数据库
6. 支付成功后，有邮箱提醒或者短息提醒用户
7. 用户通过去官网登陆账号来查看自己的产品来看购买记录
