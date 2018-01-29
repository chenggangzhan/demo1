# 写在前面

由于最近公司业务不是很忙，空闲时间比较多，于是就在纠结Vue.js（之前就学习过）和Node.js先专研哪个比较好，最终选择了先玩玩Node.js。经过一段时间的学习，我决定两路开工。使用Node.js给前端写接口，配备后台管理功能，先把后台搭建好。大概几天过后，后台一些简单的功能实现后，就开始用Vue.js开始搭建前台，也一直在想做点什么比较好，于是就做了个豆瓣评分类似的项目。

> 前端项目地址 https://github.com/chenggangzhan/demo1  

## 技术栈(Vue2.js + Node.js 全栈项目)

> 由于页面不是很多，vuex用的不多，关键掌握怎么实现就好了

`vue2` + `vuex` + `vue-router` + `webpack` + `fetch` + `sass` + `flex` + `svg` + `阿里字体图标`

## 运行

```
git clone https://github.com/chenggangzhan/demo1.git

cd vue-video

npm install  建议使用淘宝镜像(https://npm.taobao.org/) =>  cnpm i

npm run dev (运行项目)

npm run build (打包项目)

ps: 如果打包之后文件运行不了，请打包之前把路由的 mode:'history'注释掉，该功能去掉了url中丑陋的 # 号

```
## 功能

* 1. 注册登录登出 + 验证码 密码检测，如果用户不存在则自动创建
* 2. 检测是否登录，如果没有登录则不允许评论和评价
* 3. 可以上传影片到后台，进行前台展示
* 4. 评分功能，初始化评分可以自由设置，如果没有人like则默认显示原始评分，如果有则计算当前vide的评分
* 5. 修改用户名，检测用户名是否跟其他人重复
* 6. 上传头像，默认没有头像
* 7. 评论功能，评论之后可以在个人中心展示，并且可以删除
* 8. 搜索功能，可以搜索存在的影片，如果没有则显示无结果
* 9. 自己喜欢的video和评论的内容会在个人中心显示

综上：

- [x] 注册
- [x] 登录
- [x] 登出
- [x] 验证码
- [x] 详情页
- [x] 分类
- [x] 分类影视列表
- [x] 修改用户名
- [x] 上传头像
- [x] 评论
- [x] 删除评论(可以左滑评论删除)
- [x] 搜索
- [x] 个人中心数据

如果觉得对你有帮助还望关注一下，有问题可以及时提哟，觉得不错的话`star`一下也是可以的哟

## 前端线上地址

项目是手机端的，请使用谷歌浏览器手机预览模式

> 首页默认一种类别只显示10个，可以查看更多显示全部 

## 前端演示

![](http://oswpupqu5.bkt.clouddn.com/vue1.gif)

### 主页

![](http://oswpupqu5.bkt.clouddn.com/home.png) ![](http://oswpupqu5.bkt.clouddn.com/search.png)

### 登录页

![](http://oswpupqu5.bkt.clouddn.com/login.png)

### 个人中心页

![](http://oswpupqu5.bkt.clouddn.com/personal.png) ![](http://oswpupqu5.bkt.clouddn.com/personal1.png)


### 详情页

![](http://oswpupqu5.bkt.clouddn.com/detail.png)


## 后台演示

![](http://oswpupqu5.bkt.clouddn.com/admin.gif)

## 有问题欢迎反馈

在使用中有任何问题，欢迎反馈给我，可以用以下联系方式跟我交流

* 邮件(624163614#qq.com, 把#换成@)
* QQ: 624163614


## 目录结构

```
|-- build                            // webpack配置文件
|-- config                           // 项目打包路径
|-- src                              // 源码目录
|   |-- assets                       // 图片文件
|   |-- base                   		 // 移动端适配
|   |-- components                   // 组件
|   |-- data                         // 接口
|   |-- router						 // 路由配置
|   |-- store                        // 状态管理
|   |-- style                        // 样式
|    	App.vue                      // 页面入口文件
|    	main.js                      // 程序入口文件
|-- static                           // 静态资源
|-- .babelrc                         // ES6语法编译配置
|-- .editorconfig                    // 代码编写规格
|-- .gitignore                       // git忽略的文件
|-- .postcssrc.js                    // post-loader的插件配置文件
|-- index.html                       // 入口html文件
|-- package.json                     // 项目及工具的依赖配置文件

```
