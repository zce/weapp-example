# 微信小程序开发教程示例

> 一个微信小程序（应用号）开发示例（豆瓣电影）

[![Build Status](https://travis-ci.org/zce/weapp-demo.svg?branch=master)](https://travis-ci.org/zce/weapp-demo)
[![Dependency Status](https://david-dm.org/zce/weapp-demo.svg)](https://david-dm.org/zce/weapp-demo)
[![devDependency Status](https://david-dm.org/zce/weapp-demo/dev-status.svg)](https://david-dm.org/zce/weapp-demo#info=devDependencies)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com/)

## 关于豆瓣API限制第三方小程序调用问题说明

很多朋友最近都在反馈豆瓣接口 403 的问题，我抽空仔细排查了一遍，豆瓣官方应该是限制了第三方小程序对豆瓣接口的调用，对于这一行为我认为“无可厚非”，因为你没有为豆瓣的免费服务“买单”，请各位不要骂街。

为了帮助更多初学者或是爱好者，我个人准备了一个反向代理服务器（免费开放）。希望各位**珍惜资源切勿滥用**，谢谢！

接口地址：https://douban.uieee.com （支持 HTTP / HTTPS）

**接口限流：10000 次 / 1 小时**，由于是豆瓣官方的限流，所以所有使用我搭建的这个反向代理服务的朋友都是**共享这 10000 次请求**的，我也没办法再去提高这个数字（普通个人用户是 100 次 / 1 小时），所以还是希望大家不要滥用。

当然如果还是不幸超出额度的话，就只能等待下一个整点，不明白为什么的朋友，可以自己 Google 一下接口限流：API Rate Limit。

如果你可以的话，建议你自己参考我的配置文件配置一个自己的反向代理服务（这样就没人跟你抢了😀）

接口配置文件仓库：https://github.com/zce/douban-api-proxy (包括解决方法)

### 具体使用

- 将豆瓣的 API 地址更改为以上地址
- 修改微信小程序后台的白名单

## 文字教程

- https://github.com/zce/weapp-demo/tree/tutorial

## 相关演示

- [视频演示如何运行当前项目](http://files.wedn.net/videos/weapp/run-it.mp4)
- [豆瓣电影小程序真机测试](http://files.wedn.net/videos/weapp/weapp.mp4)

很多朋友给我发消息说希望可以真机体验一下，所以前段时间我抽空把这个小程序发布了，大家可以通过微信扫码体验：

![DoubanFilm](https://user-images.githubusercontent.com/6166576/36627844-fc2a74ce-1983-11e8-98b3-25efff7e1d2b.jpg)

源码我放在了：https://github.com/zce/weapp-douban

## 相关项目

- [zce/weapp-demo](https://github.com/zce/weapp-demo) - 包含开发工作流版本的豆瓣电影
- [zce/weapp-todos](https://github.com/zce/weapp-todos) - 一个简单的任务清单小程序
- [zce/weapp-locally](https://github.com/zce/weapp-locally) - 本地生活，本地吃喝玩乐
- [zce/weapp-beauty](https://github.com/zce/weapp-beauty) - 拍拍测颜值，AI
- ~~[zce/weapp-boilerplate](https://github.com/zce/weapp-boilerplate) - 一个小程序的快速开发骨架~~

## 有想法？

Welcome PR / Issue / WeChat！

### 交流群

微信群垃圾广告和无意义的分享链接太多，最近狠下心清理了~
改用 QQ 群，单独审核，禁止广告，我的目的很简单，就是留出一个干净的环境，让志同道合的一起玩，谢谢大家

![IT BETTER群二维码](https://user-images.githubusercontent.com/6166576/39342428-99c27a22-4a0a-11e8-8cc1-fa10f2dafe23.png)

### 我的微信

如果你不喜欢热闹，或者加不进去，可以告诉我（注意我不收红包！有问题直接留言就行，只求描述到我能看懂！我尽快回复）

![我的微信](qrcode1.png)

## 许可

[MIT](./LICENSE) &copy; [汪磊](http://github.com/zce)
