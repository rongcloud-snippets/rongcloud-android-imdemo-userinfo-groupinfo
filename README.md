# rongcloud-android-imdemo-userinfo&groupinfo

rongcloud-android-imdemo-userinfo&groupinfo 是基于融云 IMKit SDK 的用户信息及群组信息功能，使用了融云最新的 4.0 SDK。


# 使用步骤

## 参数配置

开发者需配置项目中的变量 `Appkey` 和 `Token`，

[AppKey 获取地址](https://developer.rongcloud.cn/app/appkey/0vMK99Huzz-qw40Ybv4NDA)

[Token 获取地址](https://developer.rongcloud.cn/apitool/Mw8EsJmV43kZBugTMSAZXg)

## 前置条件

1. 为了配合 Demo 中的代码，需要执行下面步骤：
   * 使用 [Token 获取地址](https://developer.rongcloud.cn/apitool/Mw8EsJmV43kZBugTMSAZXg) 获取 Token，userId 需要使用 “tester1”，将该 Token 配置到 RCSConfig 中进行连接。
   * 使用 [开发者后台 - 服务管理 - API 调用 - 群组服务](https://developer.rongcloud.cn/apitool/aItWe5MFHcuygEQzblxxMg) 创建群组，groupId 需要使用 group1，群组成员的 userId 需要使用 tester1、tester2

2. 新用户默认是空的会话列表，是无法进入会话页面的。开发者可在 [开发者后台 - 服务管理 - API 调用 - 消息服务](https://developer.rongcloud.cn/apitool/kNUDHRczlPHkECa0SJ8X3Q)  中调用对应接口给当前用户 tester1 和群组 group1 发送消息。

   发送成功后，接收方的会话列表展示会话。

## 功能实现

Demo 中实现了用户信息代理、群组信息代理和设置当前登录者的用户信息，为了方便演示，代码中写死了对于用户 Id 和群组 Id 的判断，开发者需要根据对 Id 的判断，去向应用服务器请求对应的用户信息或群组信息。




# 更多

[融云官网](https://www.rongcloud.cn/)

[融云文档](https://docs.rongcloud.cn/v3/)
